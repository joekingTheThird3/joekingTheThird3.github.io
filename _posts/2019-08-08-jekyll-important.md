---
---
Important stuff about the site generator Jekyll:

<br>

* * *

{% assign image_files = site.static_files %}
{% for myimage in image_files %}
  {{ myimage.path }}
{% endfor %}

