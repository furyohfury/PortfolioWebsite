---
layout: game-page
title: "Sequence drift"
description: "Разработка игры в ходе Ludum dare 59 в паре с художником"
image: "/assets/images/sequence-drift-preview.jpg"  # Превью для карточки
priority: -2
---

## Играть в браузере:
<div class="unity-container" id="unity-loader-container">
  <div id="game-cover" style="
    position: absolute; 
    width: 100%; 
    height: 100%; 
    background: url('{{ "/assets/images/sequence-drift-preview.jpg" | relative_url }}') no-repeat center; 
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
  const gameUrl = "{{ '/builds/sequence-drift/index.html' | relative_url }}";
  
  // Создаем iframe динамически
  container.innerHTML = `<iframe src="${gameUrl}" allowfullscreen style="width:100%; height:100%; border:none;"></iframe>`;
  
  // Скрываем обложку
  cover.style.display = 'none';
}
</script>

## Скриншоты
<div class="gallery">
  {% for screenshot in site.sequence-drift-screenshots %}
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
- [Ludum Dare](https://ldjam.com/events/ludum-dare/59/sequence-drift)

## Технологии
- DOTween
- Awaitable

## Достигнутые в ходе работы цели
- Создание небольшой игры для гейм джема за 3 дня
- Работа в качестве разработчика в паре с художником