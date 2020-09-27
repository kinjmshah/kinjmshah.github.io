---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: true
---
{% include base_path %}

[Haptic](/_portfolio/hapticVel.md)

{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}


