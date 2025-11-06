---
layout: home
title: "Hi! I'm Eric Sigg"
collection: portfolio
entries_layout: grid
permalink: /
author_profile: true
---


Welcome to my portfolio! I'm excited to show off some of the projects I've worked on throughout my time at the University of Pennsylvania, in academic courses as well as for my own original research and for fun.

![My Image](/assets/images/coverImage.jpg)

<div class="projects-grid">
  {% assign projects = site.portfolio | sort: "order" %}
  {% for project in projects %}
  <div class="project-item">
    <a href="{{ project.url }}">
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
      <h2>{{ project.title }}</h2>
    </a>
  </div>
  {% endfor %}
</div>
