---
layout: default
title: Zuchtwissen
seo_title: Zuchtwissen | Greenfallow Labradors
description: Fachbeiträge zu Gesundheit, Genetik und Zucht bei Labrador Retrievern aus Arbeitslinien.
permalink: /zuchtwissen/
---

<section class="posts-page">
  <header class="posts-page__header">
    <p class="eyebrow">Wissenswertes</p>
    <h1>Zuchtwissen</h1>
    <p>Grundlegende Beiträge zu Gesundheit, Genetik und Zucht.</p>
  </header>

  <div class="post-list">
    {% for post in site.posts %}
      {% assign topic = post.topic | default: post.categories.first %}
      {% if topic == "Gesundheit" or topic == "Zucht und Genetik" %}
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
      {% endif %}
    {% endfor %}
  </div>
</section>
