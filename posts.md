---
layout: default
title: Posts
permalink: /posts/
---

<header class="post-header">
  <h1 class="post-title">{{ page.title | escape }}</h1>
</header>


<ul>
  {% for post in site.posts %}
    <li>
      {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      <span class="post-meta">{{ post.date | date: date_format }}</span>

      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </li>

  {% endfor %}
</ul>
