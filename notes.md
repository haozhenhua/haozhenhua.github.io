---
layout: page
title: 阅读笔记
permalink: /notes/
subtitle: 个人摘录、批注与读后感。与每日早报分开存放。
---

<p class="empty">这一栏目前是空的。之后会把值得留下来的阅读笔记以 Markdown 文章的形式放在这里，同样可以按标签和日期查找。</p>

{% assign notes = site.posts | where_exp: "post", "post.categories contains 'notes' or post.category == 'notes'" %}
{% if notes.size > 0 %}
  {% for post in notes %}
    {% include post-card.html %}
  {% endfor %}
{% endif %}
