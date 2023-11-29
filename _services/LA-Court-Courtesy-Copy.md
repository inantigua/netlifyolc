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


