# 油管科技访谈来源

供每日早报对照。只收录访谈或长视频对谈，不把频道里的广告、短视频、预告或课程碎片写进正文。

## 抓取说明

YouTube 官方 Atom 订阅（`https://www.youtube.com/feeds/videos.xml?channel_id=…`）在本机环境中可能返回 404，不要把它当成频道不存在。改用下面的办法：

1. 用桌面浏览器 User-Agent 打开 `https://www.youtube.com/@HANDLE/videos`。
2. 从页面里的 `ytInitialData` 解析 `lockupViewModel`：标题在 `metadata.lockupMetadataViewModel.title.content`，视频 ID 在 `contentId` 或 `watchEndpoint.videoId`，相对发布时间常见为 `5d ago`、`17h ago` 这种简写。
3. 再打开 `https://www.youtube.com/watch?v=VIDEO_ID`，读取视频页上的发布时间、时长和官方简介（`ytInitialPlayerResponse` 里的 `videoDetails` / `microformat`，或页面的 `datePublished`、`duration`）。
4. 筛选：时长约 15 分钟及以上，近约 7–10 天内发布，内容是访谈或对谈。同一节目的新一集可以写；已经写进查重档案的同一条视频不要再写。
5. 依据官方简介、章节目录与出品方说明写中文 brief，保留英文标题、频道、时长、发布时间和视频链接。不要编造嘉宾或主持人说过的话，不要转载字幕或全文。节目简介里的市场排名、融资或业绩数字，要标明是节目或出品方的说法。
6. 每天选四至六条质量较高的即可，不必把所有频道都写满。若某期只是在复述当天早报其他栏目已经写过的新闻，不要再展开，必要时一行「续报」。

## 当前名单

| 节目 | 手柄 | 备注 |
| --- | --- | --- |
| Lex Fridman | `@lexfridman` | 长访谈；非科技主题可略过 |
| Dwarkesh Patel | `@DwarkeshPatel` | 优先访谈；个人长文口述若特别相关可写一条 |
| Y Combinator | `@ycombinator` | 只取访谈/对谈（如 Lightcone、How to Build the Future），跳过短课程 |
| Lenny's Podcast | `@lennyspodcast` | 产品与增长访谈 |
| a16z | `@a16z` | 访谈与主题对谈 |
| All-In Podcast | `@allin` | 若只是复述已写新闻则跳过或一行续报 |
| No Priors | `@NoPriorsPodcast` | AI 与创业访谈 |
| Latent Space | `@LatentSpacePod` | AI 工程访谈 |
| The Pragmatic Engineer | `@pragmaticengineer` | 软件工程访谈 |
| Acquired | `@acquiredfm` | 更新较慢，有新长访谈再写 |

`@thisweekinstartups` 的 `/videos` 页目前仍是多年前的旧内容，暂不作为可靠来源。中文科技访谈频道以后可以再补进本表。
