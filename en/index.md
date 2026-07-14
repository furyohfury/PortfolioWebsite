---
layout: default
title: "Unity Developer Portfolio"
lang: en
---
{% assign t = site.data.t[page.lang] %}

<section class="portfolio-panel hero-panel">
  <nav class="top-nav" aria-label="Primary navigation">
    <a class="nav-pill active" href="{{ '/en/' | relative_url }}">Home</a>
    <button class="theme-button" type="button" aria-label="Toggle light or dark theme" disabled>
      <span class="theme-icon" aria-hidden="true"></span>
    </button>
    <div class="language-toggle" aria-label="Language switcher">
      <a class="language-option" href="{{ '/' | relative_url }}">RU</a>
      <a class="language-option active" href="{{ '/en/' | relative_url }}">EN</a>
    </div>
  </nav>

  <div class="hero-grid">
    <div class="hero-copy">
      <p class="section-kicker">Unity Developer</p>
      <h1>Artem Kuzminikh</h1>
      <p class="hero-lead">
        I build 2D and 3D Unity games, design gameplay architecture, and turn prototypes into clear playable experiences.
      </p>

      <div class="contact-actions" aria-label="{{ t.contacts }}">
        <a class="icon-action icon-email is-placeholder" href="mailto:artemkuzminikh@gmail.com" aria-label="{{ t.email_label }}"></a>
        <a class="icon-action icon-telegram is-placeholder" href="https://t.me/artemkuzminikh" aria-label="{{ t.telegram_label }}"></a>
        <a class="icon-action" href="https://github.com/furyohfury" aria-label="GitHub">
          <img src="https://github.githubassets.com/favicons/favicon.svg" alt="">
        </a>
        <a class="icon-action" href="https://furyohfury.itch.io/" aria-label="itch.io">
          <img src="https://static.itch.io/images/itchio-textless-black.svg" alt="">
        </a>
        <a class="icon-action" href="https://hh.ru/resume/2eda4b93ff0ed8f2ba0039ed1f38384d4c7761" aria-label="hh.ru">
          <img src="https://i.hh.ru/images/logos/svg/hh.ru.svg" alt="">
        </a>
        <a class="resume-button contact-resume-button" href="{{ '/assets/files/resume.pdf' | relative_url }}" download>
          {{ t.download_resume }}
          <span aria-hidden="true">→</span>
        </a>
      </div>
    </div>

    <div class="hero-visual" aria-hidden="true">
      <img src="{{ '/assets/images/crossbow-pvp-preview.png' | relative_url }}" alt="">
    </div>
  </div>
</section>

<section class="portfolio-panel projects-panel">
  <div class="section-heading">
    <p class="section-kicker">{{ t.projects_title }}</p>
  </div>

  <div class="portfolio-project-grid">
    {% assign sorted_projects = site.projects | where: "lang", page.lang | sort: "priority" %}
    {% for project in sorted_projects %}
      <article class="portfolio-project-card">
        <a class="project-media" href="{{ project.url | relative_url }}" aria-label="{{ project.title }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
        </a>
        <div class="project-card-body">
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
          <div class="tech-tags" aria-label="{{ t.game_technologies }}">
            {% for tech in project.technologies limit: 4 %}
              <span>{{ tech }}</span>
            {% endfor %}
          </div>
          <a class="project-link" href="{{ project.url | relative_url }}">
            <span>View Project</span>
            <span class="arrow-circle" aria-hidden="true">→</span>
          </a>
        </div>
      </article>
    {% endfor %}
  </div>
</section>

<section class="portfolio-panel story-panel">
  <div class="section-heading centered">
    <p class="section-kicker">{{ t.about_me }}</p>
  </div>

  <div class="story-stack">
    <article class="story-block">
      <h3>{{ t.skills_title }}</h3>
      <ul>
        {% for skill in t.skills_list %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>
    </article>

    <article class="story-block">
      <h3>{{ t.experience_title }}</h3>
      <h4>Bibamus</h4>
      <p><strong>{{ t.job_role }}</strong><br>{{ t.job_date }}</p>
      <ul>
        {% for item in t.job_description %}
          <li>{{ item }}</li>
        {% endfor %}
      </ul>
    </article>

    <article class="story-block">
      <h3>{{ t.courses_title }}</h3>
      <ul>
        <li><strong>Otus</strong> - <a href="https://otus.ru/certificate/bc7bdffd58dd452abe5645de0b2d0c88/">{{ t.certificate }}</a>, 05.2024 - 03.2025. {{ t.otus_desc }}</li>
        <li><strong>Netology</strong> - <a href="https://netology.ru/sharing/26274951829d26fd5eec9f350a43c47a">{{ t.certificate }}</a>, 04.2023 - 03.2024. {{ t.netology_desc }}</li>
      </ul>
    </article>

    <article class="story-block">
      <h3>{{ t.education_title }}</h3>
      <p><strong>{{ t.university }}</strong>, Moscow<br>{{ t.specialty }}<br>2015-2020</p>
    </article>
  </div>

</section>
