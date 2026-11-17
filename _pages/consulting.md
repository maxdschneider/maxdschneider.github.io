---
layout: page
title: Consulting
permalink: /consulting/
description: 
nav: true
nav_order: 5
display_categories: [work, fun]
horizontal: false
---

<div markdown="1">
I specialize in the following topics and am available for consulting or contract engagements. [Contact me](https://maxdschneider.github.io/contact/) to discuss your project and where I can offer support.

-	**Predictive Analytics & Statistical Modeling**: Regression modeling, Bayesian methods, time-series methods, geospatial and spatiotemporal modeling, clustering, and advanced statistical techniques.
-	**Machine Learning & Computational Methods**: Machine learning algorithms, large-scale simulations, and high-performance computational modeling.
-	**Model Performance & Validation**: Model evaluation, performance metric development, statistical testing, and validation frameworks.
-	**Research & Decision Intelligence**: Survey design, experimental design, questionnaire development, and decision, judgment and user experience research methods.
-	**Forecasting & Risk Analytics**: Uncertainty quantification, probabilistic forecasting, and risk assessment.
-	**Data Visualization & Business Intelligence**: Data storytelling, dashboard and interactive tool development, map design, and effective visual communication.
-	**User-Centered Product & Communication Strategy**: Stakeholder needs assessment, user-focused technical product development, usability testing, and translating user perspectives into actionable insights.

</div>

<div markdown="1">
Click on the images below to learn more about past consulting work.
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
