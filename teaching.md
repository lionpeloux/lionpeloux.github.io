---
layout: default
title: Teaching
subtitle: main ressources about talks and workshops
permalink: /teaching/
---

<h2 class="content-subhead"> Slides from my talks </h2>

<div class="pure-g">
{% for page in site.pages %}
  {% if page.layout == 'slide' %}
    <div class="pure-u-1 pure-u-md-1-2">
      <a class="" href="{{ site.baseurl}}{{page.url}}">
        <img class="pure-img-responsive" src="{{ site.baseurl}}{{page.url}}thumbnail.png" alt="{{ page.title }}">
      </a>
    </div>
    <div class="pure-u-1 pure-u-md-1-2">
      <h1>{{ page.title }}</h1>
      <h2>{{ page.place }}</h2>
      {{ page.description }}
    </div>
  {% endif%}
{% endfor %}
</div>




{% comment %}
<div class="pure-g">
  {% for page in site.pages %}

      <h1>{{ page.title }}</h1>

      <div class="pure-u-1 pure-u-md-1-2">
        <a class="" href="{{ site.baseurl}}{{page.url}}">
          <img class="pure-img-responsive" src="{{ site.baseurl}}{{page.url}}thumbnail.png" alt="{{ page.title }}">
        </a>
      </div>
      <div class="pure-u-1 pure-u-md-1-2">
        <h1>{{ page.title }}</h1>
        {{ page.description}}
      </div>


  {% endfor %}
</div>
{% endcomment %}
