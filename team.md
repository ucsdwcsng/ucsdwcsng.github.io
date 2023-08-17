---
layout: articles
title: Team
---
<div class="article-list grid grid--p-3">
  <div class="cell cell--12 cell--md-6 cell--lg-4">
    <div class="card card--flat">
      <div class="card__image"><img src="/assets/images/teampic/dinesh.jpg" /></div>
      <div class="card__content">
        <header>
          <h3> Dinesh Bharadia </h3>
          <h4> Principal Investigator, Associate Professor ECE </h4>
        </header>
      </div>
    </div>
  </div>
  <div class="cell cell--12 cell--md-6 cell--lg-4">
    <div class="card card--flat">
      <div class="card__image"><img src="/assets/images/teampic/fred.jpg" /></div>
      <div class="card__content">
        <header>
          <h3>Fred Harris </h3>
          <h4> Honorable Member, Adjunct Professor ECE </h4>
        </header>
      </div>
    </div>
  </div>
</div>

<div class="article-list grid grid--sm grid--p-3">
{% for people in site.data.people %}
 <div class="cell cell--12 cell--md-4 cell--lg-3">
    <div class="card card--flat">
      <div class="card__image">
        <img class="image" src="{{ people.picture }}" />
          <div class="overlay overlay--bottom">
            <header>
              <h3>{{ people.name }}</h3>
              <h4> {{ people.role }} </h4>
            </header>
          </div>
      </div>
    </div>
  </div>
{% endfor %}
</div>
<div>
  <h2>Masters Students</h2>
  <div class="row">
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "MS" %}
          {% if people.col == 1 %}
            <h4>{{ people.name }}</h4>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "MS" %}
          {% if people.col == 2 %}
            <h4>{{ people.name }}</h4>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>
  <h2>Undergraduate Students</h2>
  <div class="row">
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "BS" %}
          {% if people.col == 1 %}
            <h4>{{ people.name }}</h4>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "BS" %}
          {% if people.col == 2 %}
            <h4>{{ people.name }}</h4>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>
  <h2>Alumni and Interns</h2>
  <div class="row">
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.col == 1 %}
          <h4>{{ people.name }} ({{ people.role }})</h4>
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.col == 2 %}
          <h4>{{ people.name }} ({{ people.role }})</h4>
        {% endif %}
      {% endfor %}
    </div>
  </div>
</div>