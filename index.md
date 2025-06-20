---
layout: default
title: Safe Superintelligence Blog
---

<h1>Safe Superintelligence Blog</h1>
<p>Блог о самой важной технической задаче нашего времени.</p>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%d.%m.%Y" }}</span>
    </li>
  {% endfor %}
</ul> 