---
layout: photography_2020
title:  "“疫情中的我们” 摄影大赛获奖名单揭晓！"
date:   2020-11-22 00:00:00 +0800
dateStr: "Nov. 22, 2020"
thumbnail: "/assets/by_year/fa2020-sp2021/photography/cover.jpg"
brief: "谢谢大家参与“疫情中的我们” 摄影大赛，大家来看看人气前三的获奖照片吧！"
categories: photography_contest fall-20
---
{% assign photography = site.data.y2020.photography %}
{% assign img_path_prefix = "/assets/by_year/fa2020-sp2021/photography/" %}

<div style="margin: 40px; font-size: 16px">
    {% for photo in photography["top_three_photos"] %}
        <h3 class="blue-highlight">{{ photo.name }}</h3>
        <div class="row">
            <div class="col-sm-6 col-sm-offset-3" style="padding: 10px" align="left">
            <img src="{{ img_path_prefix }}{{ photo.img }}" style="width:540px;"/>
            </div>
        </div>
    {% endfor %}
</div>

<div style="margin: 40px; font-size: 16px">
    <p align="center">
        <span style="color: #ff0000">恭喜</span>以上三位同学获奖!
    </p>
</div>