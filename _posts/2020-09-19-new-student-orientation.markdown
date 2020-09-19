---
layout: orientation_1
title:  "【回顾】UFCSA 2020新生Orientation"
date:   2020-09-19 00:00:00 +0800
dateStr: "Sept. 19, 2020"
thumbnail: "/assets/by_year/fa2020-sp2021/orientation/orientation.png"
brief: "9月19日在Bilibili，我们发布了2020年秋季UFCSA的新生Orientation！"
categories: orientation fall-20
---
{% assign orientation = site.data.y2020.orientation %}
{% assign img_path_prefix = "/assets/by_year/fa2020-sp2021/orientation/" %}

<div class="row">
  <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
    <h3>由于疫情的原因，今年的Orientation我们选择在Bilibili上举行</h3>
  </div>
</div>

<div class="special-box-wrapper">
  <div class="special-box">
    <h3 class="blue-highlight" style="margin:5px"><a href="https://www.bilibili.com/video/BV1wZ4y1K7XH/">点击这里前往Bilibili观看视频</a></h3>
  </div>
</div>

<div class="text-responsive" style="margin: 40px">
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">学校有各种组织</p>
    </div>
  </div>
    {% for speaker in orientation["part-1"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless speaker.brief == '' %}
          <p>{{ speaker.brief }}</p>
        {% endunless %}
        <img src="{{ img_path_prefix }}{{ speaker.img }}" style="width:540px;height:337px;"/>
        {% unless speaker.brief2 == '' %}
          <p>{{ speaker.brief2 }}</p>
        {% endunless %}
        </div>
      </div>
    {% endfor %}
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">学长学姐们有各种干货</p>
    </div>
  </div>
    {% for speaker in orientation["part-2"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless speaker.brief == '' %}
          <p>{{ speaker.brief }}</p>
        {% endunless %}
        <img src="{{ img_path_prefix }}{{ speaker.img }}" style="width:540px;height:337px;"/>
        {% unless speaker.brief2 == '' %}
          <p>{{ speaker.brief2 }}</p>
        {% endunless %}
        </div>
      </div>
    {% endfor %}
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">村有各种课外活动</p>
    </div>
  </div>
    {% for speaker in orientation["part-3"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless speaker.brief == '' %}
          <p>{{ speaker.brief }}</p>
        {% endunless %}
        <img src="{{ img_path_prefix }}{{ speaker.img }}" style="width:540px;height:337px;"/>
        <img src="{{ img_path_prefix }}{{ speaker.img2 }}" style="width:540px;height:337px;" onerror="this.style.display='none'"/>
        {% unless speaker.brief2 == '' %}
          <p>{{ speaker.brief2 }}</p>
        {% endunless %}
        </div>
      </div>
    {% endfor %}
  <div class="row">
    <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
      <p>{{ orientation.final-word.brief }}</p>      
      <p>{{ orientation.final-word.brief2 }}</p>
    </div>
  </div>
  <p>{{ orientation.final-word.final }}</p>
</div>
