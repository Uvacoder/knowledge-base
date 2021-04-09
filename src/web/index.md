---
title: Web
nav:
  order: 2
---

These are latest changes in the Web section :

<div class="stack">

{% for entry in collections.web %}

  <article class="card">
    <h2 class="card__title"><a href="{{ entry.url }}">{{ entry.data.title }}</a></h2>
    <p class="card__meta">{{ entry.date | date("Do MMMM YYYY") }}</p>
  </article>
{% endfor %}

</div>
