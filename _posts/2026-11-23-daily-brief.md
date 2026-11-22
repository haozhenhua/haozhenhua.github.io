---
layout: post
title: "早报 · 2026-11-23"
date: 2026-11-23 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-23 07:50:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/23/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 23 日（星期一）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:33 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:33，昌平原文页约在 07:37；X 热榜约在 07:33–07:38，科技圈检索约在其后不久；油管频道页约在 07:33，节目页约在 07:37。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 `feeds.reuters.com` 再次出现 TLS 连接失败，美联社 RSSHub 返回 403，《纽约时报》正文页返回 403，东方财富行情接口返回 502，均已在相应栏目说明。写稿时尚未到 09:15 中间价和 09:30 开盘，人民币中间价与 A 股本期采用 11 月 20 日（星期五）已公布的官方读数。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期一，写稿时官方中间价和开盘价尚未公布，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 `docs/brief-memory/finance-history.json`。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,578.15 美元/盎司 | 较上一期早报（2026-11-22 07:31:38 Asia/Shanghai (UTC+8)）+39.15（+1.11%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 `3578.149902`，报价单位为美元/盎司；`updatedAt` 为 `2026-11-22T23:32:40Z`（合 2026-11-23 07:32:40 Asia/Shanghai）。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,539.00）计算 | 2026-11-23 07:32:40 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7131（11 月 20 日） | 较上一发布日（2026-11-19，6.7128）变动 +0.0003 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-23 07:33:04 返回的最新一条仍是 11 月 20 日的 6.7131；更早记录为 11 月 19 日 6.7128、11 月 18 日 6.7118、11 月 17 日 6.7132、11 月 16 日 6.7141。**本期采用 11 月 20 日已公布中间价**（写稿时尚未到当日 09:15 发布时间）。变化栏按官方上一发布日口径 | 采集 2026-11-23 07:33:04 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.693346 | 较上一期早报（2026-11-20 08:02:32 Asia/Shanghai (UTC+8)）+0.001366（+0.02%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。`time_last_update_utc` 为 Sun, 22 Nov 2026 00:02:32 +0000（合 2026-11-22 08:02:32 Asia/Shanghai），较上一期早报所用的 11 月 20 日那一笔日更已刷新；`time_next_update_utc` 显示为 Mon, 23 Nov 2026 00:35:42 +0000（约合 08:35:42 Asia/Shanghai），采集时尚未到达 | 2026-11-22 08:02:32 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3533.79 | −43.83（−1.23%） | [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 返回：最新价 3533.79，涨跌 −43.83，涨跌幅 −1.23%，昨收 3577.62，开盘 3527.30，最高 3538.27，最低 3500.83，行情时间戳 `20261120161427`（2026-11-20 16:14:27）。[新浪财经](https://hq.sinajs.cn/list=s_sh000001,s_sz399001) 交叉核对价格一致（3533.7929，涨跌 −43.8245），涨跌幅显示为 −1.22%，与腾讯的四舍五入略有差别；本期采用腾讯口径，以便与前几期早报一致。[东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 本次返回 502，故不以它为数值来源。写稿时尚未开盘，**本期采用 11 月 20 日（星期五）收盘价，不是今日盘中或开盘价** | 采集 2026-11-23 07:33:04 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10256.39 | −326.81（−3.09%） | 同上来源：腾讯财经最新价 10256.39，涨跌 −326.81，涨跌幅 −3.09%，昨收 10583.20，开盘 10402.29，最高 10436.04，最低 10256.39，行情时间戳 `20261120161412`（2026-11-20 16:14:12）。新浪财经交叉核对价格与涨跌幅一致 | 采集 2026-11-23 07:33:04 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报回升约 1.11%，报 3,578.15 美元/盎司。市场化参考汇率随接口日更从 11 月 20 日那一笔刷新为 11 月 22 日的 6.693346，较上一期所用读数略升 0.02%。官方中间价本期继续采用 11 月 20 日已公布的 6.7131，较 19 日中间价上调 0.0003；A 股本期采用 11 月 20 日收盘价，上证下跌 1.23%，深成指下跌 3.09%。这些官方数字都不是今日开盘或收盘。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [`/api/weather/view?stationid=54511`](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 `lastUpdate` 为 2026/11/23 06:50；本次采集时间为 2026-11-23 07:33:04 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。预警列表中有一条：北京市气象台 2026 年 11 月 22 日 15 时 30 分发布大风蓝色预警信号。

**当前实况**（`lastUpdate` 2026/11/23 06:50）：气温 4.2℃，体感温度 0.8℃，相对湿度 33%，东北风微风，风速 2.4 米/秒，降水量 0.0，气压 1021.0 百帕。

**今日（11 月 23 日）预报**：白天晴，最高 8℃，西北风 3～4 级；夜间晴，最低 −4℃，西北风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 24 日 | 白天晴，夜间晴 | 7℃ / −3℃ | 白天西南风微风，夜间西南风微风 |
| 11 月 25 日 | 白天晴，夜间晴 | 9℃ / −2℃ | 白天南风微风，夜间北风微风 |
| 11 月 26 日 | 白天晴，夜间多云 | 11℃ / 0℃ | 白天西北风微风，夜间西北风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 `docs/brief-memory/seen.json`。昨日及此前已写过的海淀区党代会安排、人大代表视察、医保钱包 2.0、未名·AI Park、与中国航油签约，以及昌平的南口古树与防火检查、小汤山冬季安全、回龙观消防演练、流村慢阻肺防治、东小口违建处置等，不再重复。今天是星期一：海淀区要闻、政务动态、部门动态和街镇动态列表较上周末没有新的近日稿件，来源较薄，故不把十月或十一月上旬的旧稿凑进目录。昌平则仍有若干上周末前后尚未写入早报的本地稿。

#### 海淀区

海淀区政府要闻栏今早仍未见比上周末更新的近日稿件。列表顶端仍是 11 月 18 日已写过的区党代会召开安排，以及更早的供暖检查、换届选举和未名·AI Park 等已见条目。本期海淀栏从缺，不拿旧闻充数。

#### 昌平区

**[e无界共生·多元融合——2026年「无界共生」昌平区融合教育案例学术交流研讨会举办](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111821140663301/index.html)**。来源：北京昌平 APP，发布于 2026-11-18。稿件称，研讨会在北师大二附中昌平实验学校举办，围绕中小学生心理健康、医教结合和家校社协同，交流融合教育案例。与会者包括区域教育管理者、一线教师和儿童医疗领域专家。北京师范大学昌平附属学校校长王鹏飞在报道中说，身心健康是学校育人的重要一环，学校已通过线上预约做心理干预，并到社区开展免费服务。这是一次区域教育研讨报道，不是对某一学生个案的诊疗结论。

**[三级议事联动 共商地下空间焕新 区政协「京华议事厅」走进史各庄街道领秀慧谷北区](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111821105076103/index.html)**。来源：北京昌平 APP，发布于 2026-11-18。11 月 16 日，区政协「京华议事厅」在领秀慧谷北区召开社区地下闲置空间提升利用协商议事会，区政协主席蒋达峰出席。报道称，议题针对 1 号楼地下一层长期被居民自发当作休闲场地、楼梯构件松动、地面铺装破损等问题；会上居民代表、设计方、物业和区发改委、住建委、消防、生态环境等部门交换意见。稿件把它写成「京华议事厅」、街道「庄庄美谈」与社区「红领行动」的三级联动，强调安全管控和按共识推进，不是已经完工的改造通报。

**[云上梯田揽星宇 溜石港邀您共赴双子座流星雨之约](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112018332278936/index.html)**。来源：北京昌平 APP，发布于 2026-11-20。稿件介绍流村镇溜石港村的冬季星空活动安排：11 月中旬至 12 月 5 日为「初探星野」阶段，每场限 12 组家庭；12 月 12 日至 18 日为双子座流星雨主活动，文中称峰值日预计每小时约 150 颗流星，并联动北京星典影城设立城市观星点；12 月 19 日至 2027 年春节前为「星光长明」阶段。这些场次、名额和「每小时约 150 颗」的说法来自报道本身，不是气象台的正式观测公报。

**[抢抓窗口期 挖蛹护绿家园 龙泽园街道社区开展美国白蛾越冬蛹集中清除行动](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026111912002797930/index.html)**。来源：北京昌平 APP，发布于 2026-11-19。报道写，龙泽园街道近期组织社区、物业和亲子志愿者分批次搜寻美国白蛾越冬蛹。其中龙跃苑东四五社区一次集中行动有 40 余人参加，稿件称累计捡拾越冬蛹 450 余只，并介绍「挖蛹兑换志愿者时长」的做法；龙锦苑二区社区则组织青年志愿者和 20 组亲子家庭，以虫蛹兑换郁金香种球。这些人数和数量来自报道本身。这是社区秋冬季虫害物理防控报道，不是全区虫害统计公报。

## 3. 全球头条

路透社世界新闻 RSS 本次 TLS 连接失败，美联社经由 RSSHub 的源返回 403，这两家不写入正文。《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写，不假装读过全文。

**续报：COP31 未能达成主要政治协议。** 前几期已写过安塔利亚谈判在化石燃料措辞上陷入僵局。 [BBC](https://www.bbc.co.uk/news/articles/cqwy06zrd26lo) 11 月 22 日报道，原定周五结束的谈判延迟到周日，成为历史上最长的联合国气候大会，但最终草案仍未获通过。报道说，文本中没有直接出现 “fossil fuels”，对煤、油、气的唯一间接提及是指向 2023 年 COP28「向远离化石燃料过渡」的表述；欧盟代表、爱尔兰部长 Darragh O'Brien 表示，一份气候协议完全不提化石燃料「是不可接受的」（报道引语为 “unconscionable”）。许多较穷国家则反对文本里缺乏帮助适应升温影响的明确资金承诺。联合国秘书长安东尼奥·古特雷斯称自己「深感失望」，并把责任指向他所说的「强大的化石燃料利益」。BBC 写道，上一次主政治协议以类似方式破裂，是 2009 年的哥本哈根大会。[《纽约时报》RSS](https://www.nytimes.com/2026/11/22/climate/cop31-climate-summit-ends-climate.html) 摘要称，欧洲和易受气候影响的国家拒绝了拟议协议，原因是沙特阿拉伯和其他石油生产国阻拦任何逐步淘汰煤、油、气的表述；该文正文页本次打不开，只根据 RSS 改写。[《卫报》](https://www.theguardian.com/environment/2026/nov/23/cop31-left-chris-bowen-stuck-between-petrostates-and-climate-reality-but-the-failure-to-say-the-f-word-is-not-his-alone) 则从澳大利亚气候与能源部长、谈判主席 Chris Bowen 的角度做分析，不另作独立事实来源。

**[Explosion on Russian ship at Libya port caused by suspected drone attack, officials say](https://www.bbc.co.uk/news/articles/cr894gjz0j0yo)**（BBC，文中标注发布于 2026-11-22 15:50 GMT，合 2026-11-22 23:50 Asia/Shanghai）。利比亚东部政府称，一艘在班加西海军基地停靠、准备补给后返回俄罗斯的船只，于周日黎明发生疑似无人机袭击造成的爆炸，并称没有人员伤亡；莫斯科尚未置评。BBC Verify 根据社交媒体视频做了地理定位，Planet Labs 卫星图像显示班加西港口在 05:47 GMT 有船起火。美国情报公司 Vantor 的高分辨率图像则显示，一艘被其指认为俄罗斯海军 20380 型「守护」级轻护舰 Merkury 的军舰，周六还停在港内，周日大部分船体已倾覆，只剩舰首可见。东部的「全国稳定政府」（GNS）未点名该船，并称正在与俄方协调调查，同时谴责这是对利比亚主权和海事安全的侵犯。报道还写，卫生部门后来接收了另一艘在班加西近海遇袭的商船伤员，伤势较轻、情况稳定。[《卫报》](https://www.theguardian.com/world/2026/nov/22/blast-russian-ship-suspected-drone-attack-benghazi-libya) 写得更具体：官员向美联社称，疑为乌克兰海上无人机，至少四架被拦截、两架击中军舰。卫报同时写明，尚无人宣称负责。乌克兰是否实施袭击，仍有待其官方说明，不把当事方或媒体的判断写成已核实事实。此事与昨日已写过的芬兰湾货船 Sparta II 遇袭不是同一事件。

**续报：韩国教育部长因高考 AI 作弊风波辞职。** [BBC](https://www.bbc.co.uk/news/articles/cw3dgk29d37no) 和[《卫报》](https://www.theguardian.com/world/2026/nov/22/south-korea-education-minister-resigns-after-ai-cheating-scandal-engulfs-university-exams) 11 月 22 日报道，教育部长崔教珍（Choi Kyo-jin）在大学入学考试（suneung）结束后提出辞职，总统李在明已接受。崔教珍对韩联社表示，作为主管部长，「我们未能提前做好准备」的批评他无法回避。教育部称，今年约 50 万名考生中，有 111 人被发现携带未经授权的智能设备。风波在考试前一周升温：去年 4 月税务会计考试第一名韩元锡（Han Won-seok）承认使用微型摄像机把题目传给 AI。卫报还写，官方临时收紧了考场措施，包括阻断公共 Wi-Fi、加倍监考、只用考场提供的橡皮、避免穿带纽扣的衣服，并对举报作弊开出至少 7.5 万美元奖励。这些人数、措施和引语来自上述报道。韩国高考 AI 作弊一事前几期已经写过，这里只补部长辞职和考后披露的设备查获数字。[《纽约时报》RSS](https://www.nytimes.com/2026/11/22/world/asia/korea-csat-exam-ai-cheating.html) 摘要提到考试前两天宣布的手机警报和眼镜检查等措施引发舆论反弹，正文页本次打不开，不展开。

**[Three killed and dozens missing after fire at Indonesian factory](https://www.bbc.co.uk/news/articles/cw8dvg5pgm0eo)**（BBC，文中标注发布于 2026-11-22 06:05 GMT，其后有更新）。报道称，西爪哇万丹省瑟朗（Serang）地区、距雅加达约 50 公里的一家糖果厂周六下午起火。万丹省长 Andra Soni 对媒体说，起火时厂内约有 60 人。BBC 在提要中写至少三人死亡、数十人失踪；同一篇较后的更新则写，截至周日晚间救援人员已找到 24 只装有遗体的袋子，搜救将在周一继续。印尼国家搜救局称已找到 15 名幸存者，另有四人送医，伤情未详。消防官员 Tubagus Machfudz 对 Kompas TV 说，他们 16:30 当地时间接到报警赶到时，大面积已经着火，无法判断厂房防护系统是否正常工作。起火原因尚未确定。[《卫报》](https://www.theguardian.com/world/2026/nov/22/fire-confectionary-factory-indonesia-jakarta) 援引搜救官员，把厂名写作 Fonusa Agung Mulia、地点在锡坎德（Cikande），并写三人死亡、36 人失踪。两家媒体的伤亡数字并不完全一致，这里并列注明，不以其中一条覆盖另一条。

**续报：美国中期选举众议院议席。** [BBC](https://www.bbc.co.uk/news/articles/c6vg29g7dlyno) 报道，民主党人 Chuck Hubbard 在北卡罗来纳州第 5 选区击败任职自 2005 年的共和党众议员 Virginia Foxx。选情于周日被认定，Hubbard 在 99% 计票完成时领先 330 票；Foxx 依法申请重计后于周日承认败选。BBC 写，民主党在本次中期选举中已至少赢得 258 个众议院议席，共和党至少 173 席，仍有 4 场选举待定；两党都从未在 1992 年之后赢过这么多众议院席位，那一年克林顿当选总统、民主党同样拿到 258 席。报道还提到，民主党此前已拿下参议院。阿拉斯加参议员席位等更早结果，前几期已经写过，这里只补这一场接近的北卡席位，以及 BBC 对整体众议院多数规模的统计。

**续报：爱荷华州叠氮化铅爆破。** 昨日 Hacker News 栏已写过美国陆军计划在爱荷华州引爆库存叠氮化铅、原定周五的行动被推迟并面临诉讼。[BBC](https://www.bbc.co.uk/news/articles/cvglrx764gdxo) 11 月 22 日报道，司法部周六向法院提交新文件，称陆军计划不顾无限期暂停的裁决，继续引爆约五吨已降解的炸药，并拟在紧急豁免下于 11 月 24 日前行动。文件写，为准备爆破已拆除存放桶装物的地堡门，材料「更容易受温度变化影响」；并称未来几天气温可能降到 30°F（−1℃）以下，「存在立即发生爆炸的风险」。原定周五的居民撤离建议此前已经发出，新的具体爆破时间政府尚未公布。这是计划与诉讼的最新进展，不是已经实施的起爆通报。

**[China's Spies Set Sights on A.I. Chips Years Before Nvidia Scandal](https://www.nytimes.com/2026/11/21/world/asia/china-nvidia-spy-chips-state-security.html)**（《纽约时报》RSS，2026-11-22 11:03:04 +0000，合 19:03 Asia/Shanghai）。RSS 摘要称，官员表示，中国的间谍机构多年来一直在开展秘密行动，帮助本国公司获取先进 AI 芯片，并收集该领域情报。加州是否调查英伟达芯片流入中国，前几期已经写过；这篇从更早的间谍活动切入，但正文页本次返回 403，只根据 RSS 改写，不假装核对了官员身份或具体案例。

## 4. Hacker News 近期文章

首页来自 [Algolia 前端接口](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集于 2026-11-23 07:33:03 Asia/Shanghai（UTC+8），共 30 条。对讨论最多或最热的若干篇打开了原文；《纽约时报》和 O'Reilly Radar 的正文页返回 403，相应条目只根据标题、RSS 或可打开的页面说明，不假装读过全文。

**[Toyota, Nissan, and Honda to standardize parts to lower costs](https://www.caranddriver.com/news/a74490092/toyota-nissan-honda-standardize-parts-lower-costs/)**（[HN](https://news.ycombinator.com/item?id=50596133)，1164 点，669 则评论）。《Car and Driver》2026-11-20 转述《Automotive News》的报道称，丰田、日产和本田将开始统一部分汽车零部件，以降低生产成本。日本汽车工业协会会长、同时也是丰田副会长的佐藤恒治（Koji Sato）本周在东京记者会上宣布了这一决定。短期内先从钢材统一质量标准、塑料和树脂的一致工艺，以及线束的统一色标开始；协会的长期打算是扩展到更多覆盖整车的部件。报道强调，这三类部件通常不被消费者注意到，因而不应影响各品牌的个性，同时又占生产成本的相当部分。这些是对行业协会宣布内容的转述。

**[Perplexity and Intelligence](https://openai.com/index/perplexity-and-intelligence/)**（[HN](https://news.ycombinator.com/item?id=50601525)，436 点，298 则评论）。OpenAI 首席科学家 Jakub Pachocki 2026-11-22 的文章，讨论的是作为度量的「perplexity」（困惑度），不是搜索公司 Perplexity。他认为，现代 AI 的关键进展来自在大规模数据上训练更好的「压缩器／预测器」，并主张把困惑度（或等价的交叉熵损失）作为比较不同开发者、并讨论共同安全标准的指标。作为第一步，他公布了 OpenAI 内部预训练困惑度的部分读数：在文中所说的当前主要评估数据集上，GPT-3.5 的对数困惑度约为 0.99，构成最初 ChatGPT 的基础；GPT-4 约为 0.91，能够有效使用思维链；当损失降到 0.8 以下，他们看到网络安全和数学等领域出现他称为「变革性」的能力。这些阈值和能力判断是作者的表述，不是第三方复现。

**[The Birds of GTA 6: A Field Guide to Vice City and Leonida's Wildlife](https://www.audubon.org/magazine/birds-of-gta-6-field-guide-vice-city-wildlife)**（[HN](https://news.ycombinator.com/item?id=50602843)，278 点，112 则评论）。Audubon 杂志 2026-11-20 刊登 Nicholas Lund 的文章，页面标题为 *I Tracked Down All 60 Birds in GTA 6: A Birder's Guide to Vice City's Wildlife*。作者写自己在游戏里找齐 60 种鸟，并讨论观察机制以及 Rockstar 的美术「哪些地方是对的」。这是一篇游戏世界里的观鸟笔记，不是对野生动物种群的实地调查。

**[Show HN: I built a game where you are an LLM's subagent](https://github.com/gulivan/worker755)**（[HN](https://news.ycombinator.com/item?id=50599762)，255 点，59 则评论）。开源浏览器游戏 [Worker 755](https://github.com/gulivan/worker755) 的说明页写，玩家扮演一名被 AI「经理」当成子智能体的员工：经理是真实的大模型，会下发任务、检查回报并写出绩效评估；玩家在终端里执行指令，限时约 90 秒。仓库介绍了免费场次、自备 API 密钥，以及沙箱或「遗留生产环境」等选项。这是作者对自己作品的说明。

**[Open Social Web Alliance](https://osw-alliance.net/en/)**（[HN](https://news.ycombinator.com/item?id=50600511)，204 点，203 则评论）。Open Social Web Alliance 的网站把自己定位为推动去中心化、公共利益导向的社交基础设施，技术上提到 ActivityPub、AT Protocol 和用于私信的 Matrix，并用电子邮件的互操作来类比。页面里有一段指向 2028 年、超过 1 亿用户的愿景文字，这是该联盟的主张，不是对当前用户规模的统计。

**[I joined the NTP Pool, but not with my Stratum 1 Pi](https://www.jeffgeerling.com/blog/2026/i-joined-the-ntp-pool/)**（[HN](https://news.ycombinator.com/item?id=50600622)，116 点，29 则评论）。Jeff Geerling 2026-11-17 写，自己把一台公开的 Stratum 2 时间服务器 `ntp-01.jeffgeerling.com` 加入了 [NTP Pool](https://www.ntppool.org/)，其时间来自工作室里的 Stratum 1 服务器；那台 Time Pi 通过 TimeHAT v6 和外置 GNSS 天线，配的是 u-blox ZED-F9T 授时模块。文章也提醒：加入 NTP Pool 的关键是长期在线并提供稳定时间，不一定非要上 GNSS。这是一篇个人实践记录。

**[A Better Vocabulary for Testing](https://alperenkeles.com/posts/vocab-for-testing/)**（[HN](https://news.ycombinator.com/item?id=50594182)，102 点，28 则评论）。Alperen Keleş 认为，单元测试、集成测试、端到端测试等常用词过于含混，主张一套更可操作的分类，并承认自己的讨论偏向随机测试。文中标注的撰写日期是 2025-08-16，今天仍出现在 HN 首页。

**[C++26 is done (again): November 2026 ISO C++ meeting trip report](https://herbsutter.com/2026/11/21/c26-is-done-again-trip-report-november-2026-iso-c-standards-meeting-buzios-brazil/)**（[HN](https://news.ycombinator.com/item?id=50600838)，56 点，31 则评论）。Herb Sutter 2026-11-21 的旅行报告写，ISO C++ 委员会在巴西布济乌斯（Búzios）再次完成了 C++26 的技术工作。三月份一度完成的草案，在随后的国际标准草案（DIS）投票中首次未能一致通过，主要意见集中在合约特性（`pre`、`post`、`contract_assert`）；这次会议处理了这些意见，计划把更新后的 C++26 文件再次交付批准投票。文中还提到，本周另有一些特性被采纳进 C++29 草案。这是委员会会议召集人的行程说明，不是标准已经正式发布。

其余首页条目（短列表）：

- [What Happened to Silicon Valley?](https://www.oreilly.com/radar/what-happened-to-silicon-valley/)（[HN](https://news.ycombinator.com/item?id=50602947)，324 点，170 则评论）：O'Reilly Radar 文章，正文页本次返回 403，只保留标题与讨论链接。
- [Ask HN: Tips for transitioning from web development to embedded/firmware?](https://news.ycombinator.com/item?id=50555002)（104 点，68 则评论）：没有站外原文的讨论帖。
- [A miniature San Francisco with live buses, planes and boats](https://smallsf.com/)（[HN](https://news.ycombinator.com/item?id=50603589)，88 点，35 则评论）：可拖动缩放的旧金山等轴测地图，页面称叠加了实时公交、渡轮、飞机和模拟路面交通。
- [All Delta Flights Through Atlanta Delayed as Automated System Falters](https://www.nytimes.com/2026/11/22/us/delta-flight-delays-system-outage.html)（[HN](https://news.ycombinator.com/item?id=50603232)，80 点，29 则评论）：《纽约时报》报道达美经亚特兰大航班因自动系统故障延误，正文页本次返回 403。
- [Nyx, the Oldest Internet Service Provider](https://nyx.net/)（[HN](https://news.ycombinator.com/item?id=50603465)，71 点，8 则评论）：自称全球最老的互联网服务商之一，免费公共接入，由志愿者运营的 501(c)(3) 非营利组织。
- [Inside PyPy: First Contact with RPython](https://bernsteinbear.com/blog/inside-pypy-first-contact-with-rpython/)（[HN](https://news.ycombinator.com/item?id=50562207)，54 点，7 则评论）：Max Bernstein 2026-11-19 写自己接触 RPython / PyPy 实现工具链的笔记。
- [Agent swarm trying to solve P vs. NP](https://pequalnp.com/)（[HN](https://news.ycombinator.com/item?id=50604314)，47 点，41 则评论）：网站展示一组 AI 智能体在公开攻击 P 对 NP 问题，并写明结论仍是「open」；这是项目自述，不是已解决该问题的证明。
- [Agentics: Mushy Software](https://12gramsofcarbon.com/p/agentics-mushy-software)（[HN](https://news.ycombinator.com/item?id=50556249)，35 点，5 则评论）：讨论用智能体充当灵活的「润滑剂」来连接内部工具，对比传统胶水代码。
- [Advice for Young Researchers](http://togelius.blogspot.com/2026/11/advice-for-young-researchers.html)（[HN](https://news.ycombinator.com/item?id=50546124)，34 点，12 则评论）：原文页本次返回 500，只保留标题与讨论链接。
- [A Beginner's Guide to Local AI with Inkling, Qwen, and Unsloth](https://www.gpupartner.com/blog/beginners-guide-local-ai-inkling-qwen-unsloth)（[HN](https://news.ycombinator.com/item?id=50603845)，107 点，32 则评论）：Jerry James 2026-11-22 写在 Windows 上用开源权重模型搭本地 AI 的入门记录。
- [I did a meditation and it sort of changed my personality?!](https://www.benkuhn.net/meditation/)（[HN](https://news.ycombinator.com/item?id=50603674)，29 点，14 则评论）：Ben Kuhn 关于一次冥想静修的个人记录。
- [Harvard CS 2881R AI Safety](https://boazbk.github.io/mltheoryseminar/)（[HN](https://news.ycombinator.com/item?id=50602153)，25 点，1 则评论）：课程页面。
- [Do Not Accept](https://donotaccept.ai/)（[HN](https://news.ycombinator.com/item?id=50604959)，23 点，18 则评论）：站点汇集与 AI 公司相关的报道与主张，首页第一条是 8 月的路透社旧闻，不把它当成今日新消息。
- [The Usefulness of Useless Knowledge [pdf]](https://www.ias.edu/sites/default/files/library/UsefulnessHarpers.pdf)（[HN](https://news.ycombinator.com/item?id=50604472)，20 点，1 则评论）
- [Assume People Are Not Interested in Your Blog Post](https://danielsada.tech/blog/assume-people-are-not-interested-in-your-blog-post/)（[HN](https://news.ycombinator.com/item?id=50603143)，18 点，10 则评论）
- [The struggle for freedom: How BSD escaped AT&T licensing](https://fosscomics.com/posts/16.%20BSD%20Unix%20Part%206%20-%20The%20Struggle%20for%20Freedom/)（[HN](https://news.ycombinator.com/item?id=50604123)，16 点，4 则评论）
- [GL.iNet Security Notice 2026-11-20](https://www.gl-inet.com/en-us/blogs/blog/glinet-security-notice-2026-11-20)（[HN](https://news.ycombinator.com/item?id=50604988)，14 点，3 则评论）
- [Will the first approved psychedelic become a blockbuster?](https://www.pharmavoice.com/news/race-first-psilocybin-blockbuster-compass-usona/875270/)（[HN](https://news.ycombinator.com/item?id=50603962)，12 点，5 则评论）
- [Localcode, open source agentic coding on your Mac with one command](https://github.com/mjwsolo/localcode)（[HN](https://news.ycombinator.com/item?id=50604540)，4 点）
- [The Gateless Gate 3D](https://frankforce.com/the-gateless-gate-3d/)（[HN](https://news.ycombinator.com/item?id=50574768)，4 点）
- [Cathedral floor emerges in Sudan, revealing one of the biggest medieval churches](https://apnews.com/article/sudan-antiquities-nubia-cathedral-1b16f67da881ee5592de4481ee55c527)（[HN](https://news.ycombinator.com/item?id=50547698)，43 点）：美联社报道，评论数本次接口未返回。
- [Progress map for the Lean formalization of Alessandro Masullo's manuscript](https://claude.ai/artifact/CtQyX8qfYAF822bgHJHHE3)（[HN](https://news.ycombinator.com/item?id=50605045)，27 点）：与近日黎曼猜想形式化讨论相关，但是另一份手稿的进度图，不与 Alpöge 那条续报混写。

## 5. X 热门与科技圈

X 热榜采集于 2026-11-23 07:33 至 07:38 Asia/Shanghai（UTC+8），使用公共趋势接口：全球 WOEID 1、中国 23424781、北京 2151330。以中国和北京 WOEID 查询时，返回结果与全球热榜高度重合，不把它当成一份独立的「中国本地热榜」。

全球热榜几乎被周末赛事和日本假期占满。靠前的是日本的[勤労感謝の日](https://x.com/search?q=%E5%8B%A4%E5%8A%B4%E6%84%9F%E8%AC%9D%E3%81%AE%E6%97%A5)（今天是日本的劳动感谢日）和[連休最終日](https://x.com/search?q=%E9%80%A3%E4%BC%91%E6%9C%80%E7%B5%82%E6%97%A5)，以及 [Steelers](https://x.com/search?q=Steelers)、[Broncos](https://x.com/search?q=Broncos)、[Eagles](https://x.com/search?q=Eagles)、[Ravens](https://x.com/search?q=Ravens)、[Giants](https://x.com/search?q=Giants) 等美式橄榄球词条，还有 [Mets](https://x.com/search?q=Mets)、[Skubal](https://x.com/search?q=Skubal) 等棒球相关词。另有 [Naruto](https://x.com/search?q=Naruto)、[#GHVIPNoche1](https://x.com/search?q=%23GHVIPNoche1) 等娱乐标签。本期未逐一核对赛果，不把热词写成比分公报。

科技和 AI 圈的讨论并不在上述热榜前排。检索近期帖文可以看到两条并行的线索。一条是对 COP31 未能达成协议的消息转发，与全球头条栏一致，这里不重复展开。另一条是开发者圈在传阅 Anthropic 关于压缩智能体工具调用、减少 token 消耗的工程说明。例如 [@0xwhrrari](https://x.com/0xwhrrari/status/2124493122549715437) 一条 11 月 22 日 21:20 Asia/Shanghai 左右的帖文（采集时约 280 次喜欢、2.6 万次浏览）把「token 用量降低约 85%、准确率从 49% 提到 74%」说成该公司已公布的数字。这些比例是社交平台上的转述，本期未打开 Anthropic 原文逐条核对，不当作已独立核验的实验结论。关于英伟达管理层和「间谍」传闻，前几期已标明是流传中的说法，本期仍不把它升格为已核实事实。

## 6. 微博热搜

接口 `https://weibo.com/ajax/side/hotSearch` 在 2026-11-23 07:33:03 Asia/Shanghai（UTC+8）返回成功（`ok=1`）。置顶/政务条目为 [#亚太同行深入人心#](https://s.weibo.com/weibo?q=%23%E4%BA%9A%E5%A4%AA%E5%90%8C%E8%A1%8C%E6%B7%B1%E5%85%A5%E4%BA%BA%E5%BF%83%23)，带「热」标，未见更多正文，只记下它是置顶政务话题。本次实时榜前 40 条未见明确的广告标。

**科技、国际与社会。** [特朗普发APEC合照配文GOAT](https://s.weibo.com/weibo?q=%E7%89%B9%E6%9C%97%E6%99%AE%E5%8F%91APEC%E5%90%88%E7%85%A7%E9%85%8D%E6%96%87GOAT) 仍是深圳峰会的余波，不重复已写过的联合声明；热搜称他把合照配上 “GOAT”，具体发帖内容本期未打开原帖逐字核对。[汇天A868飞行汽车试飞成功](https://s.weibo.com/weibo?q=%E6%B1%87%E5%A4%A9A868%E9%A3%9E%E8%A1%8C%E6%B1%BD%E8%BD%A6%E8%AF%95%E9%A3%9E%E6%88%90%E5%8A%9F) 出现在热搜，本期未核对公司或民航主管部门公告，只作为话题记下，不把标题写成已确认的适航结论。[特斯拉FSDV15安全处理能力提升25倍](https://s.weibo.com/weibo?q=%E7%89%B9%E6%96%AF%E6%8B%89FSDV15%E5%AE%89%E5%85%A8%E5%A4%84%E7%90%86%E8%83%BD%E5%8A%9B%E6%8F%90%E5%8D%8725%E5%80%8D) 是热搜标题里的性能数字，未核对该公司发布说明，只作为流传中的说法。[孩子用AI写小说被说不是自己写](https://s.weibo.com/weibo?q=%E5%AD%A9%E5%AD%90%E7%94%A8AI%E5%86%99%E5%B0%8F%E8%AF%B4%E8%A2%AB%E8%AF%B4%E4%B8%8D%E6%98%AF%E8%87%AA%E5%B7%B1%E5%86%99) 是一条带「新」标的教育和生成式 AI 话题，未见权威调查，不展开细节。[血压这个区间不再视作接近正常](https://s.weibo.com/weibo?q=%E8%A1%80%E5%8E%8B%E8%BF%99%E4%B8%AA%E5%8C%BA%E9%97%B4%E4%B8%8D%E5%86%8D%E8%A7%86%E4%BD%9C%E6%8E%A5%E8%BF%91%E6%AD%A3%E5%B8%B8) 涉及健康口径，本期未打开指南或卫健部门原文，不写成新的医学标准。[A股迎来三大利好](https://s.weibo.com/weibo?q=A%E8%82%A1%E8%BF%8E%E6%9D%A5%E4%B8%89%E5%A4%A7%E5%88%A9%E5%A5%BD) 更像市场传闻式标题，具体读数见金融栏，不把热搜当成官方利好清单。[私闯果园糟蹋水果主播下架所有视频](https://s.weibo.com/weibo?q=%E7%A7%81%E9%97%AF%E6%9E%9C%E5%9B%AD%E7%B3%9F%E8%B8%9F%E6%B0%B4%E6%9E%9C%E4%B8%BB%E6%92%AD%E4%B8%8B%E6%9E%B6%E6%89%80%E6%9C%89%E8%A7%86%E9%A2%91)、[主播糟蹋千斤苹果仅赔6000元](https://s.weibo.com/weibo?q=%E4%B8%BB%E6%92%AD%E7%B3%9F%E8%B8%9F%E5%8D%83%E6%96%A4%E8%8B%B9%E6%9E%9C%E4%BB%85%E8%B5%946000%E5%85%83) 是同一社会事件的不同热搜表述，细节以调查和当事人说明为准，这里不根据标题裁判。

**速览。** 其余靠前条目多为综艺、剧集和体育，如央视主持人假牙、青稚直播、华鼎奖、成毅、朱一龙与赵丽颖、樊振东对阵约内斯库和弗朗西斯卡、阿尔卡拉斯首夺总决赛冠军、利物浦 4 比 0 曼联、IU 演唱会、国乒 U19 男团，以及赵本山女儿、中戏同学当 NPC 等娱乐话题，不展开。

## 7. 油管科技访谈

对照 `docs/youtube-sources.md` 的频道名单，从各频道 `/videos` 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。Lex Fridman、Dwarkesh Patel、Y Combinator、a16z、All-In、No Priors、Latent Space、The Pragmatic Engineer 等频道近一周的节目，多数已在前几期写过；其余未写过的长访谈，发布时间多在 10 天以外。因此今天能新写的条数很少。

**[The new rules of product management in the AI era | Sherif Mansour (Head of AI, Atlassian)](https://www.youtube.com/watch?v=hRtmV1mCBSE)**  
Lenny's Podcast · 1:21:38 · 发布于 2026-11-22 21:30:32 Asia/Shanghai（UTC+8）。官方简介称，嘉宾 Sherif Mansour 是 Atlassian（Jira 与 Confluence 背后的公司）的 AI 与产品工艺负责人，在该公司工作 17 年：他曾是 Confluence 的第一位产品经理，后来成为该公司首位 Distinguished PM，现在同时负责全公司产品管理的工艺，以及 Atlassian 的 AI 产品策略。简介列出的讨论点包括：产品经理的首要工作是建立「共享大脑」；艺术家、科学家与总经理三类产品经理；为什么 AI 时代产品经理岗位仍在增加；Atlassian 为何比以往雇用更多初级人员；以及新任产品经理管理者最常见的错误。章节目录里还有「Atlassian 的 AI builder 实验及其揭示的问题」「吞吐量不再是瓶颈，方向才是」「给 AI 做产品时产品经理真正该做什么」等条目。这些都是节目简介和章节里的议题，不是对某一内部实验数据的独立核实，也不编造他们在节目中说过的话。

## 8. 本月阅读与今日书摘

今天是星期一。按 [本月阅读计划](/reading/)，工作日若有预先写好的分期书摘，应写入早报；若当天没有安排章节，则只保留书单和进度，不硬塞新的摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。计划写明下一本是《人件》，但仓库里的分期文稿尚未写入《人件》各工作日的书摘，故本期不编造章节摘要，只保留书单与进度指引。具体安排见仓库 [`docs/reading-plan-2026-11.md`](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

星期一早上，金融市场还停在上一个交易日：中间价和 A 股仍是周五那组官方数字，黄金则较上一期早报回升了一点。真正把周末推进一步的，是气候谈判的收场。COP31 拖成历史上最长的一届大会，最终仍没能在「要不要写出化石燃料」这件事上达成主协议，这比前两天的「卡在措辞上」又明确了一步。与此同时，班加西港的疑似无人机袭击把战场的边缘再向外推到了地中海，韩国则在高考 AI 作弊风波后换下了教育部长。Hacker News 上最热闹的，一边是丰田、日产、本田要统一那些消费者看不见的零件，一边是 OpenAI 首席科学家把困惑度重新提成衡量「智力基底」的尺子。X 的热榜仍被比赛和日本假期占着，开发者圈则在传阅如何让智能体少消耗一些 token。北京市区今早已经回到零上，但最低气温今晚仍会落到 −4℃；海淀要闻栏这个周一早晨还是空的，昌平则是融合教育、地下空间议事、流星雨和入冬挖蛹这些更贴近社区的事情。阅读上，《人月神话》已经读完，下一本《人件》还在等分期书摘写进计划，今天先不硬造章节。若只从今天唯一新写的访谈里留一句，Mansour 那期更值得记住的不是工具清单，而是简介里反复出现的判断：当吞吐不再是瓶颈，真正要盯住的是方向，以及一个还能被共享的「大脑」。
