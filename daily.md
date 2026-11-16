---
layout: page
title: 每日早报
permalink: /daily/
subtitle: 按日期排列的每日信息整理。可用标签过滤主题，每篇文章都保留出处链接。
---

<p class="source-note">惯例是每个自然日一篇，文件位于仓库 <code>_posts/YYYY-MM-DD-daily-brief.md</code>。首期于 2026-11-16 下午编发，之后计划在每天 09:00（Asia/Shanghai，UTC+8）前更新。</p>

{% assign briefs = site.posts | where_exp: "post", "post.categories contains 'daily' or post.category == 'daily'" %}
{% if briefs.size == 0 %}
  <p class="empty">还没有早报。</p>
{% else %}
  {% assign year = "" %}
  {% for post in briefs %}
    {% assign y = post.date | date: "%Y" %}
    {% if y != year %}
      {% assign year = y %}
      <h2>{{ year }}</h2>
    {% endif %}
    {% include post-card.html %}
  {% endfor %}
{% endif %}
