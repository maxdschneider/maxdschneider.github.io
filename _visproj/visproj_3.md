---
layout: page
title: Disentangling wind or water damages from hurricanes using time series models
description: 
img: assets/img/Schneider-AGU-Logo.jpg
importance: 3
category: work
permalink: /visproj/proj-url/
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
    {% include figure.liquid loading="eager" path="assets/img/Schneider-AGU-Logo.jpg" title="Statwork image" class="img-fluid rounded z-depth-1" %}
  </div>

The US COASTAL Act of 2012 mandated ascribing building damages from hurricanes as caused by either wind or water, for which the required hydrodynamic modelling of hurricanes must be at a high level of accuracy. While interning at the National Oceanic and Atmospheric Administration, I analyzed the predictive performance of this geophysical modelling system. I built time series models of prediction errors on wind- and water-related observations for Hurricane Irma (2017). Quantifying the autoregressive and other temporal structure in model errors helped inform priorities for model development that can further reduce error. I further consulted a multi-agency science team behind the US COASTAL Act in propagating errors across their complex coupled hurricane models. 
