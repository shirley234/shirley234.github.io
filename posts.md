---
layout: default
title: "Posts"
---


<div class="row g-5 mb-5">
  <div class="col-md-12">
    <h3 class="fw-bold border-bottom pb-3 mb-5">{{ page.title }}</h3>
  </div>
</div>


<ul>
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      {{ post.date | date: "%B %-d, %Y" }}
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>