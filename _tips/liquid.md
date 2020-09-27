---
date: 2015-09-06 12:00:00
layout: post
title: Liquid
subtitle: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
image: /images/index/kitchen_design01.png
optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559825288/theme17_nlndhx.jpg
category: tips
tags:
  - work
  - career
author: thiagorossener
---

liquid test

{{ post.title }}

<ul>
  {% for post in site.canvas %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    <img src="{{ post.image }}" width="100%">
    
  {% endfor %}
</ul>
