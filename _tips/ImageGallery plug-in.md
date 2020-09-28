---
date: "2020-07-25 12:45:07"
layout: tips
title: Image Gallery
description: 그냥 테스툥
image: /images/index/kitchen_design01.png
category: tips
tags:
  - jjong
author: JJong
paginate: false

galleries:
  - title: 좀되라구
    image: /images/test/cake.png
    url: /
  - title: Link to image gallery
    image: /images/test/candy.png
    url: /without-plugin/image-gallery
---

### Image gallery index

Index 단위로 불러오는 Gallery
Reference site : https://jekyllcodex.org/without-plugin/image-gallery-index/

{% if page.galleries %}{% include image-gallery-index.html %}{% endif %}

### Image Gallery

폴더 단위로 불러오는 Gallery
Reference site : https://jekyllcodex.org/without-plugin/image-gallery/

{% include image-gallery.html folder="/images/test/" %}
