---
layout: page
title: I was thinking ...
tagline: (Uh-oh. Here we go again.)
---
{% include JB/setup %}
{% assign posts_collate = site.posts %}
{% include JB/posts_collate %}

<h2>The Posts are below.</h2>
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


