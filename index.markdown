---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Camer Scrapes
---

<div class="posts">
    {% for post in site.posts %}
        <article>
            <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
            Published on {{ post.date | date_to_string }}
            {{ post.excerpt }}
        </article>
    {% endfor %}
</div>