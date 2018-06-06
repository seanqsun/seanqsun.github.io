---
layout: post
permalink: /blog/
title: blog
command: ls -l
---

### total {{ site.posts | size }}
<div class="posts">
  {% assign sorted = site.posts | sort: 'date' %}
  {% for post in sorted %}
    <article class="post">

      <h5>{{ post.description }}</h5>

      <a href="{{ site.baseurl }}{{ post.url }}" class="link2">Read</a>
    </article>
  {% endfor %}
</div>

<hr>

