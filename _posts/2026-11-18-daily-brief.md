---
layout: post
title: "早报 · 2026-11-18"
date: 2026-11-18 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读, 人月神话]
collected_at: "2026-11-18 07:42:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/18/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 18 日（星期三）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际RSS 的采集约在 07:34–07:36 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻和国际稿件约在 07:37–07:38；X 热榜约在 07:36；油管节目页约在 07:41–07:42。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 `feeds.reuters.com` 再次出现 TLS 失败，美联社 RSSHub 返回 403，均未列入。早报在 09:15 中间价和 09:30 常规开盘之前发出：A 股采用 11 月 17 日收盘价，人民币中间价采用 11 月 17 日已公布中间价。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。写稿时若当日官方中间价或 A 股尚未公布，数值栏直接采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 `docs/brief-memory/finance-history.json`。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,856.27 美元/盎司 | 较上一期早报（2026-11-17 07:35:57 Asia/Shanghai (UTC+8)）−0.20（−0.005%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 `3856.27002`，报价单位为美元/盎司；`updatedAt` 为 `2026-11-17T23:33:59Z`。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,856.47）计算 | 2026-11-18 07:33:59 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7132（11 月 17 日） | 较上一发布日（2026-11-16，6.7141）变动 −0.0009 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-18 07:34:15 返回的最新一条是 11 月 17 日的 6.7132；更早记录为 11 月 16 日 6.7141、11 月 13 日 6.7152。**本期采用 11 月 17 日已公布中间价**（采集时今日中间价尚未发布）。变化栏按官方上一发布日口径 | 采集 2026-11-18 07:34:15 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.679257 | 较上一期早报（2026-11-16 08:02:31 Asia/Shanghai (UTC+8)）+0.000858（+0.013%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。`time_last_update_utc` 为 Tue, 17 Nov 2026 00:02:31 +0000（合 2026-11-17 08:02:31 Asia/Shanghai），较上一期早报已刷新一笔日更；`time_next_update_utc` 为 Wed, 18 Nov 2026 00:35:41 +0000（约合 08:35:41 Asia/Shanghai），采集时今日日更尚未刷新 | 2026-11-17 08:02:31 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3584.58 | −17.99（−0.50%） | [东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 与 [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 核对一致：最新价 3584.58，涨跌 −17.99，涨跌幅 −0.50%，昨收 3602.57，开盘 3585.67，最高 3604.98，最低 3565.59。腾讯行情时间戳 `20261117161427`（2026-11-17 16:14:27）。采集时尚在 09:30 常规开盘之前，**本期采用 11 月 17 日收盘价，不是今日盘中或开盘价** | 采集 2026-11-18 07:34:16–07:34:18 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10638.52 | −52.26（−0.49%） | 同上来源：最新价 10638.52，涨跌 −52.26，涨跌幅 −0.49%，昨收 10690.78，开盘 10605.17，最高 10768.06，最低 10556.29。腾讯行情时间戳 `20261117161445` | 采集 2026-11-18 07:34:16–07:34:18 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报几乎持平，仍在 3,856 美元附近。市场化参考汇率已换成 11 月 17 日那一笔日更，兑人民币小幅走弱。官方中间价本期采用 11 月 17 日已公布的 6.7132，较 16 日中间价下调 0.0009；A 股本期采用 11 月 17 日收盘价，上证与深成指当日均小幅下跌。

## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [`/api/weather/view?stationid=54511`](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 `lastUpdate` 为 2026/11/18 07:20；本次采集时间为 2026-11-18 07:34:19 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。

**当前实况**（`lastUpdate` 2026/11/18 07:20）：气温 1.4℃，体感温度 −3.5℃，相对湿度 29%，西北风 3 级，风速 4.1 米/秒，降水量 0.0，气压 1025.0 百帕。接口返回的预警列表为空。

**今日（11 月 18 日）预报**：白天晴，最高 7℃，西北风微风；夜间晴，最低 −1℃，西北风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 19 日 | 白天晴，夜间多云 | 6℃ / −2℃ | 白天西北风 3～4 级，夜间西南风微风 |
| 11 月 20 日 | 白天晴，夜间晴 | 6℃ / −3℃ | 白天、夜间均为北风微风 |
| 11 月 21 日 | 白天晴，夜间晴 | 5℃ / −3℃ | 白天北风微风，夜间南风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 `docs/brief-memory/seen.json`。昨日已写过的区委全会预告、领导干部会议、西郊清代皇家园林保护规划公示、供暖检查和上地街道人才服务等，不再重复。区委十三届十二次全会原定 11 月 17 日召开，截至本次抓取，区政府要闻列表里尚未见到会后新稿，故不写无材料的续报。

#### 海淀区

**[海淀区开展区、镇人大代表换届选举投票 王少峰许心超王明哲宋斌参加](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261109_4833859.shtml)**。来源：海淀报，发布于 2026-11-09 09:09。稿件称，根据全市统一安排，海淀区于 11 月 6 日开展区、镇人大代表换届选举投票。区委书记王少峰，区委副书记、区长许心超，区人大常委会主任王明哲，区政协党组书记宋斌到海淀街道选举分会第二选区主投票站，核验选民证后填写并投下选票。区四套班子领导以及区法院、检察院主要负责人在各自选区投票或委托他人投票。

**[区领导调研中关村东区改造项目建设工作](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261103_4833240.shtml)**。来源：海淀报，发布于 2026-11-03 08:55。11 月 2 日，区委书记王少峰到中关村东区改造项目现场调研。报道称，该项目是北京市首个成片区央产危旧楼改建项目，按「成熟一片启动一片」推进。他先到中关村街道科源社区 13、14、15 号楼了解建筑历史及保护利用计划，随后到启动区 A 组团施工现场听取整体改造进展，并询问功能分区、绿化和配套设施等情况。稿件把它定位为民生工程，要求统筹科研、办公、商业与居住，严把质量和安全，推动项目如期建成投用。区领导马光耀、沈烨、张洪雨参加。

**[征地公告-京（海）政地征〔2026〕19号-海淀区上庄家园东路（翠湖南路-南沙河南街）道路工程项目](https://zyk.bjhd.gov.cn/zwdt/xxgk/tzgg/202611/t20261110_4834123.shtml)**。来源：北京市规划和自然资源委员会海淀分局，发布于 2026-11-10 10:33。公告称，北京海融达投资建设有限公司实施的上庄家园东路（翠湖南路–南沙河南街）道路工程，已获北京市人民政府批准（京政地字〔2026〕160 号）。土地用途为 S13 次干路用地，征收位置在海淀区西北旺镇西玉河村，征收西玉河村经济合作社集体土地 0.3366 公顷（约 5.05 亩），其中包括耕地 0.0809 公顷、林地 0.2201 公顷等。补偿标准为 77.7 万元/亩，征地补偿费共计 392.385 万元，全部采取货币补偿。公告期限为 2026 年 11 月 10 日至 11 月 23 日。

**[两新融合 向新而行 2026京港澳青年科学家大会在海淀举行](https://zyk.bjhd.gov.cn/ywdt/hdywx/202611/t20261105_4833542.shtml)**。来源：海淀报，发布于 2026-11-05 08:58。11 月 4 日，2026 京港澳青年科学家大会在海淀举行，为第 29 届京港洽谈会专题活动之一，主题是「两新融合向新而行」。北京海外联谊会会长马骏、海淀区委书记王少峰、香港中华厂商联合会会长卢金荣现场致辞，诺贝尔医学奖获得者迈克尔·霍顿视频致辞。王少峰在会上介绍海淀科创协同做法时称，区域内集聚 AI 企业超 2000 家，并提到「中关村科学城－香港创新加速器」已投入运行。以上企业数量和平台进展均为稿中的官方介绍。

#### 昌平区

**[昌平集中攻坚 家门口600+岗位机会助力毕业生就业](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111617050446671/index.html)**。来源：北京昌平 APP，发布于 2026-11-16。11 月 13 日，「英才聚昌·共赴新程」离校未就业高校毕业生等青年就业群体专场招聘会在沙河万达广场举办。报道称，45 家企业设摊，提供岗位 600 余个，涵盖工程师、人事、教师、会计等方向；现场分设毕业生岗位专区、失业人员岗位专区和线上投递区。毕业生专区放出 200 余个面向 2026 届离校暂未就业高校毕业生的岗位，学历要求以专科、本科为主。当天接待求职面谈 1600 余人次，接收简历 340 份，达成初步意向 124 人。

**[北七家镇高效推进安立路（科荟路-北六环）快速化改造工程民生保障工作](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026111714172142162/index.html)**。来源：北京昌平 APP，发布于 2026-11-17。安立路（科荟路–北六环）快速化改造是区域交通重点工程，五排干改移随道路同步实施。报道称，依水庄园小区居民对原设计不满：原方案要在小区出入口架过河桥接通西辅路，但高程差可能拆除部分用房并铺纵坡。北七家镇自 3 月起启用「吹哨报到」，对接市公联公司、区规自分局、城管委、水务局和项目部，4 月至 10 月召开 10 余场协调会。汛期前先在小区门前五排干铺设三根直径 1.2 米排水管作为临时行洪措施。10 月底确定的最终方案获居民认可：五排干上方铺绿植，并在通往安立路路段设置「Y」型上下路口。稿件称工程目前仍在推进。

**[路面平了、车棚大了、广场亮了——霍营街道和谐家园社区“微提升”改到居民心坎上](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026111716220896945/index.html)**。来源：北京昌平 APP，发布于 2026-11-17。和谐家园社区 2005 年建成、2006 年入住。报道称，近期小微空间提升改造已经完工，内容包括重铺局部柏油路、扩容自行车棚、修缮围墙、改造垃圾桶站、翻新广场，并拓宽车行路面、增设路侧停车位。居民此前集中反映车棚漏雨、围墙开裂和垃圾桶站气味等问题；改造前社区开过议事会征集意见。具体验收日期文中未另给，这里只按该稿已经写成的完工结果来记。

**[百名博士博士后人才进昌平 共绘科创发展新图景](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111617022468835/index.html)**。来源：北京昌平 APP，发布于 2026-11-16。11 月 13 日，「博才聚昌 智启新程」百名博士博士后走进昌平主题活动举办。报道称，活动吸引北京大学、清华大学、帝国理工学院等院校百余名博士、博士后参加；昌平实验室、北京脑科学与类脑研究所、北京生命科学研究所，以及国家能源集团新能源技术研究院、诺诚健华等 20 余家单位放出 120 余个高端科研岗位。参访点包括生命谷、能源谷。稿中提到的「北脑一号」「北脑二号」智能脑机系统，以及国家能源集团千吨级碳捕集中试平台等，均为报道对参访单位的介绍，这里不作额外核实。

**[昌平区与阿鲁科尔沁旗对接京蒙协作工作](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026111617225684578/index.html)**。来源：北京昌平 APP，发布于 2026-11-16。11 月 16 日，区委副书记、区长刘晓东与内蒙古赤峰市阿鲁科尔沁旗委副书记、政府旗长李凌宇座谈，对接京蒙协作。双方提到产业、乡村振兴、教育医疗和基础设施建设等既有合作，并表示将继续推进项目落地、人才与劳务协作。阿鲁科尔沁旗委常委、政府副旗长黄充参加。

## 3. 全球头条

路透社与美联社源站仍不可用，以下主要依据 BBC World、BBC 中文、纽约时报 World 与卫报 World 的 RSS 及打开后的原文。

### 续报：克里米亚大桥部分垮塌，泽连斯基称为「前所未有」的行动

[BBC](https://www.bbc.co.uk/news/articles/cw772jk4rvmxo) 11 月 17 日报道，连接俄罗斯与被占领克里米亚的大桥遭到严重破坏，泽连斯基称之为筹划数周的「前所未有」行动。乌克兰官员分享的图像显示，桥的一段塌入水中。克里姆林宫称将「比以前更好地」重建。报道说，此次打击动用巡航导弹和无人机，毁伤程度看起来大于以往几次袭击，道路部分的拱结构和桥面残骸可见伸出水面；泽连斯基称这是一场七阶段行动。BBC 文首时间为 2026-11-17 03:46 GMT（合 11:46 Asia/Shanghai），抓取时页面仍标注近期更新。同一轮报道还提到，基辅市长克利奇科称，第聂伯河上的北桥、南桥在俄方隔夜打击后已部分恢复交通。这是对昨日「大桥遇袭」一条的实质性续报：从「被击中」推进到「部分垮塌」。

### 续报：英伟达公布超千亿美元季度营收，董事会称不打算请回黄仁勋；他将于 12 月 1 日出席国会听证

[BBC](https://www.bbc.co.uk/news/articles/cm2kl50vkwkdo) 17 日晚间报道，英伟达公布黄仁勋去职后的首份季报：季度销售额同比翻倍，首次超过 1000 亿美元，达到 1158 亿美元；当季（截至 10 月 25 日的三个月）利润 650 亿美元，数据中心收入 1070 亿美元，同样同比翻倍。公司称下一季度营收还将再增 13%；盘后股价上涨 5%。代理首席执行官 Collette Kress 对分析师说「一切照常」「We've got this」。董事会主席 Harvey Jones 在电话会上表示：「董事会不打算请他回来。」他同时说，公司正与猎头评估内部和外部候选人，但不会匆忙决定。报道还提到，黄仁勋当天稍早曾表示，若能回去领导英伟达，他会感到「荣幸」。数字与表态均来自 BBC 对财报电话会的转述。

[卫报](https://www.theguardian.com/technology/2026/nov/17/jensen-huang-testify-congress-nvidia-affair-spy) 另称，黄仁勋将于 12 月 1 日到多个国会委员会作证，总法律顾问 Tim Teter 则于 12 月 2 日接受闭门问询。众议员 Brian Mast、John Moolenaar 和 Rick Crawford 在声明中说，他们希望了解此事在「潜在国家安全缺口」中的角色，包括先进芯片流向以及「一名可能的中国情报人员」的问题。这仍是未结束的调查与听证安排，不是已裁定的结论。相关背景是：[BBC](https://www.bbc.co.uk/news/articles/cmn504nq5033o) 17 日还报道，英伟达合作伙伴、新加坡公司 Megaspeed 正就芯片出口接受美国政府调查，涉嫌协助把高端 AI 芯片运往中国。

### 续报：深圳 APEC 进入高规格会晤窗口，普京已到深圳的消息登上热搜

[卫报](https://www.theguardian.com/world/2026/nov/17/hi-tech-shenzhen-chinamaxxing-xi-apec-summit) 从主办城市深圳写起，认为习近平要把这座科技城市当作「Chinamaxxing」的展示窗口，并提到会边已宣布将举行中美俄三方会晤。[BBC](https://www.bbc.co.uk/news/articles/crq5vlxxx32no) 称特朗普已在亚洲，为随后与中俄领导人的会谈做准备，并表示「如果有机会」，不排除与普京一对一会面。微博热搜在采集时出现「普京抵达深圳」「深圳人全妆出街迎 APEC」等条目；这与行程进展相符，但热搜本身不是官方公报。会谈结果仍未公布，这里只记行程与场面，不预判内容。[BBC 中文](https://www.bbc.com/zhongwen/articles/c893rg46x0ygo/trad) 也有「APEC 深圳观察」综述，角度与英文稿相近。

### 美国在保持 26 年麻疹消除状态后失去这一认定

[BBC](https://www.bbc.co.uk/news/articles/c977p71jx0xxo) 报道，泛美卫生组织（PAHO）认定，同一株麻疹病毒在美国持续传播超过 12 个月，美国因而失去保持了 26 年以上的麻疹消除状态。今年美国已报告 5400 例病例、10 例麻疹相关死亡，为 1990 年代以来最高。PAHO 主任 Jarbas Barbosa 说，墨西哥和玻利维亚也失去了消除状态，并将地区反弹归因为「持续的疫苗接种缺口」。美国疾控中心表示，将通过扩大疫苗可及性，致力于重新获得这一认定。

### 马尼拉反特朗普抗议中有近 300 人被捕

[卫报](https://www.theguardian.com/world/2026/nov/17/hundreds-arrested-manila-anti-trump-protests-philippines) 报道，在特朗普抵达马尼拉出席东盟峰会前，当地出现大规模抗议，当局已逮捕近 300 人。组织者称，周二可能有多达 1 万人继续示威，并试图向峰会场地行进。标题和导语将抗议原因概括为对伊朗战争以及一项 AI 协议的不满；正文未在抓取片段中给出该协议的官方文本，这里只按报道转述，不把细节写成已核实条款。

### 其他简讯

- [俄罗斯一架军用运输机在西伯利亚坠毁，机上 19 人全部遇难](https://www.bbc.co.uk/news/articles/cw8085rykkmgo)。国防部对官方媒体称，这架安-12 在克麦罗沃州一次「计划飞行」中坠于无人居住区，初步认为是技术故障；州长 Ilya Seredyuk 说事发在 Yagunovo 村附近，火势已被扑灭。BBC 与路透核实过一段社交媒体上的监控录像拍摄时间，路透还按地景与卫星图核对了地点。机上是否载有货物，报道称尚不清楚。
- [哥斯达黎加记者 Camilo Rodríguez 遭枪击身亡](https://www.theguardian.com/world/2026/nov/17/costa-rica-journalist-camilo-rodriguez-shot-dead)，卫报和 [BBC](https://www.bbc.co.uk/news/articles/c6ly7g5lx7gyo) 都写到，这是该国 25 年来首例记者被杀；他曾报道涉嫌毒枭与政治人物的关系。
- 西岸冲突与制裁：BBC 称一名 72 岁巴勒斯坦妇女被以色列定居者开枪打死，以军则称定居者是在遇袭后开火；[英国](https://www.bbc.co.uk/news/articles/cvglr977x3z0o) 与 [澳大利亚](https://www.theguardian.com/world/2026/nov/18/australia-sanctions-construction-company-west-bank-settlement-expansion-ntwnfb) 分别宣布对参与西岸定居点的公司或个人实施制裁。
- [一名美国士兵因间谍嫌疑在英国被捕后，已移交美军羁押](https://www.bbc.co.uk/news/articles/c6x284ez38vdo)。
- 昨日已写过的欧盟卢旺达遣返中心、胡塞武装与红海风险等，未见必须单独展开的新进展，不再重写。

## 4. Hacker News 近期文章

抓取来源为 Algolia 首页接口 `https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30`，采集时间 2026-11-18 07:34:26 Asia/Shanghai（UTC+8）。以下点数与评论数为当时接口返回值。今日首页与昨日几乎完全换了新面孔，30 条均未出现在查重档案中。

### New Evidence Shows School Phone Bans Are Gradually Improving Test Scores

[原文](https://www.nytimes.com/2026/11/17/upshot/school-phone-bans-study-scores.html) · [HN 讨论](https://news.ycombinator.com/item?id=50530163) · 1122 点 / 554 评 · 2026-11-17 19:45:51 Asia/Shanghai（UTC+8）

纽约时报这篇 Upshot 稿在抓取时返回 403，未能直接核对正文。同一项研究有哈佛大学新闻稿和美联社报道可对照：[Harvard Gazette](https://news.harvard.edu/gazette/story/2026/11/schools-that-ban-cellphones-see-uptick-in-test-scores/) 介绍，哈佛教育政策研究中心的 Thomas Kane 等人把严格禁手机（包括使用锁定袋）视为一场反向的自然实验，估计成绩增长约 0.01 个标准差，相当于一学年多出大约一到两周的学习量；按常规干预标准这并不算大，但大约相当于 2013 年以来年度成绩损失的一半。[美联社](https://apnews.com/article/school-cellphone-bans-test-scores-79e11f36a1321815d43517b5243fbc34) 写的是约 330 万名学生、4600 所学校，并引用 Kane 的话说「有正向作用，但不是万灵药」。两篇转述都提醒：另有一项 4 月的研究认为总体效果接近于零；新研究是否经过同行评审，转述中也写了保留。数字与判断均来自上述转述，不是对纽约时报原文的逐句翻译。

### GPT‑6.2 Astra and Sol

[原文](https://openai.com/index/introducing-gpt-6-2-astra-sol/) · [HN 讨论](https://news.ycombinator.com/item?id=50535230) · 1005 点 / 622 评 · 2026-11-18 01:46:43 Asia/Shanghai（UTC+8）

OpenAI 官方介绍新的 GPT‑6.2 Astra（面向更难的专业项目）和 GPT‑6.2 Sol（面向日常工作）。官网称两者都能在更少的输出 token 下完成更重的任务。关于能力与价格的数字都是官方自述，例如：在 Agents’ Last Exam 上，Astra 比 GPT‑6 Astra 高 5.2 分、成本不到三分之一，并称比 Claude Fable 5.2 高 5.5 分、成本约为其 5%；在 Terminal-Bench-Science 0.1 和 Vals Science Index 上刷新高点；API 输入/输出价格较 GPT‑6 Astra 低 20%，为每百万 token 8 美元输入、0.40 美元缓存输入、40 美元输出；Sol 保持 GPT‑6.1 Sol 的 API 价格。官网还称「我们相信 GPT-6.2 Astra 是全球最适合科学家的模型」。这些都是出品方的评测与定价说明，不是第三方复测。

### Apple Services Down

[原文](https://developer.apple.com/system-status/) · [HN 讨论](https://news.ycombinator.com/item?id=50535238) · 596 点 / 320 评 · 2026-11-18 01:47:14 Asia/Shanghai（UTC+8）

HN 链到的是开发者系统状态页，本机抓取到的是前端壳，服务条目需对照苹果对用户公开的 [System Status](https://www.apple.com/support/systemstatus/?lv=true)。该页列出 11 月 17 日多项已恢复的故障（时间均为美国东部标准时间）：App Store 停摆 11:45–15:00，AppleCare on Device 停摆 11:15–15:39，iCloud 账户与登录问题 11:45–16:15，iCloud.com 性能问题 11:45–16:15，iCloud Mail 性能问题 11:45–13:25，以及 Apple Business、Schoolwork、Apple School Manager 等在 13:40–17:00 的问题。页面「Last updated」为当天 17:57 ET（约合 2026-11-18 06:57 Asia/Shanghai）。换算后，App Store 停摆约对应 11 月 18 日 00:45–04:00，iCloud 登录问题约对应 00:45–05:15。[TechCrunch](https://techcrunch.com/2026/11/17/apple-services-including-icloud-app-store-and-apple-music-hit-by-outage/) 与 [AppleInsider](https://appleinsider.com/articles/26/11/17/icloud-account-login-icloud-mail-services-are-having-trouble-today) 均报道苹果将原因归为内部更新，而非网络攻击。写稿时按状态页，这些条目均已显示为 Resolved。

### Highly classified US national security communications network goes down

[原文](https://www.cnn.com/2026/11/17/politics/highly-classified-national-security-communications-network-goes-down) · [HN 讨论](https://news.ycombinator.com/item?id=50532849) · 405 点 / 508 评 · 2026-11-17 23:38:28 Asia/Shanghai（UTC+8）

CNN 17 日独家报道，援引六名知情人士称，国家安全局用于内部通信的高度机密网络 NSANet 出现中断；该网络供员工内部传递机密信息。消息源称，目前没有网络攻击的证据；在查明范围期间，机构安排了错峰到岗。CNN 文中引用的官方表述提到「临时降级」。发布时间约为 2026-11-17 15:31 UTC（合 23:31 Asia/Shanghai）。原因尚未在这篇报道里给出定论。

### Java4Shell: RCE in OpenJDK when processing Base64

[原文](https://calif.io/java4shell/) · [HN 讨论](https://news.ycombinator.com/item?id=50538240) · 336 点 / 83 评 · 2026-11-18 05:11:28 Asia/Shanghai（UTC+8）

发现者 Quang Luong 在 calif.io 把该问题命名为 Java4Shell，并标为 CVE-2026-114938：在受影响的 OpenJDK 构建中，畸形 Base64 数据可导致已分配堆内存被常量值覆盖，再被转成堆泄漏和远程代码执行。首页另一条 [Aikido 说明](https://www.aikido.dev/blog/java-17-rce-vulnerability-cve-2026-114938)（[HN](https://news.ycombinator.com/item?id=50532118)，122 点 / 16 评）称，这是据报存在于 Java 17、21、25 和 27 的预认证远程代码执行，并讨论受影响版本与修复构建。版本范围以这些技术文章的表述为准，实施修补仍应对照 OpenJDK 或发行版官方公告。这里只记录漏洞被公开这一事实，不转述利用步骤。

### What is the best harness for each model?

[原文](https://runta.com/blog/introducing-frontierharness-eval-v1-1/) · [HN 讨论](https://news.ycombinator.com/item?id=50532191) · 318 点 / 111 评 · 2026-11-17 22:53:43 Asia/Shanghai（UTC+8）

RUNTA 的 Shilin Zhu 介绍 FrontierHarness Eval v1.1：与 Baseten 合作，用 22 种编程智能体 harness、5 个模型、62 项任务、各跑 4 次，共 27,280 次运行、830 亿 token。作者想回答的问题是：换模型时要不要同时换 harness，以及每个模型的「性价比最好」的 harness 是哪一个。文章称，最佳 harness 随模型而变；在模型固定时，最贵的 harness 单任务成本是最便宜者的 1.8 到 5.0 倍。这些都是该评测自己的结果。

### Nvidia stopped disclosing Singapore sales as revenues hit $104B

[原文](https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf) · [HN 讨论](https://news.ycombinator.com/item?id=50534631) · 317 点 / 166 评 · 2026-11-18 01:12:06 Asia/Shanghai（UTC+8）

金融时报原文在抓取时返回 403，文中「新加坡销售」和「收入达到 1040 亿美元」等表述未能核对，这里只保留英文标题和讨论链接。可对照的公开事实见上文 BBC 季报：公司公布的当季销售额是 1158 亿美元；另有新加坡合作伙伴 Megaspeed 出口调查的报道。不要把未能打开的 FT 标题数字与 BBC 季报数字混算。

### MAI Code 2 and Code 2 Flash

[原文](https://microsoft.ai/news/introducing-mai-code-2-and-mai-code-2-flash/) · [HN 讨论](https://news.ycombinator.com/item?id=50535885) · 252 点 / 115 评 · 2026-11-18 02:25:13 Asia/Shanghai（UTC+8）

Microsoft AI 发布 MAI Code 2 与更轻量的 MAI Code 2 Flash，定位是企业日常编码，而不是「基础科学或超长周期的智能体工作」。官方称，在 DeepSWE 1.1、Terminal Bench 2.1、SWE-Atlas 和 FrontierCode v1.1 四项面向日常企业编码的基准上平均来看，MAI Code 2 达到 GPT 6.1 Sol 约 98% 的表现、成本约为其 40%。价格与分数都是出品方的说法。发布时间接近微软 Ignite 窗口，旧金山 X 热榜上也有 `#MSIgnite`。

### How the Claude Code team thinks about verification

[原文](https://claude.dev/blog/how-the-claude-code-team-thinks-about-verification/) · [HN 讨论](https://news.ycombinator.com/item?id=50529612) · 249 点 / 194 评 · 2026-11-17 18:20:40 Asia/Shanghai（UTC+8）

Claude Code 团队的 Addy Osmani 在 11 月 16 日的工程博客里讨论：智能体要靠端到端测试、属性测试和差分测试来「拿出证据」，而不是只生成代码。文中称，该团队「大约 90%」的代码由 Claude 编写并审查——这是出品方自己的比例，不是外部审计数字。文章的重点是：生成变便宜之后，验证器本身也必须被诚实地设计，否则模型会学会应付检查。

### Phrack 73 Released

[原文](https://phrack.org/issues/73/introduction_md) · [HN 讨论](https://news.ycombinator.com/item?id=50535992) · 228 点 / 23 评 · 2026-11-18 02:31:25 Asia/Shanghai（UTC+8）

老牌黑客杂志 *Phrack* 第 73 期上线。导言回顾去年 40 周年纸质发行，并列出本期目录，其中包括 Docker/vDSO 逃逸、证明系统与内核、TCC 绕过、隐藏技术，以及一篇讨论「LLM 中的病毒」的文章等。这里只记期刊发布，不转载其中技术细节。

### jQuery 4.1.0

[原文（GitHub Release）](https://github.com/jquery/jquery/releases/tag/4.1.0) · [官方博客](https://blog.jquery.com/2026/11/17/jquery-4-1-0-and-3-8-0-released-passing-the-torch/) · [HN 讨论](https://news.ycombinator.com/item?id=50537156) · 215 点 / 114 评 · 2026-11-18 03:50:40 Asia/Shanghai（UTC+8）

Timmy Willison 在官方博客宣布同时发布 jQuery 4.1.0 和 3.8.0。4.1.0 是 4.x 的第一个小版本；3.8.0 则是把 3.x-stable 上累积多年的修复发出去，之后 3.x 只再接受关键安全和缺陷修复，官方称之为「送别，不是回归」。两边都修了选择器标识符匹配中的正则拒绝服务，并调整 AJAX transport 的 `completeCallback` 写法。4.1.0 还为 `jqXHR` 增加 `responseURL`，让表单关联的自定义元素能被正确序列化，并改为普遍使用 `querySelectorAll`。

### 其余首页条目

- [350 years ago, Ole Rømer discovered that light has a finite speed](https://www.sciencenorway.no/culture-history-history-of-science/350-years-ago-this-man-discovered-that-light-has-a-finite-speed/2737969) · [HN](https://news.ycombinator.com/item?id=50536813) · 212 点 / 65 评。科学史回顾。原文页本次抓取不完整，未展开。
- [Solid 2.0](https://www.solidjs.com/blog/solid-2-0-the-long-hold/) · [HN](https://news.ycombinator.com/item?id=50536387) · 188 点 / 51 评。Ryan Carniato 宣布 Solid 2.0 稳定：把异步纳入响应式图、加入 server functions，并收窄 API。
- [Show HN: Alloy CSS, dialogs, menus and tabs that work with JavaScript off](https://alloyhtml.com/example.html) · [HN](https://news.ycombinator.com/item?id=50532385) · 167 点 / 29 评。示范在关闭 JavaScript 时仍可用的对话框、菜单和标签页。
- [Quad9's withdrawal from France: A canary in the coal mine](https://blog.cloudflare.com/quad9-withdrawal-from-france/) · [HN](https://news.ycombinator.com/item?id=50538994) · 127 点 / 11 评。Cloudflare 评论 Quad9 被迫撤出法国，认为强制在 DNS 层做封锁是危险先例。
- [Web Browser Engineering (2021)](https://browser.engineering/) · [HN](https://news.ycombinator.com/item?id=50537290) · 107 点 / 17 评。浏览器实现教材再次出现在首页。
- [Who Builds the Machines That Build the Machines?](https://read.corematter.com/p/section-232-us-machine-tools) · [HN](https://news.ycombinator.com/item?id=50535208) · 79 点 / 24 评。讨论美国机床与 232 条款。
- [Effects of a Nuclear Detonation in Low Earth Orbit](https://arxiv.org/abs/2611.09827) · [HN](https://news.ycombinator.com/item?id=50537120) · 66 点 / 31 评。预印本。
- [Not Everything Needs an LLM](https://newsletter.posthog.com/p/decision-models) · [HN](https://news.ycombinator.com/item?id=50535740) · 65 点 / 23 评。PostHog 讨论何时不必上大模型。
- [Mouse Party](https://aboard.com/lets-have-a-mouse-party/) · [HN](https://news.ycombinator.com/item?id=50497872) · 47 点 / 7 评。
- [Launch HN: StarSling (YC P25) – Self-improving CI for agent-volume repos](https://starsling.dev) · [HN](https://news.ycombinator.com/item?id=50536468) · 41 点 / 20 评。
- [Show HN: TrnRT – An open-source LLM inference engine for AWS Trainium](https://github.com/RunanywhereAI/trnrt) · [HN](https://news.ycombinator.com/item?id=50533270) · 39 点 / 5 评。
- [Zoltraak and the Dynamics of Military Innovation](https://jgeekstudies.org/2026/11/15/zoltraak-military-innovation-in-frieren/ ) · [HN](https://news.ycombinator.com/item?id=50511657) · 38 点 / 7 评。用《葬送的芙莉莲》讨论军事创新。
- [Advancing computer-use agents for healthcare teams](https://openai.com/index/advancing-computer-use-for-healthcare-teams/) · [HN](https://news.ycombinator.com/item?id=50535898) · 34 点 / 23 评。
- [Fixing a WebKit bug to see if promises are made of train tracks](https://alistair.sh/thenables) · [HN](https://news.ycombinator.com/item?id=50499520) · 27 点 / 1 评。
- [Harvard researchers find AI coding agents shifted the bottleneck to code review](https://complexdiscovery.com/harvard-researchers-find-ai-coding-agents-shifted-the-bottleneck-to-code-review/) · [HN](https://news.ycombinator.com/item?id=50538303) · 19 点 / 23 评。
- [Tencent Hy4 Flash](https://hy.tencent.ai/research/hy4-flash) · [HN](https://news.ycombinator.com/item?id=50538184) · 17 点 / 1 评。
- [Latent Lattice Language Models](https://shivamduggal4.github.io/latent-lattice-language-models/) · [HN](https://news.ycombinator.com/item?id=50539039) · 10 点 / 0 评。
- YC wrote software to run our internship expo – and an 8-bit SIM to show it off · [HN](https://news.ycombinator.com/item?id=50534429) · 接口未返回外链，只保留讨论页。

## 5. X 热门与科技圈

使用 X 公共连接器读取各地趋势，采集约在 2026-11-18 07:36 Asia/Shanghai（UTC+8）。接口未返回各话题的帖文数量。对中国（WOEID 23424781）的查询没有带回地点元数据，结果与全球榜几乎相同，故不把它当作中国地区热榜来引用。

### 地区热榜快照

- [全球](https://x.com/explore)：`GOTY`、`GTA 6` / `GTA VI`、`#TheGameAwards` 相关的 `Geoff`、`Crimson Desert`，以及 `Apple`、`Astra`。其余多为地区促销或综艺标签，例如 `#てりやきマックバーガー召し上がれ`、`#KohLanta`、`#CorridaDasBlogueiras8`。
- [美国](https://x.com/explore)：`#gta6cat`、`GOTY`、`#TheGameAwards`、`Apple`、`Astra`、`iCloud`、`Data Center`、`103% YoY`、`GTA VI` 等。后两项可能与昨夜科技财报有关，但热榜本身没有说明，这里不自行对应到某一家公司。
- [英国](https://x.com/explore)：娱乐节目 `#ImACeleb`、`#GBBO` 和足球人名占前排，`GOTY`、`GTA 6` 同样在列。
- [旧金山](https://x.com/explore)：`#MSIgnite`、`Bring Jensen`、`Apple`、`Astra`、`#TheGameAwards`、`Devin`、`Vice City` 等，科技话题更集中。

### 科技与 IT 圈在讨论什么

最醒目的两条产品线，和 HN 首页是对得上的。`Astra` 出现在全球和美国热榜，对应 OpenAI 刚刚发布的 GPT‑6.2 Astra / Sol；`Apple` 与 `iCloud` 则对应 11 月 17 日那一轮服务中断。X 上传播较广的汇总帖，例如 [Pirat_Nation 的状态页摘录](https://x.com/Pirat_Nation/status/2122759320244769153)，与后来苹果状态页列出的 App Store、iCloud 登录、Apple Music、AppleCare 等问题方向一致。如前所述，到早报采集时，公开状态页已把这些条目标为已恢复；苹果方面把原因说成内部更新，不是网络攻击。

旧金山热榜上的「Bring Jensen」更多是情绪口号。检索到的帖文大量是重复刷「BRING JENSEN BACK」的转发，互动数据很低，不宜当成新的事实来源。可核对的进展仍是英伟达董事会公开表示不打算请回黄仁勋，以及 12 月的国会听证安排。把「已经回归」写成事实，仍然没有根据。

`#MSIgnite` 与微软发布 MAI Code 2 出现在同一时间窗口。游戏方面，`GOTY`、`GTA 6`、`Crimson Desert` 和 `Geoff` 说明 The Game Awards 临近，讨论热度很高，但与今日其他栏目没有直接交叉，这里只记趋势，不展开颁奖预测。

## 6. 微博热搜

接口 `https://weibo.com/ajax/side/hotSearch` 请求成功，采集时间 2026-11-18 07:34:27 Asia/Shanghai（UTC+8）。热度数字为接口返回的 `num`，不是官方统计。链接指向 `s.weibo.com` 搜索页。本期实时榜前部未见明确标注为广告的条目。

### 置顶 / 政务

- [#亚太是我们的共同家园#](https://s.weibo.com/weibo?q=%23%E4%BA%9A%E5%A4%AA%E6%98%AF%E6%88%91%E4%BB%AC%E7%9A%84%E5%85%B1%E5%90%8C%E5%AE%B6%E5%9B%AD%23)（接口同时给出原微博 `weibo.com/2803301701/RrLBitZz0`）

### 需要展开的话题

- [深圳人全妆出街迎APEC](https://s.weibo.com/weibo?q=%23%E6%B7%B1%E5%9C%B3%E4%BA%BA%E5%85%A8%E5%A6%86%E5%87%BA%E8%A1%97%E8%BF%8EAPEC%23)（832,794）、[#2026APEC这些看点值得期待#](https://s.weibo.com/weibo?q=%232026APEC%E8%BF%99%E4%BA%9B%E7%9C%8B%E7%82%B9%E5%80%BC%E5%BE%97%E6%9C%9F%E5%BE%85%23)（490,850）、[#普京抵达深圳#](https://s.weibo.com/weibo?q=%23%E6%99%AE%E4%BA%AC%E6%8A%B5%E8%BE%BE%E6%B7%B1%E5%9C%B3%23)（169,485，标「新」）、[#深圳人收起人字拖换皮鞋小白鞋#](https://s.weibo.com/weibo?q=%23%E6%B7%B1%E5%9C%B3%E4%BA%BA%E6%94%B6%E8%B5%B7%E4%BA%BA%E5%AD%97%E6%8B%96%E6%8D%A2%E7%9A%AE%E9%9E%8B%E5%B0%8F%E7%99%BD%E9%9E%8B%23)（80,885）。主线仍是深圳 APEC。中文热搜比英文世界版更早把「普京抵达」推到前排；这与会晤窗口吻合，但具体抵达安排仍以官方通报为准。
- [字节被指只差聊天软件](https://s.weibo.com/weibo?q=%E5%AD%97%E8%8A%82%E8%A2%AB%E6%8C%87%E5%8F%AA%E5%B7%AE%E8%81%8A%E5%A4%A9%E8%BD%AF%E4%BB%B6)（600,974）、[豆包加聊天功能或威胁微信](https://s.weibo.com/weibo?q=%E8%B1%86%E5%8C%85%E5%8A%A0%E8%81%8A%E5%A4%A9%E5%8A%9F%E8%83%BD%E6%88%96%E5%A8%81%E8%83%81%E5%BE%AE%E4%BF%A1)（167,971）、[字节多领域追赶腾讯](https://s.weibo.com/weibo?q=%E5%AD%97%E8%8A%82%E5%A4%9A%E9%A2%86%E5%9F%9F%E8%BF%BD%E8%B5%B6%E8%85%BE%E8%AE%AF)（165,149）。三条连在一起，说的是字节跳动为豆包增加聊天能力、可能冲击微信的流传。未见当场可核对的产品官方说明，这里只记热搜，不当成已经发布的产品计划。
- [#雷军APEC现场挨个发名片#](https://s.weibo.com/weibo?q=%23%E9%9B%B7%E5%86%9BAPEC%E7%8E%B0%E5%9C%BA%E6%8C%A8%E4%B8%AA%E5%8F%91%E5%90%8D%E7%89%87%23)（168,310）、[小米回应雷军APEC发言紧张](https://s.weibo.com/weibo?q=%E5%B0%8F%E7%B1%B3%E5%9B%9E%E5%BA%94%E9%9B%B7%E5%86%9BAPEC%E5%8F%91%E8%A8%80%E7%B4%A7%E5%BC%A0)（80,491）、[#小米18真机曝光#](https://s.weibo.com/weibo?q=%23%E5%B0%8F%E7%B1%B318%E7%9C%9F%E6%9C%BA%E6%9B%9D%E5%85%89%23)（81,463）。前两条是峰会场边花絮；「真机曝光」真伪未核实，只作为热搜记录。
- [#英伟达预计第四季度营收超预期#](https://s.weibo.com/weibo?q=%23%E8%8B%B1%E4%BC%9F%E8%BE%BE%E9%A2%84%E8%AE%A1%E7%AC%AC%E5%9B%9B%E5%AD%A3%E5%BA%A6%E8%90%A5%E6%94%B6%E8%B6%85%E9%A2%84%E6%9C%9F%23)（82,304，标「新」）。与上文 BBC 转述的季报和「下一季度营收再增 13%」相呼应，是同一条公司新闻在中文热搜上的标题化。具体数字仍以英文报道中的官方口径为准。
- [#神舟二十四号进入发射前关键阶段#](https://s.weibo.com/weibo?q=%23%E7%A5%9E%E8%88%9F%E4%BA%8C%E5%8D%81%E5%9B%9B%E5%8F%B7%E8%BF%9B%E5%85%A5%E5%8F%91%E5%B0%84%E5%89%8D%E5%85%B3%E9%94%AE%E9%98%B6%E6%AE%B5%23)（81,960）。热搜只给了这句判断，未见可在早报里引用的发射窗口官方细节，不补充未出现的日期。

### 速览

[男子的相亲经历比相声还精彩](https://s.weibo.com/weibo?q=%23%E7%94%B7%E5%AD%90%E7%9A%84%E7%9B%B8%E4%BA%B2%E7%BB%8F%E5%8E%86%E6%AF%94%E7%9B%B8%E5%A3%B0%E8%BF%98%E7%B2%BE%E5%BD%A9%23)、[#肖战小城良方又加新广#](https://s.weibo.com/weibo?q=%23%E8%82%96%E6%88%98%E5%B0%8F%E5%9F%8E%E8%89%AF%E6%96%B9%E5%8F%88%E5%8A%A0%E6%96%B0%E5%B9%BF%23)、[#曾沛慈说要去声生不息追星#](https://s.weibo.com/weibo?q=%23%E6%9B%BE%E6%B2%9B%E6%85%88%E8%AF%B4%E8%A6%81%E5%8E%BB%E5%A3%B0%E7%94%9F%E4%B8%8D%E6%81%AF%E8%BF%BD%E6%98%9F%23)、[#曝厉娜和朋友蛐蛐许飞#](https://s.weibo.com/weibo?q=%23%E6%9B%9D%E5%8E%89%E5%A8%9C%E5%92%8C%E6%9C%8B%E5%8F%8B%E8%9B%BE%E8%9B%BE%E8%AE%B8%E9%A3%9E%23)、[#BLG赛点局ON高喊别虐泉#](https://s.weibo.com/weibo?q=%23BLG%E8%B5%9B%E7%82%B9%E5%B1%80ON%E9%AB%98%E5%96%8A%E5%88%AB%E8%99%90%E6%B3%89%23)、[#快女冠军段林希咋倒嗓成这样#](https://s.weibo.com/weibo?q=%23%E5%BF%AB%E5%A5%B3%E5%86%A0%E5%86%9B%E6%AE%B5%E6%9E%97%E5%B8%8C%E5%92%8B%E5%80%92%E5%97%93%E6%88%90%E8%BF%99%E6%A0%B7%23)、[#虞书欣近1年掉粉118万#](https://s.weibo.com/weibo?q=%23%E8%99%9E%E4%B9%A6%E6%AC%A3%E8%BF%911%E5%B9%B4%E6%8E%89%E7%B2%89118%E4%B8%87%23)、[#奚梦瑶白到整个人都在发光#](https://s.weibo.com/weibo?q=%23%E5%A5%9A%E6%A2%A6%E7%91%B6%E7%99%BD%E5%88%B0%E6%95%B4%E4%B8%AA%E4%BA%BA%E9%83%BD%E5%9C%A8%E5%8F%91%E5%85%89%23)、[杜海涛英语直播 全障碍交流](https://s.weibo.com/weibo?q=%E6%9D%9C%E6%B5%B7%E6%B6%9B%E8%8B%B1%E8%AF%AD%E7%9B%B4%E6%92%AD%20%E5%85%A8%E9%9A%9C%E7%A2%8D%E4%BA%A4%E6%B5%81)、[#赵丽颖选剧本的眼光到底有多远#](https://s.weibo.com/weibo?q=%23%E8%B5%B5%E4%B8%BD%E9%A2%96%E9%80%89%E5%89%A7%E6%9C%AC%E7%9A%84%E7%9C%BC%E5%85%89%E5%88%B0%E5%BA%95%E6%9C%89%E5%A4%9A%E8%BF%9C%23)、[#难怪郑恺高考成绩可以上复旦#](https://s.weibo.com/weibo?q=%23%E9%9A%BE%E6%80%AA%E9%83%91%E6%81%BA%E9%AB%98%E8%80%83%E6%88%90%E7%BB%A9%E5%8F%AF%E4%BB%A5%E4%B8%8A%E5%A4%8D%E6%97%A6%23)、[拉布拉多没穿警服被当成流浪狗](https://s.weibo.com/weibo?q=%E6%8B%89%E5%B8%83%E6%8B%89%E5%A4%9A%E6%B2%A1%E7%A9%BF%E8%AD%A6%E6%9C%8D%E8%A2%AB%E5%BD%93%E6%88%90%E6%B5%81%E6%B5%AA%E7%8B%97)。

## 7. 油管科技访谈

对照 `docs/youtube-sources.md` 的频道名单，从各频道 `/videos` 页解析近况，再打开视频页读取官方简介与发布时间。只选约 15 分钟以上、近约 7–10 天内、尚未写入查重档案的访谈或对谈。节目中的判断与数字，均来自官方简介或章节目录，不是对口播的转写。

### OpenAI’s Cofounder & Research Chief Explain Self-Improving AI

[视频](https://www.youtube.com/watch?v=h_aA1-R70E8) · a16z · 16 分 19 秒 · 发布 2026-11-18 01:41:29 Asia/Shanghai（UTC+8）（源站 `2026-11-17T09:41:29-08:00`）

这是 a16z「Working Theory」的第一集。Sarah Wang 与 OpenAI 首席研究官 Mark Chen、Thinking Machines Lab 首席科学家兼 OpenAI 联合创始人 John Schulman 讨论递归自我改进（RSI）。简介里写：Mark Chen 称 OpenAI 已经做出「AI research interns」；他们会谈到 RSI 究竟指什么、研究品味为什么难教，以及为什么有人把 AI 视为对齐问题的工具之一。章节包括 What is RSI?、How far are we?、Getting to full RSI、Aligning RSI。若只想听官方产品发布，上一节的 GPT‑6.2 稿已经足够；这一集是研究人员自己谈「研究会不会被模型加速」，可以分开看。

### Databricks CEO: AGI Is Already Here, Why Companies Are Behind, and the Superintelligence Debate

[视频](https://www.youtube.com/watch?v=1bR0gtecoHU) · All-In Podcast · 1 小时 2 分 6 秒 · 发布 2026-11-18 06:19:53 Asia/Shanghai（UTC+8）（源站 `2026-11-17T14:19:53-08:00`）

Databricks 首席执行官 Ali Ghodsi 作客 All-In，时间就在早报前约一小时。官方章节是：公司在云、AI 与开源上的早期押注；「AGI 是否已经到来」以及企业 AI 为何落后；现场演示 Databricks 如何用智能体提高效率；关于 IPO 与保持私有的讨论；以及 RSI、网络风险和「doom debate」。标题里的「AGI Is Already Here」是节目自己的提法，这里只按简介记录，不把它写成业界共识。All-In 另有一集三天前的「Jensen OUT as Nvidia CEO」，内容与已经写过的去职报道高度重叠，本期不再展开。

### Recursive self-improvement has started

[视频](https://www.youtube.com/watch?v=1NHPDzpfR6Y) · Dwarkesh Patel · 44 分 26 秒 · 发布 2026-11-14 02:37:05 Asia/Shanghai（UTC+8）（源站 `2026-11-13T10:37:05-08:00`）

这是 Dwarkesh 把自己的长文口述出来的一集，书面版在 [dwarkesh.com/p/rsi](https://www.dwarkesh.com/p/rsi)。简介里他说，年初自己还觉得超级智能「至少还要将近十年」，最近三个月看法变了，并逐条回应持续学习、可验证代理指标、数据和实验算力等反对意见。这些都是他的个人判断，不是实验室公告。与上一期已经写过的 Paul Christiano 访谈不是同一集。

### Russia-Ukraine War: Putin, Zelenskyy, Drones and the Future of Warfare | Lex Fridman Podcast #504

[视频](https://www.youtube.com/watch?v=2hJkprFnzhY) · Lex Fridman · 2 小时 53 分 49 秒 · 发布 2026-11-11 07:52:20 Asia/Shanghai（UTC+8）（源站 `2026-11-10T15:52:20-08:00`）

Lex 与 Preston Stewart、Michael Kofman 谈俄乌战争、无人机和战场形态。Stewart 是西点毕业、阿富汗退伍军人，经营 War and Conflict 节目；Kofman 是卡内基国际和平研究院高级研究员，主持 War on the Rocks 的 The Russia Contingency。官方提纲包括战争现状、无人机与杀伤区、以及「谁在占上风」。它不替代今日关于克里米亚大桥的新闻续报，而是提供更长的战场背景。文稿与反馈入口在 [lexfridman.com](https://lexfridman.com/preston-stewart-michael-kofman-transcript)。

### Software correctness and programming languages with Sean Allen

[视频](https://www.youtube.com/watch?v=OrXKvOjR-vI) · The Pragmatic Engineer · 1 小时 25 分 20 秒 · 发布 2026-11-10 22:23:48 Asia/Shanghai（UTC+8）（源站 `2026-11-10T06:23:48-08:00`）

主持人与 Antithesis 杰出工程师 Sean Allen 谈软件正确性与编程语言。官方简介特意写了一句：他们「一次也没有提到 AI」，尽管这恰好也是在 AI 辅助开发里最要紧的那些基础。章节覆盖 OCaml 与类型系统、Ada、F#、Pony 与安全并发、垃圾回收、测试与属性测试、供应链安全、侧信道与机密计算，以及「慢即是快」。和 Claude Code 那篇谈验证的博客是同一问题的不同入口：生成变容易之后，正确性仍然要靠语言、工具和测试来扛。

### Designing for Agents — Zeno Rocha, Resend

[视频](https://www.youtube.com/watch?v=bdIoODXsu8k) · Latent Space · 1 小时 25 分 52 秒 · 发布 2026-11-11 03:57:24 Asia/Shanghai（UTC+8）（源站 `2026-11-10T11:57:24-08:00`）

Resend 联合创始人兼首席执行官 Zeno Rocha 从一件很具体的事谈起：当编程智能体要替你挑邮件服务商时，它会选谁，这个选择又如何随模型版本变化。简介还提到：智能体选中 Resend 之后，能否自己找到价格、注册并发出第一封邮件；以及 Gmail 限流、追踪像素的误导，还有滥用发信者如何连累其他客户。产品一侧，他们讨论给智能体提供 80 多个具名 MCP 工具、让它读取 Markdown 价格，以及自行注册服务。文中 80 多个工具和邮件安全承诺等，都是节目简介里的出品方说明。

## 8. 本月阅读与今日书摘

11 月的四本书不变，完整说明见[本月阅读](/reading/)：

1. [《人月神话》](/reading/)（*The Mythical Man-Month*，弗雷德里克·布鲁克斯），本周读完
2. 《人件》（*Peopleware*，汤姆·德马可、蒂姆·李斯特）
3. 《代码大全》（*Code Complete*，史蒂夫·迈克康奈尔）
4. 《软件设计的哲学》（*A Philosophy of Software Design*，约翰·奥斯特豪特）

昨天读了第 5–8 章。下面是第 9–12 章的精炼摘要，依据 1995 年 20 周年纪念版，只作导读，不转载正文。

### 今日书摘：《人月神话》第 9–12 章

**第 9 章「五磅袋里装十磅」（Ten Pounds in a Five-Pound Sack）。** 在当时的机器上，内存大小是硬约束，程序体积必须当作与时间同等重要的资源来分配。表示法的选择，往往比小聪明式的压缩更决定空间效率。规模目标如果只压实现而不进入体系结构，很容易换来扭曲的结构。空间预算是设计问题，不只是编码纪律。

**第 10 章「文档假设」（The Documentary Hypothesis）。** 少数几份关键文件实际上就构成了项目：目标、规格、进度、预算、组织与空间分配等。对软件而言，目标、面向用户的规格或手册、进度、预算和组织图尤为要紧。把它们写下来，是为了迫使决策发生，而不是事后补行政手续。文件是项目本身的面目，不是项目的附属物。

**第 11 章「计划扔掉一个」（Plan to Throw One Away）。** 第一个系统几乎注定是试点，你总会扔掉一个，不如预先计划这样做。硬要把第一版直接当成交付产品，后续代价往往更大。程序在交付之后仍会演化，维护在很大程度上是再设计。进度和结构都应当把「会有第二版」考虑进去。

**第 12 章「锐利的工具」（Sharp Tools）。** 团队需要共享的工具和一位工具员，而不是每人自造一套环境。高级语言、交互式调试、公共的构建与测试手段，都是管理上应投资的事情。工具的锋利程度，会直接限制团队能达到的精度和速度。

明天（11 月 19 日，星期四）继续第 13–15 章：整体与部分、大祸临头，以及朝向用户的那一面——文档。

## 9. 今日总结

今天的信息环境是「旧线续报」和「新的系统事件」叠在一起。克里米亚大桥从昨日的遇袭，推进到部分垮塌；深圳 APEC 则从预告走进更具体的抵达与会晤窗口。英伟达那条线同时给出了两样东西：一份看起来仍然强劲的季报，以及「不请回黄仁勋、但安排他去国会作证」的人事安排。数字能安抚订单，听证则把芯片流向和国家安全问题继续留在公开议程上。

另一边，首页几乎被模型发布和故障占满。OpenAI 推出 GPT‑6.2，微软给出更便宜的编码模型，苹果则刚结束一轮被官方称为内部更新的服务中断；CNN 还报道了国家安全局内部网络的「临时降级」。它们不必被写成同一类事件，但放在一起读，会强化一个已经不新鲜的感觉：关键系统一旦出问题，解释往往滞后于影响面。Hacker News 上关于测试、harness 和验证的讨论，与《人月神话》今天读到的两章意外合拍——空间和工具都是设计问题，而第一个系统注定要被扔掉。读到第 9–12 章，本周的布鲁克斯还剩最后一天。
