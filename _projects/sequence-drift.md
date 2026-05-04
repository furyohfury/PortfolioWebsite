---
layout: game-page
title: "Sequence drift"
description: "Разработка игры в ходе Ludum dare 59 в паре с художником"
image: "/assets/images/sequence-drift-preview"  # Превью для карточки
priority: -2
---

## Играть в браузере:
<iframe frameborder="0" src="https://itch.io/embed-upload/17238634?color=333333" allowfullscreen="" width="1280" height="720"><a href="https://furyohfury.itch.io/sequence-drift">Play Sequence Drift on itch.io</a></iframe>

## Скриншоты
<div class="gallery">
  {% for screenshot in site.iron-frontier-screenshots %}
    <a href="{{ screenshot.image | relative_url }}" 
       data-lightbox="gallery" 
       data-title="Скриншот"
       {% if forloop.first == false %} style="display: none;" {% endif %}>
       
       <img src="{{ screenshot.image | relative_url }}" alt="Скриншот" class="project-image">
       
       {% if forloop.first %}
         <p style="text-align: center; cursor: pointer;">📸 Нажмите, чтобы посмотреть все скриншоты</p>
       {% endif %}
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
- [Itch.io](https://furyohfury.itch.io/sequence-drift)
- [Ludum Dare] (https://ldjam.com/events/ludum-dare/59/sequence-drift)

## Технологии
- DOTween
- Awaitable

## Достигнутые в ходе работы цели
- Создание небольшой игры для гейм джема за 3 дня
- Работа в качестве разработчика в паре с художником