---
title: "Notes — Service36"
layout: default
---

# Технические заметки Сервис36.рф

Здесь будут собираться инженерные записи: наблюдения, грабли, интересные моменты по ремонту Apple.

<ul class="case-list">
  {% assign allnotes = site.notes | sort: "date" | reverse %}
  {% for n in allnotes %}
    <li>
      <a href="{{ n.url | relative_url }}">{{ n.title }}</a>
      {% if n.date %}
        <span style="color:#9b9ba0;"> — {{ n.date | date: "%d.%m.%Y" }}</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>
