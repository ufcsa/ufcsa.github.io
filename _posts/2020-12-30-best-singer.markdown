---
layout: best_singer2020
title:  "【回放】UFCSA 2020十佳歌手总决赛现场"
date:   2021-01-03 00:00:00 +0800
dateStr: "Jan. 03, 2021"
thumbnail: "/assets/events/bestsinger2020.jpg"
brief: "十佳歌手决赛回放， 尽情感受当晚的现场气氛吧！"
categories: best_singer fall-20
---
{% assign best_singer = site.data.y2020.best_singer %}
{% assign img_path_prefix = "/assets/by_year/fa2020-sp2021/best_singer2020/" %}

<div class="row">
  <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
      <h3>决赛回放可在bilibili上观看，尽情感受当晚的现场气氛吧！</h3>
  </div>
</div>

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">决赛结果</h3>
    {% for res in best_singer["result"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 1px" align="left">
        <p>{{ res.singer }}</p>
        </div>
      </div>
    {% endfor %}
</div>

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">决赛回放</h3>
    <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 1px">
            <iframe width="540" height="360" src="//player.bilibili.com/player.html?aid=671105766&bvid=BV1zU4y1x7jV&cid=277678573&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
        </div>
    </div>
</div>

<div class="text-responsive" style="margin: 40px">
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">12进6 1V1淘汰赛 </p>
    </div>
  </div>
      <p>决赛第一轮采用1v1淘汰制，十二名（6组）选手根据初赛评分两两分为一组，分别现场演唱一首完整指定曲目，由五位学生评委评定，优胜的选手晋级决赛第二轮，另一名选手被淘汰。<br><br> 以下为第一轮对战名单。</p>
   <img src="/assets/by_year/fa2020-sp2021/best_singer2020/battle1.png" />
      <br><br>

  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">前六 排名赛</p>
    </div>
  </div>
   <p>第二轮由优胜的选手依次演唱准备好的歌曲，<br>根据三位明星评委与往届十大冠军打分从高到低排出前六名次。</p>  
   <br>



  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">奖品介绍</p>
    </div>
  </div>
  <br>
    <img src="/assets/by_year/fa2020-sp2021/best_singer2020/bestsinger2020.png"  style="width:480px;height:360px;"/>
 {% for award in best_singer["award"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless award.singer_award == '' %}   
          <p>{{ award.singer_award }}</p>   
        {% endunless %}
        </div>
      </div>
    {% endfor %}
 <p>同时，本次线上直播增设了幸运观众奖<br>
 一等奖x1  dyson吹风机一台<br>
二等奖x8 微信100元红包<br>
一起来发弹幕吧! 说不定，锦鲤就是你自己!</p>  





 <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">明星评委</p>
    </div>
  </div>
  {% for judges in best_singer["star_judges"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        {% unless judges.name == '' %}
         <img src="{{ img_path_prefix }}{{ judges.pic }}" style="width:480px;height:560px;"/>
          <h3 style="color:blue">{{ judges.name }}</h3><br>
            <p>{{ judges.introduction }}</p>
        {% endunless %}
        </div>
      </div>
    {% endfor %}
  <div class="row">
    <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">   
    <br>    
        <p style="color:red">{{ best_singer.final-word.final }}</p>  
  </div>

</div>
