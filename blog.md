---
layout: page
title: Blog
published: true
---










<div class="posts">
  {% for post in paginator.posts %}
  <div class="post">
    <span class="post-date indent">{{post.dateL}}</span>
    <h1 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>
    <a href='{{ site.baseurl}}/{{post.category}}' class='indent'>{{post.category}}</a>

    {% comment %}<span class="post-date">{{ post.date | date_to_string }}</span>{% endcomment %}
  <!--<span class="post-date">{{post.dateL}}</span>
  <span>{{post.category}}</span>-->
    <!--{{ post.content }}-->
  </div>
  {% endfor %}
</div>

<div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-item older" href="{{ site.baseurl }}/page{{paginator.next_page}}">Older</a>
  {% else %}
    <span class="pagination-item older">Older</span>
  {% endif %}
  {% if paginator.previous_page %}
    {% if paginator.page == 2 %}
      <a class="pagination-item newer" href="{{ site.baseurl }}/">Newer</a>
    {% else %}
      <a class="pagination-item newer" href="{{ site.baseurl }}/page{{paginator.previous_page}}">Newer</a>
    {% endif %}
  {% else %}
    <span class="pagination-item newer">Newer</span>
  {% endif %}
</div>
