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

<div class="spark-home">

<section class="spark-hero-wrap">
  <div class="spark-hero">
    <img class="spark-hero-media" src="{{ '/assets/img/sparklab/robot-dance.gif' | relative_url }}" alt="Robot arms from Daniel Brown's ARIA Lab dancing in sync" fetchpriority="high">
    <div class="spark-hero-credit">Robots courtesy of Daniel Brown's <a href="https://aria-lab.cs.utah.edu/" target="_blank" rel="noopener">ARIA Lab</a>, our collaborators on the NSF center</div>
    <div class="spark-hero-body">
      <div class="spark-hero-kicker">SPARK Lab · University of Utah</div>
      <h1><b>S</b>ystems for <b>P</b>erception, <b>A</b>ction, <b>R</b>easoning, and <b>K</b>nowledge</h1>
      <p>We study the convergence of automation and intelligence. Our mission is to build Lifelong Embodied Agents: intelligent systems that perceive, act, remember, and improve forever, by learning from real interaction.</p>
      <a class="spark-btn spark-btn-solid" href="{{ '/publications/' | relative_url }}">Our research <i class="fas fa-arrow-right"></i></a>
      <a class="spark-btn spark-btn-ghost" href="#join-us">Join us</a>
    </div>
  </div>

  <div class="spark-highlight">
    <div class="spark-highlight-icon"><i class="fas fa-handshake"></i></div>
    <div>
      <span class="spark-eyebrow">New · NSF Center</span>
      <h3>SPARK Lab is part of the NSF Center for Human and Robot Co-Adaptation</h3>
      <p>A $30M, five-year NSF center led by UT Austin with Indiana University, MIT, Tufts, Yale, and the University of Utah, studying how people and robots learn from each other over long-term, real-world interaction. <a href="https://attheu.utah.edu/science-technology/u-researchers-join-nsf-center-that-studies-how-robots-and-people-learn-to-work-together/" target="_blank" rel="noopener">Read the announcement</a>.</p>
    </div>
  </div>
</section>

<section>
  <span class="spark-eyebrow">What we work on</span>
  <h2 class="spark-section-title">Research</h2>
  <p>Lifelong Embodied Agents are continual learners grounded in a body, robotic or simulated, that accumulate skills and knowledge over time.</p>
  <div class="spark-themes">
    <div class="spark-theme-card">
      <i class="fas fa-globe"></i>
      <h3>Web &amp; computer-use agents</h3>
      <p>How can artificial agents navigate the open web with the fluidity of a human user?</p>
    </div>
    <div class="spark-theme-card">
      <i class="fas fa-robot"></i>
      <h3>Embodied agents in the real world</h3>
      <p>How can we design agents that can be deployed in real-world settings, from browsers to robot arms?</p>
    </div>
    <div class="spark-theme-card">
      <i class="fas fa-infinity"></i>
      <h3>Lifelong learning &amp; exploration</h3>
      <p>How can these agents learn continuously and accumulate knowledge over time without forgetting?</p>
    </div>
    <div class="spark-theme-card">
      <i class="fas fa-people-arrows"></i>
      <h3>Human–robot co-adaptation</h3>
      <p>How can people and robots adapt to each other over long-term interaction at home, in hospitals, and beyond?</p>
    </div>
  </div>
</section>

<section>
  <div class="spark-section-head">
    <div>
      <span class="spark-eyebrow">Featured work</span>
      <h2 class="spark-section-title">Recent papers</h2>
    </div>
    <a class="spark-more" href="{{ '/publications/' | relative_url }}">All publications →</a>
  </div>
  <div class="spark-papers">
    <a class="spark-paper" href="https://timewarp-web.github.io/" target="_blank" rel="noopener">
      <div class="spark-paper-img"><img src="{{ '/assets/img/timeWarp.png' | relative_url }}" alt="TimeWarp overview figure" loading="lazy"></div>
      <div class="spark-paper-body">
        <span class="spark-venue">NeurIPS 2026</span>
        <h3>TimeWarp: Evaluating Web Agents by Revisiting the Past</h3>
        <p>A benchmark for how robust web agents are to website UIs changing over time.</p>
      </div>
    </a>
    <a class="spark-paper" href="https://alexgill321.github.io/KNOWS-benchmark/" target="_blank" rel="noopener">
      <div class="spark-paper-img"><img src="{{ '/assets/img/knows.png' | relative_url }}" alt="KNOWS benchmark overview figure" loading="lazy"></div>
      <div class="spark-paper-body">
        <span class="spark-venue">Findings of EMNLP 2026</span>
        <h3>The Hard Part Comes After Search: Benchmarking Web Agents on Synthesizing, Organizing, and Displaying Knowledge</h3>
        <p>KNOWS tests whether web agents can turn what they find into usable artifacts, not just retrieve it.</p>
      </div>
    </a>
    <a class="spark-paper" href="https://dora-explore.github.io/" target="_blank" rel="noopener">
      <div class="spark-paper-img"><img src="{{ '/assets/img/DORA.png' | relative_url }}" alt="DORA Explorer overview figure" loading="lazy"></div>
      <div class="spark-paper-body">
        <span class="spark-venue">Preprint 2026</span>
        <h3>DORA Explorer: Improving the Exploration Ability of LLMs Without Training</h3>
        <p>Training-free exploration for LLM agents.</p>
      </div>
    </a>
    <a class="spark-paper" href="https://iclr-blogposts.github.io/2026/blog/2026/web-agent/" target="_blank" rel="noopener">
      <div class="spark-paper-img"><img src="{{ '/assets/img/iclrBlogpost-26.png' | relative_url }}" alt="Computer Use Survey figure" loading="lazy"></div>
      <div class="spark-paper-body">
        <span class="spark-venue">ICLR Blogposts 2026</span>
        <h3>Computer Use Survey: A Visual Survey of Computer Use Agents</h3>
        <p>An illustrated tour of how computer-use agents work today.</p>
      </div>
    </a>
  </div>
</section>

<section>
  <span class="spark-eyebrow">Latest</span>
  <h2 class="spark-section-title" id="news">News</h2>
  <ul class="spark-news">
    <li class="is-big">
      <span class="spark-news-date">October 2026</span>
      Our web agent benchmark <a href="https://alexgill321.github.io/KNOWS-benchmark/" target="_blank" rel="noopener">KNOWS</a>, a collaboration with Utah NLP, has been accepted to Findings of EMNLP 2026!
    </li>
    <li class="is-big">
      <span class="spark-news-date">September 2026</span>
      <a href="https://timewarp-web.github.io/" target="_blank" rel="noopener">TimeWarp</a> has been accepted to NeurIPS 2026!
    </li>
    <li class="is-big">
      <span class="spark-news-date">September 2026</span>
      SPARK Lab joins the new $30M <a href="https://attheu.utah.edu/science-technology/u-researchers-join-nsf-center-that-studies-how-robots-and-people-learn-to-work-together/" target="_blank" rel="noopener">NSF Center for Human and Robot Co-Adaptation</a>, alongside UT Austin, Indiana University, MIT, Tufts, and Yale.
    </li>
    <li>
      <span class="spark-news-date">September 2026</span>
      New robots have arrived in the lab!
    </li>
    <li>
      <span class="spark-news-date">August 2026</span>
      New member, Minh Pham-Dinh, joined SPARK Lab!
    </li>
    <li>
      <span class="spark-news-date">July 2026</span>
      Check out our new work on training-free exploration for LLM agents, <a href="https://dora-explore.github.io/" target="_blank" rel="noopener">DORA Explorer</a>.
    </li>
    <li>
      <span class="spark-news-date">March 2026</span>
      We launched the website for SPARK Lab!
    </li>
    <li>
      <span class="spark-news-date">March 2026</span>
      Check out our web agent benchmark, <a href="https://timewarp-web.github.io/" target="_blank" rel="noopener">TimeWarp</a>.
    </li>
    <li>
      <span class="spark-news-date">February 2026</span>
      Our <a href="https://iclr-blogposts.github.io/2026/blog/2026/web-agent/" target="_blank" rel="noopener">Computer Use Survey</a> has been accepted to ICLR Blogposts 2026!
    </li>
    <li>
      <span class="spark-news-date">January 2026</span>
      Two new members, Dai-Jie Wu and Priya Gurjar, joined SPARK Lab!
    </li>
  </ul>
</section>

<section>
  <span class="spark-eyebrow">Inside the lab</span>
  <h2 class="spark-section-title">Life at SPARK</h2>
  <!-- To add a photo: drop it in assets/img/sparklab/ and add one more <img> line with its real width/height. -->
  <div class="spark-gallery">
    <button class="spark-gallery-btn is-prev" type="button" aria-label="Previous photo"><i class="fas fa-chevron-left"></i></button>
    <div class="spark-gallery-track" tabindex="0" aria-label="Photos from the lab">
      <img src="{{ '/assets/img/sparklab/pi-whiteboard.jpg' | relative_url }}" width="1600" height="1200" alt="Prof. Kenneth Marino at a whiteboard sketching a SPARK Lab architecture next to a mobile robot" loading="lazy">
      <img src="{{ '/assets/img/sparklab/teleop.gif' | relative_url }}" width="400" height="624" alt="A lab member teleoperating robot arms with a VR headset" loading="lazy">
      <img src="{{ '/assets/img/sparklab/hello-robot.jpg' | relative_url }}" width="900" height="1200" alt="Two Hello Robot Stretch mobile manipulators in the lab" loading="lazy">
    </div>
    <button class="spark-gallery-btn is-next" type="button" aria-label="Next photo"><i class="fas fa-chevron-right"></i></button>
  </div>
</section>

<section>
  <span class="spark-eyebrow">The team</span>
  <h2 class="spark-section-title" id="people">People</h2>
  <div class="spark-people">
  {% assign faculty = site.data.members | where: "category", "faculty" %}
  {% assign phd = site.data.members | where: "category", "phd" %}
  {% assign masters = site.data.members | where: "category", "masters" %}
  {% assign all_members = faculty | concat: phd | concat: masters %}
  {% for member in all_members %}
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
</section>

<section>
  <span class="spark-eyebrow">Work with us</span>
  <h2 class="spark-section-title" id="join-us">Join Us</h2>
  <div class="spark-join">
    <h4>For current University of Utah students</h4>
    <p>If you are a current University of Utah MS or undergraduate student, please email Prof. Kenneth Marino from a Utah email with your CV, a list of what ML-related courses you have taken, what your research interests are, why you think that our group would be the best place to do your research, and what you are hoping to get out of a research collaboration.</p>
    <h4>For prospective graduate students</h4>
    <p>We are actively looking for ambitious graduate students to join our group. The best (and only) way to do this is to apply to one of the graduate programs at Utah's Kahlert School of Computing. Be sure to mention your interest in working with Prof. Kenneth Marino in your application. In general, we are looking for students with:</p>
    <ul>
      <li>Motivation to pursue new research directions</li>
      <li>Strong programming skills</li>
      <li>Strong research skills</li>
      <li>Background in machine learning</li>
    </ul>
  </div>
</section>

</div>

<script>
  // Sliding gallery: arrows scroll by roughly one photo and hide at either end.
  document.querySelectorAll(".spark-gallery").forEach(function (gallery) {
    var track = gallery.querySelector(".spark-gallery-track");
    var prev = gallery.querySelector(".is-prev");
    var next = gallery.querySelector(".is-next");
    function update() {
      var max = track.scrollWidth - track.clientWidth - 2;
      prev.hidden = track.scrollLeft <= 2;
      next.hidden = track.scrollLeft >= max;
    }
    function step(dir) {
      track.scrollBy({ left: dir * track.clientWidth * 0.8, behavior: "smooth" });
    }
    prev.addEventListener("click", function () { step(-1); });
    next.addEventListener("click", function () { step(1); });
    track.addEventListener("scroll", update, { passive: true });
    window.addEventListener("resize", update);
    track.querySelectorAll("img").forEach(function (img) { img.addEventListener("load", update); });
    update();
  });
</script>
