---
layout: default
title: "TierrasSapiens"
---
<div class="post-list">
{% for post in site.posts %}
  <div class="post-item">
    
    {% if post.image %}        <img class="post-thumb" src="{{ post.image }}" alt="thumb">
    {% endif %}
    
    <a class="post-title" href="{{ post.url | relative_url }}">       {{ post.title }}
    </a>

  </div>
{% endfor %}
</div>