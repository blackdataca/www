---
layout: content
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>

      <div class="date">
        {{ post.date | date: "%B %e, %Y" }}
      </div>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
