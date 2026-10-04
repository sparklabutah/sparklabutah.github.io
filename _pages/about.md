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
      <a class="spark-btn spark-btn-solid" href="#research">Our research <i class="fas fa-arrow-right"></i></a>
      <a class="spark-btn spark-btn-ghost" href="{{ '/join/' | relative_url }}">Join us</a>
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

<section id="research">
  {% assign research = site.data.research %}
  <div class="spark-section-head">
    <div>
      <span class="spark-eyebrow">What we work on</span>
      <h2 class="spark-section-title">Research</h2>
    </div>
    <a class="spark-more" href="{{ '/publications/' | relative_url }}">All publications →</a>
  </div>
  <p class="spark-research-intro" data-default="Our work toward Lifelong Embodied Agents spans three threads: computer use, embodied multimodal agents, and NLP. Pick a thread to browse related papers.">Our work toward Lifelong Embodied Agents spans three threads: computer use, embodied multimodal agents, and NLP. Pick a thread to browse related papers.</p>

  <div class="spark-filter" role="group" aria-label="Filter papers by research thread">
    <button type="button" class="spark-chip is-active" data-filter="all" aria-pressed="true">All <span class="spark-chip-count">{{ research.papers.size }}</span></button>
    {% for theme in research.themes %}
    {% assign count = 0 %}
    {% for paper in research.papers %}{% if paper.themes contains theme.key %}{% assign count = count | plus: 1 %}{% endif %}{% endfor %}
    <button type="button" class="spark-chip" data-filter="{{ theme.key }}" data-question="{{ theme.question | escape }}" data-empty="{{ theme.empty | escape }}" aria-pressed="false"><i class="{{ theme.icon }}"></i> {{ theme.name }} <span class="spark-chip-count">{{ count }}</span></button>
    {% endfor %}
  </div>

  <div class="spark-papers">
    {% for paper in research.papers %}
    <a class="spark-paper" href="{{ paper.link }}" target="_blank" rel="noopener" data-themes="{{ paper.themes | join: ' ' }}">
      <div class="spark-paper-img"><img src="{{ paper.image | prepend: '/assets/img/' | relative_url }}" alt="" loading="lazy"></div>
      <div class="spark-paper-body">
        <span class="spark-venue">{{ paper.venue }}</span>
        <h3>{{ paper.title }}</h3>
        <p>{{ paper.blurb }}</p>
        <div class="spark-paper-tags">
          {% for key in paper.themes %}{% assign theme = research.themes | where: "key", key | first %}<span>{{ theme.name }}</span>{% endfor %}
        </div>
      </div>
    </a>
    {% endfor %}
  </div>
  <p class="spark-papers-empty" hidden></p>
  <div class="spark-papers-more">
    <button type="button" class="spark-chip" hidden>Show all {{ research.papers.size }} papers</button>
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

  // Research browser: topic chips filter the paper cards. "All" shows the
  // first few papers with a button to reveal the rest.
  (function () {
    var section = document.getElementById("research");
    if (!section) return;
    var LIMIT = 6;
    var chips = section.querySelectorAll(".spark-filter .spark-chip");
    var cards = section.querySelectorAll(".spark-paper");
    var intro = section.querySelector(".spark-research-intro");
    var empty = section.querySelector(".spark-papers-empty");
    var more = section.querySelector(".spark-papers-more .spark-chip");
    var expanded = false;

    function apply(filter, question, emptyText) {
      var shown = 0;
      var matches = 0;
      cards.forEach(function (card) {
        var match = filter === "all" || card.dataset.themes.split(" ").indexOf(filter) !== -1;
        if (match) matches++;
        var visible = match && (filter !== "all" || expanded || shown < LIMIT);
        if (visible) shown++;
        card.hidden = !visible;
      });
      intro.textContent = filter === "all" ? intro.dataset.default : question;
      empty.hidden = matches > 0;
      empty.textContent = emptyText || "No papers in this area yet.";
      more.hidden = !(filter === "all" && !expanded && matches > LIMIT);
    }

    chips.forEach(function (chip) {
      chip.addEventListener("click", function () {
        chips.forEach(function (c) {
          c.classList.toggle("is-active", c === chip);
          c.setAttribute("aria-pressed", c === chip ? "true" : "false");
        });
        apply(chip.dataset.filter, chip.dataset.question, chip.dataset.empty);
      });
    });

    more.addEventListener("click", function () {
      expanded = true;
      apply("all");
    });

    apply("all");
  })();
</script>
