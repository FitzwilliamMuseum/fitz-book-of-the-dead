---
title: "Book of the Dead: spells"
permalink: /explore/book-of-the-dead/spells
layout: default
image: /images/thumbnails/04a.jpg
---

### What are these spells like?
{: .lead }

We use the word ‘spell’ to indicate the individual sections of a Book of the Dead. They are also often referred to as ‘chapters’ or ‘utterances’.

The spells were written down to help the person named in the papyrus to pass safely through any difficult or dangerous situations in the afterlife. One of the most important spells is Chapter or [Spell 125]({{site.baseurl}}/explore/the-book-of-the-dead/spell-125) which usually contains a scene showing the heart of the dead person being weighed against _maat_ (divine order and cosmic balance). The same spell also contains a long text referred to as the Negative Confession, in which the dead person recites a number of things he or she has not done.

[![Vignette from Ramose Book of the Dead]({{site.baseurl}}/images/papyrus/bd72redtext.jpg){: .img-fluid }  
Opening phrase from Spell 72

Each spell, or chapter, of the Book of the Dead is introduced with a phrase, usually written in red, to indicate its purpose. For example, [spell 72](explore/the-book-of-the-dead/spell-72) begins with the phrase (written in red ink) ‘Spell for going out in the day’. (The English word ‘[rubric](http://en.wikipedia.org/wiki/Rubric)’ comes from _ruber_, the Latin word for red.)

The Egyptian _r_ is the word which is usually translated as ‘spell’; the hieroglyph is a simplified image of a mouth, indicating that the meaning of the word is connected with speech or things coming out of a person’s mouth.

Spells are often illustrated with small pictures (vignettes). Some spells contain many vignettes, although the majority have a single illustration. In the case of the [Book of the Dead of Ramose]({{site.baseurl}}/ramose/background/book-of-the-dead), the vignettes are of particularly high quality and we are fortunate that the colours have survived relatively well because they have not been subjected to constant light.

### Ordering and selection of spells
{: .lead  }

The numbering system used today to identify the different spells was first assigned by the German scholar Richard Lepsius in 1842. He published a Ptolemaic Book of the Dead and numbered the individual spells in the order they appeared in that particular papyrus. It is clear that this order was not particularly standardised and the selection of spells varies too from papyrus to papyrus, probably according to the arrangement determined by the scribe responsible.

We do not know whether the person buying a papyrus would necessarily be involved in selecting and ordering the spells. In some cases it is clear that the person whose name appears on the papyrus had purchased one that was already pre-written, with spaces left for the buyer’s name to be inserted. This is not the case with Ramose’s Book of the Dead.

### Spells in the Book of the Dead of Ramose
{: .lead }
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
