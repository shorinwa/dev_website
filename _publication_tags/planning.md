---
title: Planning
layout: publications
permalink: publications/planning
---
  

{% assign groups = "Collaborative Manipulation,Game Theoretic Planning,Cooperative Planning" | split: ',' %}

{% for pub_group in groups %}
<div class="publication-head-content">
<h3> {{pub_group}} </h3>
</div>
{% assign keyword = pub_group | downcase | replace: " ", "\_" %}
{% bibliography --query @*[keywords={{keyword}}] %}
{% endfor %}
