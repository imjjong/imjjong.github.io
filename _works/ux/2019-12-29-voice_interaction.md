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

  <style>
    .container1 {
      display: -webkit-flex;
          display: flex;
          -webkit-flex-flow: row wrap;
          flex-flow: row wrap;

          max-width: 50rem;
          box-sizing: border-box;
          min-height: 150px;
          min-width: 150px;
          display: block;
    }
    .container3 {
          display: -webkit-flex;
          display: flex;
          -webkit-flex-flow: row wrap;
          flex-flow: row wrap;

          max-width: 50rem;
          box-sizing: border-box;
          min-height: 150px;
          min-width: 150px;
        }
        .f1, .f2, .f3{
          box-sizing: border-box;
          min-height: 150px;
          min-width: 150px;
          display: block;
        }

        @media (max-width: 768px){
          .f1, .f2, .f3{
              width: 100%;
            }
        }
        @media screen and (min-width: 768px) and (max-width: 1024px){
          .f1 {
            width: 50%;
           }

          .f4 {
            width: 50%;
            }
          }
          .container3{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            }
        }
         @media (min-width: 1024px) {
           .f1 {
            width: 50%;
           }
           .f2 {
            width: 50%;
           }
          .f3 {
            width: 100%;
            }
          .container3{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            }
         }
  </style>
</head>
<body>

<div class="container1" style="color: rgb(0, 119, 255); ">
  <div class="d1" style="background-color: #003476;">
    <div class="d2" style="background-color: #0062d2;">2
    </div>
    <div class="d3" style="background-color: #b4d2f7;">3
    </div>
  
  </div>
  <div class="d4" style="background-color: #d5dfef;">
    4
  </div>
</div>

<div class="container3" style="color: #EEEEEE; ">
  <div class="f1" style="background-image: url('/images/04.png');"></div>
  <div class="f4" style="background-color: #121212;">
    <div class="f2" style="background-color: #ffffff;"><h4>어떻게 보이지 않는 정보를 쉽게 전달할 것 인가?</h4>
    </div>
    <div class="f3" style="background-color: #000000;">3
    </div>
  </div>
</div>

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
