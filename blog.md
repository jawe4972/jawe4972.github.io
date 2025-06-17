---
layout: default
title: Blog
permalink: /blog/
---

# Course Project Blog

This blog documents my journey through my current course project. I'll be sharing updates on progress, technical challenges encountered, solutions developed, and reflections on my learning.

## Recent Posts

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
    <div class="post-preview">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      
      {% if post.excerpt %}
        <div class="post-excerpt">
          {{ post.excerpt }}
        </div>
      {% endif %}
      
      <a href="{{ post.url | relative_url }}">Read more...</a>
    </div>
    <hr>
  {% endfor %}
{% else %}
  <p>No posts yet. Check back soon!</p>
{% endif %}
