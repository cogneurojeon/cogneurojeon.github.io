---
title: Blog
permalink: /news/
---

## **Latest News**
<hr>

<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains 'blog' %}
    <div class="list-item">
      <h3 class="list-post-title">
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }} ({{post.date | date: "%m/%d/%y" }})</a> 
      </h3>
      <p>{{ post.excerpt }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>
