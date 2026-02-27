
---
layout: default
title: Works
permalink: /works/
---

# Works

<div class="grid">
  {% for work in site.works reversed %}
    <a class="card" href="{{ site.baseurl }}{{ work.url }}">
      <div class="thumb">
        {% if work.image %}
          <img src="{{ site.baseurl }}{{ work.image }}" alt="{{ work.title }}">
        {% endif %}
      </div>
      <div class="card-title">{{ work.title }}</div>
    </a>
  {% endfor %}
</div>