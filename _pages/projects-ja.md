---
layout: page
title: 研究プロジェクト
permalink: /ja/projects/
description: これまでに取り組んだ研究プロジェクトおよび現在進行中の研究を紹介します。
nav: false
---

<div class="text-end mb-3">
  <a href="{{ '/projects/' | relative_url }}">English</a>
</div>

<div class="projects">

{% assign research_projects = site.projects | where: "category", "Research" %}
{% assign sorted_projects = research_projects | sort: "importance" %}

<div class="row row-cols-1 row-cols-md-3">

{% for project in sorted_projects %}
{% if project.published != false %}

<div class="col mb-4">

  <a
    href="{{ project.ja_url | default: project.url | relative_url }}"
    style="text-decoration: none; color: inherit;"
  >

    <div class="card h-100 hoverable">

      {% if project.img %}
      <img
        src="{{ project.img | relative_url }}"
        class="card-img-top"
        alt="{{ project.title_ja | default: project.title }}"
      >
      {% endif %}

      <div class="card-body">

        <h5 class="card-title">
          {{ project.title_ja | default: project.title }}
        </h5>

        <p class="card-text">
          {{ project.description_ja | default: project.description }}
        </p>

      </div>

    </div>

  </a>

</div>

{% endif %}
{% endfor %}

</div>

</div>
