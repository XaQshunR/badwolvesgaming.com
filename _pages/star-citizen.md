---
layout: splash
permalink: /star-citizen/
title: Star Citizen
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "assets/images/star-citizen/banner.jpg"
  actions:
    - label: "Apply Now"
      url: "https://robertsspaceindustries.com/orgs/BADWOLVES"
  caption: "Bad Wolves Syndicate"
excerpt: "Apply to join our fleet today!"
intro: 
  - excerpt: 'Bad Wolves Syndicate, a coalition committed to organized teamwork and strategic alliances. Guided by seasoned leadership, we excel in diverse operations—specialized conflicts to industry endeavors. Join us in redefining synergy and excellence. Unleash your potential with Bad Wolves Syndicate! We specialize in organizing, leading, and executing a varity of operations:'
specialties:
  - image_path: assets/images/star-citizen/scouting.jpg
    title: "Scouting"
    excerpt: "Conducting covert reconnaissance operations."
  - image_path: assets/images/star-citizen/infiltration.jpg
    title: "Infiltration"
    excerpt: "Coordination quick, targeted infantry and space combat operations."
  - image_path: assets/images/star-citizen/industry.jpg
    title: "Industry"
    excerpt: "We support various industrial efforts in frontier systems with our various outposts and facilities."
join_star_citizen:
  - image_path: assets/images/game-logos/sc.png
    title: "Not a Star Citizen?"
    excerpt: 'Use our recruitment code **STAR-MLS6-L3PL** to join the Star Citizen universe and start with an extra 5,000 UEC!'
    url: "https://robertsspaceindustries.com/enlist?referral=STAR-MLS6-L3PL"
    btn_label: "Enlist Today!"
    btn_class: "btn--primary"
fleetyards:
  - image_path: assets/images/star-citizen/fleetyards.png
    title: "Join our Fleet"
    excerpt: 'Join our fleet on FleetYards.net and help us build our fleet!'
    url: "https://fltyrd.net/fi/mHVrl4vKEA/"
    btn_label: "Apply Now"
    btn_class: "btn--primary"
---

{% include specialties id="intro" type="center" %}

{% include feature_row id="specialties" %}

{% include feature_row id="join_star_citizen" type="left" %}

{% include feature_row id="fleetyards" type="right" %}
