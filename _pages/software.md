---
title: "Albrechtsen Lab - Software"
layout: gridlay
excerpt: "Albrechtsen Lab -- Software."
sitemap: false
permalink: /software/
---
# Software


{% assign number_printed = 0 %}
{% for software in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if software.software %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  {% if software.name %}
  <h2>{{ software.name }}</h2>
  {% endif %}
  <pubtit>{{ software.title }}</pubtit>
  {% if software.image %}
  <img src="{{ '/images/pubpic/' | append: software.image | relative_url }}" class="img-responsive" width="33%" style="float: left" alt="{{ software.name | default: software.title | escape }} software illustration" />
  {% endif %}
  {% if software.image_credit %}
  <p class="small">Image: <a href="{{ software.image_source_url | default: software.link.url }}" target="_blank" rel="noopener noreferrer">{{ software.image_credit }}</a>, <a href="{{ software.image_license_url }}" target="_blank" rel="noopener noreferrer">{{ software.image_license }}</a>.</p>
  {% endif %}
  <p>{{ software.description }}</p>
  <p><em>{{ software.authors }}</em></p>
  <p><strong><a href="{{ software.link.url }}">{{ software.link.display }}</a></strong></p>
  <p><strong><a href="{{ software.software }}">software website</a></strong></p>  
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>
