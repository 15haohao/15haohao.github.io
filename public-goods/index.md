---
layout: default
title: Public Goods
---

# Public Goods

Below are tools, datasets, and templates I make publicly available.

<div class="grid">
{% for item in site.data.public_goods %}
  <a class="pg-card" href="{{ item.link }}" target="_blank" rel="noopener">
    <div class="pg-title">{{ item.title }}</div>
    <div class="pg-meta">{{ item.desc }}</div>
    <div class="pg-tags">
      {% for t in item.tags %}
        <span class="tag">{{ t }}</span>
      {% endfor %}
    </div>
    <div class="pg-meta" style="margin-top:10px;"><u>{{ item.link_text }}</u> →</div>
  </a>
{% endfor %}
</div>