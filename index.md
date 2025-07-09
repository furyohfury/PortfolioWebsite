---
layout: default
title: Главная
---

# Привет! ??  
Меня зовут Артем, я Unity-разработчик.  

## ?? Мои проекты  
<div class="game-grid">
  {% for project in site.projects %}
    <div class="game-card">
      <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
      <img src="{{ project.image }}" alt="{{ project.title }}">
    </div>
  {% endfor %}
</div>
