---
permalink: /service/
title: "Academic Service"
author_profile: true
---

I contribute to the research community through reviewing, area chair service,
and other academic activities. A selected record will be added here.

Area Chair
------

{% if site.data.service.area_chair.size > 0 %}
{% for item in site.data.service.area_chair %}
* **{{ item.venue }}**, {{ item.year }}
{% endfor %}
{% else %}
* To be updated
{% endif %}

Reviewer
------

{% if site.data.service.reviewer.size > 0 %}
{% for item in site.data.service.reviewer %}
* **{{ item.venue }}**, {{ item.year }}
{% endfor %}
{% else %}
* To be updated
{% endif %}

Other Service
------

{% if site.data.service.other.size > 0 %}
{% for item in site.data.service.other %}
* **{{ item.activity }}**, {{ item.year }}
{% endfor %}
{% else %}
* To be updated
{% endif %}

<p class="page-note">
To update this page, add venues and years to <code>_data/service.yml</code>.
</p>

