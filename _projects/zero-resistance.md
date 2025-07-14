---
layout: default
title: "Zero resistance"
description: "2D сайдскроллер в космосе. Разработана в ходе геймджема"
image: "/assets/images/zero-resistance-preview.png"  # Превью для карточки
---

## Геймплейное видео:
<iframe 
  width="960" 
  height="540" 
  src="https://www.youtube.com/embed/3abxonV4zNg" 
  frameborder="0" 
  allowfullscreen>
</iframe>

## Скриншоты
 <div class="gallery">
    {% for screenshot in site.zero-resistance-screenshots %}
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
- ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Windows, WebGl](https://furyohfury.itch.io/zeroresistanceweb3)

## Технологии  
- Zenject
- DOTween

## Достигнутые в ходе работы цели
- Построение небольшой игры в ходе трехдневного геймджема