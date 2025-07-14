---
layout: game-page
title: "Neon What"
description: "2D платформер-пазл с уровнями на время. Клон игры Neon White"
image: "/assets/images/neon-what-preview.png"  # Превью для карточки
---

## Геймплейное видео:
<iframe 
  width="960" 
  height="540" 
  src="https://www.youtube.com/embed/pUgfg5Ovkwk" 
  frameborder="0" 
  allowfullscreen>
</iframe>

## Скриншоты
<div class="gallery">
    <a href="{{ '/assets/images/neon-what-preview.png' | relative_url }}" data-lightbox="gallery" data-title="Описание1">
        <img src="{{ '/assets/images/neon-what-preview.png' | relative_url }}" width="1280" alt="Описание1">
    </a>
    <a href="{{ '/assets/images/pikmin-preview.png' | relative_url }}" data-lightbox="gallery" data-title="Описание2">
        <img src="{{ '/assets/images/pikmin-preview.png' | relative_url }}" width="1280" alt="Описание2">
    </a>
    <a href="{{ '/assets/images/zero-resistance-preview.png' | relative_url }}" data-lightbox="gallery" data-title="Описание3">
        <img src="{{ '/assets/images/zero-resistance-preview.png' | relative_url }}" width="1280" alt="Описание3">
    </a>
</div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.3/js/lightbox-plus-jquery.min.js"></script>
<script>
    // Инициализация с настройками
    lightbox.option({
        'resizeDuration': 200,
        'wrapAround': true,
        'fadeDuration': 200,
        'disableScrolling': true
    })
</script>

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