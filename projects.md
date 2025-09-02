---
layout: default
title: Projects
---

<section class="section">
  <h2>Projects</h2>
  <p>Selected projects showcasing my work in Machine Learning, Data Science, and Networking.</p>
  <div class="grid">
    {% for project in site.data.projects %}
      <div class="card">
        <h3>{{ project.name }}</h3>
        <p>{{ project.description }}</p>
        <p><a href="{{ project.url }}" target="_blank">View Project</a></p>
      </div>
    {% endfor %}
  </div>
</section>