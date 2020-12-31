---
layout: best_singer2020
title:  "记得去哔哩哔哩看CSA十佳歌手总决赛"
date:   2020-12-30 00:00:00 +0800
dateStr: "Dec. 30, 2020"
thumbnail: "/assets/events/bestsinger2020.jpg"
brief: "美东2021年1月1日晚9:40/国内2021年1月2日早10:40 十佳歌手决赛， 不见不散！"
categories: best_singer fall-20
---
{% assign best_singer = site.data.y2020.best_singer %}
{% assign img_path_prefix = "/assets/by_year/fa2020-sp2021/best_singer2020/" %}

<div class="row">
  <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
      <h3>经过层层筛选，共12名选手脱颖而出，迎来最终的battle。
    决赛将在bilibili直播同步播出，届时会在佛大学生群里分享观赛链接，请拭目以待！</h3>
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
