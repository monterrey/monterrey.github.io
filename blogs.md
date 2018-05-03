---
layout: page
title: Blog
permalink: /blog/
---
<div class="container">
I will list my blogs here

<ul class="list-group">
  {% for post in site.posts %}

      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <a class="post-link list-group-item" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>


  {% endfor %}
</ul>
</div>
