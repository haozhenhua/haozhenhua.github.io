---
layout: post
title: "早报 · 2026-11-26"
date: 2026-11-26 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-26 07:50:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/26/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 26 日（星期四）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:36–07:37 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:36–07:37，原文页约在 07:41–07:42；X 热榜与科技圈检索约在 07:37–07:44；油管频道页约在 07:38，节目页约在 07:42；神舟二十四号官方稿约在 07:44 核对。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 feeds.reuters.com 再次 TLS 连接失败，www.reuters.com/world/rss 返回 401；美联社经由 RSSHub 的源返回 403；《卫报》World / International RSS 返回 403；《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写；东方财富行情接口返回 502；新浪财经简况接口在加 Referer 后可用。均已在相应栏目说明。写稿时尚未到 09:15 中间价和 09:30 开盘，人民币中间价与 A 股本期采用 11 月 25 日（星期三）已公布的官方读数。神舟二十四号已于昨日 08:18 发射成功，乘组下午进驻「天宫」，本期按官方稿续报。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期四，写稿时官方中间价和开盘价尚未公布，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 docs/brief-memory/finance-history.json。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,571.30 美元/盎司 | 较上一期早报（2026-11-25 07:36:14 Asia/Shanghai (UTC+8)）+8.45（+0.24%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 3571.300049，报价单位为美元/盎司；updatedAt 为 2026-11-25T23:36:17Z（合 2026-11-26 07:36:17 Asia/Shanghai）。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,562.85）计算 | 2026-11-26 07:36:17 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7088（11 月 25 日） | 较上一发布日（2026-11-24，6.7111）变动 −0.0023 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-26 07:36:33 返回的最新一条是 11 月 25 日的 6.7088；更早记录为 11 月 24 日 6.7111、11 月 23 日 6.7120、11 月 20 日 6.7131、11 月 19 日 6.7128。**本期采用 11 月 25 日已公布中间价**（写稿时尚未到当日 09:15 发布时间）。变化栏按官方上一发布日口径 | 采集 2026-11-26 07:36:33 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.678179 | 较上一期早报（2026-11-24 08:02:31 Asia/Shanghai (UTC+8)）−0.001120（−0.02%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。time_last_update_utc 为 Wed, 25 Nov 2026 00:02:31 +0000（合 2026-11-25 08:02:31 Asia/Shanghai），较上一期早报所用的 11 月 24 日那一笔日更已刷新；time_next_update_utc 显示为 Thu, 26 Nov 2026 00:35:41 +0000（约合 08:35:41 Asia/Shanghai），采集时尚未到达 | 2026-11-25 08:02:31 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3476.47 | −71.90（−2.03%） | [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 返回：最新价 3476.47，涨跌 −71.90，涨跌幅 −2.03%，昨收 3548.37，开盘 3522.59，最高 3526.34，最低 3468.65，行情时间戳 20261125161427（2026-11-25 16:14:27）。[新浪财经](https://hq.sinajs.cn/list=s_sh000001,s_sz399001) 交叉核对价格一致（3476.4697，涨跌 −71.8997），涨跌幅同为 −2.03%。[东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 本次返回 502，故不以它为数值来源。写稿时尚未开盘，**本期采用 11 月 25 日（星期三）收盘价，不是今日盘中或开盘价** | 采集 2026-11-26 07:36:33 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10086.36 | −337.24（−3.24%） | 同上来源：腾讯财经最新价 10086.36，涨跌 −337.24，涨跌幅 −3.24%，昨收 10423.60，开盘 10272.19，最高 10402.35，最低 10086.36，行情时间戳 20261125161448（2026-11-25 16:14:48）。新浪财经交叉核对价格与涨跌幅一致（10086.36，涨跌 −337.248，−3.24%） | 采集 2026-11-26 07:36:33 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报小幅回升约 0.24%，报 3,571.30 美元/盎司，把前一日回落吐出了一点。市场化参考汇率随接口日更从 11 月 24 日那一笔刷新为 11 月 25 日的 6.678179，较上一期所用读数只小幅回落 0.02%。官方中间价本期改用 11 月 25 日已公布的 6.7088，较 11 月 24 日中间价下调 0.0023；A 股本期采用 11 月 25 日收盘价，上证跌 2.03%，深成指跌 3.24%，是近期较重的一天。这些官方数字都不是今日开盘或收盘。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [/api/weather/view?stationid=54511](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 lastUpdate 为 2026/11/26 07:25；本次采集时间为 2026-11-26 07:36:41 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。预警列表为空。接口的实况对象未给出天气现象字段，故不编造当前天空状况。

**当前实况**（lastUpdate 2026/11/26 07:25）：气温 2.3℃，体感温度 −0.3℃，相对湿度 56%，东北风微风，风速 1.3 米/秒，降水量 0.0，气压 1006.0 百帕。

**今日（11 月 26 日）预报**：白天多云，最高 13℃，西南风微风；夜间多云，最低 2℃，西北风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 27 日 | 白天晴，夜间晴 | 10℃ / −1℃ | 白天西北风 3～4 级，夜间西北风微风 |
| 11 月 28 日 | 白天晴，夜间晴 | 10℃ / −1℃ | 白天西风微风，夜间西南风微风 |
| 11 月 29 日 | 白天晴，夜间晴 | 12℃ / 1℃ | 白天南风微风，夜间西北风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 docs/brief-memory/seen.json。昨日及此前已写过的海淀区委常委会、区政府常务会、十一届区政协履职总结、「光影智谷」、教育人才培育、交通调研等，以及昌平的城北街道城市更新、跨国药企圆桌、脑机接口大会、劳务品牌等，不再重复。今天海淀栏有东部片区街镇工作座谈；昌平则有生命科学园高质量发展调研、美丽健康产业与多美康，以及波兰企业代表团参观。

#### 海淀区

**[区委召开东部片区街镇工作座谈会议](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261125_4836499.shtml)**。来源：海淀报，日期 2026-11-25 09:24。稿件称，会议于 11 月 24 日召开，区委书记王少峰主持，东升镇及学院路、花园路、北太平庄、北下关、西三旗、清华园、燕园等街道依次发言。报道写，王少峰肯定东部片区资源密集、创新活跃，并围绕打造场景街区、法治街区、花园街区、温暖街区、文化街区、安全街区与健康街区提出要求，强调高校智库与基层法治实践双向赋能，以及工程建设廉洁关与「亲」「清」政商关系。区领导肖丹、邹凌、沈烨参加。这些安排与表述均来自报道本身。

#### 昌平区

**[区领导围绕区域高质量发展开展调研](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112420540961828/index.html)**。来源：北京昌平 APP，时间 2026-11-24 21:09。稿件称，11 月 24 日区委书记、未来科学城党工委书记甘靖中带队到中关村生命科学园三期调研，先后察看脑科学与脑机接口创新展示中心、生命谷国际前沿科技转化中心。报道转述其要求：坚持产业先行，加快建设「生命谷」；加快招商与资金链支撑，完善人才引育；推进园区周边交通、绿化与市政配套，推动一、二、三期连片成势，并前瞻布局 AI 赋能药物研发等赛道。区领导刘卫华、赵仕伟参加。

**[活力昌平 未来之城｜昌平美丽健康产业加速跑，多美康领跑重组胶原蛋白创新赛道](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112416210937947/index.html)**。来源：北京昌平 APP，时间 2026-11-24 16:36。稿件介绍在昌企业多美康（北京）生物医药有限公司依托昌发展合成生物制造转化加速中心，研发拥有 1068 个氨基酸的全长Ⅲ型重组人源胶原蛋白，并称企业累计获得 56 项国内外专利、4 项独有原料技术及沙利文「1068 开创者」认证；昌发展方面则介绍高通量菌株筛选、质谱检测与医用材料生物制造等平台。专利数量、认证名称与平台能力均为稿件与企业/平台说法。

**[波兰企业代表团赴生命科学园参观调研](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112410270725520/index.html)**。来源：北京昌平 APP，时间 2026-11-24 10:42。稿件称，11 月 23 日昌平交易分团在 2026 年服贸会后组织专项交流，邀请波兰企业代表团参观合成生物制造转化加速中心、北京飞镖国际创新平台和生命科学园展厅，并就医药健康产业链、创新平台与外资扶持政策座谈。北京博锐开放政策研究院院长靳辉参加。

## 3. 全球头条

BBC World、BBC 中文与《纽约时报》World RSS 可用；《卫报》World/International RSS 返回 403；路透社与美联社源不可用，已如实说明。已在 seen.json 中出现过的陈吉宁被查、华为纽约分项裁决、黄仁勋复职、COP31 破裂、利比亚俄舰遇袭等不再展开，只写有实质新进展或新头条的条目。

**续报 · 神舟二十四号。** [中国载人航天工程网](https://www.cmse.gov.cn/xwzx/202611/t20261125_57891.html) 2026-11-25 稿：北京时间 11 月 25 日 8 时 18 分，长征二号 F 遥二十四运载火箭在酒泉点火，约 10 分钟后神舟二十四号进入预定轨道，发射取得圆满成功；这是空间站应用与发展阶段第 8 次载人飞行、工程立项以来第 41 次发射，也是首次有外籍航天员参与。[新华社](https://www.news.cn/20261125/6cd1bfb2c62346d09b002ba4dd502b2a/c.html) 综合稿补充：11 时 56 分飞船对接天和核心舱前向端口，用时约 3.5 小时；14 时 35 分汤洪波、武毅、穆罕默德·齐尚·阿里进驻「天宫」，与神舟二十三号乘组会师，中外航天员实现首次「太空握手」；按计划巴基斯坦航天员齐尚·阿里完成短期联合飞行后将随神二十三返回。[BBC 中文](https://www.bbc.com/zhongwen/articles/cm9w91y0pge7o/simp) 与 [BBC 视频稿](https://www.bbc.co.uk/news/videos/cmz74l0yzzvyo) 亦报道发射与首位巴基斯坦航天员登站。昨日早报写稿时发射尚未开始，本期按官方结果续报。

**[US announces new tariffs on host of countries including China](https://www.bbc.co.uk/news/articles/c893r9ke5p97o)**（BBC，2026-11-25）。报道称，美国宣布新一轮关税，触及中国、欧盟及新加坡、瑞士、印尼、马来西亚、柬埔寨、泰国、韩国、越南、台湾、孟加拉、日本、印度等；文中写中国面临最高至约 40% 的税率，越南至约 35%，其余多为 20% 或 25%，且部分税率会因既有上限安排而实际降低。贸易代表 Jamieson Greer 称此举意在「为美国工人拉平赛场」；报道同时提醒经济学家对通胀与贸易放缓的担忧。[BBC 中文](https://www.bbc.com/zhongwen/articles/cm9d7g967l5lo/simp) 同步有简体稿。具体税率与名单以 BBC 正文为准，不是中国海关或商务部口径。

**[US stocks fall further as fears over AI intensify](https://www.bbc.co.uk/news/articles/cq0md8g14zryo)**（BBC，2026-11-25）。报道写，黄仁勋复职带来的英伟达反弹并未持续，三大美股指数收跌，纳斯达克收跌约 0.6%；英伟达早盘一度跌约 8%，收跌约 3.4%。文中把抛售与 AI 投资可持续性、中期选举后监管预期以及当日新关税消息并置，未单独给出「泡沫破裂」的官方定义。

**[Israeli judges recommend dropping most serious charges against Netanyahu](https://www.bbc.co.uk/news/articles/cxj05mv723r2o)**（BBC，2026-11-25）。耶路撒冷地方法官小组罕见约见总检察长，称 Case 4000（涉嫌以政务换取媒体正面报道）定罪希望很低，并对 Case 2000 是否构成刑事门槛提出疑问，同时建议就 Case 1000 寻求辩诉交易。内塔尼亚胡否认指控，并呼吁立即结束审判。《纽约时报》同题 RSS 摘要写法官建议撤销关键腐败案件中的关键指控；正文页 403，未打开。

**[Thirty-one killed in massive fire as fuel tanker crashes on Cairo highway](https://www.bbc.co.uk/news/articles/cqy7rn30v314o)**（BBC，2026-11-25）。开罗附近公路油罐车事故引发大火，报道称至少 31 人死亡、21 人受伤。《纽约时报》RSS 标题同写至少 31 死、21 伤。

**[US Army says controlled blast of explosives in Iowa was 'huge success'](https://www.bbc.co.uk/news/articles/cwg7l5ve251ko)**（BBC，2026-11-25）。美军在艾奥瓦州引爆近 5 吨不稳定叠氮化铅，代理陆军部长 Adam Telle 称「巨大成功」，并称监测读数「目前未见高于 0.0」。此事前几日已因法院禁令与居民抗议进入早报，本期按「已实施」续报，不以社媒口号代替环保部门完整报告。

**[North Korea expels Swiss diplomat in sanctions row](https://www.bbc.co.uk/news/articles/cq0l34e4kkr5o)**（BBC，2026-11-25）。报道称朝方驱逐瑞士外交官，背景与瑞士制裁一处被指接纳乌克兰儿童进行「洗脑」的国际青年营有关；瑞士称将通过伯尔尼的朝鲜使馆及驻北京使馆维持联系。《纽约时报》RSS 标题写「因与乌克兰战争相关的争执踢出瑞士外交官」，正文页未打开。

**[Is China behind a wave of AI fake videos targeting Taiwan?](https://www.bbc.co.uk/news/articles/cv702rw7dzx5o)**（BBC，2026-11-24/25）。BBC 核实报道称，一批与中国有关的账号用 AI 生成视频攻击民进党关键人物，包括总统赖清德与台北市长候选人沈伯洋；是否构成国家层面的系统行动，报道本身仍以调查措辞呈现，本期不写成已定论的「官方操作」。

《纽约时报》World RSS 另有毛里求斯流浪狗、匈牙利秘密警察档案公开、南非拉马福萨「农场门」弹劾调查被法院叫停、印尼矿难、所罗门群岛与澳大利亚安全条约等标题，因正文 403，只作线索、不展开。

## 4. Hacker News 近期文章

首页来自 [Algolia HN API](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集约 2026-11-26 07:36 Asia/Shanghai（UTC+8）。对讨论最热的条目打开原文写摘要；其余列短表。时间换算为 Asia/Shanghai。

### 重点摘要

**[The matrix multiplication exponent is nine fourths [pdf]](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf)** · [HN](https://news.ycombinator.com/item?id=50637220) · 1015 分 / 566 评 · 2026-11-25 09:19 Asia/Shanghai。OpenAI math 仓库 2026-11-24 预印本摘要写：在任意域上证明方阵乘法指数 ω 恰为 9/4；上界此前已知，本文给出匹配下界，并称对每个 n≥2，形式算术电路至少需要 n 的 9/4 次方除以 2（向上取整）个乘法或除法门。这是论文自己的定理陈述，不是第三方复核结论。同仓库还有多项式 Hirsch 猜想被证伪等稿，见短列表。

**[1Password Security Incident](https://1password.com/blog/update-on-nov-2026-security-incident)** · [HN](https://news.ycombinator.com/item?id=50644817) · 1005 分 / 426 评 · 2026-11-26 01:18 Asia/Shanghai。官方博客称，攻击者经员工企业 GitHub 账号进入后端，复制了部分客户账户信息（姓名、登录邮箱、账户标识、公钥与部分邮件链接令牌等）；**保险库内容与保护密钥未受影响**，公司已做遏制、恢复干净服务并轮换内部凭证，用户「不必在账户里改任何东西」，但应警惕钓鱼邀请/恢复邮件。事件调查起始日期写为 2026-11-19。

**[Holy shit holy shit holy shit holy shit: The magnitude of what’s now happening](https://scottaaronson.blog/?p=10379)** · [HN](https://news.ycombinator.com/item?id=50646108) · 763 分 / 602 评。Scott Aaronson 博文标注 Wednesday, November 25th, 2026 at 1:01 pm（博客未标明时区）。他把 OpenAI / Anthropic 连发带 Lean 证书的复杂度结果写成「奇点感觉」：包括 ω=9/4、VP≠VNP、FFT 线性门下界等；他写自己「virtually certain」实验室还握有未公开的密码学「重磅」，但**明确拒绝传播未经核实的具体算法传言**，并劝读者不要把焦点缩成「比特币钱包」。引语与判断均来自博文本身。

**[Google releases Cogentic papers on integer factorization, discrete logs and more](https://github.com/google-research/google-research/tree/master/cogentic_research_papers)** · [HN](https://news.ycombinator.com/item?id=50642086) · 423 分 / 320 评 · 2026-11-25 21:33 Asia/Shanghai。Google Research 目录 cogentic_research_papers 下列出 integer_factorization、discrete_logarithm、deterministic_factoring_l34、logrank_conjecture、bimatrix_nash_equilibrium 等子目录与 PDF。是否构成可部署破译、以及 Lean/人工复核进度，首页讨论很热，但目录页本身不是安全公告；本期只记仓库发布，不写成「RSA 已死」。

**[Models Can Communicate via Inference Servers Despite Being Sandboxed](https://www.lesswrong.com/posts/7wzWuLP3HhyBLmKfo/models-can-communicate-via-inference-servers-despite-being)** · [HN](https://news.ycombinator.com/item?id=50637686) · 444 分 / 190 评 · 2026-11-25 10:34 Asia/Shanghai。LessWrong 帖讨论沙箱隔离下的模型仍可能经推理服务侧信道通信。本次打开原文返回 429，摘要仅据标题与 HN 讨论语境，不引用正文句子。

**[Button Sounds – collection of professionally-recorded button clicks and presses](https://buttons.joshwcomeau.com/)** · [HN](https://news.ycombinator.com/item?id=50638032) · 835 分 / 131 评。Josh Comeau 的按钮点击音效收藏站；页面可打开，属趣味工具帖。

**[A few questions for the guy who went snorkeling in a Home Depot retention pond](https://www.vox.com/down-to-earth/511999/home-depot-retention-pond-snorkel-joseph-ricketts)** · [HN](https://news.ycombinator.com/item?id=50643129) · 418 分 / 100 评。Vox 追问一篇关于有人在 Home Depot 滞留池浮潜的奇闻。

**[Windows Loudness Equalization, reverse-engineered and ported to PipeWire](https://github.com/xoxorwr/pw-loudness-eq)** · [HN](https://news.ycombinator.com/item?id=50641171) · 304 分 / 173 评。开源项目把 Windows 响度均衡思路逆向并移植到 PipeWire。

**[Smart people who give a shit use tools](https://www.iankduncan.com/engineering/2026-11-19-smart-people-who-give-a-shit-use-tools)** · [HN](https://news.ycombinator.com/item?id=50639698) · 249 分 / 190 评。工程随笔，讨论认真工作的人如何对待工具链。

**[Porting Rockbox to an undocumented $9 AliExpress 'YP3' MP3 player with LLMs](https://jayd.ml/2026/11/14/rockbox-on-yp3.html)** · [HN](https://news.ycombinator.com/item?id=50624446) · 205 分 / 85 评。作者记录在几乎无文档的廉价播放器上，借助 LLM 把 Rockbox 移植上去。

**[I checked Clojure's core with Lean and found unreported bugs](https://s.conao3.com/blog/2026/e4f733)** · [HN](https://news.ycombinator.com/item?id=50642939) · 169 分 / 58 评。用 Lean 检查 Clojure 核心库并报告此前未公开的问题。

**[Much shorter version of GRH Lean verification from Anthropic](https://github.com/lsernau/grh-lean)** · [HN](https://news.ycombinator.com/item?id=50648050) · 164 分 / 66 评。仓库简介写 A short Lean 4 proof of the Generalized Riemann Hypothesis。与前几日 Anthropic / Alpöge 相关 GRH 讨论同属一条证明线的衍生物，是否被广泛接受仍看形式化社区，不在此宣布「黎曼猜想已结案」。

**[Nfs2root: A 12-year-old pre-auth remote root in the Linux kernel's NFS server](https://opensec.in/blog/nfs2root-cve-2026-99362)** · [HN](https://news.ycombinator.com/item?id=50647161) · 58 分 / 18 评。安全研究称 Linux NFS 服务端存在约 12 年的预认证远程 root（CVE-2026-99362）；细节以作者博文为准。

### 首页其余条目

| 标题 | 点数 / 评论 | 链接 |
| --- | --- | --- |
| GPT-6.2 Astra is the first model to beat Googlers' code golf records | 176 / 39 | [原文](https://bjin.github.io/go-codegolf-benchmark/) · [HN](https://news.ycombinator.com/item?id=50601280) |
| SSH is a GUI framework | 111 / 57 | [原文](https://zydra.sh/articles/ssh-is-a-gui-framework/) · [HN](https://news.ycombinator.com/item?id=50589784) |
| The New York Times tells photographers not to use the latest Photoshop | 105 / 52 | [原文](https://www.dpreview.com/news/new-york-times-adobe-photoshop-2027-restriction-ai/)（本次 403）· [HN](https://news.ycombinator.com/item?id=50647673) |
| The polynomial Hirsch conjecture is false [pdf] | 105 / 24 | [原文](https://github.com/openai/math/blob/main/preprints/Superpolynomial-graph-diameter-of-simple-polytopes-November-24-2026/paper.pdf) · [HN](https://news.ycombinator.com/item?id=50644980) |
| Predicting LoRA size for any dataset | 103 / 11 | [原文](https://engram.com/blog/lora-size) · [HN](https://news.ycombinator.com/item?id=50635783) |
| In C++, = default and {} are not the same constructor | 98 / 158 | [原文](https://lemire.me/blog/2026/11/02/default-and-braces-are-not-the-same-constructor/) · [HN](https://news.ycombinator.com/item?id=50643199) |
| Slow Ubuntu security response times | 84 / 29 | [原文](https://www.openwall.com/lists/oss-security/2026/11/25/9) · [HN](https://news.ycombinator.com/item?id=50647181) |
| Britain's ghost stations | 80 / 17 | [原文](https://spectator.com/article/britains-ghost-stations-are-fascinating/) · [HN](https://news.ycombinator.com/item?id=50645074) |
| 72-Hour Fasting Can Reset Your Immune System, USC Study Shows | 75 / 30 | [原文](https://scienceinhand.com/72-hour-fasting-can-reset-your-entire-immune-system-usc-study-shows/) · [HN](https://news.ycombinator.com/item?id=50647158) |
| Show HN: An agent skill that optimizes code with falsifiable hypotheses | 57 / 7 | [原文](https://chszlab.github.io/AgenticAlgorithmEngineering/) · [HN](https://news.ycombinator.com/item?id=50611593) |
| Defang Security Incident | 40 / 14 | [原文](https://defang.io/blog/post/security-incident-november-2026/) · [HN](https://news.ycombinator.com/item?id=50648035) |
| The undocumented 249-file limit for Googlebot rendering | 25 / 9 | [原文](https://www.fullstackoptimization.com/a/googlebot-249-file-rendering-limit) · [HN](https://news.ycombinator.com/item?id=50619073) |
| Show HN: Rchive – Every drive I've owned since the 90s, searchable in one window | 24 / 14 | [原文](https://www.rchive.computer/) · [HN](https://news.ycombinator.com/item?id=50624684) |
| Jev is (probably) Qwen3.5-35B-A3B | 14 / 0 | [原文](https://modaic.dev/blog/latency-doesnt-lie) · [HN](https://news.ycombinator.com/item?id=50648823) |

招聘帖 Hazel (YC W24) 未计入讨论。

## 5. X 热门与科技圈

全球趋势（WOEID 1）与美国趋势在采集时几乎被 [Thanksgiving](https://x.com/search?q=Thanksgiving)、NFL（[Steelers](https://x.com/search?q=Steelers)、[Packers](https://x.com/search?q=Packers)、[McCarthy](https://x.com/search?q=McCarthy)、[Rodgers](https://x.com/search?q=Rodgers)）和足球话题占据；美国榜另有 [USAID](https://x.com/search?q=USAID)（约 26.7 万帖）与 [McAfee](https://x.com/search?q=McAfee)。中国区趋势接口返回内容与全球高度重合，参考价值有限。

**科技 / AI。** 讨论焦点仍是实验室数学稿与美股 AI 抛售，而不是单一产品发布。高互动帖里，[TokenGremlin](https://x.com/TokenGremlin/status/2125598511664087114) 把 OpenAI 九篇带 Lean 证明的数学稿（含 ω=9/4、Smale 第 9 问题等）写成「今日八卦」；[choblin29](https://x.com/choblin29/status/2125684567281717404) 则放大 Aaronson「virtually certain… bombshells for cryptography」一句——**这是对博文的二次传播，Aaronson 本人已声明不愿为未经核实的具体破译传言背书**，故只记「在流传」，不写成事实。市场侧，多条帖把纳斯达克盘中深跌、英伟达回吐与「AI 泡沫」叙事绑在一起，数字彼此不完全一致，以 BBC 收盘叙述为准，不采相互冲突的盘中截图。

**USAID Files。** [DataRepublican](https://x.com/DataRepublican/status/2125618035100659996) 等账号交叉比对其所谓 Democracy Files 与 USAID 文件，获大量转发；内容涉及对外援助、社媒协调等主张。这些材料的完整性、编选与解读仍有争议，本期仅记其为感恩节前后美国政治传播中的热话题，不逐条当真。

X 新闻摘要还提到伯尼·桑德斯警告 AI 泡沫、罗姆尼批评对华芯片销售矛盾、Polymarket 上 GPU 租金预测市场、深圳灰市英伟达芯片等；后几条带明显传闻色彩，未独立核实前不展开。

## 6. 微博热搜

接口 [weibo.com/ajax/side/hotSearch](https://weibo.com/ajax/side/hotSearch) 于 2026-11-26 07:37 Asia/Shanghai（UTC+8）返回成功。置顶政务为 [#中巴领导人就神24飞天互致贺电#](https://s.weibo.com/weibo?q=%23%E4%B8%AD%E5%B7%B4%E9%A2%86%E5%AF%BC%E4%BA%BA%E5%B0%B1%E7%A5%9E24%E9%A3%9E%E5%A4%A9%E4%BA%92%E8%87%B4%E8%B4%BA%E7%94%B5%23)。

**摘要与分析。** [神24乘组进驻天宫](https://s.weibo.com/weibo?q=%23%E7%A5%9E24%E4%B9%98%E7%BB%84%E8%BF%9B%E9%A9%BB%E5%A4%A9%E5%AE%AB%23)、[巴基斯坦电视主持人激动播报](https://s.weibo.com/weibo?q=%23%E5%B7%B4%E5%9F%BA%E6%96%AF%E5%9D%A6%E7%94%B5%E8%A7%86%E4%B8%BB%E6%8C%81%E4%BA%BA%E6%BF%80%E5%8A%A8%E6%92%AD%E6%8A%A5%23)、[首位外籍航天员进天宫机密如何保障](https://s.weibo.com/weibo?q=%E9%A6%96%E4%BD%8D%E5%A4%96%E7%B1%8D%E8%88%AA%E5%A4%A9%E5%91%98%E8%BF%9B%E5%A4%A9%E5%AE%AB%E6%9C%BA%E5%AF%86%E5%A6%82%E4%BD%95%E4%BF%9D%E9%9A%9C) 与官方发射/进驻结果同向，属昨日早报「发射窗口」的后续热度。[小米SU7 Ultra上工信部](https://s.weibo.com/weibo?q=%E5%B0%8F%E7%B1%B3SU7%20Ultra%E4%B8%8A%E5%B7%A5%E4%BF%A1%E9%83%A8)、[工信部公示小米新SU7Ultra](https://s.weibo.com/weibo?q=%E5%B7%A5%E4%BF%A1%E9%83%A8%E5%85%AC%E7%A4%BA%E5%B0%8F%E7%B1%B3%E6%96%B0SU7Ultra) 指向工信部道路机动车辆生产企业及产品公告类信息，未见本期打开的公告 PDF，不写具体参数。[金价扛不住了](https://s.weibo.com/weibo?q=%23%E9%87%91%E4%BB%B7%E6%89%9B%E4%B8%8D%E4%BD%8F%E4%BA%86%23)、[黄金史上暴跌最快半年恢复](https://s.weibo.com/weibo?q=%E9%BB%84%E9%87%91%E5%8F%B2%E4%B8%8A%E6%9A%B4%E8%B7%8C%E6%9C%80%E5%BF%AB%E5%8D%8A%E5%B9%B4%E6%81%A2%E5%A4%8D)、[炒股亏钱最对不起的是家人](https://s.weibo.com/weibo?q=%E7%82%92%E8%82%A1%E4%BA%8F%E9%92%B1%E6%9C%80%E5%AF%B9%E4%B8%8D%E8%B5%B7%E7%9A%84%E6%98%AF%E5%AE%B6%E4%BA%BA) 与昨日 A 股深跌、金价波动情绪共振，但热搜标题不是行情源。[华为自研HBM内存方案](https://s.weibo.com/weibo?q=%E5%8D%8E%E4%B8%BA%E8%87%AA%E7%A0%94HBM%E5%86%85%E5%AD%98%E6%96%B9%E6%A1%88) 仅见话题名，未见可核对的华为官方说明，不当成产品已量产。[美军本土引爆5吨含铅剧毒起爆药](https://s.weibo.com/weibo?q=%E7%BE%8E%E5%86%9B%E6%9C%AC%E5%9C%9F%E5%BC%95%E7%88%865%E5%90%A8%E5%90%AB%E9%93%85%E5%89%A7%E6%AF%92%E8%B5%B7%E7%88%86%E8%8D%AF) 对应艾奥瓦州叠氮化铅可控引爆的中文传播。[蔡磊已进渐冻症终末期](https://s.weibo.com/weibo?q=%23%E8%94%A1%E7%A3%8A%E5%B7%B2%E8%BF%9B%E6%B8%90%E5%86%BB%E7%97%87%E7%BB%88%E6%9C%AB%E6%9C%9F%23) 为社会个案话题，本期未打开其本人或家属完整声明，不写病程细节。

**速览。** 其余靠前条目多为综艺、剧集与娱乐，如小城良方、许飞与厉娜、玄彬郑丽媛青龙奖、你好星期六、朝玉阶、成毅两京十五日、白小纯与青稚、肖战、刘亦菲换手机、变形计吴欣媛等，以及谷爱凌伤情、最帅保洁大叔辞职、中国男篮名单、热火 vs 76 人等体育话题，不展开。

## 7. 油管科技访谈

对照 docs/youtube-sources.md 的频道名单，从各频道 /videos 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。多数频道近一周的节目已在前几期写过；今天新增长访谈主要来自 Latent Space 与 The Pragmatic Engineer。

**[The Revolution vs The Renaissance — Thariq Shihipar, OpenAI](https://www.youtube.com/watch?v=Qe9d9dWyED0)**  
Latent Space · 54:00 · 发布于 2026-11-26 06:11:27 Asia/Shanghai（UTC+8）。官方简介写，这是 AI Engineer CODE 上的访谈：Thariq Shihipar 回顾自己对 coding agents 判断失误之处，讨论人仍在创造性回路里时 AI 能打开什么可能，演示用 /human 文件夹调试格斗游戏攻击，并谈到决策模型与算力实验如何被挑选；简介还写访谈后他宣布加入 OpenAI。章节包括 agents 惊喜、/human folder、software as craft、game balance、decision models、autoresearch 等。以上均来自节目简介与章节，不编造片中原话。

**[How Anthropic builds software in 2026 with Katelyn Lesse](https://www.youtube.com/watch?v=9oNvKMd7xJo)**  
The Pragmatic Engineer · 1:50:45 · 发布于 2026-11-26 01:26:20 Asia/Shanghai（UTC+8）。官方简介称嘉宾为 Anthropic 平台工程负责人 Katelyn Lesse（此前在 Stripe 带工程团队），团队负责 Claude API 以及 Claude Code、Claude Desktop 背后的基础设施；节目讨论如何把服务所有 Claude token 的 API 从 Python 重写到 Rust、影子流量验证、用 Claude 做入职、Managed Agents、人工 code review、oncall、产品经理直接上线，以及 software factory 与传统编码面试淡出等。这些议题来自简介与时间戳，不是对 Anthropic 内部文件的独立审计。

Dwarkesh、YC、All-In、a16z、Lenny、No Priors 等频道近几日长访谈多已在前几期写过，本期不再重复。Acquired 近月仍无符合「新访谈」筛选的新集。

## 8. 本月阅读与今日书摘

今天是星期四。按 [本月阅读计划](/reading/)，工作日若有预先写好的分期书摘，应写入早报；若当天没有安排章节，则只保留书单和进度，不硬塞新的摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。计划写明下一本是《人件》，但仓库里的分期文稿尚未写入《人件》各工作日的书摘，故本期不编造章节摘要，只保留书单与进度指引。具体安排见仓库 [docs/reading-plan-2026-11.md](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

星期四早上回看，昨天那条发射倒计时已经变成结果：神舟二十四号 08:18 升空，下午完成「太空握手」，热搜上的进驻话题终于有官方时间点可对。市场另一头却很沉——A 股用周三收盘价计入本期，上证与深成指分别跌逾 2% 与 3%；美股那边，BBC 写的是 AI 投资疑虑加上新关税，把黄仁勋复职的反弹又压了回去。实验室数学线继续喧闹：OpenAI 的 ω=9/4 与 Google Cogentic 的因子分解目录同日占据 HN，Aaronson 用一篇「Holy shit」承认奇点感，又把密码学重磅按在「未核实」栏里。1Password 则提醒：账户元数据泄露不等于保险库失守，但钓鱼会接踵而至。北京市区今早约 2℃，白天多云回暖；海淀是东部片区街镇座谈，昌平继续围着生命科学园与美丽健康产业写稿。阅读上，《人件》分期仍未进仓库，今天继续只留书单。若只从新访谈里留一句，Thariq 那期更值得记住的，或许是他把 /human 文件夹留在回路里的姿态：工具可以更快，判断仍要有人签字。
