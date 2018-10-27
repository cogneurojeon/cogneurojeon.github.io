---
title: Blog
permalink: /news/
---

### **Latest Posts**

<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains 'blog' %}
    <div class="list-item">
      <h2 class="list-post-title">
        <a href="{{ site.baseurl }}{{ post.url }}">- {{ post.title }}</a> (<small>{{post.date | date: "%m/%d/%y" }}</small>)
      </h2>
      <p>{{ post.excerpt }}</p>
    </div>
    {% endif %}
  {% endfor %}
</div>
