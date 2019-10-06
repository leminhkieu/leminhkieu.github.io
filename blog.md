---
layout: main
title : Blog
header : Blog
group: navigation
---


## Recent posts

<ul class="posts">
            {% for post in site.posts offset: 0 limit: 6 %}
            <li>
            <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ base.url }}{{ post.url }}">{{ post.title }}</a><br/>
            <!-- {{ post.excerpt | strip_html | truncatewords:75 }} -->
            </li>
            {% endfor %}
        </ul>
        
 <br/>

More about me on my [Twitter](https://twitter.com/kieuleminh).

## All posts
        
<ul class="posts">
        {% for post in site.posts offset: 6 %}
            <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ base.url }}{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
</ul>