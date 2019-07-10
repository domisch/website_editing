+++
# Slider widget.
widget = "slider"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 50  # Order that this section will appear.
title = "Highlights slider"


# Slide interval.
# Use `false` to disable animation or enter a time in ms, e.g. `5000` (5s).
interval = 4500

# Slides.
# Duplicate an `[[item]]` block to add more slides.


[[item]]
  title = "Conservation planning"
  content = "Spatially explicit species distribution models improve the spatial prioritization"
  align = "center"

  overlay_color = "#555"  # An HTML color value.
  overlay_img = "headers/gurobi_delta.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.5  # Darken the image. Value in range 0-1.

 cta_label = "Read the paper here"
  cta_url = "https://onlinelibrary.wiley.com/doi/10.1111/ddi.12891"
  cta_icon_pack = "fas"




[[item]]
  title = "AI & Sustainable Development Goals"
  content = "The role of artificial intelligence in achieving the SDGs"
  align = "center"  # Choose `center`, `left`, or `right`.

  # Overlay a color or image (optional).
  #   Deactivate an option by commenting out the line, prefixing it with `#`.
  overlay_color = "#666"  # An HTML color value.
  overlay_img = "headers/AI_SDG_header.png"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.5  # Darken the image. Value in range 0-1.

  # Call to action button (optional).
  #   Activate the button by specifying a URL and button label below.
  #   Deactivate by commenting out parameters, prefixing lines with `#`.
  cta_label = "Read more on arXiv"
  cta_url = "https://arxiv.org/abs/1905.00501"
  cta_icon_pack = "fas"
  #cta_icon = "graduation-cap"



[[item]]
  title = "New dataset"
  content = "Geomorpho90m - New global 90m topographical variables"
  align = "center"

  overlay_color = "#333"  # An HTML color value.
  overlay_img = "headers/topo_90m.png"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.5  # Darken the image. Value in range 0-1.


  cta_label = "Browse the variables at LandGIS"
  cta_url = "https://landgis.opengeohub.org/#/?base=Stamen%20(OpenStreetMap)&center=47.1754,20.7857&zoom=4&opacity=80&layer=dtm_dev-scale_merit.dem_m"
  cta_icon_pack = "fas"
  #cta_icon = "graduation-cap"



[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["10px", "0", "10px", "0"]


+++

