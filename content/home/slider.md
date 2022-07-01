---
widget: slider  # Use the Slider widget as this page section
weight: 50  # Position of this section on the page
active: true  # Publish this section?
headless: true  # This file represents a page section.

design:
  # Slide height is automatic unless you force a specific height (e.g. '400px')
  slide_height: ''
  is_fullscreen: true
  # Automatically transition through slides?
  loop: true
  # Duration of transition between slides (in ms)
  interval: 5000

content:
  slides:
    - title: New hydrographic network
      content: Hydrography90m - A new high-resolution global hydrographic dataset
      align: center
      background: 
        position: center
        color: '#666'  # white is '#666'    #000  #000000
        brightness: 0.5
        media: '/headers/hydrograpyh90m.png'
      link:
        icon:
        icon_pack: fas
        text: Browse the data here
        url: 'https://geo.igb-berlin.de/maps/351/view'
    - title: The new EPTO database
      content: Global aquatic insect occurences
      align: center
      background: 
        position: center
        color: '#666'  # white is '#666'
        brightness: 0.5
        media: '/headers/EPTO_database.png'
      link:
        icon:
        icon_pack: fas
        text: Browse the data here
        url: 'https://geo.igb-berlin.de/maps/609/view'
    - title: New topographical data
      content: Geomorpho90m - New global 90m topographical variables
      align: center
      background:
        position: center
        color: '#666'  # white is '#666'
        brightness: 0.5
        media: '/headers/topo_90m.png'
      link:
        icon: 
        icon_pack: fas
        text: Browse the variables at OpenLandMap
        url: 'https://www.openlandmap.org/#/?base=Stamen%20(OpenStreetMap)&center=26.8842,38.4204&zoom=3.294688713147893&opacity=40&layer=dtm_roughness_merit.dem_m'


---

