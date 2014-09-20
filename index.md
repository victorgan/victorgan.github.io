---
layout: default
title: Home
---
[<i class="fa fa-rss"></i>](/about.xml)
[<i class="fa fa-linkedin"></i>](https://www.linkedin.com/in/victorgan)
[<i class="fa fa-github"></i>](https://github.com/victorgan)

                    <li><a href="/"><i class="fa fa-globe fa-2x"></i></a> </li>
                    <li><a href="#"><i class="fa fa-envelope fa-2x"></i></a> </li>
                    <li><a href="#"><i class="fa fa-linkedin fa-2x"></i></a> </li>
                    <li><a href="#"><i class="fa fa-github fa-2x"></i></a> </li>
                    <!-- <li><a href="#"><i class="fa fa-pinterest fa-2x"></i></a> </li> -->
                    <!-- <li><a href="#"><i class="fa fa-bitbucket fa-2x"></i></a> </li> -->
                    <li><a href="#"><i class="fa fa-twitter fa-2x"></i></a> </li>
                    <!-- <li><a href="#"><i class="fa fa-stack-exchange fa-2x"></i></a> </li> -->


{% for post in site.posts %}

{{ post.date | date_to_string }} - [ {{ post.title }} ]({{ post.url }})

{% endfor %}
