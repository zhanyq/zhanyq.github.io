---
layout: home
title: Blog-test
permalink: /blog/
---
Welcome to my blog! Here are my latest posts:

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}
