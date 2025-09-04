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
- ![HH icon](https://i.hh.ru/images/logos/svg/hh.ru.svg){: .icon}[Резюме на hh](https://hh.ru/resume/2eda4b93ff0ed8f2ba0039ed1f38384d4c7761)


## Мои проекты  
<div class="game-grid">
{% assign sorted_projects = site.projects | sort: "priority" %}
{% for project in sorted_projects %}
  <div class="game-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <a href="{{ project.url | relative_url }}">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image" />
    </a>
    <!-- <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image"> -->
  </div>
{% endfor %}
</div>
