---
title: "hydrographr: an R package for scalable hydrographic data processing"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors: 
  - M. Schürz
  - A. Grigoropoulou
  - J.R. Garcia Marquez
  - T. Tomiczek
  - M. Floury
  - C. Schürz
  - G. Amatulli
  - H.-P. Grossart
  - S. Domisch


# Author notes (optional)
author_notes:
   - 'Equal contribution'
   - 'Equal contribution'

date: '2023-11-01'
doi: '10.1111/2041-210X.14226'

# Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

# Publication name and optional abbreviated publication name.
publication: '_Methods in Ecology and Evolution_, 14, 2953-2963'
publication_short: '_Methods in Ecology and Evolution_, 14, 2953-2963'

abstract: __1.__ Freshwater ecosystems are considered biodiversity hotspots, but assessing the spatial distribution of species remains challenging. One major obstacle lies in the complex geospatial processing of large amounts of data, such as stream network, sub-catchment and basin data, that are necessary for addressing the longitudinal connectivity among water bodies. Workflows thus need to be scalable, especially when working across large spatial extents and at high spatial resolution. This in turn requires advanced command-line GIS skills and programming language integration, which often poses a challenge for freshwater researchers.    __2.__ To address this challenge, we developed the package \texttt{hydrographr} that provides scalable hydrographic data processing in R. The package contains functions for downloading data of the high-resolution Hydrography90m dataset, processing, reading and extracting information, as well as assessing network distances and connectivity. While the functions are, by default, tailored towards the Hydrography90m data, they can also be generalized towards other data and purposes, such as efficient cropping and merging of raster and vector data, point-raster extraction, raster reclassification, and data aggregation. The package depends on the open-source software GDAL/OGR, GRASS-GIS and the AWK programming language in the Linux environment, allowing a seamless language integration. Since the data is processed outside R, _hydrographr_ allows creating scalable geo-processing workflows.   __3.__ We illustrate the \texttt{hydrographr} functions using two workflows that focus on (i) a freshwater species distribution modelling approach, and (ii) assessing stream connectivity given the fragmentation by dams. We also provide a detailed guide for the initial installation of the required software. Windows users need to first enable the Windows Subsystem for Linux (WSL) feature, and can then follow the same software installation as Linux users. \texttt{hydrographr} is maintained on GitHub at [https://github.com/glowabio/hydrographr](https://github.com/glowabio/hydrographr).  __4.__ _hydrographr_ provides a set of key functions for processing freshwater geospatial data. We expect that the package will support the freshwater-related research communities given the easy-to-use wrapper functions that allow capitalizing on powerful open-source command-line software, which may otherwise require a steep learning curve. Users can thus perform large-scale freshwater-specific longitudinal connectivity and network analyses across large geographic extents while staying within the R environment.
# Summary. An optional shortened abstract.
# summary: We identify 15 pressing priority needs, grouped into five research areas, in an effort to support informed stewardship of freshwater biodiversity.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
- name: R-package
  url: https://github.com/glowabio/hydrographr
- name: Installation
  url: https://glowabio.github.io/hydrographr/articles/hydrographr.html
- name: SDM workflow
  url: https://glowabio.github.io/hydrographr/articles/case_study_cuba.html
- name: Connectivity workflow
  url: https://glowabio.github.io/hydrographr/articles/case_study_brazil.html

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  # focal_point: ''
  # preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
   - hydrographr
   - hydrography90

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example


---
