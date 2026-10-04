---
layout: page
title: Blog
permalink: /blog.html
---

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

## Recommended reading

<ul class="post-list">
  <li>
    <h3><a class="post-link" href="https://magazine.sebastianraschka.com/?utm_source=homepage_recommendations&utm_campaign=4634702">Ahead of AI</a></h3>
    <p>A newsletter on machine learning and AI research, by Sebastian Raschka.</p>
  </li>
  <li>
    <h3><a class="post-link" href="https://aiengineersjourney.substack.com">An AI Engineer's Journey</a></h3>
    <p>Practical machine learning education through building small, real-world systems.</p>
  </li>
</ul>
