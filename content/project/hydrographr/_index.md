---
title: The hydrographr R-package
subtitle : "Scalable hydrographic data processing in R"
summary: Scalable hydrographic data processing in R
tags:
- Hydrography90m
- R-package
- Open-source

date: '2023-01-26T00:00:00Z'

# Optional external URL for project (replaces project detail page).
# external_link: 'https://github.com/glowabio/hydrographr'

image:
  caption: The hydrography R-package
  focal_point: Smart

links:
 - icon: github
   icon_pack: fab
   name: Get the R-package
   url: https://github.com/glowabio/hydrographr
#url_code: ''
#url_pdf: ''
#url_slides: ''
#url_video: ''


# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# authors:
#  - maria-ueblacker
#  - jaime-garcia-marquez
#  - admin

---

<!--- [!["hydrographr"](/hydrographr.png)](https://github.com/glowabio/hydrographr) -->

We have developed the _hydrographr_ R-Package that facilitates the download and data processing of the [Hydrography90m](https://hydrography.org/hydrography90m/hydrography90m_layers/) data (which can be visualized at the [IGB-GeoNode](https://geo.igb-berlin.de/maps/351/view)). The package is maintained at https://github.com/glowabio/hydrographr and the installation procedure is available [here](https://glowabio.github.io/hydrographr/articles/hydrographr.html). 

_hydrographr_ provides functions to allow scalable hydrographical data extraction and analysis workflows. The R-functions are wrappers around the open-source geospatial GDAL and GRASS-GIS software that run in the Linux environment and enable fast and memory-efficient data processing.

We will soon upload a vignette that showcases the functionality of _hydrographr_. In the meantime, feel free to explore the package and drop us a line [here](https://github.com/glowabio/hydrographr/issues) if you have any questions.

We thank [NFDI4Biodiversity](https://www.nfdi4biodiversity.org) and [NFDI4Earth](https://www.nfdi4earth.de/) for providing the funding that helped us getting the _hydrographr_ package together! 

!["NFDI"](/nfdi_logos.png)


