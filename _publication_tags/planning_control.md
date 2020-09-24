---
title: Planning and Control
layout: publications
permalink: publications/planning_control
---
  

{% assign groups = "Collaborative Manipulation,Game Theoretic Planning,Cooperative Planning,Formation Control,Persistent Surveillance,Coverage Control,Signal Temporal Logic,Pursuit Evasion,Soft Robotics,Belief Space Control,Optimal Control" | split: ',' %}

{% for pub_group in groups %}
<div class="publication-head-content">
<h3> {{pub_group}} </h3>
</div>
{% assign keyword = pub_group | downcase | replace: " ", "\_" %}
{% bibliography --query @*[keywords={{keyword}}] %}
{% endfor %}
