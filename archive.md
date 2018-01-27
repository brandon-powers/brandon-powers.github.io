---
layout: page
title: Archive
---

<div class="posts">
  {% for post in paginator.posts %}
  <div class="post">
    <h4 class="post-title">
      <a href="{{ site.baseurl }}/{{ post.url }}">
        {{ post.title }}
      </a>
    </h4>

    <span class="post-date">{{ post.date | date_to_string }}</span>
  </div>
  {% endfor %}
</div>