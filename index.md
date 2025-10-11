---
layout: default
title: "Home"
---

<h2>Welcome to my blog! ✨</h2>
<p>Here you’ll find my latest science stories and thoughts — not poetry.</p>

<div class="post-list">
  {% for post in site.posts %}
    {% unless post.categories contains "poetry" %}
      <article class="post-content">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
        <div>{{ post.excerpt }}</div>
      </article>
    {% endunless %}
  {% endfor %}
</div>
