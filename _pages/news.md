---
title: "News"
layout: textlay
sitemap: false
permalink: /news.html
---

### News

<div class="jumbotron">
{% for article in site.data.news %}
* <b>{{ article.date }}</b>
{{ article.headline }}
{% endfor %}
</div>
