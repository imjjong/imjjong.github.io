---
date: "2019-12-29 12:45:07"
layout: post
title: Voice Interation design
description: MWo, OTR design
image: /images/index/voice-interaction01.png
category: work
tags:
  - jjong
author: JJong
paginate: false
# 아래 문장은 html output할지 여부 결정
published: ture
order: 3
---

<h3>Voice Guide Principle 작성</h3>
<h3>Hands free design</h3>
<head>
  <link rel="stylesheet" type="text/css" href="/assets/slick/slick.css" />
  <link rel="stylesheet" type="text/css" href="/assets/slick/slick-theme.css" />
</head>
<body>

<iframe width="560" height="315" src="https://www.youtube.com/embed/3LwJQt_uIX4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

https://www.behance.net/gallery/103245823/SAMSUNG-Bixby-X-Language-education?tracking_source=search_projects_recommended%7Cbixby

https://www.behance.net/gallery/102088625/Samsung-Bixby-Voice-Forever?tracking_source=search_projects_recommended%7Cbixby

https://www.behance.net/gallery/72492973/Common-Voice?tracking_source=search_projects_recommended%7Cvoice%20design

https://good-design.org/projects/samsung-family-hub-5-0/

http://design.samsung.com/global/contents/family_hub/

<div class="text_box" style="text-align: center;">
  <h4>Hands-free control</h4>
  <p>Use Bixby on your Galaxy phone to control your smart devices by voice.
Adjusting the temperature or playing music is as simple as saying it.</p>
  <video width="100%" height="20%" controls>
  <source src="https://images.samsung.com/is/content/samsung/assets/us/smart-things/mobile/P6_Smart-Home-PFS_Bixby_M.mp4" type="video/mp4">
  </video>
</div>

<section class="regular slider" style=" background-color: gray">
  <div>
    <div style="width: 100%; height: 100px; background: red">1</div>
    <div style="width: 100%; height: 70px; background: blue">2</div>
    <div style="width: 100%; height: 70px; background: green">3</div>
  </div>
  <div>
    <div class="container" style="height: 700px">
      <div class="item">A</div>
      <div class="item">B</div>
      <div class="item">C</div>
      <div class="item">D</div>
    </div>
  </div>
  
   
  <div>
    <img src="http://placehold.it/350x300?text=6" />
  </div>
</section>

<script
      src="https://code.jquery.com/jquery-2.2.0.min.js"
      type="text/javascript"
    ></script>

    <script
      src="/assets/slick/slick.js"
      type="text/javascript"
      charset="utf-8"
    ></script>
    <script type="text/javascript">
      $(document).on("ready", function () {
        $(".regular").slick({
          dots: true,
          infinite: true,
          slidesToShow: 1,
          slidesToScroll: 1,
          adaptiveHeight: true,
        });
      });

</script>
</body>
