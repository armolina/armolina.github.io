---
layout: default
---

# Últimos posts
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }} ({{ post.date | date: "%Y/%m/%d" }})
        <p><a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a></p>
      </div>
    </article>
  {% endfor %}
</div>