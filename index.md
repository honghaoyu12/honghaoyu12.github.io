---
layout: home
title: Home
---

I am a researcher working at the intersection of machine learning, systems, and human-centered computing. This scaffolded homepage is designed to make your academic profile easy to understand at a glance and straightforward to maintain over time.

You can use this page to describe your research agenda in plain language, point visitors to your best papers, and share a short note about current collaborations, open positions, or ongoing projects.

## Selected Work

Selected publications and projects will appear here as they are added.

{% assign featured_publications = site.publications | sort: "date" | reverse | slice: 0, 3 %}
{% if featured_publications.size > 0 %}
<div class="collection-list">
  {% for item in featured_publications %}
    <article class="collection-item">
      <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
      <p class="collection-meta">
        {% if item.venue %}{{ item.venue }}{% endif %}
        {% if item.venue and item.date %} · {% endif %}
        {% if item.date %}{{ item.date | date: "%Y" }}{% endif %}
      </p>
      <p>{{ item.summary }}</p>
    </article>
  {% endfor %}
</div>
{% else %}
<div class="collection-item collection-empty">
  <p>No publications have been added yet.</p>
</div>
{% endif %}
