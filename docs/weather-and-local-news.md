# 天气与本地新闻来源

供每日早报第 2 节对照。预报城市为北京市区；本地新闻只收海淀区、昌平区的真正本地报道。不要编造温度、天气或新闻条目。抓取时使用桌面浏览器 User-Agent；本机环境里 `https` 通常可用，部分站点的纯 `http` 可能被中间代理返回 500，不要据此判断源站不存在。

## 北京市区天气预报

优先使用中国气象局城市预报，不必打开浏览器。

1. 请求 `https://weather.cma.cn/api/weather/view?stationid=54511`。
2. 站点 `54511` 的 `name` 为「北京」，`path` 为「中国, 北京, 北京」，这是该局城市预报中的北京市站，不要改成海淀、昌平或其他区县站。公开页面为 `https://weather.cma.cn/web/weather/54511.html`。
3. JSON 里的 `now` 是当前实况（气温、体感 `feelst`、湿度、风向风力、风速、降水量、气压），`daily` 是逐日预报（白天/夜间天气现象、最高/最低气温、风向风力），`lastUpdate` 是源站更新时间，`alarm` 是预警列表。温度用摄氏度。风速在该局页面上以米/秒标注，气压以百帕标注；接口本身未单独给出单位字段，写稿时按页面单位记录，不要擅自换算。
4. 写出当前或当日早晨实况、今日预报，以及未来 2–3 天的高温、低温和天气现象。降水、风力和空气质量只在同一来源确实提供时才写。日预报对象目前没有降水量字段，不要编造雨量。该接口目前也不提供 AQI，不要把其他来源的空气质量混进这组预报。
5. 在文中同时给出公开页链接、接口 `lastUpdate`，以及本次采集时间（Asia/Shanghai，UTC+8）。

备用核对（不要无故替换主源）：

- 中国天气网北京 7 天预报页：`https://www.weather.com.cn/weather/101010100.shtml`（城市代码 `101010100`，标题为北京天气预报）。页面可用来核对天气现象与高低温。该站 `d1.weather.com.cn` 的实况接口在本机测试中返回 403，不要依赖它做自动化。
- Open-Meteo 预报接口 `https://api.open-meteo.com/v1/forecast` 在本机测试中曾连接超时，空气质量子接口有时可用，但与主源不是同一套数据，不能把那里的 AQI 写进中国气象局预报。
- `https://wttr.in/Beijing?format=j1` 有时可用，但是第三方汇总，读数可能与中国气象局不一致，只宜在主源失败时作为后备，并在文中标明。
- 中央气象台页面 `https://www.nmc.cn/publish/forecast/ABJ/beijing.html` 可打开，但其 ` /rest/weather?stationid=54511` 在本机测试中返回空数据，不宜作为首选接口。

主源失败时换用上述仍能成功的来源，并在文中说明换源原因；任何情况下都不要编造温度或天气。天气预报数字每天更新，不必写入 `docs/brief-memory/seen.json`。

## 海淀区、昌平区本地新闻

写稿前先读 `docs/brief-memory/seen.json`。已经写过的本地事件不要再写，除非有实质性新进展（续报）。全国新闻只是顺便提到区名的不要写，广告不要写。按区分列，不要把海淀和昌平的归属写混。保留原标题并链接原文，用中文做摘要，不转载全文。有材料时每区约 3–5 条，来源较薄就少写。

本机用 `curl` 加桌面 User-Agent 打开下列 `https` 列表页即可，一般不必再加特殊请求头。解析列表里的标题、日期和文章链接，再打开原文页核对事实；海淀区文章正文多在页面中部（常见容器包括 `#mainText`），昌平区文章常见 `ArticleTitle`、`PubDate`、`ContentSource` 等 meta，正文在标题与页脚之间。

### 海淀区

| 用途 | URL | 备注 |
| --- | --- | --- |
| 区政府首页 | `https://www.bjhd.gov.cn/` | 可先看要闻入口 |
| 要闻动态 | `https://www.bjhd.gov.cn/ywdt/` | 栏目总入口 |
| 海淀动态 / 海淀要闻 | `https://zyk.bjhd.gov.cn/ywdt/hdywx/` | 首选区政要闻列表 |
| 政务动态 | `https://zyk.bjhd.gov.cn/ywdt/hdyw/` | 与上栏常有交叉 |
| 部门动态 | `https://zyk.bjhd.gov.cn/ywdt/bmdt/` | 部门工作，更新较慢 |
| 街镇动态 | `https://zyk.bjhd.gov.cn/ywdt/jzdt/` | 街道、镇的本地稿 |
| 通知公告 | `https://zyk.bjhd.gov.cn/zwdt/xxgk/tzgg/` | 公示、规划等，择与居民相关者 |

海淀区融媒体中心在区政府网站有机构栏目，日常新闻稿常见来源标注为「海淀报」。不要把中央或全市要闻栏（例如北京政府网站要闻）当作海淀本地新闻。

### 昌平区

| 用途 | URL | 备注 |
| --- | --- | --- |
| 区政府首页 | `https://www.bjchp.gov.cn/` | 首页常有近期 APP 新闻 |
| 要闻动态 | `https://www.bjchp.gov.cn/cpqzf/ywdt26/` | 栏目总入口 |
| 昌平快讯 | `https://www.bjchp.gov.cn/cpqzf/ywdt26/cpkx/` | 首选区政新闻列表 |
| APP 新闻 | `https://www.bjchp.gov.cn/cpqzf/ywdt26/zwxmt/apptt/` | 北京昌平 APP 稿，偏现场与活动 |
| 部门动态等 | 见要闻动态页内链接 | 如空气质量日报，属区生态环境局口径，不要拿来替代北京市区天气预报 |

稿件来源常见为「北京昌平 APP」。区融媒体中心官方微博「昌平报」可作为线索，但早报条目仍应链接到可核对的官网正文。城市级或部委稿件若只是转载在区政府「热点转载」栏，一般不算昌平本地新闻。

发布当天稿件时，把新写入的本地新闻追加进 `docs/brief-memory/seen.json`，标识约定见 `docs/brief-memory/README.md`。
