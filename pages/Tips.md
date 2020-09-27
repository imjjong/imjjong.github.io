---
layout: page
menu: true
date: "2019-12-30 01:01:0"
title: How to use the jekyll theme
permalink: /Tips/
description: Some description.
---


### {{ page.title }}



how to use Load Site
1. sudo gulp
2. sudo bundle exec jekyll serve 2>/dev/null


### list

<ul>
  {% assign posts = site.tips | where_exp:"post","post.is_generated != true" %} 
  {% for post in posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    <img class="img" data-aos="fade-in"  data-aos-delay="1000" url='https://source.unsplash.com/random' width="30%">
  {% endfor %}
</ul>