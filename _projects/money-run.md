---
layout: game-page
title: "Money run"
description: "Казуальный 3D раннер"
image: "/assets/images/money-run-preview.png"  # Превью для карточки
priority: 4
---

## Геймплейное видео:
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/hYA5fsOqavc"
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe src="https://vkvideo.ru/video_ext.php?oid=-231591601&id=456239021&hd=2&hash=baa042c8113ad7f7&autoplay=1" width="853" height="480" style="background-color: #000" allow="encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" frameborder="0" allowfullscreen></iframe>
</div>

## Скриншоты
 <div class="gallery">
    {% for screenshot in site.money-run-screenshots %}
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
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/Tests/tree/RichRun)

## Технологии  
- Zenject
- DOTween
- Cinemachine

## Достигнутые в ходе работы цели
- Управление персонажем с помощью Touch в Input System
- Реализация анимации перемещения с использованием Blend Tree
- Переключение состояния аниматора при смене модели игрока