---
date: "2020-09-1 01:00:00"
layout: tips
title: layout_study_of_responsive_web
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
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@100;300;400;500;700;900&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap" rel="stylesheet">
    <style>

        .text_box{
            background-color: black;
            width: auto;
            /* 일정 이상 width 값이 커지 않도록 제한두기*/
            max-width: 50rem;
            padding: 0 1.25rem;
        }
        .container1 {
          display: -webkit-flex;
          display: flex;
          -webkit-flex-flow: row wrap;
          flex-flow: row wrap;

          max-width: 50rem;
          box-sizing: border-box;
          min-height: 150px;
          min-width: 150px;
        }
        .container2 {
          display: -webkit-flex;
          display: flex;
          -webkit-flex-flow: row wrap;
          flex-flow: row wrap;

          max-width: 50rem;
          box-sizing: border-box;
          min-height: 150px;
          min-width: 150px;
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
        .f1, .f2, .f3, .f4 {
          box-sizing: border-box;
          min-height: 150px;
          min-width: 150px;
          display: block;
        }


        @media (max-width: 768px){
            .text_box{
                background-color: gold;
                display: block;
            }
            .d1, .d2, .d3, .d4, .d5 {
          width: 100%;
            }
            .e1, .e2, .e3 {
              width: 100%;
            }
            .f1, .f4{
              width: 100%;
            }
        }

        @media screen and (min-width: 768px) and (max-width: 1024px){
            .text_box{
                background-color: blue;
                /* 아래 문장은 양쪽으로 자동 Margin값주기 */
                margin: 0 auto 0;
            }
            .d1{
              width: 100%;
            }
            .d2, .d3, .d4, .d5 {
           width: 50%;
          }

          .container1{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            }
          .e1 {
            width: 60%;
            -webkit-order: 2;
            order: 2;
            }

          .e2 {
            width: 40%;
            -webkit-order: 1;
            order: 1;
           }

          .e3 {
            width: 100%;
            -webkit-order: 3;
            order: 3;
           }
          .container2{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            }
          .f1 {
            width: 25%;
           }

          .f4 {
            width: 75%;
            }
          }
          .container3{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            }

        @media (min-width: 1024px) {
          .text_box{
            background-color:rgba(10, 185, 19, 0.493);
            margin: 0 auto 0;
            display: flex;
            justify-content: center;
          }
          .d1 {
              width: 60%;
            }
            .d2 {
              width: 40%;
            }
            .d3, .d4 {
            width: 33%;
            }
            .d5 {
            width: 34%;
            }
          .container1 {
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
          }
          .e1{
            width: 60%;
          }
          .e2 {
            width: 20%;
          }

          .e3 {
            width: 20%;
          }
          .container2{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
          }
          .f1 {
            width: 50%;
           }

          .f4 {
            width: 50%;
            }
          .container3{
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            }
        }

#font_apple{
line-height: 1.52381;
font-size: 21px;
font-weight: 500;
letter-spacing: .011em;
font-family:"SF Pro KR","SF Pro Display","SF Pro Icons","Apple Gothic","HY Gulim","MalgunGothic","HY Dotum","Lexi Gulim","Helvetica Neue","Helvetica","Arial",sans-serif;
}

.appleFont {
font-family: 'Noto Sans KR','Roboto',sans-serif;
}
</style>

</head>

Web의 Landscape대한 고민
https://material.io/resources/devices/
http://troy.labs.daum.net/
http://iosres.com/
반응형 범위 기준
mobie 768
pad 1024
PC
<br>

### Single Text box

<br>

<body>
  <div class="text_box" id="box_size">device_screen_size</div>
  <br>
  <div class="text_box" id="screen_size">browser_size</div>
  <br>
  <div class="text_box">text_area</div>

  <script>
    var box = document.getElementById('box_size');
    box.style.color = 'black';
    box.innerText = screen.width;

    var screen = document.getElementById('screen_size');
    screen.style.color = 'gold';
    
    function displayWindowSize(){
      screen.innerText = window.innerWidth;
}
window.addEventListener("resize", displayWindowSize);
    
  </script>
</body>

How to use code of the response web

```css
.text_box {
  background-color: black;
  width: auto;
  /* 일정 이상 width 값이 커지 않도록 제한두기*/
  max-width: 50rem;
  padding: 0 1.25rem;
}

@media (max-width: 768px) {
  .text_box {
    background-color: gold;
    display: block;
  }
}

@media screen and (min-width: 768px) and (max-width: 1024px) {
  .text_box {
    background-color: blue;
    /* 아래 문장은 양쪽으로 자동 Margin값주기 */
    margin: 0 auto 0;
  }
}
@media (min-width: 1024px) {
  .text_box {
    background-color: rgba(10, 185, 19, 0.493);
    margin: 0 auto 0;
    display: flex;
    justify-content: center;
  }
}
```

reference site : https://developers.google.com/web/fundamentals/design-and-ux/responsive/patterns?hl=ko

### 유동형 Mostly Fluid

<div class="container1" style="color: gold; ">
  <div class="d1" style="background-color: #003476;">1
  </div>
  <div class="d2" style="background-color: #0062d2;">2
  </div>
  <div class="d3" style="background-color: #b4d2f7;">3
  </div>
  <div class="d4" style="background-color: #d5dfef;">4
  </div>
  <div class="d5" style="background-color: #dfe1e5;">5
  </div>
</div>

### 열 끌어놓기 Column Drop

<div class="container2" style="color: rgb(0, 119, 255); ">
  <div class="e1" style="background-color: #003476;">1
  </div>
  <div class="e2" style="background-color: #0062d2;">2
  </div>
  <div class="e3" style="background-color: #b4d2f7;">3
  </div>
</div>

### 레이아웃 시프터 Layout shifter

<div class="container3" style="color: rgb(0, 119, 255); ">
  <div class="f1" style="background-color: #003476;">1
  </div>
  <div class="f4" style="background-color: #d5dfef;">
    <div class="f2" style="background-color: #0062d2;">2
    </div>
    <div class="f3" style="background-color: #b4d2f7;">3
    </div>
  </div>
</div>
