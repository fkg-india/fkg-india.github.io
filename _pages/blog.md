---
layout: single
title: "Blog"
permalink: /blog/
author_profile: false
related: false
toc: true
toc_label: "Posts"
toc_icon: "blog"
toc_sticky: true
articlecolour: "#00001a"
paginate: 5
paginate_path: "/page:num/"
---

<h1>Blog Posts</h1>

{% if paginator.posts %}
  {% for post in paginator.posts %}
    <div class="post">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </div>
  {% endfor %}
  
  <div class="pagination">
    {% if paginator.previous_page %}
      <a href="{{ paginator.previous_page_path }}">&laquo; Previous</a>
    {% endif %}
    <span>Page {{ paginator.page }} of {{ paginator.total_pages }}</span>
    {% if paginator.next_page %}
      <a href="{{ paginator.next_page_path }}">Next &raquo;</a>
    {% endif %}
  </div>
{% else %}
  <p>No blog posts found.</p>
{% endif %}