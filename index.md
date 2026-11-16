---
layout: default
title: 首页
---

<section class="intro prose">
  <h1>阅读过滤</h1>
  <p>这是 haozhenhua 的个人主页，用来过滤、摘要和编辑日常读到的信息。站点以博客形式发布，不经营新闻业务。公开来源的每日整理放在「每日早报」，自己的摘录与评论放在「阅读笔记」。</p>
</section>

<h2 class="section-head">最新文章</h2>
{% if site.posts.size == 0 %}
  <p class="empty">还没有文章。</p>
{% else %}
  {% for post in site.posts limit: 12 %}
    {% include post-card.html %}
  {% endfor %}
{% endif %}

{% if site.posts.size > 12 %}
  <p><a href="{{ "/daily/" | relative_url }}">查看全部每日早报</a></p>
{% endif %}
