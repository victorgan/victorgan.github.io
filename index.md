---
layout: default
title: Home
---
[Feed]({% post_url /atom.xml %})

{% for post in site.posts %}

{{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{{ post.excerpt }}

{% endfor %}
