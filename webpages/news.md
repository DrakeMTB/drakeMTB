---
layout: page
title: Latest News!
stitle: news
permalink: /news/
---

<div class="postgrid gridposts">
  <div class="posts">
    {% for post in site.posts %}
    <article class="post">

      <h2>{{ post.title }}</h2>

        <div>
          {{ post.content | strip_html | truncatewords:50}}
        </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
</div>
