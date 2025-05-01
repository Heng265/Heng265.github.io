---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-04-29
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: background.jpg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        I am a researcher in Marine Technology, specializing in fluid-structure interaction (FSI), wind-assisted ship propulsion (WASP), and aeroelasticity of wingsails. My research bridges computational fluid dynamics (CFD), structural mechanics, and experimental methods to develop and evaluate innovative propulsion solutions for greener shipping.

        My work focuses on the design and analysis of crescent-shaped wingsails, where I combine high-fidelity CFD (URANS, LES, IDDES) and finite element methods in a two-way coupled framework to understand their aerodynamic performance and structural response. I also engage in offshore renewable energy research, particularly the performance assessment of floating wind farms and shared mooring systems.

        I am passionate about advancing sustainable maritime technologies through interdisciplinary research that integrates simulation, design, and real-world application. I welcome collaborations in wind propulsion, FSI, and marine renewables. Let’s connect! 🌊🚢
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
        featured_only: true  
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
