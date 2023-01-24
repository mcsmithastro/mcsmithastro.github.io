---
layout: page
permalink: /publications/
title: publications
description:
years: [2023,2022,2021,2020,2019,2018]
nav: true
---
<a href="https://ui.adsabs.harvard.edu/public-libraries/01Dbbf1dT4-gyB51ouj0ZA">ADS Library</a> and <a href="https://orcid.org/0000-0002-9849-877X">ORCID ID: 0000-0002-9849-877X</a>
<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
