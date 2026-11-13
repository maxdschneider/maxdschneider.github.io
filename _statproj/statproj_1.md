---
layout: page
title: Validating probabilistic aftershock forecasts while incorporating user needs
description: 
img: assets/img/usgs-aftershock-forecast-testing.png
importance: 1
permalink: /statproj/testing-usgs-aftershock-forecasts/
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
      grid-template-columns: minmax(0, 6fr) minmax(0, 6fr);
    }
  }
</style>

<div class="statwork-layout">
  <div>
    {% include figure.liquid loading="eager" path="assets/img/usgs-aftershock-forecast-testing.png" title="Statwork image" class="img-fluid rounded z-depth-1" %}
  </div>

  <div style="min-width: 0;">
    <p>
The U.S. Geological Survey forecasts aftershocks after large earthquakes using probabilistic statistical models. This system expands on cutting-edge statistical models, using additional methods to account for known issues with aftershock data and model parameters. I am leading a multidisciplinary team to assess the forecast performance of these forecast methods. I developed new approaches to testing probabilistic forecasts, detailing what would matter most to diverse user groups of the USGS operational forecasts (e.g., emergency managers vs. geoscientists) whose forecast priorities may conflict (e.g., focusing on underpredictions vs. model misspecifications). This work has quantified time-varying tradeoffs between forecast accuracy and precision, for instance when using generic forecasting parameter values rather than those calibrated to the ongoing aftershock sequence. Our findings will improve the USGS forecasting system by disentangling how statistical methods drive forecast performance, and better managing these impacts for different user groups.
    </p>
  </div>
</div>

