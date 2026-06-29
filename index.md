---
layout: default
title: Home
---

<header class="page-header">
  <h1>Blog</h1>
</header>

<div class="post-list">
  {% for post in site.posts %}
    <span class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></span>
    <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
  {% endfor %}
</div>
