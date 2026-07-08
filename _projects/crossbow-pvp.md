---
layout: game-page
title: "Crossbow PVP"
description: "Мультиплеерный 1x1 шутер на основе Unity netcode"
image: "/assets/images/crossbow-pvp.png"  # Превью для карточки
priority: -5
lang: ru
---
{% assign t = site.data.t[page.lang] %}
<!--
## {{ t.play_in_browser }} (без СДК яндекс игр)
<div class="unity-container" id="unity-loader-container">
  <div id="game-cover" style="
    position: absolute; 
    width: 100%; 
    height: 100%; 
    background: url('{{ "/assets/images/santa-preview.png" | relative_url }}') no-repeat center; 
    background-size: cover; 
    z-index: 2; 
    display: flex; 
    justify-content: center; 
    align-items: center;
    border-radius: 10px;">
    
    <button class="btn" onclick="loadUnityGame()" style="padding: 20px 40px; font-size: 1.5rem; cursor: pointer;">
      Run Game 🎮
    </button>
  </div>

  <div id="iframe-placeholder" style="width: 100%; height: 100%;"></div>
</div>

<script>
function loadUnityGame() {
  const container = document.getElementById('iframe-placeholder');
  const cover = document.getElementById('game-cover');
  
  // URL вашего билда
  const gameUrl = "{{ '/builds/santa/index.html' | relative_url }}";
  
  // Создаем iframe динамически
  container.innerHTML = `<iframe src="${gameUrl}" allowfullscreen style="width:100%; height:100%; border:none;"></iframe>`;
  
  // Скрываем обложку
  cover.style.display = 'none';
}
</script>
-->

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
  {% for screenshot in site.crossbow-pvp-screenshots %}
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
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](https://github.com/furyohfury/FreeRealEstate/tree/multiplayers)

## {{ t.game_technologies }}
- Netcode for Gameobjects
- DOTween
- UniTask
- Zenject
- R3

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.crossbow_pvp_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>