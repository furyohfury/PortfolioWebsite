---
layout: default
title: furyohfury's Unity портфолио
description: ""
---

## Привет 👋
Меня зовут Артем, я Unity-разработчик.
На этом сайте вы можете посмотреть на прототипы(и не только) проектов, сделанных мной!
## Контакты:
- Почта - artemkuzminikh@gmail.com
- Телеграм - t.me/artemkuzminikh
- Телефон - +79670201329

[Мой GitHub](https://github.com/furyohfury)  
[Мой itch.io](https://furyohfury.itch.io/)


## Мои проекты  
<div class="game-grid">
{% for project in site.projects %}
  <div class="game-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
  </div>
{% endfor %}
</div>
