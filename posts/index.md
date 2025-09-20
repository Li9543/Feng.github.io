---
layout: page
title: 所有文章
permalink: /posts/
---

<h2>📚 文章列表</h2>

<ul>
{% for post in site.posts %}
  <li>
    <span>{{ post.date | date: "%Y-%m-%d" }}</span>
    &nbsp;→&nbsp;
    <a href="{{ post.url }}">{{ post.title }}</a>
    <br>
    <small>{{ post.excerpt | strip_html }}</small>
  </li>
{% endfor %}
</ul>
