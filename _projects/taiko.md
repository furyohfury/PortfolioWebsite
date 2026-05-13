---
layout: game-page
title: "Taiko"
description: "Ритм-игра taiko"
image: "/assets/images/taiko-preview.png"  # Превью для карточки
priority: 3
lang: ru
---
{% assign t = site.data.t[page.lang] %}
## {{ t.gameplay_video }}
<div class="video-grid">
<iframe 
  width="853" 
  height="480" 
  src="https://www.youtube.com/embed/Rv4SX6Viylc" 
  frameborder="0" 
  allowfullscreen>
</iframe>
<iframe src="https://vkvideo.ru/video_ext.php?oid=-231591601&id=456239022&hd=2&hash=c26e640104b6f2cc&autoplay=1" width="853" height="480" style="background-color: #000" allow="encrypted-media; fullscreen; picture-in-picture; screen-wake-lock;" frameborder="0" allowfullscreen></iframe>
</div>

## {{ t.screenshots }}
<div class="gallery">
  {% for screenshot in site.taiko-screenshots %}
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
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/FreeRealEstate/tree/Taiko)
- [GoogleDrive .apk](https://drive.google.com/file/d/1CwqQrRcmiv9DTQFTY_kUM9-Rbo4HtuHo/view?usp=sharing)

## {{ t.game_technologies }}
- Firebase
- Addressables
- VContainer
- DOTween
- R3 (UniRx)
- UniTask

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.taiko_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>