---
layout: default
title: Blog
permalink: /blog/
---

# Course Project Blog

This blog documents my journey through my current course project.

## Recent Posts

{% raw %}
{% for post in site.posts %}
  <article class="post-preview">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    
    {% if post.excerpt %}
      <div class="post-excerpt">
        {{ post.excerpt | strip_html | truncatewords: 30 }}
      </div>
    {% endif %}
    
    <a href="{{ post.url }}" class="read-more">Read more →</a>
  </article>
  {% unless forloop.last %}<hr>{% endunless %}
{% endfor %}
{% endraw %}
