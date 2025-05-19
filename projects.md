---
layout: page
title: Projects
permalink: /projects/
---

# Projects

<h2>Debug Output</h2>
<p>{{ site.projects | inspect }}</p>

<div class="project-grid">
  {% for project in site.projects %}
    <p>{{ project.title }}</p>
  {% endfor %}
</div>

<div class="project-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <img src="{{ project.image }}" alt="{{ project.title }}" />
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <a class="button" href="{{ project.url }}">Learn More</a>
    </div>
  {% endfor %}
</div>