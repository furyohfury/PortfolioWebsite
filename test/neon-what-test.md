---
layout: default
title: "Neon What"
description: "2D платформер-пазл с уровнями на время. Клон игры Neon White"
image: "/assets/images/neon-what-preview.png"  # Превью для карточки
---
{% include gallery.html %}

## Скриншоты
<div style="display: flex; gap: 10px;">
    <a href="{{ '/assets/images/neon-what-preview.png' | relative_url }}" target="_blank">
        <img src="{{ '/assets/images/neon-what-preview.png' | relative_url }}" width="100" />
    </a>
    <a href="{{ '/assets/images/neon-what-preview.png' | relative_url }}" target="_blank">
        <img src="{{ '/assets/images/neon-what-preview.png' | relative_url }}" width="100" />
    </a>
    <a href="{{ '/assets/images/neon-what-preview.png' | relative_url }}" target="_blank">
        <img src="{{ '/assets/images/neon-what-preview.png' | relative_url }}" width="100" />
    </a>
</div>

## Скриншоты с превью
<!-- Подключаем стили Lightbox -->
<link href="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.3/css/lightbox.min.css" rel="stylesheet">

<!-- Галерея с превью -->
<div style="display: flex; gap: 10px; margin: 20px 0;">
    <!-- Первая картинка -->
    <a href="{{ '/assets/images/neon-what-preview.png' | relative_url }}" data-lightbox="gallery" data-title="Описание 1">
        <img src="{{ '/assets/images/neon-what-preview.png' | relative_url }}" width="150" />
    </a>
    <!-- Вторая картинка -->
    <a href="{{ '/assets/images/neon-what-preview.png' | relative_url }}" data-lightbox="gallery" data-title="Описание 2">
        <img src="{{ '/assets/images/neon-what-preview.png' | relative_url }}" width="150" />
    </a>
</div>

<!-- Подключаем скрипт Lightbox -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.3/js/lightbox.min.js"></script>

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