---
layout: post
title: "早报 · 2026-11-27"
date: 2026-11-27 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-27 07:50:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/27/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 27 日（星期五）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:38–07:39 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:38–07:39，原文页约在 07:40–07:42；X 热榜与新闻摘要约在 07:40 前后；油管频道页约在 07:40–07:41，节目页约在 07:42。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 feeds.reuters.com 再次 TLS 连接失败，www.reuters.com/world/rss 返回 401；美联社经由 RSSHub 的源返回 403；《卫报》World / International RSS 返回 403；《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写；东方财富行情接口返回 502；新浪财经简况接口在加 Referer 后可用。均已在相应栏目说明。写稿时尚未到 09:15 中间价和 09:30 开盘，人民币中间价与 A 股本期采用 11 月 26 日（星期四）已公布的官方读数。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期五，写稿时官方中间价和开盘价尚未公布，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 docs/brief-memory/finance-history.json。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,566.00 美元/盎司 | 较上一期早报（2026-11-26 07:36:17 Asia/Shanghai (UTC+8)）−5.30（−0.15%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 3566.0，报价单位为美元/盎司；updatedAt 为 2026-11-26T23:38:48Z（合 2026-11-27 07:38:48 Asia/Shanghai）。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,571.30）计算 | 2026-11-27 07:38:48 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7096（11 月 26 日） | 较上一发布日（2026-11-25，6.7088）变动 +0.0008 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-27 07:38:57 返回的最新一条是 11 月 26 日的 6.7096；更早记录为 11 月 25 日 6.7088、11 月 24 日 6.7111、11 月 23 日 6.7120、11 月 20 日 6.7131。**本期采用 11 月 26 日已公布中间价**（写稿时尚未到当日 09:15 发布时间）。变化栏按官方上一发布日口径 | 采集 2026-11-27 07:38:57 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.683199 | 较上一期早报（2026-11-25 08:02:31 Asia/Shanghai (UTC+8)）+0.005020（+0.08%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。time_last_update_utc 为 Thu, 26 Nov 2026 00:02:31 +0000（合 2026-11-26 08:02:31 Asia/Shanghai），较上一期早报所用的 11 月 25 日那一笔日更已刷新；time_next_update_utc 显示为 Fri, 27 Nov 2026 00:35:41 +0000（约合 08:35:41 Asia/Shanghai），采集时尚未到达 | 2026-11-26 08:02:31 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3476.88 | +0.41（+0.01%） | [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 返回：最新价 3476.88，涨跌 +0.41，涨跌幅 +0.01%，昨收 3476.47，开盘 3490.14，最高 3497.81，最低 3455.04，行情时间戳 20261126161427（2026-11-26 16:14:27）。[新浪财经](https://hq.sinajs.cn/list=s_sh000001,s_sz399001) 交叉核对价格一致（3476.8816，涨跌 +0.4119），涨跌幅同为 +0.01%。[东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 本次返回 502，故不以它为数值来源。写稿时尚未开盘，**本期采用 11 月 26 日（星期四）收盘价，不是今日盘中或开盘价** | 采集 2026-11-27 07:38:57 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10084.04 | −2.32（−0.02%） | 同上来源：腾讯财经最新价 10084.04，涨跌 −2.32，涨跌幅 −0.02%，昨收 10086.36，开盘 10184.94，最高 10235.50，最低 9979.06，行情时间戳 20261126161415（2026-11-26 16:14:15）。新浪财经交叉核对价格与涨跌幅一致（10084.04，涨跌 −2.312，−0.02%） | 采集 2026-11-27 07:38:57 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报小幅回落约 0.15%，报 3,566.00 美元/盎司，把前一日那一点回升又吐了回去。市场化参考汇率随接口日更从 11 月 25 日那一笔刷新为 11 月 26 日的 6.683199，较上一期所用读数升 0.08%。官方中间价本期改用 11 月 26 日已公布的 6.7096，较 11 月 25 日中间价上调 0.0008；A 股本期采用 11 月 26 日收盘价，上证几乎平收（+0.01%），深成指微跌 0.02%，是周三深跌之后的横盘，不是今日开盘或收盘。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [/api/weather/view?stationid=54511](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 lastUpdate 为 2026/11/27 07:25；本次采集时间为 2026-11-27 07:38:58 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按该局页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。预警列表中有一条：北京市气象台 2026 年 11 月 26 日 14 时 40 分发布大风蓝色预警信号。接口的实况对象未给出天气现象字段，故不编造当前天空状况。

**当前实况**（lastUpdate 2026/11/27 07:25）：气温 9.3℃，体感温度 4.9℃，相对湿度 29%，西北风 3 级，风速 4.6 米/秒，降水量 0.0，气压 1013.0 百帕。

**今日（11 月 27 日）预报**：白天晴，最高 10℃，西北风 3～4 级；夜间多云，最低 0℃，西北风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 28 日 | 白天多云，夜间晴 | 11℃ / −1℃ | 白天西北风微风，夜间南风微风 |
| 11 月 29 日 | 白天晴，夜间晴 | 10℃ / 0℃ | 白天西南风微风，夜间北风微风 |
| 11 月 30 日 | 白天多云，夜间多云 | 12℃ / 0℃ | 白天东南风微风，夜间东北风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。早晨实况已到 9.3℃，接近今日预报最高气温，和昨天预报里「白天西北风 3～4 级」的方向一致；夜间最低气温由此前展望中的 −1℃ 调整为 0℃，并改为多云。

### 海淀区与昌平区本地新闻

写稿前已对照 docs/brief-memory/seen.json。昨日及此前已写过的海淀东部片区街镇工作座谈、区委常委会与区政府常务会、十一届区政协履职总结、「光影智谷」、教育人才培育、交通调研等，以及昌平的生命科学园调研、美丽健康产业与多美康、波兰企业代表团、城北街道城市更新、跨国药企圆桌、脑机接口大会等，不再重复。今天海淀栏主要是 11 月 25 日的区委常委会；昌平则有八达岭奥莱用地续期、东小口燃气预约式指导、都市芳园旧改基本竣工、北七家路网，并对美国白蛾越冬蛹除治作续报。

#### 海淀区

**[区委常委会召开会议 传达学习贯彻习近平总书记重要讲话精神 听取区政府党组、区法院党组、区检察院党组工作汇报](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261126_4836790.shtml)**。来源：海淀报，日期 2026-11-26 09:26。稿件称，会议于 11 月 25 日召开，区委书记王少峰主持。议程包括传达学习亚太经合组织第三十三次领导人非正式会议及相关纪念活动、市委常委会会议精神，并通报北京市经济和信息化局印发的《北京市具身智能机器人产业高质量发展行动方案（2026-2028年）》，研究区里落实措施；听取区政府、区法院、区检察院党组 2026 年主要工作和 2027 年安排；还研究了《海淀区「十五五」时期城市管理发展规划》《海淀区「十五五」时期城市更新规划》等事项。报道转述会议要求：结合海淀科创特色加强国际交流合作；推动具身智能产业，支持高校院所攻关，争取专用算力集群和模型测试场在海淀布局，并在公共服务、安全生产及「百年京张 AI 创新带」等区域有序开放标杆场景。对区政府的要求集中在岁末经济运行、民生保障与城市安全，以及「1+X+1」现代化产业体系和南北一体发展。这些安排与表述均来自报道本身。

海淀区政务动态、部门动态和街镇动态列表今早未见比上述常委会更新的近日稿件，来源较薄，故不把已写过的旧稿凑进目录。

#### 昌平区

**[全市首例商业用地使用权提前续期项目落地昌平 八达岭奥莱破解「年限之困」焕新启航](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112516115771901/index.html)**。来源：北京昌平 APP，日期 2026-11-25。稿件称，北京八达岭奥莱项目土地延期已获市政府批复并完成合同签订，是全市首例商业用地使用权到期前提前续期的城市更新项目。报道写，项目一期于 2015 年投用，二期已纳入北京市城市更新储备项目库，但国有土地使用权将于 2037 年 9 月到期，剩余约 11 年，影响长期信贷融资、资产估值和股东决策。稿件把后续「带动数亿元投资、引入更多国际一线品牌」写成展望，不是已经完成的投资统计。作为操作先例，报道称区里形成了从政策申请到合同签署的流程，供后续同类问题参考。

**[商户下单执法队上门，东小口镇推行预约式合规指导，筑牢燃气安全防线](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112516410267654/index.html)**。来源：北京昌平 APP，日期 2026-11-25。报道称，东小口镇综合行政执法队依托全市「预约式」合规指导机制，联合燃气专业力量走进盛天广场、小站公园，为餐饮等燃气非居经营主体提供上门问诊。企业经「京通」平台预约，监管部门提供政策咨询和现场指导；稿件写明，指导记录不直接作为行政处罚依据。现场检查管道、阀门、报警器和紧急切断阀等，并当场说明整改标准。截至发稿，东小口镇已完成 11 家燃气非居用户的预约式上门指导。服务还覆盖市容、工地扬尘和垃圾分类等事项。

**[都市芳园社区老旧小区改造项目基本竣工](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112515244980297/index.html)**。来源：北京昌平 APP，日期 2026-11-25。稿件称，11 月 23 日，东小口镇都市芳园社区旧改随着最后一段柏油路面铺设完毕，历时三年的工程基本竣工，仍待收尾、验收和后期管护。报道写，改造初期原设计为恢复混凝土路面，居民建议改为降噪更好的柏油路；社区上报后，镇里组织居民代表，会同区城管委、设计、施工、监理和物业议事，最终确定园区道路统一铺设柏油路面。嘉湖园、锦湖园、镜湖园、翠湖园 100 余户居民自发众筹路缘石主材费用，镇党委政府统筹落实施工费用。这是社区旧改竣工报道，不是对全部楼体改造细项的验收公报。

**[织密交通路网 畅通民生归途 北七家镇提质升级绘就便民出行新图景](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112516224118240/index.html)**。来源：北京昌平 APP，日期 2026-11-25。报道称，北七家镇已累计推动北清路快速化改造一期、鲁疃西路南延、北苑东路等 44 条市政道路建设，其中 21 条已竣工通车，规划道路实施里程较五年前新增 26.72 公里；2021 年至 2026 年完成北清路辅路、定泗路辅路、八曹路等 26 条乡村公路大修，总里程超 46.3 公里；另完成 6 条农村道路备案，打通包括北清路 1.1 公里路段在内的 5 条断头路，并在温蓬片区、名佳花园社区周边铺设通学绿道。上述里程和条数均为报道给出的累计统计。

**续报：美国白蛾越冬蛹除治。** 此前早报已写过东小口部署、龙泽园和回龙观新龙城等地的挖蛹行动。区政新闻 11 月 25 日稿 **[累计挖除 7.89 万枚 昌平区扎实推进美国白蛾越冬蛹除治工作](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112516122884630/index.html)** 给出了全区进展：覆盖 21 个街道（镇）、185 个村（社区），发动 5947 人次，累计挖除越冬蛹 7.8943 万枚；报道按「每头雌蛾产卵 800 至 2000 粒」测算，称本轮挖除可减少来年第一代幼虫近亿头——这是稿件中的推算，不是已发生的减虫结果。报道还写，今年发生程度明显重于常年，第三代幼虫危害树木数量为去年同期的 2.56 倍。集中除治按市级部署将推进至 12 月底，随后转入常态化排查，持续到明年 3 月成虫羽化前。

## 3. 全球头条

BBC World、BBC 中文和《纽约时报》World RSS 于 2026-11-27 07:38:58–07:38:59 Asia/Shanghai（UTC+8）抓取成功。《卫报》World / International RSS 返回 403；路透社 feeds.reuters.com TLS 失败，www.reuters.com/world/rss 返回 401；美联社 RSSHub 源返回 403，这三家本期不列入。纽约时报正文页返回 403，相关条目只根据 RSS 标题与摘要改写，不假装读过全文。

**[US too focused on Middle East and not pushing Russia hard enough, Zelensky tells BBC](https://www.bbc.co.uk/news/articles/c820q9wgrpyyo)**（BBC，RSS 时间 Thu, 26 Nov 2026 22:49:27 GMT，合 2026-11-27 06:49:27 Asia/Shanghai）。续报：泽连斯基此前已公开说，特朗普把普京称作朋友「很奇怪」。他在基辅办公室接受 BBC 采访时再次使用「aggressor」「killer」等说法，并抱怨美国在和谈中对俄施压不够、防空导弹交付迟缓。稿件写，阿布扎比最近一轮和谈没有明显进展，泽连斯基的概括是「The more we know, the more problems」；他还说，对侵略者「过分中立」等于同时站在受害者和侵略者一边。特朗普 11 月 26 日在 Truth Social 发文，称上周在中国与普京会晤时曾敦促俄方停止在欧洲各地的军事进攻，并认为与乌克兰达成和平协议「大有可能」。这些是当事双方的公开表态，不是和谈已经取得突破。

**[German boat dealer suspected of supplying Channel smuggling gangs, BBC finds](https://www.bbc.co.uk/news/articles/cqlymky8kpzjo)**（BBC，RSS 时间 Thu, 26 Nov 2026 05:00:24 GMT，合 13:00:24 Asia/Shanghai）。BBC 与德国 WDR、NDR、《南德意志报》和法国《世界报》根据警方、法庭和税务文件报道，西部德国小型船企 MaReBoote 的经营者 Marvin Reuter 被欧洲调查人员视为英吉利海峡偷渡网络的重要供货商；法方文件称，今年前四个月被查获的偷渡中，近三分之一涉及该公司的船或发动机。Reuter 正在抗拒向法国引渡，可能面临偷运、共谋和过失致人死亡等指控，目前在被证明有罪之前应被视为无罪。BBC 写，他的设备被怀疑与两起共四人死亡的事故有关；记者在多特蒙德附近与他对质时，他拒绝回答并表示要报警。

**[Diesel tanker carrying up to 7,000 tonnes capsizes near Ibiza, killing one](https://www.bbc.co.uk/news/articles/c9gklryvj24do)**（BBC，RSS 时间 Thu, 26 Nov 2026 22:01:22 GMT，合 2026-11-27 06:01:22 Asia/Shanghai）。马耳他籍油轮 Med Emre 在距伊维萨约 25 海里处倾覆，船上载有最多约 7,000 吨柴油。17 名船员全部获救，其中 7 人送医，1 人随后不治。巴利阿里自治区主席称，可能的燃料泄漏信息仍少；瓦伦西亚海事官员对法新社说，船周围一度出现的小片油膜已经「消失」，并称情况已稳定，周五上午还将再查。船体并非完全沉没，仍部分没于水中，事故原因不明。

**[Two Italians killed in strike in Kuwait, as Iran denies responsibility](https://www.bbc.co.uk/news/articles/c39w9y5dx4k5o)**（BBC，RSS 时间 Thu, 26 Nov 2026 21:17:53 GMT，合 2026-11-27 05:17:53 Asia/Shanghai）。续报：上周科威特曾称击退针对美军驻地空军基地的伊朗无人机。意大利外交部称，两名为德国莱茵金属（Rheinmetall）工作的意大利技术员在此次袭击中死亡。科威特国防部较早时说，在侦测并拦截来自伊朗的多架无人机后，坠落弹片造成两人（另有一名科威特人和一名巴基斯坦人）受伤。伊朗外长阿拉格希否认责任，称事件看起来「可疑」，并向意、科两国表示慰问；军方发言人说伊朗「没有实施任何军事或进攻行动」。科威特军方则称之为「卑劣的伊朗侵略」。责任归属仍有争议，本期只记录双方说法。

**[Hope for millions as cheaper HIV prevention jab reaches Africa](https://www.bbc.co.uk/news/articles/cmly7jve72r2o)**（BBC，RSS 时间 Thu, 26 Nov 2026 11:00:39 GMT，合 19:00:39 Asia/Shanghai）。全球基金称，来那卡韦（lenacapavir）仿制药的首批全球货运已于周三抵达赞比亚，乌干达的交付将在随后数日到位，津巴布韦等国预计明年初跟进。BBC 写，该针剂一年注射两次，预防感染的有效性接近 100%，预期费用约为每人每年 40 美元；吉列德原研药在美国的年费用约为 2.8 万美元。2024 年在乌干达和南非、超过 5,000 名青少年女性参与的临床试验中，接种组无人感染。这些有效性和价格数字均来自报道对试验和采购安排的转述。

**[Myanmar refuses to comply with parts of ICJ genocide ruling](https://www.bbc.co.uk/news/articles/c61wr87wyg5wo)**（BBC，RSS 时间 Thu, 26 Nov 2026 10:25:51 GMT，合 18:25:51 Asia/Shanghai）。续报：国际法院上周裁定缅甸在 2017 年对罗兴亚人的军事行动中构成灭绝种族。政变后执政的敏昂莱在裁决后首次公开回应，称「灭绝种族」一词严重损害国家声誉；据官方媒体，他在周三的会议上说，缅甸会采取「负责任国家」认为适当的行动，但不会遵守它认为「不适当」的要求。声明未具体说明反对裁决的哪些部分。缅甸否认种族灭绝，称部队是在回应武装组织袭击。

**[Nine injured, three critically, after Bangkok oil refinery explosion](https://www.bbc.co.uk/news/articles/crx209kwk4kzo)**（BBC，RSS 时间 Thu, 26 Nov 2026 16:21:19 GMT，合 2026-11-27 00:21:19 Asia/Shanghai）。曼谷东部帕卡农（Phra Khanong）的 Bangchak 炼厂约在当地 14:45 发生爆炸并起火。当局称 9 人受伤；法新社引述当地医院说，其中 3 人危重，早先曾报 4 人。公司称大火在 30 分钟内得到控制，原因仍在调查。泰国能源部长称，爆炸发生在距储油区约 100 米的蒸馏塔，影响看来有限，但因炼厂位于居民区，生产将暂停，直至可以安全恢复。公司称周边空气质量监测在正常范围。

**[特朗普深圳会晤一周后再挥关税大棒 对华税率可达 40%](https://www.bbc.com/zhongwen/articles/c9ly484v6pdzo/simp)**（BBC 中文，2026-11-26T08:34:56Z，合 16:34:56 Asia/Shanghai）。续报昨日美国宣布对多个贸易伙伴加征新关税。BBC 中文写，拟议名单包括中国、欧盟、日本、韩国和台湾等 14 个经济体；对中国的税率上限最高可达 40%，越南最高 35%，其余多为 20% 或 25%，但若计入此前协议中的关税上限，实际缴纳可能低于公布税率。对中国多数商品的拟议税率最高为 20%，部分为 10% 或豁免；报道称，只有在美方认定磋商未能充分解决问题时，才会考虑把对所有中国商品的上限提至 40%。新关税须经公众咨询和听证，最早明年 1 月生效。中国外交部发言人郭嘉昆称之为「政治操弄」；驻美使馆对 BBC 表示，关税战不符合任何人的利益。同一报道还写，中国商务部把锑、镓、锗等对美出口管制的暂停期延长至 1 月 27 日。

**[BBC 事实查核：纪录显示，特朗普的帐户今年交易了 44 次 Nvidia 股票](https://www.bbc.com/zhongwen/articles/cm62p52417ywo/simp)**（BBC 中文，2026-11-26T13:23:19Z，合 21:23:19 Asia/Shanghai）。BBC 事实查核根据美国总统财务披露材料报道，特朗普的投资组合今年多次交易英伟达股票，稿件写明纪录显示为 44 次。这是对披露文件的核对，不是对交易盈亏或内幕的司法结论，也与公司本身的产品发布无关。

**[香港宏福苑大火一年后：居民受压、媒体噤声，为何悼念也变得小心翼翼？](https://www.bbc.com/zhongwen/articles/cw8dv46pv125o/simp)**（BBC 中文，RSS 时间 Thu, 26 Nov 2026 05:41:40 GMT，合 13:41:40 Asia/Shanghai；页面 published 时间显示 2026-11-24T10:01:57Z）。BBC 中文在火灾一周年前夕采访遗属和新闻工作者：港府官员称「政府绝对容许」合法活动，但有遗属表示悼念受到压力，也有传媒人称相关周年报道在制作完成后「被抽起」。《纽约时报》World RSS 同日也有 [Hong Kong Grieves Fire Victims Under Watchful Eye of Authorities](https://www.nytimes.com/2026/11/26/world/asia/hong-kong-fire-wang-fuk-court-anniversary.html)，摘要写市民默哀 168 名遇难者，官方则警告不要利用灾难制造分裂；正文页 403，细节以 BBC 中文采访为主。

**[九合一选前反转：沈伯洋破天荒取消台北「选前之夜」](https://www.bbc.com/zhongwen/articles/cwz0kymdzdd8o/simp)**（BBC 中文，2026-11-26T13:41:15Z 左右，页面 published 2026-11-26T11:06:46Z，合 19:06:46 Asia/Shanghai）。11 月 25 日晚，民进党台北市长参选人沈伯洋宣布取消原定大型造势，改为线上直播。报道写，这是 1994 年台北市长恢复直选以来，首次有民进党参选人不举办实体选前之夜。导火索是仁爱路封路四天搭建舞台、多条公交改道后的交通投诉；国民党参选人蒋万安阵营表示可把市府路路权「礼让」给对方，沈伯洋竞选总干事回应「市府路我们不会使用」。学者对 BBC 中文表示，取消活动可为交通争议「止血」，但也减少了实体造势凝聚声势的窗口。投票尚未开始，这里只记竞选安排的变化，不预测结果。

美国法院裁定华为共谋窃取商业机密等罪名成立、但敲诈勒索组织罪无罪，BBC 中文 11 月 26 日有综述，与 11 月 25 日早报已写的同一判决重复，本期不展开。开罗油罐车事故造成 31 人死亡后，[埃及当局逮捕一名司机](https://www.bbc.co.uk/news/articles/c3gre90l0g45o)，官员称其承认超车时超速并刮碰到油罐车，作为昨日报道的续报记一笔。加沙地带 11 月 26 日的以色列空袭中，哈马斯政治官员哈立德·阿布·纳达（Khaled Abu Nada）及其妻子等八名巴勒斯坦人死亡，BBC 有报道，属持续冲突中的新伤亡，不在此展开战况复盘。

《纽约时报》World RSS 中，因正文 403、只据标题与摘要可写的还有：英国净移民降至疫情除外、1997 年以来最低，主要因欧盟以外入境减少；欧洲在网络攻击和炸弹威胁之后，「生存主义」进入更多政府的应急宣传；英国公布与爱泼斯坦有关联的前大使曼德尔森（Peter Mandelson）任命相关文件；以及一些巴西人被高薪许诺骗去为俄军作战。这些条目未能核对正文，不作进一步转述。

## 4. Hacker News

当前首页来自 [Algolia 前端接口](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集于 2026-11-27 07:38:57 Asia/Shanghai（UTC+8）。首页仍以昨日已写过的 Scott Aaronson 博文 *Holy shit holy shit holy shit holy shit: The magnitude of what's now happening*（[原文](https://scottaaronson.blog/?p=10379) · [HN](https://news.ycombinator.com/item?id=50646108)，1968 分 / 1797 评）居首，本期不再重写。以下对讨论较多或点数较高、且尚未写入查重档案的条目打开原文，写中文摘要；招聘帖不计入讨论。

**[Intel One Mono font (2023)](https://github.com/intel/intel-one-mono)** · [HN](https://news.ycombinator.com/item?id=50653667) · 448 分 / 234 评 · 2026-11-26 18:11:01 Asia/Shanghai（UTC+8）。这是 2023 年已发布的开源等宽字体再次出现在首页。仓库介绍写，Frere-Jones Type 与英特尔品牌团队合作，针对容易产生视觉疲劳和误读的开发者（包括低视力开发者）做了可读性设计，提供 Light 到 Bold 四档及斜体，覆盖 200 余种拉丁字母语言，许可为开源字体许可。

**[Collection of preserved UI style guides](https://aresluna.org/ui-style-guides/)** · [HN](https://news.ycombinator.com/item?id=50649834) · 402 分 / 93 评 · 2026-11-26 08:40:00 Asia/Shanghai（UTC+8）。设计师 Marcin Wichary 把从 1980 年代初至今的界面风格指南收集到一处，页面标明采集时有 79 份。作者写，不少 PDF 原本散落各处，他按主题和年代分组，有的自己扫描，有的为旧站点做了镜像。条目从 Amiga 的 Intuition/Workbench、Android Material、BlackBerry 等开始，是一份档案型目录，不是新的设计规范发布。

**[Nextcloud Office Desktop app](https://nextcloud.com/blog/euro-office-comes-to-your-desktop-with-the-nextcloud-office-desktop-app/)** · [HN](https://news.ycombinator.com/item?id=50654289) · 390 分 / 199 评 · 2026-11-26 19:50:49 Asia/Shanghai（UTC+8）。Nextcloud 博文介绍桌面端 Office 应用，把在线办公套件接到本地桌面，面向希望把文档留在自建或欧洲云上的用户。这是公司自己的产品发布说明，不是第三方评测。

**[Minipg: PostgreSQL as a Single Executable](https://progrium.github.io/minipg/)** · [HN](https://news.ycombinator.com/item?id=50650892) · 287 分 / 44 评 · 2026-11-26 11:00:48 Asia/Shanghai（UTC+8）。Jeff Lindsay 的项目把 PostgreSQL 收成一个可执行文件：一个 `.pgdb` 目录里放数据、配置、凭证和版本，`minipg app.pgdb` 即可打开 psql。说明写，它嵌入 Docker Hub 的 `postgres:18-alpine` 镜像，用 Zig 库 h9 在宿主上直接跑 Alpine 的 Postgres，不必再起 Linux 内核或 Docker；演示包约 35 MB。页面同时提醒这是实验性做法。

**[Lions' Commentary on Unix: Why It Was Secretly Copied for 20 Years](https://fosscomics.com/posts/17.%20Lions%27%20Commentary%20on%20Unix/)** · [HN](https://news.ycombinator.com/item?id=50651719) · 270 分 / 61 评 · 2026-11-26 13:12:59 Asia/Shanghai（UTC+8）。漫画文章回顾 John Lions 1976 年在新南威尔士大学为 Unix Version 6 内核写的讲义。1979 年 AT&T 收紧 Version 7 许可、限制课程讨论源码后，这本注释的传播也受到严格控制，却在此后约二十年里以私下复制的方式继续流传。文章讲的是这段许可与教学史，不是新发现一份佚失手稿。

**[AMD-specific fork of llama.cpp](https://devnull.land/amd-specific-llama-cpp)** · [HN](https://news.ycombinator.com/item?id=50657265) · 257 分 / 64 评 · 2026-11-26 01:11:29 Asia/Shanghai（UTC+8）次日。作者建议 AMD 显卡用户尝试 `llama-cpp-rdna-boosts`，并给出自己的测速：生成从每秒 35 个 token 提到 55，prefill 从 700 提到 1300，同时写明 YMMV。文章把这类分叉放在 2026 年 11 月大量「针对特定硬件、用前沿模型快速改写」的推理引擎潮流里讨论，并提醒其中不少项目高度依赖自动生成代码，结果需自行验证。上述速度是作者个人环境中的说法。

**[Moat: OpenRouter replacement](https://commandcode.ai/moat)** · [HN](https://news.ycombinator.com/item?id=50652184) · 241 分 / 133 评 · 2026-11-26 14:32:48 Asia/Shanghai（UTC+8）。Command Code 的产品页自称「AI token 界的 Costco」：每月 5 美元即可按批发价使用 100 多个开源模型，并宣称没有用量上限。页面把价格和「会员池汇集用量」作为出品方卖点。这些是营销表述，不是对实际可用性和成本的独立审计。

**[OpenAI may be in cost control mode](https://micjm.com/blog/openai-is-in-cost-control-mode/)** · [HN](https://news.ycombinator.com/item?id=50652527) · 225 分 / 212 评 · 2026-11-26 15:33:12 Asia/Shanghai（UTC+8）。micjm 根据自己的对战评测数据提出一个解释：GPT-6.2 Astra 与 Sol 发布后口碑不佳，可能是因为它们被调成更省成本——相对对手，每个任务的输出 token 和推理 token 都下降了。文章用成本比、Elo 和置信区间作图，并把 6.2 写成相对 6 / 6.1 的离群点。这是该站点基于自有评测的推断，不是 OpenAI 的官方说明。

**[YouTube Ad Punisher – Auto-reloads YouTube pages when an ad plays](https://github.com/antonpictures/youtube-punisher)** · [HN](https://news.ycombinator.com/item?id=50657530) · 210 分 / 295 评 · 2026-11-27 01:36:47 Asia/Shanghai（UTC+8）。浏览器扩展在检测到广告播放时自动刷新页面并尽量保持播放位置。仓库说明把动机写成：传统广告拦截容易被 YouTube 的反广告拦截提示挡住，这个项目改走「让广告无法完整播完」的路。讨论区对是否违反服务条款、以及刷新是否真能绕过检测有争议，这里只介绍项目自述。

**[CTO of 'RansomwareHelp' Indicted for Wire Fraud](https://krebsonsecurity.com/2026/11/cto-of-ransomwarehelp-indicted-for-wire-fraud/)** · [HN](https://news.ycombinator.com/item?id=50657645) · 180 分 / 82 评 · 2026-11-27 01:47:45 Asia/Shanghai（UTC+8）。Brian Krebs 报道，佛罗里达州网站 ransomwarehelp.com 的联合创始人兼技术负责人 Juan Ricardo Palacio Escobar，被指控电汇欺诈。站点曾宣传「不要支付赎金」、自称用专有密码学工具恢复数据且「绝不代客户向攻击者支付」。克雷布斯写，罗德岛联邦大陪审团起诉书及 FBI 诱捕行动显示，该公司实际上向勒索软件组织购买解密密钥，再向受害者加价收费。文章注明起诉不等于定罪。页面日期为 2026-11-20，今日仍在 HN 首页。

**[An algebraic quantization of gravity from the null cone](https://arxiv.org/abs/2611.34924)** · [HN](https://news.ycombinator.com/item?id=50651863) · 192 分 / 66 评 · 2026-11-26 13:37:51 Asia/Shanghai（UTC+8）。Venkatesa Chandrasekaran 2026 年 11 月 25 日提交的预印本（arXiv:2611.34924，hep-th）提出一种在四维洛伦兹时空上、不依赖背景的真空广义相对论量子化方案：在体子区域相交的光锥上求解约束，得到有限牛顿常数下的约化相空间，再把泊松括号提升为对易关系。这是预印本，不是已被社区接受的定论。

**[IBM gives H-1B, green card holders 3 weeks to relocate from US or leave company](https://economictimes.indiatimes.com/nri/work/ibm-gives-h-1b-green-card-holders-3-weeks-to-relocate-from-us-or-leave-company-december-31-deadline-set/articleshow/136180168.cms?from=mdr)** · [HN](https://news.ycombinator.com/item?id=50658170) · 99 分 / 71 评 · 2026-11-27 02:35:37 Asia/Shanghai（UTC+8）。《经济时报》报道，IBM 通知部分持 H-1B 签证和绿卡的美国员工，须在约三周内决定是否迁往其他国家，否则离开公司；选择不搬迁者可获三个月遣散，最后工作日为 2026 年 12 月 31 日。报道称，咨询业务部门将不再为大多数职位担保签证和绿卡，印度可能是主要接收地。这是对该报报道的摘要，不是 IBM 官方声明原文。

其余首页条目（短列表）：

| 标题 | 链接 | 一句中文 | 热度 |
| --- | --- | --- | --- |
| Tell HN: Happy Thanksgiving | [HN](https://news.ycombinator.com/item?id=50655664) | 首页上的感恩节问候帖 | 559 分 / 132 评 |
| Google Will Make AI Agents Use Its MCP Servers. The Gmail One Can't Send Email | [原文](https://techstackups.com/articles/google-workspace-ai-agents-mcp/) · [HN](https://news.ycombinator.com/item?id=50653477) | 讨论 Google 让 Workspace 智能体走自家 MCP，以及 Gmail 接口据称还不能发信 | 198 分 / 184 评 |
| The history of civilization is the history of wheat | [原文](https://asteriskmag.com/issues/16/marginal-grains) · [HN](https://news.ycombinator.com/item?id=50634381) | 从小麦和「边缘谷物」重新看文明史 | 145 分 / 108 评 |
| AI made self-hosting fun again | [原文](https://janlukas.blog/posts/ai-self-hosting) · [HN](https://news.ycombinator.com/item?id=50660180) | 作者写，用编程智能体改 Docker Compose 后，自托管重新变得愿意折腾 | 134 分 / 79 评 |
| Curiosity Is No Solo Act | [原文](https://thereader.mitpress.mit.edu/curiosity-is-no-solo-act/) · [HN](https://news.ycombinator.com/item?id=50636931) | 谈好奇心并非纯粹的个人禀赋 | 115 分 / 28 评 |
| Show HN: Three Linux VMs in a browser tab, each running a different browser | [原文](https://michidk.github.io/sidebyside/) · [HN](https://news.ycombinator.com/item?id=50656036) | 在一个标签页里并排跑三台 Linux 虚拟机和三种浏览器 | 105 分 / 26 评 |
| Discovery of curse ritual in trash dump surprises Egyptologist | [原文](https://phys.org/news/2026-11-discovery-curse-ritual-trash-dump.html) · [HN](https://news.ycombinator.com/item?id=50619466) | 垃圾堆里发现诅咒仪式遗存的考古报道 | 88 分 / 50 评 |
| NormalScript: A perfectly normal scripting language | [原文](https://psychoscript.com/) · [HN](https://news.ycombinator.com/item?id=50651430) | 一套自称「完全正常」的脚本语言项目页 | 67 分 / 12 评 |
| Rvoip 0.5 the complete VoIP stack in Rust | [原文](https://github.com/eisenzopf/rvoip) · [HN](https://news.ycombinator.com/item?id=50658632) | Rust 实现的完整 VoIP 栈 0.5 版 | 60 分 / 13 评 |
| Show HN: Olumino, a Markdown notes and spaced repetition app | [原文](https://olumino.app) · [HN](https://news.ycombinator.com/item?id=50651099) | Markdown 笔记加间隔重复的应用 | 53 分 / 31 评 |
| George Whitesides, 1939-2026 | [原文](https://www.science.org/content/blog-post/george-whitesides-1939-2026) · [HN](https://news.ycombinator.com/item?id=50657936) | 化学家 George Whitesides 的纪念文章 | 46 分 / 6 评 |
| Show HN: SimDrop – Running iOS simulators in the macOS Finder sidebar | [原文](https://github.com/rxliuli/sim-drop) · [HN](https://news.ycombinator.com/item?id=50657070) | 把 iOS 模拟器放到 Finder 侧栏 | 35 分 / 8 评 |
| Largest 2D Chart library in the world using BUI: BlenderUI | [原文](https://bui.preetham.top/charts/) · [HN](https://news.ycombinator.com/item?id=50658193) | 用 BlenderUI 做的二维图表库展示页 | 33 分 / 2 评 |
| Top-cited AI scientists at four US companies compared | [原文](https://topcitedscientists.com/figures/ai-at-four-us-companies/) · [HN](https://news.ycombinator.com/item?id=50658910) | 比较四家美国公司高被引 AI 学者 | 18 分 / 11 评 |
| Novita, StreamLake, etc. are ByteDance Ark wrappers | [原文](https://kendell.dev/blog/arkwrapper/) · [HN](https://news.ycombinator.com/item?id=50660273) | 作者指部分推理服务是字节跳动方舟接口的封装 | 5 分 / 0 评 |
| Kamil Khan Mumtaz: Pakistani architect, admired at home, almost invisible abroad | [原文](https://worksinprogress.co/issue/the-greatest-architect-youve-never-heard-of-is-in-pakistan/) · [HN](https://news.ycombinator.com/item?id=50659841) | 介绍在巴基斯坦受推崇、在国外较少被写到的建筑师 | 180 分 / 31 评 |

招聘帖 Head of Software Engineering – NOX Metals 未计入讨论。

## 5. X 热门与科技圈

全球趋势（WOEID 1）与美国趋势在采集时几乎被 [Thanksgiving](https://x.com/search?q=Thanksgiving)（约 239 万帖）和 NFL（[Bears](https://x.com/search?q=Bears)、[Eagles](https://x.com/search?q=Eagles)、[Lions](https://x.com/search?q=Lions)、[Cowboys](https://x.com/search?q=Cowboys)、[Gibbs](https://x.com/search?q=Gibbs)、[Caleb Williams](https://x.com/search?q=Caleb%20Williams) 等）占满；全球榜另有西班牙辩论话题（[#DebateA4RTVE](https://x.com/search?q=%23DebateA4RTVE)、[Abascal](https://x.com/search?q=Abascal)、[Colau](https://x.com/search?q=Colau)）和 [#FreePalestine](https://x.com/search?q=%23FreePalestine)。中国区趋势接口返回内容与全球高度重合，参考价值有限。

**科技 / AI。** 节日期间，热榜本身几乎没有单独的产品发布词条。X 新闻摘要把讨论焦点放在智能体编排、安全发布节奏和中美模型差距上，但这些摘要带有「可能随帖文演变、需另行核实」的声明，本期只作流传中的话题记录，不当成已核实事实。[Gemini 4 Neon Leads Multi-Agent AI Swarms](https://x.com/i/trending/2125734003978440946) 把 Google Antigravity 上的多代理编排写成开发者正在尝试的工作流，并给出摘要中的排行数字——Gemini 4 Neon 的发布此前早报已经写过，这里不当成新品首发。[OpenAI and Anthropic Staff Question Releasing Powerful AI Models](https://x.com/i/trending/2125304097138262034) 称两家公司有员工担心未发布模型已超过现有安全措施，并提到高规格内控讨论；来源是「内部人士」类转述，未见到两家公司的对等公开声明，只记「在流传」。[US Chip Rules and AI Safeguards Delay Chinese Models to 2027](https://x.com/i/trending/2125650660528210247) 称智谱、月之暗面等把旗舰模型推迟到 2027 年，并提到蒸馏受限和芯片规则——同样未经本期独立核对，不当成各实验室已经宣布的日程。HN 上同期更具体的材料，是 micjm 那篇关于 Astra / Sol「可能在控成本」的评测文，见上一栏。

公开检索里高互动的原创帖不多。有一条把「中国实验室转而蒸馏 Gemini 4 Neon」写成传闻的讨论，例如 [sonuv_dev](https://x.com/sonuv_dev/status/2125981720017268787)，互动量有限，同样只记流传。

## 6. 微博热搜

接口 [weibo.com/ajax/side/hotSearch](https://weibo.com/ajax/side/hotSearch) 于 2026-11-27 07:38:58 Asia/Shanghai（UTC+8）返回成功。置顶政务为 [#总书记寄语中国航天事业#](https://s.weibo.com/weibo?q=%23%E6%80%BB%E4%B9%A6%E8%AE%B0%E5%AF%84%E8%AF%AD%E4%B8%AD%E5%9B%BD%E8%88%AA%E5%A4%A9%E4%BA%8B%E4%B8%9A%23)。带「商」标记的广告或商业推广包括 [广州车展热门新车比亚迪第三代唐](https://s.weibo.com/weibo?q=%E5%B9%BF%E5%B7%9E%E8%BD%A6%E5%B1%95%E7%83%AD%E9%97%A8%E6%96%B0%E8%BD%A6%E6%AF%94%E4%BA%9A%E8%BF%AA%E7%AC%AC%E4%B8%89%E4%BB%A3%E5%94%90)、[全新红旗H9上市](https://s.weibo.com/weibo?q=%E5%85%A8%E6%96%B0%E7%BA%A2%E6%97%97H9%E4%B8%8A%E5%B8%82)，不作为新闻条目。

**摘要与分析。** [从5到24看载人航天之路](https://s.weibo.com/weibo?q=%E4%BB%8E5%E5%88%B024%E7%9C%8B%E8%BD%BD%E4%BA%BA%E8%88%AA%E5%A4%A9%E4%B9%8B%E8%B7%AF) 是神舟二十四号发射和进驻之后的回顾性热度，与前两日早报的官方续报同向，不再展开过程。[全球首个乙肝治愈新药中国获批](https://s.weibo.com/weibo?q=%E5%85%A8%E7%90%83%E9%A6%96%E4%B8%AA%E4%B9%99%E8%82%9D%E6%B2%BB%E6%84%88%E6%96%B0%E8%8D%AF%E4%B8%AD%E5%9B%BD%E8%8E%B7%E6%89%B9) 仅见话题名，本期未打开药品审评或企业公告，不写药名、适应症或「已经治愈」这类结论。[英伟达东南亚停供或影响评级](https://s.weibo.com/weibo?q=%E8%8B%B1%E4%BC%9F%E8%BE%BE%E4%B8%9C%E5%8D%97%E4%BA%9A%E5%81%9C%E4%BE%9B%E6%88%96%E5%BD%B1%E5%93%8D%E8%AF%84%E7%BA%A7) 是市场传闻口吻，未见本期核对的公司或评级机构原文，不当成已宣布的停供。[立陶宛要求台当局更名](https://s.weibo.com/weibo?q=%E7%AB%8B%E9%99%B6%E5%AE%9B%E8%A6%81%E6%B1%82%E5%8F%B0%E5%BD%93%E5%B1%80%E6%9B%B4%E5%90%8D) 属国际政治话题，细节未核到立陶宛官方声明，只记热搜上有这一说法。[中纪委一天连打三虎](https://s.weibo.com/weibo?q=%E4%B8%AD%E7%BA%AA%E5%A7%94%E4%B8%80%E5%A4%A9%E8%BF%9E%E6%89%93%E4%B8%89%E8%99%8E)、[上海百亿养老集资骗局股东潜逃海外](https://s.weibo.com/weibo?q=%E4%B8%8A%E6%B5%B7%E7%99%BE%E4%BA%BF%E5%85%BB%E8%80%81%E9%9B%86%E8%B5%84%E9%AA%97%E5%B1%80%E8%82%A1%E4%B8%9C%E6%BD%9C%E9%80%83%E6%B5%B7%E5%A4%96)、[武大调查谈话238人次](https://s.weibo.com/weibo?q=%E6%AD%A6%E5%A4%A7%E8%B0%83%E6%9F%A5%E8%B0%88%E8%AF%9D238%E4%BA%BA%E6%AC%A1)、[北大教师右眼被注入工业气体获赔388万](https://s.weibo.com/weibo?q=%E5%8C%97%E5%A4%A7%E6%95%99%E5%B8%88%E5%8F%B3%E7%9C%BC%E8%A2%AB%E6%B3%A8%E5%85%A5%E5%B7%A5%E4%B8%9A%E6%B0%94%E4%BD%93%E8%8E%B7%E8%B5%94388%E4%B8%87) 和 [三只松鼠致歉声明](https://s.weibo.com/weibo?q=%E4%B8%89%E5%8F%AA%E6%9D%BE%E9%BC%A0%E8%87%B4%E6%AD%89%E5%A3%B0%E6%98%8E) 都是热度靠前的社会或消费话题，本期未打开通报、判决或企业声明全文，不根据标题写案情或道歉内容。[董明珠称汽车行业有老鼠](https://s.weibo.com/weibo?q=%E8%91%A3%E6%98%8E%E7%8F%A0%E7%A7%B0%E6%B1%BD%E8%BD%A6%E8%A1%8C%E4%B8%9A%E6%9C%89%E8%80%81%E9%BC%A0) 只见话题名，不引申为对某一企业的查实指控。

**速览。** 体育方面，[U17国足8比0斐济](https://s.weibo.com/weibo?q=U17%E5%9B%BD%E8%B6%B38%E6%AF%940%E6%96%90%E6%B5%8E)、[国足回应U17国足8比0斐济](https://s.weibo.com/weibo?q=%E5%9B%BD%E8%B6%B4%E5%9B%9E%E5%BA%94U17%E5%9B%BD%E8%B6%B38%E6%AF%940%E6%96%90%E6%B5%8E) 以及董路、詹俊的评论帖靠前。其余多为综艺、剧集和娱乐，如许飞与厉娜、三只松鼠员工取名、肖战、徐璐、向太继女、JackeyLove 转会传闻、花花复盘等，不展开。

## 7. 油管科技访谈

对照 docs/youtube-sources.md 的频道名单，从各频道 /videos 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。Lex Fridman、Dwarkesh Patel、Y Combinator、Lenny's Podcast、a16z、All-In、No Priors、The Pragmatic Engineer 等频道近一周的节目，多数已在前几期写过。All-In 今天新上线的是拉斯维加斯扑克对局长视频，不是科技访谈，故不写入本栏。因此今天能新写的长访谈很少。

**[How Clay Builds GTM Agents — Jeff Barg, Head of AI](https://www.youtube.com/watch?v=qjPcaZf_plo)**  
Latent Space · 1:12:23 · 发布于 2026-11-26 19:48:59 Asia/Shanghai（UTC+8）。官方简介写，主持人 Swyx 与 Basil 访问 Clay 的 AI 负责人 Jeff Barg：Clay 已从「在表格单元格里填写内容的智能体」走到「能搭整套 GTM 工作流的编码智能体」；简介称，目前约一半的智能体工作发生在 Claude Code 这类外部工具里，而不是只发生在 Clay 自己的智能体中。Barg 的回答被概括为：他们希望在顾客所在的地方与之汇合，并且不希望自家智能体明显强过「Clay + Claude Code」。简介还提到若干出品方口径的数字与情节：线索评估已经饱和约一年，前沿模型更多用在更上层的任务；把数据集里约 4,000 万家公司全部做客户匹配，按他的计算大约只需 1,500 美元；以及 OpenAI 在他们把约 25% 的工程力量投入一个月后、上线前两天取消了 ChatGPT Apps 发布。章节包括 GTM engineer、Avenue 并入 Clay、Claygents 与 Sculptor、何时值得做 post-training、手写的 BullMQ 栈、以及「智能体仍不会调试自己的 traces」。以上均来自节目简介与章节，不编造片中原话；其中的费用、比例和「取消发布」都是节目或出品方的说法。

## 8. 本月阅读与今日书摘

今天是星期五。按 [本月阅读计划](/reading/)，工作日若有预先写好的分期书摘，应写入早报；若当天没有安排章节，则只保留书单和进度，不硬塞新的摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。计划写明下一本是《人件》，但仓库里的分期文稿尚未写入《人件》各工作日的书摘，故本期不编造章节摘要，只保留书单与进度指引。具体安排见仓库 [docs/reading-plan-2026-11.md](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

星期五早上，金融市场终于补上了周四那一组官方数字：人民币中间价略上调，A 股在周三深跌之后几乎走平，黄金则较上一期早报又低了一点。真正把隔夜信息环境拧在一起的，是几条「还在进行中」的外交和安全新闻：泽连斯基对 BBC 把美国的中东重心和对俄施压说得很直白，科威特设施遇袭造成意大利技术人员死亡而伊朗否认，缅甸则公开表示不会执行国际法院裁决中它认为不适当的部分。美国新关税的细节也被写成「对华上限或达 40%」，但生效仍要等咨询和听证，不宜把标题税率当成已经开征。Hacker News 在昨天那组数学稿之后，今天更多是字体、界面档案、单文件 Postgres 和推理引擎分叉这类工具讨论；OpenAI「是不是在控成本」也只是评测站的推断。X 上几乎是感恩节和橄榄球的天下。微博还停在航天回顾、消费纠纷和几条未核到原文的社会话题里。北京市区今早已经到 9.3℃，白天晴，但大风蓝色预警还在。海淀栏是常委会上的具身智能和「十五五」城市更新，昌平则把全市首例商业用地提前续期写到了八达岭奥莱。阅读上，《人月神话》已经读完，下一本《人件》还在等分期书摘写进计划，今天先不硬造章节。若只从今天唯一新写的访谈里留一句，Clay 那期更值得记住的不是 1,500 美元算尽全球公司，而是他们似乎并不打算让自己的智能体，明显强过顾客已经在用的外部工具。
