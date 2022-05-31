---
title: "Hydrography90m: A new high-resolution global hydrographic dataset"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors: 
  - G. Amatulli
  - J.R. Garcia Marquez
  - T. Sethi
  - J. Kiesel
  - A. Grigoropoulou
  - M. Üblacker
  - L. Shen
  - S. Domisch
# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2022-06-01'
doi: '10.1016/j.ecolmodel.2013.02.019'

# Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

# Publication name and optional abbreviated publication name.
publication: '_Ecological Modelling_, 257, 1-10, https://doi.org/10.1016/j.ecolmodel.2013.02.019'
publication_short: '_Ecological Modelling_, 257, 1-10'

abstract: The geographic distribution of streams and rivers drives a multitude of patterns and processes in hydrology, geomorphology, geography and ecology. Therefore, a hydrographic network that accurately delineatesboth small streams and large rivers with equal precision, along with their topographic and topological properties, would be indispensable in the earth sciences. However, no such hydrographic study has been publishedto date. Perhaps equally critical is the absence of small headwater streams in global hydrographies, as theseare estimated to contribute to more than 70 % of overall stream length. We aimed to fill this gap by using theMERIT Hydro Digital Elevation Model at 3 arc-sec (ca. 90 m at the equator) to derive a globally seamless, standardised hydrographic network, the 'Hydrography90m', with corresponding stream topographic and topologicalinformation. A central feature of the network is the minimal upstream contributing area, i.e. flow accumulation,of 0.05 km2 (or 5 ha) to initiate a stream channel, which allowed us to extract headwater stream channels ingreat detail. By employing a suite of GRASS GIS hydrological modules, we calculated the range-wide upstreamflow accumulation and flow direction to delineate a total of 1.6 million drainage basins, and extracted globallya total of 726 million unique stream segments with their corresponding sub-catchments. In addition, we computed stream topographic variables comprising stream slope, gradient, length, and curvature attributes, as wellas stream topological variables to allow for network routing and various stream order classifications. We validated the spatial accuracy and flow accumulation of Hydrography90m against NHDPlus HR, an independent,national high-resolution hydrographic network dataset of the United States. Our validation shows that the newlydeveloped Hydrography90m has the highest spatial precision, and contains more headwater stream channelscompared to three other global hydrographic datasets. This inclusive approach provides a vital, and long-overdue baseline for assessing actual streamflow in headwaters, and opens new research avenues for high-resolution studies of surface water worldwide. Hydrography90m thus offers significant potential to facilitate the assessment offreshwater quantity and quality, inundation risk, biodiversity and conservation, as well as resource managementobjectives in a globally comprehensive and standardised manner. We provide all the computed layers for visualisation and download in 20° × 20° tiles at https://public.igb-berlin.de/index.php/s/agciopgzXjWswF4. While the entire dataset can be used directly in standard GIS applications, we recommend its seamless integration with hydrological modules in open-source QGIS and GRASS GIS software to further customise the data and derive optimal utility from it.

# Summary. An optional shortened abstract.
# summary: We identify 15 pressing priority needs, grouped into five research areas, in an effort to support informed stewardship of freshwater biodiversity.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://doi.org/10.1016/j.ecolmodel.2013.02.019'
url_code: ''
url_dataset: 'https://public.igb-berlin.de/index.php/s/agciopgzXjWswF4'
url_poster: ''
url_project: ''
url_slides: ''
url_source: 'https://geo.igb-berlin.de/maps/new?layer=geonode:hydrography90m_v1_stream_order_strahler_cog&view=True'
url_video: 'https://av.tib.eu/media/56343'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#  focal_point: ''
#  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  # - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example

---




+++
title = "Choice of study area and predictors affect habitat suitability projections, but not the performance of species distribution models of stream biota"
date = "2013-05-01"
authors = ["__Domisch, S.__", "Kuemmerlen, M.", "J&auml;hnig, S.C.", "Haase, P."]
publication_types = ["2"]
publication = "Ecological Modelling, (257), _pp. 1-10_, https://doi.org/10.1016/j.ecolmodel.2013.02.019"
publication_short = "_Ecological Modelling_ (257), 1-10"
abstract = "Species distribution models (SDMs) that provide extrapolations of species habitat suitability are increasingly being used in stream ecosystems, however the effects of different modelling techniques on model projections remain unknown. We tested how different study areas and predictors affect SDMs by using consensus projections of a fixed set of 224 stream macroinvertebrate species and five algorithms implemented in BIOMOD/R. Four modelling designs were applied: (1) a landscape as a continuous study area without any discrimination between terrestrial and aquatic realms, (2) a stream network masked a posteriori from the previous design, (3) a stream network as the study area during the model-building stage, and (4) same as (3) but with a hydrologically corrected set of predictors. The true skill statistic (TSS) and accuracy of the consensus projections were not influenced by the different designs (TSS ranged from 0.80 to 1.00, accuracy ranged from 0.70 to 0.96). The projections of design (4) yielded a strong reduction in false positive predictions compared to (1) (on average by 56%), (2) (11%) or (3) (8%). Our results show how SDMs with equally high accuracy may differ widely in habitat suitability projections for benthic macroinvertebrates. As model performance and output are not necessarily congruent, habitat suitability projections of stream biota need to be carefully assessed."
abstract_short = ""
image_preview = ""
selected = false
projects = []
tags = []
url_pdf = "https://www.sciencedirect.com/science/article/pii/S0304380013001063/pdfft?md5=e9e7894559f2480a255631c942f651c7&pid=1-s2.0-S0304380013001063-main.pdf"
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""
math = true
highlight = true
[header]
image = ""
caption = ""
+++
