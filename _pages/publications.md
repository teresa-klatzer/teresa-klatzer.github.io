---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
years: [2018, 2017, 2016, 2015]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
