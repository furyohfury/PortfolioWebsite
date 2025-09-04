---
layout: game-page
title: "Card auto-battler"
description: "Карточный автобатлер"
image: "/assets/images/card-autobattler-preview.png"  # Превью для карточки
---

## Геймплейное видео:
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/TrY9toIFcAA" 
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe src="https://vkvideo.ru/video_ext.php?oid=-231591601&id=456239020&hd=2&hash=dbdb1be04ce6dbaa&autoplay=1" width="853" height="480" style="background-color: #000" allow="encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" frameborder="0" allowfullscreen></iframe>
</div>

## Скриншоты
 <div class="gallery">
    {% for screenshot in site.card-autobattler-screenshots %}
  <a href="{{ screenshot.image | relative_url }}" data-lightbox="gallery" data-title="Скриншот">
        <img src="{{ screenshot.image | relative_url }}" alt="Скриншот" class="project-image">
    </a>
{% endfor %}
</div> 

<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.3/js/lightbox-plus-jquery.min.js"></script>
<script>
    // Инициализация с настройками
    lightbox.option({
        'resizeDuration': 200,
        'wrapAround': true,
        'fadeDuration': 200,
        'disableScrolling': false,
        'fitImagesInViewport': false,
        'maxWidth': 1280,
        'maxHeight': 720,
        'positionFromTop': 100
    })
</script>

## Ссылки  
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/Otus_Homework/tree/Eighth_EventBus)

## Технологии  
- DOTween
- Zenject

## Достигнутые в ходе работы цели
- Построение игровой логики на основе паттерна Event bus (шина событий)
- Разделение логики и визуала с помощью отдельных пайплайнов