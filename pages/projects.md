---
layout: list
collection: "projects"
title: Projects
description: "A selection of our work and projects."
permalink: "/projects/"
header_transparent: true

hero:
  enabled: true
  heading: "Projects"
  sub_heading: "Our portfolio of work and projects."
  text_color: "#FFFFFF"
  background_color: false
  background_gradient: true
  background_image: "/assets/images/gen/home/home-2-large.webp"
  background_image_blend_mode: overlay # "overlay", "multiply", "screen"
  fullscreen_mobile: false
  fullscreen_desktop: false
  height: "500px"
  buttons:
    enabled: false
    list:
      - text: "Contact Us"
        url: "/contact"
        external: false
        fa_icon: false
        size: large
        outline: true
        style: "light"

grid:
  collection: "projects"
  sort_by: "weight" # "date", "weight"
  columns: 2
  prevent_click: false

intro:
  enabled: false
  align: left
  image: false
  heading: "We are a full service digital agency"
  sub_heading: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut eget sapien in elit semper accumsan. Pellentesque accumsan ut tortor eu varius. Sed id tincidunt massa, ut egestas orci."
  features:
    enabled: true
    list:
      - text: "Some of our projects are open source"
        fa_icon: false
  buttons:
    enabled: true
    list:
      - text: "View Github"
        url: "https://github.com/zerostaticthemes"
        external: true
        fa_icon: "fab fa-github"
        size: "large"
        outline: false
        style: "primary"

outro:
  enabled: true
  align: left
  image: false
  heading: "Ready to get started?"
  sub_heading: "Contact us today for a free quote!"
  buttons:
    enabled: true
    list:
      - text: "Get A Quote"
        url: "/contact"
        external: false
        fa_icon: false
        size: "normal"
        outline: false
        style: "primary"
---
