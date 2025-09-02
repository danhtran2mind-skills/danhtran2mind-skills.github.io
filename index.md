---
layout: default
title: Home
---

<!-- Skills Section -->
<section class="section">
  <h2>Skills</h2>
  <div class="grid">
    {% for skill in site.data.skills %}
      <div class="card">
        <p>{{ skill }}</p>
      </div>
    {% endfor %}
  </div>
</section>

<!-- Platform Course Section -->
<section class="section">
  <h2>Platform Course</h2>
  <div class="grid">
    {% for platform in site.data.platforms %}
      <div class="card">
        <a href="{{ platform.url }}" target="_blank">{{ platform.name }}</a>
      </div>
    {% endfor %}
  </div>
</section>

<!-- Certificates Section -->
<section class="section">
  <h2>Certificates</h2>
  <p>Certificates earned through course or program completion from educational platforms.</p>
  <div class="grid">
    {% for cert in site.data.certificates %}
      <div class="card">
        <h3>{{ cert.name }}</h3>
        <p>Issuer: {{ cert.issuer }}</p>
        <p>Date: {{ cert.date }}</p>
        {% if cert.url %}
          <p><a href="{{ cert.url }}" target="_blank">View Certificate</a></p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>

<!-- Certifications Section -->
<section class="section">
  <h2>Certifications</h2>
  <p>Industry-recognized credentials granted by professional organizations for specific skills or roles.</p>
  <div class="grid">
    {% for cert in site.data.certifications %}
      <div class="card">
        <h3>{{ cert.name }}</h3>
        <p>Issuer: {{ cert.issuer }}</p>
        <p>Date: {{ cert.date }}</p>
        {% if cert.url %}
          <p><a href="{{ cert.url }}" target="_blank">View Certification</a></p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>