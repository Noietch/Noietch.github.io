---
layout: page
permalink: /projects/
title: Projects
description:
years: [2026, 2025, 2022]
nav: false
---
<!-- _pages/projects.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
