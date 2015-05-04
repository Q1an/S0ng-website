---
layout : page
title : My Blog
tagline : blah blah blah
---
{% include JB/setup %}

A short list of blogs:
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

