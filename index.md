---
layout: page
title: CoderCoop
tagline: Programming for Everyone
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <li><h3>{{ post.date | date_to_string }} &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h3> {{ post.content | split:"<!--more-->" | first }}</li>
  {% endfor %}
</ul>







