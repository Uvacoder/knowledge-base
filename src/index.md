---
title: Welcome to my own slightly opinionated knowledge base!
nav:
  order: 1
  title: Home
---

<h2>Web</h2>
<div class="stack">
{% for entry in collections.web %}
  <article class="card">
    <h2 class="card__title"><a href="{{ entry.url }}">{{ entry.data.title }}</a></h2>
    <p class="card__meta">{{ entry.date | date("Do MMMM YYYY") }}</p>
  </article>
{% endfor %}
</div>
