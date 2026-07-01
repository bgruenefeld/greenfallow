---
layout: default
title: Beitragsarchiv
seo_title: Beitragsarchiv | Greenfallow Labradors
description: Alle Beiträge von Greenfallow Labradors in chronologischer Übersicht.
permalink: /posts-archive/
---

<section class="posts-page">
  <header class="posts-page__header">
    <p class="eyebrow">Archiv</p>
    <h1>Alle Beiträge</h1>
    <p>Chronologische Übersicht aller veröffentlichten Beiträge.</p>
  </header>

  <div class="post-list">
    {% for post in site.posts %}
      {% assign topic = post.topic | default: post.categories.first | default: "Neuigkeiten" %}
      <article class="post-card">
        <p class="post-card__date">{{ post.date | date: "%d.%m.%Y" }} · {{ topic }}</p>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        {% if post.description %}
          <p>{{ post.description }}</p>
        {% else %}
          <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
        {% endif %}
        <a class="text-link" href="{{ post.url | relative_url }}">Weiter lesen</a>
      </article>
    {% endfor %}
  </div>
</section>
