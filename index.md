---
layout: default
title: "TierraSapiens"
---
<div class="post-list">
{%- for post in site.posts -%}  <div class="post-item">
    {% if post.image %}
    <img class="post-thumb" src="{{ post.image | relative_url }}" alt="thumb"/>
    {% endif %}
    <div class="post-content"> 
        <a class="post-title" href="{{ post.url | relative_url }}">
            {{ post.title }}
        </a>
        <div class="post-meta"> Fecha de publicación: {{ post.date | date: "%d/%m/%Y" }}
            {% if post.author %}
                | Autor: {{ post.author }}
            {% endif %}
        </div>
    </div>
</div>
{%- endfor -%}  </div>