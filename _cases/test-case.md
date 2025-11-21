---
layout: default
---

<main class="case">
  <article class="case-body">
    <header>
      <h1>{{ page.title }}</h1>
      {% if page.date %}
        <p class="case-date">{{ page.date | date: "%d %B %Y" }}</p>
      {% endif %}
    </header>

    <section class="case-content">
      {{ content }}
    </section>

    <footer class="case-footer">
      <p><a href="{{ '/cases/' | relative_url }}">← Back to all cases</a></p>
    </footer>
  </article>
</main>
