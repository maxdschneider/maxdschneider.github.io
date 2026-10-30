---
layout: page
title: statworks
permalink: /statworks/
description: A growing collection of your cool statworks.
nav: true
nav_order: 4
display_categories: [work, fun]
horizontal: false
---

<!-- pages/statworks.md -->
<div class="statworks">
{% if site.enable_statworks_categories and page.display_categories %}
  <!-- Display categorized statworks -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_statworks = site.statworks | where: "category", category %}
  {% assign sorted_statworks = categorized_statworks | sort: "importance" %}
  <!-- Generate cards for each statworks -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_statworks %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_statworks %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display statworks without categories -->

{% assign sorted_statworks = site.statworks | sort: "importance" %}

  <!-- Generate cards for each statworks -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_statworks %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_statworks %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
