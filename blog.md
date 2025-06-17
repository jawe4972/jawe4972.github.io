---
layout: default
title: Blog
permalink: /blog/
---

# Course Project Blog

This blog documents my journey through my current course project. I'll be sharing updates on progress, technical challenges encountered, solutions developed, and reflections on my learning.

## Recent Posts

{% for post in site.posts reversed %}
<div class="post-preview">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p class="post-meta">
    Posted on {{ post.date | date: "%B %d, %Y" }}
  </p>
  
  {% if post.excerpt %}
    <p>{{ post.excerpt }}</p>
  {% endif %}
  
  <a href="{{ post.url | relative_url }}" class="read-more">Read More</a>
</div>
<hr>
{% endfor %}


