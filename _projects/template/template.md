<!-- 
---
layout: game-page
title: "NAME"
description: "DESC"
image: "/assets/images/IMAGE.png"  # Превью для карточки
---

## Скриншоты
 <div class="gallery">
    {% for screenshot in site.neon-what-screenshots %}
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
- ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon}[GitHub](GITHUB_LINK)
- ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon}[Windows, Android](GITHUB_LINK)

## Технологии  


## Достигнутые в ходе работы цели -->