---
title: "Conservation and Population Genomics Workshop 2026"
layout: gridlay
excerpt: "Hands-on conservation genomics workshop at Mpala Research Centre, Kenya"
sitemap: false
permalink: /workshop/
---

# Conservation genomics workshop 2026

<div markdown="0" id="carousel" class="carousel slide stable-carousel" data-ride="carousel" data-interval="4000" data-pause="hover">
  <ol class="carousel-indicators">
    <li data-target="#carousel" data-slide-to="0" class="active"></li>
    <li data-target="#carousel" data-slide-to="1"></li>
    <li data-target="#carousel" data-slide-to="2"></li>
  </ol>

  <div class="carousel-inner" markdown="0">
    <div class="item active">
      <img src="{{ '/images/slider/wildeBeastMap.png' | relative_url }}" alt="Map of wildebeest populations" />
    </div>
    <div class="item">
      <img src="{{ '/images/slider/wildebeestPCA_admix.png' | relative_url }}" alt="Population structure analyses" />
    </div>
    <div class="item">
      <img src="{{ '/images/slider/wildebeest_het.png' | relative_url }}" alt="Genetic diversity analysis" />
    </div>
  </div>

  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

## General information

**Dates:** August 19-23, 2026 <br/>
**Venue:** [Mpala Research Centre](https://mpala.org/), Laikipia, Kenya <br/>
**Participants:** Approximately 25 students from Kenya and other African countries <br/>
**Format:** On-site lectures with hands-on exercises run on a server in Copenhagen <br/>
**Context:** The workshop is connected with the annual African BioGenome Project (AfricaBP) Open Institute Eastern Africa Regional Workshop in Nairobi on August 17-18, 2026. <br/>
**Registration:** Registration information will be provided through the African BioGenome Project. <br/>
**What will be supplied:** Simple dorm-style accommodation, all meals during the workshop and transport pick-up Nanyuki-Mpala (on August 18 and back 23) will be provided at no cost to workshop participants.  <br/>
**Prerequisites:** Participants are expected to have some previous exposure to and experience with genetics, preferably with population genetics. Experience with NGS data, genomics, statistics and/or programming is considered an advantage, but not an absolute requirement. Participants must bring a laptop that can access the internet (wifi is available).   <br/>


The workshop is a comprehensive, hands-on introduction to population genomic analyses of next-generation sequencing data, with an emphasis on wildlife conservation. Lectures will be combined with practical computer exercises, discussions, and research talks presenting conservation genomics case studies.

## Topics

- Introduction to conservation genetics and next-generation sequencing data
- Genetic diversity, heterozygosity, FST, and runs of homozygosity
- Selection and genome scans
- Population structure and admixture
- Gene flow, D-statistics
- Demographic inference, the site frequency spectrum
- Applying conservation genomics in practice

## Intended learning outcomes

After the workshop, participants should be able to:

- Describe how short-read NGS data are processed before population genomic analyses.
- Estimate and interpret genome-wide heterozygosity, FST, runs of homozygosity, and inbreeding coefficients.
- Use PCA and admixture analyses to investigate population structure.
- Understand approaches for studying gene flow, selection, and demographic history.
- Relate population genomic results to conservation units and management decisions.

## Instructors

{% assign number_printed = 0 %}
{% for yml in site.data.workshop %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if yml.highlight == 1 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<div class="well">
<h2>{{ yml.name }}</h2>
<pubtit>{{ yml.title }}</pubtit>
<img src="{{ '/images/teampic/' | append: yml.image | relative_url }}" class="img-responsive" width="33%" style="float: left" alt="{{ yml.name }}" />
<p>{{ yml.description }}{% if yml.website %} <strong><a href="{{ yml.website }}">Website</a></strong>{% endif %}</p>
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

<p>&nbsp;</p>

## Venue and practical information

Mpala Research Centre is in the Laikipia ecosystem, approximately four hours by road from Nairobi. The centre hosts Kenyan and international researchers and students and provides facilities for field biology and molecular research. The surrounding conservancy has a rich diversity of wildlife, with approximately 100 recorded mammal species. More information about the research centre, conservancy, and accommodation is available from [Mpala](https://mpala.org/).

Participants must bring a laptop. The practical exercises will use a remote server, so laptops with any major operating system can be used.

## Preliminary program

### Wednesday, August 19

- Morning: Introduction to conservation genetics
           Introduction to linux/bash and Jupyter notebooks
- Afternoon: Introduction to NGS data

### Thursday, August 20

- Morning: Demographic inference, coalescence, SFS
- Afternoon: Research talks

### Friday, August 21

- Morning: Admixture
- Afternoon: PCA \nGene flow

### Saturday, August 22

- Morning: Relatedness, FST
- Afternoon: Positive selection, genome scans

### Sunday, August 23

- Morning: Heterozygosity, and runs of homozygosity
- Afternoon: Conservation genomics in practice
              Research talks

### Daily schedule

- 09:00-12:00: Morning lecture and practical
- 12:00-13:00: Lunch
- 13:00-16:00: Afternoon lecture and practical
- 16:00-18:00: Seminar or short field trip
- 16:00-18:00: Field trip, seminar, or other activity
- 18:00-19:00: Dinner
