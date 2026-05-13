---
layout: game-page
title: "Iron frontier"
description: "Участие в разработке карточной стратегии-рогалика в составе инди-студии Bibamus"
image: "/assets/images/iron-frontier-preview.jpg"  # Превью для карточки
priority: -4
lang: ru
---
{% assign t = site.data.t[page.lang] %}
## {{ t.gameplay_video }}
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

## {{ t.screenshots }}
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

## {{ t.game_links }}
- [Steam](https://store.steampowered.com/app/2131290/Iron_Frontier/)

## {{ t.game_technologies }}
- Zenject
- Awaitable
- DOTween

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.iron_frontier_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>