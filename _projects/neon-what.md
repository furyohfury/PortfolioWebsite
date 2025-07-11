---
layout: default
title: "Neon What"
description: "2D платформер-пазл с уровнями на время. Клон игры Neon White"
image: "/assets/images/neon-what-preview.png"  # Превью для карточки
---

## Геймплейное видео:
<iframe 
  width="560" 
  height="315" 
  src="https://www.youtube.com/embed/ВАШ_ID_ВИДЕО" 
  frameborder="0" 
  allowfullscreen>
</iframe>

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