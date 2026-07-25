---
permalink: /photography/
title: "Photography"
author_profile: true
---

<div class="intro-panel">
  <p class="page-kicker">Outside research</p>
  <p class="intro-lead">Photography is how I keep a record of places, light, and ordinary moments.</p>
  <p>This archive is organized by region and will grow as new photographs are added.</p>
</div>

<nav class="region-nav" aria-label="Photography regions">
{% for album in site.data.photo_albums %}
  <a href="#{{ album.slug }}">{{ album.title }}</a>
{% endfor %}
</nav>

<div class="photo-albums">
{% for album in site.data.photo_albums %}
  <section class="photo-album" id="{{ album.slug }}">
    <div class="photo-album__heading">
      <div>
        <span class="photo-album__region">{{ album.region }}</span>
        <h2>{{ album.title }}</h2>
        <p>{{ album.description }}</p>
      </div>
      <span class="photo-album__count">
        {% if album.photos.size > 0 %}{{ album.photos.size }} photographs{% else %}Coming soon{% endif %}
      </span>
    </div>

    {% if album.photos.size > 0 %}
    <div class="photo-grid">
      {% for photo in album.photos %}
      <figure class="photo-item">
        <a href="{{ photo.src | relative_url }}" class="image-popup">
          <img src="{{ photo.src | relative_url }}" alt="{{ photo.alt | default: album.title }}" loading="lazy">
        </a>
        {% if photo.caption %}<figcaption>{{ photo.caption }}</figcaption>{% endif %}
      </figure>
      {% endfor %}
    </div>
    {% else %}
    <div class="photo-placeholder">
      <span class="photo-placeholder__mark" aria-hidden="true"></span>
      <span>Collection in progress</span>
    </div>
    {% endif %}
  </section>
{% endfor %}
</div>

<p class="page-note">
Add optimized images under <code>images/photography/&lt;region&gt;/</code>, then
list them in <code>_data/photo_albums.yml</code>. Each region will appear as its
own section automatically.
</p>
