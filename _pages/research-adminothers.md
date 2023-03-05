---
title: "Research (Admin Data/Others)"
permalink: /research-adminothers/
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
  {% if post.type == "others" %}
    {% include archive-single-research.html %}
  {% endif %}
{% endfor %}

<!-- 
Education
======
* B.S. in GitHub, GitHub University, 2012
* M.S. in Jekyll, GitHub University, 2014
* Ph.D in Version Control Theory, GitHub University, 2018 (expected)

Work experience
======
* Summer 2015: Research Assistant
  * Github University
  * Duties included: Tagging issues
  * Supervisor: Professor Git

* Fall 2015: Research Assistant
  * Github University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub
  
Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams -->
