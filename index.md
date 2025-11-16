---
layout: default
title: "Realidad Alterna"
---

# Bienvenido a Realidad Alterna

Exploración, ciencia, tecnología, cultura, misterio y mundos posibles.

---

## Últimos artículos

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>  
      <small> — {{ post.date | date: "%d/%m/%Y" }}</small>
    </li>
  {% endfor %}
</ul>
