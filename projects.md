---
layout: page
title: Projects
permalink: /projects/
---

Welcome to my project showcase.  
This is a collection of personal, academic, and experimental projects that reflect my work in game development, computer graphics, computer vision, and other areas of software engineering.

Feel free to explore!

<div class="filter-buttons">
  <button data-filter="all" class="active">All</button>
  <button data-filter="game">Games</button>
  <button data-filter="plugin">Plugins</button>
  <button data-filter="computer graphics">Graphics</button>
  <button data-filter="computer vision">Vision</button>
  <button data-filter="c++">C++</button>
  <button data-filter="python">Python</button>
  <button data-filter="UE5">UE5</button>
  <button data-filter="blender">blender</button>
  <button data-filter="team project">Team project</button>
  <button data-filter="solo project">Solo project</button>
</div>

<div class="project-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <div class="project-status {{ project.status | downcase }}">
        {% if project.status == "done" %}
          <span class="dot"></span> Done
        {% elsif project.status == "in progress" %}
          <span class="dot"></span> In Progress
        {% elsif project.status == "abandoned" %}
          <span class="dot"></span> Abandoned
        {% elsif project.status == "prototype" %}
          <span class="dot"></span> Prototype
        {% endif %}
      </div>
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <a class="button" href="{{ project.url | relative_url }}">Learn More</a>
    </div>
  {% endfor %}
</div>