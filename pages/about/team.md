---
permalink: /about/team.html
layout: people
title: Future of Meetings Collaborators
---

<h1>Future of Meetings Project Collaborators</h1><br>

<div class="container-fluid">
  <div class="row">
    {% for collaborator in site.collaborators %}
       {% if collaborator.active and collaborator.hidden != true %}
         {% comment %}
         {% include standard_person_card.md person=collaborator %}
         {% endcomment %}
       {{ collaborator.name }}
       {% endif %}
    {% endfor %}
  </div>
</div>

