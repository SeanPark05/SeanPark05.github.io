---
title: "Research"
layout: gridlay
sitemap: false
permalink: /research/
---

<style>
img{
  border-radius: 10px;
}
.col-md-3 {
  margin-top:10px;
  margin-bottom:10px;
  padding:0px;
  display:block;
  overflow:hidden;
  text-align:center;
  display: table-cell;
  background: white;
  border-radius: 20px;
  height: auto;
}
iframe {
  margin:0;
  padding:0;
  width: 175px;
  display: inline;
  vertical-align: middle;
}
.jumbotron{
    padding:3%;
    padding-bottom:10px;
    padding-top:10px;
    margin-top:10px;
    margin-bottom:30px;
    background-color: #252829;
    color: #b0ada8;
}
</style>

### Research

<div class="jumbotron">
<div class="col-md-12 col-sm-12">
<h4>We design heterogeneous catalysts.</h4>

Example description
</div>
</div>

{% if site.data.grants %}
<div class="jumbotron">
### Grants
<ul>
{% for grant in site.data.grants %}
 <li> {{ grant.name }} </li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.awards %}
<div class="jumbotron">
### Awards
<ul>
{% for award in site.data.awards %}
 <li> {{ award.name | replace: "-","&#8211;"}} </li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.people %}
<div class="jumbotron">
### Students and mentoring
<ul>
{% for student in site.data.people %}
 <li> {{ student.name }}, {{student.location}} ({{student.degree}}, {{student.year}}) </li>
{% endfor %}
</ul>
</div>
{% endif %}

<div class="jumbotron">
  <h4>Sponsors</h4>
  <div style='display:block; text-align:center; margin-left:auto; margin-right:auto;'>
 {% for funder in site.data.funders %}<a href="{{ funder.url }}" target="_blank"><img src='{{ site.url }}{{ site.baseurl }}/images/{{ funder.image }}' style='max-height: 80px; max-width: 200px; margin: 1%'/></a>{% endfor %}
  </div>
</div>
