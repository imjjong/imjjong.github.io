---
date: "2020-08-26 12:45:07"
layout: tips
title: How to make slider
description: 그냥 테스툥
image: /images/index/kitchen_design01.png
category: tips
tags:
  - jjong
author: JJong
paginate: false

galleries:
  - title: 좀되라구
    image: /images/cake.png
    url: /
  - title: Link to image gallery
    image: /images/candy.png
    url: /without-plugin/image-gallery
---

  <head>
   
    <!-- 슬라이드 플러그인앱 -->
  <link rel="stylesheet" type="text/css" href="/assets/css/slick/slick.css" />
  <link rel="stylesheet" type="text/css" href="/assets/css/slick/slick-theme.css" />
    <style type="text/css">
      html,
      body,ul,ol {
        margin: 0;
        padding: 0;
      }

      * {
        box-sizing: border-box;
      }

      .slider {
        width: 90%;
        margin: 100px auto;
        padding-top: 24px;
      }

      .slick-slide {
        margin: 0px 20px;
      }

      .slick-slide img {
        width: 100%;
      }

      .slick-prev:before,
      .slick-next:before {
        color: black;
      }

      .slick-slide {
        transition: all ease-in-out 0.3s;
        opacity: 0.2;
      }

      .slick-active {
        opacity: 0.5;
      }

      .slick-current {
        opacity: 1;
      }
      .container {
        display: inline-grid;
        justify-items: stretch;
        width: 100%;
        gap: 10px;
        text-align: center;
        background-color: antiquewhite;
      }
      .item {
          background-color: rgb(50, 37, 175);
        }
      @media (min-width: 1024px){
        .slider {
        width: 980px;
        margin: 100px auto;

        }
        .container {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr 1fr;
        background-color: yellow;
        }
      }

      .container2 {
        display: grid;
        gap: 10px 10px;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: repeat(3, minmax(100px, auto));
        background-color: yellow;
      }
      .item2 {
        background-color: rgb(88, 175, 37);
        /* grid-column-start: 1;
        grid-column-end: 3;
        grid-row-start: 1;
        grid-row-end: 2; */
      }
      .item2:nth-child(1) {
        grid-column: 1 / 3;
        grid-row: 1 / 2;
        /* 1번 라인에서 2칸 */
        grid-column: 1 / span 1;
        /* 1번 라인에서 3칸 */
        grid-row: 1 / span 3;
      }
      .item2:nth-child(5) {
        /* 1번 라인에서 2칸 */
        grid-column: 3 / span 1;
        /* 1번 라인에서 3칸 */
        grid-row: 3 / span 2;
      }
      .container3 {
        display: grid;
        gap: 10px 10px;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: repeat(1, minmax(100px, auto));
        background-color: yellow;
      }
      .item3 {
        background-color: rgb(9, 86, 187);
      }

      .container4 {
        display: grid;
        gap: 10px 10px;
        grid-template-columns: 1fr 1fr;
        /* grid-template-rows: repeat(1, minmax(100px, auto)); */
        background-color: yellow;
      }
      .item4 {
        background-color: rgb(9, 86, 187);
      }
      .item4:nth-child(3) {
        /* 1번 라인에서 2칸 */
        grid-column: 2 / span 1;
        /* 1번 라인에서 3칸 */
        grid-row: 1 / span 2;
      }
      .container5 {
        display: grid;
        gap: 10px 10px;
        grid-template-columns: 1fr 1fr;
        /* grid-template-rows: repeat(1, minmax(100px, auto)); */
        background-color: yellow;
      }
      .item5 {
        background-color: rgb(9, 86, 187);
      }
      .item5:nth-child(1) {
        /* 1번 라인에서 2칸 */
        grid-column: 1 / span 1;
        /* 1번 라인에서 3칸 */
        grid-row: 1 / span 2;
      }
      .container6 {
        display: grid;
        gap: 10px 10px;
        grid-template-columns: 1fr 1fr 1fr;
        /* grid-template-rows: repeat(1, minmax(100px, auto)); */
        background-color: yellow;
      }
      .item6 {
        background-color: rgb(9, 86, 187);
      }
      .item6:nth-child(1) {
        /* 1번 라인에서 2칸 */
        grid-column: 1 / span 2;
        /* 1번 라인에서 3칸 */
        grid-row: 1 / span 2;
      }
    </style>


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
          <div class="item">E</div>
          <div class="item">F</div>
          <div class="item">G</div>
          <div class="item">H</div>
          <div class="item">I</div>
        </div>
      </div>
      <div>
        <div class="container2" style="height: 700px">
          <div class="item2">A</div>
          <div class="item2">B</div>
          <div class="item2">C</div>
          <div class="item2">D</div>
          <div class="item2">E</div>
          <div class="item2">F</div>
          <div class="item2">G</div>
          <div class="item2">H</div>
          <div class="item2">I</div>
        </div>
      </div>
      <div>
        <div class="container3" style="height: 700px">
          <div class="item3">A</div>
          <div class="item3">B</div>
        </div>
      </div>
      <div>
        <div class="container4" style="height: 700px">
          <div class="item4">A</div>
          <div class="item4">B</div>
          <div class="item4">C</div>
        </div>
      </div>
      <div>
        <div class="container5" style="height: 700px">
          <div class="item5">A</div>
          <div class="item5">B</div>
          <div class="item5">C</div>
        </div>
      </div>
      <div>
        <div class="container6" style="height: 700px">
          <div class="item6">A</div>
          <div class="item6">B</div>
          <div class="item6">C</div>
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
      src="/assets/js/slick/slick.js"
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
