---
layout: about
title: Home
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

<div style="margin-bottom: 2rem; margin-top: -1rem; max-width: 100%; box-sizing: border-box; overflow: hidden;">
    <h1 class="spark-tagline" style="text-align: center; margin: 0; line-height: 1.2; font-weight: 300;"><b>S</b>ystems for <b>P</b>erception, <b>A</b>ction, <b>R</b>easoning, and <b>K</b>nowledge</h1>
    
    <div style="text-align: left; margin-top: 1.5rem; font-size: 1.1rem; line-height: 1.6;">
      <p>We study the convergence of automation and intelligence. Our mission is to build Lifelong Embodied Agents — intelligent systems that perceive, act, remember, and improve forever, by learning from real interaction.</p>
    </div>
  </div>

<div style="font-size: 1.1rem; line-height: 1.6; margin-bottom: 3rem;">
<p>Lifelong Embodied Agents are continual learners grounded in a body: robotic or simulated, that accumulate skills and knowledge over time. Some of the research questions that we wish to uncover:</p>
  
  <ul>
    <li>How can artificial agents navigate the open web with the fluidity of a human user?</li>
    <li>How can we design agents that can be deployed in real world settings?</li>
    <li>How can these agents learn continuously and accumulate knowledge over time without forgetting?</li>
  </ul>
</div>

<h2 id="news">News</h2>

<div style="max-height: 9.5rem; overflow-y: auto; margin-bottom: 3rem; padding: 0.75rem 1rem; border: 1px solid var(--global-divider-color); border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.08); background: var(--global-bg-color);">
  <ul style="list-style-type: none; padding-left: 0; margin: 0;">
    <li style="margin-bottom: 0.75rem;">
      <strong>August 2026:</strong> New member, Minh Pham-Dinh joined SPARK Lab!
    </li>
    <li style="margin-bottom: 0.75rem;">
      <strong>July 2026:</strong> Check out our new work on training-free exploration for LLM agents, <a href="https://dora-explore.github.io/" target="_blank" style="text-decoration: underline;">DORA Explorer</a>.
    </li>
    <li style="margin-bottom: 0.75rem;">
      <strong>March 2026:</strong> We launched the website for SPARK Lab!
    </li>
    <li style="margin-bottom: 0.75rem;">
      <strong>March 2026:</strong> Check out our web agent benchmark, <a href="https://timewarp-web.github.io/" target="_blank" style="text-decoration: underline;">TimeWarp</a>.
    </li>
    <li style="margin-bottom: 0.75rem;">
      <strong>February 2026:</strong> Our <a href="https://iclr-blogposts.github.io/2026/blog/2026/web-agent/" target="_blank" style="text-decoration: underline;">Computer Use Survey</a> has been accepted to ICLR Blogposts 2026 !
    </li>
    <li style="margin-bottom: 0.75rem;">
      <strong>January 2026:</strong> Two new members, Dai-Jie Wu and Priya Gurjar joined SPARK Lab!
    </li>
  </ul>
</div>

<h1 id="people">People</h1>

<div class="members-grid" style="display: grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap: 1.5rem; margin-bottom: 3rem;">
{% assign faculty = site.data.members | where: "category", "faculty" %}
{% assign phd = site.data.members | where: "category", "phd" %}
{% assign masters = site.data.members | where: "category", "masters" %}
{% assign all_members = faculty | concat: phd | concat: masters %}
{% for member in all_members %}
<div class="member-card" style="border: 1px solid var(--global-divider-color); border-radius: 8px; overflow: hidden; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
  <div class="member-photo" style="width: 100%; aspect-ratio: 1 / 1; overflow: hidden; background-color: #f5f5f5; display: flex; align-items: center; justify-content: center;">
    {% if member.image %}
    <img src="{{ member.image | prepend: '/assets/img/' | relative_url }}" alt="{{ member.name }}" style="width: 100%; height: 100%; object-fit: cover;">
    {% else %}
    <div style="font-size: 5rem;">⚡</div>
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
