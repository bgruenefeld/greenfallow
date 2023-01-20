---
layout: post
title: Neuigkeiten
---

  {% for post in site.posts %}
    <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    <p class="author">
      <span class="date">{{ post.date }}</span>
    </p>
    <div class="content">
      {{ post.content }} <a href="{{ post.url }}">... weiter lesen ...</a>
    </div>
  {% endfor %}

