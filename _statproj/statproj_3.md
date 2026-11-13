---
layout: page
title: Machine learning for spatial classification of agricultural abandonment
description: 
img: assets/img/agr-abandonment-field-size-spatial-effect.png
importance: 3
permalink: /statproj/spatial-machine-learning-agricultural-abandonment/
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
    {% include figure.liquid loading="eager" path="assets/img/agr-abandonment-field-size-spatial-effect.png" title="Spatial Effect of Field Size in Predicting Agricultural Abandonment" class="img-fluid rounded z-depth-1" %}
  </div>

Agricultural land-use change is shaped by complex spatial relationships that are difficult to capture with conventional statistical approaches, particularly at the fine spatial resolutions needed for regional decision-making. I developed [the first predictive models of agricultural abandonment across the entire European continent](https://www.sciencedirect.com/science/article/abs/pii/S0048969718324021), using spatial machine learning to classify where active farmland is most likely to transition to fallow land. I derived a mathematically optimal framework for the boosted regression algorithm, focusing on the base learner, loss function, and early stopping criteria to avoid overfitting. Applying this framework to satellite image-derived data, I estimated spatial effects of factors such as field size (left) on predicted agricultural abandonment, among other predictive biophysical, socioeconomic and policy-related variables. Quantifying these non-linear dynamics supports more targeted, region-specific agricultural and land-management policies, which I presented in academic seminars as well as to agricultural organizations and farmers. 
