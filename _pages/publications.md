---
layout: page
permalink: /publications/
title: All Publications
description: 
years: [ 2024, 2023, 2022, 2021, 2020, preprint]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papersall -q @*[year={{y}}]* %}
{% endfor %}

</div>
