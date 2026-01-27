---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 3
display_categories: false
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Display full project content -->
  {% for project in sorted_projects %}
    <div class="project-full">
      <h3>{{ project.title }}</h3>
      <p><strong>{{ project.description }}</strong></p>
      {{ project.content }}
      <hr>
    </div>
  {% endfor %}
</div>

<style>
.project-full {
  margin-bottom: 3rem;
  padding: 1.5rem;
  background-color: #f8f9fa;
  border-radius: 8px;
}

.project-full h3 {
  color: #2c3e50;
  margin-bottom: 1rem;
}

.project-full p {
  font-size: 1.1rem;
  line-height: 1.6;
}

.project-full hr {
  margin-top: 2rem;
  border-top: 2px solid #dee2e6;
}
</style>
