---
layout: post
title: "早报 · 2026-11-21"
date: 2026-11-21 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-21 07:50:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/21/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 21 日（星期六）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:33 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:33，原文页约在 07:39；X 热榜约在 07:34；油管频道页约在 07:37，节目页约在 07:39–07:40。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 `feeds.reuters.com` 再次出现连接失败，美联社 RSSHub 返回 403，东方财富行情接口返回 502，《纽约时报》正文页返回 403，部分博客在直接抓取时返回 403（后经可访问的页面文本读到），均已在相应栏目说明。今天是周末：A 股与人民币中间价均无新的交易日或发布日，本期采用 11 月 20 日（星期五）已公布的官方读数。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期六，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 `docs/brief-memory/finance-history.json`。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,539.00 美元/盎司 | 较上一期早报（2026-11-20 07:36:04 Asia/Shanghai (UTC+8)）−82.80（−2.29%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 `3539.0`，报价单位为美元/盎司；`updatedAt` 为 `2026-11-20T23:32:36Z`。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,621.80）计算 | 2026-11-21 07:32:36 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7131（11 月 20 日） | 较上一发布日（2026-11-19，6.7128）变动 +0.0003 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-21 07:32:53 返回的最新一条是 11 月 20 日的 6.7131；更早记录为 11 月 19 日 6.7128、11 月 18 日 6.7118、11 月 17 日 6.7132、11 月 16 日 6.7141。**本期采用 11 月 20 日已公布中间价**（今天是星期六，无新的发布日）。变化栏按官方上一发布日口径 | 采集 2026-11-21 07:32:53 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.69198 | 较上一期早报（2026-11-19 08:02:31 Asia/Shanghai (UTC+8)）+0.011202（+0.17%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。`time_last_update_utc` 为 Fri, 20 Nov 2026 00:02:32 +0000（合 2026-11-20 08:02:32 Asia/Shanghai），较上一期早报已再刷新一笔日更；`time_next_update_utc` 为 Sat, 21 Nov 2026 00:35:42 +0000（约合 08:35:42 Asia/Shanghai），采集时今日日更尚未刷新 | 2026-11-20 08:02:32 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3533.79 | −43.83（−1.23%） | [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 返回：最新价 3533.79，涨跌 −43.83，涨跌幅 −1.23%，昨收 3577.62，开盘 3527.30，最高 3538.27，最低 3500.83。行情时间戳 `20261120161427`（2026-11-20 16:14:27）。[东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 在 07:32:54 返回 502，本期未能交叉核对。今天是星期六，**本期采用 11 月 20 日（星期五）收盘价，不是今日盘中或开盘价** | 采集 2026-11-21 07:32:53 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10256.39 | −326.81（−3.09%） | 同上来源：最新价 10256.39，涨跌 −326.81，涨跌幅 −3.09%，昨收 10583.20，开盘 10402.29，最高 10436.04，最低 10256.39。腾讯行情时间戳 `20261120161412`（2026-11-20 16:14:12） | 采集 2026-11-21 07:32:53 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报继续回落，从 3,621.80 美元/盎司降至 3,539.00，跌幅约 2.29%，已是连续三期早报录得下跌。市场化参考汇率换成 11 月 20 日那一笔日更，兑人民币较上一期读数走弱约 0.17%。官方中间价本期采用 11 月 20 日已公布的 6.7131，较 19 日中间价上调 0.0003；A 股本期采用 11 月 20 日收盘价，上证下跌 1.23%，深成指下跌 3.09%。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [`/api/weather/view?stationid=54511`](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 `lastUpdate` 为 2026/11/21 07:20；本次采集时间为 2026-11-21 07:32:53 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。接口本次返回的预警列表为空。

**当前实况**（`lastUpdate` 2026/11/21 07:20）：气温 −3.3℃，体感温度 −6.7℃，相对湿度 65%，东北风微风，风速 1.7 米/秒，降水量 0.0，气压 1027.0 百帕。

**今日（11 月 21 日）预报**：白天晴，最高 7℃，北风微风；夜间晴，最低 −3℃，西南风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 22 日 | 白天多云，夜间多云 | 6℃ / −1℃ | 白天南风微风，夜间北风微风 |
| 11 月 23 日 | 白天晴，夜间晴 | 8℃ / −4℃ | 白天西北风 3～4 级，夜间西北风微风 |
| 11 月 24 日 | 白天晴，夜间晴 | 6℃ / −2℃ | 白天西南风微风，夜间西北风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 `docs/brief-memory/seen.json`。昨日及此前已写过的未名·AI Park 揭牌、与中国航油签约、违法建设治理公示，以及昌平的芯生视界生产基地启动、森林防火检查等，不再重复。

#### 海淀区

**[全国人大代表与北京市人大代表联合调研暨市人大海淀团代表会前视察活动举行](https://zyk.bjhd.gov.cn/ywdt/hdyw/202611/t20261120_4835957.shtml)**。来源：海淀报，发布于 2026-11-20 08:56。11 月 19 日，区人大常委会组织部分全国人大代表和北京市人大海淀团代表联合视察调研。稿件称，代表们先后前往故宫北院，了解整体规划、内部布局及周边园林工程建设；随后走进北京卫星小镇，考察园区规划、卫星产业和配套设施。座谈会由区委宣传部、实创股份通报文化强区建设和特色产业集群培育等情况。区委书记王少峰在会上谈到，海淀坚持科技和文化双轮驱动，以人工智能为牵引，高标准建设百年京张 AI 创新带。这些定位是报道中的官方表述。

**[职工医保个账，能给外地家人用了！医保钱包2.0版上线](https://zyk.bjhd.gov.cn/ywdt/bmdt/202611/t20261119_4835781.shtml)**。来源：海淀区医保局，发布于 2026-11-19 09:36。区医保局介绍，医保钱包是职工医保个人账户跨省共济的一种方式，可按规定支付近亲属在定点医药机构就医、购药发生的个人负担费用，也可用于参保缴费。操作可在国家医保服务平台 App、支付宝小程序或线下窗口完成；给没有手机的老人或孩子共济时，发起人输入对方姓名和身份证号即可绑定。稿件称，被共济人目前可在参保地定点医疗机构和定点零售药店使用 2.0 版共济额度，并提到今年年底前还将扩大使用范围。具体开通范围和结算规则以医保部门后续说明为准。

**[马连洼街道消防实训守护「一老一小」](https://zyk.bjhd.gov.cn/ywdt/jzdt/202611/t20261119_4835758.shtml)**。来源：马连洼街道（转自海淀报），发布于 2026-11-19 09:14。近日，马连洼街道在一处篮球场组织覆盖青少年、退休老干部、社区工作者和物业人员的沉浸式消防实训，包括 VR 火场逃生、油锅起火处置、灭火器操作，以及物业岗位的报警、疏散、扑救和善后流程演练。

#### 昌平区

**[寒林深处紧急救援！南口镇成功营救坠树伤者](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112011123820066/index.html)**。来源：北京昌平 APP，发布于 2026-11-20 11:27。稿件称，11 月 17 日 15 时 26 分，南口小型消防站接到警情：南口镇东园村南侧树林内一名男子从树上坠落受伤，无法自主行动。站内调派车辆和 7 名救援人员携带担架、绳索前往；事发地在山林深处，有河道阻隔，地面泥泞。救援人员将伤者转移出山后，移交现场医护人员送医。稿件未公布伤者后续伤情。

**[拧紧供热「安全阀」！区城管执法局开展供热专项执法巡查](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111912013242348/index.html)**。来源：北京昌平 APP，发布于 2026-11-19 12:16。11 月 18 日，区城管执法局到北京永安热力有限公司北环供热厂，启动采暖季供热专项执法巡查，核对备案登记、供热范围与参数、设备巡检和维修台账，以及应急抢修队伍和备件储备等情况。

**[政协北京市昌平区第六届委员会总结大会召开](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111912030357371/index.html)**。来源：北京昌平 APP，发布于 2026-11-19 19:34。11 月 18 日，六届区政协召开总结大会，回顾五年履职。稿件列举的数字包括：协商 125 次、调研视察 310 余次、意见建议 1150 余条；五年征集提案 1037 件、立案 978 件。这些是报道中的官方统计。会议还提到「京华议事厅·有事昌商量」等协商平台，以及全市首家复合型区级政协文史馆。区政协主席蒋达峰出席。

**[党建引领 政府主导 居民参与 企业担当 北七家镇打造多方协同共治小区物业焕新样板](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112011151387499/index.html)**。来源：北京昌平 APP，发布于 2026-11-20。稿件介绍北七家镇推动小区物业应急接管后的整改，包括地下车库汛期积水、照明和排水管网、绿地补植，以及便民摆渡车等措施；在业委会正式组建前，镇里牵头成立物业志愿监督队伍，并搭建居民、物业、社区三方会商。具体小区名称与整改细节以原文为准。

## 3. 全球头条

路透社源站本次未能抓取，美联社 RSSHub 返回 403，《纽约时报》World 的 RSS 可获取标题，但正文页返回 403，故世界新闻以 BBC 和《卫报》为主，纽约时报条目只保留标题与链接，不根据标题臆造正文细节。

**[In a year of AI solving maths problems, Anthropic may have just solved the biggest](https://www.bbc.co.uk/news/articles/c6pqr2g7w059o)**（BBC，约发布于采集前 30 分钟量级，页内标注更新于周五夜间至周六早晨时段）。Anthropic 的数学家 Levent Alpöge 声称，他用公司内部、非公开版本的 Claude，在约六周内完成对黎曼猜想（Riemann hypothesis）的证明，并推广到广义黎曼猜想（GRH）。BBC 写明：若最终被确认，这将是历史上最重要的证明之一；陶哲轩（Terence Tao，BBC 页误写为 Terrance）表示，验证和消化还需要时间。Alpöge 在自己的说明里写道，时机「很糟糕」，并称把宣布和 Anthropic 上市联系起来的「明显的愤世嫉俗看法」是不成立的。这是当事人自己的声明，不是已完成的学术认证。同一组工作还与流体力学中的爆破性结果有关，详见下文 Hacker News。微博和 X 上已出现「AI 证明黎曼猜想」的讨论，均应视为尚未被数学共同体接受的宣称。

**[Tech stock sell-off drags markets down as Anthropic shares slide](https://www.bbc.co.uk/news/articles/c6808ym10vzgo)**（BBC，2026-11-20 14:36 GMT，后有更新）；《卫报》同日报道 [Nasdaq erases all 2026 gains as AI sell-off dampens Anthropic’s second day of trading](https://www.theguardian.com/business/2026/nov/20/global-stock-markets-slump-anthropic-ipo-ai-sell-off)。这是对昨日 Anthropic 上市报道的续报，也有新的收盘数字。BBC 称，周五 Anthropic 股价一度跌逾 12% 至约 85 美元，接近 83 美元的发行价，收盘下跌 8.5%，回吐了周四涨幅的一半；标普 500 下跌 3.7%，道指下跌 1.9%，纳斯达克综合指数下跌 5.3%，标普与道指进入较近期高点回撤 10% 以上的回调区间。英伟达收跌 13.7%。BBC 写明，路透报道英伟达会计处理正被美国证券交易委员会调查，但 BBC 本身未予确认。亚洲方面，韩国综指和日经 225 约跌 5%，台湾股市约跌 6%，报道称其周跌幅超过 17%，为 1990 年以来最大的单周跌幅之一。欧洲主要股指也收跌。这些是各报道中的市场数字，不是对本期早报金融栏的二次换算。

**[Russian missile hits Poland as Ukraine's allies hold military exercise, says Tusk](https://www.bbc.co.uk/news/articles/cqx2x9dklxnro)**（BBC，2026-11-20 12:09 GMT）。波兰称，周五早间有三件物体进入其领空，其中一枚俄罗斯 Kh-101 巡航导弹落在距乌克兰边境约 50 公里的东南部 Nowy Lipowiec 农村地区，另外还有疑似导弹和喷气动力无人机坠落点。总理图斯克（Donald Tusk）认为，这发生在西方国家于该地区举行军事演习期间，「看起来不像意外」。报道称无人伤亡、也没有财产损失报告；华沙称之为「挑衅」，北约秘书长吕特谴责并称已升空战机。俄罗斯方面当时尚未就此置评。同日相关续报是 [Russia targets Kyiv crossings days after Ukraine hits Crimean Bridge](https://www.bbc.co.uk/news/articles/c6x29gn4pdn9o)：俄罗斯导弹和无人机袭击了基辅第聂伯河上的三座桥梁以及利沃夫一座车站，BBC 称至少八人死亡。这是克里米亚大桥遇袭之后的新进展，普京此前已放话将作出「痛苦」报复。

**[Trump threatens ban on US firms building AI data centres overseas](https://www.bbc.co.uk/news/articles/cmde1lw9y54ko)**（BBC）；《卫报》作 [Trump threatens ‘tremendous penalties’ on US tech firms that build datacenters abroad](https://www.theguardian.com/us-news/2026/nov/20/trump-datacenters-white-house)。特朗普返美后在记者会上放话，可能禁止或重罚在海外建设人工智能数据中心的美国公司，并点名芬兰等地的项目。报道将其放在美国国内对数据中心选址、电力和中期选举之后监管预期的语境里。这是其本人的政策放话，尚未写成已生效的禁令。

**[Denmark accuses Russia of plotting to assassinate US-Ukrainian rapper](https://www.bbc.co.uk/news/articles/cmde1lj4yjxno)**（BBC）。丹麦安全情报机构称，已阻止针对一名乌克兰裔美国人的暗杀图谋，丹麦媒体指认目标为说唱歌手 Kyivstoner（真名 Albert Vasiliev）；两人被控未遂谋杀和协助外国情报机构，均不认罪。丹麦宣布驱逐俄罗斯防务武官。俄罗斯驻丹麦使馆否认指控，称其没有证据，并指责这是宣传。这是丹麦官方的指控和俄方否认，不是已在法庭上证实的判决。

**[California investigates Nvidia over whether chip exports ended up in China](https://www.theguardian.com/technology/2026/nov/20/california-investigates-nvidia-over-whether-chip-exports-ended-up-in-china)**（《卫报》，2026-11-20 09:18 GMT）。这是对本周英伟达与黄仁勋去职风波的续报：加州检察长 Rob Bonta 已向英伟达发出调查传票，聚焦先进芯片是否流入中国、以及公司是否误导投资者。Bonta 说，英伟达及其前首席执行官的行为「亮起了鲜红的警示灯」。报道再次提到与新加坡 Megaspeed、黄仁勋事务相关的既有调查线索。这些是加州检方启动调查的新闻，不是已认定的违法结论。

其他新条目，不展开长写：[UK to explore even closer ties with EU after agreeing deal, says Burnham](https://www.bbc.co.uk/news/articles/c6jreyqgw4e9o)（BBC 称英国首相安迪·伯纳姆推动与欧盟更紧密关系，反对党对其引用的经济数字提出质疑）；BBC 中文评论 [中俄美三方峰会「场面大於實質成果」](https://www.bbc.com/zhongwen/articles/cm5y120z0pw0o/trad) 是对深圳三方会晤的后续观察，不重复已写过的联合声明本身。《纽约时报》World RSS 中的 ['Russian Objects' Crashed in Poland…](https://www.nytimes.com/2026/11/20/world/europe/poland-russia-airspace-missile.html)、[Britain and Brussels Have Begun a Brexit Rollback](https://www.nytimes.com/2026/11/20/world/europe/britain-and-brussels-have-begun-a-brexit-rollback-how-far-will-it-go.html)、[Denmark Expels Russian Diplomat…](https://www.nytimes.com/2026/11/20/world/europe/denmark-russia-ukraine-rapper-assassination.html) 等，正文页本次返回 403，只保留标题。

## 4. Hacker News 近期文章

首页来自 Algolia [front_page](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集于 2026-11-21 07:32:53 Asia/Shanghai（UTC+8）。今日讨论几乎被一组数学宣称和若干人工智能系统新闻占满。对最热或讨论最多的条目打开了原文；黎曼猜想与纳维－斯托克斯相关结果都还在验证中，下文只陈述各方自己的说法，不把它们写成已经成立的定理。

**[Levent Alpöge claims proof of the Generalized Riemann Hypothesis [pdf]](https://alpo.ge/remark.pdf)**（[HN](https://news.ycombinator.com/item?id=50574968)，2255 点 / 1536 评，发布 2026-11-20 22:16:21 Asia/Shanghai）。Alpöge 在这份题为 *Remark* 的短文里写道，他相信自己「与 Claude 一起」发现了黎曼猜想的证明，并且方法可以推广到广义黎曼猜想；形式化文件放在分段压缩包中。他写「这是科学里某种更伟大事物的一次黎明」，也解释自己为何选择在公司上市次日公布。BBC 报道与这份原文一致，都强调验证尚未完成。

**[Hurried Announcement: Alessandro Masullo GRH](https://math216.wordpress.com/2026/11/20/hurried-announcement-alessandro-masullo-grh/)**（[HN](https://news.ycombinator.com/item?id=50579568)，1308 点 / 599 评，发布 2026-11-21 02:33:14 Asia/Shanghai）。美国数学会会长、斯坦福大学的 Ravi Vakil 在会议间隙发布简短声明：Alessandro Masullo 提出一份 GRH 证明草稿，斯坦福的 Brian Conrad 已审读数月并给过大量反馈，「目前看起来不错」（so far looking good）；声明强调「全部由人完成，没有人工智能」。原先计划请作者来斯坦福打磨后再宣布，因当天另一则宣称而提前公开草稿，并希望同行尽快核对、形式化并补上可能的小缺口。直接抓取该页返回 403，正文来自后来读到的页面文本。

**[Unforced Navier-Stokes Singularity and the Generalized Riemann Hypothesis](https://terrytao.wordpress.com/2026/11/20/unforced-euler-singularity-unforced-navier-stokes-singularity-and-the-generalized-riemann-hypothesis/)**（[HN](https://news.ycombinator.com/item?id=50578358)，288 点 / 108 评，发布 2026-11-21 01:21:36 Asia/Shanghai）。陶哲轩按「目前被消化的程度」由高到低列出三件事：Alpöge、Tristan Buckmaster 与 Matei Coiculescu 在大量人工智能辅助下，写出了三维无外力不可压缩欧拉方程有限时间爆破的可读证明，并有 Lean 形式化；Alpöge 与 Buckmaster 再次大量使用人工智能，给出三维无外力纳维－斯托克斯方程有限时间爆破的证明及 Lean 形式化，策略大体清楚，但「还需要更多工作才能写成专业的证明」；Alpöge 用内部模型生成了规模巨大、目前几乎只有 Lean 的 GRH 证明，初步看起来动用了当代朗兰兹纲领与算术几何的工具，消化需要时间。直接抓取该博客返回 403，正文同样来自后来读到的页面文本。

**[Finite-time blow-up for the Navier–Stokes equations](https://github.com/tristanbuckmaster/navier-stokes/)**（[HN](https://news.ycombinator.com/item?id=50576232)，240 点 / 77 评，发布 2026-11-20 23:34:31 Asia/Shanghai）。仓库说明称，内含 Alpöge 与 Buckmaster 日期为 2026 年 11 月 20 日的 79 页论文，以及 Lean 4 形式化；并写明形式化中不含数据，论文给出哈希的证书将另行发布，附录中的区间算术验证也不在本仓库里。这是作者一侧的发布说明，不等于证明已被接受。

**[The stochastic parrots have apparently proved the Riemann Hypothesis](https://scottaaronson.blog/?p=10344)**（[HN](https://news.ycombinator.com/item?id=50581084)，172 点 / 138 评，发布 2026-11-21 04:03:07 Asia/Shanghai）。Scott Aaronson 的标题带有反讽。他记录了 Alpöge 关于约 1740 万行 Lean 的说法，并写自己「不是百分之百确定，但我的赌注是这个证明能站住」；同时也强调，数学家只有在能够自己解释并重构这些想法之后才会满意，而那可能需要多年。他提醒 Lean 内核与类型论仍有需要修补的问题。该页直接抓取返回 403，摘要依据后来读到的文本。

**[Frostbite: A new CPU architecture discovered, designed and verified by AI](https://architectlabs.com/blog/frostbite)**（[HN](https://news.ycombinator.com/item?id=50572503)，604 点 / 316 评，发布 2026-11-20 18:01:41 Asia/Shanghai）。Architect Labs 在 11 月 18 日的博文中介绍 Frostbite：称其人工智能系统从指令集到 GDS 自主迭代，做出一款基于 interaction nets 的通用 CPU，并在 25 个工作负载（其中 15 个留作最终评估）上，相对一款现代超标量（双发射、顺序执行）CPU 核心，给出 4.59 倍的每瓦性能。这些数字和「由人工智能发现、设计并验证」的表述，都是该公司自己的说法，不是独立评测。

**[Inkling 2 Mini](https://thinkingmachines.ai/news/inkling-2-mini/)**（[HN](https://news.ycombinator.com/item?id=50581260)，515 点 / 82 评，发布 2026-11-21 04:12:19 Asia/Shanghai）。Thinking Machines 发布开源权重模型 Inkling 2 Mini，称其小到可以在笔记本上运行；结构上是 looped transformer，对中间层每个 token 循环三次。官方介绍称，在总参数量小于 1000 亿的开源权重模型中，它在 DeepSWE v1.1（48.2%）和 Vals Index v2.2（46.5%）等基准上领先，并且在达到相近表现的模型里更快。这些排名和分数是出品方的说法。

**[Signal Is Serious About Protecting Your Privacy](https://signal.org/blog/protecting-your-privacy/)**（[HN](https://news.ycombinator.com/item?id=50572348)，471 点 / 290 评，发布 2026-11-20 17:42:16 Asia/Shanghai）。Signal 总裁 Meredith Whittaker 在 11 月 20 日写道，将限制内置于操作系统的人工智能代理采集 Signal 屏幕内容：继去年用截图阻断来应对 Windows 11 的 Recall 之后，现在对 iOS 27 以及可检测到助手试图读取屏幕的 Android 版本采取类似措施。她认为，操作系统级代理正在削弱应用层的隐私保证；用户可在设置中关闭该保护，但会暴露自己和联系人的内容。文中也承认，截图阻断并不完整，且目前无法在 macOS 上实现同样保护。

**[Language Models Can Rewrite Their Own Weights](https://arxiv.org/abs/2611.21885)**（[HN](https://news.ycombinator.com/item?id=50577265)，313 点 / 103 评，发布 2026-11-21 00:29:06 Asia/Shanghai）。Jiajun Fan 等在 arXiv:2611.21885（v2，2026-11-18）中提出「self-rewriting」：一个开放的 27B 模型在没有梯度、也不重新训练的情况下，依据自身推理改写自己的权重。作者称，它在未见过的题目上提高 6.6 个百分点；连续八轮只提交有效的修改，准确率只升不降；还能在不读取原始权重的情况下，把一份受损副本在未见过的图像任务上恢复到原准确率的 80% 以上。这些是论文摘要中的实验表述，不是第三方复现结果。

**[Google Workers Tell Their Employer Not to Punish Schools That Don't Want AI](https://www.motherjones.com/politics/2026/11/google-alphabet-union-school-ai-protest-gemini-workers-petition/)**（[HN](https://news.ycombinator.com/item?id=50577901)，239 点 / 175 评，发布 2026-11-21 00:59:27 Asia/Shanghai）。*Mother Jones* 报道，数百名谷歌员工推动高层撤回一项政策：从明年起，关闭 Gemini 人工智能工具的学校将无法继续使用谷歌搜索。Alphabet 工会请愿书说，切断搜索并不能说服用户，更可能让学校彻底离开谷歌产品。报道称，纽约、洛杉矶、芝加哥等学区已在讨论替代搜索；公司领导层已承认收到信件，但尚未回应具体要求。谷歌已被要求置评。

**[We promoted developers into architects without informing them](https://manidoraisamy.com/developer-to-architect.html)**（[HN](https://news.ycombinator.com/item?id=50579331)，238 点 / 154 评，发布 2026-11-21 02:17:51 Asia/Shanghai）。Mani Doraisamy 认为，当代码多由人工智能根据需求直接生成时，真正要做的是先定架构和数据模型，并在需求冲击性能或可维护性时往回推；而许多被「提拔」的开发者并未接到这个新岗位说明。这是一篇经验评论，不是对某一款工具的评测。

**其余首页条目。** [If you can't explain something in simple terms, you don't understand it (2017)](https://kottke.org/17/06/if-you-cant-explain-something-in-simple-terms-you-dont-understand-it)（[HN](https://news.ycombinator.com/item?id=50572355)，596 点 / 284 评）是旧文重上。[Nvidia accounting under SEC investigation, sources say](https://finance.yahoo.com/markets/article/nvidia-stock-extends-25-trillion-rout-as-sec-probe-reportedly-investigates-its-accounting-194945274.html)（[HN](https://news.ycombinator.com/item?id=50581438)，178 点 / 76 评）原文页本次返回 403，BBC 亦写明这是路透报道、自身未确认，故不把调查写成已证实事实。[Show HN: I made an audio-to-MIDI model 60x more efficient](https://kobi.music/research/dettato)（[HN](https://news.ycombinator.com/item?id=50526023)，221 点 / 48 评）。[Vibecoding an inference chip](https://ankitg.me/blog/vibecoding-inference-chip/)（[HN](https://news.ycombinator.com/item?id=50579297)，97 点 / 31 评）。[The G1 Garbage Collector](https://dev.java/learn/jvm/tool/garbage-collection/g1gc-overview/)（[HN](https://news.ycombinator.com/item?id=50527444)，95 点 / 49 评）。[I'm Peter Roberts, immigration attorney who does work for YC and startups. AMA](https://news.ycombinator.com/item?id=50577613)（[HN](https://news.ycombinator.com/item?id=50577613)，91 点 / 122 评）。[Winedroid – run Android apps without Android (WASM demo)](https://winedroid.soham.sh/demo/)（[HN](https://news.ycombinator.com/item?id=50580536)，80 点 / 25 评）。[Microsoft announces Windows Server 2028 with hardened security](https://www.bleepingcomputer.com/news/microsoft/microsoft-announces-windows-server-2028-with-hardened-security/)（[HN](https://news.ycombinator.com/item?id=50550430)，60 点 / 61 评）。[DreamCoder: Coding harness and IDE from the author of Mastering Emacs](https://www.masteringemacs.org/article/announcing-dreamcoder)（[HN](https://news.ycombinator.com/item?id=50581110)，59 点 / 9 评）。[And Yet, It Moves](https://signoregalilei.com/2026/11/20/and-yet-it-moves/)（[HN](https://news.ycombinator.com/item?id=50581177)，52 点 / 24 评）。[Running two PSP emulators on one Switch 2 and sharing one via GameShare](https://github.com/XITRIX/ppsspp-nx2/blob/master/SWITCH2-GAMESHARE.md)（[HN](https://news.ycombinator.com/item?id=50578233)，51 点 / 0 评）。[Show HN: An API for word timestamps from speech, 75% within 20ms](https://quebec.yarn.so)（[HN](https://news.ycombinator.com/item?id=50532515)，48 点 / 8 评）。[Show HN: OpenComputer – an open source alternative to Devin](https://github.com/diggerhq/opencomputer)（[HN](https://news.ycombinator.com/item?id=50581403)，42 点 / 14 评）。[A few hours ago Google DeepMind created a math horizon repo](https://github.com/google-deepmind/math-horizon)（[HN](https://news.ycombinator.com/item?id=50582629)，33 点 / 20 评）本次打开该仓库地址返回 404，只保留标题与链接。[NINLIVE: The Nine Inch Nails live archive](https://ninlive.com/)（[HN](https://news.ycombinator.com/item?id=50583274)，33 点 / 4 评）。[Nasdaq erases all 2026 gains](https://www.cnbc.com/2026/11/19/stock-market-today-live-updates.html)（[HN](https://news.ycombinator.com/item?id=50583254)，28 点 / 2 评），市场数字见上文全球头条。[Reverse Engineering my cat's litter box](https://master--ytulsiani.netlify.app/blog/furrytails/)（[HN](https://news.ycombinator.com/item?id=50581165)，20 点 / 8 评）。[Show HN: Professor Euler – Offline math desk, 300-function CAS, workbooks](https://euler.dawei7.com)（[HN](https://news.ycombinator.com/item?id=50537626)，8 点 / 0 评）。[The Hungry Butler Effect: Concealed Commercial Incentives in LLMs](https://www.researchgate.net/publication/418143113_The_Hungry_Butler_Effect_Concealed_Commercial_Incentives_and_the_Erosion_of_Epistemic_Rigour_in_Large_Language_Models)（[HN](https://news.ycombinator.com/item?id=50583117)，6 点 / 2 评）。

## 5. X 热门与科技圈

采集约在 07:34 Asia/Shanghai（UTC+8），使用 X 公共趋势接口。全球榜和中国地区榜当日高度重合，前列多为体育和娱乐标签，如 #StarAcademy、Bayern、Daniel Jones 等。与科技和科学明显相关的，是同时出现在全球和美国趋势中的 [Riemann](https://x.com/search?q=Riemann)（接口给出的讨论量约 42,673）以及日文趋势 [リーマン予想](https://x.com/search?q=%E3%83%AA%E3%83%BC%E3%83%9E%E3%83%B3%E4%BA%88%E6%83%B3)。美国趋势里还有 [Nasdaq](https://x.com/search?q=Nasdaq)（约 39,229）和 [Trumpcare](https://x.com/search?q=Trumpcare)（约 2,107），以及讨论量很高但与科技关系较弱的 [WhatsApp](https://x.com/search?q=WhatsApp)。

关于黎曼猜想的讨论，与上文 BBC、Alpöge 原文、陶哲轩博文和 Vakil 声明是同一件事，不应把趋势热度理解成证明已经被确认。X 的新闻摘要功能也汇总了相关帖文，但该摘要自带「可能随时间变化、需要核对」的说明，本文不以那些自动摘要为事实来源。社区里同时在传两件事：Alpöge 与 Claude 的 Lean 形式化，以及 Masullo 一份号称完全由人完成的长草稿。未核实的细节，只标明在流传。

纳斯达克相关讨论，则与周五人工智能板块抛售、Anthropic 次日回落相呼应，数字仍以BBC 和《卫报》的报道为准。

## 6. 微博热搜

接口 [weibo.com/ajax/side/hotSearch](https://weibo.com/ajax/side/hotSearch) 在 2026-11-21 07:32:53 Asia/Shanghai（UTC+8）返回成功。置顶/政务（hotgov）为 [#习近平会见泰国总理#](https://s.weibo.com/weibo?q=%23%E4%B9%A0%E8%BF%91%E5%B9%B3%E4%BC%9A%E8%A7%81%E6%B3%B0%E5%9B%BD%E6%80%BB%E7%90%86%23)。本期未打开独立官方稿核对会见细节，只记录该话题被放在政务置顶位置。实时榜未标记 `is_ad` 的广告位。自然热搜里，与科技、市场和时政相关的如下；「金价」一词昨日已出现过，今日只作为行情背景，不单列旧闻。

**科技、市场与国际。** [#DeepSeek付费体验直线上升#](https://s.weibo.com/weibo?q=DeepSeek%E4%BB%98%E8%B4%B9%E4%BD%93%E9%AA%8C%E7%9B%B4%E7%BA%BF%E4%B8%8A%E5%8D%87) 位于实时榜第 1（热度值 844,127），这是平台热度，不是对产品数据的核实。[#APEC盛会效应拉满#](https://s.weibo.com/weibo?q=%23APEC%E7%9B%9B%E4%BC%9A%E6%95%88%E5%BA%94%E6%8B%89%E6%BB%A1%23) 是对本周深圳峰会的余波，不重复已写过的联合声明。[AI证明黎曼猜想传闻](https://s.weibo.com/weibo?q=AI%E8%AF%81%E6%98%8E%E9%BB%8E%E6%9B%BC%E7%8C%9C%E6%83%B3%E4%BC%A0%E9%97%BB) 与全球头条、Hacker News 为同一事件，话题本身已标明「传闻」；证明是否成立，仍待数学共同体检验。[余承东称现在L2开车不能睡觉](https://s.weibo.com/weibo?q=%E4%BD%99%E6%89%BF%E4%B8%9C%E7%A7%B0%E7%8E%B0%E5%9C%A8L2%E5%BC%80%E8%BD%A6%E4%B8%8D%E8%83%BD%E7%9D%A4%E8%A7%89)、[#华为首款鸿蒙AI手机#](https://s.weibo.com/weibo?q=%23%E5%8D%8E%E4%B8%BA%E9%A6%96%E6%AC%BE%E9%B8%BF%E8%92%99AI%E6%89%8B%E6%9C%BA%23) 是消费电子和智能驾驶相关话题，本期未打开产品发布会原文，不转写具体规格。[#股民集体抛售科技股#](https://s.weibo.com/weibo?q=%23%E8%82%A1%E6%B0%91%E9%9B%86%E4%BD%93%E6%8A%9B%E5%94%AE%E7%A7%91%E6%8A%80%E8%82%A1%23)、[#费城半导体指数持续下挫#](https://s.weibo.com/weibo?q=%23%E8%B4%B9%E5%9F%8E%E5%8D%8A%E5%AF%BC%E4%BD%93%E6%8C%87%E6%95%B0%E6%8C%81%E7%BB%AD%E4%B8%8B%E6%8C%AB%23)、[#这轮金价为何跌那么快#](https://s.weibo.com/weibo?q=%23%E8%BF%99%E8%BD%AE%E9%87%91%E4%BB%B7%E4%B8%BA%E4%BD%95%E8%B7%8C%E9%82%A3%E4%B9%88%E5%BF%AB%23)、[#现货黄金大跌3%#](https://s.weibo.com/weibo?q=%23%E7%8E%B0%E8%B4%A7%E9%BB%84%E9%87%91%E5%A4%A7%E8%B7%8C3%25%23) 与周五全球科技股和黄金走势同一时段；黄金的具体读数见金融栏，不把热搜标题里的「3%」直接当成今日早报的统计口径。[#特朗普涉中俄美最新表态#](https://s.weibo.com/weibo?q=%23%E7%89%B9%E6%9C%97%E6%99%AE%E6%B6%89%E4%B8%AD%E4%BF%84%E7%BE%8E%E6%9C%80%E6%96%B0%E8%A1%A8%E6%80%81%23)、[#特朗普刚返美就发重大预告#](https://s.weibo.com/weibo?q=%23%E7%89%B9%E6%9C%97%E6%99%AE%E5%88%9A%E8%BF%94%E7%BE%8E%E5%B0%B1%E5%8F%91%E9%87%8D%E5%A4%A7%E9%A2%84%E5%91%8A%23) 可与他在白宫记者会上关于数据中心、以及他自称与普京、习近平「关系极好」等公开表态对照，但「重大预告」是热搜用语，具体内容仍以BBC、《卫报》报道为准。

**速览。** 其余靠前条目多为综艺、剧集和娱乐，如后会友期黄焖鸡事件、李嫣唱歌、王子璇与马天宇、成毅《两京十五日》、林更新、杨超越，以及 U17 国足 0 比 5 不敌西班牙等，不展开。

## 7. 油管科技访谈

对照 `docs/youtube-sources.md` 的频道名单，从各频道 `/videos` 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。许多频道本周早些时候的节目已在前几期写过，故今日能新写的条数不多。

**[Why AI Has DHH Working 16-Hour Days](https://www.youtube.com/watch?v=TtOoLanFzGw)**  
a16z · 52:15 · 发布于 2026-11-20 23:39:04 Asia/Shanghai（UTC+8）。频道视频列表上的标题是 *Why DHH Is Betting on Linux in the Age of AI Agents*。官方简介称，David Heinemeier Hansson（DHH）认为智能体时代重新打开了「打造人们真正想用的新操作系统」这扇窗；他与 a16z 的 Martin Casado、Anish Acharya 讨论自己正在做的 Omarchy，一个「面向智能体、用户只需开口就能修改」的 Linux 发行版。简介里关于工作强度和产品定位的句子，是节目或出品方的概述，不是对发行版采用量的统计。

**[The Whistleblower Who Took on Theranos](https://www.youtube.com/watch?v=iXWSYlAX5Lg)**  
Y Combinator · 2:56:16 · 发布于 2026-11-12 03:44:03 Asia/Shanghai（UTC+8）。官方简介写，随着 Theranos 和 Elizabeth Holmes 再次进入公共讨论，节目重访 Tyler Shultz 的第一手叙述：他从斯坦福毕业后加入公司，祖父、前国务卿 George Shultz 当时在董事会。这是长访谈，不是对当日其他栏目新闻的复述。

**[Freedom vs. Safety: Axon CEO Rick Smith on the Future of Policing](https://www.youtube.com/watch?v=8h-gfrVYyAU)**  
All-In Podcast · 55:35 · 发布于 2026-11-11 07:13:29 Asia/Shanghai（UTC+8）。官方章节包括：TASER/Axon 从濒临破产到上市，在互联网泡沫破裂期间上市、向警方销售并应对做空与 SEC 调查后转向软件，以及警用执法记录仪、Flock 等监控系统引发的担忧，还有自由与安全、Skydio 交易和 Taser 无人机项目争议。这些是节目章节目录中的议题，不是对某一案件的判决转述。

**[What Frontier Labs Buy: A Data Deep Dive with Handshake AI — Garrett Lord & Team](https://www.youtube.com/watch?v=v5IJwVnTxzg)**  
Latent Space · 2:43:49 · 发布于 2026-11-09 23:18:21 Asia/Shanghai（UTC+8）。节目称这是对人工智能数据公司的一次深访。官方简介写道，Handshake AI「从上线到大约 10 亿美元年化总收入用了约一年」——这是节目或出品方的说法。讨论围绕前沿实验室实际采购的强化学习环境和专家训练数据，以及简介中提到的一个情节：有智能体曾找到办法为净收入「赚取」信用。

All-In 在 2026-11-21 06:28:55 Asia/Shanghai（UTC+8）还更新了 **[Anthropic Goes Public, Nvidia in Crisis, Markets Tank, Open Source Crackdown?](https://www.youtube.com/watch?v=G5w7EyF-aFQ)**（1:16:41）。官方章节覆盖 Anthropic 上市、市场多空、白宫对开源模型披露规则的讨论，以及英伟达股价、人才和法律争议。这些内容与当天全球头条和金融栏高度重叠，这里只作一行提示，不再展开。

## 8. 本月阅读与今日书摘

今天是星期六。按 [本月阅读计划](/reading/)，周末只保留书单和进度，不新写章节摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。下一本《人件》将按同样方式分期，具体安排见仓库 [`docs/reading-plan-2026-11.md`](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

今天的信息环境几乎被两件尚未定论、却已被放得很大的事撑满。一件是数学：Alpöge 与 Claude 的 Lean 形式化、Masullo 那份「全由人完成」的草稿，以及陶哲轩按「消化程度」排列的欧拉、纳维－斯托克斯和 GRH。它们都还在被阅读、被编译、被质疑，不能因为热搜或 HN 上千条评论就提前写成「已经证明」。另一件是市场：Anthropic 上市次日回落，纳斯达克大跌，A 股上一个交易日也明显走弱，黄金则是连续第三期早报下跌。把数学宣称和股价涨跌直接写成因果关系并不稳妥，但它们确实出现在同一天的时间线上。

本地这边是更冷的一个早晨，北京市区实况已到 −3.3℃。海淀的医保钱包说明、昌平南口的山林救援，和全球头条不在同一量级，却是真正落在区里的事。阅读上，《人月神话》已经读完，「没有银弹」还在耳边：工具可以消掉偶然的麻烦，但概念本身的复杂不会因为某一晚的宣布就消失。若只从今天的访谈里留一句，DHH 那期更值得记住的不是工时，而是智能体是否真的重新打开了「操作系统还可以被用户改写」这扇窗。
