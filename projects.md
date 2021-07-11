---
layout: main
---

## Projects

I started reading regularly in Dec'2019 and have not stopped since. I enjoy fiction the most
but occasionally also try books around personal-development, biographies, etc.

I use this page to get myself into the habit of writing more. Below you can find
a list of my recommended books; books that I have read recently; and, some
random ramblings around the same.

I am quite active on as well.

---


### 项目 projects

<ul class="related-posts">

{% assign blog_posts = site.posts | where: 'projects', true %}
{% for post in blog_posts %}
        <li class="main-page-list">
            <h4>
            <a href="{{ post.goodreads_url }}">
                <span>{{ post.title }}</span>
            </a>
                <small>by {{ post.author }}.</small>
                <small>published {{ post.year }}.</small>
            </h4>
        </li>
        {% if forloop.last %}</ul>{% endif %}
{% endfor %}
