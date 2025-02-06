---
title: Datasets
---
{% for dataset in site.datasets %}

  <h2>{{ dataset.name }}</h2>

  <ul>

  {% assign paper = site.publications | where:"dataset", dataset.name | first %}

  {% if dataset.authors %}
  <li>Authors: <i>{{ dataset.authors }}</i></li>
  {% elsif paper.authors %}
  <li>Authors: <i>{{ paper.authors }}</i></li>
  {% endif %}

  {% if dataset.date %}
  <li>Date: <i>{{ dataset.date | date_to_string }}</i></li>
  {% elsif paper.date %}
  <li>Date: <i>{{ paper.date | date_to_string }}</i></li>
  {% endif %}

  {% if paper %}
  <li>Paper: {{ paper.title }}</li>
  <li>Published at: {{ paper.pubvenue }}</li>
  {% endif %}

  </ul>

  <a href="{{ dataset.link }}" target="_blank"><img src="/assets/images/button_dataset.png"></a> {% if paper.link %} <a href="{{ paper.link }}" target="_blank"><img src="/assets/images/button_publisher.png"></a> {% endif %} {% if paper.arxiv %} <a href="{{ paper.arxiv }}" target="_blank"><img src="/assets/images/button_arxiv.png"></a> {% endif %}

  <p>{{ dataset.content | markdownify }}</p>

{% endfor %}
