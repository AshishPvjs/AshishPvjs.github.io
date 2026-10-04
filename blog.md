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

<p>From <a href="https://goyalpramod.github.io/blog/">Pramod's Blog</a>: long, first-principles ML explainers, with some philosophy, life, and food posts too.</p>

<ul class="post-list">
  <li>
    <span class="post-meta">Oct 1, 2026 · 79 min · #rl #ml</span>
    <h3><a class="post-link" href="https://goyalpramod.github.io/blog/blogs/notes_on_RL/">Notes on RL</a></h3>
    <p>Notes on reinforcement learning concepts.</p>
  </li>
  <li>
    <span class="post-meta">Sep 25, 2026 · 15 min · #systems #llm</span>
    <h3><a class="post-link" href="https://goyalpramod.github.io/blog/blogs/supe_fast_inference/">Super Fast Inference</a></h3>
    <p>CUDA optimisation for fast inference.</p>
  </li>
  <li>
    <span class="post-meta">Jun 21, 2025 · 237 min · #llm #ml</span>
    <h3><a class="post-link" href="https://goyalpramod.github.io/blog/blogs/evolution_of_LLMs/">Evolution of LLMs</a></h3>
    <p>Language model development since the Transformer.</p>
  </li>
  <li>
    <span class="post-meta">Feb 15, 2025 · 44 min · #agents #llm</span>
    <h3><a class="post-link" href="https://goyalpramod.github.io/blog/blogs/AI_agents_from_first_principles/">AI Agents from First Principles</a></h3>
    <p>Building up AI agents from the basics.</p>
  </li>
  <li>
    <span class="post-meta">Feb 10, 2025 · 95 min · #diffusion #ml</span>
    <h3><a class="post-link" href="https://goyalpramod.github.io/blog/blogs/demysitifying_diffusion_models/">Demystifying Diffusion Models</a></h3>
    <p>Diffusion architectures and the maths behind them.</p>
  </li>
  <li>
    <span class="post-meta">Jan 3, 2025 · 53 min · #llm #ml</span>
    <h3><a class="post-link" href="https://goyalpramod.github.io/blog/blogs/Transformers_laid_out/">Transformers Laid Out</a></h3>
    <p>Transformer architecture fundamentals.</p>
  </li>
</ul>
