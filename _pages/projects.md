---
layout: default
title: Cristian Avelar-Romero – Projects
permalink: /projects/
---

<h2>Projects</h2>

{% for project in site.projects %}
  <div class="gallery-item" style="margin-bottom: 1.5rem;">
    <a href="{{ project.url | relative_url }}">
      <h3>{{ project.title }}</h3>

      {% if project.image %}
        <img
          src="{{ project.image | relative_url }}"
          alt="{{ project.title }}"
          style="max-width: 300px;"
        >
      {% endif %}
    </a>

    <p>{{ project.description }}</p>
  </div>
{% endfor %}
