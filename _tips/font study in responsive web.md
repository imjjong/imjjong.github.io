---
date: "2020-09-1 01:00:00"
layout: tips
title: Font study in responsive Web
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


        @media (max-width: 37.5rem){
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

        @media screen and (min-width: 37.5rem) and (max-width: 1024px){
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
font-family:"SF Pro KR","SF Pro Display","SF Pro Icons","Apple Gothic","HY Gulim","MalgunGothic","HY Dotum","Lexi Gulim","Helvetica Neue","Helvetica","Arial",sans-serif;
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

@media (max-width: 37.5rem) {
  .text_box {
    background-color: gold;
    display: block;
  }
}

@media screen and (min-width: 37.5rem) and (max-width: 1024px) {
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

<br>
<div id="font_apple">
  P tag<br>
  A14 Bionic을 탑재했다는 건, 당신의 아이디어에 생명력을 불어넣을 파워를 갖췄다는 뜻이죠. 4K 동영상 촬영부터 편집까지 모두 하나의 기기에서 처리할 수 있습니다. 또한, 2세대 Apple Pencil의 역동적인 브러시와 섬세한 음영 표현을 활용해 순수 회화에서 상업 일러스트 작업까지 가능하죠.1 여기에 A14 Bionic의 향상된 그래픽과 머신 러닝 성능이 사진 편집, 작곡 등 다양한 분야에 걸쳐 새로운 창작의 가능성을 한껏 열어줍니다.
</div>

<br>
reference<br>
https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/typography/
<br>

<table>
  <thead>
    <tr>
      <th>Type</th>
      <th>Mobile</th>
      <th>Tablet</th>
      <th>PC</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>H1</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>H2</td>
      <td>10</td>
      <td>44</td>
      <td>44</td>
    </tr>
    <tr>
      <td>H3</td>
      <td>4</td>
      <td>3</td>
      
    </tr>
    <tr>
      <td>P</td>
      <td>7</td>
      <td>17</td>
      <td>17</td>
    </tr>
    <tr>
      <td>line-height</td>
      <td>1</td>
      <td>2</td>
      <td>line-height: 1.58824;</td>
    </tr>
    <tr>
      <td>letter-spacing</td>
      <td>1</td>
      <td>2</td>
      <td>letter-spacing: 0em;</td>
    </tr>
  </tbody>
</table>

<div class="appleFont" style="
-webkit-font-smoothing: antialiased;
direction: ltr;
text-align: left;
margin: 0;
padding: 0;
color: #1d1d1f;
font-style: normal;
word-break: keep-all;
font-size: 44px;
font-weight: 600;
line-height: 1.20455;
letter-spacing: 0em;">
  개인정보 보호
</div>

<div class="appleFont" style="color: #1d1d1f;
-webkit-font-smoothing: antialiased;
direction: ltr;
text-align: left;
margin: 0;
padding: 0;
font-style: normal;
word-break: keep-all;
font-size: 17px;
font-weight: 400;
line-height: 1.58824;
letter-spacing: 0em; max-width: 50rem;">
다른 모든 Apple 제품과 마찬가지로 iPad Air 역시 당신의 개인정보 보호 및 보안을 염두에 두고 설계되었습니다. 결코 쉽지만은 않은 작업이죠. 하지만 그런 것만이 진정한 혁신이라 우리는 믿습니다.
</div>

Font
Rem 단위로 하자!
https://offroadcode.com/rem-calculator

Html font-size 16px 기준
8px = 0.5rem
9px = 0.5625rem
10px = 0.625rem
11px = 0.6875rem
12px = 0.75rem
13px = 0.8125rem
14px = 0.875rem
15px = 0.9375rem
16px = 1rem (base)
18px = 1.125rem
20px = 1.25rem
22px = 1.375rem
24px = 1.5rem
26px = 1.625rem
28px = 1.75rem
30px = 1.875rem
32px = 2rem
34px = 2.125rem
36px = 2.25rem
38px = 2.375rem
40px = 2.5rem
참고사이트 : https://yeoninim.tistory.com/38

<div style="color: #1d1d1F; font-size: 5rem;font-weight: 700; line-height: 1.05; letter-spacing: -0.015rem; margin-left:24px;-webkit-font-smoothing: antialiased;">
H0 키친 디자인을 위한<br> 유럽 식문화 조사
</div>

# H1 키친 디자인을 위한<br> 유럽 식문화 조사

font-size rem(56px) color #1d1d1F line-height: 1.08

## H2 키친 디자인을 위한<br> 유럽 식문화 조사

font-size rem(48px) color #1d1d1F line-height: 1.09

### H3 키친 디자인을 위한<br> 유럽 식문화 조사

font-size rem(40px) color #1d1d1F line-height: 1.10

#### H4 키친 디자인을 위한<br> 유럽 식문화 조사

font-size rem(32px) color #1d1d1F line-height: 1.11

##### H5 키친 디자인을 위한<br> 유럽 식문화 조사

font-size rem(24px) color #1d1d1F line-height: 1.12

###### H6 키친 디자인을 위한<br> 유럽 식문화 조사

font-size rem(16px) color #1d1d1F line-height: 1.13

Normal 일반글 사이즈

# 사진 못 찍기가 이렇게 어렵습니다.

완전히 새로운 듀얼 카메라 시스템. 와이드 카메라에서 울트라 와이드 카메라까지, 사진 촬영에 있어 당신의 지평이 더욱 넓어집니다. 새롭게 설계된 인터페이스는 새로운 울트라 와이드 카메라를 활용하여 프레임 밖의 장면까지도 보여주고, 필요하면 그 조차도 카메라에 담을 수 있게 해줍니다. 게다가 동영상은 촬영도, 편집도 사진 다루듯 손쉽게 할 수 있죠. 세상에서 가장 사랑받는 카메라에 이제 새로운 시각이 더해졌습니다.
P Font Css------------------------------------

color #8c8c8c
font-size rem(16px)
font-weight 700
line-height 1.45
letter-spacing -0.015rem
font-family "SF Pro Text","SF Pro Icons","Helvetica Neue","Helvetica","Arial",sans-serif
-webkit-font-smoothing antialiased
