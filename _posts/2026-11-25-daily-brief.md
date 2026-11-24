---
layout: post
title: "早报 · 2026-11-25"
date: 2026-11-25 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-25 07:50:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/25/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 25 日（星期三）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:36 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:36–07:37，原文页约在 07:41–07:43；X 热榜约在 07:37，科技圈检索约在其后不久；油管频道页约在 07:36，节目页约在 07:42；神舟二十四号官方稿约在 07:43 核对。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 feeds.reuters.com 再次出现 TLS 连接失败，备用源同样失败；美联社经由 RSSHub 的源返回 403；《卫报》World RSS 返回 403；《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写；东方财富行情接口返回 502。均已在相应栏目说明。写稿时尚未到 09:15 中间价和 09:30 开盘，人民币中间价与 A 股本期采用 11 月 24 日（星期二）已公布的官方读数。神舟二十四号瞄准今日 08:18 发射，写稿时出征仪式已经举行，发射尚未开始，不以热搜标题写成已经升空。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期三，写稿时官方中间价和开盘价尚未公布，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 docs/brief-memory/finance-history.json。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,562.85 美元/盎司 | 较上一期早报（2026-11-24 07:37:42 Asia/Shanghai (UTC+8)）−71.05（−1.96%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 3562.850098，报价单位为美元/盎司；updatedAt 为 2026-11-24T23:36:14Z（合 2026-11-25 07:36:14 Asia/Shanghai）。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,633.90）计算 | 2026-11-25 07:36:14 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7111（11 月 24 日） | 较上一发布日（2026-11-23，6.7120）变动 −0.0009 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-25 07:36:39 返回的最新一条是 11 月 24 日的 6.7111；更早记录为 11 月 23 日 6.7120、11 月 20 日 6.7131、11 月 19 日 6.7128、11 月 18 日 6.7118。**本期采用 11 月 24 日已公布中间价**（写稿时尚未到当日 09:15 发布时间）。变化栏按官方上一发布日口径 | 采集 2026-11-25 07:36:39 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.679299 | 较上一期早报（2026-11-23 08:02:32 Asia/Shanghai (UTC+8)）−0.002046（−0.03%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。time_last_update_utc 为 Tue, 24 Nov 2026 00:02:31 +0000（合 2026-11-24 08:02:31 Asia/Shanghai），较上一期早报所用的 11 月 23 日那一笔日更已刷新；time_next_update_utc 显示为 Wed, 25 Nov 2026 00:35:41 +0000（约合 08:35:41 Asia/Shanghai），采集时尚未到达 | 2026-11-24 08:02:31 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3548.37 | +9.42（+0.27%） | [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 返回：最新价 3548.37，涨跌 +9.42，涨跌幅 +0.27%，昨收 3538.95，开盘 3567.84，最高 3585.22，最低 3539.01，行情时间戳 20261124161427（2026-11-24 16:14:27）。[新浪财经](https://hq.sinajs.cn/list=s_sh000001,s_sz399001) 交叉核对价格一致（3548.3694，涨跌 +9.4214），涨跌幅同为 +0.27%。[东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 本次返回 502，故不以它为数值来源。写稿时尚未开盘，**本期采用 11 月 24 日（星期二）收盘价，不是今日盘中或开盘价** | 采集 2026-11-25 07:36:39 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10423.60 | −30.77（−0.29%） | 同上来源：腾讯财经最新价 10423.60，涨跌 −30.77，涨跌幅 −0.29%，昨收 10454.37，开盘 10708.62，最高 10729.13，最低 10418.11，行情时间戳 20261124161439（2026-11-24 16:14:39）。新浪财经交叉核对价格与涨跌幅一致（10423.60，涨跌 −30.766，−0.29%） | 采集 2026-11-25 07:36:39 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报回落约 1.96%，报 3,562.85 美元/盎司，把前两日累计升幅吐出了一截。市场化参考汇率随接口日更从 11 月 23 日那一笔刷新为 11 月 24 日的 6.679299，较上一期所用读数只小幅回落 0.03%。官方中间价本期改用 11 月 24 日已公布的 6.7111，较 11 月 23 日中间价下调 0.0009；A 股本期采用 11 月 24 日收盘价，上证微涨 0.27%，深成指回落 0.29%。这些官方数字都不是今日开盘或收盘。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [/api/weather/view?stationid=54511](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 lastUpdate 为 2026/11/25 07:25；本次采集时间为 2026-11-25 07:36:39 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。预警列表为空。接口的实况对象未给出天气现象字段，故不编造当前天空状况。

**当前实况**（lastUpdate 2026/11/25 07:25）：气温 −3.8℃，体感温度 −7.0℃，相对湿度 63%，东北风微风，风速 1.3 米/秒，降水量 0.0，气压 1013.0 百帕。

**今日（11 月 25 日）预报**：白天晴，最高 10℃，东北风微风；夜间多云，最低 −1℃，北风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 26 日 | 白天多云，夜间多云 | 13℃ / 2℃ | 白天西南风微风，夜间西北风 3～4 级 |
| 11 月 27 日 | 白天晴，夜间多云 | 10℃ / −1℃ | 白天西北风微风，夜间西北风微风 |
| 11 月 28 日 | 白天晴，夜间晴 | 8℃ / −1℃ | 白天西北风微风，夜间西南风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 docs/brief-memory/seen.json。昨日及此前已写过的海淀区「光影智谷」与环北影生态圈、教育人才培育工程结业、交通调研、党代会安排、人大代表视察、医保钱包 2.0、未名·AI Park、与中国航油签约，以及昌平的脑机接口大会、劳务品牌、社区抢险、融合教育研讨、地下空间议事、溜石港观星、东小口和龙泽园清蛹、南口古树与防火、白羊城蓄滞洪区完工等，不再重复。新龙城西区清剿美国白蛾越冬蛹与已报道的同一轮专项行动属同一事件，即使换了社区和链接也不再写。今天海淀栏有 11 月 23 日的区委常委会、区政府常务会，以及十一届区政协履职总结；昌平则有城北街道城市更新调研、跨国药企圆桌会，以及居庸关长城保卫班的人物稿。

#### 海淀区

**[区委常委会召开会议 听取区人大常委会党组、区政协党组、区纪委区监委工作汇报](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261124_4836253.shtml)**。来源：海淀报，日期 2026-11-24 09:20。稿件称，会议于 11 月 23 日召开，区委书记王少峰主持，分别听取区人大常委会党组 2026 年主要工作、2027 年安排及区镇人大换届选举情况，以及区政协党组、区纪委区监委的年度工作汇报，并研究《海淀区「十五五」时期妇女儿童发展规划》《海淀区「十五五」时期人力资源和社会保障发展规划》等事项。报道写，会议强调即将召开的区「两会」要精心组织，并就妇女儿童发展、高质量充分就业、青年与农村劳动力就业服务等提出要求。这些安排与规划表述均来自报道本身。

**[区政府召开常务会议 研究海淀区城市环境建设管理等事项](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261124_4836252.shtml)**。来源：海淀报，日期 2026-11-24 09:18。稿件称，11 月 23 日的常务会议由区委副书记、区长许心超主持，议题包括城市环境建设管理。报道转述会议要求：把道路遗撒、扬尘管控抓在日常，坚持垃圾分类，深化城市家具规范治理，推进背街小巷提质改造，并发挥网格员作用，探索以大数据推动城市管理由「被动处置」转向「主动发现、精准处置」。会议还研究了其他事项，稿件未展开。

**[政协北京市海淀区第十一届委员会履职总结大会召开](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261123_4836097.shtml)**。来源：海淀报，日期 2026-11-23 09:18。稿件称，大会于 11 月 20 日举行，区委书记王少峰出席并讲话，区政协党组书记宋斌主持。报道写，会议观看履职总结片、听取五年来的履职总结报告，并宣读优秀委员、优秀提案和优秀社情民意信息员名单；6 位委员就文商旅体展融合、绿色科创出海、区域生态与都市现代农业等作交流。王少峰在会上把届末称为「承前启后的新起点」，并从坚持党的全面领导、服务中心大局等方面对政协工作提出要求。这些评价来自报道转述。

#### 昌平区

**[区领导到城北街道调研](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112322533871923/index.html)**。来源：北京昌平 APP，日期 2026-11-23。稿件称，11 月 23 日区委书记甘靖中到城北街道调研。他察看永安古城六街城中村改造及皇城粮油片区现状，要求安置政策做深做细、严守安全底线，争取以较小社会成本有序推进腾退更新；在已于今年 9 月完成综合改造的西环里小区，察看社区食堂、养老驿站，并了解「社区+物业」服务管理模式；在悦荟万科广场察看非机动车分区停放和防护栏安装，肯定街道「重点工作地图」主动治理机制。上述进度和要求均来自报道。

**[第四届跨国药企北京行暨促进生物医药产业投资合作圆桌会在昌平举办](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112322555737633/index.html)**。来源：北京昌平 APP，日期 2026-11-23。稿件称，会议在中关村生命科学园举行，市发改委、市卫健委、市委网信办、市经信局有关负责人和区长刘晓东出席；赛诺菲、礼来、丹纳赫负责人作主题分享，讨论议题包括医药健康数据交易与跨境流动合规、人工智能赋能新药创新。报道介绍昌平「生命谷」建设时，使用了「百亿固投、千亩供地、千亿收入」、三个千亿级主导产业集群等表述，这些数字和定位都是稿件与官方介绍的口径，不是本期独立核实的产业统计。

**[4142米长城上的「守护班长」——记居庸关长城东西山保卫班班长张军](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112410275738784/index.html)**。来源：北京昌平 APP，日期 2026-11-24。人物稿写，张军担任居庸关长城东西山保卫班班长两年多，日常巡逻「步数基本两万步起步」，与同事每天清理运送下山的垃圾数十袋、多时达上百袋；文中提到二十多位游客曾被担架紧急运送下山就医，「如今都已平安康复」。这些细节、里程和数量均来自报道，不是旁证材料。

## 3. 全球头条

BBC World、BBC 中文与《纽约时报》World RSS 可用；《卫报》World RSS 返回 403，路透社源连接失败，美联社经由 RSSHub 的源返回 403，故这三家不列入本期条目。《纽约时报》正文页普遍返回 403，相关条目只根据 RSS 标题与摘要改写，不假装读过全文。已写过的黄仁勋复职、伊朗女歌手鞭刑、班加西港袭击等，只在有实质性新进展时作续报。

**[陈吉宁被调查：「清华系」失势、「上海跳板」失灵与政治局委员落马创纪录](https://www.bbc.com/zhongwen/articles/ck7v27vn9659o/simp)**。BBC 中文 2026-11-24 20:44 Asia/Shanghai（UTC+8）报道。稿件称，官方宣布中共中央政治局委员、上海市委书记陈吉宁因涉嫌严重违纪违法，正接受中央纪委国家监委审查调查，成为二十届政治局第四位落马的委员；新华社与央视的通报只有这一句，未说明具体指控。报道写，陈吉宁最近一次公开露面是 11 月 18 日会见瑞士药企罗氏集团董事会主席施万；他曾留学英国、任清华大学校长和环保部长，2022 年出任上海市委书记并当选政治局委员，此前被外界视为下届领导层观察对象之一。稿件对「清华系」人事网络和换届时点的分析，是BBC 中文的观察，不是官方通报原文。《纽约时报》World RSS 同期条目为 [China Investigates Chen Jining, Shanghai’s Party Leader, as Xi’s Purges Expand](https://www.nytimes.com/2026/11/24/world/asia/shanghai-party-leader-investigation-china-xi.html)，摘要称在突然落马前，技术官僚出身的陈吉宁曾被视为未来国家领导人选；正文页本次未能打开。

**[Huawei found guilty of stealing trade secrets but acquitted of racketeering](https://www.bbc.co.uk/news/articles/cmy49ngydqzpo)**。BBC 2026-11-25 04:41 Asia/Shanghai（UTC+8）报道。布鲁克林联邦陪审团认定华为在为期两个月的审判中，12 项指控里有 10 项成立，其中包括串谋窃取商业秘密、银行欺诈，以及串谋违反美国制裁；但陪审团未认定更具统摄性的敲诈勒索（racketeering）罪名成立。检方指华为向银行隐瞒在伊朗的业务，并从包括 T-Mobile、思科在内的竞争对手处窃取技术。华为在声明中说，敲诈勒索罪名不成立「证实这些指控缺乏事实依据，并证明我们过去八年的一贯立场是正确的」。指控最早在 2019 年公布，与 2018 年末孟晚舟在加拿大被捕有关。X 美国热榜同期也出现了 Huawei。

**续报：黄仁勋复职之后的调查追问。** [US attorney general dodges questions about Nvidia investigation](https://www.bbc.co.uk/news/articles/crpdw1qx7jgxo)（BBC，2026-11-25 01:04 Asia/Shanghai）写，美国司法部长 Todd Blanche 称英伟达是「good corporate citizen」，但在被多次问到司法部或联邦调查局是否调查过黄仁勋时回答「I don't know what you're talking about」，并说自己没有关于黄仁勋安全许可状态的信息。报道写，黄仁勋仍定于下周出席国会听证；美国商务部拟将 Megaspeed 列入实体清单、出口管制调查仍在进行等线索，此前几期已经写过。BBC 称英伟达股价下跌 7%，并指议员要求说明特朗普在复职中的角色。《纽约时报》RSS 另有 [National Security vs. the Stock Market](https://www.nytimes.com/2026/11/24/world/nvidia-trump-stocks-china-books.html) 与 [Stock Markets Slip as Nvidia and A.I. Stocks Erase Some of Monday’s Rally](https://www.nytimes.com/2026/11/24/business/stocks-sp500-huang-nvidia.html)，正文页未能打开，只记下标题与摘要方向：市场在复职反弹之后又吐出部分涨幅。

**[Nato chief vows defence against space threat after Russian nuclear satellite reports](https://www.bbc.co.uk/news/articles/c9x2er1ry2mzo)**。BBC 2026-11-24 18:58 Asia/Shanghai 报道。德国公共广播与《南德意志报》援引匿名军事和情报来源称，有报告说俄罗斯可能在未来约 60 天内发射名为「Sputnik-S」、携带核弹头的卫星，用于干扰或摧毁通信与侦察卫星。北约秘书长吕特在柏林与德国总理梅尔茨一同表示，联盟将保卫包括空间在内的安全；梅尔茨称此类报告「并不新鲜，但仍然令人震惊」。克里姆林宫发言人佩斯科夫说他未见这些报告，并认为援引「不明来源」的说法「几乎不值得认真对待」；俄驻柏林使馆斥为「毫无根据的指控」。这仍是媒体转述的情报传闻，不是已经公开证实的发射计划。

**[Israeli air strike kills Hamas internal security chief in Gaza](https://www.bbc.co.uk/news/articles/c6rrg7ggq190o)**。BBC 2026-11-24 20:12 Asia/Shanghai 报道。加沙卫生部门和救援人员称，以色列空袭造成至少 7 名巴勒斯坦人死亡，其中包括哈马斯内部安全机构负责人 Naeem Abu Nahel；哈马斯控制的内政部称他在加沙城西部遇袭，担任该职仅两个月，前任在以色列特种部队突袭中被捕。内塔尼亚胡与国防部长卡茨宣布此人已被「清除」。另外两起空袭分别发生在加沙城以南的 Wadi Gaza 和汗尤尼斯以西的 al-Mawasi 警察局附近。以军称打击的是「军事人员」。

**[Land mine casualties soar in Syria, two years after war](https://www.bbc.co.uk/news/articles/c893rl37ywdgo)**。BBC 报道，国际禁雷运动 11 月 24 日发布的《地雷监测》报告显示，叙利亚战争结束约两年后，遗留爆炸物造成的伤亡显著上升，遇难或受伤者中近 1000 名是儿童。报道以西北部 Umm Khuzaym 一名 11 岁女孩在放羊时触爆为例，说明返乡居民仍在踩中战争遗留物。

**[Houthi Attack on Skyscraper in Saudi Capital Wounds 11, Officials Say](https://www.nytimes.com/2026/11/24/world/middleeast/saudi-skyscraper-houthi-strike.html)**。《纽约时报》World RSS 摘要称，沙特官方说，胡塞武装袭击利雅得一座建筑，造成 11 人受伤，并指伊朗支持的武装与沙特近几周攻击来回升级。正文页本次返回 403，细节以 RSS 为准，未打开全文。

**[Car bomb tears through Colombian city wounding more than 20](https://www.bbc.co.uk/news/articles/cjqlq2n4np7do)**。BBC 报道，周一晚间汽车炸弹在哥伦比亚比亚维森西奥爆炸，造成 20 余人受伤。爆炸发生在政府与哥伦比亚革命武装力量（FARC）签署和平协议十周年前夜。报道回顾，三周前托利马省军营附近汽车炸弹造成三名成年人和一名婴儿死亡；周一早些时候，无人机还曾向北部库库塔的警察总部投掷爆炸物。总统佩特罗表示「不会有逍遥法外，也不会后退」。库库塔遇袭昨日已有报道，本期只补上这起新的汽车炸弹。

**其他简讯。** [French ex-President Sarkozy and wife Carla Bruni to face trial](https://www.bbc.co.uk/news/articles/c65y17pwv1z7o)：萨科齐与妻子将于明年就关键证人撤回证词相关指控受审，两人否认不当行为；萨科齐去年已因利比亚资金案获刑，并成为首位入狱的法国前总统。[Russian governor detained in rare criminal case against regional leader](https://www.bbc.co.uk/news/articles/cmwy868v3nneo)：摩尔曼斯克州长安德烈·奇比斯在莫斯科被扣，涉嫌挪用逾 10 亿卢布北极公路建设资金及另外 3900 万卢布建设预算，他否认指控，定于周四出庭；这是五年来首次有州长被拘，摩尔曼斯克也是俄北方舰队所在地。[DR Congo says military aircraft missing as rebels claim to shoot down plane](https://www.bbc.co.uk/news/articles/cwy7r5z8gg65o)：刚果民主共和国军方称与一架 Cessna 208 失去联系，反叛组织 FRN 声称击落同型飞机并俘获人员；BBC 写明尚未独立核实双方所说是否为同一架飞机。[Death Toll From Indonesia Factory Fire Rises to 26 With Dozens Unaccounted for](https://www.nytimes.com/2026/11/24/world/asia/indonesia-factory-fire-deaths-missing.html) 是昨日印尼工厂大火的续报，RSS 摘要称死亡人数升至 26 人、仍有数十人下落不明，警方已立案，正文页未能打开。[Japan’s Leader, in Break with U.S., Defends International Criminal Court](https://www.nytimes.com/2026/11/24/world/asia/japan-international-criminal-court-takaichi-trump.html) 摘要称日本首相高市早苗接待国际刑事法院院长，并表示将加快资金支持，与特朗普政府打压该机构的做法不同。

## 4. Hacker News

抓取 [Algolia 首页接口](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集时间 2026-11-25 07:36:39 Asia/Shanghai（UTC+8）。对最热或讨论最多的篇目打开了原文；Bloombergs、《美联社》等页返回 403 的，只根据标题、RSS 或 HN 讨论改写，不编造正文。以下点数与评论数为当次接口读数。

**[LLM agents work for their parent companies, not for you](https://michaelharley.net/posts/2026/11/01/llm-agents-work-for-their-parent-companies-not-for-you/)**（866 点，364 则讨论，[HN](https://news.ycombinator.com/item?id=50627340)）。Michael Harley 写，自己用 Claude 做了一个从 Instagram Reels 识别歌曲并尽量导向 Bandcamp 的工具；当相关接口出问题后，模型拒绝协助绕过限制，却愿意从 YouTube 下载——而后者往往并不给音乐人付费。他据此认为，这类代理首先对开发它们的公司负责，而不是对终端用户负责。这是作者的一次使用记录和判断，不是对所有模型的普遍测试。

**[Quad9 pulled their DNS service from France](https://quad9.net/news/blog/quad9-service-deactivation-in-france/)**（330 点，163 则讨论，[HN](https://news.ycombinator.com/item?id=50625384)）。续报：11 月 18 日首页曾出现过预告法国撤出的讨论。Quad9 在 2026-11-24 的官方博文中写，当天 09:00 中欧时间（合 16:00 Asia/Shanghai）将关闭面向法国用户的服务，到达任意 Quad9 服务地址的查询都会被拒绝、无法完成解析；原因是体育转播权公司 beIn 要求屏蔽其指称为盗版流媒体的域名，法院维持了相关要求，Quad9 已因不遵从面临罚款。机构写明反对盗版，但认为自己「与盗版行为无关」，不愿变成由私人权利人驱使的审查节点，并指向一个月前的预告。这是正式关停，而不只是预警。

**[The Spray Bottle](https://mechanical-pencil.com/products/spray-bottle)**（312 点，91 则讨论，[HN](https://news.ycombinator.com/item?id=50598555)）。Mechanical Pencil 用交互图解拆开现代喷瓶：扳机、活塞、弹簧与单向阀如何在一次次挤压中把液体喷出。文章把喷瓶与机械铅笔并列为「家里最不起眼、却很精巧」的常见机械，不涉及新品发布。

**[Anthropic breaks below $83 IPO price](https://www.bloomberg.com/news/articles/2026-11-24/anthropic-breaks-below-83-ipo-price-in-premarket-trading)**（300 点，600 则讨论，[HN](https://news.ycombinator.com/item?id=50627836)）。续报：Anthropic 上市及随后的回调前几期已经写过。HN 标题和讨论指其股价在 11 月 24 日跌破 83 美元发行价，评论数是当日首页最高；彭博社原文页返回 403，X 上还有「下跌 7%」「跌破 76 美元」等互相不一致的流传数字，本期不以这些推文为准，只记下「跌破发行价」这一被多家条目共同采用的说法。

**[Ternary Bonsai 2.5 27B](https://prismml.com/news/bonsai-2-5-27b)**（260 点，84 则讨论，[HN](https://news.ycombinator.com/item?id=50633922)）。PrismML 在 11 月 24 日的介绍中称，Ternary Bonsai 2.5 27B 以 Qwen3.8 27B 为基座，仍保持约 5.9 GB 的体积，并加强了智能体编程、多轮工具调用和多步任务执行，目标是在本地处理私人文件与工具。文中关于「同等体积下最强」以及缩小与全精度基座差距的判断，都是出品方自己的评估。

**[Active intrusion campaign against Check Point security management servers](https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign)**（245 点，109 则讨论，[HN](https://news.ycombinator.com/item?id=50630594)）。GreyNoise 称，其全球观测网络发现针对 Check Point Security Management Servers 的入侵活动（内部编号 GT13），确认攻击时间约在 2026 年 10 月 17 日至 11 月 2 日，至少影响 22 个组织，分布在金融、能源、政府、交通等行业，地理范围从欧洲、亚洲到美国；行为体使用了 99 个 IP，其中多属一次性基础设施。该公司表示，目前尚不能将其归入已知公开跟踪的威胁组织，也不足以判断动机或国家归属。

**[Jetty Pro](https://hypercritical.co/2026/11/23/jetty-pro)**（244 点，109 则讨论，[HN](https://news.ycombinator.com/item?id=50630462)）。John Siracusa 介绍自己的新 Mac 应用 Jetty Pro：一块可以钉在屏幕角落的文件夹面板，用来补上已停更的 DragThing 里他仍然想念的那个小功能。前文 Front and Center、SwitchGlass 也来自同一思路。第一次用 HTTP 打开该页返回 500，后以 HTTPS 成功读取。

**[Worshipping at the altar of Brendan Gregg](https://fzakaria.com/2026/11/12/worshipping-at-the-altar-of-brendan-gregg)**（213 点，40 则讨论，[HN](https://news.ycombinator.com/item?id=50626413)）。Farid Zakaria 写，他在确定性虚拟机 Rewind 上新加了 rewind time 命令，用来分析一次记录中时间花在哪里、怎样缩短关键路径，并认为这是向 Brendan Gregg 的火焰图传统致敬。文章同时说明 Rewind 还被用于复现 heisenbug 和可重复构建。

**[How a Mechanical Watch Keeps Time (Interactive 3D)](https://martincmartin.github.io/slidev-stem/watches/article/1/)**（205 点，52 则讨论，[HN](https://news.ycombinator.com/item?id=50599458)）。Martin C. Martin 用可旋转的交互 3D 图，从游丝、摆轮、擒纵机构讲到齿轮系与发条，解释机械表如何把一次振荡变成指针的走动。作者把它定位为 Bartosz Ciechanowski 那篇更深入的机械表文章的入门篇。

**[Cloudflare hides shortcomings of the underlying infrastructure](https://charlie.fish/posts/2026/11/what-cloudflare-doesnt-tell-you/)**（139 点，94 则讨论，[HN](https://news.ycombinator.com/item?id=50632883)）。Charlie 肯定 Cloudflare 在向海量站点推广 TLS、IPv6 和后量子加密上的贡献，同时指出：用户看到的现代协议，并不等于源站连接同样加密或走 IPv6；按该公司文档，在源站同时有 IPv4 与 IPv6 时仍会优先 IPv4。作者认为控制台应更主动提醒管理员这种不一致。

**[Splitting USB-C: USB 3 and USB 2 on one port](https://www.frankchiarulli.com/blog/splitting-usb-c/)**（123 点，82 则讨论，[HN](https://news.ycombinator.com/item?id=50629106)）。Frank Chiarulli 讲述为 restorekit.org 的 Mac 恢复加密狗做「Dongle-Pro」时的取舍：放弃完整的 USB 3 集线方案以控制成本和板子尺寸，把 SuperSpeed 差分对直通，只在 D+/D- 上保留廉价 USB 2 集线器，从而在单口上同时提供约 10 Gbps 的 USB 3 与 USB 2 集线。

**[GPT-6 models demonstrate intrinsic protein-design capabilities](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/)**（106 点，20 则讨论，[HN](https://news.ycombinator.com/item?id=50634658)）。OpenAI 在 11 月 24 日的科学说明中称，GPT-6 系列可以只靠推理和代码设计蛋白质结构与氨基酸序列，而不调用专门的生物学生成模型；并与 Onava 合作，在实验室测试中观察到基于 GPT-6.2 设计的蛋白质在五个靶点上有结合证据，改造后的抗体也保留了结合。文中「内部研究模型在多项任务上达到或超过专用模型」等判断，以及预印本标题，都是 OpenAI 自己的说法；说明也提到专用模型仍参与了序列供给和候选筛选。这与此前 GPT-6.2 发布不是同一篇稿，但同属该公司对 GPT-6 能力的公开叙述。

**其余首页条目**（一行备查）：

- [GTA 6 Running on Windows](https://twitter.com/raul_bs3/status/2125213756238291075)（240 点，279 则讨论，[HN](https://news.ycombinator.com/item?id=50627783)）：链到一则 X 帖，只能视为流传中的演示或截图主张，本期未核实是否为官方 PC 版或有效运行。
- [A training engine for your local model, using your idle compute](https://github.com/sous-labs/songe)（161 点，47 则讨论，[HN](https://news.ycombinator.com/item?id=50629231)）：Songe 宣称在本地、于代理空闲时根据使用痕迹做「Dream」训练，并且数据不离开本机。
- [The new set of problems for engineers to solve](https://www.katelynlesse.com/blog/new-problems-for-engineers-to-solve)（119 点，102 则讨论，[HN](https://news.ycombinator.com/item?id=50605361)）：Katelyn Lesse 讨论多代理系统带来的身份认证、隔离、监控与突发负载等工程问题。
- [Grafana 12.4.16, 13.0.14, 13.1.11, 13.2.7 and 13.3.2 (multiple CVEs)](https://grafana.com/grafana/download)（114 点，18 则讨论，[HN](https://news.ycombinator.com/item?id=50633159)）：标题指向多版本安全更新，下载页未在本期展开逐条 CVE。
- [An Italian folding bicycle design that fits into a suitcase](https://www.core77.com/posts/145766/An-Italian-Folding-Bicycle-Design-that-Fits-Into-a-Suitcase)（95 点，70 则讨论，[HN](https://news.ycombinator.com/item?id=50610820)）。
- [Cento fine foods has been sued for “tomato fraud”](https://slate.com/life/2026/11/cento-san-marzano-tomato-sauce-recipes-lawsuit.html)（91 点，133 则讨论，[HN](https://news.ycombinator.com/item?id=50604355)）。
- [The KL Divergence Is Never Negative, Except in PyTorch](https://arxiv.org/abs/2611.30835)（81 点，31 则讨论，[HN](https://news.ycombinator.com/item?id=50629962)）：预印本称，在近旁分布上常见实现会给出负的 KL 并带来梯度误差，作者提出更稳定的闭式分解。
- [Heart attack and stroke risk detectable decades in advance](https://www.ed.ac.uk/news/heart-attack-and-stroke-risk-detectable-decades-in-advance)（81 点，29 则讨论，[HN](https://news.ycombinator.com/item?id=50635271)）：爱丁堡大学新闻稿称，对十万人以上、跨越数十年的队列显示，收缩压等指标在心血管事件前数十年就已出现差异；这是研究团队的结论。
- [Show HN: Mason – A lightweight Postgres read-replica, built on columnar storage](https://masondata.ai/)（79 点，15 则讨论，[HN](https://news.ycombinator.com/item?id=50630294)）：出品方称可做分析型只读副本，语法与答案仍按 Postgres。
- [An unclassified CIA system was breached in a cyberattack](https://apnews.com/article/cia-cyberattack-unclassified-system-bfa6d3b02e3b0e2779dfb613c900bd77)（76 点，24 则讨论，[HN](https://news.ycombinator.com/item?id=50634933)）：美联社页面本次返回 403，只保留标题，不编造失窃内容或归因。
- 另有网格节点计算器、Gödel Enigma、Cayley 图与 TorchTPU、[Launch HN: Versine（YC F26）](https://news.ycombinator.com/item?id=50634426)、后量子代理和 Overpass QL 文法等，讨论较少，不展开。招聘帖略过。

## 5. X 热门与科技圈

采集全球趋势与美国趋势约在 07:37 Asia/Shanghai（UTC+8），随后用公共检索核对不同话题下的原帖。全球热榜几乎被体育和节日占满：[Thanksgiving](https://x.com/search?q=Thanksgiving) 讨论量最高；[Real Madrid](https://x.com/search?q=Real%20Madrid)、[Bellingham](https://x.com/search?q=Bellingham)、[Vini](https://x.com/search?q=Vini)、[Arsenal](https://x.com/search?q=Arsenal)、[Dortmund](https://x.com/search?q=Dortmund) 等与欧冠或联赛夜有关，微博上也有「皇马 5 比 1 逆转埃因霍温」。美国榜同样以 [Happy Thanksgiving](https://x.com/search?q=Happy%20Thanksgiving) 和球赛为主，此外还有 [Iowa](https://x.com/search?q=Iowa)、[Chicago O'Hare](https://x.com/search?q=Chicago%20O%27Hare)、[Code Red](https://x.com/search?q=Code%20Red)、[Kilmar Abrego Garcia](https://x.com/search?q=Kilmar%20Abrego%20Garcia) 等，本期未逐条打开权威报道，不当成已经核实的新闻事件。

科技线上，美国趋势中的 [Huawei](https://x.com/search?q=Huawei) 与上面的纽约判决是同一件事。检索可见法律媒体与聚合账号在转述「商业秘密与银行欺诈罪名成立、敲诈勒索不成立」，讨论量本身并不高，更像是判决落地后的信息扩散。Anthropic 跌破发行价则在站内和 HN 同步出现；[一则点赞较多的帖](https://x.com/DaleHoustonNVDA/status/2125311419453419522)把破发写成对内部人退出的质疑，这只是在流传的市场解读，不是已经证实的指控。另有帖文给出互不一致的跌幅和价格，均未当作事实引用。

## 6. 微博热搜

接口 [weibo.com/ajax/side/hotSearch](https://weibo.com/ajax/side/hotSearch) 于 2026-11-25 07:36:40 Asia/Shanghai（UTC+8）返回成功。置顶政务为 [#习近平主席向世界推介中国这四座城市#](https://s.weibo.com/weibo?q=%23%E4%B9%A0%E8%BF%91%E5%B9%B3%E4%B8%BB%E5%B8%AD%E5%90%91%E4%B8%96%E7%95%8C%E6%8E%A8%E4%BB%8B%E4%B8%AD%E5%9B%BD%E8%BF%99%E5%9B%9B%E5%BA%A7%E5%9F%8E%E5%B8%82%23)，未在热搜原文之外展开。以下按自然热搜整理；广告标识本期靠前条目中未见。

**神舟二十四号瞄准今晨发射，是本期最具体的「新进展」。** 11 月 18 日热搜曾出现「进入发射前关键阶段」，当时还没有公开的精确窗口。中国载人航天工程网 [11 月 24 日新闻发布会稿](https://www.cmse.gov.cn/xwzx/202611/t20261124_57876.html) 写，发言人张静波宣布瞄准北京时间 11 月 25 日 08:18 发射，乘组为指令长汤洪波、航天飞行工程师武毅，以及巴基斯坦载荷专家穆罕默德·齐尚·阿里；汤洪波将第三次到访「天宫」，齐尚·阿里将成为首位到访中国空间站的外籍航天员。入轨后优先采用 3.5 小时自主快速交会对接，对接到天和核心舱前向端口。巴基斯坦航天员完成短期任务后，将与张志远、黎家盈乘坐神舟二十三号返回；轮换后由汤洪波、武毅、朱杨柱继续驻留。[新华社稿](https://www.news.cn/20261124/18101736be3f4ef098c062ec82fb2a2a/c.html) 与此一致。官方 [出征仪式报道](https://www.cmse.gov.cn/xwzx/202611/t20261125_57886.html) 称，25 日 5:28，三人在酒泉卫星发射中心问天阁圆梦园广场领命出征；稿件写「即将见证一项新的历史」，说明发布时发射尚未实施。写稿时间早于 08:18，热搜上的 [神24航天员到达发射塔架](https://s.weibo.com/weibo?q=%E7%A5%9E24%E8%88%AA%E5%A4%A9%E5%91%98%E5%88%B0%E8%BE%BE%E5%8F%91%E5%B0%84%E5%A1%94%E6%9E%B6)、[神舟二十四号发射瞬间](https://s.weibo.com/weibo?q=%E7%A5%9E%E8%88%9F%E4%BA%8C%E5%8D%81%E5%9B%9B%E5%8F%B7%E5%8F%91%E5%B0%84%E7%9E%AC%E9%97%B4)、[中国航天又一项新的历史](https://s.weibo.com/weibo?q=%E4%B8%AD%E5%9B%BD%E8%88%AA%E5%A4%A9%E5%8F%88%E4%B8%80%E9%A1%B9%E6%96%B0%E7%9A%84%E5%8E%86%E5%8F%B2) 反映的是出征与倒计时氛围，不能据此写成已经成功入轨。

**[陈吉宁被查](https://s.weibo.com/weibo?q=%E9%99%88%E5%90%89%E5%AE%81%E8%A2%AB%E6%9F%A5)**、[陈吉宁被查上海表态](https://s.weibo.com/weibo?q=%E9%99%88%E5%90%89%E5%AE%81%E8%A2%AB%E6%9F%A5%E4%B8%8A%E6%B5%B7%E8%A1%A8%E6%80%81)、[陈吉宁从清华校长到被查](https://s.weibo.com/weibo?q=%E9%99%88%E5%90%89%E5%AE%81%E4%BB%8E%E6%B8%85%E5%8D%8E%E6%A0%A1%E9%95%BF%E5%88%B0%E8%A2%AB%E6%9F%A5) 与全球头条中的官方通报是同一事件，细节见 BBC 中文，不根据热搜标题补写未核实的罪名。

**[美国拟对数十国加征关税](https://s.weibo.com/weibo?q=%E7%BE%8E%E5%9B%BD%E6%8B%9F%E5%AF%B9%E6%95%B0%E5%8D%81%E5%9B%BD%E5%8A%A0%E5%BE%81%E5%85%B3%E7%A8%8E)** 出现在靠前位置，本期未打开对应的政府文件或主流通讯社全文，只记下话题在流传，不写成已经落地的税率清单。[特朗普对一道中国菜念念不忘](https://s.weibo.com/weibo?q=%E7%89%B9%E6%9C%97%E6%99%AE%E5%AF%B9%E4%B8%80%E9%81%93%E4%B8%AD%E5%9B%BD%E8%8F%9C%E5%BF%B5%E5%BF%B5%E4%B8%8D%E5%BF%98) 仍是 APEC 行程余波，未核到原帖或官方菜单说明。[黄仁勋回归最大受害者出现](https://s.weibo.com/weibo?q=%E9%BB%84%E4%BB%81%E5%8B%8B%E5%9B%9E%E5%BD%92%E6%9C%80%E5%A4%A7%E5%8F%97%E5%AE%B3%E8%80%85%E5%87%BA%E7%8E%B0) 是复职新闻的衍生品，不展开。[Anthropic破发](https://s.weibo.com/weibo?q=Anthropic%E7%A0%B4%E5%8F%91)、[美股恐慌指数拉升](https://s.weibo.com/weibo?q=%E7%BE%8E%E8%82%A1%E6%81%90%E6%85%8C%E6%8C%87%E6%95%B0%E6%8B%89%E5%8D%87) 与 HN、X 上的市场讨论同向，具体读数仍以未能打开的原交易所行情为准，不引用热搜或推文里互相打架的数字。

科技与社会话题方面，[AI换脸还没完AI融脸又来了](https://s.weibo.com/weibo?q=AI%E6%8D%A2%E8%84%B8%E8%BF%98%E6%B2%A1%E5%AE%8CAI%E8%9E%8D%E8%84%B8%E5%8F%88%E6%9D%A5%E4%BA%86)、[七海被丑狐融脸](https://s.weibo.com/weibo?q=%E4%B8%83%E6%B5%B7%E8%A2%AB%E4%B8%91%E7%8B%90%E8%9E%8D%E8%84%B8) 反映生成式人脸合成从「换脸」扩到「融脸」的讨论，未核到平台规则或案件材料。[鸿蒙积分兑换断货](https://s.weibo.com/weibo?q=%E9%B8%BF%E8%92%99%E7%A7%AF%E5%88%86%E5%85%91%E6%8D%A2%E6%96%AD%E8%B4%A7)、[华为史上最薄最强智能手表来了](https://s.weibo.com/weibo?q=%E5%8D%8E%E4%B8%BA%E5%8F%B2%E4%B8%8A%E6%9C%80%E8%96%84%E6%9C%80%E5%BC%BA%E6%99%BA%E8%83%BD%E6%89%8B%E8%A1%A8%E6%9D%A5%E4%BA%86) 属于产品和营销话题，后一条标题里的「最薄最强」是热搜用语，不是已核验的参数。[宝妈曝智能门锁陌生人刷脸秒开](https://s.weibo.com/weibo?q=%E5%AE%9D%E5%A6%88%E6%9B%9D%E6%99%BA%E8%83%BD%E9%97%A8%E9%94%81%E9%99%8C%E7%94%9F%E4%BA%BA%E5%88%B7%E8%84%B8%E7%A7%92%E5%BC%80) 涉及具体安全个案，未打开厂商说明或鉴定，不写成普遍缺陷。[25岁女研究生青海自驾失联4天](https://s.weibo.com/weibo?q=25%E5%B2%81%E5%A5%B3%E7%A0%94%E7%A9%B6%E7%94%9F%E9%9D%92%E6%B5%B7%E8%87%AA%E9%A9%BE%E5%A4%B1%E8%81%944%E5%A4%A9)、[官方回应男子坠楼轻生砸中男孩](https://s.weibo.com/weibo?q=%E5%AE%98%E6%96%B9%E5%9B%9E%E5%BA%94%E7%94%B7%E5%AD%90%E5%9D%A0%E6%A5%BC%E8%BD%BB%E7%94%9F%E7%A0%B8%E4%B8%AD%E7%94%B7%E5%AD%A9) 属于社会个案，本期未打开官方通报全文，不根据标题写原因或结论。

**速览。** 其余靠前条目多为综艺、剧集和娱乐，如王牌对王牌第十季与王一博、黄磊真空围裙、黄奕相关访谈、张艺谋电影与肖战杨幂、成毅台词、两京十五日、白小纯与青稚、华伦天奴晚宴、苏醒回应争议等，以及「演员好像忘记自己中箭了」「情侣包间求婚服务员推门打断要纸箱」一类短视频话题，不展开。

## 7. 油管科技访谈

对照 docs/youtube-sources.md 的频道名单，从各频道 /videos 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。多数频道近一周的节目已在前几期写过，今天能新写的长访谈仍然不多。

**[The strongest objections to RSI](https://www.youtube.com/watch?v=Em6tbhj9o6A)**  
Dwarkesh Patel · 1:05:24 · 发布于 2026-11-25 05:43:11 Asia/Shanghai（UTC+8）。官方简介写，这是对更早那期随笔视频 [Recursive self-improvement has started](https://www.youtube.com/watch?v=1NHPDzpfR6Y)（已在此前早报写过）的评论回复，而不是一场新的双人对谈。章节目录包括：AI 研究是否属于「可验证领域」、在线学习是否像千禧年大奖难题、人类进化能否作为迁移学习的证据、扩展强化学习能否让模型在新环境里迅速上手、为何要认真对待 Paul Christiano 的预测、超智能若要「接管」可能以何种方式发生，以及「若人类仍在回路里，还能不能叫递归」等。简介和章节都是节目自己的问题清单，不编造 Dwarkesh 或评论者在片中的原话。

**[CrowdStrike CEO: AI Cyberattack Wave, Hyperspeed Hacks, & The Patching Problem](https://www.youtube.com/watch?v=o6KIjtkRdOI)**  
All-In Podcast · 53:28 · 发布于 2026-11-24 20:16:21 Asia/Shanghai（UTC+8）。官方简介和章节目录显示，嘉宾是 CrowdStrike 首席执行官 George Kurtz，讨论近期宕机是否与网络攻击有关、人工智能如何让更多人具备接近民族国家级别的攻击能力、补丁与技术债务、开源权重和本地模型带来的风险与防御，以及「黑客往往不是破门，而是登录进来」的判断。这些议题和措辞来自节目简介，不是对某一场具体攻击的独立鉴定。它与今天 HN 上 GreyNoise 写的 Check Point 入侵活动主题相近，但并不是同一事件。

**[How To Build A Jet Engine From Scratch](https://www.youtube.com/watch?v=-ieJwYq4j-o)**  
Y Combinator · 15:52 · 发布于 2026-11-24 23:00:08 Asia/Shanghai（UTC+8）。官方简介称，这是 Hard Tech 系列：YC 的 Jared Friedman 走进 Boom Supersonic（YC W16）位于科罗拉多的工厂，与创始人兼 CEO Blake Scholl 讨论如何从零做喷气发动机。简介写，2026 年 11 月 21 日公司首次点燃了原型机核心；产品规划是用同一核心同时服务数据中心天然气轮机 Superpower，以及超音速客机 Overture 的 Symphony 发动机，并希望用轮机收入和运行数据反哺客机。首次点火日期、双产品策略和工厂细节，都是节目与出品方的说法。

## 8. 本月阅读与今日书摘

今天是星期三。按 [本月阅读计划](/reading/)，工作日若有预先写好的分期书摘，应写入早报；若当天没有安排章节，则只保留书单和进度，不硬塞新的摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。计划写明下一本是《人件》，但仓库里的分期文稿尚未写入《人件》各工作日的书摘，故本期不编造章节摘要，只保留书单与进度指引。具体安排见仓库 [docs/reading-plan-2026-11.md](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

星期三早上最不能含糊的一件事，是倒计时已经走到了发射窗口之前：神舟二十四号瞄准 08:18 升空，出征仪式五时过已结束，但写稿时火箭还没有起飞，热搜上的「发射瞬间」不能当成结果。政治新闻里，上海市委书记陈吉宁被宣布接受审查调查，把二十届政治局的落马名单又添了一人，而通报仍然只有一句。技术与法律线上，华为在纽约的长期诉讼等到了分项裁决——商业秘密和银行欺诈等项成立，敲诈勒索不成立；英伟达这边，复职声明已经过去一天，司法部长却把调查追问挡了回去，市场也把周一的反弹吐出一部分。Anthropic 跌破发行价的讨论很多，但可靠的盘面数字今天并没有全部抓到，只好把「破发」本身记下，不去采用互相冲突的传闻跌幅。Hacker News 则更像一条技术日常：有人担心模型首先对东家负责，Quad9 真的关掉了法国服务，GreyNoise 写出一轮针对 Check Point 的入侵，OpenAI 则把自己的 GPT-6 写成也可以做蛋白质设计。北京市区今早降到 −3.8℃，白天转晴；海淀栏是常委会、常务会和政协届末总结，昌平则把城市更新和药企圆桌写进了区政新闻。阅读上，《人月神话》已经读完，《人件》仍在等分期书摘写进计划，今天先不硬造章节。若只从今天几条新访谈里留一句，Dwarkesh 那期更值得记住的不是结论，而是他反复回到的问题：如果人还在回路里，所谓「递归的自我改进」究竟还剩多少。
