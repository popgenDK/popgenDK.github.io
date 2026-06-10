---
title: "EPIC seminar series"
layout: gridlay
excerpt: "..."
sitemap: false
permalink: /EPIC_seminar/
---

# Next up

{% assign number_printed = 0 %}
{% for date in site.data.EPIC_seminar %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if date.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <b><i>{{ date.day }}</i></b><br />
  <b>{{ date.title1 }}</b><br />
  <em>{{ date.speaker1 }}</em><br />
  <b>{{ date.title2 }}</b><br />
  <em>{{ date.speaker2 }}</em><br />
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

# Full list of past talks

{% for date in site.data.EPIC_seminar %}
{% if date.highlight == 0 %}

  <b>{{ date.day }} </b> <br />
  <b>{{ date.title1 }} </b> <br />
  <em>{{ date.speaker1 }} </em> <br />
  <b>{{ date.title2 }} </b> <br />
  <em>{{ date.speaker2 }} </em><br />

{% endif %}
{% endfor %}
