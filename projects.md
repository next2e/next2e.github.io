---
layout: main
---

# 2WebsitE - Projects

## Current

### All-Wing

<div class="row">
  {% for project in site.data.projects.current.allwing %}
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

### Individual Projects

<div class="row">
  {% for project in site.data.projects.current.individual %}
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

## Previous

### All-Wing

<div class="row">
  {% for project in site.data.projects.previous.allwing %}
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

### Individual Projects

<div class="row">
  {% for project in site.data.projects.previous.individual %}
  {% include project.html project=project %}
  <!-- if last column in row -->
  {% assign remainder = forloop.index | modulo:3 %}
  {% if remainder == 0 and forloop.last == false %}
</div>
<div class="row">
  {% endif %}
  {% endfor %}
</div>
