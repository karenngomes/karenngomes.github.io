---
layout: page
permalink: /repositories/
title: repositories
description: My GitHub profile and repositories.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    <div class="repo p-2 text-center">
      <a href="https://github.com/{{ user }}">
        <img class="only-light w-100" alt="{{ user }} GitHub stats" src="https://github-stats-extended.vercel.app/api?username={{ user }}&count_private=true&theme={{ site.repo_theme_light }}">
        <img class="only-dark w-100" alt="{{ user }} GitHub stats" src="https://github-stats-extended.vercel.app/api?username={{ user }}&count_private=true&theme={{ site.repo_theme_dark }}">
      </a>
    </div>
    <div class="repo p-2 text-center">
      <a href="https://github.com/{{ user }}">
        <img class="only-light w-100" alt="{{ user }} top languages" src="https://github-stats-extended.vercel.app/api/top-langs?username={{ user }}&theme={{ site.repo_theme_light }}">
        <img class="only-dark w-100" alt="{{ user }} top languages" src="https://github-stats-extended.vercel.app/api/top-langs?username={{ user }}&theme={{ site.repo_theme_dark }}">
      </a>
    </div>
  {% endfor %}
</div>

{% endif %}

{% if site.data.repositories.featured_repos %}

## Highlights

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.featured_repos %}
    {% assign repo_parts = repo | split: '/' %}
    <div class="repo p-2 text-center">
      <a href="https://github.com/{{ repo }}">
        <img class="only-light w-100" alt="{{ repo }}" src="https://github-stats-extended.vercel.app/api/pin?username={{ repo_parts[0] }}&repo={{ repo_parts[1] }}&theme={{ site.repo_theme_light }}">
        <img class="only-dark w-100" alt="{{ repo }}" src="https://github-stats-extended.vercel.app/api/pin?username={{ repo_parts[0] }}&repo={{ repo_parts[1] }}&theme={{ site.repo_theme_dark }}">
      </a>
    </div>
  {% endfor %}
</div>
{% endif %}
