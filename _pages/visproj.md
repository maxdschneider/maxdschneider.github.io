---
layout: page
title: Visualization Work
permalink: /visproj/
description: 
nav: true
nav_order: 4
display_categories: [work, fun]
horizontal: false
---

<!-- pages/visproj.md -->
<div class="visproj">
{% if site.enable_visproj_categories and page.display_categories %}
  <!-- Display categorized visproj -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_visproj = site.visproj | where: "category", category %}
  {% assign sorted_visproj = categorized_visproj | sort: "importance" %}
  <!-- Generate cards for each visproj -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_visproj %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_visproj %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display visproj without categories -->

{% assign sorted_visproj = site.visproj | sort: "importance" %}

  <!-- Generate cards for each visproj -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_visproj %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_visproj %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
