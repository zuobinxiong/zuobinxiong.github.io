---
layout: page
permalink: /publications/
title: Publications
description: Selected publications. For full publication list, please refer to <a href='https://scholar.google.com/citations?user=a92n-HkAAAAJ'>Google Scholar</a>.

years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year" style="color: var(--global-theme-color)">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
