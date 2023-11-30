---
title: "Courtesy and Chamber Copy Delivery - Los Angeles Courts"
date: 2019-01-28T15:15:26+10:00
weight: 2
---

Courtesy Copy Printing & Delivery to the following Courthouses 


> *Price include only the first 20 pages, after the first 20 pages….$.20 per page
> 
> *Blue Backing, if required is included.
>
> *Exhibit Tabs are considered a page. 



<div class="container pt-6 pb-6">
    <div class="row">
        {% assign promoted_teams = site.team | where: "promoted", true | sort: "weight" %}
        {% for team in promoted_teams %}
        <div class="col-12 col-md-6 mb-2">
            <div class="team team-summary team-summary-large">
                {% if team.image %}
                <div class="team-image">
                    <img width="90" height="90" alt="{{ team.title }}" class="img-fluid mb-2" src="{{ team.image | relative_url }}" />
                </div>
                {% endif %}
                <div class="team-meta">
                    <h2 class="team-name"><a href="{{ team.url | relative_url }}">{{ team.title }}</a></h2>
                    <p class="team-description">{{ team.jobtitle }}</p>
                    {% if team.linkedinurl %}
                    <a target="_blank" href="{{ team.linkedinurl }}" rel="noreferrer">LinkedIn</a>
                    {% endif %}
                </div>
                <div class="team-content">{{ team.content | truncate: 120 }}</div>
            </div>
        </div>
        {% endfor %}
    </div>
    <div class="row pt-6 pb-6">
        {% assign teams = site.team | where: "promoted", empty | sort: "weight" %}
        {% for team in teams %}
        <div class="col-12 col-md-4 mb-3">
            <div class="team team-summary">
                {% if team.image %}
                <div class="team-image">
                    <img width="60" height="60" alt="{{ team.title }}" class="img-fluid mb-2" src="{{ team.image | relative_url }}" />
                </div>
                {% endif %}
                <div class="team-meta">
                    <h2 class="team-name"><a href="{{ team.url | relative_url }}">{{ team.title }}</a></h2>
                    <p class="team-description">{{ team.jobtitle }}</p>
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</div>






{% if site.data.onlinelegalcourierservicescourts %}
<div class="strip strip-grey">
  <div class="container pt-6 pb-6 pt-md-10 pb-md-10">
    <div class="row justify-content-start">

      {% for feature in site.data.onlinelegalcourierservicescourts %}
      <div class="col-12 col-md-6 col-lg-4 mb-2">
        <div class="feature">
          {% if feature.image %}
          <div class="feature-image"><img alt="{{ feature.title }} logo" src="{{ feature.image.url | relative_url }}" width="{{ feature.image.width }}" height="{{ feature.image.height }}" /></div>
          {% endif %}
          <h2 class="feature-title">{{ feature.title }}</h2>
          <div class="feature-content">{{ feature.description }}</div>
        </div>
      </div>
      {% endfor %}

    </div>
  </div>
</div>
{% endif %}


{% if site.data.onlinelegalcourierlosangelesprices %}
<div class="strip strip-grey">
  <div class="container pt-6 pb-6 pt-md-10 pb-md-10">
    <div class="row justify-content-start">

      {% for feature in site.data.onlinelegalcourierlosangelesprices %}
      <div class="col-12 col-md-6 col-lg-4 mb-2">
        <div class="feature">
          {% if feature.image %}
          <div class="feature-image"><img alt="{{ feature.title }} logo" src="{{ feature.image.url | relative_url }}" width="{{ feature.image.width }}" height="{{ feature.image.height }}" /></div>
          {% endif %}
          <h2 class="feature-title">{{ feature.title }}</h2>
          <div class="feature-content">{{ feature.description }}</div>
        </div>
      </div>
      {% endfor %}

    </div>
  </div>
</div>
{% endif %}

{% if site.data.onlinelegalcourierservices %}
<div class="strip strip-grey">
  <div class="container pt-6 pb-6 pt-md-10 pb-md-10">
    <div class="row justify-content-start">

      {% for feature in site.data.onlinelegalcourierservices %}
      <div class="col-12 col-md-6 col-lg-4 mb-2">
        <div class="feature">
          {% if feature.image %}
          <div class="feature-image"><img alt="{{ feature.title }} logo" src="{{ feature.image.url | relative_url }}" width="{{ feature.image.width }}" height="{{ feature.image.height }}" /></div>
          {% endif %}
          <h2 class="feature-title">{{ feature.title }}</h2>
          <div class="feature-content">{{ feature.description }}</div>
        </div>
      </div>
      {% endfor %}

    </div>
  </div>
</div>
{% endif %}




<div class="strip">
  <div class="container pt-6 pb-6 pb-md-10">
    <div class="row justify-content-start">
      {% assign limit = site.home.limit_services | default: 6 %}
      {% for service in site.services limit: limit %}
      <div class="col-12 col-md-4 mb-1">
        <div class="service service-summary">
          <div class="service-content">
            <h2 class="service-title">
              <a href="{{ service.url | relative_url }}">{{ service.title }}</a>
            </h2>
            <p>{{ service.content | markdownify | strip_html | truncate: 100 }}</p>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
    <div class="row justify-content-center">
      <div class="col-auto">
        <a class="button button-primary" href="{{ "services" | relative_url }}">View All Onlinelegalcourier.com Services</a>
      </div>
    </div>
  </div>
</div>


