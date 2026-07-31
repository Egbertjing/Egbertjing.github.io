---
permalink: /blog/
title: "Blog"
author_profile: true
---

<div class="intro-panel intro-panel--compact">
  <p class="page-kicker">Working notes</p>
  <p class="intro-lead">Ideas in progress on language agents, safety, systems, and research practice.</p>
  <p>This is a notebook rather than a publication list: shorter observations, experiments, reading notes, and lessons that are still taking shape.</p>
</div>

{% assign blog_posts = site.blog | sort: "date" | reverse %}

<div class="blog-grid">
  {% for post in blog_posts %}
    {% include blog-card.html post=post %}
  {% endfor %}
</div>
