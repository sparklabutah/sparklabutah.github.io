---
layout: about
title: home
permalink: /
subtitle:

profile:
  align: right
  image:
  image_circular: false
  more_info:

selected_papers: false
social: false

announcements:
  enabled: false
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

<div style="text-align: center; margin-bottom: 2rem;">
  {% include figure.liquid path="assets/img/humanAI.png" class="img-fluid" width="100%" %}
</div>

We conduct research in systems, programming languages, and computer architecture.

---

## Faculty

<div class="members">
{% assign faculty = site.data.members | where: "category", "faculty" %}
{% for member in faculty %}
<div class="member">
  <div class="member-photo">
    {% if member.image %}
    <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" alt="{{ member.name }}">
    {% else %}
    <div class="member-placeholder">{{ member.name | slice: 0 }}</div>
    {% endif %}
  </div>
  <div class="member-info">
    <h4>{% if member.website %}<a href="{{ member.website }}">{{ member.name }}</a>{% else %}{{ member.name }}{% endif %}</h4>
    <p class="member-title">{{ member.title }}</p>
  </div>
</div>
{% endfor %}
</div>

## PhD Students

<div class="members">
{% assign students = site.data.members | where: "category", "phd" %}
{% for member in students %}
<div class="member">
  <div class="member-photo">
    {% if member.image %}
    <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" alt="{{ member.name }}">
    {% else %}
    <div class="member-placeholder">{{ member.name | slice: 0 }}</div>
    {% endif %}
  </div>
  <div class="member-info">
    <h4>{% if member.website %}<a href="{{ member.website }}">{{ member.name }}</a>{% else %}{{ member.name }}{% endif %}</h4>
    <p class="member-title">{{ member.title }}</p>
  </div>
</div>
{% endfor %}
</div>
<!-- 
## Alumni

<div class="members alumni-list">
{% assign alumni = site.data.members | where: "category", "alumni" %}
{% for member in alumni %}
<div class="member-inline">
  {% if member.website %}<a href="{{ member.website }}">{{ member.name }}</a>{% else %}{{ member.name }}{% endif %}{% if member.position %} ({{ member.position }}){% endif %}
</div>
{% endfor %}
</div> -->
