---
layout: default
title: "Intro"
---

{% if site.show_excerpts %}
  {% include home.html %}
{% else %}
  {% include archive.html title="Plan" %}
{% endif %}
