---
title: "Wildlife Genomics Course, 2nd Edition"
layout: gridlay
excerpt: "Wildlife Genomics Course, 2nd Edition"
sitemap: false
permalink: wildlife_genomics_course/
---


# Course: Introduction to wildlife genomics

<figure>
  <img src="{{ site.url }}{{ site.baseurl }}/images/slider/logo.png" style="width: 840px" alt="Wildlife genomics course">
</figure>

## General info

**Date:** August 12-23, 2024 <br/>
**Place:** Pwani University, Kilifi, Kenya  <br/>
**Organized by:** Pwani University, University of Copenhagen, the African BioGenome Project. <br/>
**Price:** Free <br/>
**Includes:** All teaching, breakfast and lunch on course days. Accommodation is NOT included. <br/>
**Sign up:** <a href="https://forms.gle/FkEj9tqE4BuFst3w6"> apply here </a>  <br/>
**Contact:** For questions write to s.wambua@pu.ac.ke or anubhabkhan@gmail.com <br/>

# Content
The course is a comprehensive introduction to population genetics and the use of genomics tools especially in the context of wildlife research and conservation. All sessions will have hands-on data analysis.
Topics: fundamental population genetics, Next-generation sequencing, genomic data analysis, application of genomics to wildlife census, trafficking and population management

## Intended Learning Outcome
- Importance of population genetics and genomics in wildlife conservation and management
- Understand what NGS short-read data looks like when it comes from the sequencer, and have an overview of what needs to be done to it before population genetic analyses can be done. 
- Understand various measures of genetic diversity, inbreeding, population structure, relatedness
- Estimate demographic history and its consequnces for population survival or extinction
- Application of genomics in wildlife management
- Metagenomes and their analysis

## Instructors

{% assign number_printed = 0 %}
{% for yml in site.data.course %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if yml.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <h2>{{ yml.name }}</h2>
  <pubtit>{{ yml.title }}</pubtit>
	  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ yml.image }}" class="img-responsive" width="33%" style="float: left" alt="{{ yml.name | escape }}" />
  <p>{{ yml.description }} <strong><a href="{{ yml.website }}">website</a></strong></p>  
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



## Time and place

The course took place from Monday August 12th to Friday August 23rd 2024 at Pwani University in Kilifi, Kenya. Lectures, computer exercises and research talks were held on campus.
You are required to bring a laptop to the course. 


# Program (preliminary)

### Day1 (12th August, 2024)
    - Theory: Introduction to population genetics, conservation genetics, evolution and genomics. 
      What information is provided by DNA? NGS vs Sanger sequencing
    - Practicals: Basic linux1. How to get help?

### Day2 (13th August, 2024)
    - Theory: how to design your wildlife genomics project?
    - Practicals: Basic linux2. Accessing freely available data for research
    
### Day3 (14th August, 2024)
    - Theory: Sequencing platforms and how they work? What data type do you need?
    - Practicals: Visualizing sequencing outputs. First steps after obtaining data: trimming and mapping raw data

### Day4 (15th August, 2024)
    - Theory: 
    - Practicals: mapping, SNP calling, SNP filtering step1

### Day5 (16th August, 2024)
     - Theory: Hardy Weinberg equilibrium, genetic diversity, various measures of diversity and relevance 
       for wildlife
     - Practicals: SNP filtering step2, Measuring genetic diversity: heterozygosity, PI and allelic 
       richness. Exploring effects of sample size

### Day6 (19th August, 2024)
     - Theory: Population structure, relatedness, inbreeding
     - Practicals: PCA, admixture, relatedness and inbreeding 

### Day7 (20th August, 2024)
    - Theory: Demographic history, why is it important? How to estimate it?
    - Practicals: PSMC, GONE

### Day8 (21st August, 2024)
    - Theory: selection/load. How to measure it?
    - Practicals: Identifying deleterious alleles and signatures of selection

### Day9 (22nd August, 2024)
    - Theory: Shades and hues of metagenomics
    - Practicals: DADA2

### Day10 (23rd August, 2024)
    - Theory: Practical considerations for metagenomic experiments
    - Practicals: Lab demo and DADA2

    
