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
          <b> Dinesh Bharadia </b>
          <p> Principal Investigator, Associate Professor ECE </p>
        </header>
      </div>
    </div>
  </div>
  <div class="cell cell--12 cell--md-6 cell--lg-4">
    <div class="card card--flat">
      <div class="card__image"><img src="/assets/images/teampic/fred.jpg" /></div>
      <div class="card__content">
        <header>
          <b>Fred Harris </b>
          <p> Honorable Member, Adjunct Professor ECE </p>
        </header>
      </div>
    </div>
  </div>
</div>

<h3>PhD Students</h3>
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

<h3>Collaborations and Postdoctoral Researchers</h3>
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
  <h3>Masters Students</h3>
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
  <h3>Undergraduate Students</h3>
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
  <h3>Alumni and Interns</h3>
  <div class="row">
    <h5>PhD and Postdocs</h5>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "PhD" or people.role == "Postdoc" %}
          {% if people.col == 1 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}<i>, {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "PhD" or people.role == "Postdoc" %}
          {% if people.col == 2 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}, <i> {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>

  <div class="row">
    <h5>Masters</h5>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "MS" %}
          {% if people.col == 1 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}<i>, {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "MS" %}
          {% if people.col == 2 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}, <i> {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>

  <div class="row">
    <h5>Undergraduate</h5>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "BS" %}
          {% if people.col == 1 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}<i>, {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "BS" %}
          {% if people.col == 2 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}, <i> {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>

  <div class="row">
    <h5>SRIP</h5>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "SRIP" %}
          {% if people.col == 1 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}<i>, {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "SRIP" %}
          {% if people.col == 2 %}
            <div class="row">
              {{ people.name }} <i>{{ people.year }}</i>{% if people.now %}, <i> {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>

  <div class="row">
    <h5>Summer Interns</h5>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "Intern" %}
          {% if people.col == 1 %}
            <div class="row">
              {{ people.name }} <i>{{ people.school }}</i>{% if people.now %}<i>, {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
    <div class="column">
      {% for people in site.data.alumni %}
        {% if people.role == "Intern" %}
          {% if people.col == 2 %}
            <div class="row">
              {{ people.name }} <i>{{ people.school }}</i>{% if people.now %}, <i> {{ people.now }}</i> {% endif %}
            </div>
          {% endif %}
        {% endif %}
      {% endfor %}
    </div>
  </div>
</div>