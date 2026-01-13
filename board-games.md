---
layout: default
title: Board Games
permalink: /board-games/
---

# 🎲 Board Games

Here you'll find my thoughts, reviews, and discussions about board games.

[← Back to Home](/)

## All Board Game Posts

<ul>
  {% for post in site.categories.board-games %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>

{% if site.categories.board-games.size == 0 %}
<p><em>No posts yet. Check back soon!</em></p>
{% endif %}
