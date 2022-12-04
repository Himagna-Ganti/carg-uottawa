---
layout: page
permalink: /publications/
title: publications
description: Please see <a href="http://www.cs.cmu.edu/~epxing/publications-2021.html">here</a> for publications.
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
