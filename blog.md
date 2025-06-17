---
layout: default
title: Blog
permalink: /blog/
---

# Course Project Blog

This blog documents my journey through my current course project. I'll be sharing updates on progress, technical challenges encountered, solutions developed, and reflections on my learning.

## Recent Posts

{% for post in site.posts %}
<div class="post">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
  
  {{ post.excerpt }}
  
  <a href="{{ post.url | relative_url }}">Read more...</a>
</div>
<hr>
{% endfor %}

