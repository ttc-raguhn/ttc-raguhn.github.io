---
layout: page
title: Galerie
permalink: /galerie/
---

## Impressionen aus dem Vereinsleben

<div class="gallery-grid">
  {% for image in site.static_files %}
    {% if image.path contains 'assets/images/gallery/' %}
      <div class="gallery-item">
        <img src="{{ image.path | relative_url }}" alt="Galeriebild">
      </div>
    {% endif %}
  {% endfor %}
</div>