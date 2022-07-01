---
layout: default
---

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}  - <span class="date">{{ post.date | date: "%d/%m/%Y" }}</span></a></h4>
    </article>
  {% endfor %}
</div>
