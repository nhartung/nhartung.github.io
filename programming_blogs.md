---
layout: page
title: Programming Blogs
subtitle: A collection of all of my blogs related to programming.
---

<ul class="posts">

  {% for post in site.posts %}
     {% if post.tags contains "programming" %}
       <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
     {% endif %}
  {% endfor %}
</ul>
