---
layout: page
title: Blog
description: Writing from Ashish Peruri.
permalink: /blog.html
---

<p class="page-subtitle">
  <a href="{{ '/notes.html' | relative_url }}">Notes on what I'm building and reading</a>
</p>

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <span class="post-meta">{{ post.date | date: site.minima.date_format }}</span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h3>
    {% if post.excerpt %}
      <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    {% endif %}
  </li>
  {% endfor %}
</ul>
