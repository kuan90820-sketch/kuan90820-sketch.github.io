---
layout: page
title: Projects
permalink: /projects/
---

# Projects

這裡整理我的研究、資料分析、政策與市場研究專案。每個專案都以「問題意識 → 方法 → 主要發現 → 可延伸方向」呈現。

<div class="project-grid">
{% for project in site.projects %}
  <a class="project-card" href="{{ project.url | relative_url }}">
    <p class="eyebrow">{{ project.category }}</p>
    <h2>{{ project.title }}</h2>
    <p>{{ project.summary }}</p>
  </a>
{% endfor %}
</div>
