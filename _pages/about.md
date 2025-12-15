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
  {% include figure.liquid path="assets/img/humanAINew.png" class="img-fluid" width="100%" %}
</div>

At Spark Lab, we study the convergence of automation and human behavior.

How can artificial agents navigate the open web with the fluidity of a human user? How can we design agents and environments to embody intelligence? How can these agents learn continuously and accumulate knowledge over time without forgetting?

Through these questions, we advance embodied AI, web automation, reinforcement learning, and behavioral modeling.

---

<h1 id="people">People</h1>

<div class="members-grid" style="display: grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap: 1.5rem; margin-bottom: 3rem;">
{% assign faculty = site.data.members | where: "category", "faculty" %}
{% assign students = site.data.members | where: "category", "phd" %}
{% assign all_members = faculty | concat: students %}
{% for member in all_members %}
<div class="member-card" style="border: 1px solid var(--global-divider-color); border-radius: 8px; overflow: hidden; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
  <div class="member-photo" style="width: 100%; aspect-ratio: 1 / 1; overflow: hidden; background-color: #f5f5f5;">
    {% if member.image %}
    <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" alt="{{ member.name }}" style="width: 100%; height: 100%; object-fit: cover;">
    {% else %}
    <div style="width: 100%; height: 100%; display: flex; align-items: center; justify-content: center; background-color: var(--global-bg-color); color: var(--global-text-color); font-size: 3rem;">{{ member.name | slice: 0 }}</div>
    {% endif %}
  </div>
  <div class="member-info" style="padding: 1rem;">
    <h4 style="margin: 0 0 0.25rem 0; font-size: 1rem;">{{ member.name }}</h4>
    <p class="member-title" style="margin: 0 0 0.5rem 0; color: var(--global-text-color-light); font-size: 0.85rem;">{{ member.title }}</p>
    <div style="display: flex; gap: 0.75rem; margin-bottom: 0.5rem;">
      {% if member.website %}
      <a href="{{ member.website }}" target="_blank" style="color: var(--global-text-color); font-size: 1.1rem;" title="Homepage">
        <i class="fas fa-home"></i>
      </a>
      {% endif %}
      {% if member.scholar %}
      <a href="{{ member.scholar }}" target="_blank" style="color: var(--global-text-color); font-size: 1.1rem;" title="Google Scholar">
        <i class="ai ai-google-scholar"></i>
      </a>
      {% endif %}
      {% if member.email %}
      <a href="mailto:{{ member.email }}" style="color: var(--global-text-color); font-size: 1.1rem;" title="Email">
        <i class="fas fa-envelope"></i>
      </a>
      {% endif %}
    </div>
    {% if member.interests %}
    <p style="margin: 0; font-size: 0.8rem; color: var(--global-text-color-light);">{{ member.interests }}</p>
    {% endif %}
  </div>
</div>
{% endfor %}
</div>

---

<h1 id="join-us">Join Us</h1>

**For Current University of Utah Students:** If you are a current University of Utah MS or undergraduate student, please email Prof. Kenneth Marino from a Utah email with your CV, a list of what ML related courses you have taken, what your research interests are, why you think that our group would be the best place to do your research, and what you are hoping to get out of a research collaboration.

**For Prospective Graduate Students:** We are actively looking for ambitious graduate students to join our group. The best (and only) way to do this is to apply to one of the graduate programs at Utah's Kahlert School of Computing. Be sure to mention your interest in working with Prof Kenneth Marino in your application. In general, we are looking for students with:
- Motivation to pursue new research directions
- Strong programming skills
- Strong research skills
- Background in Machine Learning