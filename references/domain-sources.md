# 全领域专业网站定向检索地图 (Domain Authority Matrix)

核心原则：**不同领域的问题，去该领域最专业、最可靠的网站定向检索，拒绝漫无目的的全网泛搜，也绝不把所有问题都死磕在某一个固定网站上。**

在制定阶段 1 的 `Evidence Checklist` 时，先判断问题所属的**垂直领域**，再按以下三个证据层级组合选择 2~3 个目标站点进行交叉验证：
- **Tier 1 一手基准/法定源 (Ground Truth)**：官方机构、法定披露、原始数据库、标准组织（查事实存否、官方参数、准确价格/政策）。
- **Tier 2 专业评测/独立数据库 (Expert & Benchmark)**：行业公认的硬核实验室、量化数据库、学术检索库（查客观横评、性能实测、独立对比）。
- **Tier 3 垂直硬核社区 (Practitioner Community)**：该领域真正懂行的从业者/发烧友聚集地（查真实体验、长期通病、隐形坑）。

---

## 1. AI、大模型与开发者工具 (AI, LLMs & DevTools)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 一手源** | 各厂商官网 Pricing / Docs / Status<br>`github.com` (Releases / Issues)<br>`huggingface.co` / `arxiv.org` | 官方API定价、Rate Limits、模型卡片、开源权重、原始技术报告、服务宕机状态 | `site:docs.anthropic.com rate limits`<br>`site:huggingface.co Qwen` |
| **Tier 2 专业评测与数据库** | **Artificial Analysis** (`artificialanalysis.ai`)<br>**LMSYS Arena** (`lmarena.ai`)<br>**LiveBench** (`livebench.ai`)<br>**SWE-bench** (`swebench.com`)<br>**OpenRouter Rankings** (`openrouter.ai/rankings`) | API真实吞吐速度(tokens/s)、首字延迟(TTFT)、各渠道价格横评、人类盲测ELO排名、防污染综合跑分、编程Agent实测通过率、实际调用量趋势 | `site:artificialanalysis.ai claude sonnet`<br>`site:lmarena.ai leaderboard` |
| **Tier 3 垂直社区** | **Linux DO** (`linux.do`)<br>**Reddit** (`r/LocalLLaMA`, `r/ClaudeAI`, `r/OpenAI`)<br>**Hacker News** (`news.ycombinator.com`)<br>**V2EX** (`v2ex.com`) | 国内API中转/订阅防封经验、本地部署显存与量化实测、模型降智吐槽、AI Coding工具工作流对比 | `site:linux.do Cursor 额度`<br>`site:reddit.com/r/LocalLLaMA` |

- 🚫 **避坑/降权**：全网泛搜“XX模型测评”出来的营销公众号、搬运跑分图的自媒体、带注册返佣链接的软文。

---

## 2. 软件工程、开源生态与网络安全 (Software, Infra & Security)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 一手源** | 语言/框架官方 Docs<br>`developer.mozilla.org` (MDN)<br>官方包管理库 (`npmjs.com`, `pypi.org`, `crates.io`, `pkg.go.dev`)<br>`datatracker.ietf.org` (RFC) | API规范、版本演进、依赖包维护状态与周下载量、网络协议标准 | `site:npmjs.com package-name`<br>`site:developer.mozilla.org` |
| **Tier 2 安全漏洞与状态库** | **NVD** (`nvd.nist.gov`) / **CVE** (`cve.org`)<br>**GitHub Advisories** (`github.com/advisories`)<br>**Snyk Vulnerability DB** (`security.snyk.io`)<br>**Downdetector** (`downdetector.com`) | 披露的CVE安全漏洞详情、受影响版本范围、补丁修复版本、全球云服务实时故障排查 | `site:github.com/advisories log4j`<br>`site:nvd.nist.gov CVE-2026` |
| **Tier 3 垂直社区** | **GitHub Issues / Discussions**<br>**Stack Overflow** (`stackoverflow.com`)<br>**Hacker News** / **Lobsters** (`lobste.rs`)<br>**先知社区** (`xz.aliyun.com`) / **FreeBuf** | 特定版本报错排查、生产环境架构选型争议、开源项目是否陷入维护停滞 | `site:github.com/org/repo/issues memory leak`<br>`site:lobste.rs rust` |

- 🚫 **避坑/降权**：机翻搬运 Stack Overflow 的采集站、CSDN 付费/抄袭水文（除非查极其特定的国内环境报错）。

---

## 3. 硬件数码、PC组件、外设与家电消费 (Hardware, Tech & Appliances)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 一手源** | 厂商官网 Spec 页 (Intel ARK, AMD, NVIDIA, Apple Specs 等)<br>**FCC ID** (`fccid.io`) | 芯片官方规格表、TDP、接口标准、无线设备内部拆解备案图 | `site:ark.intel.com` |
| **Tier 2 硬核实验室评测** | **RTINGS** (`rtings.com` — 显示器/电视/耳机/键鼠/吸尘器量化测试天花板)<br>**NotebookCheck** (`notebookcheck.net` — 笔记本/移动CPU/GPU详尽测试库)<br>**TechPowerUp** (`techpowerup.com` — 显卡/SSD数据库与拆解)<br>**极客湾 SoCPK** (`socpk.com` — 手机/移动芯片能效曲线)<br>**GSMArena** (`gsmarena.com` — 手机参数与续航标准测试)<br>**充电头网** (`chongdiantou.com` — 充电器/移动电源协议与拆解)<br>**Audio Science Review** (`audiosciencereview.com` — 音频设备客观声学测量)<br>**Puget Systems** (`pugetsystems.com` — 生产力工作站基准) | 屏幕色准/响应时间/频闪实测、笔记本散热与功耗墙、显卡PCB用料、充电头纹波与温升、耳机频响曲线 | `site:rtings.com monitor review`<br>`site:notebookcheck.net RTX`<br>`site:techpowerup.com ssd-specs`<br>`site:chongdiantou.com 拆解` |
| **Tier 3 垂直社区** | **Chiphell** (`chiphell.com` — 高端PC硬件/装机/外设开箱实测)<br>**Reddit** (`r/buildapc`, `r/Monitors`, `r/MouseReview`, `r/headphones`)<br>**什么值得买** (`smzdm.com` — **重点看评论区真实追评解毒**，警惕主楼)<br>**酷安** (手机/数码体验) / **耳机大家坛** (`erji.net`) | 长期使用的品控通病（如掉驱动、啸叫、断连、售后扯皮）、历史真实成交好价 | `site:chiphell.com 显示器`<br>`site:reddit.com/r/Monitors` |

- 🚫 **避坑/降权**：纯罗列参数并附带淘宝/京东/Amazon 返利链接的“十大排行榜”导购站、无实测数据的开箱吹捧文。

---

## 4. 学术科研、科学事实与工程技术 (Academic, Science & Engineering)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 论文与原始库** | **Google Scholar** (`scholar.google.com`)<br>**Semantic Scholar** (`semanticscholar.org`)<br>**arXiv** (`arxiv.org` — 物理/数学/CS预印本)<br>**PubMed / PMC** (`pubmed.ncbi.nlm.nih.gov` — 生物医学)<br>**IEEE Xplore** / **ACM DL** / **Nature** / **Science**<br>**SSRN** (`ssrn.com`) / **NBER** (`nber.org` — 经济学)<br>**中国知网** (`cnki.net`) | 科学结论的原始研究论文、实验方法、样本量、引用次数、作者机构 | `site:arxiv.org`<br>`site:pubmed.ncbi.nlm.nih.gov` |
| **Tier 2 学术基准与统计** | **OpenReview** (`openreview.net` — AI顶会ICLR/NeurIPS公开审稿意见与打分！)<br>**Papers With Code** (`paperswithcode.com`)<br>**Our World in Data** (`ourworldindata.org` — 全球能源/人口/环境长周期数据) | 某篇顶会论文到底有没有创新（看审稿人尖锐提问）、算法是否开源可复现、全球宏观科学统计 | `site:openreview.net`<br>`site:ourworldindata.org` |
| **Tier 3 学术评议与社区** | **PubPeer** (`pubpeer.com` — 论文同行质疑/造假勘误数据库)<br>**Retraction Watch** (`retractionwatch.com` — 撤稿追踪)<br>**小木虫** (`muchong.com`) / **知乎**（实名科研答主） | 某项轰动研究是否被同行质疑数据造假、实验能否复现、期刊审稿周期与水刊避坑 | `site:pubpeer.com`<br>`site:retractionwatch.com` |

- 🚫 **避坑/降权**：“震惊！科学家最新发现…”类的二手科普自媒体（往往严重曲解相关性与因果性，或把小鼠体外实验吹成人类神药）。

---

## 5. 医疗健康、疾病诊疗、药品与营养学 (Medicine, Pharma & Nutrition)

> ⚠️ **医疗健康领域铁律**：严禁采信普通自媒体、养生号、百度搜索前排广告/百家号。必须定向检索循证医学机构与药监数据库。

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 法定药监与公卫机构** | **国家药监局 NMPA** (`nmpa.gov.cn`)<br>**FDA** (`fda.gov` — Drugs@FDA)<br>**WHO** (`who.int`) / **CDC** (`cdc.gov`)<br>**MedlinePlus** (`medlineplus.gov` — 美国国立医学图书馆) | 药品/医疗器械是否获批上市、官方说明书（适应症/禁忌症/黑框警告）、传染病与疫苗官方指南 | `site:fda.gov drug approval`<br>`site:nmpa.gov.cn` |
| **Tier 2 循证医学与专业指南** | **默沙东诊疗手册** (`msdmanuals.cn` / `msdmanuals.com` — 免费公开的医学教科书级参考，分大众版与专业版)<br>**Mayo Clinic** (`mayoclinic.org`) / **Cleveland Clinic** (`clevelandclinic.org`)<br>**UpToDate** (`uptodate.com` — 临床循证医学金标准)<br>**Cochrane Library** (`cochranelibrary.com` — 循证系统评价)<br>**Examine.com** (`examine.com` — 膳食补剂/营养学循证研究天花板，纯论文汇总无带货)<br>**Drugs.com** (`drugs.com`) / **丁香园用药助手** (`drugs.dxy.cn`) | 疾病标准诊疗路径、症状鉴别、某种补剂/保健品到底有没有人体临床证据、药物相互作用排查 | `site:msdmanuals.cn`<br>`site:mayoclinic.org`<br>`site:examine.com creatine`<br>`site:drugs.com interaction` |
| **Tier 3 专业医疗社区** | **丁香园** (`dxy.cn`)<br>**医脉通** (`medlive.cn`)<br>**Reddit** (`r/AskDocs`, `r/medicine`) | 临床医生对指南落地的讨论、医药行业政策解读 | `site:dxy.cn` |

- 🚫 **避坑/降权**：一切带货保健品的健康博主、民营医院 SEO 页面、无临床文献支撑的偏方帖。

---

## 6. 金融投资、宏观经济与公司商业数据 (Finance, Macro & Corporate Data)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 法定披露与统计局** | **SEC EDGAR** (`sec.gov/edgar` — 美股10-K/10-Q/S-1原始财报)<br>**巨潮资讯网** (`cninfo.com.cn` — A股证监会指定上市公司公告唯一一手源)<br>**港交所披露易** (`hkexnews.hk` — 港股招股书与财报)<br>**FRED** (`fred.stlouisfed.org` — 美联储宏观经济数据库)<br>**国家统计局** (`stats.gov.cn`) / **中国人民银行** (`pbc.gov.cn`)<br>**World Bank Data** (`data.worldbank.org`) / **IMF** (`imf.org`) | 公司真实营收/利润/现金流/高管薪酬、IPO招股书风险因素、官方GDP/CPI/利率历史序列 | `site:sec.gov/Archives/edgar`<br>`site:cninfo.com.cn`<br>`site:hkexnews.hk`<br>`site:fred.stlouisfed.org` |
| **Tier 2 市场终端与商业库** | **Yahoo Finance** (`finance.yahoo.com`) / **TradingView** (`tradingview.com`)<br>**东方财富** (`eastmoney.com`) / **同花顺**<br>**Crunchbase** (`crunchbase.com`) / **IT桔子** (`itjuzi.com` — 一级市场融资)<br>**Macrotrends** (`macrotrends.net` — 美股长周期财报比率)<br>**权威财经媒体**：彭博 (`bloomberg.com`)、路透 (`reuters.com`)、财新 (`caixin.com`)、华尔街见闻 | 实时股价/市值、估值倍数(PE/PB/PS)、初创公司融资轮次与投资方、突发商业并购新闻 | `site:finance.yahoo.com`<br>`site:crunchbase.com` |
| **Tier 3 投资者社区** | **集思录** (`jisilu.cn` — 可转债/ETF/分级基金/低风险套利硬核数据社区)<br>**雪球** (`xueqiu.com` — 只看深度财报拆解长文，过滤情绪喊单)<br>**Seeking Alpha** (`seekingalpha.com`)<br>**Reddit** (`r/SecurityAnalysis`, `r/ValueInvesting`) | 财报疑点扒皮、套利规则实操、看空/看多逻辑交锋 | `site:jisilu.cn`<br>`site:seekingalpha.com` |

- 🚫 **避坑/降权**：荐股群软文、混淆“营收/GMV/估值/利润”口径的公关通稿、未标注币种与财年口径的二手数据图。

---

## 7. 企业级软件 (B2B SaaS)、互联网服务与商业防坑 (SaaS & Consumer Trust)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 一手源** | 官网 Pricing / SLA / Terms of Service / Privacy Policy / Security Trust Center (SOC2/ISO27001) | 企业版隐藏限制、数据归属与是否用于训练、退款条款、合规认证 | `site:vendor.com/terms` |
| **Tier 2 软件评测与替代库** | **G2** (`g2.com`) / **Capterra** (`capterra.com`)<br>**Gartner Peer Insights** (`gartner.com/reviews`)<br>**TrustRadius** (`trustradius.com`)<br>**AlternativeTo** (`alternativeto.net` — 查软件平替/开源替代品神器)<br>**Product Hunt** (`producthunt.com`) / **少数派** (`sspai.com`) | B2B软件真实采购评价、实施难度、客服响应速度、寻找某款收费软件的开源/免费替代方案 | `site:g2.com Notion`<br>`site:alternativeto.net` |
| **Tier 3 消费者防坑与投诉库** | **Trustpilot** (`trustpilot.com` — 国际网站/独立站/SaaS防诈骗与售后口碑必查)<br>**黑猫投诉** (`tousu.sina.com.cn` — 国内商家霸王条款/自动扣费/跑路维权统计)<br>**国家企业信用信息公示系统** (`gsxt.gov.cn`) / **天眼查** / **企查查** | 验证某海外网站是不是杀猪盘/骗子站、某服务扣费后能不能退、国内公司是否经营异常或涉诉 | `site:trustpilot.com`<br>`site:tousu.sina.com.cn` |

- 🚫 **避坑/降权**：搜索引擎里买关键词竞价排名的山寨官网、标题为“2026最佳XX软件Top 10”但排名第一就是文章发布者自己产品的软文。

---

## 8. 法律法规、政务政策、专利与国家标准 (Law, Policy, Patents & Standards)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 法定与官方数据库** | **国家法律法规数据库** (`flk.npc.gov.cn` — 全国人大官方唯一现行法律库)<br>**中国政府网** (`gov.cn`) 及各部委官网 (`.gov.cn`)<br>**中国裁判文书网** (`wenshu.court.gov.cn`) / **人民法院案例库** (`rmfyalk.court.gov.cn`)<br>**国家标准全文公开系统** (`openstd.samr.gov.cn` — GB国标查询)<br>**Cornell LII** (`law.cornell.edu` — 美国法律公开库)<br>**EUR-Lex** (`eur-lex.europa.eu` — 欧盟法规如GDPR/AI Act原文) | 现行有效的法律条文原文（确认是否已修订或废止）、国务院/部委红头文件、强制性国家标准(GB) | `site:gov.cn`<br>`site:law.cornell.edu`<br>`site:eur-lex.europa.eu` |
| **Tier 2 专业检索库** | **北大法宝** (`pkulaw.com`) / **威科先行** (`lawinfochina.com`)<br>**Google Patents** (`patents.google.com`) / **国家知识产权局** (`cnipa.gov.cn`)<br>**Justia** (`justia.com`) | 法规历史沿革对比、司法判例检索、专利权利要求书与法律状态 | `site:patents.google.com`<br>`site:pkulaw.com` |

- 🚫 **避坑/降权**：引用已废止旧法的营销号文章（如把《民法典》生效前已废止的单行法当现行法引用）、非 `.gov` 域名的代办中介网站。

---

## 9. 游戏、影视、动漫与图书文娱 (Gaming, Film, Anime & Books)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 平台一手数据** | **SteamDB** (`steamdb.info` — Steam在线人数峰值/各区历史底价/更新变更记录)<br>**Steam 商店页** (`store.steampowered.com` — 近期评测好评率)<br>**Box Office Mojo** (`boxofficemojo.com`) / **猫眼专业版**（实时票房） | 游戏真实在线人数（有没有鬼服）、历史最低折扣价、近期更新是否引发差评轰炸、真实票房数据 | `site:steamdb.info`<br>`site:store.steampowered.com` |
| **Tier 2 评分聚合与维基** | **Metacritic** (`metacritic.com`) / **OpenCritic** (`opencritic.com`)<br>**PCGamingWiki** (`pcgamingwiki.com` — PC游戏帧率解锁/宽屏补丁/存档路径/Bug修复圣经)<br>**HowLongToBeat** (`howlongtobeat.com` — 游戏通关时长统计)<br>**IMDb** (`imdb.com`) / **Rotten Tomatoes** (`rottentomatoes.com`) / **Letterboxd** | 媒体均分 vs 玩家均分差异、PC版移植优化质量与报错修复、通关所需时间 | `site:pcgamingwiki.com`<br>`site:metacritic.com`<br>`site:howlongtobeat.com` |
| **Tier 3 垂直文娱社区** | **豆瓣** (`douban.com` — 图书/电影/剧集评分与深度书评影评)<br>**Bangumi 番组计划** (`bgm.tv` — 硬核ACG评分与制作人员考据)<br>**NGA 玩家社区** (`nga.cn` / `bbs.nga.cn` — 数值机制测算/硬核攻略)<br>**Goodreads** (`goodreads.com`) / **MyAnimeList** (`myanimelist.net`) | 作品真实口碑、译本质量对比（买哪个出版社的译本好）、游戏深层数值机制 | `site:douban.com`<br>`site:bgm.tv`<br>`site:nga.cn` |

- 🚫 **避坑/降权**：AI 批量生成的“XX游戏攻略/结局解析”采集站（内容往往张冠李戴，把别的技能/剧情混进来）。

---

## 10. 汽车、旅游出行与品质生活 (Auto, Travel & Lifestyle)

| 层级 | 推荐专业网站 (域名) | 最擅长解决的具体问题 | 定向搜索示例 |
|------|-------------------|-------------------|-------------|
| **Tier 1 官方与监管源** | 各国领事馆/移民局官网 (签证政策一手源)<br>**IATA Travel Centre** / **外交部领事直通车**<br>**NHTSA** (`nhtsa.gov` — 美国公路安全局碰撞测试与召回) / **中保研 C-IASI** (`ciasi.org.cn` — 汽车碰撞安全测试) | 签证免签/落地签最新官方政策、汽车碰撞安全评级、官方召回公告 | `site:nhtsa.gov`<br>`site:ciasi.org.cn` |
| **Tier 2 专业测评与故障统计** | **车质网** (`12365auto.com` — 国内汽车质量投诉统计库，查某车型通病极准！)<br>**懂车帝** (`dongchedi.com`) / **汽车之家** (`autohome.com.cn` — 实测续航/加速/拆解)<br>**Consumer Reports** (`consumerreports.org`) / **Wirecutter** (`nytimes.com/wirecutter`)<br>**SeatGuru** / **AeroLOPA** (`aerolopa.com` — 航司客机精准座位图) | 某款车型的变速箱/异响/车机真实投诉量、冬测续航达成率、飞机哪个座位窗户对齐/间距大 | `site:12365auto.com`<br>`site:dongchedi.com` |
| **Tier 3 垂直玩家社区** | **飞客茶馆** (`flyert.com` — 国内酒店/航司常旅客、信用卡权益硬核社区)<br>**FlyerTalk** (`flyertalk.com` — 国际常旅客社区)<br>**TripAdvisor** (`tripadvisor.com`) / **穷游** (`qyer.com`) | 酒店会员升房厚道程度、航司里程兑换甜点、近期机场/景区真实避坑 | `site:flyert.com`<br>`site:flyertalk.com` |

---

## 11. 未知/小众细分领域的「两步跳动态探源协议」(Two-Hop Dynamic Routing)

人类知识领域无穷无尽。当用户提问涉及上述 10 大领域之外的**细分/冷门领域**（例如：特种化工、跨境物流清关、宠物疾病、冷门乐器、特定行业招投标、某地房产政策等）时，**严禁直接拿问题长句在全网盲搜**，必须执行以下动态判断：

### 第一步：先在思考中回答「领域三问」（锚定信源类型）
1. **谁定规则（Tier 1）？** 这个细分领域的监管部门、行业协会、发证机构或国际标准组织是谁？
2. **谁有数据（Tier 2）？** 这个行业从业者天天查参数、查行情、查排名的垂直数据库或行业门户网站叫什么？
3. **谁在实操（Tier 3）？** 真正掏钱买单或干这行的老手，聚集在哪个垂直论坛或贴吧/Subreddit？

### 第二步：两步跳检索（Two-Hop Search）
- **Hop 1（探源）**：如果你脑中知道该领域的权威站点域名，直接用；如果不确定，先用 1 次极简搜索查找该领域的权威站点（例如搜 `"跨境电商" 权威数据网站` 或 `"aquarium" best forum` 或 `"pet toxicology" database`）。
- **Hop 2（定向深挖）**：拿到 2~3 个垂直专业域名后，用 `site:domain` 或携带该专业站点名称进行定向检索，并将不同站点的结论交叉比对。
