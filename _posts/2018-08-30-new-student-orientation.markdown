---
layout: orientation_1
title:  "【回顾】UFCSA 2018新生Orientation"
date:   2018-08-26 18:00:00 -0500
dateStr: "Aug. 26, 2018"
thumbnail: "/assets/by_year/fa2018-sp2019/orientation/orientation.jpg"
brief: "8月26日，在Retiz Union Grand Ballroom，我们迎来了300多位 2018 秋季的新同学和许多老生朋友！"
categories: orientation fall-18
---
{% assign orientation = site.data.y2018.orientation %}
{% assign img_path_prefix = "/assets/by_year/fa2018-sp2019/orientation/" %}

<div class="text-responsive" style="margin: 40px">
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">第一部分</p>
    </div>
  </div>
    {% for speaker in orientation["part-1"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless speaker.brief == '' %}
          <p>{{ speaker.brief }}</p>
        {% endunless %}
        <img src="{{ img_path_prefix }}{{ speaker.img }}" />
        {% unless speaker.brief2 == '' %}
          <p>{{ speaker.brief2 }}</p>
        {% endunless %}
        </div>
      </div>
    {% endfor %}
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">第二部分</p>
    </div>
  </div>
    {% for speaker in orientation["part-2"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless speaker.brief == '' %}
          <p>{{ speaker.brief }}</p>
        {% endunless %}
        <img src="{{ img_path_prefix }}{{ speaker.img }}" />
        {% unless speaker.brief2 == '' %}
          <p>{{ speaker.brief2 }}</p>
        {% endunless %}
        </div>
      </div>
    {% endfor %}
  <div class="row">
    <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
      <p>{{ orientation.final-word.brief }}</p>      
      <img src="{{ img_path_prefix }}{{ orientation.final-word.img }}" />
      <img src="{{ img_path_prefix }}{{ orientation.final-word.img2 }}" />
      <p>{{ orientation.final-word.brief2 }}</p>
    </div>
  </div>
  <p>{{ orientation.final-word.final }}</p>
</div>
