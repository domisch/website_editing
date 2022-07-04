---
title: Hydrography90m
summary: Delineating a high-resolution global stream network
tags:
- Geo-informatics
- Hydrography90m
- Open-source GIS
- Discharge

date: '2022-05-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Hydrography90m (&copy; Amatulli et al. 2022)
  focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

authors:
  - giuseppe-amatulli
  - longzhu-shen
  - jens-kiesel
  - jaime-garcia-marquez
  - afroditi-grigoropoulou
  - maria-ueblacker
  - admin




---


The **Hydography90m** dataset

__>> [Click here for the visualization](https://geo.igb-berlin.de/maps/351/view/) <<__

We used the MERIT Hydro Digital Elevation Model at 3 arc-sec (∼90 m at the equator) to derive a globally seamless, standardised hydrographic network, the "Hydrography90m", with corresponding stream topographic and topologicalinformation. A central feature of the network is the minimal upstream contributing area, i.e. flow accumulation,of 0.05 km2 (or 5 ha) to initiate a stream channel, which allowed us to extract headwater stream channels ingreat detail. By employing a suite of GRASS GIS hydrological modules, we calculated the range-wide upstreamflow accumulation and flow direction to delineate a total of 1.6 million drainage basins, and extracted globallya total of 726 million unique stream segments with their corresponding sub-catchments. In addition, we computed stream topographic variables comprising stream slope, gradient, length, and curvature attributes, as wellas stream topological variables to allow for network routing and various stream order classifications. We validated the spatial accuracy and flow accumulation of Hydrography90m against NHDPlus HR, an independent,national high-resolution hydrographic network dataset of the United States. Our validation shows that the newly developed Hydrography90m has the highest spatial precision, and contains more headwater stream channels compared to three other global hydrographic datasets. This inclusive approach provides a vital, and long-overdue baseline for assessing actual streamflow in headwaters, and opens new research avenues for high-resolution studies of surface water worldwide. Hydrography90m thus offers significant potential to facilitate the assessment offreshwater quantity and quality, inundation risk, biodiversity and conservation, as well as resource managementobjectives in a globally comprehensive and standardised manner. We provide all the computed layers for visualisation and download in 20° × 20° tiles.

Check out the paper in  [_Earth System Science Data_](https://essd.copernicus.org/preprints/essd-2022-9/). The data can be downloaded [here](https://hydrography.org/hydrography90m/hydrography90m_layers/) and visualized [here](https://geo.igb-berlin.de/maps/351/view/). 

-----

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe src="https://geo.igb-berlin.de/maps/351/embed" min-width : 900px ; style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border:0;" title="Hydrography90m" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>


