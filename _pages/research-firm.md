---
# layout: archive
title: "Research (firm)"
permalink: /research-firm/
author_profile: true
redirect_from:
  - /resume
header: 
  caption: 
  cta_url:
  image: image
  overlay_color: #RRGGBB
  overlay_image: banner_2.jpg
---

{% include base_path %}

{% for post in site.research reversed %}
  {% if post.type == "admin" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}

{% for post in site.research reversed %}
  {% if post.type == "firm" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}

{% for post in site.research reversed %}
  {% if post.type == "others" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}
