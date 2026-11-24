---
layout: page
title: Forecasting rare events even with complex and patchy data
description: 
img: assets/img/Bayesian-aftershock-parameter-estimates-PNW.png
importance: 2
permalink: /statproj/bayesian-models-pnw/
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
      grid-template-columns: minmax(0, 8fr) minmax(0, 4fr);
    }
  }
</style>

<div class="statwork-layout">
  <div>
    {% include figure.liquid loading="eager" path="assets/img/PNW-seismicity-map-tectonics.png" title="Seismicity map for PNW splits by tectonic regime" class="img-fluid rounded z-depth-1" %}
     {% include figure.liquid loading="eager" path="assets/img/Bayesian-aftershock-parameter-estimates-PNW.png" title="Bayesian posterior estimates for three aftershock parameters for different tectonic regimes in the PNW" class="img-fluid rounded z-depth-1" %}
  </div>

The Pacific Northwest (PNW) has multiple tectonic environments and but also a limited record of earthquakes detected by country-specific seismic networks, which makes it hard for best-practice statistical models to forecast future earthquakes. In my PhD work, I [compiled multiple earthquake datasets for the international PNW](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/94/5/2500/624503/Earthquake-Catalog-Processing-and-Swarm) and characterized them by their underlying tectonic regimes. I developed [a Bayesian approach to estimate parameters](https://pubs.geoscienceworld.org/ssa/tsr/article/4/4/259/649311/What-Do-We-Know-Without-the-Catalog-Eliciting) in a space-time point process model (the first of its kind for the PNW) that handles complex, data-limited environments better than traditional parameter estimation techniques. Applying it, I showed how key parameters, such as aftershock productivity and temporal decay rates, [differ across tectonic regimes, regions and earthquake clustering processes](https://pubs.geoscienceworld.org/ssa/bssa/article-abstract/115/5/2219/654484/Bayesian-ETAS-Modeling-for-the-Pacific-Northwest). This allows for more accurate and stable earthquake forecasts than current practice (e.g., in the U.S. Geological Survey’s aftershock forecasting system), giving forecast providers new statistical tools for reliable forecasts precisely where observational data are scarce.
