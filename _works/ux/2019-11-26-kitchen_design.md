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

Hello, Kitchen

<head>
    <style>

        .text_box{
            background-color: black;
            width: auto;
            /* 일정 이상 width 값이 커지 않도록 제한두기*/
            max-width: 50rem;
            padding: 0 1.25rem;
        }

        @media (max-width: 37.5rem){
            .text_box{
                background-color: gold;
                display: block;
            }
        }

        @media screen and (min-width: 37.5rem) and (max-width: 1024px){
            .text_box{
                background-color: blue;
                /* 아래 문장은 양쪽으로 자동 Margin값주기 */
                margin: 0 auto 0;
            }
        }
        @media (min-width: 1024px) {
            .text_box{
                background-color:rgba(10, 185, 19, 0.493);
                margin: 0 auto 0;
                display: flex;
                justify-content: center;
            }
        }

        /* 'phone': 320px,

'tablet': 768px,
'desktop': 1024px \*/
</style>

</head>
<section>
    <article role="article" class="post-content">
        <div class="text_box">text_area</div>
    </article>
    <div id="red_box">text_area</div>
</section>
