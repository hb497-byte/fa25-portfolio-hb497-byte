---
layout: default
title: Hillary Browne - Portfolio
permalink: /projects/
---

<div class="gallery-container">
  <div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title | escape }}" />
        </a>
        <h2 class="gallery-title">{{ project.title | escape }}</h2>
      </div>
    {% endfor %}
  </div>
</div>
