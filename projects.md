---
title: Projects
description: "Research software, prototypes, datasets, and other selected work."
permalink: /projects/
---

This page is a home for research projects that do not fit neatly into a publication list. It works well for software systems, experimental demos, datasets, and collaborative initiatives.

<div class="collection-list">
  {% assign items = site.projects | sort: "date" | reverse %}
  {% for item in items %}
    <article class="collection-item">
      <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
      <p class="collection-meta">
        {% if item.role %}{{ item.role }}{% endif %}
        {% if item.role and item.date %} · {% endif %}
        {% if item.date %}{{ item.date | date: "%B %Y" }}{% endif %}
      </p>
      <p>{{ item.summary }}</p>
    </article>
  {% endfor %}
</div>

