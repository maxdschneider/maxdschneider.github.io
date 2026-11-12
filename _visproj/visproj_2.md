---
layout: page
title: Methods for choosing color palettes for natural hazard maps
description: 
img: assets/img/criteria-based-seismic-hazard-mapping.png
importance: 2
category: work
permalink: /visproj/color-palettes-natural-hazard-maps/
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
    {% include figure.liquid loading="eager" path="assets/img/criteria-based-seismic-hazard-mapping.png" title="German seismic hazard map, redesigned using criteria for colors and classification scheme" class="img-fluid rounded z-depth-1" %}
  </div>

Natural hazards like earthquakes, floods, and fires are communicated through maps, generally using a discrete set of colors. Which color palette should hazard maps use, and how many colors should they have? I surveyed the literature from data visualization, statistics, cartography and cognitive psychology to identify key criteria for selecting a color palette and classifying the data being mapped into a discrete number of colors. I worked with a research team to applied these criteria to redesign the German national seismic hazard map, guided by key principles of seismic hazard that the map needed to communicate. We user-tested the redesigned map against the original map, finding that the new map better communicated several key principles of seismic hazard in Germany. This work provides easy-to-implement criteria for hazard mappers to make difficult design choices that determine how risk is communicated; the resulting publication has been widely cited across the natural hazards.
