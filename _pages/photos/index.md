---
layout: page
title: "All Photos"
permalink: "/photos/"
---

<div style="overflow: hidden;">
  <ul style="list-style-type: none">
    {% for post in site.posts %}
      <li>
      <a href="{{ post.url | prepend: site.baseurl }}">
        <div style="margin: 4px; float: left; background-image: url({{ post.img_url }}); background-size: cover; background-position: center; width: 190px; height: 190px;"></div>
      </a>
      </li>
    {% endfor %}
  </ul>
</div>

<!-- <div style="overflow: hidden;">
  <ul style="list-style-type: none">
    {% for post in site.posts offset: 3 limit: 12 %}
      <li>
      <div>
        <a href="{{ post.url | prepend: site.baseurl }}"><img style="overflow: hidden; width: 190px; height: 190px; float: left; padding: 5px;" src="{{ post.img_url }}" title="{{ post.title }}" alt="{{ post.title }}"></a>
      </div>
      </li>
    {% endfor %}
  </ul>
</div> -->
