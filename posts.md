---
layout: default
title: "Posts"
---
<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {{ post.date | date: "%B %-d, %Y" }}
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>