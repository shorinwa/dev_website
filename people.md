---
title: People
permalink: /people/
---

<!-- ## Lab Members -->


{% assign all_people = site.people %}
 
{% assign all_roles = 'Research Team' | split: '|'  %}

{% for role in all_roles %}

{% assign people_for_role = all_people | where: 'position',role %}


<div class="pos-header">
<!--
{% if role == 'Research Engineer' %}
  <h3>Research Engineers</h3>
{% elsif role == 'Postdoctoral Scholar' %}
  <h3>Postdoctoral Scholars</h3>
{% elsif role == 'PhD Candidate' %}
  <h3>PhD Candidates</h3>
{% elsif role == 'Graduate Student' %}
  <h3>Graduate Students</h3>
{% endif %}
-->
</div>

<h3>Principal Investigator</h3>
<div class="list-item-people">
        <p class="list-post-title">
		<a href="https://web.stanford.edu/~schwager/">
		<img class="profile-thumbnail" src="{{site.url}}/images/people/macschwager.jpg"></a>
		<a class="name" href="https://web.stanford.edu/~schwager/"><b>Mac Schwager</b></a>
		</p>
</div>

<br>
<h3>Research Team</h3>

<style> p{margin:0; padding:0;} </style>
<style> hr{margin:0; padding:0;} </style>










<div class="content list people">
  {% for person in all_people %}
	{% if person.position == 'Research Engineer' %}
    
      <div class="list-item-people">
        <p class="list-post-title">
          {% if person.avatar %}
            <a href="{{site.url}}{{person.url}}">
              <img class="profile-thumbnail" src="{{site.url}}/images/people/{{person.avatar}}"></a>
           {% endif %}
           <a class="name" href="{{site.url}}{{person.url}}"><b>{{person.name}}</b></a>
		   
        </p>
		<p> {{person.position}} <hr> </p>
		<p style="width: 200px;"> {{person.description}} </p>
      </div>
	  
	{% endif %}
     
  {% endfor %}
  
  
  {% for person in all_people %}
	{% if person.position == 'Postdoctoral Scholar' %}
    
      <div class="list-item-people">
        <p class="list-post-title">
          {% if person.avatar %}
            <a href="{{site.url}}{{person.url}}">
              <img class="profile-thumbnail" src="{{site.url}}/images/people/{{person.avatar}}"></a>
           {% endif %}
           <a class="name" href="{{site.url}}{{person.url}}"><b>{{person.name}}</b></a>
		   
        </p>
		<p> {{person.position}} <hr> </p>
		<p style="width: 200px;"> {{person.description}} </p>
      </div>
	  
	{% endif %}
     
  {% endfor %}
  
  
  {% for person in all_people %}
	{% if person.position == 'PhD Candidate' %}
    
      <div class="list-item-people">
        <p class="list-post-title">
          {% if person.avatar %}
            <a href="{{site.url}}{{person.url}}">
              <img class="profile-thumbnail" src="{{site.url}}/images/people/{{person.avatar}}"></a>
           {% endif %}
           <a class="name" href="{{site.url}}{{person.url}}"><b>{{person.name}}</b></a>
		   
        </p>
		<p> {{person.position}} <hr> </p>
		<p style="width: 200px;"> {{person.description}} </p>
      </div>
	  
	{% endif %}
     
  {% endfor %}
  
  
  {% for person in all_people %}
	{% if person.position == 'Graduate Student' %}
    
      <div class="list-item-people">
        <p class="list-post-title">
          {% if person.avatar %}
            <a href="{{site.url}}{{person.url}}">
              <img class="profile-thumbnail" src="{{site.url}}/images/people/{{person.avatar}}"></a>
           {% endif %}
           <a class="name" href="{{site.url}}{{person.url}}"><b>{{person.name}}</b></a>
		   
        </p>
		<p> {{person.position}} <hr> </p>
		<p style="width: 200px;"> {{person.description}} </p>
      </div>
	  
	{% endif %}
     
  {% endfor %}
</div>
{% endfor %}