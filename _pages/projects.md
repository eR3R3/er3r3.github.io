---
layout: page
title: all projects
permalink: /projects/
description:
nav: true
nav_order: 3
display_categories: [art, computer-science, math]
horizontal: false
_styles: >
  .post > .post-header { display: none; }
  .featured-strip {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
    margin: 0.5rem 0 2.75rem 0;
  }
  @media (min-width: 768px) {
    .featured-strip { grid-template-columns: 1fr 1fr; }
  }
  .featured-tile {
    position: relative;
    display: block;
    padding: 1.5rem 1.75rem;
    border-top: 1px solid var(--global-divider-color);
    border-bottom: 1px solid var(--global-divider-color);
    background: transparent;
    transition: background-color 0.25s ease, border-color 0.25s ease;
  }
  .ft-main {
    display: block;
    text-decoration: none !important;
    color: var(--global-text-color);
  }
  .ft-main:hover { color: var(--global-text-color); text-decoration: none !important; }
  .featured-tile:hover {
    background: rgba(127, 127, 127, 0.06);
    border-color: var(--global-text-color);
    color: var(--global-text-color);
    text-decoration: none !important;
  }
  .ft-headline {
    font-size: 1.05rem;
    font-weight: 700;
    letter-spacing: 0.02em;
    color: var(--global-text-color);
    margin: 0 0 0.65rem 0;
    text-transform: none;
  }
  .ft-title {
    font-size: 1.75rem;
    font-weight: 600;
    letter-spacing: -0.01em;
    line-height: 1.05;
    margin: 0 0 0.35rem 0;
  }
  .ft-sub {
    font-size: 0.8rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--global-text-color-light);
    margin: 0;
    font-weight: 500;
  }
  .ft-sublink {
    display: inline-block;
    margin-top: 0.9rem;
    font-size: 0.85rem;
    color: var(--global-theme-color);
    text-decoration: none;
    border-bottom: 1px solid transparent;
    transition: border-color 0.2s ease;
  }
  .ft-sublink:hover {
    text-decoration: none;
    border-bottom-color: var(--global-theme-color);
    color: var(--global-theme-color);
  }
  .projects-page-title {
    font-size: 2.5rem;
    font-weight: 300;
    letter-spacing: -0.01em;
    margin: 2rem 0 1.25rem 0;
  }
---

<div class="featured-strip">
  <div class="featured-tile">
    <a class="ft-main" href="{{ '/projects/2_project/' | relative_url }}">
      <p class="ft-headline">CVPR 2026 Poster</p>
      <h2 class="ft-title">GeoCGA</h2>
      <p class="ft-sub">Sole First Author</p>
    </a>
    <a class="ft-sublink" href="https://cvpr.thecvf.com/virtual/2026/poster/38204" target="_blank" rel="noopener">CVPR virtual site</a>
  </div>
  <div class="featured-tile">
    <a class="ft-main" href="{{ '/projects/1_project/' | relative_url }}">
      <p class="ft-headline">ISEF 2026 Finalist</p>
      <h2 class="ft-title">CaRF</h2>
      <p class="ft-sub">Team Shanghai</p>
    </a>
    <a class="ft-sublink" href="https://isef.net/project/teca020-carf-camera-aware-referring-field" target="_blank" rel="noopener">ISEF project page</a>
  </div>
</div>

<h1 class="projects-page-title">All Projects</h1>

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
