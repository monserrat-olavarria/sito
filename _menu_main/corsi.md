---
layout: post
title: "corsi 2020"
permalink: "/corsi/"
category: corsi
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
  link: "/tiritinlalla/"
---
<!-- 
<div class="embed-responsive embed-responsive-16by9">
<iframe width="560" height="315" src="https://www.youtube.com/embed/5DbXNHvHHk4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<br><br>
-->
#### Scuole di musica

#### [Centro Ottava](https://www.centrottava.it/)  
* Sabato 10:30  alle 11:30 primi passi cantando, per bambini da 0 a 36 mesi accompagnati da un genitore.
* Sabato 11:30  alle 12:30 giochi in musica, per bambini da 3 a 5 anni 

#### [Scuola Popolare di Musica del Tiburtino](https://www.scuolapopolaremusicatiburtino.it)  
* Giovedì 18:00 alle 19:00 Dai 3 ai 6 anni – Propedeutica musicale
* Venerdì 17:00 alle 18:00 Dai 3 ai 6 anni – Propedeutica musicale

<p>
<div class="embed-responsive embed-responsive-16by9">
<iframe width="560" height="315" src="/video/piccoli_canti.mp4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
</p>

#### Asili nido e scuole dell'infanzia

#### [In crescendo](https://www.increscendo.it/)
#### [Il paese delle meraviglie](https://asilonidoilpaesedellemeraviglie.eu/)
#### [Cocchi di Mamma](http://www.cocchidimamma.it/)
#### [Il girotondo](https://www.schoolandcollegelistings.com/IT/Monte-Porzio-Catone/1345476828812498/Monte-Porzio-Catone-La-Porziana-Asilo-Nido) 
#### [Il Carosello](http://www.ilcarosello.it/)


<br><br>


#### Laboratori di educazione musicale 
###### a cura di Monserrat Olavarria
<br>
<div class="container">
 {% for post in site.categories[page.category] %}
  <div class="row">
    <div class="col-sm">
        <!-- Card -->
          <div class="card">
             <!-- Card image -->
             <img class="card-img-top" src="{{post.image}}" alt=" image of {{post.image}}">
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

<div class="container" >
<h5>Se volete informazioni potete contattarmi   </h5>
<form action="https://formspree.io/{{site.email}}" method="POST">
    <div class="form-group row">
        <div class="col-md-6">

            <input class="form-control" type="text" name="name" placeholder="Nome">
        </div>
        <div class="col-md-6">
            <input class="form-control" type="email" name="_replyto" placeholder="E-mail">
        </div>
    </div>
    <textarea rows="8" class="form-control mb-3" name="message" placeholder="Messaggio"></textarea>
    <input class="btn btn-success" type="submit" value="invio">
</form>
</div>