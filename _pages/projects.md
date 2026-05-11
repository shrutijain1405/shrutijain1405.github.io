---
layout: page
title: Projects
permalink: /projects/
description: A collection of research projects and course work spanning computer vision, multimodal learning, NLP, and autonomous systems.
nav: true
nav_order: 3
horizontal: false
---

<style>
  .projects-container {
    max-width: 1400px;
    margin: 0 auto;
  }
  .projects-container .card {
    width: 100%;
    margin-bottom: 1.5rem;
  }
  .projects-container .card-body {
    padding: 1.5rem 2rem;
  }
</style>

<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="projects-container row row-cols-1">
    {% for project in sorted_projects %}
      {% include projects.html %}
    {% endfor %}
  </div>
</div>