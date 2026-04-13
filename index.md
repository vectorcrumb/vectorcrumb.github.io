---
layout: default
title: Home
---

<div class="home-intro">
  <p>Hi, I'm [Your Name]. Welcome to my corner of the internet.</p>
  <p>I write about things I'm building, thinking about, and learning. You can find my writing on the <a href="/blog">blog</a>, tools I've made on the <a href="/tools">tools</a> page, and projects I'm working on under <a href="/projects">projects</a>.</p>
</div>

<div class="recent-posts">
  <h2>Recent posts</h2>
  <div class="post-list">
    {% for post in site.posts limit:10 %}
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <span class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></span>
    {% endfor %}
  </div>
</div>
