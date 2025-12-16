---
layout: default
title: "Notes & Articles"
permalink: /notes/
description: "Notes and articles on psychotherapy, somatic therapy and spiritual therapy... And everything in between."
---



<section>
  <div class="container">
  <h1 class="text-center mt-5">Notes</h1>
    <div class="inside-container">
      {% for post in site.posts %}
        <div class="blue-box">
          <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
          <p class="mb-0"><em>{{ post.date | date: "%B %d, %Y" }}</em></p>
        </div>
      {% endfor %}
    </div>
  </div>
</section>