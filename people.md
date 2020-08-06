---
title: People
permalink: /people/
---

<!-- ## Lab Members -->

{% assign all_people = site.people %}
 
{% assign all_roles = 'Research Team' | split: '|'  %}

{% for role in all_roles %}

  {% assign people_for_role = all_people | where: 'position',role %}

  <br>
  <div class="people-title">
    <h3>Principal Investigator</h3>
  </div>
  <div class="list-item-people">
    <p class="list-post-title">
      <a href="https://web.stanford.edu/~schwager/">
        <img
          class="pi-thumbnail"
          src="{{site.url}}/images/people/macschwager.jpg">
      </a>
      <a class="name" href="https://web.stanford.edu/~schwager/">
        <b>Mac Schwager</b>
      </a>
      <p> Assistant Professor </p>
    </p>
  </div>

  <div class="people-title">
    <h3>Research Team</h3>
  </div>

  <div class="content list people">

    {% for person in all_people %}
      {% if person.position == 'researchengineer' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'postdoc' %}
        {% include person.html position=person.position %}
      {% endif %} 
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'phd' %}
        {% include person.html position=person.position %}
      {% endif %} 
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'gradstudent' %}
        {% include person.html position=person.position %}
      {% endif %} 
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'undergrad' %}
        {% include person.html position=person.position %}
      {% endif %} 
    {% endfor %}

    {% for person in all_people %}
      {% if person.position == 'affiliate' %}
        {% include person.html position=person.position %}
      {% endif %}
    {% endfor %}

  </div>
{% endfor %}