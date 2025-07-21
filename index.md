---
layout: home
title: ElektrikDepo Blog
---

# ElektrikDepo Blog

Hoş geldiniz! Aşağıda en güncel blog yazılarımızı bulabilirsiniz:

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
    <small>{{ post.date | date: "%d %B %Y" }}</small>
  </article>
{% endfor %}