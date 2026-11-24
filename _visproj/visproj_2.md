---
layout: page
title: Improving hazard communication with evidence-based map design
description: 
img: assets/img/criteria-based-seismic-hazard-mapping.png
importance: 2
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

<div markdown="1">
Natural hazards like earthquakes, floods, and fires are communicated through maps, generally using a discrete set of colors. Which color palette should hazard maps use, and how many colors should they have? I surveyed the literature from data visualization, statistics, cartography and cognitive psychology to identify key criteria for selecting a color palette and classifying mapped data into a discrete number of colors. I applied these criteria to redesign the German national seismic hazard map, guided by key principles of seismic hazard that the map needed to communicate. I ran a controlled task-based user experiment, finding that the new map better communicated several of these principles better than the original. [Our widely-cited publication](https://nhess.copernicus.org/articles/23/2505/2023/) provides easy-to-implement criteria that help organizations make informed map design decisions, reduce ambiguity in hazard interpretation, and communicate risk more effectively to diverse audiences. These improvements support better-informed decisions in hazard planning, risk management and emergency preparedness.
</div>