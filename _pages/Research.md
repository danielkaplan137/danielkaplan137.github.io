---
layout: archive
title: "Research"
permalink: /Research/
author_profile: true
---

{% include base_path %}

My work is focused on the interesting world of electrons interacting in solids. I blend in tools from ab-initio approaches to condensed matter (like Density Functional Theory) to model electron dynamics in real systems.

I am particularly interested in the response of electrons to electromagnetic fields and particularly the emerging universe of nonlinear responses in materials. 

{% for post in site.research %}
  {% include archive-single.html %}
{% endfor %}
