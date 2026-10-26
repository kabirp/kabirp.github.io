---
layout: default
permalink: /blog/
title: blog
description: Writing and guest posts on Kabir Peshawaria's personal website.
nav: true
nav_order: 1
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 10
  sort_field: date
  sort_reverse: true
  trail:
    before: 1
    after: 3
---

<div class="blog-index">
  <header class="blog-header">
    <h1>{{ site.blog_name }}</h1>
    <p>{{ site.blog_description }}</p>
  </header>

{% if page.pagination.enabled %}
{% assign postlist = paginator.posts %}
{% else %}
{% assign postlist = site.posts %}
{% endif %}

  <ul class="post-list">
    {% for post in postlist %}
      {% assign read_time = post.content | strip_html | number_of_words | divided_by: 200 | plus: 1 %}
      <li>
        <article aria-labelledby="post-{{ forloop.index }}">
          <p class="post-meta">
            <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%B %-d, %Y' }}</time>
            {% if post.guest_post %}&nbsp; &middot; &nbsp; Guest post{% endif %}
          </p>
          <h2 id="post-{{ forloop.index }}">
            <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>
          {% if post.description %}<p class="post-description">{{ post.description }}</p>{% endif %}
          <p class="post-meta">
            {% if post.author %}{{ post.author }} &nbsp; &middot; &nbsp;{% endif %}{{ read_time }} min read
          </p>
        </article>
      </li>
    {% endfor %}
  </ul>

{% if page.pagination.enabled %}{% include pagination.liquid %}{% endif %}

</div>
