---
layout: post
title: Blog
permalink: /blog/
navigation_weight: 5
---

<div class="home">

 
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        {{post.content}}
      </li>
    {% endfor %}

  </ul>


</div>
