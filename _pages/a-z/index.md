---
layout: page
title: "Recipe Index"
permalink: "/recipes/"
---
<div class = "index-list">
{% assign sorted_posts = site.posts | sort: 'indexed_ingredient' %}
<ul>
  {% for post in sorted_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
</div>
