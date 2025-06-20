---
layout: default
title: Blog
permalink: /blog/
---
{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <small>{{ post.date | date: "%d/%m/%Y" }}</small>
    <p>{{ post.excerpt | truncate: 160 }}</p>
  </article>
{% endfor %}