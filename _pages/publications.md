---
layout: page
permalink: /publications/
title: Publications
order: 3
description: Publications by year.
years: [2024, 2023, 2022, 2021]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">
For the most up-to-date list, please refer to my <a href="https://scholar.google.com/citations?user=V-guxukAAAAJ">Google Scholar</a>.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
