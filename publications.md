---
title: Publications
permalink: /publications/
layout: publications
---

{% assign years = "2020,2019,2018,2017,2016,2015,2014,2013" | split: ',' %}

{% for pub_year in years %}
<div class="publication-head-content">
<h3> {{pub_year}} </h3>
</div>
{% bibliography --query @*[year={{pub_year}}] %}
{% endfor %}

<p class="pub-bib">Download <a href="../papers/papers.bib">bibtex</a>.</p>
<br>