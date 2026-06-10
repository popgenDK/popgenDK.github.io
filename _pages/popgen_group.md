---
title: "Albrechtsen Lab - Popgen group"
layout: gridlay
excerpt: "Albrechtsen Lab -- Popgen Group."
sitemap: false
permalink: /popgen_group/
---


# Population and Statistical genetics at the Bioinformatic Center at UCPH

We are meta group of labs that work with various parts of population, medical and statistical genetics at the Biocenter at University of Copenhagen. The meta group consists of 5 labs that works with focus on different organisms and systems. We apply and develop methods for analyzing large scale next generation sequencing data. 




<div class="row">
 
<div class="col-sm-6 clearfix">
 <div class="well">

  <h2>Hans Siegismund</h2>

  <pubtit>Associate Professor</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/HS.jpg" class="img-responsive" width="33%" style="float: left" alt="Hans Siegismund" />
  <p>We work on population genetics, phylogeography and speciation processes of large African mammals, mainly bovids and great apes. Another research area includes the study of evolutionary genetics of foot-and-mouth-disease (FMD) virus in East Africa.</p>
  <p><strong><a href="https://website.popgen.dk/popgen_group">my website</a></strong></p>
 </div>
</div>

<div class="col-sm-6 clearfix">
 <div class="well">

  <h2>Ida Moltke</h2>

  <pubtit>Associate professor</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/IM.jpg" class="img-responsive" width="33%" style="float: left" alt="Ida Moltke" />
  <p>We develop and apply statistical methods to genomic data with the purpose of gaining insights into human disease, history and evolution. For instance, by studying DNA from the Greenlandic population we recently identified a genetic variant that explains 10-15% of all cases of type 2 diabetes in Greenland. We have also looked into the migration history of the Artic and are currently investigating how the Greenlanders have genetically adapted the Arctic cold and their very fat-rich diet consisting mainly of seal and fish.</p>
  <p><strong><a href="https://website.popgen.dk/popgen_group">my website</a></strong></p>
 </div>
</div>


</div>


<div class="row">
 
<div class="col-sm-6 clearfix">
 <div class="well">

  <h2>Rasmus Heller</h2>

  <pubtit>Associate Professor</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/RH.jpg" class="img-responsive" width="33%" style="float: left" alt="Rasmus Heller" />
  <p>I am interested in applying population and evolutionary genetics to answer questions about animal biology, particularly in large mammals. Most of my work has revolved around large African mammals. My research tries to address a range of topics in these species, including the historical drivers of population dynamics, how variation emerges and is retained, speciation, adaptive evolution and the relationship between phenotypic and genomic variation. I am also interested in topics of a more immediate interest in species conservation such as landscape genetics, the effect of habitat fragmentation, population connectivity etc </p>
  <p><strong><a href="https://website.popgen.dk/popgen_group">my website</a></strong></p>
 </div>
</div>

<div class="col-sm-6 clearfix">
 <div class="well">

  <h2>Anders Albrechtsen</h2>

  <pubtit>Professor</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/AA3.jpg" class="img-responsive" width="33%" style="float: left" alt="Anders Albrechtsen" />
  <p>Our group develops statistical and computational methods for analysis of genomic data including methods for performing multi-loci association studies, methods for detecting and correcting for population stratification, methods for detecting natural selection, loci dependent methods for modeling identity-by-descent and various methods for analysis of second generation sequencing data.</p>
  <p><strong><a href="https://website.popgen.dk/popgen_group">my website</a></strong></p>
 </div>
</div>


</div>

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
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ software.image }}" class="img-responsive" width="33%" style="float: left" alt="{{ software.name | default: software.title | escape }}" />
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
