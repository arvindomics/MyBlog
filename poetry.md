---
layout: default
title: "Poetry Collection ✨"
permalink: /poetry/
---

<h2>My Shayari & Poetry</h2>

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "poetry" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span style="font-size:0.9em; color:#888;">— {{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>
