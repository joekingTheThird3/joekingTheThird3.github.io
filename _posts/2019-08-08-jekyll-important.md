---
title: Important stuff about Jekyll I learned
tags: code jekyll important
---
Important stuff about the site generator Jekyll:

<br>

* * *

{% assign image_files = site.static_files %}
{% for myimage in image_files %}
  {{ myimage.path }}
{% endfor %}

