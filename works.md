---
layout: default
title: Works
permalink: /works/
---

# Works

<div class="grid">
  {% assign sorted_works = site.works | sort: "order" %}
  {% for work in sorted_works %}
    <a class="card" href="{{ work.url | relative_url }}">
      <div class="thumb">
        {% if work.image %}
          <img src="{{ work.image | relative_url }}" alt="{{ work.title }}">
        {% endif %}
      </div>
      <div class="card-title">{{ work.title }}</div>
    </a>
  {% endfor %}
</div>