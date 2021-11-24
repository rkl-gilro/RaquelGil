---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2020]
years_conf: [2020, 2019, 2017, 2016]
nav: true
---

## Journals ##

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers_journals -q @*[year={{y}}]* %}
{% endfor %}

</div>



## Conferences ##

<div class="publications">

{% for y in page.years_conf %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
