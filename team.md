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

<h2>PhD Students</h2>
<div class="article-list grid grid--sm grid--p-3">
{% for people in site.data.people %}
  {% if people.role == "PhD" %}
   <div class="cell cell--12 cell--md-4 cell--lg-3">
      <div class="card card--flat">
        <div class="card__image">
          <img class="image" src="{{ people.picture }}" />
            <div class="overlay overlay--bottom">
              <header>
                {{ people.name }}
              </header>
            </div>
        </div>
      </div>
    </div>
  {% endif %}
{% endfor %}
</div>

<h2>Collaborations and Postdoctoral Researchers</h2>
<div class="article-list grid grid--sm grid--p-3">
{% for people in site.data.people %}
  {% if people.role != "PhD" %}
   <div class="cell cell--12 cell--md-4 cell--lg-3">
      <div class="card card--flat">
        <div class="card__image">
          <img class="image" src="{{ people.picture }}" />
            <div class="overlay overlay--bottom">
              <header>
                {{ people.name }}
                {{ people.role }}
              </header>
            </div>
        </div>
      </div>
    </div>
  {% endif %}
{% endfor %}
</div>
<div>
  <h2>Masters Students</h2>
  <div class="row">
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "MS" %}
          {% if people.col == 1 %}
            <p>{{ people.name }}</p>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "MS" %}
          {% if people.col == 2 %}
            <p>{{ people.name }}</p>
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
            <p>{{ people.name }}</p>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.people_text %}
        {% if people.role == "BS" %}
          {% if people.col == 2 %}
            <p>{{ people.name }}</p>
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
          <p> {{ people.name }} ({{ people.role }})</p>{% if people.now %}<i> {{ people.now }}</i> {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.col == 2 %}
          <p>{{ people.name }} ({{ people.role }})</p>{% if people.now %}<i> {{ people.now }}</i> {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>
</div>