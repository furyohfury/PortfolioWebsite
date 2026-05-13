---
layout: game-page
title: "Totally not pikmin"
description: "3D game with controlling a group of minions."
image: "/assets/images/pikmin-preview.png"  # Превью для карточки
priority: 2
lang: en
---
{% assign t = site.data.t[page.lang] %}
## {{ t.gameplay_video }}
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/Ymxn-hAhA-U" 
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe 
src="https://vkvideo.ru/video_ext.php?oid=-231591601&id=456239019&hd=2&hash=91cd2a2812a6dac4" 
width="853" height="480" 
allow="autoplay; encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" 
frameborder="0" 
allowfullscreen>
</iframe>
</div>

## {{ t.screenshots }}
<div class="gallery">
  {% for screenshot in site.pikmin-screenshots %}
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
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/FreeRealEstate/tree/Pikmin)
- ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Windows](https://furyohfury.itch.io/totally-not-pikmin)

## {{ t.game_technologies }}  
- Unity Behaviour
- R3
- UniTask
- DOTween
- Zenject

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.pikmin_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>