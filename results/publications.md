---
title: Publications
---

{% assign tag_list = site.publications | map: 'tags' | join: ',' | split: ',' | uniq %}

<b>Filter by tag:</b> &nbsp; {% for tag in tag_list%} <a href="javascript:show('{{tag}}')">#{{tag}}</a> &nbsp; {% endfor %} <a href="javascript:show('_all')">Show All</a> 

<br/>

{% for paper in site.publications %}

<div class="paper" tags="{% for tag in paper.tags %}{{tag}}{% if forloop.last == false %}{{" "}}{% endif %}{% endfor %} _all">
  <h2>{{ paper.title }}</h2>

  <ul>

  <li>Published at: {{ paper.pubvenue }}</li>
  <li>Authors: <i>{{ paper.authors }}</i></li>
  <li>Date: <i>{{ paper.date | date: "%B %Y" }}</i></li>
  <li>Tags: {%- for tag in paper.tags -%} &nbsp; #{{tag}} {%- endfor -%}</li>

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

   <br/><br/><br/>

</div>

{% endfor %}

<script>

function show_all() {

    if(fragment == "") {

        var papers = document.getElementsByClassName("paper");

        for(i = 0; i < papers.length; i++) {
            papers[i].style.display = "block";
        }
    }
}

function show(selection) {

    var papers = document.getElementsByClassName("paper");
    for(i = 0; i < papers.length; i++) {
        if(papers[i].getAttribute("tags").split(" ").includes(selection)) {
            papers[i].style.display = "block";
        } else {
            papers[i].style.display = "none";
        }
    }
}

var fragment = window.location.hash.substring(1);

if(fragment == "") {
    show_all();
} else {
    show(fragment);
}

</script>

