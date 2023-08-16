---
layout: articles
title: Team
---
<div class="article-list grid grid--sm grid--p-3">
{% for people in site.data.people %}
  <div class="cell cell--12 cell--md-6 cell--lg-4">
    <div class="card card--flat">
      <div class="card__image"><img src="{{ people.picture }}" /></div>
      <div class="card__content">
        <header>
          <h3>{{ people.name }}</h3>
          <h4> {{ people.role }} </h4>
        </header>
      </div>
    </div>
  </div>
{% endfor %}
</div>