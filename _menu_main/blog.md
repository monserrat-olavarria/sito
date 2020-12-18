---
layout: post
title: "blog"
permalink: "/blog/"
category: blog
image: 
card:
  image: "/image/monserrat_canta.jpg"
  title: " Monserrat Olavarria"
  subtitle: "cantante <br> educatrice musicale"
  text:  "insegnante accreditato Audiation Institute, educatrice Cemea, mediatrice culturale, formatrice, si dedica alla scrittura, all'illustrazione e al teatro"
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
<br>
<div class="container">
 {% for post in site.categories[page.category] %}
  <div class="row">
    <div class="col-sm">
        <!-- Card -->
          <div class="card">
             <!-- Card image -->
             <img class="card-img-top" src="{{post.image}}" >
             <!-- Card content -->
             <div class="card-body">
                <!-- Title -->
                <h4 class="card-title"><a href="{{ post.url }}"> {{ post.title }}</a></h4>
                <h5 class="blue-text pb-2"><strong>{{post.subtitle}}</strong></h5>
                <!-- Text -->
                <p class="card-text">{{post.excerpt }}</p>
                    <!-- Button -->
                <a href="{{ post.url }}" class="btn btn-unique">leggi</a>
             </div>
  </div>
            <br>
  {% endfor %}
</div>

