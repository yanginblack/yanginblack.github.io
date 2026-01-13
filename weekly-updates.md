---
layout: default
title: Weekly Updates
permalink: /weekly-updates/
---

# 📅 Weekly Updates

Here you'll find my weekly summaries and updates.

[← Back to Home](/)

## All Weekly Updates

<ul>
  {% for post in site.categories.weekly-updates %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>

{% if site.categories.weekly-updates.size == 0 %}
<p><em>No posts yet. Check back soon!</em></p>
{% endif %}
