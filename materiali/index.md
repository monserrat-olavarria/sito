---
layout: page
title: "Materiali didattici"
category: "materiali didattici"
permalink: "/materiali/"
image: "http://www.concertoconmammaepapa.it/web/wp-content/uploads/2019/08/musica-nova-14-dicembre-2019.jpg"
card:
  image: "/image/monserrat_canta.jpg"
  title: " Monserrat Olavarria"
  subtitle: "cantante <br> docente di musica"
  text: "Mi dedico alla composizione di materiale originale, canzoni, canti e filastrocche che utilizzo nei propri percorsi didattici con i bambini di diverse età."
  link: "/chisono/"
social:
  youtube: "https://www.youtube.com/channel/UCMQJkzvobU3ZikrzYaY3x7w/featured/"
  me: "https://m.me/avenidamerica/"
  facebook: "https://www.facebook.com/avenidamerica/"
sidebar:
  image: "/image/tiritinlalla_1980.jpg"
  title: ""
  subtitle: "Tiritinlallà"
  text: "il mio ultimo disco"
  link: "/dischi/tiritinlalla/"
---
<!-- 
<video   controls>
    <source src="/video/piccoli canti.mp4" type="video/mp4">
</video>
-->

{% assign video_head = "  " %}
{% assign video_files = site.static_files | where: "video", true %}


{% for myvideo in video_files %}
{% assign video_head = myvideo.basename | split: " , " | first  %}

{% if video_head_old !=  video_head  %}
<br>
<h2> {{ video_head }}</h2>
{% endif %}
<div class="embed-responsive embed-responsive-16by9">
  <video   controls>
    <source src="{{ myvideo.path | escape }}" type="video/{{ myvideo.extname | remove_first: "." }} ">
    <p> {{ myvideo.basename }}</p>
    <p>Your user agent does not support the HTML5 video element. </p>
  </video>


{% assign video_head_old = video_head    %}
</div>
  <p> {{ myvideo.basename | split: " , " | last }}</p>
{% endfor %}