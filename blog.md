---
layout: page
title: Blog
permalink: /blog/
---

# Blog

{% for post in site.posts %}
<article class="post-list-item">
  <p class="eyebrow">{{ post.date | date: "%Y.%m.%d" }}</p>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
</article>
{% endfor %}
