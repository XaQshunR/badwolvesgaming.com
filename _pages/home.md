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
  - image_path: assets/images/game-logos/pax-dei.png
    alt: "Pax Dei"
  - image_path: assets/images/game-logos/vtt-2.png
    alt: "Virtual Tabletop Games"
  - image_path: assets/images/game-logos/ascension-wow.png
    alt: "Ascension WoW"
  - image_path: assets/images/game-logos/ark.png
    alt: "Ark: Survival Evolved"
  - image_path: assets/images/game-logos/league-of-legends.png
    alt: "League of Legends"
  - image_path: assets/images/game-logos/eso.png
    alt: "Elder Scrolls Online"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="about" type="left" %}

{% include feature_row id="hosting" type="right" %}

### Some games we play
<div class="gallery games">
  {% for img in page.games %}
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
  <!-- <figcaption markdown="1">
  **Some** of the games we like to play.
  </figcaption> -->
</div>
<!-- ### Some of the games we like to play. -->

<!-- {% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include documents-collection.html collection=games sort_by=page.sort_by sort_order=page.sort_order type=grid %}
</div> -->
