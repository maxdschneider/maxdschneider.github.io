---
layout: page
title: Consulting
permalink: /consulting/
description: Short intro statement.
nav: true
nav_order: 4
display_categories: [work, fun]
horizontal: false
---

<!-- pages/consulting.md -->
<div class="consulting">
{% if site.enable_consulting_categories and page.display_categories %}
  <!-- Display categorized consulting -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_consulting = site.consulting | where: "category", category %}
  {% assign sorted_consulting = categorized_consulting | sort: "importance" %}
  <!-- Generate cards for each consulting -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_consulting %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_consulting %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display consulting without categories -->

{% assign sorted_consulting = site.consulting | sort: "importance" %}

  <!-- Generate cards for each consulting -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for statwork in sorted_consulting %}
      {% include statworks_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for statwork in sorted_consulting %}
      {% include statworks.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
