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
        <h3>Thumbnail label</h3>
        <p>...</p>
        <p><a href="{{ service_path }}" class="btn btn-primary" role="button">voir les services</a> </p>
      </div>
    </div>
  </div>
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="http://lorempixel.com/g/128/128/nature/" alt="...">
      <div class="caption">
        <h3>Thumbnail label</h3>
        <p>...</p>
        <p><a href="#" class="btn btn-primary" role="button">Button</a> <a href="#" class="btn btn-default" role="button">Button</a></p>
      </div>
    </div>
  </div>
</div>

{% for post in site.posts limit:5 %}
 <h3>{{ post.date | date_to_string }} &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h3>
{% endfor %}

[plus d'articles]({{ BASE_PATH }}/archive.html)

