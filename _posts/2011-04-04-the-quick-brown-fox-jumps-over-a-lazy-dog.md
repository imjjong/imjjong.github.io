---
date: 2018-10-09 12:26:40
layout: post
title: The quick brown fox jumps over a lazy dog
subtitle: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_760/v1506079212/jekflix-capa_vfhuzh.png
optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1506079212/jekflix-capa_vfhuzh.png
category: css
tags:
  - css
  - tips
author: thiagorossener
---

<ul>
{% for member in site.data.book.members %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>

<p>
{% assign sorted = site.works | sort: 'order' %}

{% for featured in sorted  %}
{{ featured.title }} hi

  <section class="hero" style="background-image: url({{ featured.image }})"></section>
{% endfor %}
</p>

Hello fuck
