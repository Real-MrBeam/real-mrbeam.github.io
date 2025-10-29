---
layout: home
title: Blog
---

<ul>
{% for post in site.posts limit:5 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small>— {{ post.date | date: "%Y-%m-%d" }}</small>
    {% if post.excerpt %}<div>{{ post.excerpt }}</div>{% endif %}
  </li>
{% endfor %}
</ul>

<p><a href="/archive.html">View all posts →</a></p>
