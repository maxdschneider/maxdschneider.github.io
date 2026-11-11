---
layout: page
title: Building Bayesian earthquake rate models for the Pacific Northwest
description: 
img: assets/img/criteria-based-seismic-hazard-mapping.png
importance: 2
category: work
permalink: /statworks/bayesian-models-pnw/
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
    {% include figure.liquid loading="eager" path="assets/img/criteria-based-seismic-hazard-mapping.png" title="Statwork image" class="img-fluid rounded z-depth-1" %}
  </div>

The Pacific Northwest (PNW) has multiple tectonic environments and regional differences that affect its earthquake activity. It also has a limited set of earthquakes recorded by country-specific seismic networks, which further complicate the ability of best-practice statistical models to forecast future earthquakes. My PhD dissertation compiled multiple earthquake datasets for the international PNW, associating them with the PNW’s tectonic regimes. I then developed a Bayesian approach to estimate parameters in a space-time point process model, showing that this better handles the complex and low-data PNW than traditional parameter estimation techniques. I applied this to study how key parameters, such as aftershock productivity and temporal decay rates, differ between different tectonic regimes, regions and earthquake clustering processes within the PNW. These results indicate major improvements in accuracy and stability of earthquake forecasts when using our novel approaches over the current practices in, e.g., the US Geological Survey’s aftershock forecasting system. 
