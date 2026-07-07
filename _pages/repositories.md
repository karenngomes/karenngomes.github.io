---
layout: page
permalink: /repositories/
title: repositories
description: My GitHub profile and repositories.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    <div class="repo p-2 text-center">
      <a href="https://github.com/{{ user }}">
        <img src="https://github.com/{{ user }}.png" alt="{{ user }}" width="120" height="120" style="border-radius: 50%">
        <p>{{ user }}</p>
      </a>
    </div>
  {% endfor %}
</div>

{% endif %}

{% if site.data.repositories.github_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    <div class="repo p-2 text-center">
      <a href="https://github.com/{{ repo }}">{{ repo }}</a>
    </div>
  {% endfor %}
</div>
{% endif %}
