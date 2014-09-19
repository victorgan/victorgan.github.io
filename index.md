---
layout: default
title: Home
---
[<i class="fa fa-rss"></i>]({% post_url /atom.xml %})

{% for post in site.posts %}

{{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})

{% endfor %}
