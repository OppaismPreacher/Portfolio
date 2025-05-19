---
layout: page
title: Projects
permalink: /projects/
---

Welcome to my project showcase.  
This is a collection of personal, academic, and experimental projects that reflect my work in game development, computer graphics, computer vision, and other areas of software engineering. Each project includes a brief overview, an image preview, and a link to learn more about its development and purpose.

Feel free to explore!

<div class="project-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <a class="button" href="{{ project.url }}">Learn More</a>
    </div>
  {% endfor %}
</div>