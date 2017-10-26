---
layout: page
title: "All Photos"
permalink: "/photos/"
---

<!-- <section class="posts clear">
    <div class="section-title"><span>Recent Recipes</span></div>
    {% for post in site.posts limit: 10 %}
        <div class="post-content">
            <a href="{{ post.url | prepend: site.baseurl }}"><img src="{{ post.img }}" title="{{ post.title }}" alt="{{ post.title }}"></a>
        </div>
    {% endfor %}
</section> -->

<div>
  {% for post in site.posts %}
    <a href="{{ post.url | prepend: site.baseurl }}"><img src="{{ post.img_url }}" title="{{ post.title }}" alt="{{ post.title }}"></a>
  {% endfor %}
</div>
