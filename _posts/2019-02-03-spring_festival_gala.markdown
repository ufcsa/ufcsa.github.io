---
layout: new_year_layout
title:  "【回顾】2019春节晚会"
date:   2019-02-03 18:00:00 -0500
dateStr: "Feb. 03, 2019"
thumbnail: "/assets/by_year/fa2018-sp2019/new_year/banner.jpg"
brief: "2019年佛罗里达大学中国学生会春节联欢晚会圆满落幕。晚会精彩纷呈，既有代表中华传统文化的水袖舞和民族舞，又有融合日韩潮流的热舞以及演奏；有惹人捧腹的小品和魔术，也有发人深省的音乐剧等。"
categories: spring_festival spring-19
---
{% assign new_year = site.data.y2018.new_year %}
{% assign img_path_prefix = "/assets/by_year/fa2018-sp2019/new_year/" %}

<div class="text-responsive">
  <p>可谓交融中西，贯通古今。下面就让我们回顾一下热烈的春晚现场吧~</p>
  <br/><br/>
  {% for item in new_year.schedule %}
    <div class="text-center">
      <div class="new_year_text_banner" style="color: #FFF">
        <p style="margin-top: 5px">{{ item.title }}</p>
      </div>
    </div>
    <div style="margin: 20px 10px">
      {{ item.brief }}
    </div>
    <div class="text-center">
      <img src="{{ img_path_prefix }}{{ item.image }}" width="512px" class="img-responsive" style="display: inline-block;" />
    </div>
    {% unless item.brief2 == ''  %}
      <div style="margin: 20px 10px">
        {{ item.brief2 }}
      </div>
    {% endunless %}
    <section style="margin-bottom: 50px"></section>
  {% endfor %}
</div>
<!-- END Thanks -->
<div class="text-center" style="margin-bottom: 50px">
  <div>
    <div class="diamond_banner_outer">
      <div class="new_year_diamond_banner">
        <div class="diamond_banner_inner">
          <div class="diamond_banner_text">
            <p>特</p>
          </div>
        </div>
      </div>
    </div>
    <div class="diamond_banner_outer">
      <div class="new_year_diamond_banner">
        <div class="diamond_banner_inner">
          <div class="diamond_banner_text">
            <p>别</p>
          </div>
        </div>
      </div>
    </div>
    <div class="diamond_banner_outer">
      <div class="new_year_diamond_banner">
        <div class="diamond_banner_inner">
          <div class="diamond_banner_text">
            <p>鸣</p>
          </div>
        </div>
      </div>
    </div>
    <div class="diamond_banner_outer">
      <div class="new_year_diamond_banner">
        <div class="diamond_banner_inner">
          <div class="diamond_banner_text">
            <p>谢</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<div class="text-center text-responsive">
  <strong>主持人：</strong>
  <p>{{ new_year.hosts }}</p>
  <strong>感谢摄影师：</strong>
  <p>{{ new_year.photographers }}</p>
  <br/>
  <strong>感谢赞助商：</strong>
  {% for sponsor in new_year.sponsors %}
    <p>{{ sponsor.name }}</p>
  {% endfor %}
  <br/>
  <strong>感谢每一位工作人员的付出！</strong>
  <img src="{{ img_path_prefix }}{{ new_year.staff_gathering_img }}" class="img-responsive" width="512px" style="display: inline-block;" />
</div>
