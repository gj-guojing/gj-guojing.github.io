---
layout: page
title: Projects
permalink: /projects/
description: Research projects and professional experience
nav: true
nav_order: 3
display_categories: false
horizontal: false
---

<!-- Table of Contents -->
<div class="projects-toc">
  <h3>Table of Contents</h3>
  <ul class="toc-list">
    <li><a href="#nanke-pangu-humanoid-robot-project">Nanke Pangu Humanoid Robot Project</a></li>
    <li><a href="#design-and-control-of-balancing-robot-stander">Design and Control of Balancing Robot, STANDER</a></li>
    <li><a href="#electromechanical-design-of-bipedal-robot-stepper">Electromechanical Design of Bipedal Robot, STEPPER</a></li>
    <li><a href="#industrial-rd-at-bosch-rexroth">Industrial R&D at Bosch Rexroth</a></li>
    <li><a href="#autonomous-inspection-robot-for-data-centers">Autonomous Inspection Robot for Data Centers</a></li>
    <li><a href="#lower-limb-exoskeleton-prototype">Lower-limb Exoskeleton Prototype</a></li>
    <li><a href="#robomaster-robotics-competition-hosted-by-dji">RoboMaster Robotics Competition (Hosted by DJI)</a></li>
  </ul>
</div>

<!-- pages/projects.md -->
<div class="projects">
  <!-- Manually specify projects in correct order -->
  {% assign project_files = "1_pangu.md,2_stander.md,3_stepper.md,4_bosch.md,5_inspection.md,6_exoskeleton.md,7_robomaster.md" | split: "," %}

  {% for project_file in project_files %}
    {% for project in site.projects %}
      {% if project.name == project_file %}
        <div class="project-full" id="{{ project.title | slugify }}">
          <h3>{{ project.title }}</h3>
          <p><strong>{{ project.description }}</strong></p>
          {{ project.content }}
          <hr>
        </div>
      {% endif %}
    {% endfor %}
  {% endfor %}
</div>

<style>
.projects-toc {
  background-color: #f8f9fa;
  padding: 1.5rem;
  border-radius: 8px;
  margin-bottom: 2rem;
  border-left: 4px solid #007bff;
}

.projects-toc h3 {
  color: #2c3e50;
  margin-top: 0;
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.toc-list {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.toc-list li {
  margin-bottom: 0.75rem;
}

.toc-list a {
  color: #007bff;
  text-decoration: none;
  font-size: 1rem;
  transition: color 0.3s ease;
}

.toc-list a:hover {
  color: #0056b3;
  text-decoration: underline;
}

.project-full {
  margin-bottom: 3rem;
  padding: 1.5rem;
  background-color: #f8f9fa;
  border-radius: 8px;
  scroll-margin-top: 2rem;
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
