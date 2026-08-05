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
{% for collection in site.data.photo_albums %}
  <a href="#{{ collection.slug }}">{{ collection.title }}</a>
{% endfor %}
</nav>

<div class="photo-collections">
{% for collection in site.data.photo_albums %}
  {% assign collection_count = 0 %}
  {% for album in collection.albums %}
    {% assign collection_count = collection_count | plus: album.photos.size %}
  {% endfor %}
  <details class="photo-collection" id="{{ collection.slug }}"{% if forloop.first %} open{% endif %}>
    <summary class="photo-collection__heading">
      <span class="photo-collection__folder" aria-hidden="true"></span>
      <div>
        <span class="photo-collection__region">{{ collection.region }}</span>
        <h2>{{ collection.title }}</h2>
        <p>{{ collection.description }}</p>
      </div>
      <span class="photo-collection__count">
        {% if collection_count > 0 %}{{ collection_count }} photographs{% else %}Coming soon{% endif %}
        <span class="photo-collection__toggle" aria-hidden="true"></span>
      </span>
    </summary>

    {% if collection.albums.size > 0 %}
    <div class="photo-albums">
      {% for album in collection.albums %}
      <section class="photo-album" id="{{ album.slug }}">
        <div class="photo-album__heading">
          <div>
            <span class="photo-album__region">{{ collection.title }}</span>
            <h3>{{ album.title }}</h3>
            <p>{{ album.description }}</p>
          </div>
          <span class="photo-album__count">{{ album.photos.size }} photographs</span>
        </div>

        <div class="photo-grid">
          {% for photo in album.photos %}
          <figure class="photo-item">
            <a href="{{ photo.src | relative_url }}" class="image-popup">
              <img
                src="{{ photo.thumb | default: photo.src | relative_url }}"
                width="{{ photo.width }}"
                height="{{ photo.height }}"
                alt="{{ photo.alt | default: album.title }}"
                loading="lazy"
                decoding="async">
            </a>
            {% if photo.caption %}<figcaption>{{ photo.caption }}</figcaption>{% endif %}
          </figure>
          {% endfor %}
        </div>
      </section>
      {% endfor %}
    </div>
    {% else %}
    <div class="photo-placeholder">
      <span class="photo-placeholder__mark" aria-hidden="true"></span>
      <span>Collection in progress</span>
    </div>
    {% endif %}
  </details>
{% endfor %}
</div>

<script>
  (function () {
    function revealHashTarget() {
      if (!window.location.hash) return;
      var target = document.getElementById(window.location.hash.slice(1));
      if (!target) return;
      var collection = target.matches(".photo-collection") ? target : target.closest(".photo-collection");
      if (collection) collection.open = true;
    }

    document.querySelectorAll(".region-nav a[href^='#']").forEach(function (link) {
      link.addEventListener("click", function () {
        var target = document.getElementById(link.getAttribute("href").slice(1));
        if (target && target.matches(".photo-collection")) target.open = true;
      });
    });
    window.addEventListener("hashchange", revealHashTarget);
    revealHashTarget();
  }());
</script>
