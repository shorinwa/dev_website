---
title: Learning
layout: publications
permalink: publications/learning
---
  

{% assign groups = "Learning Dynamical Systems,Learning Controllers,Learning Optimization Solutions" | split: ',' %}

{% for pub_group in groups %}
<div class="publication-head-content">
<h3> {{pub_group}} </h3>
</div>
{% assign keyword = pub_group | downcase | replace: " ", "\_" %}
{% bibliography --query @*[keywords={{keyword}}] %}
{% endfor %}
