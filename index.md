---
layout: default
title: Index
---
# Index des solutions
 
<ul>
{% for page in site.pages %}
  {% if page.path contains 'content/' %}
    <li><a href="{{ page.url | relative_url }}">{{ page.title | default: page.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>