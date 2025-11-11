---
layout: page
title: All Posts
permalink: /posts/
---

# All Posts

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p><small>{{ post.date | date: "%B %-d, %Y" }}</small></p>
  {% if post.excerpt %}
    <p>{{ post.excerpt | strip_html | truncate: 200 }}</p>
  {% endif %}
{% endfor %}
