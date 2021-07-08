---
layout: default
permalink: /explore/book-of-the-dead/
title: Explore the Book of the Dead
---

![Vignette from Ramose Book of the Dead]({{site.baseurl}}/images/papyrus/bod1.jpg){: .img-fluid }

Vignette from Spell 15:
> ‘for worshipping Ra  
when he rises in the horizon until the  
occurrence of his setting in life’

from the Book of the Dead of Ramose

The Book of Dead is a collection of spells, also known as chapters, which were provided in a person’s burial to help him or her to pass successfully into the afterlife and to survive some of the strange perils there. They were most often written on papyrus or linen.

The phrase ‘Book of the Dead’ (German _Totenbuch_) was first coined in 1842 by a German Egyptologist, Karl Richard Lepsius, when he published a Ptolemaic Book of the Dead in the [Museo Egizio at Turin](http://www.museoegizio.it/pages/hp_en.jsp). The numbering system he used to identify the different spells or chapters is still used today, with extra numbers added to spells which did not exist in that particular papyrus.

The ancient Egyptians themselves referred to this text as ‘Recitations (spells) for going out in the day’. The origin of these spells can be traced back through earlier funerary literature to the texts written on the inside of some pyramids around 2350 to 2160 BC.

<div class="container mb-3">
  <div class="row">
  {% assign rows = site.bod.size | divided_by: 2.0 | ceil %}
  {% for i in (1..rows) %}
  {% assign offset = forloop.index0 | times: 2 %}
  {% assign sorted = site.bod | sort:"order" %}
    {% for bod in sorted limit:2 offset:offset %}
    <div class="col-md-4 mb-3">
      <div class="card h-100" >
        <a href="{{site.url}}{{site.baseurl}}{{ bod.permalink }}" class="stretched-link">
          <img class="card-img-top" src="{{site.url}}{{site.baseurl}}{{bod.image}}" alt="Card image cap" width="300" height="300"/>
        </a>
        <div class="card-body">
          <h3 class="lead mt-2">
            <a href="{{site.url}}{{site.baseurl}}{{ bod.permalink }}" class="stretched-link">{{bod.title}}</a>
          </h3>
        </div>
      </div>
    </div>
    {% endfor %}
  {% endfor %}
  </div>
</div>

## Background reading
{: .lead }

<div class="container mb-3">
  <div class="row">
  {% assign rows = site.explore.size | divided_by: 2.0 | ceil %}
  {% for i in (1..rows) %}
  {% assign offset = forloop.index0 | times: 2 %}
  {% assign sorted = site.explore | sort:"order" %}
    {% for bod in sorted limit:2 offset:offset %}
    <div class="col-md-4 mb-3">
      <div class="card h-100" >
        <a href="{{site.url}}{{site.baseurl}}{{ bod.permalink }}" class="stretched-link">
          <img class="card-img-top" src="{{site.url}}{{site.baseurl}}{{bod.image}}" alt="Card image cap" width="300" height="300"/>
        </a>
        <div class="card-body">
          <h3 class="lead mt-2">
            <a href="{{site.url}}{{site.baseurl}}{{ bod.permalink }}" class="stretched-link">{{bod.title}}</a>
          </h3>
        </div>
      </div>
    </div>
    {% endfor %}
  {% endfor %}
  </div>
</div>
