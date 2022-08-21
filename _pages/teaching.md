---
layout: page
permalink: /hackathons/
title: hackathons
description: 
nav: true
nav_order: 5
display_categories: [2022, 2021, 2020]
horizontal: false
---

<!-- pages/hackathons.md -->
<div class="hackathons">
{%- if site.enable_hackathon_categories and page.display_categories %}
  <!-- Display categorized hackathons -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_hackathons = site.hackathons | where: "category", category -%}
  {%- assign sorted_hackathons = categorized_hackathons | sort: "importance" %}
  <!-- Generate cards for each hackathon -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for hackathon in sorted_hackathons -%}
      {% include hackathons_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for hackathon in sorted_hackathons -%}
      {% include hackathons.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display hackathons without categories -->
  {%- assign sorted_hackathons = site.hackathons | sort: "importance" -%}
  <!-- Generate cards for each hackathon -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for hackathon in sorted_hackathons -%}
      {% include hackathons_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for hackathon in sorted_hackathons -%}
      {% include hackathons.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
