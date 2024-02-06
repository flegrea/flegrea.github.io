---
title: Publications
---
{% for paper in site.publications %}

  <h2>{{ paper.title }}</h2>

  <ul>

  <li>Published at: {{ paper.pubvenue }}</li>
  <li>Authors: <i>{{ paper.authors }}</i></li>
  <li>Date: <i>{{ paper.date | date_to_string }}</i></li>
  <li>Link: <a href="{{ paper.link }}">{{ paper.link }}</a></li>

  </ul>

  <p>{{ paper.abstract | markdownify }}</p>

{% endfor %}
