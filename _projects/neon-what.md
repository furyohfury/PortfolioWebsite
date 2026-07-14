---
layout: game-page
title: "Neon What"
description: "2D платформер-пазл с уровнями на время. Клон игры Neon White"
image: "/assets/images/neon-what-preview.png"  # Превью для карточки
technologies:
  - Atomic framework
  - Zenject
  - unity-ai
  - DOTween
priority: 1
lang: ru
---
{% assign t = site.data.t[page.lang] %}
## {{ t.gameplay_video }}
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/q-3dstQtX5M" 
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe 
src="https://vkvideo.ru/video_ext.php?oid=-231591601&id=456239017&hd=2&hash=ddcc9bb9b15d6a76" 
width="853" height="480" 
allow="autoplay; encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" 
frameborder="0" 
allowfullscreen>
</iframe>
</div>

## {{ t.screenshots }}
<div class="gallery">
  {% for screenshot in site.neon-what-screenshots %}
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
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/Otus_Homework/tree/Project)
- ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Windows, Android](https://furyohfury.itch.io/neon-what)

## {{ t.game_technologies }}  
- Atomic framework ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/StarKRE22/Atomic)
- Zenject
- unity-ai (FSM)
- DOTween

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.neon_what_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>
