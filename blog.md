---
layout: default
title: Blog
permalink: /blog/
---

# Course Project Blog

This blog documents my journey through my current course project. I'll be sharing updates on progress, technical challenges encountered, solutions developed, and reflections on my learning.

{% for post in site.posts %}
  ## [{{ post.title }}]({{ post.url | relative_url }})
  *{{ post.date | date: "%B %d, %Y" }}*

  {{ post.excerpt }}
  
  [Read more]({{ post.url | relative_url }})
  <hr/>
{% endfor %}
