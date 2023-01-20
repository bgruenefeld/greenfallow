---
layout: post
title: Neuigkeiten
---
  
  <ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} ... weiter lesen</a>
    </li>
  {% endfor %}
</ul>

