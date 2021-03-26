---
layout: page
title: Blog
permalink: /blog/
show_sidebar: true
hero_height: is-small
---

<div class="posts">
    {% for post in site.posts limit:5 %}
        <article>
            <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
            Published on {{ post.date | date_to_string }}
           {{ post.content }}
        </article>
    {% endfor %}
</div>