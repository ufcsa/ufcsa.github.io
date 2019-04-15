---
layout: mid-autumn_festival_1
title:  "【回顾】2018 CSA中秋晚会圆满落幕"
date:   2018-09-26 18:00:00 -0500
dateStr: "Sep. 26, 2018"
thumbnail: "/assets/by_year/fa2018-sp2019/mid_autumn/mid-autumn.jpg"
brief: "又是一个中秋月，夏日的脚步在不经意间已悄然走过。独在异乡为异客，每逢佳节倍思亲。CSA为远在他乡的UF留学生安排了一场精彩的中秋晚会，并为大家准备了甜美的月饼～"
categories: mid-autumn fall-18
---
{% assign mid-autumn = site.data.y2018.mid-autumn %}
{% assign img_path_prefix = "/assets/by_year/fa2018-sp2019/mid_autumn/" %}

<div class="text-responsive" style="margin: 40px; text-align:center">
  {% for item in mid-autumn.schedule %}
    <div class="row">
      <div style="padding: 20px">
      <div class="special-box-wrapper">
        <div class="special-box">
          <p class="blue-highlight" style="margin:5px">{{ item.title }}</p>
        </div>
      </div>
      <p class="text-responsive" style="padding:10px 0px;">{{ item.brief }}</p>
      {% unless item.img == '' %}
        <img class="img-responsive" src="{{ img_path_prefix }}{{ item.img }}" />
      {% endunless %}
      {% unless item.img2 == '' %}
        <img class="img-responsive" src="{{ img_path_prefix }}{{ item.img2 }}" />
      {% endunless %}
      </div>
    </div>
  {% endfor %}
  <div class="row">
    <div style="padding: 20px">
      <p>{{ mid-autumn.final_words.brief }}</p>      
      <img src="{{ img_path_prefix }}{{ mid-autumn.final_words.img }}" class="img-responsive" />
      <img src="{{ img_path_prefix }}{{ mid-autumn.final_words.img2 }}" class="img-responsive" />
    </div>
  </div>
</div>
