---
title: "Cases — Service36"
layout: default
---

# 📱 Все кейсы ремонта

Ниже список всех кейсов, которые опубликованы на Service36 GitHub Pages.

{% assign all = site.cases | sort: "date" | reverse %}
<ul>
  {% for c in all %}
    <li>
      <a href="{{ c.url | relative_url }}">{{ c.title }}</a>
      {% if c.date %}
        — <span style="color:#777">{{ c.date | date: "%d.%m.%Y" }}</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>
