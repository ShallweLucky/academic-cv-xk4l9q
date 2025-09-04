---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
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
        url: uploads/Wei Xumin_CV.pdf
    design:
      css_class: dark
      # Avatar customization
      avatar:
        size: medium  # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I have a solid background across physics, materials, and coding, and more importantly, I am highly hands-on: I participated in the development of the Shenzhen Large-scale Scientific Facility Platform, independently built complex optical setups, published an Applied Physics Letters(Nature Index) paper as first author.

        Shenzhen Large-scale Scientific Facility Platform provides access to High Performance Computing cluster, as well as a wide range of advanced imported characterization instruments(keysight PNA Network Analyzer N5227B, Keithley 4200A-SCS Parameter Analyzer, Probe Station...).😃
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


