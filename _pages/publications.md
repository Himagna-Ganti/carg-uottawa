---
layout: page
permalink: /publications/
title: publications
description: PhD Student and RA/TA, <a href="https://www2.uottawa.ca/en" target="_blank">University of Ottawa</a>
years: [2022, 2021, 2020, 2019]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
