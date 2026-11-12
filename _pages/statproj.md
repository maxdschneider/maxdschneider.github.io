---
layout: page
title: Statistical Projects
permalink: /statproj/
description: 
nav: true
nav_order: 4
display_categories: [work, fun]
horizontal: false
---

<!-- pages/statproj.md -->
<div class="statproj">
{% if site.enable_statproj_categories and page.display_categories %}
  <!-- Display categorized statproj -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_statproj = site.statproj | where: "category", category %}
  {% assign sorted_statproj = categorized_statproj | sort: "importance" %}
  <!-- Generate cards for each statproj -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_statproj %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_statproj %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display statproj without categories -->

{% assign sorted_statproj = site.statproj | sort: "importance" %}

  <!-- Generate cards for each statproj -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_statproj %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_statproj %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
