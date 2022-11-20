---
layout: page
permalink: /publications/
title: publications
description: Find the full list in our <a href="https://scholar.google.ca/citations?hl=en&user=1HJ-KYMAAAAJ&view_op=list_works&sortby=pubdate" target="_blank"><u>Google Scholar profile</u></a>.
years: [1999, 2000, 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022]
nav: true
nav_order: 5
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
