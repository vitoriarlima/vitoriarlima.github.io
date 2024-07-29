---
layout: default
title: "Portfolio"
permalink: /portfolio/
---

# Portfolio

## Finance Projects
{% for project in site.portfolio %}
{% if project.category == "finance" %}
- **[{{ project.title }}]({{ project.url }})**
  <br>
  {{ project.description }}
{% endif %}
{% endfor %}

## Deep Learning / AI Research Projects
{% for project in site.portfolio %}
{% if project.category == "ai" %}
- **[{{ project.title }}]({{ project.url }})**
  <br>
  {{ project.description }}
{% endif %}
{% endfor %}

## Data Science Projects
{% for project in site.portfolio %}
{% if project.category == "data-science" %}
- **[{{ project.title }}]({{ project.url }})**
  <br>
  {{ project.description }}
{% endif %}
{% endfor %}
