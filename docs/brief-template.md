# 每日早报模板

供后续定时任务对照。不要编造数字、引语、标题或行情；每一项都要有当次抓取的来源链接，时间换算为 Asia/Shanghai（UTC+8）并标注时区。

## 文件

- 路径：`_posts/YYYY-MM-DD-daily-brief.md`
- 建议固定 permalink：`/YYYY/MM/DD/daily-brief/`

## Front matter

```yaml
---
layout: post
title: "早报 · YYYY-MM-DD"
date: YYYY-MM-DD HH:MM:SS +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 全球头条, Hacker News, X, 微博]
collected_at: "YYYY-MM-DD HH:MM:SS Asia/Shanghai (UTC+8)"
permalink: /YYYY/MM/DD/daily-brief/
---
```

若当天是补发或下午编发，在文首说明，不要假装写于 09:00 之前。

## 正文结构（按此顺序）

1. **金融市场**：黄金 XAU/USD；美元兑人民币（准确标注是中间价还是市场化参考汇率）；上证指数 000001；深证成指 399001。列出数值、涨跌（如有）、来源链接、采集时间。A 股若仍在交易，写明「盘中」。
2. **全球头条**：BBC World、BBC 中文、NYT World、The Guardian World；路透或美联社仅在源实际可用时加入。中文摘要，保留原标题与链接，不整篇转载。
3. **Hacker News 近期文章**：抓取当前首页（Algolia `https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30` 或官方首页 / hnrss）。对最热或讨论最多的 8–12 篇打开原文（并用 HN 讨论作评论语境），写中文摘要，保留英文标题，同时链接原文与 HN 帖。引语最多一两句，不转载全文。其余首页条目用短列表：英文标题、链接、一行中文、HN 点数与评论数。检查链接时只丢掉真正的 404；401/403/405 仍可列出。时间用 Asia/Shanghai。
4. **X 热门与科技圈**：全球及有关地区趋势，加上 AI/IT 圈讨论。使用已安装的 X 公共连接器工具，不要自造接口。摘要并分析，引用帖子或趋势链接。未核实传言标明「在流传」。明显的假模型名垃圾信息可省略。
5. **微博热搜**：请求 `https://weibo.com/ajax/side/hotSearch`，使用桌面 User-Agent、`Referer: https://weibo.com/`、`Accept: application/json`。区分置顶/政务（hotgov）、自然热搜与广告。科技、AI、IT、国际、重大社会话题写摘要与分析；纯娱乐放进「速览」。链接到 `s.weibo.com` 搜索页。接口失败时在文中说明，不要编造话题。
6. **今日总结**：短评当天的信息环境。

## 文风

- 正文用中文，外文与 HN 标题保持英文。
- 用 Markdown 链接引用。
- 不编造，不整篇转载受版权保护的文本。
