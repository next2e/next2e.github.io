---
layout: main
permalink: photos.html
---

# 2WebsitE - Photo Gallery

## PHOTOS!!!

{% for image in site.static_files %}

{% if image.path contains 'img/gallery' %}

![{{ image.basename }}]({{ site.url }}{{ image.path }}){:.img-thumbnail}

{% endif %}

{% endfor %}
