---
layout: default
title: My Unity portfolio
lang: en
---

{% assign t = site.data.t[page.lang] %}

## Artem Kuzminikh

<div class="info-block" markdown="1">

### {{ t.contacts }}

* **{{ t.email_label }}:** [artemkuzminikh@gmail.com](mailto:artemkuzminikh@gmail.com)
* **{{ t.telegram_label }}:** [t.me/artemkuzminikh](https://t.me/artemkuzminikh)
* **Github:** ![GitHub icon](https://github.githubassets.com/favicons/favicon.svg){: .icon} [{{ t.github_link }}](https://github.com/furyohfury)
* **itch.io:** ![Itch icon](https://static.itch.io/images/itchio-textless-black.svg){: .icon} [{{ t.itch_link }}](https://furyohfury.itch.io/)
* **hh.ru:** ![HH icon](https://i.hh.ru/images/logos/svg/hh.ru.svg){: .icon} [{{ t.hh_link }}](https://hh.ru/resume/2eda4b93ff0ed8f2ba0039ed1f38384d4c7761)

</div>

<div class="two-column-layout">

  <div class="column-left">
    <div class="info-block">
      <h3>{{ t.skills_title }}</h3>
      <ul>
        {% for skill in t.skills_list %}
          <li>{{ skill }}</li>
        {% endfor %}
      </ul>
    </div>

    <div class="info-block">
      <h3>{{ t.projects_title }}</h3>
      <div class="game-grid">
        {% assign sorted_projects = site.projects | where: "lang", page.lang | sort: "priority" %}
        {% for project in sorted_projects %}
          <div class="game-card">
            <h4><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h4>
            <a href="{{ project.url | relative_url }}">
              <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image" />
            </a>
          </div>
        {% endfor %}
      </div>
    </div>
  </div>

  <div class="column-right">
    <div class="info-block">
      <h3>{{ t.experience_title }}</h3>
      <h4>Bibamus</h4>
      <b>{{ t.job_role }}</b><br>
      {{ t.job_date }}
      <ul>
        {% for item in t.job_description %}
          <li>{{ item }}</li>
        {% endfor %}
      </ul>
    </div>

    <div class="info-block">
      <h3>{{ t.courses_title }}</h3>
      <ul>
        <li><b>Otus</b><br>
          <img src="https://otus.ru/static/img/favicons/favicon-32x32.png" class="icon" alt="OTUS icon">
          <a href="https://otus.ru/certificate/bc7bdffd58dd452abe5645de0b2d0c88/">{{ t.certificate }}</a>
          05.2024 - 03.2025<br>
          {{ t.otus_desc }}
        </li>
        <li><b>Netology</b><br>
          <img src="https://netology.ru/favicon-32x32.png" class="icon" alt="Netology icon">
          <a href="https://netology.ru/sharing/26274951829d26fd5eec9f350a43c47a">{{ t.certificate }}</a>
          04.2023 - 03.2024<br>
          {{ t.netology_desc }}
        </li>
      </ul>
    </div>

    <div class="info-block">
      <h3>{{ t.education_title }}</h3>
      <b>{{ t.university }}</b>, Moscow<br>
      {{ t.specialty }}<br>
      2015-2020
    </div>
  </div>
</div>