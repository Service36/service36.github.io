---
title: "Cases — Service36"
layout: default
---

# Кейсы ремонта устройств Apple

Ниже — реальные кейсы ремонта iPhone, iPad и Mac в Service36 (Воронеж).

{% assign grouped = site.cases | sort: "date" | reverse | group_by: "device" %}

<div class="device-grid">
  {% for group in grouped %}
    <div class="device-card">
      <h3>
        {% if group.name == "iphone" %}iPhone
        {% elsif group.name == "ipad" %}iPad
        {% elsif group.name == "mac" %}Mac / MacBook
        {% else %}Other{% endif %}
      </h3>
      <small>{{ group.items | size }} case(s)</small>
      <ul class="case-list">
        {% for c in group.items %}
          <li>
            <a href="{{ c.url | relative_url }}">{{ c.model | default: c.title }}</a>
            {% if c.date %}
              <span style="color:#9b9ba0;"> — {{ c.date | date: "%d.%m.%Y" }}</span>
            {% endif %}
          </li>
        {% endfor %}
      </ul>
    </div>
  {% endfor %}
</div>
