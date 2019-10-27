---
layout: main
---

# 2WebsitE - Projects

## All-Wing

<div class="row">
  {% for project in site.data.projects.allwing %}
  {% include project.html project=project %}
  <!-- if last column in row -->
  {% assign remainder = forloop.index | modulo:3 %}
  {% if remainder == 0 and forloop.last == false %}
</div>
<div class="row">
  {% endif %}
  {% endfor %}
</div>

---

## Individual Projects

<div class="row">
  {% for project in site.data.projects.individual %}
  {% include project.html project=project %}
  <!-- if last column in row -->
  {% assign remainder = forloop.index | modulo:3 %}
  {% if remainder == 0 and forloop.last == false %}
</div>
<div class="row">
  {% endif %}
  {% endfor %}
</div>