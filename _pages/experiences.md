---
layout: page
title: Experiences
permalink: /experiences/
description: I am keen on voluntary activities and discover the world !
nav: true
nav_order: 4
display_categories: [work, fun]
horizontal: false
---

<div class="projects">
<!-- Display projects without categories -->
  {% assign projects = site.experiences %}
  {% if projects %}
    {% assign sorted_projects = projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    <div class="grid">
      <div class="row row-cols-1 row-cols-md-2">
        {% for project in sorted_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
    </div>
  {% endif %}
</div>



