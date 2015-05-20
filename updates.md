---
layout: page
title: "Updates"
group: navigation
---
{% include JB/setup %}
{% assign page_list = site.pages %}

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
