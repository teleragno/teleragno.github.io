---
layout: page
title: Teleragno - FAI associatif à Marseille
header: Teleragno
tagline: Fournisseur d'accès internet associatif à Marseille
---
{% include JB/setup %}

<div class="row">
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="http://lorempixel.com/128/128/nature/" alt="...">
      <div class="caption">
        <h3>Services</h3>
        <p>
		L'association est capable de fournir à ses adhérents différents types de service comme : WiFi, boîte mail, VPN, ...
	</p>
        <p><a href="/services.html" class="btn btn-primary" role="button">En savoir plus</a> </p>
      </div>
    </div>
  </div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="http://lorempixel.com/g/128/128/nature/" alt="...">
      <div class="caption">
        <h3>L'association</h3>
        <p>
		Teleragno est un FAI associatif, local, membre de la Fédération FDN.
		Nous sommes attachés à la neutralité du net.

		Tout cela est obscurs ? Venez nous rencontrer.
	</p>
        <p><a href="/a-propos.html" class="btn btn-primary" role="button">En savoir plus</a> </p>
      </div>
    </div>
  </div>
</div>

<div class="row">

<h2>Les dernier articles</h2>

{% for post in site.posts limit:5 %}
 <h3>{{ post.date | date_to_string }} &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h3>
{% endfor %}

[plus d'articles]({{ BASE_PATH }}/archive.html)
</div>


