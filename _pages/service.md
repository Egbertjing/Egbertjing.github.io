---
permalink: /service/
title: "Academic Service"
author_profile: true
---

<div class="intro-panel">
  <p class="page-kicker">Community</p>
  <p class="intro-lead">I contribute to the research community through reviewing, area chair service, and other academic activities.</p>
</div>

<div class="service-grid">
  <section class="service-column">
    <h2>Area Chair</h2>
    {% if site.data.service.area_chair.size > 0 %}
    <ul class="service-list">
      {% for item in site.data.service.area_chair %}
      <li><strong>{{ item.venue }}</strong><span>{{ item.year }}</span></li>
      {% endfor %}
    </ul>
    {% else %}
    <p class="empty-state">To be updated</p>
    {% endif %}
  </section>

  <section class="service-column">
    <h2>Reviewer</h2>
    {% if site.data.service.reviewer.size > 0 %}
    <ul class="service-list">
      {% for item in site.data.service.reviewer %}
      <li><strong>{{ item.venue }}</strong><span>{{ item.year }}</span></li>
      {% endfor %}
    </ul>
    {% else %}
    <p class="empty-state">To be updated</p>
    {% endif %}
  </section>
</div>

<p class="page-note">
To update this page, add venues and years to <code>_data/service.yml</code>.
</p>
