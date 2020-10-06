---
date: "2019-11-29 12:45:07"
layout: tips
title: Wow Animation
description: 그냥 테스툥
image: /images/index/kitchen_design01.png
category: tips
tags:
  - jjong
author: JJong
paginate: false
---

<head>
  <link rel="stylesheet" href="/assets/wow_animate/animate.css">
  <script src="/assets/wow_animate/wow.min.js"></script>
  <script>
  new WOW().init();

</script>

</head>

<body>
  <style>
    .boxStyle{
      width: 100px;
      height: 100px;
      background-color:#F5F5F7;
      border-radius: 20px;
      left: 100px;
    }
    </style>
<h1>How to use the WOW Animate</h1>
<p>Reference site : https://wowjs.uk/</p>

<br>
<h5 style="color: #0f44a7">animated bounce delay-2s</h5>
<div class="boxStyle">animated<br>bounce<br>delay-2s</div>

<br>
<h5 style="color: #0f44a7">animated bounce delay-2s</h5>
<div class="boxStyle">animated<br>bounce<br>delay-2s</div>

<h1 class="animated bounce delay-2s">H1</h1>
<h2 class="wow bounceInUp">H2</h2>
<h3 class="wow slideInLeft" data-wow-duration="2s" data-wow-delay="5s">H3</h3>
<h4 class="wow bounceInUp">H4</h4>
<h5 class="wow bounceInUp">H5</h5>
<h6 class="wow slideInLeft" data-wow-duration="2s" data-wow-delay="5s">H6</h6>

<h2 data-wow-delay="5s" class="wow FadeIn">날아가세</h2>
<h2 data-wow-delay="10s" class="wow FadeOut">날아가세</h2>
<h2 class="wow bounceInUp">애니메이션 WOW</h2>

<div class="wow bounceInUp">
Content to Reveal Here
</div>

### Scroll Animation
