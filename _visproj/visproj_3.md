---
layout: page
title: Visualizing uncertainty for better decisions during crisis situations
description: 
img: assets/img/uncertainty-visualizations-aftershock-forecast-maps.png
importance: 3
permalink: /visproj/uncertainty-visualizations-aftershock-forecasts
---

<style>
  .statwork-layout {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    align-items: start;
  }

  @media (min-width: 768px) {
    .statwork-layout {
      grid-template-columns: minmax(0, 7fr) minmax(0, 5fr);
    }
  }
</style>

<div class="statwork-layout">
  <div>
    {% include figure.liquid loading="eager" path="assets/img/uncertainty-visualizations-aftershock-forecast-maps.png" title="Uncertainty visualizations tested for aftershock forecast maps" class="img-fluid rounded z-depth-1" %}
  </div>

All probabilistic forecasts come with uncertainty but depicting this on hazard forecast maps for non-technical audiences is challenging and often omitted entirely. I designed uncertainty visualizations for aftershock forecast maps using three approaches from data visualization and statistics best practices. I tested these visualizations for aftershock forecast maps in a large-sample online experiment, where participants used these forecast maps to perform judgment and decision tasks. While all approaches helped users find where there were likely to be few or many aftershocks (as forecasted), only one approach supported users to identify potential surprises: areas where forecasts show low aftershock activity but uncertainty leaves open the possibility of significantly more events. [These findings provide practical guidance](https://nhess.copernicus.org/articles/22/1499/2022/) for improving how forecast providers communicate uncertainty, helping decision-makers better anticipate unexpected outcomes and make more uncertainty-aware decisions during earthquake response and crisis management.