---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

## Projects

Our currently active projects include:

- **Andreev reflection across tunnel junctions** - can we measure quantum properties by injecting Cooper pairs on the atomic scale ?

            We pioneered a new technique to measure Andreev reflection across a metal-superconductor tunnel junction that can have 
            broad applicability to probe quantum materials. We are looking to grow this technique - discovery of new quantum materials, 
            solving contested materials, and finding new ap

- **Chalcogenophosphates in low dimensions** - can we introduce "complex" properties of oxide-like materials into 2D materials paradigm?

            Graphene is built from one element, TMDs and BN have two. Chalcogenophosphates have a minimum of three, but can have
            4,5,6 or even more. Elemental complexity leads to  many unique properties in the bulk, such as intrinsic phase transitions and 
            suprisingly strong non-linear optical properties, whose detailed origins remain unknown for now. We want to understand
            how these properties translate into low-dimensional forms and are looking for new devices and applications for these materials.

- **Mixed-D stacking** - how do we integrate materials that cannot be grown by CMOS into future electronic devices? 

            This project seeks new approaches to interface materials beyond heterostructure growth, and Scotch-tape like methods.
            Specifically we are developing methodologies to lift, transfer and stack materials without utilzing adhesives, lithography and 
            other contaminating agents. And we are also interested in emergent properties of such interfaces, such as n-type doping 
            at the MoS2/diamond interface.



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
