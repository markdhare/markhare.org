---
layout: default
title: Writing
permalink: /writing/
description: Articles and short notes by Mark Hare.
---

<header class="page-header">
  <p class="eyebrow">Archive</p>
  <h1>Writing</h1>
  <p>Articles, observations, and notes.</p>
</header>

<ol class="post-list archive-list">
  {% for post in site.posts %}
    <li>
      <article>
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        {% if post.description %}<p>{{ post.description }}</p>{% endif %}
      </article>
    </li>
  {% endfor %}
</ol>

