---
layout: page
permalink: /publications/
title: Publications
description: Publications in reversed chronological order. 
years: [2022,2021,2019,2018,2017,2016,2015,2014,2013,2012,2010]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>