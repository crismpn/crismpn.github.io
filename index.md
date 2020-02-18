---
layout: page
title: About me
subtitle: Doctoral Researcher at University of Minho

---

Member of KEG (Knowledge Engineering Group) at <a href="https://www.uminho.pt/PT" target="_blank">University of Minho's</a> <a href="http://algoritmi.uminho.pt" target="_blank">Algoritmi Research Center</a>. 
Invited Assistant Professor, teaching Knowledge Discovery.

---

##  Interests

<div class="main-explain-area jumbotron">
    <strong><i class="fa fa-book"></i> Research:</strong><br> 
        Data Mining | Electronic Health Record | Interoperability | Business Intelligence | Knowledge Extraction | Decision Support Systems  <br><br><br>

</div> 

---

## Lastest publications

#### Book chapters
{% for pub in site.data.publications.bookchaps limit: 1%}
 {% assign counter = counter | plus:1 %}
  {{ counter }}. {{ pub.authors }} ({{ pub.year }}). _**{{ pub.title }}**_. {% if pub.volume %}{{ pub.volume }},{% endif %} {% if pub.booktitle %}{{ pub.booktitle }}{% endif %} {% if pub.conference %}{{ pub.conference }}{% endif %}. <a href="{{ pub.url }}" target="_blank"><i class="fa fa-external-link" aria-hidden="true"></i></a> 
{% endfor %}

#### Journals
{% for pub in site.data.publications.journals limit: 1%}
 {% assign counter = counter | plus:1 %}
  {{ counter }}. {{ pub.authors }} ({{ pub.year }}). _**{{ pub.title }}**_. {{pub.journal}}{% if pub.volume %}, {{ pub.volume }}{% endif %}{% if pub.publisher %}, {{ pub.publisher}}{% endif %}. <a href="{{ pub.url }}" target="_blank"><i class="fa fa-external-link" aria-hidden="true"></i></a>  
{% endfor %}

#### Conf. Papers
{% for pub in site.data.publications.confs limit: 1%}
 {% assign counter = counter | plus:1 %}
  {{ counter }}. {{ pub.authors }} ({{ pub.year }}). _**{{ pub.title }}**_. {{ pub.conference }} <a href="{{ pub.url }}" target="_blank"><i class="fa fa-external-link" aria-hidden="true"></i></a>  
{% endfor %}

<p><a href="/publications"><i class="fa fa-plus-square"></i> <strong>Show More</strong></a></p>
