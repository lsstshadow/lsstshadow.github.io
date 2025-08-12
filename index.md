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

