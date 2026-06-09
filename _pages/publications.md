---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<style>
  /* Venue category legend */
  .pub-legend {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin: 1.5rem 0 0.5rem;
    font-size: 0.9rem;
  }
  .pub-legend .legend-item {
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
  }
  .pub-legend .legend-swatch {
    display: inline-block;
    width: 1.6rem;
    height: 1rem;
    border-radius: 0.2rem;
  }

  /* CV-style numbering: restart per section (Conference / Journal / Preprint) */
  .publications ol.bibliography {
    counter-reset: pub-counter;
  }
  .publications ol.bibliography > li {
    counter-increment: pub-counter;
  }
  .publications ol.bibliography > li .title::before {
    content: "[" counter(pub-counter) "] ";
    font-weight: bolder;
    margin-right: 0.15rem;
  }
</style>

<div class="pub-legend">
  <span class="legend-item"><span class="legend-swatch" style="background-color:#aa1d22"></span> Security</span>
  <span class="legend-item"><span class="legend-swatch" style="background-color:#21568b"></span> AI / ML</span>
  <span class="legend-item"><span class="legend-swatch" style="background-color:#6c757d"></span> Neutral (Journal / Preprint)</span>
</div>

<div class="publications">

<h2 class="bibliography">Conference Papers</h2>
{% bibliography --query @inproceedings --group_by none %}

<h2 class="bibliography">Journal Articles</h2>
{% bibliography --query @article --group_by none %}

<h2 class="bibliography">Preprints</h2>
{% bibliography --query @misc --group_by none %}

</div>
