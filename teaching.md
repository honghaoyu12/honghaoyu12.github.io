---
title: Teaching
description: "Courses taught, assisted, or developed."
permalink: /teaching/
---

Use this page for courses, tutorials, and mentorship-related teaching work. If teaching is not part of your public profile yet, we can hide this section later.

<div class="collection-list">
  {% assign items = site.teaching | sort: "date" | reverse %}
  {% for item in items %}
    <article class="collection-item">
      <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
      <p class="collection-meta">
        {% if item.role %}{{ item.role }}{% endif %}
        {% if item.role and item.term %} · {% endif %}
        {% if item.term %}{{ item.term }}{% endif %}
      </p>
      <p>{{ item.summary }}</p>
    </article>
  {% endfor %}
</div>

