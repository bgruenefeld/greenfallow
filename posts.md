---
layout: post
title: Neuigkeiten
---
  
  <ul>
  {% for post in site.posts %}
    <li>
      <h2>{{ post.title }}</h2><a href="{{ post.url }}"> ... weiter lesen</a>
    </li>
  {% endfor %}
</ul>

