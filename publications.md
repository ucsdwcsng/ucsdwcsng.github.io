---
layout: article
title: Publications
article_header:
  type: overlay
  theme: dark
  background_color: '#203028'
  background_image:
    src: /bearl.jpeg
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
---
<ul>
{% for paper in site.data.publications %}
  <li>
    <a href="{{ paper.paper }}"> {{ paper.title }}</a>
    <i>{{ paper.authors }}</i>
  </li>
{% endfor %}
</ul>

