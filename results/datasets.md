---
title: Datasets
---
{% for dataset in site.datasets %}

  <h2>{{ dataset.name }}</h2>

  <ul>

  {% assign paper = site.publications | where:"dataset", dataset.name | first %}

  {% if paper %}
  <li>Paper: {{ paper.title }} (<a href="{{ paper.link }}">link</a>)</li>
  <li>Published at: {{ paper.pubvenue }}</li>
  {% endif %}

  <li>Authors: <i>{{ dataset.authors }}</i></li>
  <li>Date: <i>{{ dataset.date | date_to_string }}</i></li>
  <li>Link: <a href="{{ dataset.link }}">{{ dataset.link }}</a></li>

  </ul>

  <p>{{ dataset.content | markdownify }}</p>

{% endfor %}
