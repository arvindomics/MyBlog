---
layout: default
title: Home
---

# Welcome to my blog! ✨
Here you’ll find my latest posts below.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span style="font-size:0.9em; color:#888;"> — {{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
