---
title: Who was Ramose?
layout: default
permalink: /ramose/
image: /images/06d.jpg
---

![Vignette from Ramose Book of the Dead]({{site.baseurl}}/images/06d.jpg)  
Detail from an unnumbered spell  

> ‘for becoming an effective one (akh)  
as the great god in the necropolis’,  
Book of the Dead of Ramose

The owner of this particular papyrus is called Ramose. His name and [job titles]({{site.baseurl}}/ramose/background/employment) are written in all the spells to make sure that they work specifically for him. From the writing and the style of clothing shown in the illustrations on the papyrus, as well as from his [burial]({{site.baseurl}}/ramose/background/discovery), we can tell that he lived around 1300 BC.

The document itself is made from individual sheets of papyrus which have been stuck together to form a large roll, which we can estimate to have been more than 20 metres in length. The overall height of the sheets is about 41 cm, which is rather larger than usual. The illustrations of the papyrus are particularly beautiful and there are places where gold has been used. These factors would have meant that Ramose’s Book of the Dead was quite an expensive document. However, his tomb is relatively small which would normally lead us to conclude that he was not particularly wealthy. As a supervisor of royal archivists he would have worked within the scribal section of the government, and so he may have had access to a better quality document than the size of his burial would suggest.


<div class="container mb-3">
  <div class="row">
{% assign rows = site.back.size | divided_by: 2.0 | ceil %}
{% for i in (1..rows) %}
{% assign offset = forloop.index0 | times: 2 %}
{% assign sorted = site.back | sort:"order" %}
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
