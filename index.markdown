---
layout: default
---

<div class="row g-5 mb-5">
  <div class="col-md-6">
    <h3 class="fw-bold">Projects</h3>
    {{ content }}
  </div>
  <div class="col-md-6">
    <img src="https://scitechdaily.com/images/Sun-Earth-Gravity-General-Relativity.jpg" alt="Home" width="10%">
  </div>
</div>

<div class="row g-5 mb-5">
  <div class="col-md-12">
    <h3 class="fw-bold border-bottom pb-3 mb-5">Blog Posts</h3>
    {% for post in site.posts %}
      <p><a href="{{ site.github.url }}/{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %-d, %Y" }}</p>
    {% endfor %}
  </div>
</div>
