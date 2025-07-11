---
layout: default
title: furyohfury's Unity портфолио
description: ""
---

## Привет 👋
Меня зовут Артем, я Unity-разработчик.
Здесь вы можете узнать обо мне и посмотреть на прототипы(и не только) моих проектов!
## Контакты:
- Почта - [artemkuzminikh@gmail.com](mailto:artemkuzminikh@gmail.com)
- Телеграм - [t.me/artemkuzminikh](https://t.me/artemkuzminikh)
- Телефон - +79670201329
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[Мой GitHub](https://github.com/furyohfury)  
- ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Мой itch.io](https://furyohfury.itch.io/)


## Мои проекты  
<div class="game-grid">
{% for project in site.projects %}
  <div class="game-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
  </div>
{% endfor %}
</div>
