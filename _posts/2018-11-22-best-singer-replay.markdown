---
layout: best_singer_layout_1
title:  "【回放】十佳歌手决赛现场回放"
date:   2018-11-22 18:00:00 -0500
dateStr: "Nov. 22, 2018"
thumbnail: "/assets/events/best_singer.jpg"
brief: "11月18日，十佳歌手圆满落幕。比赛紧张激烈，但选手们依然在现场发挥出了自己的特色，给现场观众带去了曲风不同、独特动听的歌声。感谢每一位选手的努力和付出！"
categories: best-singer videos fall-18
---
{% assign best-singer = site.data.y2018.best-singer %}

<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">第一轮： 十六强对唱</h3>
    {% for singing_pair in best-singer["singing_pairs"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        <p>{{ singing_pair.caption }}</p>
        <iframe width="540" height="360"
        src="https://www.youtube.com/embed/{{ singing_pair.youtube_id }}"></iframe>
        </div>
      </div>
    {% endfor %}
</div>
<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">第二轮： 十强独唱</h3>
    <p>统计了评委打分以及现场观众投票后，本届比赛的十佳歌手脱颖而出！恭喜大家！</p>
    {% for singing_pair in best-singer["top-ten"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        <p>{{ singing_pair.caption }}</p>
        <iframe width="540" height="360"
        src="https://www.youtube.com/embed/{{ singing_pair.youtube_id }}"></iframe>
        </div>
      </div>
    {% endfor %}
</div>
<div style="margin: 40px; font-size: 16px">
  <h3 class="blue-highlight">第三轮：三强决赛</h3>
    <p>统计了评委打分以及现场观众投票后，本届比赛的前三甲脱颖而出！</p>
    {% for singing_pair in best-singer["top-three"] %}
      <div class="row">
        <div class="col-sm-6 col-sm-offset-3" style="padding: 20px">
        <p>{{ singing_pair.caption }}</p>
        <iframe width="540" height="360"
        src="https://www.youtube.com/embed/{{ singing_pair.youtube_id }}"></iframe>
        </div>
      </div>
    {% endfor %}
</div>
