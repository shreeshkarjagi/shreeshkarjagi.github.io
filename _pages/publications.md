---
layout: page
permalink: /publications/
title: Publications
description: My research interests focuses on bioelectronics, neural interfaces, signal processing, machine learning and digital health.
years: [2024, 2023]   # which years to display
nav: true
nav_order: 1
---

<!-- This page lists publications by year in descending order. -->

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  <!-- Use the Jekyll Scholar tag to display references from 'papers.bib' for that year -->
  {% bibliography -f papers -q "@*[year={{ y }}]*" %}
{% endfor %}

</div>
