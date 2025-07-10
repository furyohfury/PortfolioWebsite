---
layout: default
title: Главная
---

# Привет! ??  
Меня зовут Артем, я Unity-разработчик.  

## Мои проекты  
<div class="game-grid">
{% for project in site.projects %}
  <div class="game-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
  </div>
{% endfor %}
</div>
