---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Display full project content -->
  {% for project in sorted_projects %}
    <div class="project-full">
      <h3>{{ project.title }}</h3>
      <p><strong>{{ project.description }}</strong></p>
      {{ project.content }}
      <hr>
    </div>
  {% endfor %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

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
{% endif %}
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
