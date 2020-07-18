---
title: People
permalink: /people/
---

## Lab Members

A bustling group of people solving challenging problems holding back multi-robot systems.

{% assign all_people = site.people %}
{% assign all_roles = 'researchengineer|gradstudent' | split: '|'  %}

{% for role in all_roles %}

{% assign people_for_role = all_people | where: 'position',role %}


<div class="pos-header">
{% if role == 'gradstudent' %}
  <h3>Graduate Students</h3>
{% elsif role == 'researchengineer' %}
  <h3>Research Engineer</h3>
{% endif %}
</div>


<div class="content list people">
  {% for person in all_people %}
    {% if person.position contains role %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if person.avatar %}
            <a href="{{site.url}}{{person.url}}">
              <img class="profile-thumbnail" src="{{site.url}}/images/people/{{person.avatar}}"></a>
           {% endif %}
           <a class="name" href="{{site.url}}{{person.url}}">{{person.name}}</a>
        </p>
      </div>
     {% endif %}
  {% endfor %}
</div>
{% endfor %}
