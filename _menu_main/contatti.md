---
layout: default
title: contatti
name: contatti
position: 01
output: true
permalink: /contatti/
---

### {{page.name}}
{{site.title}}

  {% if  site.phone %}
cellulare: {{site.phone}}
  {% endif %}
    {% if  site.email %}

email: [{{site.email}}](mailto:{{site.email}})
  {% endif %}

#### Potete usare questa pagina per mandarmi un  email

<form action="https://formspree.io/{{site.email}}" method="POST">
    <div class="form-group row">
        <div class="col-md-6">

            <input class="form-control" type="text" name="name" placeholder="Nome Cognome">
        </div>
        <div class="col-md-6">
            <input class="form-control" type="email" name="_replyto" placeholder="E-mail xxx@yyyy.zz">
        </div>
    </div>
    <textarea rows="8" class="form-control mb-3" name="message" placeholder="Messaggio"></textarea>
    <input class="btn btn-success" type="submit" value="invio">
</form>
