---
layout: default
title: Мое Unity портфолио
---

## Привет 👋
Меня зовут Артем, я Unity-разработчик.

<div class="two-column-layout">

  <div class="column-left">
    
    <h3>Опыт работы</h3>
    <p>Здесь можно описать ваши Unity проекты и стаж.</p>

    <h3>Мои проекты</h3>
    <div class="game-grid">
      {% assign sorted_projects = site.projects | sort: "priority" %}
      {% for project in sorted_projects %}
        <div class="game-card">
          <h4><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h4>
          <img src="{{ project.image | relative_url }}" class="project-image" />
        </div>
      {% endfor %}
    </div>

  </div>

  <div class="column-right">

    <div class="info-block">
      <h3>Навыки</h3>
      <ul>
        <li>C# / .NET</li>
        <li>Unity (URP, DOTween)</li>
        <li>HLSL Shaders</li>
        <li>WebGL / Yandex Games</li>
      </ul>
    </div>

    <div class="info-block">
  <h3>Контакты</h3>
  <ul>
    <li>
      - Почта - [artemkuzminikh@gmail.com](mailto:artemkuzminikh@gmail.com)
    </li>
    <li>
      - Телеграм - [t.me/artemkuzminikh](https://t.me/artemkuzminikh)
    </li>
    <li>
      - ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[Мой GitHub](https://github.com/furyohfury)  
    </li>
    <li>
      - ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Мой itch.io](https://furyohfury.itch.io/)
    </li>
    <li>
      - ![HH icon](https://i.hh.ru/images/logos/svg/hh.ru.svg){: .icon}[Резюме на hh](https://hh.ru/resume/2eda4b93ff0ed8f2ba0039ed1f38384d4c7761)
    </li>
  </ul>
</div>

  </div>

</div>