---
layout: best_singer_layout_1
title:  "UFCSA 2020秋季十佳歌手初赛人气选拔"
date:   2020-12-13 00:00:00 +0800
dateStr: "Dec. 13, 2020"
thumbnail: "/assets/by_year/fa2020-sp2021/best_singer2020_pre/cover_pic.png"
brief: "2020年秋季十佳歌手初赛人气选拔，快来看看选手们的表现吧！"
categories: best_singer fall-20
---
{% assign best_singer_pre = site.data.y2020.best_singer_pre %}
{% assign img_path_prefix = "/assets/by_year/fa2020-sp2021/best_singer2020_pre/" %}

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">十佳歌手赛制</h3>
    {% for rule in best_singer_pre["contest_rules"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 1px" align="left">
        <p>{{ rule.content }}</p>
        </div>
      </div>
    {% endfor %}
</div>

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">评审方式</h3>
    {% for rule in best_singer_pre["scoring_rules"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 1px" align="left">
        <p>
            <strong>{{ rule.sub }}</strong>{{ rule.content }}
        </p>
        </div>
      </div>
    {% endfor %}
</div>

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">初赛完整录播(包括晋级以及未晋级选手)</h3>
    <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 1px">
            <iframe width="540" height="360" src="//player.bilibili.com/player.html?aid=800478694&bvid=BV1zy4y1q75u&cid=261572662&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
        </div>
    </div>
</div>

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">初赛晋级选手演唱歌曲</h3>
    {% for video in best_singer_pre["videos"] %}
        <p><strong>{{ video.name }}</strong></p>
        <div class="row">
            <div class="col-sm-6 col-sm-offset-3" style="padding: 5px">
                <iframe width="540" height="360" src="{{ video.src }}" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
            </div>
        </div>
    {% endfor %}
</div>


