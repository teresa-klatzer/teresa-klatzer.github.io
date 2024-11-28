---
layout: page
permalink: /talks/
title: Talks
description: Selected talks and posters.
nav: true
nav_order: 3
years: [2024, 2023, 2022, 2021, 2018, 2017, 2016, 2015]
---


<div class="publications">
{%- for y in page.years %}
{% bibliography -f talks_posters.bib -q @*[year={{y}}]* %}
{% endfor %}
</div>

