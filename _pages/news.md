---
title: "News"
layout: textlay
sitemap: false
permalink: /news.html
---

<style>
.jumbotron{
    padding:3%;
    padding-bottom:10px;
    padding-top:10px;
    margin-top:10px;
    margin-bottom:30px;
    background-color: #252829
}
</style>

### News

<div class="jumbotron">
{% for article in site.data.news %}

* <span style="font-size: 120%"><b>{{ article.date }}</b>   
{{ article.headline }}
</span>
{% endfor %}

</div>
