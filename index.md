---
layout: default
title: Inicio
---

# Mi Blog en GitHub Pages

Bienvenido a mi blog estático. Aquí están los posts más recientes:

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p><small>{{ post.date | date: "%d-%m-%Y" }}</small></p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
