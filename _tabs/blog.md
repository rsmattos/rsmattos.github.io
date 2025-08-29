---
layout: page
title: Blog
icon: fas fa-pen-nib
order: 30
permalink: /blog/
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="post-meta"> — {{ post.date | date: "%Y-%m-%d" }}</span>
      {% if post.excerpt %}<p>{{ post.excerpt }}</p>{% endif %}
    </li>
  {% endfor %}
</ul>
