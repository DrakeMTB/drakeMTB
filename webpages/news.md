---
layout: page
title: Latest News!
permalink: /news/
---

<div class="postgrid gridposts">
  <div class="posts">
    {% for post in site.posts %}
    <article class="post">

      <h2>{{ post.title }}</h2>

        <div class="entry">
          {{ post.content | strip_html | truncatewords:25}}
        </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
</div>
