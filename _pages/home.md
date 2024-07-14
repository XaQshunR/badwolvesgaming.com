---
layout: splash
permalink: /
title: Bad Wolves Gaming
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
      Learn more about the pack, what games we play, and our history.
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
games_gallery:
  - image_path: assets/images/game-logos/sc.png
    alt: "Star Citizen"
  - image_path: assets/images/game-logos/pax-dei.png
    alt: "Pax Dei"
  - image_path: assets/images/game-logos/minecraft.png
    alt: "Minecraft"
  - image_path: assets/images/game-logos/eso.png
    alt: "Elder Scrolls Online"
games:
  - title: >
      Explore the games we play.
    url: "/about/#games-we-play"
    btn_label: "View Games"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="about" type="left" %}

{% include feature_row id="hosting" type="right" %}

<div class="gallery games">
  {% for img in page.games_gallery %}
    <figure>
      {% if img.url %}
        <a href="{{ img.url | relative_url }}"
          {% if img.title %}title="{{ img.title }}"{% endif %}>
            <img src="{{ img.image_path | relative_url }}"
                alt="{% if img.alt %}{{ img.alt }}{% endif %}">
        </a>
      {% else %}
        <img src="{{ img.image_path | relative_url }}"
            alt="{% if img.alt %}{{ img.alt }}{% endif %}">
      {% endif %}
    </figure>
  {% endfor %}
</div>

{% include feature_row id="games" type="center" %}
