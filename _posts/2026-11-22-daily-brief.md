---
layout: post
title: "早报 · 2026-11-22"
date: 2026-11-22 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-22 07:45:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/22/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 22 日（星期日）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:32 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:32，昌平原文页约在 07:35，海淀区一则通知公告原文约在 07:38；X 热榜约在 07:32，科技圈检索约在其后不久；油管频道页约在 07:32，节目页约在 07:35。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 `feeds.reuters.com` 再次出现连接失败，美联社 RSSHub 返回 403，《纽约时报》正文页返回 403，Science.org 与 Mozilla 博客在直接请求时返回 403（后经可访问的页面文本读到），均已在相应栏目说明。今天是周末：A 股与人民币中间价均无新的交易日或发布日，本期采用 11 月 20 日（星期五）已公布的官方读数。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期日，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 `docs/brief-memory/finance-history.json`。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,539.00 美元/盎司 | 较上一期早报（2026-11-21 07:32:36 Asia/Shanghai (UTC+8)）0.00（0.00%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 `3539.0`，报价单位为美元/盎司；`updatedAt` 为 `2026-11-21T23:31:38Z`。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,539.00）计算，故与上一期早报持平 | 2026-11-22 07:31:38 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7131（11 月 20 日） | 较上一发布日（2026-11-19，6.7128）变动 +0.0003 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-22 07:32:00 返回的最新一条是 11 月 20 日的 6.7131；更早记录为 11 月 19 日 6.7128、11 月 18 日 6.7118、11 月 17 日 6.7132、11 月 16 日 6.7141。**本期采用 11 月 20 日已公布中间价**（今天是星期日，无新的发布日）。变化栏按官方上一发布日口径 | 采集 2026-11-22 07:32:00 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.69198 | 较上一期早报（2026-11-20 08:02:32 Asia/Shanghai (UTC+8)）0.000000（0.00%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。`time_last_update_utc` 仍为 Fri, 20 Nov 2026 00:02:32 +0000（合 2026-11-20 08:02:32 Asia/Shanghai），与上一期早报为同一笔日更读数；`time_next_update_utc` 显示为 Sat, 21 Nov 2026 01:07:42 +0000（约合 09:07:42 Asia/Shanghai），该预定时间在采集时已经过去，但 `time_last_update` 尚未刷新 | 2026-11-20 08:02:32 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3533.79 | −43.83（−1.23%） | [东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 返回：最新价 3533.79，涨跌 −43.83，涨跌幅 −1.23%，昨收 3577.62，开盘 3527.30，最高 3538.27，最低 3500.83。[腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 交叉核对数字一致，腾讯行情时间戳 `20261120161427`（2026-11-20 16:14:27）。今天是星期日，**本期采用 11 月 20 日（星期五）收盘价，不是今日盘中或开盘价** | 采集 2026-11-22 07:32:00 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10256.39 | −326.81（−3.09%） | 同上来源：最新价 10256.39，涨跌 −326.81，涨跌幅 −3.09%，昨收 10583.20，开盘 10402.29，最高 10436.04，最低 10256.39。腾讯行情时间戳 `20261120161412`（2026-11-20 16:14:12） | 采集 2026-11-22 07:32:00 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报持平，仍为 3,539.00 美元/盎司。市场化参考汇率仍是 11 月 20 日那一笔日更，读数未变。官方中间价本期继续采用 11 月 20 日已公布的 6.7131，较 19 日中间价上调 0.0003；A 股本期采用 11 月 20 日收盘价，上证下跌 1.23%，深成指下跌 3.09%。今天不是交易日，这些官方数字都不是今日开盘或收盘。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [`/api/weather/view?stationid=54511`](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 `lastUpdate` 为 2026/11/22 07:20；本次采集时间为 2026-11-22 07:31:59 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。接口还将今日标注为节气「小雪」。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。接口本次返回的预警列表为空。

**当前实况**（`lastUpdate` 2026/11/22 07:20）：气温 −2.0℃，体感温度 −5.3℃，相对湿度 58%，西南风微风，风速 1.7 米/秒，降水量 0.0，气压 1023.0 百帕。

**今日（11 月 22 日）预报**：白天多云，最高 7℃，南风微风；夜间多云，最低 −1℃，北风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 23 日 | 白天晴，夜间晴 | 8℃ / −3℃ | 白天西北风 3～4 级，夜间西北风微风 |
| 11 月 24 日 | 白天晴，夜间晴 | 7℃ / −3℃ | 白天西南风微风，夜间西南风微风 |
| 11 月 25 日 | 白天晴，夜间晴 | 9℃ / −2℃ | 白天南风微风，夜间东北风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 `docs/brief-memory/seen.json`。昨日及此前已写过的海淀区人大代表视察、医保钱包 2.0、未名·AI Park、与中国航油签约、违法建设治理公示，以及昌平的南口山林救援、供热巡查、政协总结大会、北七家物业焕新等，不再重复。今天是星期日：海淀区要闻、政务动态和街镇动态列表较昨日没有新的近日稿件，来源较薄，故只写一条近日通知公告，不把十月以前的旧稿凑进目录。

#### 海淀区

**[电信网络诈骗案件冻结资金返还公示](https://zyk.bjhd.gov.cn/zwdt/xxgk/tzgg/202611/t20261119_4835844.shtml)**。来源：北京市公安局海淀分局，发布于 2026-11-19 15:22。公示编号为「2026年28号」。稿件称，2023 年 5 月海淀分局辖区内发生 1 起电信网络诈骗案件，办案民警通过资金溯源冻结涉案账号，挽回部分被骗资金。现依《电信网络新型违法犯罪案件冻结资金返还若干规定实施细则》办理返还，并将农业银行账户（户名：陶雪，账号在公示中完整写出）内人民币 13,657.47 元，返还至事主万某某名下工商银行账户。公示要求，如有异议，自公示日起三十日内与海淀分局刑侦支队反诈中心联系。这是一份办案公示，不是新的案情通报。

#### 昌平区

**[区领导带队到南口镇检查古树保护与利用、森林防火等工作](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111917591779012/index.html)**。来源：北京昌平 APP，发布于 2026-11-19 18:14。11 月 19 日，区委副书记、区长刘晓东到南口镇檀峪村古青檀公园，听取全区古树资源与保护情况，并查看古树生长状况。报道称，该公园以「北京现存最古老的一级古青檀」为核心。他随后到檀峪村管护站检查进山卡口值守，并听取森林防火基础设施、防火责任和美国白蛾防控情况。此前一期早报已写过 11 月中旬的森林防火检查，这是 19 日一次更具体的南口现场检查，重点也扩大到古树保护与「古树+文旅」，不重复此前那一次的行程。

**[绷紧安全弦 守好平安线 小汤山镇持续筑牢冬季安全「防火墙」](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111919191932316/index.html)**。来源：北京昌平 APP，发布于 2026-11-19。报道写，小汤山镇在酸枣岭村和市场街社区检查沿街「九小场所」、出租房屋和商户的用火用电、消防设施，并在各村、社区入户核验一氧化碳和烟感报警器，强调严禁使用煤炉、炭火、柴炉取暖，同时签订预防煤气中毒责任书。重点场所清查还涉及经营性自建房、温室大棚、废品回收点、电动车棚和楼道等。

**[实训强本领、防患于未「燃」，回龙观街道消防宣传月多点位开展实战化应急演练](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112011123393267/index.html)**。来源：北京昌平 APP，发布于 2026-11-20。稿件称，全国消防宣传月期间，回龙观街道在商业综合体、商务楼宇、医疗和养老机构组织实战演练，面向 700 余名商户员工、企业职员和医护人员等，开展逃生疏散和灭火器材实操。点位包括金域国际中心、昌发展万科广场、北京天空之城、泰华龙旗广场，以及首都医科大学附属北京回龙观医院、首开寸草养老院。这些人数和场所名称来自报道本身。

**[深耕山区群众健康管理 织密慢阻肺防治服务网](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112018301593082/index.html)**。来源：北京昌平 APP，发布于 2026-11-20。第 25 个世界慢阻肺病日前后，流村镇组织流村社区卫生服务中心及下属站点，以「早诊断早管理，共创美好生活」为主题开展宣传，并称要把高危人群筛查、肺功能评估、家庭医生签约和长期随访连成闭环，纠正「慢性咳喘是衰老正常表现」等认知。这是基层公共卫生服务报道，不是对某一诊疗结果的统计公报。

**[新生违建「不过夜」 东小口镇快速处置违建](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111717041352752/index.html)**。来源：北京昌平 APP，发布于 2026-11-17。稿件称，11 月 12 日东小口镇接到违建举报，确认后依据《北京市禁止违法建设若干规定》向当事人送达《责令改正通知书》，并开展劝导；当事人于 11 月 16 日自行拆除。报道把它写成「发现、核查、处置」的一次闭环，不涉及更大范围的拆除清单。

## 3. 全球头条

路透社世界新闻 RSS 本次连接失败，美联社经由 RSSHub 的源返回 403，这两家不写入正文。《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写，不假装读过全文。

**续报：克里米亚大桥与泽连斯基对英表态。** [BBC](https://www.bbc.co.uk/news/articles/c6wy0qj7w5zqo) 11 月 21 日发自基辅的报道写，乌克兰总统泽连斯基在会见英国卫生大臣 Wes Streeting 时，把对连接俄罗斯与被占克里米亚的大桥的多次袭击称为「fair response」，理由是俄罗斯对乌克兰桥梁发动了 109 次袭击。他对 BBC 说，桥被袭后俄方对乌克兰的猛烈打击，只是「普京不想停下来」的信号。Streeting 表示此行是为了表明欧洲对乌克兰的支持。克里米亚大桥遇袭一事，前几期早报已经写过，这里只补他与英方会谈时的新表态。同日 BBC 另有报道：[Zelensky says Putin is a 'killer' after Trump calls Russian leader a friend](https://www.bbc.co.uk/news/articles/cxnv4zvmdy0jo)，把这句表态放在特朗普于深圳会晤后称与普京关系很好的背景里，亦不展开已写过的峰会本身。

**[Russia-bound ship attacked in Gulf of Finland](https://www.bbc.co.uk/news/articles/cj752ddve27ko)**（BBC，2026-11-21 18:22 GMT，合 2026-11-22 02:22 Asia/Shanghai）。报道称，一艘驶往俄罗斯波罗的海飞地加里宁格勒的货船 Sparta II 在芬兰湾东部遭无人机袭击，随后起火并漂入芬兰水域。芬兰国防军表示，袭击很可能来自乌克兰；基辅方面尚未置评。芬兰总理 Petteri Orpo 说：「战争正在溢到我们的邻近海域。」加里宁格勒州长称初步信息是两架无人机，并表示对当地补给「没有威胁」。报道还写，该船曾被美国和乌克兰列入制裁名单。芬兰军方的判断是当事方说法，乌克兰是否实施袭击，仍有待其官方说明。

**[Fight over fossil fuels leaves COP31 climate talks in deadlock](https://www.bbc.co.uk/news/articles/c6ly5w40eg07o)**（BBC，发自土耳其安塔利亚，2026-11-21）。报道写，COP31 谈判已超时一天以上，因无法就新的全球气候协议达成一致而陷入僵局，并曾暂停至夜间。欧盟与太平洋岛国等反对最新草案完全不提减少化石燃料需求；另一争议是非洲集团要求增加适应资金，而欧盟先前表示不会支持。原定周日上午离开的谈判团队已把航班改到周一。若无法达成联合国气候进程所需的共识，会议可能在没有协议的情况下暂停、留到明年再开。BBC 称，这种情况自 COP 机制启动以来只出现过一次。《卫报》同日另有一篇署名 Fiona Harvey 的[独家报道](https://www.theguardian.com/environment/2026/nov/21/china-commits-low-carbon-electrification-help-others-improve)：中国代表团高级顾问、中科院能源与环境政策教授王毅表示，终端电气化方向明确，应在用电端电气化的同时让电力来源更清洁；稿件并称，各国在 COP31 被推动承诺到 2035 年将能源中电力占比提高到 35%。这是《卫报》对中方顾问表态和会议倡议的转述，不是已经通过的决议。

**[Mexican drug lord on FBI's 10 most wanted list arrested in shoot-out](https://www.bbc.co.uk/news/articles/ckz749ey0r75o)**（BBC；《卫报》[同行报道](https://www.theguardian.com/world/2026/nov/21/alleged-mexican-drug-cartel-boss-el-chapo-isidro-meza-flores-arrested)）。墨西哥国防部称，当地时间周五，特种部队在锡那罗亚州瓜萨韦拘捕了 Fausto Isidro “Chapo Isidro” Meza Flores 及其他七人。BBC 写，行动中有七名嫌疑人死亡，另有四名前往增援的墨西哥士兵死亡。FBI 曾将其列入十大通缉犯，并指其向美国输送芬太尼、可卡因和海洛因等毒品；美国寻求引渡。NYT World RSS 也有抓捕与人物介绍，但正文页本次 403，不另转写细节。

**[FBI reportedly investigating apparent hack of its criminal database](https://www.bbc.co.uk/news/articles/cvze7de86pk3o)**（BBC，2026-11-21）。报道引述美国媒体、称两名知情人士透露：FBI 正在调查其国家犯罪信息中心（NCIC）数据库是否遭到入侵。该库供联邦和地方执法共享通缉与背景调查信息。FBI 未立即回应 BBC 问询。特朗普当天接受 Fox News 采访时说，他「刚刚听说」，「这不好」，又说「也许我们会了解到原本不会知道的事情」。报道提醒，此事发生在美国上周一系列技术故障之后；官方曾表示那些故障并非网络攻击。在更多独立确认之前，这仍是「据报正在调查」的事件，不是已经定性的攻击结论。

**[Man convicted of starting Palisades fire in Los Angeles](https://www.bbc.co.uk/news/articles/c64gn0gy8rj3o)**（BBC，2026-11-21）。报道称，一名 30 岁的洛杉矶居民被裁定纵火罪成立，这起山火导致 12 人死亡，烧毁 6,800 多栋建筑。RSS 摘要与标题一致；具体庭审细节以原文为准。

**[Mamdani announces plan to close New York's Rikers Island jail by 2032](https://www.bbc.co.uk/news/articles/cmjeqv89egylo)**（BBC，2026-11-21 00:01 GMT，合 08:01 Asia/Shanghai）。报道写，纽约计划关闭争议已久的 Rikers Island 监狱，目标年份是 2032 年；关闭动议可追溯到 2019 年市议会投票，此后因安置问题多次推迟。

BBC 中文近日较多是对已写过的深圳峰会、Anthropic 上市的回顾，以及 11 月 28 日台湾「九合一」地方选举的[选前情势梳理](https://www.bbc.com/zhongwen/articles/cmp3vyl0x1x6o/simp)。峰会与上市不重复展开；台湾选举尚未投票，这里只记下投票日将近。NYT World RSS 还可看到：凯特王妃以 BBC 纪录片回顾癌症治疗、五角大楼限制与加拿大军方「社交活动」的备忘录、联合国未能就致命自主武器达成约束等，因正文 403，本期不深写。

## 4. Hacker News 近期文章

首页来自 [Algolia 前端接口](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集于 2026-11-22 07:31:59 Asia/Shanghai（UTC+8）。对讨论最多或点数最高的若干新条目打开了原文；昨日已写过的 Masullo GRH 草稿、Inkling 2 Mini 介绍，以及 “We promoted developers into architects without informing them”，只在需要时作一行对照，不重写。

**续报：[Lean verification of the Riemann Hypothesis](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/)**（[HN 讨论](https://news.ycombinator.com/item?id=50589618)，744 点，594 则评论）。Lean 与 Mathlib 社区 2026-11-21 13:55 UTC（合 21:55 Asia/Shanghai）发表联合声明，并写明得到 Lean FRO 与 Mathlib Initiative 背书。声明说，Levent Alpöge 于 11 月 20 日发布了一份约 1,700 万行的 Lean 库，宣称证明黎曼猜想；社区「对 Alpöge 的证明正确有充分信心」，并「在此证明该命题与证明均为正确」。其依据包括：命题本身已在 Mathlib 的 `RiemannHypothesis` 中、由 Lean 与数论专家审看；已有数十人复现同一导出文件且能编译通过；社区用 `comparator` 与 `con-leche --compare` 核对所证命题正是 Mathlib 中的陈述；导出证明还经过 Lean 官方内核以及 `con-leche`、`con-ron` 等独立检查器。声明把这四条与 Kevin Buzzard 此前关于「Lean 证明如何算被检查」的[标准](https://xenaproject.wordpress.com/2026/11/12/and-the-proof-is-checked-in-lean/)相对应，并指向 Andrew Sutherland（MIT）整理的[验证文件页](https://math.mit.edu/~drew/grh/)（页面写明最后更新 2026-11-21 12:55 UTC，合 20:55 Asia/Shanghai；其中部分检查仍在进行）。这是形式化验证社区的公开背书，不是数学刊物的最终发表，也不自动结束对证明思路的消化，以及对 Masullo 那份「全由人完成」草稿的并行讨论。相关 HN 条目 [Verification files for the Lean proof of the Riemann Hypothesis](https://math.mit.edu/~drew/grh/)（[讨论](https://news.ycombinator.com/item?id=50590441)，83 点，28 则评论）只作为同一续报的出处，不另起一篇。

**[Brazil's tax authority open-sources its tax calculator on GitHub under MIT](https://www.gov.br/receitafederal/pt-br/assuntos/noticias/2026/novembro/receita-federal-publica-primeiro-codigo-fonte-aberto-no-github-e-amplia-transparencia-da-reforma-tributaria)**（[HN](https://news.ycombinator.com/item?id=50532613)，687 点，222 则评论）。巴西联邦税务局 2026-11-16 的公告称，已按 11 月 12 日 Cotec 第 342 号条例，把消费税制改革中的税金计算器源码以 MIT 许可放到 GitHub 公共仓库。稿件说，这是该局首次在公共协作环境正式发布软件，目的是让企业与软件商使用与税务当局相同的 CBS 等新税计算逻辑。发布时间早于今日，但本日仍在 HN 首页高位。

**[Ask HN: I have been unemployed for 2y. 15 years of experience, US. What to do?](https://news.ycombinator.com/item?id=50583761)**（585 点，643 则评论）。这是一条没有站外原文的讨论帖：提问者称自己有 15 年经验、在美国失业两年。评论区热度很高，内容是求职经验交换，不是一则可核实的新闻事件，这里只记下讨论本身。

**[Detonating a pile of lead azide](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really)**（[HN](https://news.ycombinator.com/item?id=50588982)，484 点，315 则评论）。Derek Lowe 2026-11-20 在 Science 的 Pipeline 博客中，用问答形式解释美国陆军计划在爱荷华州伯灵顿附近引爆库存叠氮化铅的背景。文章写，这是一种比 PETN 更敏感的「始发炸药」，常用于炮弹起爆；该设施地下库中约 68 桶、重约 9,500 至 10,000 磅的物料已存放约 20 年，因部分溶解后再结晶而变得更敏感。原定「今天」实施的爆破至少推迟到周一，并面临法律行动。这些数量、地点和推迟，都是作者对已报道计划的转述。该页直接抓取返回 403，正文经可访问的页面文本读到。

**[Why there are still no non-WebKit browsers on iOS](https://blog.mozilla.org/en/mozilla/internet-policy/apple-ios-browser-engine-rules/)**（[HN](https://news.ycombinator.com/item?id=50575644)，458 点，251 则评论）。Mozilla 2026-11-20 的政策文章写，尽管欧盟 DMA 和日本的类似规则要求 iOS 允许替代浏览器引擎，但「近三年里，还没有一家开发者能在 iOS 上推出非 WebKit 浏览器」。文章认为苹果的条件「难以实际操作」，举例称若要使用 Gecko，不能直接更新现有 Firefox，而必须做一个独立的第二款应用，再让用户迁移书签与密码。这是 Mozilla 的立场陈述。该页直接抓取同样 403，正文经可访问的页面文本读到。

**[My monitor was cutting my download speed by 75%](https://blog.tymscar.com/posts/studiodisplayethernet/)**（[HN](https://news.ycombinator.com/item?id=50587875)，437 点，216 则评论）。Oscar Molnar 写自己有 2.5 Gbps 对称带宽，却在 Studio Display XDR 的「一根线」方案下只测到约 600 Mbps 下载、上传仍约 2.4 Gbps。排查后，他把问题定位到经显示器转发的 USB-C 到 2.5G 以太网路径。这是一篇个人排障记录，不是对某款显示器的普遍测试结论。

**[Pill to treat pancreatic cancer hailed as 'biggest breakthrough in decades'](https://www.theguardian.com/society/2026/nov/20/pill-pancreatic-cancer-breakthrough-daraxonrasib)**（[HN](https://news.ycombinator.com/item?id=50582069)，419 点，116 则评论）。《卫报》2026-11-20 报道，试验药物 daraxonrasib 在 61 名新近确诊、癌症已扩散的胰腺癌患者中，约十二分之一的人癌症变得检测不到，几乎所有人的肿瘤停止生长；用药一年后 76.6% 的患者仍在世，而仅化疗通常约为 40%–45%。报道同时写明，医生认为它还不能被称为治愈，也不知道药效能维持多久。这些比例来自该报道对试验的转述。

**[RCE in Gnupg](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html)**（[HN](https://news.ycombinator.com/item?id=50587208)，221 点，89 则评论）。Werner Koch 在 2026-11-20 19:01:51 CET（合 2026-11-21 02:01:51 Asia/Shanghai）宣布 GPGME 2.3.1，修复所有先前版本中的严重缺陷（内部编号 T8557，CVE-2026-129975）。公告称，一枚带有特制超长 user id 的 OpenPGP 密钥可触发 double-free，或被用来从应用中带出数据；远程代码执行「不能被排除」，因此建议立即更新。漏洞由 Johan Carlsson 发现，经 GitLab 于 11 月 12 日告知。

**[LLMs can read and write executables byte by byte from a hex dump](https://sgiannopoulos.github.io/blog/machine-code-programming/)**（[HN](https://news.ycombinator.com/item?id=50546587)，170 点，117 则评论）。George Xenos 与 Sotiris Giannopoulos 的博文称，在没有反汇编器或编译器、只给十六进制转储的情况下，GPT-6.1 Sol（这是作者使用的模型名称）能够逐字节阅读和改写可执行文件，并在他们给出的样本里解释二进制、分析恶意软件、甚至直接改字节来加功能。文中还提到 DeepSeek V4.1 Flash 对恶意软件样本得出了相同判断。这些都是作者对自己实验的描述，不是第三方复现报告。

其余首页条目（短列表）：

- [I'm quite pleased by the tech architecture of my art website](https://klauria.tech/klauria-art/)（[HN](https://news.ycombinator.com/item?id=50577991)，133 点，31 则评论）：Kshitij Lauria 写自己把画作放到带地图标记的网站上，并分享架构取舍。
- [Show HN: Zero C# – C# without a runtime or GC](https://onurgumus.github.io/zero-csharp/index.html)（[HN](https://news.ycombinator.com/item?id=50590279)，116 点，92 则评论）：项目称基于 bflat 分支，把 C# 编成不带 .NET 运行时和垃圾回收的原生程序，内存用 arena，并可在 Linux、macOS、Windows、WebAssembly 以及 386 上的 DOS 运行。
- [PostgreSQL Extensions in Go](https://jespino.github.io/gopgext/)（[HN](https://news.ycombinator.com/item?id=50591260)，107 点，17 则评论）：gopgext 用 TinyGo 把 Go 函数标成 PostgreSQL 扩展；作者标明项目仍是实验性的。
- [Inkling-2-Mini in 5.4 GB Memory](https://github.com/ShinMegamiBoson/lookatmyquant)（[HN](https://news.ycombinator.com/item?id=50591853)，310 点，80 则评论）：仓库与页面主体介绍的是量化编译器 LookAtMyQuant；与昨日已写的 Inkling 2 Mini 官方介绍不是同一篇文章，这里不把标题里的「5.4 GB」自动写成官方运行需求。
- [Getting the mind to steer the body to steer you](https://notnottalmud.substack.com/p/getting-the-mind-to-steer-the-body)（[HN](https://news.ycombinator.com/item?id=50583028)，104 点，41 则评论）
- [Exponential Behavior in Magic: The Gathering](https://levineuwirth.org/essays/exponential-magic/)（[HN](https://news.ycombinator.com/item?id=50546495)，84 点，59 则评论）
- [Upload2Shell (CVE-2026-125396)](https://pwn.ai/upload2shell)（[HN](https://news.ycombinator.com/item?id=50592097)，60 点，20 则评论）
- [Show HN: An ASCII cell aquarium for your terminal](https://github.com/kborer/cells/)（[HN](https://news.ycombinator.com/item?id=50541047)，47 点，16 则评论）
- [Tropical Rainforests Species may be surprisingly young](https://phys.org/news/2026-11-species-tropical-rainforests-young-emergence.html)（[HN](https://news.ycombinator.com/item?id=50532417)，34 点，14 则评论）
- [Advice for the next 100 Rust GUIs](https://linebender.org/blog/next-100-guis/)（[HN](https://news.ycombinator.com/item?id=50593737)，26 点，1 则评论）
- [Windows has two settings that bring work back after restart, both off by default](https://www.makeuseof.com/windows-can-bring-your-work-back-after-restart/)（[HN](https://news.ycombinator.com/item?id=50560203)，22 点，11 则评论）
- [PcapAnalyzer – self-hosted pcap analyzer with 27 problem detectors](https://github.com/sebaandrada-cell/PcapAnalyzer)（[HN](https://news.ycombinator.com/item?id=50594132)，22 点，2 则评论）
- [Bolt's Scooters Are Becoming Accessibility Sensors](https://geoawesome.com/bolt-scooters-accessibility-mapping-wheels4wheels/)（[HN](https://news.ycombinator.com/item?id=50533517)，18 点，22 则评论）
- [The Emergence of Inequality in the Czech Corded Ware Culture](https://www.jna.uni-kiel.de/index.php/jna/article/view/1560/1746)（[HN](https://news.ycombinator.com/item?id=50593637)，13 点，9 则评论）
- [Context-Generic Programming v0.8.0 – Pluggable trait implementations for Rust](https://contextgeneric.dev/blog/v0.8.0-release/)（[HN](https://news.ycombinator.com/item?id=50548136)，12 点，0 则评论）
- [Pandex – Official European Law for AI Agents, over MCP](https://www.pandex.io)（[HN](https://news.ycombinator.com/item?id=50593481)，11 点，1 则评论）
- [Tasklet (YC P26) Is Hiring Product and Agent Infra Engineers](https://tasklet.ai/careers)（[HN](https://news.ycombinator.com/item?id=50593679)）：招聘帖，不展开。

## 5. X 热门与科技圈

X 热榜采集于 2026-11-22 07:32:13 Asia/Shanghai（UTC+8），使用公共趋势接口：全球 WOEID 1、美国 23424977。以中国 WOEID 23424781 查询时，返回结果与全球热榜高度重合，不把它当成一份独立的「中国本地热榜」。

全球和美国热榜几乎被周末赛事占满。全球靠前的是 Flamengo、Merentiel、Mineiro、Vini、Real Madrid、Mbappe 等足球相关词，以及 [Ohio State](https://x.com/search?q=Ohio%20State)、[Michigan](https://x.com/search?q=Michigan)、[Nebraska](https://x.com/search?q=Nebraska)、[Ryan Day](https://x.com/search?q=Ryan%20Day) 等美国大学橄榄球词条，另有 [#UFCQatar](https://x.com/search?q=%23UFCQatar)。美国热榜同样以大学橄榄球和 UFC 为主。本期未逐一核对赛果，不把热词写成比分公报。

科技和 AI 圈的讨论，并不在上述热榜前排，而更多是对周五已发生事件的周末余波。X 的新闻摘要和近期帖文仍然集中在三件事：Lean 社区对 Alpöge 证明的核验、英伟达与 Anthropic 股价在上周的大跌，以及 Inkling 2 Mini 等可以在笔记本电脑上运行的开源权重模型。其中形式化证明的进展，以上面 Hacker News 栏目的社区声明为准，不把社交平台上的「已经证明」当成最终数学结论。关于英伟达管理层和「间谍」传闻，前几期已标明是流传中的说法，周末热帖里仍有人在讨论，本期不把传闻升格为已核实事实。也有摘要提到 François Chollet 回顾两年来基准测试的变化、以及批评者在电视节目上谈论 AI 融资循环，这些都是平台上的讨论线索，具体数字仍以当事人原文或正式财务披露为准。

## 6. 微博热搜

接口 `https://weibo.com/ajax/side/hotSearch` 在 2026-11-22 07:32:00 Asia/Shanghai（UTC+8）返回成功（`ok=1`）。置顶/政务条目为 [#和合共生#](https://s.weibo.com/weibo?q=%23%E5%92%8C%E5%90%88%E5%85%B1%E7%94%9F%23)，带「热」标，未见更多正文，这里只记下它是置顶政务话题。本次实时榜前 50 条未见明确的广告标。

**科技、国际与社会。** [#图览APEC中国年75项主要成果#](https://s.weibo.com/weibo?q=%23%E5%9B%BE%E8%A7%88APEC%E4%B8%AD%E5%9B%BD%E5%B9%B475%E9%A1%B9%E4%B8%BB%E8%A6%81%E6%88%90%E6%9E%9C%23)、[#特朗普说媒体报道不完深圳全景#](https://s.weibo.com/weibo?q=%23%E7%89%B9%E6%9C%97%E6%99%AE%E8%AF%B4%E5%AA%92%E4%BD%93%E6%8A%A5%E9%81%93%E4%B8%8D%E5%AE%8C%E6%B7%B1%E5%9C%B3%E5%85%A8%E6%99%AF%23) 是深圳峰会的余波，不重复已写过的联合声明。[#特朗普深圳不拉窗帘原因找到了#](https://s.weibo.com/weibo?q=%23%E7%89%B9%E6%9C%97%E6%99%AE%E6%B7%B1%E5%9C%B3%E4%B8%8D%E6%8B%89%E7%AA%97%E5%B8%98%E5%8E%9F%E5%9B%A0%E6%89%BE%E5%88%B0%E4%BA%86%23) 是围绕行程细节的热搜说法，未核实，只作为流传中的话题。[韩国涉嫌作弊满分考生遗书公开](https://s.weibo.com/weibo?q=%E9%9F%A9%E5%9B%BD%E6%B6%89%E5%AB%8C%E4%BD%9C%E5%BC%8A%E6%BB%A1%E5%88%86%E8%80%83%E7%94%9F%E9%81%97%E4%B9%A6%E5%85%AC%E5%BC%80) 与此前已写过的韩国高考 AI 作弊风波相关；热搜称有遗书被公开，具体文件真伪与内容，本期未打开权威报道核对。[2名在华日本人发生冲突1人死亡](https://s.weibo.com/weibo?q=2%E5%90%8D%E5%9C%A8%E5%8D%8E%E6%97%A5%E6%9C%AC%E4%BA%BA%E5%8F%91%E7%94%9F%E5%86%B2%E7%AA%811%E4%BA%BA%E6%AD%BB%E4%BA%A1) 说的不是北京本地新闻。据[共同社](https://china.kyodonews.net/articles/-/18645)、[联合早报](https://www.zaobao.com.sg/news/china/story20261121-10036866)等报道，2026 年 11 月 18 日凌晨，两名 50 多岁的日本男子在上海聚餐后发生纠纷，一人死亡，另一人被当地警方拘留；中国有关部门于 20 日向日本驻上海总领事馆通报，领事随后探视。起因和详细经过仍在调查，不以热搜标题代替警方结论。[张朝阳被北京证监局出具警示函](https://s.weibo.com/weibo?q=%E5%BC%A0%E6%9C%9D%E9%98%B3%E8%A2%AB%E5%8C%97%E4%BA%AC%E8%AF%81%E7%9B%91%E5%B1%80%E5%87%BA%E5%85%B7%E8%AD%A6%E7%A4%BA%E5%87%BD) 可与中国证监会网站「监管措施·北京」栏目在 2026-11-20 列出的[《关于对张朝阳采取出具警示函措施的决定》](https://www.csrc.gov.cn/csrc/c100045/common_list_gd.shtml)对照；热搜将这一名字与知名企业家联系起来，但公开讨论里已有人提醒同名问题，本期未打开决定书正文核对当事人身份，故不写成某一位公众人物。[本轮金价急跌类似历史3次](https://s.weibo.com/weibo?q=%E6%9C%AC%E8%BD%AE%E9%87%91%E4%BB%B7%E6%80%A5%E8%B7%8C%E7%B1%BB%E4%BC%B4%E5%8E%86%E5%8F%B23%E6%AC%A1)、[黄金抄底机会出现了吗](https://s.weibo.com/weibo?q=%E9%BB%84%E9%87%91%E6%8A%84%E5%BA%95%E6%9C%BA%E4%BC%9A%E5%87%BA%E7%8E%B0%E4%BA%86%E5%90%97)、[为什么全世界所有资产都在跌](https://s.weibo.com/weibo?q=%E4%B8%BA%E4%BB%80%E4%B9%88%E5%85%A8%E4%B8%96%E7%95%8C%E6%89%80%E6%9C%89%E8%B5%84%E4%BA%A7%E9%83%BD%E5%9C%A8%E8%B7%8C)、[但斌称一觉醒来血雨腥风](https://s.weibo.com/weibo?q=%E4%BD%86%E6%96%8C%E7%A7%B0%E4%B8%80%E8%A7%89%E9%86%92%E6%9D%A5%E8%A1%80%E9%9B%A8%E8%85%A5%E9%A3%8E) 是对上周五全球资产波动的讨论；黄金与 A 股的具体读数见金融栏，不把热搜标题里的比喻当成统计口径。[顺丰速运被暂停参加全军采购活动](https://s.weibo.com/weibo?q=%E9%A1%BA%E4%B8%B0%E9%80%9F%E8%BF%90%E8%A2%AB%E6%9A%82%E5%81%9C%E5%8F%82%E5%8A%A0%E5%85%A8%E5%86%9B%E9%87%87%E8%B4%AD%E6%B4%BB%E5%8A%A8) 出现在热搜，本期未核对官方通报全文，不展开细节。[小雪](https://s.weibo.com/weibo?q=%E5%B0%8F%E9%9B%AA) 与气象接口标注的节气相合，不是另一次天气事件。[央视揭秘网络女主播真实生态](https://s.weibo.com/weibo?q=%E5%A4%AE%E8%A7%86%E6%8F%AD%E7%A7%98%E7%BD%91%E7%BB%9C%E5%A5%B3%E4%B8%BB%E6%92%AD%E7%9C%9F%E5%AE%9E%E7%94%9F%E6%80%81)、[原来转账是可以拦截的](https://s.weibo.com/weibo?q=%E5%8E%9F%E6%9D%A5%E8%BD%AC%E8%B4%A6%E6%98%AF%E5%8F%AF%E4%BB%A5%E6%8B%A6%E6%88%AA%E7%9A%84)、[羽绒服生意变天了](https://s.weibo.com/weibo?q=%E7%BE%BD%E7%BB%92%E6%9C%8D%E7%94%9F%E6%84%8F%E5%8F%98%E5%A4%A9%E4%BA%86) 偏消费与社会话题，不深写。

**速览。** 其余靠前条目多为综艺、剧集和娱乐，如王子璇、余文乐、成毅《两京十五日》、田曦薇与张凌赫、周杰、白小纯粉丝群、张元英、帐中香、王菲与李嫣、陈伟霆、白鹿，以及阿尔卡拉斯晋级、王楚钦孙颖莎外卡争议、樊振东出战等体育话题，不展开。

## 7. 油管科技访谈

对照 `docs/youtube-sources.md` 的频道名单，从各频道 `/videos` 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。Lex Fridman、Dwarkesh Patel、Y Combinator、Lenny's Podcast、a16z、No Priors、Latent Space、The Pragmatic Engineer 等频道本周早些时候的节目，多数已在前几期写过；All-In 最新一期 *Anthropic Goes Public, Nvidia in Crisis, Markets Tank, Open Source Crackdown?* 昨日已作一行提示，不再展开。因此今日能新写的条数很少。

**[GTA 6, Crime, Money, Prison & the Biggest Jewel Thief in US History](https://www.youtube.com/watch?v=v1X9Fqs5a14)**  
Lex Fridman Podcast #505 · 3:21:14 · 发布于 2026-11-19 11:15:09 Asia/Shanghai（UTC+8）。官方简介称，嘉宾 Larry Lawton 是美国历史上最著名的珠宝盗窃者之一，后来被 FBI 抓住，在监狱中度过十多年（包括长时间单独关押），出狱后开办 Reality Check Program，帮助处在风险中的青少年远离监狱。章节目录包括：GTA 6、1980 年代迈阿密犯罪、电影 *Scarface*、单独监禁、第一次珠宝店抢劫、监狱经济与邮票、美国大规模监禁、狱中的精神病态者、纽约黑帮，以及入狱第一天和最危险的监狱帮派。这些是节目简介和章节里的议题，不是对某一案件的法庭转述，也不把游戏评测写成新闻。

## 8. 本月阅读与今日书摘

今天是星期日。按 [本月阅读计划](/reading/)，周末只保留书单和进度，不新写章节摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。下一本《人件》将按同样方式分期，具体安排见仓库 [`docs/reading-plan-2026-11.md`](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

周末把金融市场暂时「冻」在上一个交易日：黄金与上一期早报持平，人民币中间价和 A 股都还是周五那组官方数字，微博上却仍在讨论「资产都在跌」。真正往前走了一步的，是数学这一侧。昨天还只能写「Lean 证明仍待检验」，今天 Lean 与 Mathlib 社区已经发出联合声明，公开背书 Alpöge 的形式化证明通过了他们列出的检查。这仍不是一份数学期刊上的最终发表，也不等于所有思路都已被读懂，但它已经从「有人宣布」变成了「有一个共同体写下了核验理由」。与此同时，COP31 在化石燃料措辞上卡着，芬兰湾的一艘货船把战场边缘又向外推了一点。北京市区今早仍在零下，海淀要闻栏这个周末几乎没有新稿，昌平则是古树、防火、供暖和慢病这些更贴近入冬的事情。阅读上继续停在《人月神话》读完之后的周末：没有银弹，也不必在星期日硬塞新的章节。若只从今天的访谈里留一句，Lawton 那期更值得记住的不是游戏本身，而是一个人如何把坐过的牢，变成后来对别人的提醒。
