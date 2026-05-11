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
  /* Override the default multi-column grid to a single wide column */
  .projects .row {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .projects .row .col-sm {
    width: 100%;
    max-width: 900px;
  }
  /* Widen the project cards */
  .projects .card {
    width: 100%;
    max-width: 900px;
  }
  /* Full-width project card content */
  .card-body {
    padding: 1.5rem 2rem;
  }
</style>

<!-- pages/projects.md -->
<div class="projects">
{% assign sorted_projects = site.projects | sort: "importance" %}
<div class="row row-cols-1" style="max-width: 900px; margin: 0 auto;">
  {% for project in sorted_projects %}
    {% include projects.html %}
  {% endfor %}
</div>
</div>