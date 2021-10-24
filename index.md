---
layout: default
title: ""
---
{% assign goodies = site.static_files | where: "goody", true %}
{% for file in goodies %}
  - [{{ file.name }}]({{ file.path }})
{% endfor %}
