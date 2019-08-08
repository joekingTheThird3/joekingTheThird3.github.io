---
title: Important stuff about Jekyll
tags: code jekyll important
---
Important stuff about the site generator Jekyll:

<br>

* * *
list of static files

{% raw %}
{% assign image_files = site.static_files %}
{% for myimage in image_files %}
  {{ myimage.path }}
{% endfor %}
{% endraw %}


{% assign image_files = site.static_files %}
{% for myimage in image_files %}
  {{ myimage.path }}
{% endfor %}

