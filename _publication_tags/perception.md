---
title: Perception
layout: publications
permalink: publications/perception
---
  

{% assign groups = "Filtering and Estimation,Localization,Mapping,Scene Reconstruction,Target Tracking" | split: ',' %}

{% for pub_group in groups %}
<div class="publication-head-content">
<h3> {{pub_group}} </h3>
</div>
{% assign keyword = pub_group | downcase | replace: " ", "\_" %}
{% bibliography --query @*[keywords={{keyword}}] %}
{% endfor %}
