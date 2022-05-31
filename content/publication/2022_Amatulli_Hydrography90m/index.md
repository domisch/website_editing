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
doi: '10.5194/essd-2022-9'

# Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

# Publication name and optional abbreviated publication name.
publication: '_EEarth System Science Data_, preprint, https://doi.org/10.5194/essd-2022-9'
publication_short: '_Earth System Science Data_, preprint'

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

url_pdf: 'https://doi.org/10.5194/essd-2022-9'
url_code: ''
url_dataset: 'https://public.igb-berlin.de/index.php/s/agciopgzXjWswF4'
url_poster: ''
url_project: 'https://geo.igb-berlin.de/maps/new?layer=geonode:hydrography90m_v1_stream_order_strahler_cog&view=True'
url_slides: ''
url_source: ''
url_video: 'https://av.tib.eu/media/56343'
url_map: ''

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

