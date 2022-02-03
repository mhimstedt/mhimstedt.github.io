---
layout: page
permalink: /publications/
title: Publications
description: Publications in reversed chronological order. 
years: [2010 2011 2012 2013 2014 2015 2016 2017 2018 2019 2020 2021 2022]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
