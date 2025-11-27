---
layout: default
title: "Notes"
permalink: /notes/
---

<section class="hero-area pb-5">
  <div class="container">
    <div class="hero-logo">
      <img src="/assets/img//psychotherapist-mexico-tania-chapper.svg" class="img-fluid mt-5">
    </div>
    <div class="inside-container" >
        <h1 class="text-center mb-5">Blog</h1>
    </div>
  
  </div>
</section>

<section>
  <div class="container">
    <div class="inside-container">
      {% for post in site.posts %}
        <div class="blue-box">
          <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
          <p>{{ post.excerpt }}</p>
        </div>
      {% endfor %}
    </div>
  </div>
</section>