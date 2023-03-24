---
layout: page
permalink: /repositories/
title: Repositories
description: Welcome to the preview of my GitHub repository, where I showcase some of my personal and school projects. Unfortunately, I can't share my work projects online because, you know, non-disclosure agreements and such. But don't worry, I've got plenty of other cool stuff to show off! Take a peek at my repo and see for yourself how I've flexed my programming muscles. Get ready to be impressed (and maybe even slightly amused)!
nav: true
nav_order: 3
---

## GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>
{% endif %}

---

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
