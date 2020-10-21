---
date: 2019-11-26 16:43:28
layout: kitchen
title: "Kitchen design"
subtitle: Oven ux design in europe target
description: first design in samsung electronic
image: /images/index/kitchen_design01.png
optimized_image:
category: work
tags: oven
author: jjong
paginate: false
order: 1
---

<html>
    <head>
        <!-- 내가 만든 CSS 넣어보기 -->
      <!-- <link rel="stylesheet" href="/assets/css/ux/ux_post_common.css"/> -->
      <style>
        /* 구글 본고딕 웹폰트 불러오기 */
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@100;300;400;500;700;900&display=swap');

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
          min-height: 100px;
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
            .d1, .d2, .d3, .d4, .d5{
              width: 100%;
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
        /* Top left text */
        .oven-wrapper{
            /* margin-left: 24px; */
            background-color: black;
            color:#FFFFFF;
        }

        .post-description {
            position: relative;
            text-align: left;
            color: white;
        }
        .top-left {
            position: absolute;
            bottom: 3rem;
            right: 3rem;
        }

        .oven-wrapper .thumb-left{
            width: 50%;
            /* height: auto; */
            /* background-color: black; */
            background-image: url(/images/uk_lcd_oven/product.png);
            background-size: cover;
            background-position:top;
            margin-left: 24px;

        }

        .oven-wrapper .thumb-center{
            width: 100%;
            height: 400px;
            background-image: url(/images/uk_lcd_oven/control.png);
            background-size: cover;
            background-position:bottom;
        }

        </style>

    </head>

</html>

<div class="container1" style="color: #1d1d1f;  text-align: center;
font-family: 'Noto Sans KR','Roboto',sans-serif;">
    <div class="d1" style=" background-color: #fbfbfd; padding: 70px 0; min-height: 20rem;">
      <h1>🍴키친 디자인을 위한 <br> 유럽 식문화 조사</h1>
    </div>
    
    <div class="d2" style="background-color: #FFFFFF; color: #1d1d1F;"><p> 런던, 파리 현지 조사<br>
      구주 Microwave 원형 과제<br>
        시기 : 2016년 하반기<br>
        진행 내용 : 1. 구주 시장 영국, 프랑스의 현지 FGD(Focuss group design) 주방내에 Needs 파악<br> 2. 가정 방문(Home visit)을 실사용환경 파악과 진행하여 신규 UX컨셉을 발굴<br>
        효과 : 가격대별 3가지 군의 전략과 컨셉으로 제안 하였으며 전자레인지의 고정되어진 Form과 사용패턴에서 벗어난 새로운 형태에 컨셉을 제안함.
      </p>
    </div>
    <div class="d3" style="background-color: #b4d2f7;"><img src="/images/01.png">
    </div>
    <div class="d4" style="background-color: #d5dfef;">4
    </div>
    <div class="d5" style="background-color: #dfe1e5;">5
    </div>
  </div>

<div>
    <img src="/images/eu_food/research.png" style="width:100%;">
</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/lphzDnh2BxE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
17년형 구주 MWO 선행 발굴 리서치 진행(한국리서치, 영국, 프랑스)<br>
FGD 및 Home vist 전자레인지 리서치<br>
신규디자인을 위한 데이터 확보를 위해서 구주 현지에 방문하여 주거, 식문화 등의 라이프 스타일 조사

{% include image-gallery.html folder="/images/uk_mwo/" %}

<div class="oven-wrapper">
    
    <div class="text-and-img">
        <div class="thumb-left" style="margin-top: 48px;"></div>
        <div class="title">
            <div class="sub-title">2014. June 입사1년차</div>
            오븐<br>컨트롤패널<br>
            디자인
        </div>
    </div>   
    <div class="post-description">
        NV9900J LCD, Dual oven LED Dual 오븐 컨트로패널 디자인

        효과 : 신규 원형 과제로 LCD, LED 등 다양한 오븐 제품군을 파생에 대응할 수 있도록 고려한 디자인으로 현재까지 5년이상 판매되고 활용되고 있는 컨트폴패널 디자인으로 구주 뿐만아니라 국내 오븐 파생되어진 과제

        Full touch controls
        A 4.6" Full touch TFT-LCD control panel makes cooking much simpler and easier. You can intuitively select and control functions and settings—such as the cooking mode, temperature and time— with a simple touch of your finger.
    </div>


        <div class="thumb-center"></div>

    <div class="post-description">
        Wi-Fi cooking control
        Built-in Wi-Fi capabilities let you remotely monitor and control your Oven using just an app*. Easily adjust settings, receive notifications and download recipes by chefs with Michelin 3-star restaurants—all from your smartphone. *Available on iPhones and Android devices. A network connection is required.

        </div>

        <div class="post-description">
            <div class="thumb-center" style="background-image: url(/images/uk_lcd_oven/product5.png);"></div>
            <div class="top-left title" style="text-align: left;">

            요리를 쉽게<br> 도와주는<br>UI 디자인
            </div>
        </div>
    <div class="reference">

    </div>
    {% include image-gallery.html folder="/images/uk_lcd_oven" %}
    <div class="referenc">
        참고 링크 : https://www.samsung.com/uk/cooking-appliances/electric-ovens/
    </div>

</div>

#### 구주 오븐 LED 디자인

Intuitive step-by-step cooking guide
Guide Lighting Control
Enjoy a much simpler and more intuitive way to cook with the Guide Lighting Control. This digital dashboard lights each step on your path to a delicious meal. You can control temperature and time settings by zone, program recipes, select cooking functions and set cleaning options easily.

{% include image-gallery.html folder="/images/uk_dual_oven/" %}

<iframe width="100%" height="315" src="https://www.youtube.com/embed/4bmsWkYfLkE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

미주 Slide-in, Freestanding Gas 레인지 파생 디자인
시기 : 2015년 상반기
내용 : 파생디자인으로 Slide-in, Freestanding 등 다양한 미주레인지 파생디자인
효과 : 엔트리부터 미들에 가격대에 해당하는 제품군에 다양한 제품들에 대응하는 파생디자인을 대응하였음.
참고 링크 : https://www.samsung.com/us/home-appliances/ranges/all-ranges/?fuel_type=Gas

{% include image-gallery.html folder="/images/us_range/" %}

https://www.samsung.com/us/home-appliances/ranges/electric/5-8-cu-ft-slide-in-induction-range-with-virtual-flame--technology-in-black-stainless-steel-ne58r9560wg-aa/

미주 Wall-Oven Combi/Single 컨트롤패널 원형과제
시기 : 2016년 상반기
내용 : 미주 시장의 신규 도입되는 Wall-Oven의 원형 과제 진행
효과 : wall Oven의 다양한 모델(Single, Double, Combi)에 적합한 컨트로패널 원형디자인 수립함.
참고 링크 : https://www.samsung.com/us/home-appliances/wall-ovens/microwave-combination-oven/30-combination-microwave-wall-oven-nq70r5511dg-aa/
https://www.samsung.com/us/home-appliances/wall-ovens/

#### 2016. 입사 3년차

2014 - 2016 oven ux design in kitchen part
https://www.samsung.com/uk/cooking-appliances/

##### Wall Oven in US

30” Microwave Combination Wall Oven in Black Stainless Steel

Guiding light controls are intuitive, with simple step-by-step instructions for choosing cooking options.

https://www.samsung.com/us/home-appliances/wall-ovens/double/30-double-wall-oven-nv51r5511dg-aa/

https://www.samsung.com/us/home-appliances/wall-ovens/microwave-combination-oven/30--combination-microwave-wall-oven-nq70m6650dg-aa/

{% include image-gallery.html folder="/images/us_oven/" %}

Single Oven
Bake, broil and roast with precise heat for even cooking and fit multiple dishes.

Double Oven
Cook at different temperatures and fit all your dishes from a rack of cookies to a turkey roast.

Microwave Combination Oven
Give your leftovers a second life with the microwave or create a gourmet meal with the oven.

Oven in Europe

- 2014~2016년 : IOT 관련 다수 기기 UX디자인 설계 경험 있음 : 오븐, 에어컨, 전자레인지 등<br>

Easy-to-use interface

Analog knobs and a digital touch screen make it easy to control the oven. And with signature LED lights, you can check on your food without opening the door.

<div>

    {% include image-gallery.html folder="/images/cook-top/" %}

</div>

폴더 단위로 불러오는 Gallery

#### hood

<div class="post-description">
    
    <div class="bottom-left">Bottom Left</div>
    <div class="top-left">Top Left</div>
</div>

<div class="title" style="color: #1d1d1F">
    디자인 검증을 위한<br> 뉴욕 User Test 진행
    <div style="width:50%;">
        <img src="/images/newyork/intro.png">
    </div>
</div>

<div>
    16년형 북미 레인지 디자인 SCR 선행 과제
    북미 현지 UT 설계 및 실사 진행(한국리서치, 뉴욕)
    신규 실물 제품을 대상으로 FGD 진행을 통한 컨셉 검증
    
    미주 레인지 & OTR 컨트롤패널 일원화 신규컨셉 과제
    시기 : 2015년 하반기
    내용 : 레인지와 OTR 컨트롤 패널의 통합하는 신규 컨셉 과제로 미주 뉴욕 현지 실사 UT를 통한 상품성 및 사용성 검증 과제를 진행
    효과 : 신규 컨셉의 문제점과 사용성 이슈들을 실제적으로 소비자들에게 확인한 데이타를 기반으로 신규 컨셉에 문제점을 경영진에게 전달하여 도입에 재고가 설득하여 잘못된 디자인되어진 제품이 시장에 출시되는 것을 막음..
</div>

{% include image-gallery.html folder="/images/newyork/" %}
