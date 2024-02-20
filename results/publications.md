---
title: Publications
---
{% for paper in site.publications %}

  <h2>{{ paper.title }}</h2>

  <ul>

  <li>Published at: {{ paper.pubvenue }}</li>
  <li>Authors: <i>{{ paper.authors }}</i></li>
  <li>Date: <i>{{ paper.date | date_to_string }}</i></li>

  </ul>

   {% if paper.link %}
   <a href="{{ paper.link }}" target="_blank"><img src="/assets/images/button_publisher.png"></a>
   {% endif %}
   {% if paper.arxiv %}
   <a href="{{ paper.arxiv }}" target="_blank"><img src="/assets/images/button_arxiv.png"></a>
   {% endif %}
   {% if paper.dataset %}
   {% assign dataset = site.datasets | where:"name", paper.dataset | first %}
   <a href="{{ dataset.link }}" target="_blank"><img src="/assets/images/button_dataset.png"></a>
   {% endif %}

  <p>{{ paper.content | markdownify }}</p>

{% endfor %}
