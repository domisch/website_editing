---
date: "2019-07-01T00:00:00+02:00"
draft: false
linktitle: Freshwater variables
menu:
  data_code:
    parent: Data & Code
    weight: 1
title: Freshwater-specific environmental variables
toc: false
type: docs
---

This tutorial shows you how to calculate stream-specific freshwater variables by relating the upstream e.g. land cover to any given downstream location using the GRASS GIS add-ons _r.stream.watersheds_ & _r.stream.variables_. The original 1km data and publication are available [here](http://www.earthenv.org/streams) - see also the original code from [spatial-ecology.net](http://spatial-ecology.net/dokuwiki/doku.php?id=wiki:grassrivarvariable).

[<img align="center" src="/img/Add-ons_for_GRASS_GIS.gif" width="700" alt="Add-on animation">](http://www.earthenv.org/streams)




__This example contains the following steps:__

- Download an exemplary digital elevation model (DEM)
- Extract the stream network from the DEM
- Delineate major drainage basins
- Crop data to a sub-basin
- Calculate the sub-watersheds for each stream grid cell (_r.stream.watersheds_)
- Calculate contiguous stream-specific variables (_r.stream.variables_)

{{% alert note %}}
The add-ons have been tested in the Linux environment. Microsoft Windows users: consider installing the OSGEO-Live Virtual machine that has GRASS GIS 7 already installed and is ready to use. Alternatively you can run the add-ons via QGIS.
{{% /alert %}}


<br/>

Create and enter the folder where the data will be stored:

```
export INDIR=$HOME/grass_hydro
mkdir $INDIR 
cd $INDIR
```

Download the script

```
cd ~
wget "http://www.spatial-ecology.net/ost4sem/exercise/basic_adv_grass/stream_variables.sh"
rstudio stream_variables.sh &
```

<br/>


Download and unzip a DEM from [WorldClim](http://www.worldclim.org/tiles.php):

```
wget -O  $INDIR/alt_16_tif.zip  "http://biogeo.ucdavis.edu/data/climate/worldclim/1_4/tiles/cur/alt_16_tif.zip"
unzip  -o $INDIR/alt_16_tif.zip  -d  $INDIR/dem
gdalinfo $INDIR/dem/alt_16.tif        # check data
```

If needed, first install the latest GRASS GIS version:

```
sudo add-apt-repository ppa:ubuntugis/ubuntugis-unstable
sudo add-apt-repository ppa:grass/grass-devel
sudo apt-get update
sudo apt-get install grass grass-gui grass-dev subversion gdal-bin libgdal-grass libalgorithms1 libbase1 libgdal-dev
```

Create the GRASS GIS data base and enter GRASS:

```
grass78  -text -c $INDIR/dem/alt_16.tif  $INDIR/grass_location
```

Read data into GRASS:

```
r.in.gdal input=$INDIR/dem/alt_16.tif    output=elevation
r.info elevation # check data
```

Open GUI and visualize the layers:
```
g.gui wxpython
```

Run hydrological conditioning:
```
g.extension  extension=r.hydrodem # download extension
# if you get an error run: sudo apt install grass-dev subversion
r.hydrodem  input=elevation  output=elevation_cond
```

Extract drainage direction and stream network
```
r.watershed  --h  # see help regarding the options and flags
r.watershed  elevation=elevation_cond  drainage=drainage   stream=stream  accumulation=accumulation  threshold=100  --o
```

Get drainage basins (last downstream segment: -l flag)
```
g.extension  extension=r.stream.basins
r.stream.basins  direction=drainage  stream_rast=stream  basins=basins_last  -l  --o
```

Categorize the single basins:
```
r.clump -d input=basins_last  output=basins_cat  --o
```

Extract the data for one basin:
```
r.mapcalc "drainage_sub = if (basins_cat==798, drainage, null() ) "  --o
r.mapcalc "stream_sub = if (basins_cat==798, stream, null() ) "  --o
```

Write files to disk:
```
r.out.gdal  input=drainage_sub   output=$INDIR/drainage_sub.tif  type=Int32  nodata=-9999  --o  -c    createopt="COMPRESS=LZW,ZLEVEL=9"
r.out.gdal  input=stream_sub     output=$INDIR/stream_sub.tif    type=Int32  nodata=-9999  --o  -c    createopt="COMPRESS=LZW,ZLEVEL=9"
```



__Create stream-specific variables, and limit the calculation only to a single basin.__

Download and install the GRASS add-ons. Work-around (December 2019) for grass78:
```
mkdir $HOME/.grass7/addons/scripts
wget -O $HOME/.grass7/addons/scripts/r.stream.watersheds "https://raw.githubusercontent.com/domisch/grass-addons/master/r.stream.watersheds"
chmod 777  $HOME/.grass7/addons/scripts/r.stream.watersheds

wget -O $HOME/.grass7/addons/scripts/r.stream.variables "https://raw.githubusercontent.com/domisch/grass-addons/master/r.stream.variables"
chmod 777  $HOME/.grass7/addons/scripts/r.stream.variables
```

Add-on 1: Calculate the sub-watershed and sub-stream sections for each stream grid cell using 2 processors:

```
r.stream.watersheds stream=stream_sub  drainage=drainage_sub  cpu=2
```

Add-on 2: Create stream-specific variables based on elevation
```
r.stream.variables  variable=elevation  output=cells,min,max,range,mean,stddev,coeff_var,sum  area=watershed  scale=1  cpu=2
```

Rename the “elevation_cells” to “flow_accumulation” and check variables:
```
r.mapcalc "flow_accummulation = elevation_cells"  --o
r.info  flow_accummulation
r.info  elevation_range
```

Get stream length (similar procedure as above):
```
r.stream.variables  variable=elevation  output=cells  area=stream  scale=1  cpu=2
r.mapcalc "stream_length = elevation_cells"  --o
r.info  stream_length 
```

Calculate the amount of rainfall within the basin:
```
wget -O  $INDIR/prec_16_tif.zip  "http://biogeo.ucdavis.edu/data/climate/worldclim/1_4/tiles/cur/prec_16_tif.zip"
unzip -q  -o $INDIR/prec_16_tif.zip  -d  $INDIR/prec
r.in.gdal input=$INDIR/prec/prec6_16.tif   output=prec6   # rainfall in June
r.stream.variables  variable=prec6  output=sum  area=watershed  scale=1  cpu=2
```

Run all 12 months in a loop:
```
for var in $(seq 1 12); do
r.in.gdal input=$INDIR/prec/prec${var}_16.tif   output=prec$var
r.stream.variables  variable=prec$var  output=sum  area=watershed  scale=1  cpu=2
done
```

Other useful add-ons for hydrological applications: http://grasswiki.osgeo.org/wiki/Hydrological_Sciences

__Other examples__

Get the stream order:
```
r.stream.order  stream_rast=stream   direction=drainage   strahler=str_order  --o
```

Get only streams and basins >=3rd order
```
r.mapcalc "str_order_3rd = if(str_order >=3, str_order, null() ) "  --o
r.stream.basins  direction=drainage  stream_rast=str_order_3rd  basins=basins_3rd_last   -l  --o
```

Stream distance - Calculates distance to and elevation above streams and outlet
```
g.extension extension=r.stream.distance
r.stream.distance   stream_rast=stream   direction=drainage   elevation=elevation_cond  method=downstream   distance=str_distance    difference=str_elevation_diff  --o
```

Stream order statistics - Calculates Horton's statistics for Strahler and Horton ordered networks created with r.stream.order Print only order statistics:
```
g.extension extension=r.stream.stats
r.stream.stats  stream_rast=stream   direction=drainage   elevation=elevation_cond  output=str_stats_o.txt    --o   
more $INDIR/str_stats_o.txt
```

Print only catchment statistics:
```
r.stream.stats  stream_rast=stream   direction=drainage   elevation=elevation_cond  output=str_stats_c.txt    -c 
more $INDIR/str_stats_c.txt
```

<br/>
_See also these useful GRASS-GIS commands for hydrological applications:_

https://grass.osgeo.org/grass78/manuals/topic_hydrology.html
https://grasswiki.osgeo.org/wiki/R.stream.*_modules <br/>
https://grasswiki.osgeo.org/wiki/Hydrological_Sciences 

