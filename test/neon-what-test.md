---
layout: default
title: "Neon What"
description: "2D платформер-пазл с уровнями на время. Клон игры Neon White"
image: "/assets/images/neon-what-preview.png"  # Превью для карточки
---


## Скриншоты
<div style="display: flex; gap: 10px;">
    <a href="/assets/images/neon-what-preview.png" target="_blank">
        <img src="/assets/images/neon-what-preview.png" width="100" />
    </a>
    <a href="/assets/images/neon-what-preview.png" target="_blank">
        <img src="/assets/images/neon-what-preview.png" width="100" />
    </a>
    <a href="/assets/images/neon-what-preview.png" target="_blank">
        <img src="/assets/images/neon-what-preview.png" width="100" />
    </a>
</div>

## Ссылки  
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/Otus_Homework/tree/Project)
- ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Windows, Android](https://furyohfury.itch.io/neon-what)

## Технологии  
- Atomic framework ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/StarKRE22/Atomic)
- Zenject
- unity-ai (FSM)
- DOTween

## Достигнутые в ходе работы цели
- Построение игровой логики на основе атомарного подхода (если вкратце то, это подход наподобие ECS, но системы находятся внутри сущности, сохраняя разделение данных и логики)
- Построение интерфейса, отделенного от игровой логики, на основе паттернов MVX
- Построение полностью контролируемого игрового цикла (используется, например, для постановки паузы)
- Создание модульной системы сохранения данных
- Реализация усправления с помощью input system. Добавление сенсорного управления для телефонов
- Реализация системы 2D освещения с использованием сгенерированных карт нормалей