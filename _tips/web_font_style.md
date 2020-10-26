---
date: "2020-10-21 01:00:00"
layout: tips
title: Web Font Style Study
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
  body{
    font-family: 'Noto Sans KR', sans-serif;
  }
  
  .text_box{
    max-width: 50rem;
    padding: 0 1.25rem;
    padding-bottom: 1.25rem;
    background-color: gray;
    width: auto;
    /* 부드럽게 폰트 표현하기 */
    -webkit-font-smoothing: antialiased;
    /* 줄 바꿈 시, 단어 단위로 끊어주는 역할 */
    word-break: keep-all;
    font-family: 'Noto Sans KR', sans-serif;
  }

  h1, h2, h3, p{
    height: 1.1875;
    background-color: rgba(247, 247, 247);
    font-weight: 700;
    letter-spacing: 0em;
  }
    /* Mobile */
    @media (max-width: 768px) {
      .text_box {
      background-color: gold;
      display: block;
      }
      h2{
        font-size: 48px;
      }
    }

    /*  Tablet*/
    @media screen and (min-width: 768px) and (max-width: 1024px) {
      .text_box {
        background-color: rgb(82, 163, 240);
        margin: 0 auto 0;
      }
      h2{
        font-size: 56px;
      }
      p{
        font-size: 56px;
      }
    }

    /* PC */
    @media (min-width: 1024px) {
      .text_box {
      background-color: rgb(226, 55, 92);
      margin: 0 auto 0;
      max-width: 50rem;
      justify-content: center;
      }
      h2{
        font-size: 80px;
      }
    }

.bongodic{
font-size: 30px;
height: 4rem;
background-color: rgba(247, 247, 247);
}

</style>
</head>
### 본고딕 Font Weight Type

<button onclick="myFunction()">Click Me</button>


<div id="myDIV" class="text_box">
  <h3 style="padding-left: 0px; padding-bottom: 20px;">본고딕 종류</h3>
  <div class="bongodic" style="font-weight: 100;">본고딕 Thin 100입니다.</div>
  <div class="bongodic" style="font-weight: 300;">본고딕 Light 300입니다.</div>
  <div class="bongodic" style="font-weight: 400;">본고딕 Reqular 400입니다.</div>
  <div class="bongodic" style="font-weight: 500;">본고딕 Medium 500입니다.</div>
  <div class="bongodic" style="font-weight: 700;">본고딕 Bold 700입니다.</div>
  <div class="bongodic" style="font-weight: 900;">본고딕 Black 900입니다.</div>
</div>

<br>
<br>
### 글자의 속성
```css
.text_box{
<!-- 부드럽게 폰트 표현하기 -->
-webkit-font-smoothing: antialiased;

<!-- 줄 바꿈 시, 단어 단위로 끊어주는 역할 -->

word-break: keep-all;

<!-- 글자 사이의 간격은 letter-spacing -->

letter-spacing: 0px;
letter-spacing: -5px;

<!-- 단어 사이의 간격은 word-spacing -->

word-spacing: -20px;
word-spacing: 0px;

<!-- 줄 간격을 조절하는 속성 -->

line-height: 1.20455;

<!-- 문단 정렬 방식을 정하는 속성은 text-align -->

text-align: left;
text-align: right;
text-align: center;
text-align: justify;

<!-- 글자의 방향을 정하는 속성 -->

direction: rtl

<!-- 글자 굵기 정하는 속성 -->

font-weight: 600;

<!-- 글자 색깔 -->

color: #1d1d1f;

}

````
### 화면의 가로 사이즈에 맞는 폰트 크기
<table>
  <thead>
    <tr>
      <th>Type</th>
      <th>Mobile</th>
      <th>Tablet</th>
      <th>PC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>H1</td>
      <td>34.6</td>
      <td>36</td>
      <td>37.3</td>
    </tr>
    <tr>
      <td>H2</td>
      <td>26.6</td>
      <td>28</td>
      <td>29.3</td>
    </tr>
    <tr>
      <td>H3</td>
      <td>24</td>
      <td>25.3</td>
      <td>26.6</td>
    </tr>
    <tr>
      <td>P</td>
      <td>20</td>
      <td>21.3</td>
      <td>22.6</td>
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

<div id="myDIV" class="text_box">
  <h3 style="padding-left: 0px; padding-bottom: 20px;">본고딕 크기</h3>
 
  <div><h1 id="h1_size">H1 스피드 그 이상의 스피드.</h1></div>
  <div><h2 id="h2_size">H2 스피드 그 이상의 스피드.</h2></div>
  <div><h3 id="h3_size">H3 스피드 그 이상의 스피드.</h3></div>
  <div><p id="p_size">H3 스피드 그 이상의 스피드.</p ></div>
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


#### 애플 사이트 속성
```css
color #8c8c8c
font-size rem(16px)
font-weight 700
line-height 1.45
letter-spacing -0.015rem
font-family "SF Pro Text","SF Pro Icons","Helvetica Neue","Helvetica","Arial",sans-serif
-webkit-font-smoothing antialiased

````

#### 참고사이트

<br>
reference<br>
https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/typography/
<br>
https://fonts.google.com/specimen/Noto+Sans+KR?selection.family=Noto+Sans+KR&sidebar.open=true
<br>
https://developer.apple.com/fonts/
<br>

<script>
  function myFunction() {
    var x = document.getElementById("myDIV");
    if (x.style.display === "none") {
      x.style.display = "block";
    } else {
      x.style.display = "none";
    }
  }
  function font_size(){
    var h1 = document.getElementById("h1_size");
    console.log(h1.style.fontSize);
  }
  font_size();
</script>
