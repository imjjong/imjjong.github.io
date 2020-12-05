---
date: "2019-11-29 12:45:07"
layout: tips
title: Text over full background-video
description: 그냥 테스툥
image: /images/index/kitchen_design01.png
category: tips
tags:
  - jjong
author: JJong
paginate: false
---

이것은 무엇이오 웹에서 입력가능하옹? 뭐짐 이제되

<style>
  body{
    background: black;
  }
  .banner{
    width: auto;
    height: auto;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .banner video{
    position: absolute;
    top: 0;
    left: 0;
    object-fit: cover;
    width: 100%;
    height: 100%;
    pointer-events: none;
  }
  .banner .content{
    position: relative;
    z-index: 1;
    max-width : 1000px;
    margin: 0 auto;
    text-align: center;
  }
  .banner .content h1{
    margin: 0;
    padding: 0;
    font-size: 4.5rem;
    text-transform: uppercase;
    color: #fff;
  }
  .bannerd iframe {
    
    
   position: absolute;
    top: 0;
    left: 0;
    object-fit: cover;
    width: 100%;
    height: 100%;
    pointer-events: none;
}
 .banner iframe{
    
   width: 100%;
   /* height: 100%; */
   height: 56.25vw; 
   /* Given a 16:9 aspect ratio, 9/16*100 = 56.25 */
   min-height: 100vh;
   min-width: 177.77vh; /* Given a 16:9 aspect ratio, 16/9*100 = 177.77 */
   position: absolute;
   top: 50%;
   left: 50%;
   transform: translate(-50%, -50%);
   
}
</style>

<div class="banner">
  <video autoplay muted loop>
    <source src="http://imjjong.woobi.co.kr/movie/cooking_oven.mp4" type="video/mp4">
  </video>
  <div class="content">
    <h1>Hello</h1>
  </div>
</div>
<!-- 
<div class="banner">
    <iframe src="http://imjjong.woobi.co.kr/movie/cooking_oven.mp4"
           frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen ></iframe>
  <div class="content">
    <h1>흥미로운 즐거운 조리경험을 위한 UX Design1</h1>
  </div>
</div> -->

<iframe src="https://player.vimeo.com/video/149915506?color=00ccff&title=0&byline=0&portrait=0" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

<p><a href="https://vimeo.com/149915506">Drone</a> from <a href="https://vimeo.com/skyless">Skyless Productions</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

http://imjjong.dothome.co.kr/cooking_oven.mp4
https://player.vimeo.com/video/76979871?background=1&autoplay=1&loop=1&byline=0&title=0
