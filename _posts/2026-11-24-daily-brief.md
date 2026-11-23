---
layout: post
title: "早报 · 2026-11-24"
date: 2026-11-24 08:00:00 +0800
category: daily
categories: [daily]
tags: [每日早报, 金融市场, 天气, 本地新闻, 全球头条, Hacker News, X, 微博, 油管访谈, 本月阅读]
collected_at: "2026-11-24 07:50:00 Asia/Shanghai (UTC+8)"
permalink: /2026/11/24/daily-brief/
excerpt_separator: "<!--more-->"
---

本期是 2026 年 11 月 24 日（星期二）的定时早报。金融市场、天气、微博热搜、Hacker News 与国际 RSS 的采集约在 07:37 Asia/Shanghai（UTC+8）；海淀区、昌平区本地新闻列表约在 07:37–07:38，原文页约在 07:40；X 热榜约在 07:38，科技圈检索约在其后不久；油管频道页约在 07:37，节目页约在 07:40。下文数字、标题与引语均来自当次抓取的公开来源；时间已换算为 Asia/Shanghai（UTC+8）。路透社 feeds.reuters.com 再次出现 TLS 连接失败，备用源返回 404；美联社经由 RSSHub 的源返回 403；《卫报》World RSS 返回 403；《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写；东方财富行情接口返回 502。均已在相应栏目说明。写稿时尚未到 09:15 中间价和 09:30 开盘，人民币中间价与 A 股本期采用 11 月 23 日（星期一）已公布的官方读数。

<!--more-->

## 1. 金融市场

黄金与市场化参考汇率的涨跌，按仓库行情档案中上一期早报的同源读数计算。人民币中间价与 A 股若来源已给出官方涨跌，变化栏仍以官方口径为主。今天是星期二，写稿时官方中间价和开盘价尚未公布，数值栏采用最近一次已公布的官方读数，并标明所属日期。本期快照将一并写入 docs/brief-memory/finance-history.json。

| 标的 | 数值 | 变化 | 说明与来源 | 时间 |
| --- | --- | --- | --- | --- |
| 黄金 XAU/USD | 3,633.90 美元/盎司 | 较上一期早报（2026-11-23 07:32:40 Asia/Shanghai (UTC+8)）+55.75（+1.56%） | [Gold-API](https://api.gold-api.com/price/XAU) 返回 3633.899902，报价单位为美元/盎司；updatedAt 为 2026-11-23T23:37:42Z（合 2026-11-24 07:37:42 Asia/Shanghai）。接口本身不提供涨跌，上表变化由本期读数减上一期同源快照（3,578.15）计算 | 2026-11-24 07:37:42 Asia/Shanghai (UTC+8) |
| 人民币汇率中间价 USD/CNY | 6.7120（11 月 23 日） | 较上一发布日（2026-11-20，6.7131）变动 −0.0011 | [中国外汇交易中心](https://www.chinamoney.com.cn/ags/ms/cm-u-bk-ccpr/CcprHisNew?startDate=&endDate=&currency=USD/CNY&pageNum=1&pageSize=5) 受权公布的**人民币汇率中间价**，不是银行柜台牌价，也不是盘中成交价。接口在 2026-11-24 07:37:46 返回的最新一条是 11 月 23 日的 6.7120；更早记录为 11 月 20 日 6.7131、11 月 19 日 6.7128、11 月 18 日 6.7118、11 月 17 日 6.7132。**本期采用 11 月 23 日已公布中间价**（写稿时尚未到当日 09:15 发布时间）。变化栏按官方上一发布日口径 | 采集 2026-11-24 07:37:46 Asia/Shanghai (UTC+8) |
| 市场化参考汇率 USD/CNY | 6.681345 | 较上一期早报（2026-11-22 08:02:32 Asia/Shanghai (UTC+8)）−0.012001（−0.18%） | [ExchangeRate-API](https://open.er-api.com/v6/latest/USD) 的**中间市场参考汇率**（mid-market reference），不是中国人民银行中间价，亦不可与上栏直接当成同一口径。time_last_update_utc 为 Mon, 23 Nov 2026 00:02:32 +0000（合 2026-11-23 08:02:32 Asia/Shanghai），较上一期早报所用的 11 月 22 日那一笔日更已刷新；time_next_update_utc 显示为 Tue, 24 Nov 2026 00:35:42 +0000（约合 08:35:42 Asia/Shanghai），采集时尚未到达 | 2026-11-23 08:02:32 Asia/Shanghai (UTC+8) |
| 上证指数 000001 | 3538.95 | +5.16（+0.15%） | [腾讯财经](https://qt.gtimg.cn/q=sh000001,sz399001) 返回：最新价 3538.95，涨跌 +5.16，涨跌幅 +0.15%，昨收 3533.79，开盘 3503.52，最高 3544.60，最低 3476.65，行情时间戳 20261123161427（2026-11-23 16:14:27）。[新浪财经](https://hq.sinajs.cn/list=s_sh000001,s_sz399001) 交叉核对价格一致（3538.9480，涨跌 +5.1551），涨跌幅同为 +0.15%。[东方财富](https://push2.eastmoney.com/api/qt/ulist.np/get?fltt=2&invt=2&secids=1.000001,0.399001&fields=f2,f3,f4,f12,f14,f15,f16,f17,f18) 本次返回 502，故不以它为数值来源。写稿时尚未开盘，**本期采用 11 月 23 日（星期一）收盘价，不是今日盘中或开盘价** | 采集 2026-11-24 07:37:46 Asia/Shanghai (UTC+8) |
| 深证成指 399001 | 10454.37 | +197.98（+1.93%） | 同上来源：腾讯财经最新价 10454.37，涨跌 +197.98，涨跌幅 +1.93%，昨收 10256.39，开盘 10155.60，最高 10510.18，最低 10118.02，行情时间戳 20261123161403（2026-11-23 16:14:03）。新浪财经交叉核对价格与涨跌幅一致 | 采集 2026-11-24 07:37:46 Asia/Shanghai (UTC+8) |

现货黄金较上一期早报再升约 1.56%，报 3,633.90 美元/盎司。市场化参考汇率随接口日更从 11 月 22 日那一笔刷新为 11 月 23 日的 6.681345，较上一期所用读数回落 0.18%。官方中间价本期改用 11 月 23 日已公布的 6.7120，较 11 月 20 日中间价下调 0.0011；A 股本期采用 11 月 23 日收盘价，上证微涨 0.15%，深成指上涨 1.93%。这些官方数字都不是今日开盘或收盘。
## 2. 天气与本地新闻

### 北京市区天气预报

预报城市为北京市区。数值来自[中国气象局城市预报（站点 54511，名称「北京」）](https://weather.cma.cn/web/weather/54511.html)的公开接口 [/api/weather/view?stationid=54511](https://weather.cma.cn/api/weather/view?stationid=54511)。站点路径为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不是海淀或昌平区站。接口返回的 lastUpdate 为 2026/11/24 07:25；本次采集时间为 2026-11-24 07:37:46 Asia/Shanghai（UTC+8）。温度单位为摄氏度。风速按该局页面所用单位记为米/秒，气压按页面所用单位记为百帕。

中国气象局该接口未提供空气质量，本期不另引其他来源的 AQI，以免把不同站点的读数混进北京市区预报。预警列表为空。

**当前实况**（lastUpdate 2026/11/24 07:25）：气温 0.5℃，体感温度 −3.3℃，相对湿度 30%，东北风微风，风速 2.4 米/秒，降水量 0.0，气压 1029.0 百帕。

**今日（11 月 24 日）预报**：白天晴，最高 7℃，西南风微风；夜间晴，最低 −3℃，西南风微风。

**未来三天展望：**

| 日期 | 天气 | 高温 / 低温 | 风 |
| --- | --- | --- | --- |
| 11 月 25 日 | 白天晴，夜间多云 | 10℃ / −1℃ | 白天东北风微风，夜间北风微风 |
| 11 月 26 日 | 白天晴，夜间晴 | 12℃ / 0℃ | 白天西风微风，夜间西北风 3～4 级 |
| 11 月 27 日 | 白天多云，夜间阴 | 12℃ / −2℃ | 白天西北风微风，夜间北风微风 |

日预报对象未给出降水量字段，故不编造未来几天的雨量。

### 海淀区与昌平区本地新闻

写稿前已对照 docs/brief-memory/seen.json。昨日及此前已写过的海淀区党代会安排、人大代表视察、医保钱包 2.0、未名·AI Park、与中国航油签约，以及昌平的融合教育研讨、地下空间议事、溜石港观星、龙泽园挖蛹、南口古树与防火等，不再重复。今天海淀要闻栏终于出现了 11 月 23 日见报的近日稿；昌平则有脑机接口大会、劳务品牌和社区抢险等新稿。白羊城蓄滞洪区完工此前已写过，即使换了链接也不再写。

#### 海淀区

**[北京「光影智谷」暨环北影文化创新生态圈共建启动](https://zyk.bjhd.gov.cn/ywdt/hdyw/202611/t20261123_4836110.shtml)**。来源：海淀报，日期 2026-11-23 09:18。稿件称，11 月 21 日下午，共建仪式在中交海淀科创园举行，北京市广播电视局、海淀区和北京电影学院负责人出席。报道写，环北影文化创新生态圈以中交海淀科创园、中影园区为核心，盘活 19 万平方米存量载体；现场还揭牌海淀区「人工智能+文化」生态服务站，稿件称之为北京首个集游戏电竞、短剧影视、「AI+文化」于一体的专业平台。文中提到海淀区联合火山引擎共建 AI 视听产业链，中交海淀科创园「光影社区」推出「千万级」专项扶持资金，并有海新域与麦芽传媒旗下平台签约。这些面积、定位和「千万级」等表述来自报道本身，不是已完成的产业统计公报。

**[海淀教育创新人才培育工程（第二期）结业](https://zyk.bjhd.gov.cn/ywdt/hdyw/202611/t20261123_4836105.shtml)**。来源：海淀报，日期 2026-11-23 09:17。11 月 21 日上午，结业活动暨「新时代校长培养模式研讨会」在北京市十一学校举行，区委书记王少峰出席。报道称，第二期学制三年，学员围绕学校价值构建、治理体系、课程开发和人机协同下教师角色等主题研修，结业现场颁发证书并展出办学治理、课程创新、五育融合、AI 赋能教学等方面的成果。王少峰在报道中谈到「五乐」一体建设（乐享课堂、乐育校园、乐野体育、乐学公园、乐知城市）。这是一期干部研修结业报道，不是对全区教育质量的评估结论。

**[以精细化治理提升群众出行获得感 区领导调研交通治理工作](https://zyk.bjhd.gov.cn/ywdt/hdyw/202611/t20261123_4836104.shtml)**。来源：海淀报。区领导先后到清河绿道、肖家河桥北、中关村北大街与清华西路交叉口，了解沿河路网、桥下空间和沿线功能提升进展。报道转述，调研强调蓝绿空间与道路衔接、盘活通行资源、用数字化手段把交通安全从「末端管理」转向「前端治理」。这是一次工作调研报道，不是某条道路已经完工或拥堵已经消除的通报。

#### 昌平区

**[脑智芯联·机遇昌平｜2026脑机接口大会在昌平开幕](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112116375932049/index.html)**。来源：北京昌平 APP，发布于 2026-11-21。稿件称，大会 11 月 21 日开幕，现场集中发布「北脑一号」智能脑机系统、非侵入式高精度脑电采集计算芯片等 15 项 2026 年国内脑机接口标志性成果，并发布《2026 脑机接口创新发展研究报告》；同时启动人才培育评价和高质量数据两个公共服务平台，为创新大赛 8 个赛道的 66 支获奖队伍颁奖。报道还给出一组区域产业数字：落地相关企业 49 家、公共服务平台 14 个，以及「3+11+13」产业体系等，这些均来自区政报道本身。[次日续稿](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112216363233999/index.html)写，11 月 22 日举办创新产品专场，15 项成果覆盖辅助诊断、神经信号采集、侵入式与非侵入式接口等方向，并同期举行 10 场平行分论坛。成果评价和技术指标以主办方和报道口径为准，这里不做独立核验。

**[昌平劳务品牌再添「新成员」 10名乡土人才当选首批「京昌文旅推介官」](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112216381542702/index.html)**。来源：北京昌平 APP，发布于 2026-11-22。11 月 20 日，「京昌文旅推介官」服务站揭牌，首批 10 名推介官当选，首期示范班 30 名学员进站培训。报道称，该项目面向种植大户、合作社社员、返乡青年等，由昌平职业学校等提供师资，培训短视频拍摄和直播话术，服务站实训与乡村实地教学并行。区人力社保局相关负责人在稿中介绍，推介官既可讲解乡村线路，也可推介苹果、草莓等地标农产品。文中还把「京昌家政」「京城消控卫士」「阳坊涮肉」「京昌飞手」与这一新品牌并列为五大劳务品牌，并称累计已带动千余人就业、预计两年内带动 3000 余人稳定就业。这些人数和预期来自报道本身。

**[东小口镇部署美国白蛾越冬蛹清除专项行动](https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/2026112114122265411/index.html)**。来源：北京昌平 APP，发布于 2026-11-21。这与昨日写过的龙泽园街道社区挖蛹是同一季节性防治主题下的另一处部署，不是同一场活动的重复稿。报道写，东小口镇 11 月 17 日召开推进会，要求按「台账清、技术准、责任实、动员广」排查树干根部、墙缝和砖石杂物堆等点位，实行一点一档、销号管理，并强调不要因「冬季无虫」而松劲。这是镇级工作部署，不是全区虫害统计。

**[深夜跑水漫楼道，房主却在外地！社区这场联合抢险，稳稳接住了居民的急难愁盼](https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/2026112312042787445/index.html)**。来源：北京昌平 APP，发布于 2026-11-23。稿件写，回龙观街道新康园社区 8 号楼一户居民家近日晚 9 点多暖气阀门接口老化开裂，门缝向外溢水，房主当时在外地。邻居报信后，社区、物业和供暖维修人员在征得入户同意后关阀换件、清理积水，并把现场情况同步给房主。这是一条社区应急处置报道，细节以稿件为准，不引申为全区供热事故统计。
## 3. 全球头条

路透社世界新闻 RSS 本次 TLS 连接失败，备用源返回 404；美联社经由 RSSHub 的源返回 403；《卫报》World RSS 也返回 403，这三家不写入正文。《纽约时报》World RSS 可用，但正文页返回 403，相关条目只根据 RSS 标题与摘要改写，不假装读过全文。

**续报：英伟达董事会宣布黄仁勋立即复职。** 前几期已写过黄仁勋去职、回归传闻和董事会一度排除复职的表态，当时部分消息只能标为流传。11 月 23 日，这件事有了公司正式声明。[英伟达新闻室](https://nvidianews.nvidia.com/news/nvidia-board-reinstates-jensen-huang-as-president-ceo-and-board-director)当天宣布，董事会一致投票，立即恢复 Jensen Huang（黄仁勋）的总裁、首席执行官和董事职务；声明写，董事会在与他一系列讨论后「对其坦诚和领导能力感到满意」，并在决策过程中听取了「美国政府高层」意见，据此认为复职「不构成国家安全风险」。董事长 Harvey C. Jones 说，董事会相信他是领导公司的合适人选，并感谢 Colette Kress 担任临时首席执行官，同时她将继续担任首席财务官。黄仁勋的声明则说，他「怀着最大的谦卑和重新的承诺」回到公司。声明同时重申：鉴于此前关于他成为外国情报工作目标的报道，由独立董事组成的调查委员会及其独立律师的调查将进行到结束，他承诺配合；董事会还新设国家安全与出口管制委员会，并开始寻聘向提名与公司治理委员会汇报的首席合规官。[CNBC](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) 11 月 23 日 8:59 AM EST（合 21:59 Asia/Shanghai）报道，该公司股票当天收涨 31%；并称自黄仁勋 11 月 8 日向员工承认一段婚外情以来，股价累计下跌近 33%。CNBC 还引述特朗普当天对该台表示，他「直接和间接」与董事会沟通过，认为黄仁勋「没有做错」；特朗普称周日与黄仁勋通了话，并要他承诺「努力工作」。报道把 11 月 13 日辞职、纽约时报关于 Alice Huang（与黄仁勋无亲属关系）的报道，以及律师事务所 Wachtell, Lipton, Rosen & Katz 协助的独立董事调查，作为背景写下，并写明调查仍将进行到底。这些股价、时间线和引语来自英伟达声明与 CNBC，不是对调查结论的预判。[BBC 中文](https://www.bbc.com/zhongwen/articles/cqvg2947xvx0o/simp) 也作了复职报道，标题写「辞职 11 天后重掌 Nvidia」。

**续报：美国商务部拟将 Megaspeed 列入实体清单。** 前几期已写过英伟达合作伙伴 Megaspeed 受到出口管制调查。[BBC](https://www.bbc.co.uk/news/articles/cv98xpg5dg5zo) 11 月 23 日 22:15 GMT（合 2026-11-24 06:15 Asia/Shanghai）报道，美国商务部宣布打算把新加坡公司 Megaspeed Ltd 列入禁止在美买卖商品的黑名单，其子公司 Speedmatrix 也被列入；生效时间在商务部公告中并未写明。BBC 写，商务部称对该公司的调查已进行近两年，怀疑其协助把英伟达先进 AI 芯片转往中国；中国已被限制购买此类技术。报道还写，该公司近期因前高管 Alice Huang 与黄仁勋的关系而受到更多关注，并称阿里巴巴「据报道」是其最大客户之一。中国方面则否认相关间谍指控，并警告不要以此为「技术封锁」的借口。这些都是政府意向和媒体转述，名单何时生效、指控是否成立，仍以主管部门后续文件为准。BBC 还提到，黄仁勋和英伟达首席法律官接下来还将出席众议院外交事务委员会的闭门说明会。

**续报：班加西遇袭之后，泽连斯基称作「示范行动」。** 昨日已写过俄罗斯轻护舰 Merkury 在利比亚班加西港疑遭无人机袭击、船体倾覆的报道，当时乌克兰是否实施袭击仍待其官方说明。[BBC](https://www.bbc.co.uk/news/articles/cm894p88jzxpo) 今天的分析稿写，这次夜间袭击由乌克兰国家安全局（SBU）与武装力量协调，总统泽连斯基称之为 “an exemplary operation”（示范行动）；俄罗斯则称这是「危险的升级」。报道还写，一同停泊的一艘货船也遭到打击；联合国利比亚特派团已表示「深切关注」。安全记者 Frank Gardner 指出，舰船停在由亲莫斯科的哈利法·哈夫塔尔控制的东部港口，而利比亚并非俄乌战争的当事方。文中把此事与上周末芬兰湾货船 Sparta II 遇袭、乌克兰此前对乌斯特-卢加石油终端和「蛛网行动」等远程打击放在一起观察，认为战争的地理边界已在扩大，但这些类比是分析，不是对新的袭击清单的独立核实。[《纽约时报》RSS](https://www.nytimes.com/2026/11/23/world/europe/ukraine-libya-russian-ships.html) 摘要称，泽连斯基表示乌克兰无人机击沉了一艘轻护舰并击中一艘干货船，行动有特种部队参与；该文正文页本次打不开，只根据 RSS 改写。

**[Iranian authorities flog singer who performed without hijab, lawyers say](https://www.bbc.co.uk/news/articles/cq1j6585l5g6o)**（BBC）。律师向 BBC 表示，著名歌手 Parastoo Ahmadi 及四名乐队或制作团队成员，已在库姆（Qom）被处以每人 74 下鞭刑。报道写，Ahmadi 在 2024 年 12 月直播演唱会上未按强制规定佩戴头巾、穿着无袖裙装；今年 6 月库姆一家刑事法庭认定她与另外八人「通过发布淫秽不雅材料冒犯公共风化」，除鞭刑外还被禁止视听活动并禁足出国两年，9 月底上诉被驳回。辩护律师对 BBC 说，他们争取改判、减刑或暂缓执行都没有成功。人权组织指责鞭刑构成残忍、不人道和有辱人格的处罚。这些细节来自律师转述和 BBC 报道，伊朗官方当天的单独说明本期未另核到。

**[Search and rescue teams race against time to find survivors after Nigeria boat tragedy](https://www.bbc.co.uk/news/articles/cq7820xjm49po)**（BBC，文中标注 2026-11-23 11:38 GMT，合 19:38 Asia/Shanghai）。尼日利亚国家应急管理署（NEMA）发言人对 BBC 表示，一艘载着前往葬礼的乘船者周五倾覆后，目前已寻获 29 具遗体、救出 50 人，搜救仍在进行。警方称船只从 Ayama 社区出发后出现机械故障。政府已下令加强对内河航道安全标准的执行。报道指出，超载、维护不足和不遵守安全规定，此前也曾造成致命事故。具体地点在 Bayelsa，人数以应急管理部门当次口径为准，后续可能还会更新。

**[India pledges $1.6bn to Nepal in reset of ties](https://www.bbc.co.uk/news/articles/cwx2ervemj4ko)**（BBC）。报道写，印度总理莫迪承诺向尼泊尔提供近 16 亿美元支持，其中大部分是能源项目信贷额度，另有约 4 亿美元赠款用于重建和基础设施。背景是尼泊尔新总理、前说唱歌手 Shah 的首次访印，以及该国在灾害后面临据政府估计高达 48 亿美元的重建需求。报道注意到，边界争议在公开讲话中基本被搁置，联合声明只承认仍有未决问题。这些金额和表述来自 BBC 对访问成果的报道。

**续报：墨西哥士兵在「Chapo Isidro」被捕后遇袭。** 前几期已写过 Fausto Isidro Meza Flores（「Chapo Isidro」）在锡那罗亚枪战中被捕。[BBC](https://www.bbc.co.uk/news/articles/c5rmgkv2lk73o) 11 月 23 日报道，国防部称士兵周日在 Sinaloa de Leyva 巡逻时遭到射击，随后扣押了 8 名涉嫌参与报复性暴力的人员，其中一人未成年，并缴获 6 辆车，其中 2 辆装有防弹装甲和枪塔。国防部长周一更新的数字是：抓捕行动中的枪战造成 4 名士兵和 16 名「有组织犯罪成员」死亡；Meza Flores 及其副手「Serafín」、财务操盘人已被空运至墨西哥城。美国司法部称这次抓捕是「一场壮观的军事行动」。被捕后当地出现设障、焚车和交火。这些伤亡和扣押数字以墨国防部当次通报为准。

《纽约时报》本期还有若干 World 头条，正文页均返回 403，只根据 RSS 记下，不作展开：[分析称超过 70 万俄罗斯士兵已在乌克兰战争中死亡](https://www.nytimes.com/2026/11/23/world/europe/russia-ukraine-war-deaths.html)，摘要写依据是被黑客获取的政府数据；[哥伦比亚库库塔发生无人机袭击，至少三人受伤](https://www.nytimes.com/2026/11/23/world/americas/colombia-drone-attack-cucuta.html)，摘要称联合国报告该国无人机爆炸袭击增加了 445%；[中国人工智能焦虑背后对核力量被「将死」的担忧](https://www.nytimes.com/2026/11/23/world/asia/china-us-nuclear-ai.html)；以及[内塔尼亚胡是否应再攻伊朗的评论](https://www.nytimes.com/2026/11/23/world/middleeast/netanyahu-israel-iran.html)。印尼糖果厂火灾已在昨日写过，纽约时报今天的 RSS 仍是同一事件，不另作续报。
## 4. Hacker News

当前首页来自 [Algolia 前端接口](https://hn.algolia.com/api/v1/search?tags=front_page&hitsPerPage=30)，采集于 2026-11-24 07:37:46 Asia/Shanghai（UTC+8）。对讨论最热或点数最高的条目打开了原文；其余用短列表列出。昨日已写过的 C++26 会议报告等不再展开。

**[Nvidia Reinstates Jensen Huang as CEO](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html)**（[HN 讨论](https://news.ycombinator.com/item?id=50611576)，1893 点 / 2995 则评论）  
与全球头条中的复职声明为同一事件，这里不重复叙述。首页上它是当前讨论量最大的条目，评论区主要围绕董事会转向、股价反弹和调查是否还会改变结局，不把评论当成新的事实来源。

**[Ladybird is now in alpha](https://ladybird.org/posts/alpha/)**（[HN 讨论](https://news.ycombinator.com/item?id=50614249)，1270 点 / 310 则评论）  
Andreas Kling 在 2026-11-23 的官方博文中宣布，独立浏览器 Ladybird 进入 alpha，可在 macOS 和 Linux 上下载。他强调引擎是从头编写、不是其他浏览器的分叉；浏览器本身「谦逊但能用」。文章写明这是 alpha：有的网站打不开，有时会崩溃，并欢迎在浏览器用内置入口报告问题。文中还写「我们希望安全研究者来攻击它」，并明确「今天不对安全性作承诺」。alpha 是滚动更新通道，不必再从源码编译才能看到新进展。

**[GLM-5.4: Toward generalized coding with our first loop transformer](https://z.ai/blog/glm-5.4)**（[HN 讨论](https://news.ycombinator.com/item?id=50609685)，1017 点 / 332 则评论）  
智谱 / Z.ai 2026-11-23 的研究博文称，GLM-5.4 是该公司首个建立在 Loop Transformer 上的旗舰模型：把 GLM-5 基座中的 28 层循环迭代两次，参数规模写法为 750B。博文宣称其「智力水平可与 2T–3T 参数模型相比」，并说这是「Generalized Coding」的起点，也就是把编程能力推广到视频生成、游戏制作、三维建模和机械设计等任务。这些对比、演示和架构细节都是出品方的说法，不是独立评测。文中也承认模型容易陷入过长的「马拉松式思考」，同时表示权重要在安全加固后「负责任地」开源，API「即将推出」。

**[Dario is hyping the dangers so OSS models are illegal and he stays in control](https://x.com/ylecun/status/2124550037912920090)**（[HN 讨论](https://news.ycombinator.com/item?id=50615308)，955 点 / 553 则评论）  
这是 Yann LeCun 2026-11-22 17:06 UTC（合 2026-11-23 01:06 Asia/Shanghai）的一则长帖，采集时约 2.2 万赞、3142 次转发。他批评 Anthropic 的 Dario Amodei「从 GPT-2 以来就把危险性说得很满，为的是让开源模型被定为非法、好让他自己保持控制」，并比喻为奥斯曼帝国禁止阿拉伯文印刷术。这是公开意见，不是对监管立法的事实报道，也不代表已有相应禁令。

**[Free alternative TV network built from the Internet Archive's forgotten videos](https://spelunkr.tv)**（[HN 讨论](https://news.ycombinator.com/item?id=50606192)，920 点 / 159 则评论）  
网站自称 SPELUNKR，首页定位是「有线电视，但更怪一些」，把互联网档案馆里较少被翻出的影像编成可连续观看的频道。本期打开了站点本身，未再逐条核对其片源授权，只把它作为一项在线实验记下。

**[Per Arm's request, this site will be discontinued on 4 December 2026 :(](https://arm.jonpalmisc.com/)**（[HN 讨论](https://news.ycombinator.com/item?id=50617499)，761 点 / 154 则评论）  
Jon's Arm Reference 是一份 AArch64 指令与系统寄存器的查阅站。站长 Jon 在首页写，Arm 的律师已通知他在 2026 年 12 月 4 日前关闭网站，否则将面临法律行动；他感谢多年来的读者，并说会寻找尽量保住书签和链接的办法。这是站长对律师函的说明，不是法庭判决摘要。

**[Apple removed my open-source app from EU App Stores after 9 years](https://github.com/glushchenko/fsnotes/discussions/2056)**（[HN 讨论](https://news.ycombinator.com/item?id=50616933)，458 点 / 96 则评论）  
开源笔记应用 FSNotes 的作者在 GitHub Discussions 发帖称，这款已上架约九年的应用被苹果从欧洲区 App Store 下架，且他的支持请求未得到回应。具体审核理由和苹果方面的说明，本期未见公司官方页面，只根据开发者帖文记录，不把下架写成已公布的政策结论。

**[Kagi Mail (public beta)](https://blog.kagi.com/kagi-mail-public-beta)**（[HN 讨论](https://news.ycombinator.com/item?id=50615481)，314 点 / 244 则评论）  
Kagi 宣布其邮件与日历服务进入公开测试：可使用 @kagimail.com 或自有域名。官方博文称，可免费试用 60 天，之后为每年 99 美元（另加销售税），Kagi Ultimate 订阅已包含此项；并强调无广告、无监控、开放标准、不锁定。这些价格和承诺来自公司公告。

**[Spacecraft reaches Mercury on second-ever mission to enter its orbit](https://www.theguardian.com/science/2026/nov/20/spacecraft-mercury-second-ever-mission-orbit-bepicolombo)**（[HN 讨论](https://news.ycombinator.com/item?id=50587439)，272 点 / 85 则评论）  
标题指向欧日联合任务 BepiColombo 进入水星轨道。原卫报正文页本次返回 403，无法核对细节，这里只保留首页标题与链接，不编造到达时间和科学成果。

**[Nospeaker ─ Make your MacBook's trackpad talk using its haptic motor](https://github.com/os6/nospeaker)**（[HN 讨论](https://news.ycombinator.com/item?id=50610318)，263 点 / 154 则评论）  
项目说明写，MacBook 触控板里没有扬声器，只有用于模拟点击的触觉马达；Nospeaker 把该马达驱动到每秒约 4000 次，从而发出可听见的「说话」声。作者提醒先把电脑静音、把笔记本放在桌上，并用一行脚本安装体验。这是作者对自己实验的说明。

**[Win4wine – Run Windows Shell as the Linux Desktop on Wine](https://github.com/mikuta0407/win4wine)**（[HN 讨论](https://news.ycombinator.com/item?id=50610743)，207 点 / 107 则评论）  
作者把它定位为个人实验：在打过补丁的 Wine 上，把 Windows XP 的 explorer.exe 当作 Linux 桌面壳来跑，任务栏、开始菜单和文件夹窗口来自 XP 本身，Linux 应用也可以出现在这套界面里。项目不附带微软文件，需用户自备 XP 的 ISO；也可用 ReactOS 或实验性的 Windows 7 壳。说明明确写，目前只在新装的 Debian 13 加官方脚本的环境里验证过，不建议当作日常桌面。

**[VP ≠ VNP over Every Field](https://github.com/anthropics/formal-math/tree/main/vp-vnp)**（[HN 讨论](https://news.ycombinator.com/item?id=50620102)，136 点 / 91 则评论）  
Anthropic 在 GitHub 仓库 formal-math 中放上一份题为 VP ≠ VNP over every field 的论文和 Lean 4 形式化。页面声称：在每个域上，哈密顿回路多项式以及特征不为 2 时的永久式，都需要超过某个次多项式门槛的门数，从而 VP 是 VNP 的真子集。仓库同时写明：这并不解决 P 与 NP；结果由内部研究用 Claude 模型发现，论文和 Lean 均由 AI 模型撰写，「尚无人类数学家核验证明」；并称其为研究工件、不接受外部贡献。这与近日黎曼猜想形式化风波是不同的问题，但同样只能标为尚未经人审的主张，不能写成定理已被证明。

**续报：Levent Alpöge 就自己的黎曼猜想形式化发帖说明。** 前几期已写过他宣称与 Claude 完成广义黎曼猜想的 Lean 形式化，以及 Lean 社区的核验声明，当时就强调仍不是期刊发表。[他在 X 上的帖文](https://x.com/__alpoge__/status/2124987173439209561)（2026-11-23 22:03 UTC，合 2026-11-24 06:03 Asia/Shanghai；[HN 讨论](https://news.ycombinator.com/item?id=50620250)）说，文中「25 万页以上」是一句玩笑，大家却当真了；Lean 代码「显然充满垃圾，但能编译」，对这类批评他表示接受，并承认应当先清理。这则自我说明降低了「篇幅神话」的分量，并没有宣布证明已经完成或被接受。

**其余首页条目：**

- [NariQ: BF16-level Qwen3.8-27B in a 10 GB file](https://huggingface.co/nari-labs/Qwen3.8-27B-NariQ-GGUF)（[HN](https://news.ycombinator.com/item?id=50611402)，105 点 / 20 则评论）— 作者称把 Qwen 模型量化进约 10 GB 文件；压缩比和精度是项目自己的说法。
- [Stalwart is now a drop-in replacement for Microsoft Exchange](https://stalw.art/blog/microsoft-exchange-replacement/)（[HN](https://news.ycombinator.com/item?id=50620349)，63 点 / 27 则评论）— 开源邮件服务器宣称可替代 Exchange，兼容程度以项目文档为准。
- [GPUI is getting its own repository](https://github.com/zed-industries/gpui)（[HN](https://news.ycombinator.com/item?id=50619103)，62 点 / 8 则评论）— Zed 把界面框架 GPUI 拆到独立仓库。
- [Derivative Flipping](http://blog.sigfpe.com/2026/11/derivative-flipping.html)（[HN](https://news.ycombinator.com/item?id=50594935)，60 点 / 6 则评论）— 一篇数学与编程随笔。
- [Bored.com: Fun, interesting and cool websites to explore when bored](https://www.bored.com/)（[HN](https://news.ycombinator.com/item?id=50619207)，58 点 / 16 则评论）— 旧目录站重新出现在首页。
- [The horse made the state](https://aeon.co/essays/the-origins-of-the-state-are-not-agrarian-but-pastoralist)（[HN](https://news.ycombinator.com/item?id=50619186)，48 点 / 48 则评论）— Aeon 文章讨论国家起源与游牧而非农耕的关系。
- [How should an LLM see a computer?](https://www.greptile.com/blog/trex-computer-use)（[HN](https://news.ycombinator.com/item?id=50615520)，37 点 / 21 则评论）— 讨论语言模型应如何「看见」计算机界面。
- [Show HN: Hermit CRM – Free open-source CRM for solopreneurs](https://hermitcrm.io/)（[HN](https://news.ycombinator.com/item?id=50609708)，30 点 / 2 则评论）
- [What does it mean to understand what we built?](https://brooker.co.za/blog/2026/11/16/understanding.html)（[HN](https://news.ycombinator.com/item?id=50595365)，16 点 / 4 则评论）
- [Show HN: Type-C – variants, options, generics and pattern matching for C](https://github.com/stass/type-c)（[HN](https://news.ycombinator.com/item?id=50602561)，13 点 / 1 则评论）
- [The AI conversation we're not having](https://www.gnanaguru.com/blog/things-two-years-in-ai-taught-me/)（[HN](https://news.ycombinator.com/item?id=50619838)，11 点 / 5 则评论）
- [Next gaming monitor should still be an OLED](https://www.rockpapershotgun.com/theyre-more-complicated-and-more-expensive-than-lcd-screens-but-your-next-gaming-monitor-should-still-be-an-oled)（[HN](https://news.ycombinator.com/item?id=50618798)，10 点 / 4 则评论）
## 5. X 热门与科技圈

全球及美国热榜来自 X 公共趋势接口，采集约在 07:38 Asia/Shanghai（UTC+8）。中国地区 WOEID 本次返回的内容与全球榜高度重合，无法当作独立的中国趋势。未核实的传言只标明在流传。

全球榜和美国榜都被 **[Nvidia](https://x.com/search?q=Nvidia)**（约 63.0 万帖）和 **[Jensen](https://x.com/search?q=Jensen)**（约 77.1 万帖）占据，美国榜上还有 **[NVDA](https://x.com/search?q=NVDA)**（约 18.0 万帖）。这与英伟达董事会宣布黄仁勋复职、美股随芯片股反弹是同一条新闻，事实以公司声明和主流报道为准，不把热榜上的涨跌预测当成收盘数据。美国榜另外出现 **[WALL-API-1.0](https://x.com/search?q=WALL-API-1.0)**、**[WALL-OSS-1.0](https://x.com/search?q=WALL-OSS-1.0)** 和 **[X Square Robot](https://x.com/search?q=X%20Square%20Robot)**。深圳公司自变量机器人（X Square Robot）在[官方博文](https://x2robot.com/blogs/wall-oss-1-en/)中称，于 2026-11-23 发布视觉—语言—动作基础模型 WALL-OSS-1.0，并称在评估者自选的 312 项真实机器人任务上取得 55.1% 的零样本成功率，同时提供 WALL-API-1.0 接口。这些成功率和任务口径是出品方的说法，不是独立评测；热榜上大量转述帖也多在重复同一组数字。

全球榜其余条目以节庆和体育为主，如 [Thanksgiving](https://x.com/search?q=Thanksgiving)（约 18.2 万帖）、西班牙电视辩论话题 [#DebateA8RTVE](https://x.com/search?q=%23DebateA8RTVE)、日本「連休明け」「和食の日」，以及足球和摔角标签。美国榜上的 [#WWERaw](https://x.com/search?q=%23WWERaw)、[X-Men](https://x.com/search?q=X-Men)、[Cyclops](https://x.com/search?q=Cyclops) 和若干球员姓名，同样偏娱乐与赛事，不展开。

科技圈讨论除复职本身外，还有两则与 Hacker News 交叉的帖文：Yann LeCun 对 Dario Amodei 开源政策的批评，以及 Levent Alpöge 就「25 万页」玩笑所作的说明，均已在 HN 栏写过，这里不重复展开。Geoffrey Hinton 向议员闭门简报、以及「AI 将让人大规模失业」等话题，也出现在 X 的新闻摘要里，但多为二手转述，本期未打开原始简报或访谈，不当成已核验的新宣言。

## 6. 微博热搜

接口 [weibo.com/ajax/side/hotSearch](https://weibo.com/ajax/side/hotSearch) 在 2026-11-24 07:37:46 Asia/Shanghai（UTC+8）返回成功（ok=1）。置顶/政务与自然热搜、广告已按接口字段区分；下列链接指向 s.weibo.com 搜索页。

**置顶或政务。** [三个时间坐标读懂APEC中国年](https://s.weibo.com/weibo?q=%23%E4%B8%89%E4%B8%AA%E6%97%B6%E9%97%B4%E5%9D%90%E6%A0%87%E8%AF%BB%E6%87%82APEC%E4%B8%AD%E5%9B%BD%E5%B9%B4%23) 带「热」标，是对刚刚结束的 APEC 相关宣传话题，前几期已写过深圳会议本身，这里只作为置顶话题记下，不把标语写成新的成果清单。

**科技、国际与社会。** 热搜前排几乎被英伟达复职占满：[黄仁勋复职原因](https://s.weibo.com/weibo?q=%E9%BB%84%E4%BB%81%E5%8B%8B%E5%A4%8D%E8%81%8C%E5%8E%9F%E5%9B%A0)（热，约 198 万）、[黄仁勋恢复英伟达CEO职务](https://s.weibo.com/weibo?q=%E9%BB%84%E4%BB%81%E5%8B%8B%E6%81%A2%E5%A4%8D%E8%8B%B1%E4%BC%9F%E8%BE%BACEO%E8%81%8C%E5%8A%A1)（热，约 32 万）、[黄仁勋称会成为更优秀的CEO](https://s.weibo.com/weibo?q=%E9%BB%84%E4%BB%81%E5%8B%8B%E7%A7%B0%E4%BC%9A%E6%88%90%E4%B8%BA%E6%9B%B4%E4%BC%98%E7%A7%80%E7%9A%84CEO)、[马斯克回应黄仁勋重任英伟达CEO](https://s.weibo.com/weibo?q=%E9%A9%AC%E6%96%AF%E5%85%8B%E5%9B%9E%E5%BA%94%E9%BB%84%E4%BB%81%E5%8B%8B%E9%87%8D%E4%BB%BB%E8%8B%B1%E4%BC%9F%E8%BE%BACEO)，以及 [美股芯片股涨疯了](https://s.weibo.com/weibo?q=%E7%BE%8E%E8%82%A1%E8%8A%AF%E7%89%87%E8%82%A1%E6%B6%A8%E7%96%AF%E4%BA%86)、[美股集体暴涨原因](https://s.weibo.com/weibo?q=%E7%BE%8E%E8%82%A1%E9%9B%86%E4%BD%93%E6%9A%B4%E6%B6%A8%E5%8E%9F%E5%9B%A0)。事实仍以英伟达声明和 CNBC 等报道为准；热搜标题里的「原因」「涨疯了」只说明讨论很热，不是对盘中或盘后涨幅的官方统计。[英伟达空头单日预亏122亿美元](https://s.weibo.com/weibo?q=%E8%8B%B1%E4%BC%9F%E8%BE%BE%E7%A9%BA%E5%A4%B4%E5%8D%95%E6%97%A5%E9%A2%84%E4%BA%8F122%E4%BA%BF%E7%BE%8E%E5%85%83) 是热搜标题中的估算数字，本期未核对这些空头头寸的原始数据，只作为流传中的说法。[特斯拉FSDv15识别小动物](https://s.weibo.com/weibo?q=%E7%89%B9%E6%96%AF%E6%8B%89FSDv15%E8%AF%86%E5%88%AB%E5%B0%8F%E5%8A%A8%E7%89%A9) 与前几日已写过的 FSD V15 话题相邻，未见新的公司公告，不展开。[特朗普把抵达深圳照片打印出来了](https://s.weibo.com/weibo?q=%E7%89%B9%E6%9C%97%E6%99%AE%E6%8A%8A%E6%8A%B5%E8%BE%BE%E6%B7%B1%E5%9C%B3%E7%85%A7%E7%89%87%E6%89%93%E5%8D%B0%E5%87%BA%E6%9D%A5%E4%BA%86)、[特朗普深圳行后劲真大](https://s.weibo.com/weibo?q=%E7%89%B9%E6%9C%97%E6%99%AE%E6%B7%B1%E5%9C%B3%E8%A1%8C%E5%90%8E%E5%8A%B2%E7%9C%9F%E5%A4%A7) 是 APEC 会后的余波话题，细节未核到原帖或官方相册说明。[猝死女教师每天在校超15个小时](https://s.weibo.com/weibo?q=%E7%8C%9D%E6%AD%BB%E5%A5%B3%E6%95%99%E5%B8%88%E6%AF%8F%E5%A4%A9%E5%9C%A8%E6%A0%A1%E8%B6%8515%E4%B8%AA%E5%B0%8F%E6%97%B6) 涉及具体个案，本期未打开权威调查或校方通报，不根据标题写原因。[县委书记走访红糖厂家说捡点渣渣吃](https://s.weibo.com/weibo?q=%E5%8E%BF%E5%A7%94%E4%B9%A6%E8%AE%B0%E8%B5%B0%E8%AE%BF%E7%BA%A2%E7%B3%96%E5%8E%82%E5%AE%B6%E8%AF%B4%E6%8D%A1%E7%82%B9%E6%B8%A3%E6%B8%A3%E5%90%83)、[脂肪肝的危害或许被低估了](https://s.weibo.com/weibo?q=%E8%84%82%E8%82%AA%E8%82%9D%E7%9A%84%E5%8D%B1%E5%AE%B3%E6%88%96%E8%AE%B8%E8%A2%AB%E4%BD%8E%E4%BC%B0%E4%BA%86) 和 [8岁男孩55斤查出脂肪肝](https://s.weibo.com/weibo?q=8%E5%B2%81%E7%94%B7%E5%AD%A955%E6%96%A4%E6%9F%A5%E5%87%BA%E8%84%82%E8%82%AA%E8%82%9D) 属于社会或健康话题，未核对原文或医学指南，不写成新的公共标准。[金价](https://s.weibo.com/weibo?q=%E9%87%91%E4%BB%B7) 仍在热搜，具体读数见金融栏。

**速览。** 其余靠前条目多为综艺、剧集和体育，如白小纯直播礼物、文吉儿、李雪琴、陈伟霆、刘恺威、成毅、舒淇与冯德伦、青稚、王菲牵李嫣、复联 5、U17 国足以第 99 分钟被绝平、国乒 U19 男团、祝启慧对阵松岛美空，以及「E法同行向上向海」等活动语，不展开。

## 7. 油管科技访谈

对照 docs/youtube-sources.md 的频道名单，从各频道 /videos 页解析近作，再打开节目页读取发布时间、时长和官方简介。只选近约 7–10 天、时长约 15 分钟以上、尚未写入查重档案的访谈。Lex Fridman、Dwarkesh Patel、Y Combinator、Lenny's Podcast、All-In、No Priors、Latent Space、The Pragmatic Engineer 等频道近一周的节目，多数已在前几期写过；All-In 一则九天前讨论黄仁勋去职的节目，既已超出「新进展」的写作价值，也已被今天的复职新闻取代，不再展开。因此今天能新写的长访谈很少。

**[Why OpenAI Acquired a Biotech Startup](https://www.youtube.com/watch?v=RwYz8XhZiu0)**  
a16z · 1:05:34 · 发布于 2026-11-23 23:30:33 Asia/Shanghai（UTC+8）。官方简介称，嘉宾是 OpenAI 的 Joy Jiao 与 Ashoka Rajendra，主持人为 a16z 的 Jay Rughani 和 Jorge Conde，讨论当科学家不再受「人类注意力」限制时，人工智能和大量并行智能体可能如何改变药物发现与开发。简介把 OpenAI 的生命科学工作追溯到科学推理，以及收购 Orchestra Bio；并列出会谈议题：在生物数据中搜索、管理临床试验、处理监管与生产流程，以及「一个人也许能同时推进多个生物技术项目」的前景。章节目录里还有「Codex for Scientists」、发现 / 开发 / 分发「三 D」、波士顿儿童医院突破、可追溯性与生物安全等条目。简介中的收购、应用场景和医院案例，都是节目与出品方的说法，并链向 OpenAI 自己关于收购 Orchestra Bio 的说明页，不是对交易条款或临床试验结果的独立核实，也不编造他们在节目中说过的话。

## 8. 本月阅读与今日书摘

今天是星期二。按 [本月阅读计划](/reading/)，工作日若有预先写好的分期书摘，应写入早报；若当天没有安排章节，则只保留书单和进度，不硬塞新的摘要。

本月四本书是：布鲁克斯《人月神话》（*The Mythical Man-Month*，1995 年 20 周年纪念版）、德马可与李斯特《人件》（*Peopleware*）、迈克康奈尔《代码大全》（*Code Complete*）、奥斯特豪特《软件设计的哲学》（*A Philosophy of Software Design*）。《人月神话》已在 11 月 16 日至 20 日五个工作日读完，最末一期是第 16–19 章，包括「没有银弹」。计划写明下一本是《人件》，但仓库里的分期文稿尚未写入《人件》各工作日的书摘，故本期不编造章节摘要，只保留书单与进度指引。具体安排见仓库 [docs/reading-plan-2026-11.md](https://github.com/haozhenhua/haozhenhua.github.io/blob/main/docs/reading-plan-2026-11.md) 与站点 [本月阅读](/reading/)。

## 9. 今日总结

星期二早上，金融市场终于有了周一那一组官方数字：人民币中间价小幅下调，A 股在上周五大跌之后收出一根温和的反弹，深成指回升得更明显一些；黄金则较上一期早报又升了一截。真正把昨天白天和夜间的信息环境拧在一起的，是英伟达董事会那份复职声明。黄仁勋的去职与回归，前几天还只能写成传闻和排除性表态，现在有了公司公告、政府「不构成国家安全风险」的表述，以及股价一天大涨的市场反应；但独立董事的调查并没有因此收场，美国商务部拟将 Megaspeed 列入实体清单，也把出口管制这条线继续往前推。班加西港的袭击则有了泽连斯基「示范行动」的定性，战争的边缘再一次被说得更清楚。Hacker News 上最热闹的，一边是这场复职，一边是 Ladybird 终于交出可下载的 alpha，以及智谱把自己的循环深度模型写成「广义编程」的起点；另一边，Anthropic 仓库里「VP ≠ VNP」的形式化和 Alpöge 承认「25 万页是玩笑」，都在提醒：能编译、能上传，还不等于已经被数学共同体接受。X 和微博几乎被同一条公司新闻占满，自变量机器人的 WALL-OSS 数字则仍是出品方口径。北京市区今早接近 0℃，白天转晴；海淀栏终于有了「光影智谷」和交通调研这些近日稿，昌平则把脑机接口大会写到了区政新闻的中心位置。阅读上，《人月神话》已经读完，下一本《人件》还在等分期书摘写进计划，今天先不硬造章节。若只从今天唯一新写的访谈里留一句，a16z 那期更值得记住的不是收购清单，而是简介里反复出现的问题：当「注意力」不再稀缺，药物研发真正要决定的，是下一步该做什么。
