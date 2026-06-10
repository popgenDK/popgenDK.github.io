---
title: "Albrechtsen Lab - Publications"
layout: gridlay
excerpt: "Albrechtsen Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

[Jump to full list](#full-list-of-publications)

## Group highlights


{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
	  <pubtit>{{ publi.title }}</pubtit>
	  <a href="{{ publi.link.url }}" target="_blank" rel="noopener noreferrer">
	     <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" alt="{{ publi.title | escape }}" title="{{ publi.abstract }}" class="img-responsive" width="33%" style="float: left" />
   </a>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  {% if publi.github %}
  <p><strong><a href="{{ publi.github }}">Code used in paper</a></strong></p>
  {% endif %}
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
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


## Full List of publications
[See google scholar for up to date publication list](https://scholar.google.com/citations?hl=en&user=20oVxFsAAAAJ&view_op=list_works&sortby=pubdate)

{% assign pub_number_printed = 1 %}

{% for publi in site.data.publist %}
  
  {{pub_number_printed}} <b>{{ publi.title }} </b> <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% assign pub_number_printed = pub_number_printed | plus: 1 %}

{% endfor %}
