---
layout: page
title: Blog
permalink: /blog/
---


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date | date: "%d" | plus:'0' }} {{ post.date | date: "%B %Y" }} - {{ post.title }}</a>
    </li>
  {% endfor %}
</ul>