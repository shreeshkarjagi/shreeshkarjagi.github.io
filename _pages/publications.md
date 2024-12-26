---
layout: page
permalink: /publications/
title: Publications
description: My research interests focuses on bioelectronics, neural interfaces, signal processing, machine learning, and digital health.
years: [2024, 2023]
nav: true
nav_order: 1
---

<div class="publications">
{% for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  {% bibliography -f papers -q "@*[year={{ y }}]*" %}
{% endfor %}
</div>
