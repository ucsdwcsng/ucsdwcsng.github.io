---
title: "News"
layout: article
permalink: /news.html
---

{% for article in site.data.news.news %}
<p><i><font color="gray">{{ article.date }}</font></i><br>
{{ article.headline }}</p>
{% endfor %}