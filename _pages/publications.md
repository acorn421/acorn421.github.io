---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<style>
  /* Section headings (Conference Papers / Journal Articles / Preprints):
     left-aligned and bright so they stand out on the dark background */
  .publications h2.bibliography {
    text-align: left;
    color: var(--global-text-color);
  }

  /* CV-style numbering: C1.., J1.., P1.. matching the CV.
     In the CV the oldest paper is #1, so the labels count DOWN from the top
     (newest first). counter-reset is set to (count + 1) per section. */
  .pub-conf ol.bibliography {
    counter-reset: pub 6; /* number of conference papers + 1 */
  }
  .pub-jour ol.bibliography {
    counter-reset: pub 4; /* number of journal articles + 1 */
  }
  .pub-pre ol.bibliography {
    counter-reset: pub 2; /* number of preprints + 1 */
  }
  .publications ol.bibliography > li {
    counter-increment: pub -1;
  }
  .pub-conf ol.bibliography > li .title::before {
    content: "[C" counter(pub) "] ";
    font-weight: bolder;
    margin-right: 0.2rem;
  }
  .pub-jour ol.bibliography > li .title::before {
    content: "[J" counter(pub) "] ";
    font-weight: bolder;
    margin-right: 0.2rem;
  }
  .pub-pre ol.bibliography > li .title::before {
    content: "[P" counter(pub) "] ";
    font-weight: bolder;
    margin-right: 0.2rem;
  }
</style>

<div class="publications">

<div class="pub-conf">
<h2 class="bibliography">Conference Papers</h2>
{% bibliography --query @inproceedings --group_by none %}
</div>

<div class="pub-jour">
<h2 class="bibliography">Journal Articles</h2>
{% bibliography --query @article --group_by none %}
</div>

<div class="pub-pre">
<h2 class="bibliography">Preprints</h2>
{% bibliography --query @misc --group_by none %}
</div>

</div>
