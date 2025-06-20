---
layout: default
title: Safe Superintelligence Blog
---

<div class="centered">
  <h1>Safe Superintelligence Blog</h1>
  <p>Блог о самой важной технической задаче нашего времени.</p>

  {% for post in site.posts %}
    <article class="post-preview">
      <h2>{{ post.title }}</h2>
      <p><em>{{ post.date | date: "%d.%m.%Y" }}</em></p>
      <div class="post-content">
        {{ post.content }}
      </div>
    </article>
  {% endfor %}
</div>
