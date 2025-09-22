---
layout: default
title: Civic Topics
description: Civic issues of the day, and contacting your legislators.
nav_section: topics
---

<section class="hero">
  <div class="container">
    <nav class="breadcrumbs" aria-label="Breadcrumb">
      <a href="{{ site.baseurl }}/">Home</a> › <span>Civic Topics</span>
    </nav>
    <h1>Civic Topics</h1>
    <p>Read the latest guidance on hot topics, and stay informed on civic issues.</p>
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
