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

  <details><summary>Abstract</summary>{{ paper.content | markdownify }}</details>
  <br/>

   {%- if paper.link -%}
   <a href="{{ paper.link }}" target="_blank" style="padding: 0.5em 1em;background-color: lightblue;color: black; font-weight: bold">Published paper</a>
   {%- endif -%}

   {%- if paper.arxiv -%}
   &nbsp;
   <a href="{{ paper.arxiv }}" target="_blank" style="padding: 0.5em 1em;background-color: orange; color: black; font-weight: bold">arXiv</a>
   {%- endif -%}

   {%- if paper.dataset -%}
   {% assign dataset = site.datasets | where:"name", paper.dataset | first %}
   <a href="{{ dataset.link }}" target="_blank" style="padding: 0.5em 1em;background-color: red;color: black; font-weight: bold">Dataset</a>
   {%- endif -%}


{% endfor %}
