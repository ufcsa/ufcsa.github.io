---
layout: best_singer2020
title:  "【回放】UFCSA 2021精彩瞬间"
date:   2022-01-06 00:00:00 +0800
dateStr: "Jan.05, 2022"
thumbnail: "/assets/by_year/2022/bestsinger2021.jpeg"
brief: "2022年UFCSA线上歌手比赛圆满落幕！非常感谢各位同学的积极参与。在经过评委们细心的考察评定后，我们终于决出了本次比赛的Top5！"
categories: best_singer fall-20
---
{% assign best_singer = site.data.y2021.best_singer %}


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
            <iframe width="540" height="360" src="//player.bilibili.com/player.html?aid=338054818&bvid=BV1gR4y1g7Mc&cid=481693395&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
        </div>
    </div>
</div>

<div class="text-responsive" style="margin: 40px">
  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">评分方式 </p>
    </div>
  </div>
      <p>由CSA特邀的五位评委为选手打分，其中去掉最高分+最低分，剩余分数取平均分作为最终评分结果。</p>
    <br>

  <div class="special-box-wrapper">
    <div class="special-box">
      <p class="blue-highlight" style="margin:5px">额外说明</p>
    </div>
  </div>
   <p>这次比赛收到了许多关于使用混响的争议。<br>为了保证公平，我们讨论后决定让使用混响的选手重发未混声的视频，并让评委们重新打分。</p>  
   <br>




</div>
