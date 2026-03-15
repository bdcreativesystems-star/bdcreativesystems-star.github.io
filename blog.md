---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog-grid">
  {% for post in site.posts %}
    <article class="blog-card">
      <a href="{{ post.url | relative_url }}" class="blog-card-link">
        <div class="blog-card-content">
          <p class="blog-meta">{{ post.date | date: "%B %d, %Y" }}</p>
          <h2>{{ post.title }}</h2>
          <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
          <span class="read-more">Read article →</span>
        </div>
      </a>
    </article>
  {% endfor %}
</div>