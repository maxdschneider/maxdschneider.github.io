---
layout: page
title: Consulting
permalink: /consulting/
description: Short intro statement.
nav: true
nav_order: 5
display_categories: [work, fun]
horizontal: false
---

<div markdown="1">
I specialize in the following topics and am available for consulting or contract work:
- Statistical models: Bayesian techniques, (generalized) linear regression, time series models, spatiotemporal methods, cluster models and more
- Machine learning algorithms and high-compute simulation studies
- Model validation, including metric development and statistical testing
- Survey and experimental methods, including questionnaire design 
- Uncertainty quantification and forecasting 
- Data visualization and map design: graphical design best practices, developing maps, graphics and interactive platforms
- User-centered model communication: eliciting user needs, developing technical products around user needs, conducting usability testing
</div>


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
