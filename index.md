---
layout: default
title: Home
---

<div class="hero">
  <h1>Ad Astra</h1>
  <p>
    I build things and write about what I learn along the way.
    Take a look at my <a href="{{ '/projects.html' | relative_url }}">projects</a>,
    read my <a href="{{ '/blog.html' | relative_url }}">blog</a>,
    or find out more <a href="{{ '/about.html' | relative_url }}">about me</a>.
  </p>
</div>

## Latest posts

<ul class="post-list">
  {% for post in site.posts limit:5 %}
  <li>
    <span class="post-meta">{{ post.date | date: site.minima.date_format }}</span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h3>
  </li>
  {% endfor %}
</ul>
