---
layout: page
title: Projects
permalink: /projects/
---

# Projects

![Test Image](/assets/images/projects/testProject.png)

<div class="project-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <img src="{{ project.image }}" alt="{{ project.title }}" />
      <h3>{{ project.title }}</h3>
      <p>Image path: {{ project.image }}</p>
      <p>{{ project.description }}</p>
      <a class="button" href="{{ project.url }}">Learn More</a>
    </div>
  {% endfor %}
</div>