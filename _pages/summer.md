---
title: "Popgen summer course"
layout: gridlay
excerpt: "Popgen summer course"
sitemap: false
permalink: /summer/
---


# Summer course in analysis of high throughput data for population genetics 2025
<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
        <li data-target="#carousel" data-slide-to="5"></li>
        <li data-target="#carousel" data-slide-to="6"></li>
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        <style>
        .resized-image {
            height: 600px; /* Set the desired height */
            width: auto;   /* Let the browser calculate the width to maintain the aspect ratio */
        }
        </style>
    
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/caucasian.phased.haplonet.merged.anno.png"   class="resized-image" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/check.anno.png"   class="resized-image" alt="Slide 3" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/sikoraPlot.jpeg"  class="resized-image" alt="Slide 5" />
        </div>       
         <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider/plaque.png"  class="resized-image" alt="Slide 6" />
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


## General info

**Date:** August 4-8, 2025 <br/>
**Place:** Copenhagen, Denmark  <br/>
**Organized by:** The Department of Biology, University of Copenhagen <br/>
**Price:** 
 - On site: Free for all PhD students at Danish, Faroese and Greenlandic universities. 200 Euro for all other students.
 - Virtual: Free 

**Includes:**
 - On site: All teaching. Food and accommodation are NOT included in the course fee. <br/>
 - Virtual: includes steaming, server access, and online teaching assistants.

**Sign up:**  [Registration is still open with this link](https://docs.google.com/forms/d/e/1FAIpQLSe-YM5Xjp-xZpognNT5khZaWjV7ai0cHrGGWph1xzx4NnGjSw/viewform?usp=header)  <br/>
**Contact:** For questions write to cphsummercourse@gmail.com  <br/>
**Credit and diploma:** The course is 2.5 ETCS credits and you will recieve a diploma. <br/>
**[github with code](https://github.com/popgenDK/courses/tree/main/summer2025)**

# Content

The course is a comprehensive introduction to a number of topics and common research tools used in analyses of next-generation sequencing (NGS) data. Topics include: genetic drift, natural selection, population structure, recent and ancient admixture, f-statistics and demographic inference. We will cover the theoretical concepts but the main focus is practical use of the methods. Lectures will be combined with hands-on computer exercises.

## Intended Learning Outcome

After the course the student should be able to:

- Use population genetic theory to infer basic population genetics characteristics from genetic data
- Be able to infer ancestry and population structure based on genetic data
- Use NGS data including low depth for population genetic inference.
- Select the optimal strategy for selection scans depending on the population genetics characteristics of the sample population, including taking population structure into account
- Interpret and discuss the results of own analyses and results in the scientific literature

## Instructors


{% assign number_printed = 0 %}
{% for yml in site.data.summer %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if yml.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <h2>{{ yml.name }}</h2>
  <pubtit>{{ yml.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ yml.image }}" class="img-responsive" width="33%" style="float: left" />
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

The course will take place from Monday August 4 to Friday August 8th 2025 at Biocenteret, Ole Maaloes Vej 5, 2200 Copenhagen N. All lectures and computer exercises will take place in room 4.0.24 (i.e. building 4, ground floor, room number 24). This includes research talks. You can enter the building from two sides as shown shown on this map.

## Laptop

You should bring a laptop to the course. We will log into a remote server from the laptop so any laptop will do regardless of operating system.

## Course material

The lecture will be based on a large amount of reading material (articles/notes) that should be read in advance - you can find them here once they are finalized (you will get an email with password). The slides used during the lectures will be made available right before the lectures.


# Program (Preliminary)
### Monday - Introduction to population genetics and NGS data

    09:00 - 09:15 Welcome (Ida Moltke)
    09:15 - 10:15 Lecture 1: Intro to basic population genetic terms and concepts (Fernando Racimo)
    10:30 - 12:00 Computer exercises I
    12:00 - 01:00 Lunch (on your own)
    01:00 - 01:45 Lecture 2: Intro to basic NGS data, data processing and formats (Anders Albrechtsen)
    01:45 - 03:15 Computer exercises II (break at 02.15)
    03:30 - 04:15 Research lecture by TBA. 
    04:15 - 07:00 Reception/social mixer

### Tuesday - Analysis of NGS data and imputation

    09:00 - 10:15 Lecture 3: Estimating allele frequencies, SNP calling and genotype calling from NGS data (Anders Albrechtsen)
    10:30 - 12:00 Computer exercises III
    12:00 - 01:00 Lunch (on your own)
    01:00 - 02:15 Lecture 4: Imputation (Anders Albrecthsen)
    02:30 - 04:00 Computer exercises IV
    04:15 - 05:00 Research lecture by TBA
    Canal boat trip

### Wednesday - Population structure

    09:00 - 10:15 Lecture 5: Population structure and admixture (Ida Moltke)
    10:30 - 12:00 Computer exercises V
    12:00 - 01:00 Lunch (on your own)
    01:00 - 02:15 Lecture 6: D/f statistics and ancient geneflow (Martin Sikora)
    02:30 - 04:00 Computer exercises VI
    04:15 - 05:00 Research lecture by TBA
    
### Thursday – Local ancestry inference and selection

    09:00 - 10:15 Lecture 7: Local ancestry inference (Katia Bougiouri)
    10:30 - 12:00 Computer exercises VII
    12:00 - 01:00 Lunch (on your own)
    01:00 - 02:15 Lecture 8: Detecting genomic regions under (positive) selection (Ida Moltke)
    02:30 - 04:00 Computer exercises VIII
    04:15 - 05:00 Research lecture by TBA

### Friday - PCA and demography

    09:00 - 10:15 Lecture 9: PCA (Anders Albrecthsen)
    10:30 - 12:00 Computer exercises IX
    12:00 - 01:00 Lunch (on your own)
    01:00 - 02:15 Lecture 10: Demography Inference (Shyam Gopalakrishnan)
    02:30 - 04:00 Computer exercises X
    04:15 - 05:00 Research lecture by TBA
    05:00 - ? Farewell drinks

## Evaluation

Participants who have participated actively in all parts of the course and completed all exercises satisfactorily will be awarded a certificate of completion at the end of the course. The work load corresponds to 2.5 ECTS points which will be given for on site participant. Note that this workload includes one week of preparation. Reading material for this is available in the above course program. 
