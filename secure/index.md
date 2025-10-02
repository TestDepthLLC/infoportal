---
layout: default
title: Digital Security
description: Staying safe online and securing your devices.
nav_section: secure
---

<section class="hero">
  <div class="container">
    <nav class="breadcrumbs" aria-label="Breadcrumb">
      <a href="{{ site.baseurl }}/">Home</a> › <span>Digital Security</span>
    </nav>
    <h1>Digital Security</h1>
    <p>Guidance on staying safe online and protecting your digital identity.</p>
  </div>
</section>

<section>
  <div class="container">
    <h2>Guides & Checklists</h2>
    <div class="grid">
      {% assign items = site.secure | sort: "title" %}
      {% for item in items %}
        {% include card.html item=item %}
      {% endfor %}
    </div>
  </div>
</section>
