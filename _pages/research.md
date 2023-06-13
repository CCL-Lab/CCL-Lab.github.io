---
# layout: archive
title: "Research"
permalink: /research/
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

<h2>Firm</h2>
{% for post in site.research reversed %}
  {% if post.type == "admin" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}

<h2>Admin Data</h2>
{% for post in site.research reversed %}
  {% if post.type == "firm" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}

<h2>Others</h2>
{% for post in site.research reversed %}
  {% if post.type == "others" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}
