---
layout: game-page
title: "Iron frontier"
description: "Участие в разработке карточной стратегии-рогалика в составе инди-студии Bibamus"
image: "/assets/images/iron-frontier-preview.jpg"  # Превью для карточки
priority: 0
---

## Геймплейное видео:
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/C0BmLHdaJBw" 
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe 
src="https://vk.com/video_ext.php?oid=-227503186&id=456239030&autoplay=0" 
width="853" height="480" 
allow="encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" 
frameborder="0" 
allowfullscreen>
</iframe>
</div>

## Скриншоты
 <div class="gallery">
    {% for screenshot in site.iron-frontier-screenshots %}
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
- [Steam](https://store.steampowered.com/app/2131290/Iron_Frontier/)

## Технологии
- Zenject
- Awaitable
- DOTween

## Достигнутые в ходе работы цели
- Выполнение задач в составе игровой инди-студии
- Работа над различными слоями проекта: кор-геймплеем, интерфейсом, мета прогрессией и др.