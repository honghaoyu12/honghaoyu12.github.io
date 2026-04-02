---
title: Publications
description: "Peer-reviewed papers, preprints, and selected manuscripts."
permalink: /publications/
---

Use this page to present your publication record in a consistent and readable format. Each publication lives in the `_publications` collection, so adding a new paper only requires creating one Markdown file.

<div class="collection-list">
  {% assign items = site.publications | sort: "date" | reverse %}
  {% if items.size > 0 %}
    {% for item in items %}
      <article class="collection-item">
        <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
        <p class="collection-meta">
          {% if item.authors %}{{ item.authors }}{% endif %}
          {% if item.authors and item.venue %} · {% endif %}
          {% if item.venue %}{{ item.venue }}{% endif %}
          {% if item.date %} · {{ item.date | date: "%Y" }}{% endif %}
        </p>
        <p>{{ item.summary }}</p>
      </article>
    {% endfor %}
  {% else %}
    <div class="collection-item collection-empty">
      <p>Publications will appear here once they are added.</p>
    </div>
  {% endif %}
</div>
