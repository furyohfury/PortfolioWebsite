---
layout: game-page
title: "Don't upset the Santa"
description: "Казуальная игра про сортировку с возможностью удаленного редактирования конфигов"
image: "/assets/images/santa-preview.png"  # Превью для карточки
priority: -5
lang: ru
---
{% assign t = site.data.t[page.lang] %}
## {{ t.gameplay_video }}
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/uxJ3RavduUo" 
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe src="https://vkvideo.ru/video_ext.php?oid=-231591601&id=456239023&hash=eb36a0dfb8f81cc6&hd=4" width="853" height="480" allow="autoplay; encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" frameborder="0" allowfullscreen></iframe>
</div>

## {{ t.screenshots }}
<div class="gallery">
  {% for screenshot in site.santa-screenshots %}
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
- [Yandex games](https://yandex.ru/games/app/509764?draft=true&lang=ru)
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/FreeRealEstate/tree/conveyors-yandex)

## {{ t.game_technologies }}
- Yandex games SDK [Link](https://assetstore.unity.com/packages/tools/integration/plugin-your-games-unified-api-for-webgl-and-mobile-stores-302343)
- DOTween
- Awaitable

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.santa_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>