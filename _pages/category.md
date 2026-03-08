---
title: "Category"
permalink: /category/
excerpt: "Notes grouped by topic"
author_profile: true
---

{% assign notes_site_url = site.notes_site_url | default: "" %}

<section class="notes-hero">
  <p class="notes-hero__kicker">Knowledge Base</p>
  <h1 class="notes-hero__title">Research Notes by Category</h1>
  <p class="notes-hero__subtitle">Each note will open on an external notes site.</p>
  {% if notes_site_url != "" %}
  <p class="notes-hero__subtitle">Notes site: <a href="{{ notes_site_url }}" target="_blank" rel="noopener noreferrer">{{ notes_site_url }}</a></p>
  {% else %}
  <p class="notes-hero__subtitle">Notes site is not published yet. Links will be enabled after deployment.</p>
  {% endif %}
</section>

{% assign note_groups = site.data.notes.categories %}
{% if note_groups and note_groups.size > 0 %}
<div class="notes-grid">
  {% for group in note_groups %}
  <article class="notes-group">
    <h2>{{ group.name }}</h2>
    {% if group.description %}
    <p class="notes-group__desc">{{ group.description }}</p>
    {% endif %}

    <ul class="notes-list">
      {% for note in group.notes %}
      {% assign note_target = "" %}
      {% if note.url %}
        {% assign note_target = note.url %}
      {% elsif note.path and notes_site_url != "" %}
        {% assign note_target = notes_site_url | append: "/" | append: note.path %}
      {% endif %}
      <li class="notes-item">
        <h3 class="notes-item__title">
          {% if note_target != "" %}
          <a href="{{ note_target }}" target="_blank" rel="noopener noreferrer">{{ note.title }}</a>
          {% else %}
          {{ note.title }}
          {% endif %}
        </h3>

        {% if note.summary %}
        <p class="notes-item__summary">{{ note.summary }}</p>
        {% endif %}

        <p class="notes-item__meta">
          {% if note.date %}<span>{{ note.date }}</span>{% endif %}
          {% if note.tags %}<span>{{ note.tags | join: " | " }}</span>{% endif %}
          {% if note.path %}<span>{{ note.path }}</span>{% endif %}
          {% unless note_target != "" %}<span>Pending publish</span>{% endunless %}
        </p>
      </li>
      {% endfor %}
    </ul>
  </article>
  {% endfor %}
</div>
{% else %}
<p>No notes yet. Add note entries to <code>_data/notes.yml</code> to render them here.</p>
{% endif %}
