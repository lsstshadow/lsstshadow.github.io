---
layout: default
title: Home
---

<div class="intro">
  
  <h1> <span class="emoji">👻</span> {{ site.title }} <span class = "emoji">🦈</span> </h1>
  <p class="tagline">A collaboration of humans who want to find things that go bump in the night.</p>
  <img src="image.jpeg" alt="Observing Program" class="intro-image">
</div>

<section class="about">
  <p>
    Welcome to the {{ site.title }} homepage. We will be doing cool science with DECam as we shadow LSST, focussing on nearby galaxy clusters in order to find young transients!
  </p>
</section>

<h2>Latest Transient</h2>
{% assign latest_transient = site.categories.transients | first %}
<p><a href="{{ latest_transient.url }}">{{ latest_transient.title }}</a> <br>
<small>{{ latest_transient.date | date: "%B %d, %Y" }}</small></p>

<h2>Latest Publication</h2>
{% assign latest_pub = site.categories.publications | first %}
<p><a href="{{ latest_pub.url }}">{{ latest_pub.title }}</a> <br>
<small>{{ latest_pub.date | date: "%B %d, %Y" }}</small></p>

<h2>Featured Team Member</h2>
<div id="featured-member"></div>

<script>
  const team = [
    { name: "Richard Gecko", role: "Overlord", photo: "richard.jpg" },
  ];

  // Pick based on day of the year so it changes daily
  const today = new Date();
  const index = today.getDate() % team.length; // or use getDay() for day-of-week
  const member = team[index];

  document.getElementById("featured-member").innerHTML = `
    <img src="${member.photo}" alt="${member.name}" style="width:150px;border-radius:50%;">
    <h3>${member.name}</h3>
    <p>${member.role}</p>
  `;
</script>


<section class="highlights">
  <div class="highlight-box">
    <h2>Latest Transient</h2>
    <p><a href="/transients/latest">SN2025abc discovered at ZTF</a></p>
  </div>

  <div class="highlight-box">
    <h2>Latest Publication</h2>
    <p><a href="/publications/latest">"Shock Interaction in SN2023jgf"</a></p>
  </div>

  <div class="highlight-box">
    <h2>Featured Team Member</h2>
    <p><a href="/team/jane-doe">Jane Doe</a></p>
  </div>
</section>

<section class="highlights">
  <div class="highlight-box">
    <h2>Latest Transient</h2>
    {% assign latest_transient = site.categories.transients | first %}
    <p><a href="{{ latest_transient.url }}">{{ latest_transient.title }}</a> <br>
    <small>{{ latest_transient.date | date: "%B %d, %Y" }}</small></p>
  </div>

  <div class="highlight-box">
    <h2>Latest Publication</h2>
    {% assign latest_pub = site.categories.publications | first %}
    <p><a href="{{ latest_pub.url }}">{{ latest_pub.title }}</a> <br>
    <small>{{ latest_pub.date | date: "%B %d, %Y" }}</small></p>
  </div>

  <div class="highlight-box">
    <h2>Featured Team Member</h2>
    <div id="featured-member"></div>
  </div>
</section>

<section class="highlights">
  <div class="highlight-box">
    <h2>Latest Transient</h2>
    {% assign latest_transient = site.categories.transients | first %}
    <p>
      <a href="{{ latest_transient.url }}">{{ latest_transient.title }}</a><br>
      <small>{{ latest_transient.date | date: "%B %d, %Y" }}</small>
    </p>
  </div>

  <div class="highlight-box">
    <h2>Latest Publication</h2>
    {% assign latest_pub = site.categories.publications | first %}
    <p>
      <a href="{{ latest_pub.url }}">{{ latest_pub.title }}</a><br>
      <small>{{ latest_pub.date | date: "%B %d, %Y" }}</small>
    </p>
  </div>

  <div class="highlight-box">
    <h2>Featured Team Member</h2>
    <div id="featured-member"></div>
  </div>
</section>

<script>
  const team = [
    { name: "Richard Gecko", role: "Role:Overlord", photo: "richard.jpg" },

  ];

  // Rotate daily based on day of the year
  const today = new Date();
  const index = today.getDate() % team.length;
  const member = team[index];

  document.getElementById("featured-member").innerHTML = `
    <img src="${member.photo}" alt="${member.name}" style="width:100px;border-radius:50%;margin-bottom:10px;">
    <h3>${member.name}</h3>
    <p>${member.role}</p>
  `;
</script>

