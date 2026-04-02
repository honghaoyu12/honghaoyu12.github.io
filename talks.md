---
title: Talks
description: "Invited talks, conference presentations, and tutorials."
permalink: /talks/
---

List invited talks, conference talks, and workshops here. Later we can add slide links, videos, or filters by year.

<div class="collection-list">
  {% assign items = site.talks | sort: "date" | reverse %}
  {% for item in items %}
    <article class="collection-item">
      <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
      <p class="collection-meta">
        {% if item.venue %}{{ item.venue }}{% endif %}
        {% if item.venue and item.location %} · {% endif %}
        {% if item.location %}{{ item.location }}{% endif %}
        {% if item.date %} · {{ item.date | date: "%B %Y" }}{% endif %}
      </p>
      <p>{{ item.summary }}</p>
    </article>
  {% endfor %}
</div>

