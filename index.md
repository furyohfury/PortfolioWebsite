---
layout: default
title: furyohfury's Unity портфолио
description: null
---

# Привет 👋
Меня зовут Артем, я Unity-разработчик.
На этом сайте вы можете посмотреть на прототипы(и не только) проектов, сделанных мной!

## Мои проекты  
<div class="game-grid">
{% for project in site.projects %}
  <div class="game-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
  </div>
{% endfor %}
</div>
