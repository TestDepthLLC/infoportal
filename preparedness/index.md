---
layout: default
title: Emergency Preparedness
description: Build resilience with checklists, calculators, and printable guides.
nav_section: preparedness
---

<section class="hero">
  <div class="container">
    <nav class="breadcrumbs" aria-label="Breadcrumb">
      <a href="{{ site.baseurl }}/">Home</a> › <span>Emergency Preparedness</span>
    </nav>
    <h1>Emergency Preparedness</h1>
    <p>Build resilience for outages, disasters, and evacuations with practical guides & checklists.</p>
  </div>
</section>

<section>
  <div class="container">
    <h2>Guides & Checklists</h2>
    <div class="grid">
      {% assign items = site.preparedness | sort: "title" %}
      {% for item in items %}
        {% include card.html item=item %}
      {% endfor %}
    </div>
  </div>
</section>
