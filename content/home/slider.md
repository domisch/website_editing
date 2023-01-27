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
        icon_pack: fab
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
        icon_pack: fab
        text: Browse the data here
        url: 'https://geo.igb-berlin.de/maps/621/view'
    - title: hydrographr
      content: Scalable hydrographic data processing in R
      align: center
      background:
        position: center
        color: '#666'  # white is '#666'
        brightness: 0.5
        media: '/headers/hydrographr_code.png'
      link:
        icon: github
        icon_pack: fab
        text: Get the R-package
        url: 'https://github.com/glowabio/hydrographr'


---

