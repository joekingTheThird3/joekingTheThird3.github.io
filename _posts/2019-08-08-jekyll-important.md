---
title: Important stuff about Jekyll
tags: code jekyll important
---
Important stuff about the site generator Jekyll:

<br>

* * *

0.
1. Jekyll uses the Liquid templating language
output content using two curly braces e.g. {%raw%}{{ variable }} {%endraw%}<br>
and perform logic statements by surrounding them in a curly brace percentage sign <br>
e.g. {%raw%}{% if statement %}{%endraw%}. 

2. <https://jekyllrb.com/docs/variables/>
<br>
All the variables set via the command line and your _config.yml are available through the site variable
3.{{site|inspect}}


* * *
list of static files - not processed by Jekyll

{% raw %}
{% assign image_files = site.static_files %}<br>
{% for myimage in image_files %}<Br>
  {{ myimage.path }}<br>
{% endfor %}<br>
{% endraw %}


{% assign image_files = site.static_files %}
{% for myimage in image_files %}
  {{ myimage.path }}
{% endfor %}

