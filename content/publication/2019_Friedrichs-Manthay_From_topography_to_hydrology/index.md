---
title: "From topography to hydrology - the modifiable area unit problem impacts freshwater species distribution models"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors: 
  - M. Friedrichs-Manthay
  - S.D. Langhans
  - T. Hein
  - F. Borgwardt
  - H. Kling
  - S.C. Jähnig
  - S. Domisch
  
# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2020-01-02'
doi: '10.1002/ece3.6110'

# Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

# Publication name and optional abbreviated publication name.
publication: '_Ecology and Evolution_, 10, 2956-2968, https://doi.org/10.1002/ece3.6110'
publication_short: '_Ecology and Evolution_, 10, 2956-2968'

abstract: Species distribution models (SDMs) are statistical tools to identify potentially suitable habitats for species. For SDMs in river ecosystems, species occurrences and predictor data are often aggregated across subcatchments that serve as modeling units. The level of aggregation (i.e., model resolution) influences the statistical relationships between species occurrences and environmental predictors—a phenomenon known as the modifiable area unit problem (MAUP), making model outputs directly contingent on the model resolution. Here, we test how model performance, predictor importance, and the spatial congruence of species predictions depend on the model resolution (i.e., average subcatchment size) of SDMs. We modeled the potential habitat suitability of 50 native fish species in the upper Danube catchment at 10 different model resolutions. Model resolutions were derived using a 90-m digital-elevation model by using the GRASS-GIS module r.watershed. Here, we decreased the average subcatchment size gradually from 632 to 2 km2. We then ran ensemble SDMs based on five algorithms using topographical, climatic, hydrological, and land-use predictors for each species and resolution. Model evaluation scores were consistently high, as sensitivity and True Skill Statistic values ranged from 86.1–93.2 and 0.61–0.73, respectively. The most contributing predictor changed from topography at coarse, to hydrology at fine resolutions. Climate predictors played an intermediate role for all resolutions, while land use was of little importance. Regarding the predicted habitat suitability, we identified a spatial filtering from coarse to intermediate resolutions. The predicted habitat suitability within a coarse resolution was not ported to all smaller, nested subcatchments, but only to a fraction that held the suitable environmental conditions. Across finer resolutions, the mapped predictions were spatially congruent without such filter effect. We show that freshwater SDM predictions can have consistently high evaluation scores while mapped predictions differ significantly and are highly contingent on the underlying subcatchment size. We encourage building freshwater SDMs across multiple catchment sizes, to assess model variability and uncertainties in model outcomes emerging from the MAUP.

# Summary. An optional shortened abstract.
# summary: We identify 15 pressing priority needs, grouped into five research areas, in an effort to support informed stewardship of freshwater biodiversity.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://onlinelibrary.wiley.com/doi/epdf/10.1002/ece3.6110'
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
  # - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example


---
