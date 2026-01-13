---
layout: default
title: Home
---

# Welcome to Yang's Blog

Welcome to my personal blog where I share weekly updates, technical insights, and thoughts on board games.

## Categories

<nav class="site-nav">
  <ul>
    <li><a href="/weekly-updates">📅 Weekly Updates</a></li>
    <li><a href="/technical-blogs">💻 Technical Blogs</a></li>
    <li><a href="/board-games">🎲 Board Games</a></li>
  </ul>
</nav>

## Recent Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      {% if post.categories %}
        <span class="post-category">{{ post.categories | join: ', ' }}</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>
