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
</style>

<!-- <div class="banner">
  <video autoplay muted loop>
    <source src="https://d2xch9q88t25k4.cloudfront.net/main-page-media/PC/mannacea.mp4" type="video/mp4">
  </video>
  <div class="content">
    <h1>Hello</h1>
  </div>
</div> -->

<div class="banner">
  <video autoplay muted loop>
    <source src="http://imjjong.woobi.co.kr/movie/cooking_oven.mp4" type="video/mp4">
  </video>
  <div class="content">
    <h1>흥미로운 즐거운 조리경험을 위한 UX Design</h1>
  </div>
</div>
