---
layout: page
title: portfolio
permalink: /portfolio/
hide: false
---
<div class="work">
  <h2>My Work</h2>
  {% for project in site.portfolio  %}
      <li>
        <img src="{{ project.thumbnail-path }}" alt="{{ project.title }}"/>
        <a href="{{ project.url }}">{{ project.title }}</a>
        <p>{{ project.short-description }}</p>
      </li>
  {% endfor %}
</div>
