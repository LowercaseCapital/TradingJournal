---
layout: page
title: Blog
permalink: /blog/
---


<ul>
  {% for post in site.posts %}
      <h3><a href="{{site.baseurl}}{{ post.url }}">{{ post.date | date: "%d" | plus:'0' }} {{ post.date | date: "%B %Y" }} - {{ post.title }}</a></h3>
      <p>{{ post.excerpt | markdownify  }}</p>
      <p><a href="{{site.baseurl}}{{ post.url }}">Read More</a></p>
  {% endfor %}
</ul>