---
layout: default
title: "Realidad Alterna"
---

<div class="intro">
  <h1>Lista de Publicaciones de Tierras Sapiens – Realidad Alterna</h1>
</div>

<div class="post-list">
{% for post in site.posts %}
  <div class="post-item">
    <a class="post-title" href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>

    {% if post.image %}
      <img class="post-thumb" src="{{ post.image }}" alt="thumb">
    {% endif %}
  </div>
{% endfor %}
</div>
