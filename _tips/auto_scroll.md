---
date: 2020-12-26 12:00:00
layout: tips
title: Auto scroll(full page)
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
<head>
  <style>
    .section {
  text-align:center;
  font-size: 3em;
}
  </style>
</head>
<body>
  <div id="fullpage">
    <div class="section">Section 1
      <img src="./45.png" alt="image_tset">
    </div>
    <div class="section">
      <div class="slide" data-anchor="slide1">Slide 2.1</div>
      <div class="slide" data-anchor="slide2">Slide 2.2</div>
    </div>
    <div class="section">Section 3</div>
    <div class="section">Section 4</div>
</div>

<script>
  new fullpage('#fullpage', {
  sectionsColor: ['yellow', 'orange', '#C0C0C0', '#ADD8E6'],
});
</script>
</body>

