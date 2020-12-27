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
  <script src="https://code.jquery.com/jquery-3.5.1.min.js" integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0=" crossorigin="anonymous"></script>
  <style>

    .section {
      color : white;
  text-align:center;
  font-size: 3em;
 }
 .s0{
   background-image: url('./45.png');
   background-size: cover;
 }

 /* 네비게이션 버튼 색깔 변경하기 */
 #fp-nav ul li a span{
   background-color: #fff;
 }

 .s01 sub{
   display: none;
 }
  </style>
</head>
<body>
  <div id="fullpage">
    <div class="section s0">Section 1
    </div>
    <div class="section s01">
      <div class="slide" data-anchor="slide1">
        <h2>Slide 2.1</h2>
        <sub>Timening visiable</sub>
      </div>
      <div class="slide" data-anchor="slide2">Slide 2.2</div>
    </div>
    <div class="section s02">Section 3</div>
    <div class="section s03">Section 4</div>
</div>


<script>
  new fullpage('#fullpage', {
  sectionsColor: ['yellow', 'orange', '#C0C0C0', '#ADD8E6'],
  navigation: true,
  navigationTooltips:['home', 'about','contact','xtras'],
  scrollingSpeed: 800,
  onLeave: function(origin, destincation, direction){
    console.log('onleave', origin.index, destincation.index);
    if(origin.index == 1){
      $('.s01 sub').hide();
    }
  },
  afterLoad: function(origin, destincation, direction){
    console.log('afterLoad')
    if(destincation.index == 1){
      $('.s01 sub').show();
    }
  }
});
  
</script>
</body>

