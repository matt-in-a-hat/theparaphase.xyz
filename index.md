---
layout: default
title: theparaphase.xyz
---
## Files

{% assign goodies = site.static_files | where: "goody", true %}
{% for file in goodies %}
  - [{{ file.name }}]({{ file.path }}) (`{{ file.modified_time }}`)
{% endfor %}
