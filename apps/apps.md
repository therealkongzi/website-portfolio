---
title: My Apps
layout: archive
permalink: /apps/
---

# My iOS Apps

Here are the apps I'm currently building and maintaining.

<div class="grid">
  {% for app in site.pages %}
    {% if app.permalink contains '/apps/' and app.title != 'My Apps' %}
      <div class="grid__item">
        <h2><a href="{{ app.permalink }}">{{ app.title }}</a></h2>
        <p>{{ app.excerpt }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>
