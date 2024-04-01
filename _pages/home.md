---
layout: splash
#hidden: true
permalink: /
excerpt: >
  18+ Online Acorn Fan Club
header:
  #overlay_color: "#f21368"
  overlay_filter: "0.25"
  overlay_image: /assets/images/banner.png
  #show_overlay_excerpt: true
  actions:
    - label: Help Gather Nuts
      url: "/join/"
intro:
  - excerpt: >
      A global, unapologetically diverse 18+ community, fostering camaraderie across various games. Nuts delivered daily.
about:
  - excerpt: >
      Learn more about the pack and our history.
    url: "/about/"
    btn_label: "Learn More"
    btn_class: "btn--primary"
    title: About
    image_path: assets/images/about.png
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

<!-- {% include gallery id="games" layout="third" %} -->

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include documents-collection.html collection=games sort_by=page.sort_by sort_order=page.sort_order type=grid %}
</div>

{:games: style="text-align: center;" height="50px"}
[![Star Citizen](/assets/images/game-logos/sc.png "Star Citizen"){: width="200px"}](/star-citizen/)
![Minecraft](/assets/images/game-logos/minecraft.png "Minecraft"){:width="200px"}
![Elder Scrolls Online](/assets/images/game-logos/eso.png "Elder Scrolls Online"){:width="200px"}
![Ark](/assets/images/game-logos/ark.png "Ark"){:width="200px"}
![Stellaris](/assets/images/game-logos/stellaris.png "Stellaris"){:width="200px"}
<br/>
{:games}

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

{% include paginator.html %}
