---
layout: splash
#hidden: true
permalink: /
excerpt: >
  18+ Online Community
header:
  #overlay_color: "#f21368"
  overlay_filter: "0.25"
  overlay_image: /assets/images/banner.png
  #show_overlay_excerpt: true
  actions:
    - label: Join The Pack
      url: "/join/"
intro:
  - excerpt: >
      A global, unapologetically diverse 18+ community, fostering camaraderie across various games. Rabies delivered daily.
about:
  - excerpt: >
      Learn more about the pack and our history.
    url: "/about/"
    btn_label: "Learn More"
    btn_class: "btn--primary"
    title: About
    image_path: assets/images/about.png
hosting:
  - excerpt: >
      A dedicated game server hosting platform available for free to pack members.
    url: "/hosting/"
    btn_label: "Check it Out"
    btn_class: "btn--primary"
    title: Bad Wolves Hosting
    image_path: assets/images/hosting/logo_325x650.png
games:
  - url: /star-citizen/
    image_path: assets/images/game-logos/sc.png
    alt: "Star Citizen"
  - image_path: assets/images/game-logos/minecraft.png
    alt: "Minecraft"
  - image_path: assets/images/game-logos/eso.png
    alt: "Elder Scrolls Online"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="about" type="left" %}

{% include feature_row id="hosting" type="right" %}

{% include gallery id="games" layout="third" %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include documents-collection.html collection=games sort_by=page.sort_by sort_order=page.sort_order type=grid %}
</div>
