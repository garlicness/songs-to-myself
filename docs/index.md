---
layout: default
---

## Les chansons

<div class="posts">
  {% assign sorted_posts = site.posts | sort: "date" | reverse %}
  {% for post in sorted_posts %}
    <article class="post">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}  - <span class="date">{{ post.date | date: "%d/%m/%Y" }}</span></a></h4>
    </article>
  {% endfor %}
</div>

## Une nouvelle

<https://github.com/garlicness/quand-manigancent-les-haricots/releases/latest>
Pour télécharger cliquer sur Asset - Epub book
