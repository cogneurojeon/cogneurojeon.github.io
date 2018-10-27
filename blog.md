---
title: Blog
permalink: /news/
---

## **Latest News**
<hr>

<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains 'news' %}
    <div class="list-item">
      <h3 class="list-post-title">
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }} <small>({{post.date | date: "%m/%d/%y" }})</small></a> 
      </h3>
      <p>{{ post.excerpt }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>
