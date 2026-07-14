---
layout: game-page
title: "Cat-cloud"
description: "Game developed during Siberian game jam 2026 as part of a team"
image: "/assets/images/cat-cloud-preview.png"  # Превью для карточки
technologies:
  - DOTween
  - UniTask
priority: -3
lang: en
---
{% assign t = site.data.t[page.lang] %}
## {{ t.play_in_browser }}
<div class="unity-container" id="unity-loader-container">
  <div id="game-cover" style="
    position: absolute; 
    width: 100%; 
    height: 100%; 
    background: url('{{ "/assets/images/cat-cloud-preview.png" | relative_url }}') no-repeat center; 
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
  const gameUrl = "{{ '/builds/cat-cloud/index.html' | relative_url }}";
  
  // Создаем iframe динамически
  container.innerHTML = `<iframe src="${gameUrl}" allowfullscreen style="width:100%; height:100%; border:none;"></iframe>`;
  
  // Скрываем обложку
  cover.style.display = 'none';
}
</script>

## {{ t.screenshots }}
<div class="gallery">
  {% for screenshot in site.cat-cloud-screenshots %}
    <a href="{{ screenshot.image | relative_url }}" 
       data-lightbox="gallery" 
       data-title="Скриншот"
       {% if forloop.first == false %} style="display: none;" {% endif %}>
       
       <img src="{{ screenshot.image | relative_url }}" alt="Скриншот" class="project-image">
       
       {% if forloop.first %}
         <p style="text-align: center; cursor: pointer;">📸 Press to look at all screenshots</p>
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
- [Itch.io](https://furyohfury.itch.io/cat-cloud)
- [SibGJ](https://platform.sibgamejam.com/games/alinaapril17/cat-cloud)
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[Github](https://github.com/D0GMAR/SibGJ2026)

## {{ t.game_technologies }}
- DOTween
- UniTask

## {{ t.game_achieved_goals }}
<ul>
        {% for skill in t.cat_cloud_goals %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>
