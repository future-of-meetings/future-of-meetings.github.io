---
permalink: /about/team.html
layout: people
title: Future of Meetings Collaborators
---

{% assign team = site.collaborators %}

<h1>Future of Meetings Project Collaborators</h1><br>

<div class="container-fluid">
  <div class="row">
    {% for collaborator in team %}
       {% if collaborator.active and collaborator.hidden != true %}
         {% include standard_person_card.md person=collaborator %}
       {% endif %}
    {% endfor %}
  </div>
</div>

