---
layout: page
title: Projects
permalink: /projects/
---

Welcome to my project showcase.  
This is a collection of personal, academic, and experimental projects that reflect my work in game development, computer graphics, computer vision, and other areas of software engineering.

Feel free to explore!

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