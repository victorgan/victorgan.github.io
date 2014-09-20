---
layout: default
title: Home
---
[<i class="fa fa-rss"></i>](/about.xml)

{% for post in site.posts %}

{{ post.date | date_to_string }} - [ {{ post.title }} ]({{ post.url }})

{% endfor %}
