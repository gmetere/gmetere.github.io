---
layout: page
title: Notebook
permalink: /notebook/
---

This notebook collects occasional notes on mathematics, teaching, writing,
and academic life.

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <p class="post-date">{{ post.date | date: "%-d %B %Y" }}</p>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {% if post.excerpt %}
        <p>{{ post.excerpt | strip_html | truncatewords: 35 }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
