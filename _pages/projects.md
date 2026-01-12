---
layout: default
title: Projects
permalink: /projects/
---

<h1>Projects</h1>
<p class="muted">Selected engineering work—design, testing, robotics, controls, and system integration.</p>

<div class="projects-list">
  {% assign sorted_projects = site.projects | sort: "date" | reverse %}
  {% for project in sorted_projects %}
    <a class="project-card__link" href="{{ project.url | relative_url }}">
      <div class="project-card">
        <div class="project-card__bar"></div>

        <div class="project-card__content">
          <h2 class="project-card__title">{{ project.title }}</h2>

          {% if project.date %}
            <div class="project-card__meta">{{ project.date | date: "%B %Y" }}</div>
          {% endif %}

          {% if project.description %}
            <p class="project-card__desc">{{ project.description }}</p>
          {% else %}
            <p class="project-card__desc">
              {{ project.excerpt | strip_html | truncate: 180 }}
            </p>
          {% endif %}
        </div>

        <div class="project-card__image">
          {% if project.image %}
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }} cover image">
          {% else %}
            <img src="{{ '/assets/images/placeholder.png' | relative_url }}" alt="Project placeholder">
          {% endif %}
        </div>
      </div>
    </a>
  {% endfor %}
</div>
