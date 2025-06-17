---
layout: default
title: Blog
permalink: /blog/
---

# Course Project Blog

This blog documents my journey through my current course project. I'll be sharing updates on progress, technical challenges encountered, solutions developed, and reflections on my learning.

## Recent Posts

{% assign posts = site.posts | where_exp: "post", "post.date <= site.time" %}
{% if posts.size > 0 %}
  <div class="post-list">
  {% for post in posts %}
    <article class="post-preview">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      
      {% if post.excerpt %}
        <div class="post-excerpt">
          {{ post.excerpt | strip_html | truncatewords: 30 }}
        </div>
      {% endif %}
      
      <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
    </article>
    {% unless forloop.last %}<hr>{% endunless %}
  {% endfor %}
  </div>
{% else %}
  <p>No posts yet. Check back soon!</p>
{% endif %}
