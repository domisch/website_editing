---
title: Conservation planning across Colombia
subtitle: "Priority areas for the freshwater fish fauna"
summary: Priority areas for the freshwater fish fauna
tags:
- Freshwater biodiversity
- Conservation planning
- Geo-informatics
- Open-source GIS



date: '2022-06-03T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Estimated proteced areas across Colombia (Tomiczek et al., unpublished)
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
  - thomas-tomiczek
  - jaime-garcia-marquez
  - admin


---

__>> [Click here for the visualization](https://geo.igb-berlin.de/maps/290/view) <<__

Colombia forms one of the global freshwater biodiversity hotspots, home to 1494 freshwater fish species. This exceptional fish fauna has, however, rarely been considered when selecting areas for biodiversity conservation. This study integrates freshwater fish distributions into a spatial prioritization exercise to assess to which extent (i) freshwater biodiversity, using fish as a proxy, is currently represented within the existing protected areas, and (ii) if alternative protected area networks may have the potential to increase the number of fish species under protection.

At first all available fish data was collated, resulting in a data base of over 112,535 geographic occurrences of 1224 freshwater fishes across Colombia with harmonized nomenclature and revised geo-referenced coordinates.

Based on a digital elevation model at 1 km<sup>2</sup> resolution, the stream network was delineated with a minimum catchment size of 90 km<sup>2</sup> and extracted the corresponding 33,612 sub-catchments that served as spatial units within the analyses. In the next step fish occurrence data and environmental variables (climate, topography, land cover, hydrology) were aggregated across the sub-catchments and an ensemble of species distribution modelling algorithms was employed to project suitable habitat of each fish species across the study area.

Following the principles of systematic conservation planning, integer linear programming was applied to delineate a hypothetical protected area network that fulfills minimum, predefined conservation targets for each fish species, i.e. maximizing species representativeness and connectivity among river catchments, while minimizing the cost of anthropogenic impact, represented by the human footprint index and required area for protection. This spatial prioritization was carried out for four different conservation targets, set to protect 20 %, 30 %, 40 % and 50 % of each fish species suitable habitats in the priority network.

The projected suitable habitats of freshwater fish show high species richness in the Amazon and Orinoco basins while endemic and threatened fish mainly are projected for the Magdalena-Cauca and Pacific-Choco region.

<br/>

_Stacking the individual fish predictions gives an estimate of species richness (low: purple, high:yellow), where red points represent the fish sampling occurences:_

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe src="https://geo.igb-berlin.de/maps/290/embed" min-width : 900px ; style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border:0;" title="Fish richness" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>

<br/>

The calculated total area of the hypothetical priority area network is between 279,077 km<sup>2</sup> and 754,400 km<sup>2</sup> for the different conservation targets. It represents 12.1 % – 32.6 % of the study area, needed for the conservation of 20 % - 50 % of 1224 Colombian freshwater fish species. Most sub-catchments are prioritized in the Amazon and Orinoco basins and the least in the Caribbean basins. The priority network extents into the neighboring countries of Colombia, signifying the need of transboundary cooperation in freshwater conservation. Between 9.2 % to 28.2 % of Colombia’s protected areas coincide with the projected priority area network. A sensitivity analysis, locking in the existing protected areas in the spatial prioritization solution, reveals a priority area network 16.3 % to 34.7 % larger than that of the minimum cost priority network. It indicates that the existing protected areas inadequately represent freshwater fish in Colombia.

Conservation efforts are best focused on the Magdalena-Cauca and Pacific-Choco basins for the expansion of protected areas, since the majority of endemic and threatened fish species occurs within those basins. This thesis represents a first important step in the integration of freshwater biodiversity for spatial area prioritization and can serve as a baseline scenario for future conservation planning exercises in Colombia.

<br/>

_Potential protected areas for this region are represented in red, here for a target of 20% of the suitable habitat of each 1224 freshwater fish in Colombia, accounting for the lowest human footprint index and sub-catchment size:_

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <iframe src="https://geo.igb-berlin.de/maps/294/embed" min-width : 900px ; style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border:0;" title="Protected areas" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>




