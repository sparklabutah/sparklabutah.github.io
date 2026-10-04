---
layout: page
permalink: /people/
title: People
description: The researchers of SPARK Lab at the University of Utah.
nav: false
---

<div class="spark-home">

<section>
  {% assign group_keys = "faculty,phd,masters,undergrad" | split: "," %}
  {% assign group_names = "Faculty,PhD Students,MS Students,Undergraduate Students" | split: "," %}
  {% for key in group_keys %}
  {% assign group = site.data.members | where: "category", key %}
  {% if group.size > 0 %}
  <h3 class="spark-people-group"><span>{{ group_names[forloop.index0] }}</span></h3>
  <div class="spark-people">
  {% for member in group %}
    <div class="spark-person">
      <div class="spark-person-photo">
        {% if member.image %}
        <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" alt="{{ member.name }}" loading="lazy">
        {% else %}
        ⚡
        {% endif %}
      </div>
      <h4>{{ member.name }}</h4>
      <p class="spark-person-title">{{ member.title }}</p>
      <div class="spark-person-links">
        {% if member.website %}<a href="{{ member.website }}" target="_blank" rel="noopener" title="Homepage"><i class="fas fa-home"></i></a>{% endif %}
        {% if member.scholar %}<a href="{{ member.scholar }}" target="_blank" rel="noopener" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
        {% if member.email %}<a href="mailto:{{ member.email }}" title="Email"><i class="fas fa-envelope"></i></a>{% endif %}
      </div>
    </div>
  {% endfor %}
  </div>
  {% endif %}
  {% endfor %}
</section>

</div>
