---
date: "2020-07-25 12:45:07"
layout: tips
title: Text over image
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

<style>
    body{
        background-color: black;
        color: #ffffff
    }
   
    .container {
        position: relative;
        text-align: center;
        color: white;
    }
    .bottom-left {
        position: absolute;
        bottom: 8px;
        left: 16px;

    }
    /* Top left text */
    .top-left {
        position: absolute;
        top: 3rem;
        left: 3rem;
        font-size: 3rem;
    }
  
      /* Clear floats after the columns */
      .row:after {
        content: "";
        display: table;
        clear: both;
      }
      .center {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 25%;
      }
      .column {
        float: left;
        width: 50%;
      }

      .box{
        width:20%;
      }

</style>
<script>console.log("hello, world")</script>

<div class="container">
    <img src="/assets/img/2020-02-28-01-31-24.png" alt="Snow" style="width:100%;">
    <div class="bottom-left">Bottom Left</div>
    <div class="top-left">Top Left</div>
</div>I

### How to center Images

<div>
  <img src="/images/test/candy.png" class="center">
</div>

#### Grid of text and image

<div class="row">
  <div class="column">
    <h3> 직관적인 오븐 컨트롤패널 디자인
    </h3>
    <p style="color : #fff"> 사용 순서에 맞게 좌에서 우로 한 방향으로 디자인함
    </p>
  </div>
  <div class="column">
    <img src="/images/uk_dual_oven/Dual_Oven.png">
  </div>
</div>

<div class="row">
  <div class="column" style="text-align: right;">
    <h3>  text-align: right;
    </h3>
    <p style="color : #fff"> 사용 순서에 맞게 좌에서 우로 한 방향으로 디자인함
    </p>
  </div>
  <div class="column">
    <img src="/images/uk_dual_oven/Dual_Oven.png">
  </div>
</div>

<div class="row">
  <div class="column" style="text-align: justify;">
    <h3>  text-align: right;
    </h3>
    <p style="color : #fff"> 사용 순서에 맞게 좌에서 우로 한 방향으로 디자인함
    </p>
  </div>
  <div class="column">
    <img src="/images/uk_dual_oven/Dual_Oven.png">
  </div>
</div>

### DIV layout Basic

<div style="background-color: #212121;">
  <div class="box" style="background-color:#FFDE03;">
    <h2>Frist</h2>
  </div>
  <div class="box" style="background-color:#0336FF;">
    <h2>Second</h2>
  </div>
  <div class="box" style="background-color:#ff0266;">
    <h2>Third</h2>
  </div>
</div>

### DIV layout Float

<div style="background-color: #212121;  width:100%; height: 10rem;">
  <div class="box" style="background-color:#FFDE03;float:right;">
    <h2>Frist</h2>
  </div>
  <div class="box" style="background-color:#0336FF;float:right;">
    <h2>Second</h2>
  </div>
  <div class="box" style="background-color:#ff0266;float:right;">
    <h2>Third</h2>
  </div>
</div>

### DIV layout Float + Image

<div style="background-color: #212121; width: 100%; height: 15rem;;">
  <div class="box" style="background-color:#FFDE03;float:right;">
    <h2>Frist</h2>
  </div>
  <div class="box" style="background-color:#0336FF;float:right;">
    <h2>Second</h2>
  </div>
  <div class="box" style="background-color:#ff0266;float:right;">
    <h2>Third</h2>
  </div>
  <img src="/images/test/cheeze.png" class="box" style="float:left; height:auto; padding-left:5rem; width: 20%;">
  <p style="color:#ffffff;">기술의 발전 덕분에 지난 100년 동안 우리가 한 주당 가사 노동에 보내는 시간이 75% 정도, 시간으로 환산하면 매일 6시간 정도 줄어들었다고 합니다. 전기, 냉장고, 세탁기, 청소기 등의 가전제품들이 발명되면서 실생활에서 꼭 해야만 하는 육체노동의 상당 부분을 덜어준 셈입니다.

    그러나 1970년대부터 등장한 PC, 인터넷, 스마트폰 같은 기술의 진보 속도는 느려지고 있고, 생활 속에서 인지할 수 있는 혁신적인 변화도 크게 느껴지지 않습니다. 편리성은 커졌지만, 그만큼 공부하고 선택해야 할 것들이 많아 기술에 대한 피로도도 높아졌습니다. ‘정말, 우리 삶은 나아지고 있을까요?’</p>

</div>

### DIV layout dual type Float

<div style="background-color: #212121;  width:100%; height: 10rem;">
  <div class="box" style="background-color:#FFDE03;float:left;">
    <h2>Frist</h2>
  </div>
  <div class="box" style="background-color:#0336FF;float:right;">
    <h2>Second</h2>
  </div>
  <div class="box" style="background-color:#ff0266;float:left;">
    <h2>Third</h2>
  </div>
</div>

### DIV layout dual type+clear Float

<div style="background-color: #212121;  width:100%; height: 10rem;">
  <div class="box" style="background-color:#FFDE03;float:left;">
    <h2>Frist</h2>
  </div>
  <div class="box" style="background-color:#0336FF;float:right;">
    <h2>Second</h2>
  </div>
  <div class="box" style="background-color:#ff0266;clear :both;">
    <h2>Third</h2>
  </div>
</div>

<div style="background-color: #212121;  width:100%; height: 10rem;">
  <div class="box" style="background-color:#FFDE03;float:left;">
    <h2>Frist</h2>
  </div>
  <div class="box" style="background-color:#0336FF;float:right;">
    <h2>Second</h2>
  </div>
  <div class="box" style="background-color:#ff0266;clear :both;">
    <h2>Third</h2>
  </div>
</div>

position: relative;
아래와 같은 속성으 사용할 수 있게됨.
left
top
bottom

position: absolute;
부모가 가로 막지않으면 문서상 위치로 이동함
절대좌표

position: fixed;
스크롤되어도 해당자리에 위치하게됨

position: static;

부모에게 가두기 위해서 부모속성에
relatvie주깅

<img class="img-rounded" src="https://images.unsplash.com/photo-1508381592917-f70a660e413e?ixlib=rb-1.2.1&auto=format&fit=crop&w=1650&q=80" alt="Thiago Rossener" width="400" height="400">
