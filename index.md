---
layout: default
title: Мое Unity портфолио
---

## Артем Кузьминых

<div class="info-block" markdown="1">

### Контакты

* **Почта:** [artemkuzminikh@gmail.com](mailto:artemkuzminikh@gmail.com)
* **Телеграм:** [t.me/artemkuzminikh](https://t.me/artemkuzminikh)
* **Github:** ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon} [Мой GitHub](https://github.com/furyohfury)
* **itch.io:** ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon} [Мой itch.io](https://furyohfury.itch.io/)
* **hh.ru:** ![HH icon](https://i.hh.ru/images/logos/svg/hh.ru.svg){: .icon} [Резюме на hh](https://hh.ru/resume/2eda4b93ff0ed8f2ba0039ed1f38384d4c7761)

</div>

<div class="two-column-layout">

  <div class="column-left">
    <div class="info-block">
      <h3>Навыки</h3>
      <ul>
        <li>Unity: 2d/3d Разработка, Tilemap, URP, UI, Addressables,Cinemachine, Animator</li>
        <li>Программирование (C#): Асинхронный код, Реактивное программирование, Test Driven Development</li>
        <li>Основы архитектуры кода и паттерны: ООП, SOLID, GRASP, KISS, DRY, YAGNI, GOF паттерны, MVX, ECS, Atomic</li>
        <li>Популярные фреймворки: ZENJECT, VCONTAINER, DOTWEEN, UNITASK, R3 (UNIRX), ENTITAS ECS</li>
        <li>Сторонние SKD: FIREBASE, Yandex игры, Playfab</li>
        <li>Игровой AI: FSM, BEHAVIOR TREE, NAVMESH</li>
        <li>Инструменты: GIT/GITHUB, Rider, профилирование и оптимизация</li>
      </ul>
    </div>

    <div class="info-block">
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

  </div>

  <div class="column-right">

    <div class="info-block" markdown="1">

###Опыт работы
##Bibamus
#Unity-разработчик
Сентябрь 2025 — настоящее время
*Работа над всеми слоями проекта
*Переработал системы на синглтонах под расширяемую архитектуру
*Доработал интерфейс игры
*Внедрял новые фичи кор-геймплея
*Разработал мета-системы апгрейдов и анлоков
*Разработал сейвлоад систему
И пр.
    </div>

    <div class="info-block">
      <h3>Курсы</h3>
      <ul>
        <li>Отус
05.2024 - 03.2025
Обучение на курсе Unity Game Developer. Professional
- Разработка прототипов на движке Unity
- Изучение принципов архитектуры проектов</li>
        <li>Нетология
04.2023 - 03.2024
Обучение на курсе Разработчик игр на Unity.
- Изучение основ движка Unity
- Основы языка C#
</li>
      </ul>
    </div>

    <div class="info-block">
      <h3>Образование</h3>
      Московский государственный технический
университет имени Н.Э. Баумана
(национальный исследовательский
университет), Москва

Проектирование технических и
технологических комплексов
2015-2020

    </div>

  </div>

</div>
