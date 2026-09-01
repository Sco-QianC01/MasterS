# Track 01 — Figures 人物：企业财务与 CFO 视角（Corporate Finance & the CFO Lens）

> **调研日期**: 2026-09-02 · **locale**: zh-CN · **Track**: 01 (figures)
> **范围锚定**: 面向创业公司与中小企业主/创始人的内部财务判断 —— 读懂三张表、预算与滚动预测、现金流与营运资金、成本核算与定价、融资结构与股权稀释。
> **明确排除**: 投行卖方并购执行、VC 投资人的看项目视角、个人理财与二级市场选股、注册会计师/中级职称考证名师。
> **Wave 2 说明**: 本 track 在 wave 2 启动，seed 候选来自已完成的 `04-canon.md`（正典作者）与 `05-sources.md`（newsletter/podcast 主创与嘉宾）。
>
> **状态**: ✅ 完成

---

## Source Manifest

> bucket 判定：`python3 tools/research/source_verifier.py classify <URL>` 自动结果，只做「升级到 surrogate_primary」的人工调整（figure 本人站 / 机构自有出版物 / 出版社官方书页 / 准则机构官方页），不私自降级。
> 403 状态码（Morgan Stanley / FASB / SEC / Carta / SaaS Capital）是反爬拦截而非死链，内容经搜索结果与二次来源交叉确认，不标 `dead`。

| source_id | url | bucket | last_checked | author/host | one-line note |
|-----------|-----|--------|--------------|-------------|---------------|
| T01-S001 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/ | verified_primary | 2026-09-02 | Aswath Damodaran / NYU Stern | Damodaran Online 主站，全部讲义数据入口 |
| T01-S002 | https://aswathdamodaran.substack.com/ | verified_primary | 2026-09-02 | Aswath Damodaran | own site — 现役主力发文渠道 Musings on Markets |
| T01-S003 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datacurrent.html | verified_primary | 2026-09-02 | Aswath Damodaran / NYU Stern | 每年 1 月刷新的免费行业 beta/WACC/ROIC 数据集 |
| T01-S004 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/webcastvalonline.htm | verified_primary | 2026-09-02 | Aswath Damodaran / NYU Stern | 25 讲免费估值公开课 webcast + slides |
| T01-S005 | https://www.themebfabershow.com/episodes/oILab0ZBVxs | verified_primary | 2026-09-02 | Meb Faber Show #619 | 2026-02 长访谈：AI 资本开支是泡沫还是繁荣 |
| T01-S006 | https://microcapclub.com/club-conversation-with-aswath-damodoran-the-dean-of-valuation/ | secondary | 2026-09-02 | MicroCapClub | 2026-01 长对谈实录，含个人史与教学观 |
| T01-S007 | https://aswathdamodaran.blogspot.com/2015/02/dcf-myth-1-if-you-have-ddiscount-rate.html | verified_primary | 2026-09-02 | Aswath Damodaran | own site — DCF 十大误区系列开篇 |
| T01-S008 | https://cup.columbia.edu/book/narrative-and-numbers/9780231180481/ | verified_primary | 2026-09-02 | Columbia University Press | publisher official page —《Narrative and Numbers》 |
| T01-S009 | https://www.morganstanley.com/im/en-us/individual-investor/insights/series/consilient-observer.html | surrogate_primary | 2026-09-02 | Michael Mauboussin / MSIM | own publication — Consilient Observer 全系列落地页 |
| T01-S010 | https://www.morganstanley.com/im/publication/insights/articles/article_capitalallocation.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — 资本配置五大用途与评估框架 |
| T01-S011 | https://www.morganstanley.com/im/publication/insights/articles/article_returnoninvestedcapital.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — ROIC 怎么算与常见坑 |
| T01-S012 | https://en.wikipedia.org/wiki/Michael_J._Mauboussin | secondary | 2026-09-02 | Wikipedia | 履历与任职沿革交叉核对 |
| T01-S013 | https://www.morganstanley.com/im/en-us/individual-investor/insights/consilient-observer/pattern-recognition-and-public-markets.html | surrogate_primary | 2026-09-02 | Mauboussin / MSIM | own publication — 2026 资本配置数据回溯至 1970 |
| T01-S014 | https://www.morganstanley.com/im/publication/insights/articles/article_roicandtheinvestmentprocess.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — ROIC 如何进入投资流程 |
| T01-S015 | https://www.morganstanley.com/im/publication/insights/articles/article_valuationmultiples.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — 倍数是压缩过的 DCF |
| T01-S016 | https://cup.columbia.edu/book/accounting-for-value/9780231151184/ | verified_primary | 2026-09-02 | Columbia University Press | publisher official page —《Accounting for Value》 |
| T01-S017 | https://business.columbia.edu/faculty/people/stephen-penman | verified_primary | 2026-09-02 | Columbia Business School | 官方教师页：George O. May 会计学讲席教授 |
| T01-S018 | https://www.degruyterbrill.com/document/doi/10.1515/ael-2013-0026/html | secondary | 2026-09-02 | Accounting, Economics & Law | 学界对 Penman 反 DCF 立场的正式评议 |
| T01-S019 | https://www.fondazioneoiv.it/wp-content/uploads/2019/05/OIVLecturePenman.pdf | secondary | 2026-09-02 | Fondazione OIV | Penman OIV 讲座全文：不要为推测付钱 |
| T01-S020 | https://www.latticework.com/p/stephen-penmans-masterclass-on-intrinsic | secondary | 2026-09-02 | Latticework / MOI Global | Penman 长访谈：内在价值、盈利质量、资本成本 |
| T01-S021 | https://www.berkshirehathaway.com/letters/1986.html | verified_primary | 2026-09-02 | Warren Buffett / Berkshire | owner earnings 定义原文（附录） |
| T01-S022 | https://www.berkshirehathaway.com/letters/letters.html | verified_primary | 2026-09-02 | Berkshire Hathaway | 1977 至今全部致股东信官方索引 |
| T01-S023 | https://www.berkshirehathaway.com/letters/2000pdf.pdf | verified_primary | 2026-09-02 | Warren Buffett / Berkshire | 2000 年信：对 EBITDA 与「非经常性」标签的直接批评 |
| T01-S024 | https://www.cnbc.com/2026/02/28/berkshire-ceo-abel-vows-to-keep-buffetts-culture-of-disciplined-investing-in-first-annual-letter.html | secondary | 2026-09-02 | CNBC | 2026-02-28 Abel 首封 CEO 信，Buffett 留任董事长 |
| T01-S025 | https://store.hbr.org/product/the-outsiders-eight-unconventional-ceos-and-their-radically-rational-blueprint-for-success/10344 | verified_primary | 2026-09-02 | Harvard Business Review Press | publisher official page —《The Outsiders》 |
| T01-S026 | https://www.50xpodcast.com/episodes/will-thorndike-the-power-of-long-holding-periods/ | verified_primary | 2026-09-02 | William Thorndike / 50X | own site — 长持有期与资本配置的完整长访谈 |
| T01-S027 | https://www.50xpodcast.com/ | verified_primary | 2026-09-02 | William Thorndike | own site — 本人主持的播客主站 |
| T01-S028 | https://valueandopportunity.com/2016/04/19/capital-allocation-capital-mangement-what-is-good-and-what-is-bad/ | secondary | 2026-09-02 | value and opportunity | 指出《The Outsiders》的幸存者偏差 |
| T01-S029 | https://www.mheducation.com/highered/mhp/product/financial-shenanigans-fourth-edition-how-detect-accounting-gimmicks-fraud-financial-reports.html | surrogate_primary | 2026-09-02 | McGraw-Hill Education | publisher official page —《Financial Shenanigans》第 4 版 |
| T01-S030 | https://www.aaii.com/authors/show/howard-schilit | secondary | 2026-09-02 | AAII | Schilit 作者页与面向散户的取证读表文章 |
| T01-S031 | https://moiglobal.com/howard-schilit-financial-shenanigans/ | secondary | 2026-09-02 | MOI Global | Schilit 长访谈落地页，含四大类舞弊框架 |
| T01-S032 | https://www.latticework.com/p/financial-shenanigans-how-to-detect | secondary | 2026-09-02 | Latticework / MOI Global | 2025-02-25 Schilit 独家长访谈 |
| T01-S033 | https://www.hbs.edu/faculty/Pages/profile.aspx?facId=6487 | verified_primary | 2026-09-02 | Harvard Business School | Robert S. Kaplan 官方教师页与全部著作 |
| T01-S034 | https://hbr.org/1988/09/measure-costs-right-make-the-right-decisions | verified_primary | 2026-09-02 | Cooper & Kaplan / HBR | 作业成本法 ABC 奠基文章 |
| T01-S035 | https://hbr.org/2004/11/time-driven-activity-based-costing | verified_primary | 2026-09-02 | Kaplan & Anderson / HBR | 自陈 ABC 实施常被放弃，改推 TDABC |
| T01-S036 | https://www.hbs.edu/ris/Publication%20Files/04-045_d62528d4-7931-4ea1-a205-d9683c639d6e.pdf | verified_primary | 2026-09-02 | Harvard Business School | TDABC 工作论文全文 PDF |
| T01-S037 | https://hbr.org/1992/01/the-balanced-scorecard-measures-that-drive-performance-2 | verified_primary | 2026-09-02 | Kaplan & Norton / HBR | 平衡计分卡原文，财务指标只是四象限之一 |
| T01-S038 | https://www.business-literacy.com/author/karen-berman-joe-knight/ | verified_primary | 2026-09-02 | Business Literacy Institute | own site — 作者与机构官方介绍页 |
| T01-S039 | https://store.hbr.org/product/financial-intelligence-revised-edition-a-manager-s-guide-to-knowing-what-the-numbers-really-mean/10833 | verified_primary | 2026-09-02 | Harvard Business Review Press | publisher official page —《Financial Intelligence》修订版 |
| T01-S040 | https://www.business-literacy.com/ | surrogate_primary | 2026-09-02 | Business Literacy Institute | own site — 财务素养培训机构主站 |
| T01-S041 | https://www.capitalallocators.com/podcast/pattern-recognition-and-public-markets/ | surrogate_primary | 2026-09-02 | Ted Seides / Capital Allocators | own site — Mauboussin 长对谈单集页（403 为反爬） |
| T01-S042 | https://aaahq.org/Accounting-Hall-of-Fame/Members/2019/Stephen-Harland-Penman | surrogate_primary | 2026-09-02 | American Accounting Association | originator — 会计名人堂 2019 入选者官方词条 |
| T01-S043 | https://business.columbia.edu/sites/default/files-efs/person/cv/Penman_CV%20June%202024.pdf | verified_primary | 2026-09-02 | Columbia Business School | Penman 本人 CV，更新至 2024-06 |
| T01-S044 | https://en.wikipedia.org/wiki/Owner_earnings | secondary | 2026-09-02 | Wikipedia | owner earnings 定义与出处交叉核对 |
| T01-S045 | https://www.joincolossus.com/episodes/88167992/thorndike-the-power-of-long-holding-periods | surrogate_primary | 2026-09-02 | Colossus / Invest Like the Best | own site — Thorndike EP.288 长访谈官方页 |
| T01-S046 | https://www.inc.com/john-case/karen-berman-patron-saint-of-open-book-management.html | secondary | 2026-09-02 | Inc. / John Case | Karen Berman 人物报道（403 为反爬） |
| T01-S047 | https://www.business-literacy.com/financial-intelligence/ | surrogate_primary | 2026-09-02 | Business Literacy Institute | own site — 财务素养在线课程与工具体系 |
| T01-S048 | https://simplenumbers.me/ | surrogate_primary | 2026-09-02 | Greg Crabtree | own site — Simple Numbers 官方站与 LER 工具 |
| T01-S049 | https://brandbuildersgroup.com/podcast/ep-591-simplifying-financial-success-for-entrepreneurs-greg-crabtree/ | verified_primary | 2026-09-02 | Brand Builders Group | 2025-05 长访谈：劳动效率比与贡献毛利 |
| T01-S050 | https://www.tengoldenrules.com/captivate-podcast/ep116-strategies-from-greg-crabtrees-fantastic-book-simple-numbers-for-big-profits/ | secondary | 2026-09-02 | Ten Golden Rules | 2026-06 长访谈：LER 2:1 为何是生死线 |
| T01-S051 | https://www.avalonaccounting.ca/books/simple-numbers-straight-talk-big-profits | secondary | 2026-09-02 | Avalon Accounting | 执业会计师对 Simple Numbers 四把钥匙的复盘 |
| T01-S052 | https://www.greatgame.com/podcast/author/greg-crabtree | secondary | 2026-09-02 | The Great Game of Business | 开卷管理阵营对 Crabtree 的常驻邀约 |
| T01-S053 | https://profitfirstbook.com/ | surrogate_primary | 2026-09-02 | Mike Michalowicz | own site — Profit First 官方书站与测算器 |
| T01-S054 | https://mikemichalowicz.com/profit-first/ | surrogate_primary | 2026-09-02 | Mike Michalowicz | own site — 作者本人站的 Profit First 页 |
| T01-S055 | https://profitfirstprofessionals.com/ | surrogate_primary | 2026-09-02 | Profit First Professionals | own site — 会计师/记账师认证体系官方站 |
| T01-S056 | https://sbo.financial/blog/accountants/accountants-review-profit-first/ | secondary | 2026-09-02 | SBO Financial | 会计师视角的系统性批评：把利润定义成现金 |
| T01-S057 | https://wanderwellconsulting.com/why-i-dont-recommend-profit-first/ | secondary | 2026-09-02 | Wanderwell Consulting | 记账事务所「为什么我不推荐 Profit First」 |
| T01-S058 | https://en.wikipedia.org/wiki/Mike_Michalowicz | secondary | 2026-09-02 | Wikipedia | 著作年表与出版社沿革交叉核对 |
| T01-S059 | https://www.venturedeals.com/ | surrogate_primary | 2026-09-02 | Brad Feld & Jason Mendelson | own site — Venture Deals 官方书站与免费课 |
| T01-S060 | https://feld.com/ | surrogate_primary | 2026-09-02 | Brad Feld | own site — 20 余年持续更新的个人博客 |
| T01-S061 | https://feld.com/archives/category/term-sheet/ | surrogate_primary | 2026-09-02 | Brad Feld | own site — Term Sheet 连载全归档，本书原型 |
| T01-S062 | https://www.wiley.com/en-us/Venture+Deals:+Be+Smarter+Than+Your+Lawyer+and+Venture+Capitalist,+4th+Edition-p-9781119594840 | surrogate_primary | 2026-09-02 | Wiley | publisher official page — 第 4 版 |
| T01-S063 | https://www.jasonmendelson.com/ | surrogate_primary | 2026-09-02 | Jason Mendelson | own site — 合著者本人站（律师 + VC 双背景） |
| T01-S064 | https://www.forentrepreneurs.com/saas-metrics-2/ | verified_primary | 2026-09-02 | David Skok | own site — SaaS Metrics 2.0，单位经济学奠基长文 |
| T01-S065 | https://www.forentrepreneurs.com/saas-economics-1/ | verified_primary | 2026-09-02 | David Skok | own site — SaaS 现金流低谷：越快增长越缺钱 |
| T01-S066 | https://www.intercom.com/blog/podcasts/david-skok-on-the-metrics-every-saas-company-should-be-tracking/ | verified_primary | 2026-09-02 | Intercom | Skok 长访谈：该盯哪些指标、什么阶段盯什么 |
| T01-S067 | https://www.saastr.com/david-skok-gp-matrix-partners-driving-saas-success-using-key-metrics-video-transcript/ | secondary | 2026-09-02 | SaaStr | Skok 大会演讲视频 + 完整文字稿 |
| T01-S068 | https://chartmogul.com/blog/david-skok-on-choosing-the-right-metrics-for-the-right-growth-stage/ | secondary | 2026-09-02 | ChartMogul | Skok 访谈：不同增长阶段盯不同指标 |
| T01-S069 | https://www.craftventures.com/articles/the-burn-multiple | surrogate_primary | 2026-09-02 | David Sacks / Craft Ventures | own publication — Burn Multiple 原文 |
| T01-S070 | https://www.craftventures.com/articles/applying-the-burn-multiple-to-marketplace-business-models | surrogate_primary | 2026-09-02 | Craft Ventures | own publication — 把 burn multiple 推广到平台型业务 |
| T01-S071 | https://medium.com/craft-ventures/the-burn-multiple-51a7e43cb200 | secondary | 2026-09-02 | Craft Ventures（官方 Medium） | 2020-04-23 首发版本，用于确认原始日期 |
| T01-S072 | https://www.thetwentyminutevc.com/davidsacks | secondary | 2026-09-02 | 20VC / Harry Stebbings | Sacks 长访谈：CAC、burn、churn 与董事会 |
| T01-S073 | https://www.cnbc.com/2026/03/26/david-sacks-trump-crypto-ai-czar.html | secondary | 2026-09-02 | CNBC | 2026-03-26 Sacks 卸任 AI/加密沙皇 |
| T01-S074 | https://techcrunch.com/2026/03/26/david-sacks-is-done-as-ai-czar-heres-what-hes-doing-instead/ | secondary | 2026-09-02 | TechCrunch | 同日报道：转任 PCAST 联席主席 |
| T01-S075 | https://www.mostlymetrics.com/ | surrogate_primary | 2026-09-02 | CJ Gustafson | own site — Mostly Metrics 主站（403 为反爬） |
| T01-S076 | https://cjgustafson.substack.com/s/run-the-numbers | verified_primary | 2026-09-02 | CJ Gustafson | Run the Numbers 播客官方栏目页 |
| T01-S077 | https://podcast.growthinreverse.com/episodes/cj-gustafson | secondary | 2026-09-02 | Growth In Reverse | 长访谈：newsletter 如何做到 6 万订阅与营收 |
| T01-S078 | https://ramp.com/authors/cj-gustafson | secondary | 2026-09-02 | Ramp | 第三方机构作者页，交叉确认在职 CFO 身份 |
| T01-S079 | https://www.sem.tsinghua.edu.cn/info/1205/32025.htm | verified_primary | 2026-09-02 | 清华大学经管学院 | 肖星官方教师页：会计系系主任、长聘教授 |
| T01-S080 | https://www.tsinghua.edu.cn/info/1179/109414.htm | verified_primary | 2026-09-02 | 清华大学 | 新百年教学成就奖官方人物报道 |
| T01-S081 | https://www.xuetangx.com/course/THU08091000367 | secondary | 2026-09-02 | 学堂在线 / 清华大学 | 《财务分析与决策》国家级一流本科课程页 |
| T01-S082 | https://book.douban.com/subject/34810876/ | verified_primary | 2026-09-02 | 豆瓣读书 | 肖星《一本书读懂财报》修订版权威书目条目 |
| T01-S083 | https://kyc.uibe.edu.cn/kydt/bdd184eac0be408392b46ea124460a5e.htm | verified_primary | 2026-09-02 | 对外经贸大学科研处 | 张新民「财务报表、企业战略与竞争力分析」官方通稿 |
| T01-S084 | https://www.icourse163.org/course/UIBE-1003252013 | secondary | 2026-09-02 | 中国大学MOOC / 对外经贸 | 张新民《财务报表分析》国家级慕课 |
| T01-S085 | https://cem.swu.edu.cn/info/1247/6266.htm | verified_primary | 2026-09-02 | 西南大学经管学院 | 第三方高校对张新民专题讲座的官方记录 |
| T01-S086 | https://soa.cufe.edu.cn/info/1025/6867.htm | verified_primary | 2026-09-02 | 中央财经大学会计学院 | 2024-05 张新民讲座官方记录（美的/格力案例） |
| T01-S087 | https://book.douban.com/subject/36285053/ | verified_primary | 2026-09-02 | 豆瓣读书 | 张新民《财务报表分析》第 6 版书目条目 |
| T01-S088 | https://www.ifrs.org/news-and-events/news/2026/08/steven-maijoor-chair-trustees-sam-woods-chair-iasb/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator official — Sam Woods 任 IASB 主席公告 |
| T01-S089 | https://www.ifrs.org/news-and-events/news/2026/06/update-on-appointment-of-new-iasb-chair/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator official — 主席交接与代理安排 |
| T01-S090 | https://www.ifrs.org/groups/international-accounting-standards-board/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator official — IASB 现任理事名单 |
| T01-S091 | https://www.fasb.org/about-us/board-members/richard-r-jones | surrogate_primary | 2026-09-02 | FASB | originator official — 现任主席页（403 为反爬） |
| T01-S092 | https://kjs.mof.gov.cn/ | verified_primary | 2026-09-02 | 中国财政部会计司 | 中国会计准则的实际制定与解释机关 |
| T01-S093 | https://www.imaglobal.org/ | surrogate_primary | 2026-09-02 | IMA | originator official — 管理会计师协会与 CMA 知识体系 |
| T01-S094 | https://www.aicpa-cima.com/resources/landing/management-accounting-cgma | surrogate_primary | 2026-09-02 | AICPA & CIMA | originator official — CGMA 管理会计能力框架 |
| T01-S095 | https://www.thesaascfo.com/ | surrogate_primary | 2026-09-02 | Ben Murray | own site — SaaS 财务口径与模板 |
| T01-S096 | https://www.thesaasacademy.com/podcasts/saas-metrics-school | verified_primary | 2026-09-02 | Ben Murray | SaaS Metrics School：单集 10 分钟讲透一个指标 |
| T01-S097 | https://www.saastr.com/category/podcasts/ | surrogate_primary | 2026-09-02 | Jason Lemkin / SaaStr | own publication — SaaStr 播客归档 |
| T01-S098 | https://bbrt.org/ | surrogate_primary | 2026-09-02 | Beyond Budgeting Round Table | originator official — Beyond Budgeting 12 原则 |
| T01-S099 | https://papers.ssrn.com/sol3/papers.cfm?abstract_id=267651 | verified_primary | 2026-09-02 | Michael C. Jensen / SSRN | 《Paying People to Lie》预算与奖金挂钩的论文版 |
| T01-S100 | https://secretcfonotebook.substack.com/p/who-the-fck-is-the-secret-cfo | verified_primary | 2026-09-02 | The Secret CFO | 匿名 CFO 自述身份与写作动机 |
| T01-S101 | https://paccesc.ruc.edu.cn/info/1118/3029.htm | verified_primary | 2026-09-02 | 全国会计专业学位研究生教育指导委员会 | 官方委员页：肖星的学术任职 |
| T01-S102 | https://www.tsinghua.org.cn/info/1012/39739.htm | verified_primary | 2026-09-02 | 清华校友总会 | 肖星讲座「从财务视角看科创企业价值创造」官方记录 |
| T01-S103 | https://www.tsinghua.edu.cn/info/1179/17161.htm | verified_primary | 2026-09-02 | 清华大学 | 肖星人物报道：教学与私募股权研究 |
| T01-S104 | https://book.douban.com/subject/35033236/ | verified_primary | 2026-09-02 | 豆瓣读书 | 《肖星的财务思维课》（机械工业出版社 2020）书目条目 |
| T01-S105 | https://kjxy.dufe.edu.cn/content_67533.html | verified_primary | 2026-09-02 | 东北财经大学会计学院 | 知名会计学者论坛：张新民专场官方记录 |
| T01-S106 | http://kjs.mof.gov.cn/gongzuotongzhi/202606/t20260618_3991879.htm | verified_primary | 2026-09-02 | 中国财政部会计司 | 2026-06-18 准则实施问答与应用案例（第二批） |
| T01-S107 | http://kjs.mof.gov.cn/zt/kjzzss/qykjzzjs/index.htm | verified_primary | 2026-09-02 | 中国财政部会计司 | 企业会计准则解释全量目录（含第 19/20 号） |
| T01-S108 | https://en.wikipedia.org/wiki/Sam_Woods_(civil_servant) | secondary | 2026-09-02 | Wikipedia | Sam Woods 履历交叉核对（英国 PRA 首席执行官） |

---

## 总览（按阵营分组）

> 排序依据：`endorsement 独立来源数` × `长材料厚度` × `与「创业公司/中小企业内部财务判断」的对齐度`。
> **对齐度**这一列是本 track 的裁决关键——很多人在财经圈影响力更大，但谈的是二级市场选股或并购执行，不进本榜。

| # | 姓名 | 阵营 | 一句话贡献 | 长材料 | 近 12 个月动态 | 争议栏 | 对齐度 |
|---|------|------|-----------|-------|--------------|-------|-------|
| 1 | Aswath Damodaran | 公司金融估值派 | 估值靠假设的诚实，不靠数据垄断 | 📖🎙️🎬 | ✅ 2026-01/02 多档长访谈 | ✅ | 高 |
| 2 | Michael Mauboussin | 公司金融估值派 / 资本配置 | 只有 ROIC > 资本成本的增长才创造价值 | 📖🎙️ | ✅ 2026 资本配置更新版 | ✅ | 中高 |
| 3 | Stephen Penman | 会计估值派（反 DCF） | 锚定已知，不为推测付钱 | 📖🎙️ | ❌ 未检索到 | ✅ | 中 |
| 4 | Warren Buffett & Charlie Munger | 价值投资资本配置派 | owner earnings：折旧是真实费用 | 📖🎬 | ✅ 2025 末卸任 CEO / 2026-02 交接 | ✅ | 中高 |
| 5 | William Thorndike | 价值投资资本配置派 | CEO 的第一职责是资本配置 | 📖🎙️ | ✅ 持续主持 50X | ✅ | 中 |
| 6 | Howard Schilit | 报表取证与准则合规派 | 看财报不是阅读，是质询 | 📖🎙️ | ❌ 最近为 2025-02 | ✅ | 中高 |
| 7 | Robert S. Kaplan | 管理会计决策派 | 分摊方式决定你以为谁在赚钱 | 📖 | ❌ 未检索到 | ✅ | 高 |
| 8 | Karen Berman & Joe Knight | 财务素养普及派 | 利润是估计，现金是事实 | 📖🎬 | ❌ 未检索到 | ✅ | 高 |
| 9 | Greg Crabtree | 中小企业现金实操派 | 老板先拿市价工资，剩下的才叫利润 | 📖🎙️ | ✅ 2026-06 长访谈 | ✅ | **最高** |
| 10 | Mike Michalowicz ⚠️ | 中小企业现金实操派（行为派） | 收入 − 利润 = 费用 | 📖🎬 | ✅ 2026 新书 | ✅✅ | 中高 |
| 11 | Brad Feld & Jason Mendelson | 创业融资与条款派 | term sheet 是经济与控制两场谈判 | 📖🎬 | ❌ 未检索到 | ✅ | 高 |
| 12 | David Skok | 创业与 SaaS 单位经济派 | 增长越快现金越紧 | 📖🎙️ | ❌ 更新停滞 | ✅ | 高 |
| 13 | David Sacks | 创业与 SaaS 单位经济派 | burn multiple：不预测的效率指标 | 📖🎙️ | ✅ 2026-03 卸任公职 | ✅ | 中高 |
| 14 | CJ Gustafson | 在职实操派 | 年度预算是三个月的协商过程 | 📖🎙️ | ✅ 每周两更 | ✅ | 高 |
| 15 | 肖星 | 中文学院派（普及） | 三张表各回答一个不同问题 | 📖🎬 | ❌ 未检索到 | ✅ | 高 |
| 16 | 张新民 | 中文学院派（战略视角） | 同样的数字，质量可以完全不同 | 📖🎬 | ❌ 未检索到 | ✅ | 高 |

**符号说明**：📖 长文/书 ｜ 🎙️ 长音频访谈 ｜ 🎬 视频课/大会演讲 ｜ ✅ 有 ｜ ❌ 未检索到 ｜ ⚠️ 争议人物

**近 12 个月有公开动态的比例：8/16 = 50%**。这是本 track 的一个真实弱点，原因见 §Phase 2 提炼提示的「冷僻信号」小节。

---

## 1. 公司金融估值派

### 1. Aswath Damodaran（阿斯瓦斯·达摩达兰）

- **核心一句话**：估值不是靠数据垄断，而是靠**把假设摊在桌面上的诚实**——你的故事必须能翻译成增长率、利润率、再投资率三个数字，数字也必须能翻译回一个你敢讲出口的故事。(evidence: [T01-S008, T01-S007])
- **身份与阵营**：**公司金融估值派**。NYU Stern 金融学教授（Kerschner Family 金融教育讲席），业内称「估值院长」。极端反常规的一点是他把整套课程、讲义、Excel 模板与全球行业数据集**全部免费公开**，不设付费墙。(evidence: [T01-S001, T01-S004, T01-S003])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **DCF Myths 系列（10 篇长文）** — 逐条拆掉「有折现率就能估值」「DCF 只适合成熟稳定公司」等常见误解，是理解他方法论的最短路径。https://aswathdamodaran.blogspot.com/2015/02/dcf-myth-1-if-you-have-ddiscount-rate.html (evidence: [T01-S007])
  - 🎙️ **The Meb Faber Show #619（2026-02）** — 长访谈，主题是 AI 资本开支：他讨论 AI 对估值与护城河的影响、软件在位者面临的创新者窘境、以及债务驱动的资本开支风险。https://www.themebfabershow.com/episodes/oILab0ZBVxs (evidence: [T01-S005])
  - 🎬 **Valuation Online Class（25 讲免费 webcast + slides + 课后测验）** — 完整复刻他学期估值课；配套的免费行业数据集每年 1 月刷新（beta / WACC / 利润率 / ROIC）。https://pages.stern.nyu.edu/~adamodar/New_Home_Page/webcastvalonline.htm (evidence: [T01-S004, T01-S003])
- **争议 / 非主流立场**：
  1. **来自会计学阵营的正面否定**：Stephen Penman 认为「把对风险的理解压缩成一个叫资本成本的数字」是虚构，且自由现金流不是价值增加量（投资使 FCF 变负、清算反而使 FCF 变正）。这直接否定 Damodaran 体系的两根支柱。(evidence: [T01-S019, T01-S016, T01-S018])
  2. **公开给热门股定价的路径依赖**：他习惯对 Tesla、Nvidia、SpaceX 等争议标的公开出具估值并复盘，批评者认为这恰恰暴露了 DCF 在高不确定性资产上的脆弱；他本人的回应是估值的价值在于**暴露隐含假设**而非预测准确。本条为**推断性归纳**，未找到单一权威来源直接如此表述。
  3. **对「护城河讲故事」的排斥**：他坚持任何定性叙事必须落到具体数字上，否则不算估值——这让他和偏定性的价值投资圈长期紧张。(evidence: [T01-S008])
- **最近 12 个月动态**：2026-01 MicroCapClub 长对谈（个人史 + 教学观 + 实用主义估值）；2026-02 Meb Faber Show #619 谈 AI 资本开支泡沫；2026-01 Create More Value 播客第 49 集，公开质疑「ROIC、资本成本、激励指标」的常规用法；据搜索结果，2026-06 与 Sparkline Capital 的 Kai Wu 谈 SpaceX 估值（约 1.3 万亿美元量级，**为其个人估算，非市场共识**）。(evidence: [T01-S006, T01-S005])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典把《Investment Valuation》《Narrative and Numbers》与其免费数据集同时列为必读，属独立于本 track 的引用；② Track 05 把他的 Substack 与 NYU 数据集分别列为 newsletter 与 dataset 两个维度的核心源；③ NYU Stern 官方教师页与讲席教授职位。(evidence: [T01-S001, T01-S002, T01-S003])
- **核心思想关键词**：叙事与数字互相约束 / 假设的诚实 / 估值 ≠ 定价（pricing vs valuation） / 免费数据的民主化 / 隐含风险溢价
- **sub_skill_candidate**: `true` — 一手材料密度全行业最高（25 讲公开课 + 十余年博客 + 每年刷新的数据集），思想体系自洽，且「估值」是创始人融资与股权稀释判断的直接上游。
- **可信度自评**: high

---

### 2. Michael Mauboussin（迈克尔·莫布森）

- **核心一句话**：**增长本身不创造价值，只有 ROIC 高于资本成本时的增长才创造价值**；而 ROIC 的分子分母都被会计准则扭曲了（研发、营销、租赁、商誉），所以第一步永远是把口径修回来。(evidence: [T01-S011, T01-S010])
- **身份与阵营**：**公司金融估值派 / 资本配置派**。Morgan Stanley Investment Management 旗下 Counterpoint Global 的 Consilient Research 主管；此前长期任 Credit Suisse 与 Legg Mason 首席投资策略师，并在哥伦比亚商学院长期兼课。(evidence: [T01-S009, T01-S012])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **Return on Invested Capital: How to Calculate ROIC and Handle Common Issues** — 全行业最实用的 ROIC 计算手册，逐项处理经营租赁资本化、研发费用化 vs 资本化、超额现金、商誉等口径坑。https://www.morganstanley.com/im/publication/insights/articles/article_returnoninvestedcapital.pdf (evidence: [T01-S011])
  - 📖 **Capital Allocation（2026 更新版，数据回溯至 1970、覆盖至 2024）** — 把公司能对现金做的事收敛成有限几种用途（并购 / 资本开支 / 研发 / 分红 / 回购 / 还债），并给出一套评估管理层配置能力的框架：过往行为 + ROIC + 激励设计。https://www.morganstanley.com/im/publication/insights/articles/article_capitalallocation.pdf (evidence: [T01-S010, T01-S013])
  - 🎙️ **Capital Allocators with Ted Seides — Pattern Recognition and Public Markets** — 与其研究配套的长对谈，谈公开市场结构变化与模式识别的边界。https://www.capitalallocators.com/podcast/pattern-recognition-and-public-markets/ (evidence: [T01-S013, T01-S041])
- **争议 / 非主流立场**：
  1. **「倍数不是估值方法，是压缩过的 DCF」** — 他明确主张 P/E、EV/EBITDA 这类倍数只是把一堆 DCF 假设塞进一个数字，用倍数「代替」估值是自欺。这直接冲撞卖方与 PE 圈以可比公司倍数为主的日常做法。(evidence: [T01-S015])
  2. **对报表原样 ROIC 的不信任** — 他要求对无形资产投入做资本化调整，而这类调整在准则合规派看来是「自制会计」，缺乏可审计性与可比性。矛盾保留：两派对「什么叫真实资本」根本没有共识。(evidence: [T01-S011, T01-S014])
  3. 他的研究几乎全部服务于**二级市场选股**语境。对创始人而言，价值在于口径与因果框架，而**不是**直接照搬其结论——本条是本 track 的使用告诫。
- **最近 12 个月动态**：2026 年发布 Capital Allocation 更新版，把资本配置与 ROIC 数据序列回溯至 1970 年、更新至 2024 年；Consilient Observer 系列保持持续更新。(evidence: [T01-S013, T01-S009])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典独立收录其 ROIC / 资本配置 / 倍数三篇研究；② Track 05 把 Consilient Observer 列为核心 newsletter；③ 被 Capital Allocators（Ted Seides）反复邀为嘉宾，属第三方长访谈背书。(evidence: [T01-S009, T01-S013, T01-S041])
- **核心思想关键词**：ROIC vs 资本成本 / 资本配置五大用途 / 倍数是压缩的 DCF / 会计口径修复 / 基准率（base rates）
- **sub_skill_candidate**: `true` — 研究体系自洽、公开长文密度极高，且「ROIC 口径怎么修」是中小企业算真实回报时的核心方法。
- **可信度自评**: high

---

### 3. Stephen Penman（斯蒂芬·佩因曼）

- **核心一句话**：**先锚定你已经知道的（账面价值与已实现盈利），把推测放到最后**；为推测付钱是投资亏损的主要来源。(evidence: [T01-S016, T01-S019])
- **身份与阵营**：**公司金融估值派内部的反对派 / 会计估值派**。哥伦比亚商学院 George O. May 财务会计学荣休讲席教授（2023 年起任 Special Lecturer），美国会计学会（AAA）会计名人堂 2019 年入选者。(evidence: [T01-S017, T01-S042])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **《Accounting for Value》（Columbia University Press, 2011）** — 系统性放下资本成本、CAPM 与 DCF，回到会计锚。https://cup.columbia.edu/book/accounting-for-value/9780231151184/ (evidence: [T01-S016])
  - 📖 **OIV Lecture: Accounting for Value — Protection from Paying Too Much（讲座全文 PDF）** — 比书更集中的一次论证，直接给出「不要为推测付钱」的操作路径。https://www.fondazioneoiv.it/wp-content/uploads/2019/05/OIVLecturePenman.pdf (evidence: [T01-S019])
  - 🎙️ **Latticework / MOI Global 长访谈 — 内在价值、盈利质量、资本成本与自欺** — 他在访谈里把「资本成本是个人的、主观的门槛率」这一非主流立场讲得最清楚。https://www.latticework.com/p/stephen-penmans-masterclass-on-intrinsic (evidence: [T01-S020])
- **争议 / 非主流立场**（本 track 中立场最硬的一位）：
  1. **资本成本是虚构**：他认为把对一家企业风险的理解压缩成单一数字是现代金融「最令人失望的部分」，主张把门槛率当作**投资人自己的要求回报**，而不是可客观测算的市场参数。这直接冲撞 Damodaran / Mauboussin / 教科书 WACC 体系。(evidence: [T01-S019, T01-S020])
  2. **自由现金流不是价值增加量**：FCF = 经营现金流 − 投资现金流，于是**投资会压低 FCF、清算会抬高 FCF**——一家投得越多越好的公司反而 FCF 为负。他据此否定 FCF 作为价值度量的资格。(evidence: [T01-S019])
  3. **反对者说什么**：《Accounting, Economics and Law》上的正式评议指出，Penman 的路径把估值对**会计政策与保守主义程度**的依赖放大了，换了一套主观性而已；且他的模型在会计口径差异大的跨国比较中失效。矛盾保留，不和稀泥。(evidence: [T01-S018])
- **最近 12 个月动态**：⚠️ **未检索到近 12 个月公开动态**。已确认的最近状态是 2023 年起在哥伦比亚商学院任 Special Lecturer、CV 更新至 2024-06。(evidence: [T01-S017, T01-S043])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典独立收录《Accounting for Value》并单列其「对 DCF 体系的正面否定」；② 美国会计学会会计名人堂 2019 入选（同行机构评选，非自营销）；③ 《Accounting, Economics and Law》为其著作组织专门评议专栏——学界认真反驳本身就是影响力证据。(evidence: [T01-S042], [T01-S018])
- **核心思想关键词**：锚定已知 / 不为推测付钱 / 会计保守主义是保护 / 反资本成本 / 盈利质量
- **sub_skill_candidate**: `false` — 思想极其重要，但公开长材料以学术著作与少量讲座为主，缺少面向经营者的实操输出；更适合作为 Phase 2 的「反面校验器」而非独立 sub-skill。
- **可信度自评**: medium — 思想脉络证据充分，但「当前 active」一项无近 12 个月证据。

---

---

## 2. 价值投资与资本配置派

### 4. Warren Buffett & Charlie Munger（沃伦·巴菲特 与 查理·芒格）

- **核心一句话**：**报表利润不是所有者能拿走的钱**——要减掉为维持现有竞争力必须持续投入的资本开支，剩下的才叫 owner earnings（所有者盈余）；任何绕开折旧的指标都在替管理层美化。(evidence: [T01-S021, T01-S023])
- **身份与阵营**：**价值投资资本配置派**。Buffett 于 2025 年底卸任 Berkshire Hathaway CEO、由 Greg Abel 接任，本人留任董事长；Munger 已故（本 track 只使用其留存文本与被反复记录的公开表述）。(evidence: [T01-S024, T01-S022])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **1986 年致股东信附录「owner earnings」原文** — 这一页定义了 owner earnings = 报告利润 + 折旧摊销等非现金费用 − 维持性资本开支，并直言这个数字**无法精确算出，但近似正确远胜精确错误**。https://www.berkshirehathaway.com/letters/1986.html (evidence: [T01-S021])
  - 📖 **2000 年致股东信** — 对 EBITDA 与「一次性 / 非经常性」标签的直接批评，是理解「为什么折旧是真实费用」的一手文本。https://www.berkshirehathaway.com/letters/2000pdf.pdf (evidence: [T01-S023])
  - 🎬 **全部致股东信官方索引（1977 至今，免费）** — 连读比任何二手解读都有效；官方站点无付费墙、无广告。https://www.berkshirehathaway.com/letters/letters.html (evidence: [T01-S022])
- **争议 / 非主流立场**：
  1. **Munger 的 EBITDA 定性**：他主张每次看到 EBITDA 就把它换成「狗屁盈利（bullshit earnings）」，理由是折旧是**已经先花掉的现金**，不是非现金费用。这句被广泛转引的表述出自《Poor Charlie's Almanack》语境；⚠️ 本 track **未能定位到 Berkshire 官方站上的逐字原文**，故标为**广泛转述、非官方一手**。反对者（PE 与杠杆融资圈）认为 EBITDA 作为**偿债能力与经营现金生成的近似**有其正当用途，两方争的其实是「用在哪个问题上」。
  2. **对股权激励费用化的立场**：Buffett 长期主张股票期权是货真价实的薪酬费用，必须进损益表；科技行业长期以「摊薄已在每股收益里体现」为由抗辩。本条为立场层面的记录，具体条文请回到原信核对。(evidence: [T01-S022])
  3. **对创业公司的适用性争议**：owner earnings 假设企业已有稳定的维持性资本开支基线，早期公司维持性与扩张性资本开支难以拆分，直接套用会得到无意义的负数——这是本 track 认定的**最重要使用边界**。
- **最近 12 个月动态**：2025 年底 Buffett 卸任 CEO；2026-02-28 Greg Abel 发出首封 CEO 致股东信，承诺延续「财务保守与纪律性投资」的文化；Buffett 留任董事长并仍每日到岗。(evidence: [T01-S024])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典把 1986 年信列为必读正典条目；② Thorndike《The Outsiders》把 Buffett 列为八位资本配置型 CEO 之一，并获 Buffett 在 2012 年致股东信中公开推荐——**互相点名**属强背书；③ owner earnings 已成为独立词条进入通用参考体系。(evidence: [T01-S021, T01-S025], [T01-S044])
- **核心思想关键词**：owner earnings / 维持性资本开支 / 折旧是真实费用 / 留存一美元创造一美元市值 / 能力圈
- **sub_skill_candidate**: `false`（作为独立人物）——但 owner earnings 与资本配置纪律应作为 Phase 2 的**核心心智模型**直接提炼。
- **可信度自评**: high（文本一手且免费公开）；Munger 语录部分 medium（转述来源）。

---

### 5. William Thorndike（威廉·索恩代克）

- **核心一句话**：**CEO 的第一职责不是运营，是资本配置**——长期回报的差距主要由「钱往哪儿放」决定，而不是由行业或运营天赋决定。(evidence: [T01-S025, T01-S026])
- **身份与阵营**：**价值投资资本配置派**。Housatonic Partners 联合创始人（1994 年创立，以超长持有期与 search fund 生态闻名）、50X 播客主持人、《The Outsiders》作者。(evidence: [T01-S027, T01-S026])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **《The Outsiders: Eight Unconventional CEOs...》（HBR Press, 2012）** — 研究八位 CEO（含 Berkshire、Teledyne、Capital Cities、General Dynamics、TCI、Washington Post 等），共同特征是盯每股价值、对现金流而非报告利润下注、极度分权的运营 + 极度集权的资本决策。https://store.hbr.org/product/the-outsiders-eight-unconventional-ceos-and-their-radically-rational-blueprint-for-success/10344 (evidence: [T01-S025])
  - 🎙️ **50X Podcast — Will Thorndike: The Power of Long Holding Periods** — 他自己主持的节目，也是他把「长持有期 + 资本配置」讲得最完整的地方。https://www.50xpodcast.com/episodes/will-thorndike-the-power-of-long-holding-periods/ (evidence: [T01-S026])
  - 🎙️ **Invest Like the Best（Patrick O'Shaughnessy）长访谈** — 第三方主持的长对谈版本，主题为「优秀资本配置者如何复利」。(evidence: [T01-S045])
- **争议 / 非主流立场**：
  1. **幸存者偏差是最主要的反驳**：批评者指出八个样本全部是事后挑出的赢家，同样的「大手笔回购 + 高杠杆 + 分权」组合在失败公司里同样常见，因此该书证明的是相关而非因果。(evidence: [T01-S028])
  2. **回购被当作通用武器的风险**：书中把机会性回购塑造成资本配置的高阶动作，后来被广泛引用为「回购总是好的」；在利率上行与估值高企时期，这一读法会造成实质损害。本条为本 track 对误读风险的判断。
  3. **对中小企业的适用边界**：书中主角多为有稳定自由现金流的成熟企业，创业公司没有可配置的现金，真正可迁移的是**决策的集中度与每股口径**，不是回购本身。
- **最近 12 个月动态**：持续主持 50X 播客（以「50 倍回报的公司/投资人」为选题）；据搜索结果，2025-06 曾在 Joys of Compounding 播客做长访谈。未检索到新书出版。(evidence: [T01-S027])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典独立收录《The Outsiders》；② Buffett 在 2012 年致股东信中公开推荐该书（跨阵营背书）；③ 被 Invest Like the Best、Capital Allocators 生态的多档节目独立邀为嘉宾。(evidence: [T01-S025, T01-S026, T01-S045])
- **核心思想关键词**：资本配置是 CEO 主业 / 每股价值 / 分权运营 + 集权配置 / 机会性回购 / 长持有期
- **sub_skill_candidate**: `false` — 一本书 + 若干访谈，思想密度高但输出体量有限；更适合作为 Phase 2 的资本配置章节素材。
- **可信度自评**: high

---

---

## 3. 报表取证与准则合规派

### 6. Howard Schilit（霍华德·席利特）

- **核心一句话**：**看财报不是阅读，是质询**——管理层的会计选择本身就是信号，你的任务是找出「哪一处的数字被时间、被分类、被口径挪动了」。(evidence: [T01-S029, T01-S031])
- **身份与阵营**：**报表取证与准则合规派**。取证会计（forensic accounting，用会计线索反查经营与舞弊的方法）领域的开创者之一，业内称「会计界的福尔摩斯」；创办 CFRA 后又创办 Schilit Forensics，客户为对冲基金、主权基金、共同基金等机构；曾就财务舞弊议题向美国国会与 SEC 作证。(evidence: [T01-S031, T01-S029])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **《Financial Shenanigans》第 4 版（McGraw-Hill, 2018）** — 把造假手法系统归为四大类：夸大收入、夸大利润（费用挪移）、现金流舞弊、关键指标舞弊；第 4 版重点补进了近 25 年的全球案例。https://www.mheducation.com/highered/mhp/product/financial-shenanigans-fourth-edition-how-detect-accounting-gimmicks-fraud-financial-reports.html (evidence: [T01-S029])
  - 🎙️ **MOI Global / Latticework 独家长访谈（2025-02-25）** — 目前可检索到的最新一次系统性长访谈，覆盖其四类框架与近年案例。https://www.latticework.com/p/financial-shenanigans-how-to-detect (evidence: [T01-S032, T01-S031])
  - 📖 **AAII 作者页（面向非机构读者的取证读表文章合集）** — 把机构方法降维到个人投资者能用的检查清单。https://www.aaii.com/authors/show/howard-schilit (evidence: [T01-S030])
- **争议 / 非主流立场**：
  1. **「所有会计选择都值得怀疑」的立场成本很高**：批评者认为取证式读表天然偏向假阳性——大量被标红的公司最终并无舞弊，只是行业惯例或准则允许的判断差异。对创始人来说，把这套用在自己公司上容易导致过度保守的会计政策。本条为本 track 的**使用边界判断**，非引自单一来源。
  2. **与准则制定机构的隐含张力**：他的核心论点之一是**准则允许的空间本身就是造假的温床**（收入确认时点、费用资本化、经营性 vs 投资性现金流分类），这与准则机构「原则导向、依赖职业判断」的立场直接冲突。(evidence: [T01-S029])
  3. **业务模式的利益结构**：Schilit Forensics 服务的是能从做空或规避踩雷中获益的机构客户，读者需意识到样本选择偏向「找问题」。
- **最近 12 个月动态**：⚠️ **未检索到近 12 个月（2025-09 至 2026-09）公开动态**。已确认的最近一次公开长访谈为 2025-02-25 的 MOI Global 独家访谈。(evidence: [T01-S032])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典独立收录《Financial Shenanigans》第 4 版；② MOI Global / Latticework 作为面向机构投资者的付费社群，独立邀其做长访谈；③ AAII（美国个人投资者协会）设有其作者页——三类互不隶属的机构。(evidence: [T01-S029, T01-S031, T01-S030])
- **核心思想关键词**：四类舞弊 / 收入质量 / 现金流分类操纵 / 关键指标（non-GAAP）操纵 / 会计选择即信号
- **sub_skill_candidate**: `false` — 方法论价值高但材料以书为主，长音视频稀薄；建议作为 Phase 2「读表红旗清单」的素材来源。
- **可信度自评**: medium — 思想与著作证据充分，但一手发声渠道（个人站/newsletter）缺失，近 12 个月无动态。

---

---

## 4. 管理会计决策派

### 7. Robert S. Kaplan（罗伯特·卡普兰）

- **核心一句话**：**你分摊间接费用的方式，决定了你以为哪些产品和客户在赚钱**——传统按人工工时或销售额分摊会系统性高估复杂小批量产品的盈利能力，把定价和砍产品线的决策全部带偏。(evidence: [T01-S034, T01-S035])
- **身份与阵营**：**管理会计决策派**的奠基者。哈佛商学院 Marvin Bower 领导力发展荣休讲席教授、高级研究员；作业成本法（ABC，按「作业」而非产量分摊间接费用）与平衡计分卡的共同提出者。(evidence: [T01-S033])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **Measure Costs Right: Make the Right Decisions（Cooper & Kaplan, HBR 1988）** — ABC 的奠基文章，核心论断是「成本失真的方向是可预测的：高产量简单品被高估成本，低产量复杂品被低估」。https://hbr.org/1988/09/measure-costs-right-make-the-right-decisions (evidence: [T01-S034])
  - 📖 **Time-Driven Activity-Based Costing（Kaplan & Anderson, HBR 2004）** — **他自己承认 ABC 失败**的那篇：大量企业因为成本高、员工反感、维护困难而中途放弃 ABC；TDABC 改为估算每笔交易占用的时间，绕开员工问卷。https://hbr.org/2004/11/time-driven-activity-based-costing (evidence: [T01-S035, T01-S036])
  - 📖 **The Balanced Scorecard: Measures That Drive Performance（Kaplan & Norton, HBR 1992）** — 明确把财务指标降格为四个维度之一（财务 / 客户 / 内部流程 / 学习成长），是「不要只看财报」这一主张的学术源头。https://hbr.org/1992/01/the-balanced-scorecard-measures-that-drive-performance-2 (evidence: [T01-S037])
- **争议 / 非主流立场**：
  1. **他是自己方法最著名的批评者**：2004 年那篇 HBR 直接承认 ABC 在规模化实施中「常被放弃」，理由是无法捕捉运营复杂性、实施太慢、建设和维护太贵。这在管理学文献里罕见——**一个框架的作者自己写下它的失败率**。(evidence: [T01-S035])
  2. **对小企业的适用性质疑**：ABC/TDABC 假设你有能力刻画作业和产能成本率；中小企业往往连准确的工时和产能基线都没有，强行实施就是把猜测装进精密外壳。业内对此的替代主张是先用**贡献毛利 + 客户分层**这类粗颗粒工具。本条为本 track 判断。
  3. **平衡计分卡的反噬**：BSC 被广泛批评为在实践中退化为「指标堆砌 + KPI 考核工具」，与其原意（讲清战略因果链）背道而驰。矛盾保留。
- **最近 12 个月动态**：⚠️ **未检索到近 12 个月的新公开发声**；HBS 官方教师页显示其为 emeritus + senior fellow 状态，著作列表持续维护。(evidence: [T01-S033])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典把 Cooper & Kaplan 1988 与 Kaplan & Anderson 2004 同时列为奠基论文；② HBS 官方教师页与讲席教授职位；③ HBR 三次以头条发表其框架，跨 16 年。(evidence: [T01-S033, T01-S034, T01-S035, T01-S037])
- **核心思想关键词**：作业成本法 ABC / 时间驱动 TDABC / 产能成本率 / 成本失真的方向可预测 / 平衡计分卡
- **sub_skill_candidate**: `false` — 学术输出为主，缺少面向创始人的长访谈；但「成本分摊如何骗你」必须进 Phase 2 心智模型。
- **可信度自评**: medium-high — 文献一手且可验证，缺「近 12 个月 active」。

---

### 8. Karen Berman & Joe Knight（凯伦·伯曼 与 乔·奈特）

- **核心一句话**：**财报里的每一个数字都是一次估计的结果**——利润是估计出来的，现金是数出来的；管理者的「财务素养」不是会算，是知道哪个数字是判断、判断的人是谁、他为什么这么判断。(evidence: [T01-S039, T01-S038])
- **身份与阵营**：**财务素养普及派**。二人共同创办 Business Literacy Institute（洛杉矶），为 American Express、P&G、GM 等大企业做管理者财务培训；Karen Berman 为创始人，**已于 2013 年去世（享年 51 岁）**；Joe Knight 为前 CFO、现任机构主要输出者，与 Harvard Business Review Press 保持近二十年的合作出版关系。(evidence: [T01-S038, T01-S046])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **《Financial Intelligence: A Manager's Guide to Knowing What the Numbers Really Mean》修订版（HBR Press）** — 这本书的写作动机本身就是判断：他们找不到一本能推荐给财富 500 强培训学员的书，因为现有的书「不是按我们培训的方式写的」。https://store.hbr.org/product/financial-intelligence-revised-edition-a-manager-s-guide-to-knowing-what-the-numbers-really-mean/10833 (evidence: [T01-S039, T01-S038])
  - 📖 **《Financial Intelligence for Entrepreneurs》** — 同一框架的创业者版本，把重心从「读懂公司报表」移到「用报表管住自己的现金」。(evidence: [T01-S047])
  - 🎬 **Business Literacy Institute 官方课程与工具页** — 机构自有的培训体系、财务素养测评与配套图表工具，是判断其方法边界的一手材料。https://www.business-literacy.com/ (evidence: [T01-S040])
- **争议 / 非主流立场**：
  1. **「利润是估计」这一表述本身有争议**：准则合规派认为这话被普及化之后，容易被读成「财报不可信、可以随便调」，而实际上准则对判断空间有明确约束。两边争的是**科普的代价**。本条为本 track 归纳。
  2. **企业培训背景带来的取向偏差**：其框架是为大企业中层管理者设计的（看懂上级发下来的报表），对创始人真正的痛点——现金什么时候断、要不要接这单、要不要融资——覆盖较浅。这是把它当作「入门第一本」而非「唯一一本」的理由。
  3. 与 Profit First / Simple Numbers 这类**行为规则派**的分歧：Berman & Knight 主张提高理解力，Michalowicz 主张绕开理解力直接改行为。见本文 §5。
- **最近 12 个月动态**：⚠️ **未检索到近 12 个月的新公开动态**；Business Literacy Institute 官方站持续运营培训与在线课程，与 HBR Press 的出版关系仍在页面上标注。(evidence: [T01-S040, T01-S038])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典把《Financial Intelligence》列为入门第一本；② Harvard Business Review Press 官方书页（出版社背书，且被列入「史上百大商业书」类榜单）；③ Inc. 杂志对 Karen Berman 的独立人物报道。(evidence: [T01-S039, T01-S038, T01-S046])
- **核心思想关键词**：财务素养是可学技能 / 利润是估计现金是事实 / 数字背后的判断者 / 开卷管理（open-book management）
- **sub_skill_candidate**: `false` — 定位是入门桥梁，思想密度不足以独立成 sub-skill，但适合作为 SKILL.md 的「术语翻译层」。
- **可信度自评**: medium — 书与机构证据充分，长音视频材料稀薄，Karen Berman 已故。

---

---

## 5. 中小企业现金实操派

### 9. Greg Crabtree（格雷格·克拉布特里）

- **核心一句话**：**老板先给自己发一份市场行情的工资，剩下的才配叫利润**；而在人力密集型业务里，唯一真正的杠杆是「每付出 1 元工资，产生多少毛利」——他称之为劳动效率比（Labor Efficiency Ratio, LER）。(evidence: [T01-S048, T01-S049])
- **身份与阵营**：**中小企业现金实操派**。执业 CPA，长期服务 100 万–5000 万美元营收区间的私营企业主；《Simple Numbers, Straight Talk, Big Profits!》与《Simple Numbers 2.0》作者。(evidence: [T01-S048, T01-S051])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **《Simple Numbers, Straight Talk, Big Profits!》与官方站的 LER 工具** — 核心是四把钥匙：给老板发真实工资、把利润目标定在税前 10-15%、按 LER 管人力、用「资本上限」控制增长速度。https://simplenumbers.me/ (evidence: [T01-S048, T01-S051])
  - 🎙️ **Brand Builders Group #591（2025-05）长访谈** — 专讲两个指标：劳动效率比与贡献毛利，是理解其体系最直接的音频材料。https://brandbuildersgroup.com/podcast/ep-591-simplifying-financial-success-for-entrepreneurs-greg-crabtree/ (evidence: [T01-S049])
  - 🎙️ **Ten Golden Rules #116（2026-06）长访谈** — 讲「为什么 LER 2:1 是生死线」——即每 1 元直接人工要产生 2 元毛利。⚠️ **该 2:1 阈值是他本人的经验值，非行业普遍基准，跨行业照搬会失效**。https://www.tengoldenrules.com/captivate-podcast/ep116-strategies-from-greg-crabtrees-fantastic-book-simple-numbers-for-big-profits/ (evidence: [T01-S050])
- **争议 / 非主流立场**：
  1. **「老板工资」这条最招反对**：会计准则不要求业主薪酬按市价计提，税务筹划上很多小企业刻意压低工资走分红。Crabtree 主张先按市价计提再看利润——支持者说这才看得出真实盈利能力，反对者说这与实际税务和现金安排脱节，制造了一套「只在他体系内成立」的利润。(evidence: [T01-S048, T01-S051])
  2. **单一比率的普适性存疑**：LER 2:1、税前利润 10-15% 这类阈值在服务业与制造业、软件与工程之间差异巨大，执业会计师的复盘文章也提示需按行业重设基准。(evidence: [T01-S051])
  3. **与 Profit First 的分野**：两者都面向小企业主、都主张「先定利润」，但 Crabtree 走的是**改口径 + 定基准**（还是在会计框架内），Michalowicz 走的是**改行为 + 多账户**（绕开会计框架）。这是本行业最具体的一组方法论对立。(evidence: [T01-S048, T01-S053])
- **最近 12 个月动态**：2026-06 在 Ten Golden Rules 播客做长访谈讲 LER；持续作为 The Great Game of Business（开卷管理阵营）的常驻嘉宾。(evidence: [T01-S050, T01-S052])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典独立收录《Simple Numbers》；② 加拿大执业事务所 Avalon Accounting 公开复盘其四把钥匙的落地效果（同业采用）；③ The Great Game of Business 长期邀其录节目。(evidence: [T01-S051, T01-S052, T01-S048])
- **核心思想关键词**：劳动效率比 LER / 老板市价工资 / 贡献毛利 / 资本上限与增长速度 / 税前利润基准线
- **sub_skill_candidate**: `true` — 与用户场景（中小企业主/创始人）对齐度最高，有可执行的口径与阈值体系，且近 12 个月持续有长访谈输出。
- **可信度自评**: high（对齐度与 active 性强）；其阈值的普适性单独标 medium。

---

### 10. Mike Michalowicz（麦克·米哈洛维奇）—— ⚠️ 争议人物

- **核心一句话**：把恒等式从「收入 − 费用 = 利润」改写成「**收入 − 利润 = 费用**」——先把利润转走到看不见的账户，剩下的钱才是你能花的；这是一条**行为规则**，不是会计规则。(evidence: [T01-S053, T01-S054])
- **身份与阵营**：**中小企业现金实操派 / 行为派**。连续创业者与畅销书作者（Penguin Random House 出版九本商业书），Profit First Professionals 认证体系联合创始人——把会计师、记账师、商业教练发展为该方法的持证服务商。(evidence: [T01-S055, T01-S058])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **《Profit First》（修订版 2017）与官方站的分账户测算器** — 核心机制是把一个银行账户拆成收入 / 利润 / 老板工资 / 税金 / 运营费用等多个账户，按固定比例分配，用「看不见就花不掉」的行为约束替代自律。https://profitfirstbook.com/ (evidence: [T01-S053])
  - 🎬 **Profit First Professionals 官方认证体系页** — 要判断这套方法的真实性质，看它怎么被商业化比看书更有效：它本质上是一套**面向会计从业者的加盟/认证生意**。https://profitfirstprofessionals.com/ (evidence: [T01-S055])
  - 📖 **两篇来自执业会计师的系统性批评**（见下）——建议与原书对读，否则你只会听到一面。(evidence: [T01-S056, T01-S057])
- **争议 / 非主流立场**（本条是本 track 内容最重的一栏）：
  1. **「把利润定义成银行存款」被指为根本性错误**：批评者指出，如果你有贷款、买固定资产、做股东分配，这些都消耗现金但**不进利润表**；把「账上剩的钱」叫利润，会在有负债或重资产时给出系统性错误的信号。有会计师直接称其为「对 GAAP 不负责任的拆解」。(evidence: [T01-S056])
  2. **把 GAAP 简化成「销售 − 费用 = 利润」是稻草人**：这是原书用来对比的靶子，而权责发生制（accrual，收入费用按发生期间而非收付现金记账）的实际内容远比这复杂——批评者认为这种简化本身就误导读者。(evidence: [T01-S056])
  3. **多账户带来真实的运营成本**：对账工作量成倍增加，记账费用上升；有记账事务所公开写「为什么我不推荐 Profit First」，理由包括对账负担、比例设定缺乏依据、以及它回避而不是解决「这门生意为什么不赚钱」。(evidence: [T01-S057])
  4. **他对会计专业本身的态度**：他公开质疑与记账师合作的价值（理由是记账师也可能误读财务信息），这进一步加剧了与专业群体的对立。(evidence: [T01-S056])
  5. **公允地说他对了什么**：对于**无负债、轻资产、老板即操盘手**的微型服务企业，这套「先付自己」的行为规则确实解决了小企业主最真实的失败模式——钱进账就花掉。把它当**现金纪律工具**而不是**财务判断工具**，是本 track 的建议用法。
- **最近 12 个月动态**：2026 年推出新书《The Money Habit》，把 Profit First 原则迁移到个人理财，同时它是他与 Page Two Books 合作的新出版厂牌 Simplified 的首本书——**注意：个人理财方向明确在本 skill 范围之外**。(evidence: [T01-S054, T01-S058])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典把《Profit First》与其批评一并收录；② Penguin Random House 长期出版关系（九本书）；③ 存在独立的持证服务商网络（Profit First Professionals），说明方法已被第三方从业者采用——**注意：认证网络是他自己运营的，不构成独立背书**，独立背书来自 ①②与两篇批评文章的存在本身。(evidence: [T01-S058, T01-S055, T01-S056, T01-S057])
- **核心思想关键词**：收入 − 利润 = 费用 / 先付自己 / 多账户行为约束 / 帕金森定律应用 / 现金纪律 ≠ 财务判断
- **sub_skill_candidate**: `false` — 方法单一且争议大；建议在 SKILL.md 中作为「现金纪律工具 + 明确的适用边界与批评」一并出现，不独立成 sub-skill。
- **可信度自评**: medium — 一手材料充足、影响力真实，但其核心概念在专业上被系统性质疑，必须成对呈现。

---

---

## 6. 创业融资与条款派

### 11. Brad Feld & Jason Mendelson（布拉德·菲尔德 与 杰森·门德尔松）

- **核心一句话**：**每一张 term sheet 都是两场谈判叠在一起——经济条款和控制权条款**；创始人的典型错误是死盯估值（经济），把董事会构成、保护性条款、清算优先权（控制）当作法务细节让掉。(evidence: [T01-S059, T01-S061])
- **身份与阵营**：**创业融资与条款派**。Feld 为 Foundry Group / Techstars 联合创始人，个人博客持续更新 20 余年；Mendelson 为律师出身的 VC，两人合著《Venture Deals》（Wiley，第 4 版 2019）。(evidence: [T01-S060, T01-S063, T01-S062])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **Term Sheet 系列博客全归档（本书原型）** — 逐条拆条款的连载，比书更早也更口语；书本身就是从这个连载长出来的。https://feld.com/archives/category/term-sheet/ (evidence: [T01-S061, T01-S060])
  - 📖 **《Venture Deals》第 4 版** — 覆盖 term sheet 全条款、VC 基金自身的经济结构（为什么 GP 会那样谈）、以及谈判中的常见陷阱。https://www.wiley.com/en-us/Venture+Deals:+Be+Smarter+Than+Your+Lawyer+and+Venture+Capitalist,+4th+Edition-p-9781119594840 (evidence: [T01-S062])
  - 🎬 **Venture Deals 官方站与配套免费在线课** — 官方站汇总了书的更新、免费课程与条款示例。https://www.venturedeals.com/ (evidence: [T01-S059])
- **争议 / 非主流立场**：
  1. **「把 VC 的账本摊开给创始人看」在行业内曾被视为背叛**：书中详解 GP/LP 结构、管理费与 carry 如何影响 VC 的谈判行为，这类信息此前主要靠圈内口耳相传。(evidence: [T01-S062, T01-S059])
  2. **视角仍然是美国 + 机构 VC**：条款体系、法律预设（特拉华州公司法）、以及「一定会有下一轮」的隐含假设，对中国境内的中小企业与非 VC 路径创业者适用性有限。本条为本 track 的适用边界判断。
  3. **与「报告估值」的张力**：Track 04 已收录的 Gornall & Strebulaev 研究显示，独角兽的报告估值平均虚高约 48%，主因正是清算优先权等下行保护条款——这从实证侧证明了本书「别只看估值」的核心主张，同时也说明**媒体口径的估值数字本身不可直接用**。(evidence: [T01-S062])
- **最近 12 个月动态**：⚠️ **未检索到第 5 版出版或近 12 个月的联合公开发声**。Feld 个人博客仍在持续更新，Venture Deals 官方站与配套课程仍在运营。(evidence: [T01-S060, T01-S059])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典独立收录并列为融资条款的唯一必读；② Wiley 官方书页与第 4 版发行；③ 被 O'Reilly 等技术教育平台收录进课程库（第三方机构采用）。(evidence: [T01-S062, T01-S059], [T01-S061])
- **核心思想关键词**：经济条款 vs 控制条款 / 清算优先权 / 董事会构成 / 保护性条款 / 期权池洗牌（option pool shuffle）
- **sub_skill_candidate**: `true`（合并为一个「融资条款」sub-skill）—— 条款体系可执行、边界清晰，且与用户场景中「融资结构与股权稀释」直接对应。
- **可信度自评**: medium-high — 著作与官方站证据充分，扣分项是近 12 个月无新动态。

---

---

## 7. 创业与 SaaS 单位经济派

### 12. David Skok（大卫·斯科克）

- **核心一句话**：**订阅制生意增长越快，现金越紧**——获客成本一次性付出、收入按月回收，于是每多签一个好客户，短期现金流反而更差；这条「现金流低谷」是订阅制创始人最常低估的结构性事实。(evidence: [T01-S065, T01-S064])
- **身份与阵营**：**创业与 SaaS 单位经济派**的奠基者。四次创业后转做 VC（Matrix Partners），以 forEntrepreneurs 博客把 SaaS 指标体系写成行业默认语言。(evidence: [T01-S064, T01-S066])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **SaaS Metrics 2.0** — 单位经济学的行业奠基长文：LTV/CAC、CAC 回收期、流失与净留存、以及「先证明单位经济成立，再踩增长油门」的顺序。https://www.forentrepreneurs.com/saas-metrics-2/ (evidence: [T01-S064])
  - 📖 **SaaS 现金流低谷（SaaS Economics 系列）** — 用现金流曲线解释为什么好生意也会缺钱，以及月付 vs 年付如何改变这条曲线。https://www.forentrepreneurs.com/saas-economics-1/ (evidence: [T01-S065])
  - 🎙️ **Intercom 播客长访谈：该盯哪些指标** — 他在访谈里强调**不同增长阶段该盯不同指标**，这是他区别于「指标清单党」的关键。https://www.intercom.com/blog/podcasts/david-skok-on-the-metrics-every-saas-company-should-be-tracking/ (evidence: [T01-S066, T01-S068])
- **争议 / 非主流立场**：
  1. **LTV/CAC ≥ 3 与回收期 < 12 个月这类阈值被过度神化**：这些是他给出的经验参考，后来被整个行业当成硬指标；批评（含 Sacks 提出 burn multiple 的动机）指出，LTV 依赖对流失率的长期外推，在早期公司数据量下几乎不可靠。(evidence: [T01-S064, T01-S069])
  2. **面向 VC 支持的高增长订阅公司**：其框架默认有外部资本可用、可以先亏后赚。对不融资的中小企业，直接搬 LTV/CAC 会把「本可以慢慢赚钱」的生意逼成烧钱生意。本条为本 track 判断。
  3. **口径战争**：LTV 该用毛利还是收入、CAC 是否含销售人员全成本——至今没有统一答案，这正是 Ben Murray、Benchmarkit 一类「口径标准化」工作存在的原因。(evidence: [T01-S095, T01-S096])
- **最近 12 个月动态**：⚠️ **未检索到近 12 个月的新公开发声或新文章**；forEntrepreneurs 站点内容仍在线并被广泛引用，但更新节奏明显放缓。(evidence: [T01-S064, T01-S065])
- **endorsement 证据（≥ 2 独立来源）**：① Track 04 正典把 SaaS Metrics 2.0 与现金流低谷两篇同时列为奠基研究；② Intercom、SaaStr、ChartMogul 三家互不隶属的机构分别邀其做长访谈或大会演讲。(evidence: [T01-S064, T01-S066, T01-S067, T01-S068])
- **核心思想关键词**：现金流低谷 / LTV/CAC / CAC 回收期 / 净收入留存 / 先证明单位经济再增长
- **sub_skill_candidate**: `false` — 内容极其重要但输出已趋停滞，且已被后续从业者（Sacks / Murray / Benchmarkit）细化；建议作为 Phase 2 的基础层素材。
- **可信度自评**: medium-high — 文本一手且影响力可验证，扣分项是近 12 个月无动态。

---

### 13. David Sacks（大卫·萨克斯）

- **核心一句话**：**用一个数字就能判断烧钱是否值得——净烧钱 ÷ 净新增 ARR**；它不需要预测未来（不像 LTV），也不惩罚沉没成本（不像 hype ratio 用累计融资额做分母），你砍完成本下个季度就能改善。(evidence: [T01-S069, T01-S071])
- **身份与阵营**：**创业与 SaaS 单位经济派 / 运营者派**。PayPal 早期高管、Yammer 创始人，Craft Ventures 联合创始人（与 Bill Lee）；2024-12 获任白宫「AI 与加密沙皇」，2026-03 因特别政府雇员 130 天上限届满卸任，转任总统科技顾问委员会（PCAST）联席主席。(evidence: [T01-S073, T01-S074])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **The Burn Multiple（2020-04-23 首发）** — 提出该指标的原文，含分档参考（业内广泛引用的分档为：< 1 极佳、1-1.5 很好、1.5-2 尚可、> 3 需警惕；⚠️ **该分档为其个人经验建议，非统计基准**）。https://www.craftventures.com/articles/the-burn-multiple (evidence: [T01-S069, T01-S071])
  - 📖 **把 burn multiple 用于平台型（marketplace）业务** — Craft Ventures 官方站的延伸文章，说明该指标如何跨业务模式迁移。https://www.craftventures.com/articles/applying-the-burn-multiple-to-marketplace-business-models (evidence: [T01-S070])
  - 🎙️ **20VC 长访谈：如何准确评估 CAC、烧钱与流失，以及好董事会长什么样** — 他谈财务判断最系统的一次长对谈。https://www.thetwentyminutevc.com/davidsacks (evidence: [T01-S072])
- **争议 / 非主流立场**：
  1. **burn multiple 隐含「ARR 增长是唯一有价值的产出」**：对非订阅制、硬件、平台早期、或刻意做慢的公司，这个分母根本不成立；把它当通用效率指标会误伤。本条为本 track 判断，与其原文限定为 SaaS 语境并不矛盾。(evidence: [T01-S069])
  2. **与 Skok 体系的正面替代关系**：他明确把 burn multiple 定位为**不依赖预测**的替代品，这等于指出 LTV/CAC 的软肋是外推假设。两套体系的支持者至今在「早期公司该看哪个」上没有共识。(evidence: [T01-S069, T01-S064])
  3. **政治身份带来的信息噪音**：2025 年起他的公开发声大量与 AI/加密政策绑定，可用的**财务方法论**新材料随之稀释；同时他兼任政府职务与 VC 合伙人期间的利益冲突问题在公开报道中被反复讨论。引用其近期言论时需区分「投资人身份」与「政策身份」。(evidence: [T01-S073, T01-S074])
- **最近 12 个月动态**：2026-03-26 宣布卸任白宫 AI 与加密沙皇（特别政府雇员 130 天用尽），转任 PCAST 联席主席；同期 Craft Ventures 在奥斯汀设立新办公室。(evidence: [T01-S073, T01-S074])
- **endorsement 证据（≥ 2 独立来源）**：① Track 05 把 Craft Ventures 文章列为 burn multiple 的原始出处；② burn multiple 已被 Drivetrain、Cube、Wall Street Prep 等多家互不隶属的工具与培训机构写进标准指标词条（方法被行业采纳）；③ 20VC 等第三方播客长访谈。(evidence: [T01-S069, T01-S071, T01-S072])
- **核心思想关键词**：burn multiple / 资本效率 / 不预测的指标 / 沉没成本无关性 / 增长质量
- **sub_skill_candidate**: `false` — 核心贡献是一个指标而非一套体系；且近期公开身份已偏离财务领域。
- **可信度自评**: medium-high

---

### 14. CJ Gustafson

- **核心一句话**：**CFO 的活儿是把「今年到底要做成什么」翻译成一份所有人都签字的数字计划**——年度预算不是财务部门的表格作业，是一场为期三个月、CEO 必须共同主导的协商过程。(evidence: [T01-S075, T01-S076])
- **身份与阵营**：**创业与 SaaS 单位经济派 / 在职实操派**。科技公司 CFO 出身（公开资料显示曾任汽配采购平台 PartsTech 的 CFO），运营 Mostly Metrics newsletter（据其自述与第三方报道，订阅规模在 6 万量级）与 Run the Numbers 播客（每周两更）。⚠️ 据 2026 年公开报道，他已转为**全职内容创作者**（两份 newsletter + 播客），在职 CFO 身份可能已变化，引用时需注明时点。(evidence: [T01-S077, T01-S078, T01-S076])
- **值得读 / 听 / 看的 3 件事**：
  - 📖 **Mostly Metrics 年度规划系列** — 他把年度预算拆成三个月的时间线与阶段性交付物，是本 track 里最贴近「创始人下周就要做的事」的材料。https://www.mostlymetrics.com/ (evidence: [T01-S075, T01-S076])
  - 🎙️ **Run the Numbers（每周两更长访谈）** — 覆盖 SaaS 指标、年度预算、人头规划、股权与稀释、融资与卖公司；嘉宾多为在职财务负责人，是本行业「同业讨论语域」的最佳采样地。https://cjgustafson.substack.com/s/run-the-numbers (evidence: [T01-S076])
  - 🎙️ **Growth In Reverse 长访谈：newsletter 是怎么做起来的** — 用来判断其内容的商业模式与潜在偏差（谁在赞助、写什么会被激励多写）。https://podcast.growthinreverse.com/episodes/cj-gustafson (evidence: [T01-S077])
- **争议 / 非主流立场**：
  1. **赞助驱动的结构性偏差**：他的内容与整个 CFO newsletter 生态高度依赖财务软件厂商赞助（Ramp 等）。Track 05 已独立观察到「财务内容源大多由财务软件厂商出资运营」这一模式——**厂商赞助会让讨论向「买软件能解决的问题」倾斜**。这不是指控，是使用其内容时必须带上的折扣。(evidence: [T01-S078], [T01-S075])
  2. **样本偏向 VC 支持的 B2B 软件公司**：他讨论的预算、人头、稀释问题默认公司有机构投资人与董事会；对自筹资金的中小企业，流程可以大幅简化。
  3. **「在职 CFO」的身份可信度是他最大的资产，也是最容易过期的部分**：一旦转为全职创作者，其内容从「我在做」变成「我在报道」，权重应下调。本条为本 track 判断。
- **最近 12 个月动态**：持续每周两更 Run the Numbers 播客与 Mostly Metrics newsletter；据搜索结果，已扩展出第二份 newsletter（Looking For Leverage）并转向全职创作。(evidence: [T01-S076, T01-S077])
- **endorsement 证据（≥ 2 独立来源）**：① Track 05 把 Mostly Metrics 列为 newsletter 维度的第一位；② OnlyCFO 在其公开推荐列表中点名（同业互推）；③ Ramp 为其设立第三方作者页。(evidence: [T01-S075, T01-S078], [T01-S100])
- **核心思想关键词**：年度规划三个月时间线 / 人头即预算 / 指标口径的政治性 / 稀释与期权池 / CFO 是翻译官
- **sub_skill_candidate**: `true` — 是全 track 中唯一同时具备「在职视角 + 高频长音频 + 面向创始人」三项的人；材料量足以支撑独立蒸馏。
- **可信度自评**: medium-high — 输出频率与第三方背书强；扣分项是身份可能已从在职 CFO 变化，且商业模式带来赞助偏差。

---

---

## 8. 中文圈

### 15. 肖星（清华大学）

- **核心一句话**：**三张表各回答一个不同的问题**——利润表看赚钱能力，资产负债表看家底与结构，现金流量表看能不能活下去；财务思维的本质是把商业模式、战略与经营管理串成一条能用数字追踪的链条。(evidence: [T01-S079, T01-S103])
- **身份与阵营**：**中文圈财务素养普及派（学院派）**。清华大学经济管理学院会计系教授、长聘教授（2014-12 起）；研究领域为新制度会计与公司治理、会计与资本市场、财务报表分析、私募股权投资；同时在全国会计专业学位研究生教育指导委员会有学术任职。(evidence: [T01-S079, T01-S101])
- **值得读 / 听 / 看的 3 件事**：
  - 🎬 **《财务分析与决策》MOOC（学堂在线 / 清华，国家精品在线课程、国家级一流本科课程）** — 中文圈财报入门的事实标准公开课，完整、免费、可回看。https://www.xuetangx.com/course/THU08091000367 (evidence: [T01-S081, T01-S079])
  - 📖 **《一本书读懂财报》（浙江大学出版社 2014；2019 年第二版）** — MOOC 的配套书，是「三张表各看什么」这一框架最普及的中文载体。https://book.douban.com/subject/34810876/ (evidence: [T01-S082, T01-S079])
  - 📖 **《肖星的财务思维课》（机械工业出版社 2020）** — 从「读懂报表」进一步走到「用财务视角做经营判断」，更贴近创始人语境。https://book.douban.com/subject/35033236/ (evidence: [T01-S104, T01-S079])
- **争议 / 非主流立场**：
  1. **她的立场本身温和，真正的分歧在方法论定位**：以上市公司报表与资本市场研究为底座的框架，落到没有审计、没有规范权责发生制记账的中小企业时会失效——很多小企业连一张可信的资产负债表都没有。这是本 track 认定的**最重要适用边界**，非她本人主张。
  2. **与张新民框架的差异**：肖星走的是「准则 + 报表结构 + 财务比率」的标准路径并强调普及性；张新民主张跳出比率分析、按战略与资产质量重构报表结构（见下条）。两人都在中文教材体系内部，分歧属**同一学科内的框架之争**，不是对立阵营。(evidence: [T01-S083], [T01-S079])
  3. **未检索到她对国际准则争议（如 IFRS 18 / 非 GAAP 指标）的公开立场**——中文学者在这类争议上的公开表态本身就稀少，这是中文一手材料的结构性缺口。
- **最近 12 个月动态**：⚠️ **未检索到 2025-09 至 2026-09 的公开动态**。可确认的最近公开活动为 2023-11-25 清华校友学习日第 49 讲「从财务视角看科创企业价值创造」；MOOC 在学堂在线按学期滚动开课。(evidence: [T01-S102, T01-S081])
- **endorsement 证据（≥ 2 独立来源）**：① 清华经管学院官方教师页与长聘教授职位；② 清华大学校级新百年教学成就奖官方报道（校级评选，非自营销）；③ 全国会计专业学位研究生教育指导委员会（教育部体系机构）官方页；④ Track 04 与 Track 05 分别把她列为中文圈必读作者与中文一手源。(evidence: [T01-S079, T01-S080, T01-S101])
- **核心思想关键词**：三张表分工 / 财务思维是黏合剂 / 商业模式→战略→经营的数字链 / 价值创造
- **sub_skill_candidate**: `false` — 材料以课程与入门书为主，缺少长访谈与观点性输出；建议作为 SKILL.md 中文术语与入门路径的引用源。
- **可信度自评**: medium — 身份与著作证据是 `.edu.cn` 一手且非常扎实，扣分项是近 12 个月无公开动态、且无长访谈材料。

---

### 16. 张新民（对外经济贸易大学）

- **核心一句话**：**同样的数字，质量可以完全不同**——不要停在比率分析，要先按战略视角重构报表结构：资产负债表左边是扩张能力、右边是四大扩张动力（金融性负债、经营性负债、股东入资、利润积累），然后再问这家公司到底靠什么创造价值。(evidence: [T01-S083, T01-S086])
- **身份与阵营**：**中文圈管理会计决策派 / 战略视角财报分析**。对外经济贸易大学会计学教授，曾任国际商学院院长、副校长；财政部会计名家；国务院学位委员会工商管理学科评议组成员；主编《财务报表分析》教材获**首届国家教材建设一等奖**。(evidence: [T01-S086, T01-S083])
- **值得读 / 听 / 看的 3 件事**：
  - 🎬 **《财务报表分析》国家级慕课（中国大学 MOOC / 对外经贸大学）** — 作者亲授的完整课程，是其框架最系统的免费材料。https://www.icourse163.org/course/UIBE-1003252013 (evidence: [T01-S084])
  - 📖 **《财务报表分析》第 6 版（中国人民大学出版社）** — 教材本体，「战略视角财报分析框架」的完整版。https://book.douban.com/subject/36285053/ (evidence: [T01-S087])
  - 🎬 **中央财经大学会计学院讲座「财报信息与企业价值贡献能力」（2024-04-02）** — 他在这场讲座里给出「三支柱两搅局」的营业利润来源拆解，以及把企业价值贡献分成**价值创造能力**与**价值整合能力**两类的判断框架。https://soa.cufe.edu.cn/info/1025/6867.htm (evidence: [T01-S086])
- **争议 / 非主流立场**：
  1. **明确反对以比率分析为中心的传统教法**：他主张先按战略重构报表结构再算比率，否则比率是没有语境的数字。这与国内大量以「偿债能力/营运能力/盈利能力」三段式比率为骨架的教材直接冲突。(evidence: [T01-S083], [T01-S086])
  2. **「资产质量」这一概念本身有争议**：他强调同样金额的资产在不同企业里价值完全不同（应收账款、存货、商誉、其他应收款的可回收性差异），主张对报表数字做质量判断。批评角度是这类判断依赖分析者的主观经验，**难以标准化、难以复核**——这与准则合规派追求可比性的取向相反。本条为本 track 归纳，非引自单一来源。
  3. **框架的自称程度需要谨慎对待**：公开材料中出现「张氏财务分析框架」「基本解决了中国企业财务报表分析的理论与方法问题」这类表述，**多来自宣传性通稿而非学术共识**，本 track 不采信其效力判断，只采信框架内容本身。
- **最近 12 个月动态**：⚠️ **未检索到 2025-09 至 2026-09 的公开动态**。可确认的近期活动为 2024-04-02 中央财经大学会计学院讲座、以及在东北财经大学「知名会计学者论坛」的专场；MOOC 在中国大学 MOOC 按学期滚动开课。(evidence: [T01-S086, T01-S105], [T01-S084])
- **endorsement 证据（≥ 2 独立来源）**：① 对外经贸大学科研处官方通稿与国际商学院官方站；② 中央财经大学、东北财经大学、西南大学三所互不隶属高校的官方讲座记录（同行邀约）；③ 教材获首届国家教材建设一等奖（国家级评审）；④ Track 04 与 Track 05 独立收录。(evidence: [T01-S083, T01-S086, T01-S105, T01-S085])
- **核心思想关键词**：战略视角财报分析 / 资产质量 / 三支柱两搅局 / 价值创造能力 vs 价值整合能力 / 扩张的四大动力
- **sub_skill_candidate**: `false` — 框架价值高，但公开材料以课程与讲座通稿为主，缺少深度长访谈；建议作为 SKILL.md 中「中文语境下的报表结构判断」引用源。
- **可信度自评**: medium — `.edu.cn` 一手证据充分，扣分项是近 12 个月无动态、且部分表述来自宣传通稿需降权。

---

---

## 9. 隐性 figure 池（准则与协会侧的规则制定者）

> **为什么单列**：这些人/角色对「你的报表长什么样」的实际影响力，远大于任何一位畅销书作者——他们改一条准则，全世界的 EBITDA、资产负债率、利润表结构就变一次。但他们**个人一手材料极少**（没有博客、没有播客、少有长访谈），因此本节一律用**机构官方页作 surrogate**，并明确标注这是从机构文件推断的角色影响力，**不是直接听到本人发声**。

### 9.1 IASB 主席与理事会（国际财务报告准则）

- **当前状态（重要且刚变）**：Andreas Barckow 的五年 IASB 主席任期于 **2026-06 结束**；**Sam Woods 获任新主席，五年任期自 2026-10-01 起**；空档期由副主席 Linda Mezon-Hutter 代理。Steven Maijoor 将自 **2027-01-01** 起任 IFRS 基金会受托人主席。(evidence: [T01-S088, T01-S089])
- **为什么这次人事值得创始人留意**：Sam Woods 来自**金融监管**（英国审慎监管局 PRA 首席执行官、英格兰银行副行长），不是会计准则出身。一位监管背景的主席上任，与 IFRS 18（2027-01-01 生效、强制披露「管理层自定义业绩指标」）的落地期重叠——这提示未来五年的方向可能更偏**披露纪律与可比性**，而非放宽判断空间。⚠️ **本条是本 track 的推断，不是 IFRS 基金会的官方表述。** (evidence: [T01-S088, T01-S108])
- **surrogate 入口**：IASB 现任理事名单 https://www.ifrs.org/groups/international-accounting-standards-board/ (evidence: [T01-S090])

### 9.2 FASB 主席与理事会（美国 GAAP）

- **当前状态**：Richard R. Jones 任 FASB 主席，任期至 **2027-06-30**；副主席 Hillary H. Salo 已获任下一任主席，七年任期自 2027-07-01 起。2026-01-01 起有三名新理事就任。(evidence: [T01-S091])
- **对创始人的意义**：如果你的公司要面向美国投资人或计划美股路径，FASB 的 ASU（准则更新）生效日期表就是你的会计政策日历；Track 05 已记录多条 ASU 在 2026-12-31 年结生效。
- **surrogate 入口**：https://www.fasb.org/about-us/board-members/richard-r-jones（403 为反爬，非死链） (evidence: [T01-S091])

### 9.3 中国财政部会计司

- **角色**：中国企业会计准则（CAS）的实际制定、解释与实施指导机关。与 IASB/FASB 不同，它**没有可识别的「明星理事」个人**，一手材料完全以司级公告形式出现——这是中文语境下 figure 稀薄的结构性原因，而不是「中国没有人在定规则」。(evidence: [T01-S092])
- **近 12 个月动态（本节唯一有明确近期动态的机构）**：2026-06-18 发布《企业会计准则实施问答和应用案例（2026 年第二批）》，指导包括《企业会计准则解释第 19 号》在内的实施口径；准则解释目录已更新至第 20 号。(evidence: [T01-S106, T01-S107])
- **⚠️ 诚实标注**：本 track **未采信任何未经 `.gov.cn` 官方页确认的司局领导姓名**。搜索结果中出现的人名无法在财政部官方页上直接核对，故不写入。
- **surrogate 入口**：会计司主页 https://kjs.mof.gov.cn/ (evidence: [T01-S092])

### 9.4 IMA（管理会计师协会）与 AICPA & CIMA 的知识体系

- **角色**：这两家决定了「管理会计师应该会什么」的能力框架——IMA 的 CMA 认证体系、AICPA & CIMA 的 CGMA 能力框架。对创始人而言，它们的价值不是考证，而是**一份别人替你整理好的、成体系的能力清单**（成本管理、规划与预算、绩效管理、内部控制、决策分析）。(evidence: [T01-S093, T01-S094])
- **⚠️ 诚实标注**：未能定位到这两家机构「知识体系负责人」的具体个人一手发声材料；本节完全以机构官方页作 surrogate。
- **surrogate 入口**：https://www.imaglobal.org/ ；https://www.aicpa-cima.com/resources/landing/management-accounting-cgma (evidence: [T01-S093, T01-S094])

### 9.5 Beyond Budgeting Round Table（BBRT）

- **角色**：预算这件事上唯一成体系的**反对派机构**。它主张把「目标、预测、资源分配」三件事拆开——因为把三者绑在一张预算表上，必然让预测变成谈判筹码。学术侧的对应文本是 Michael Jensen 的《Paying People to Lie》：预算与奖金挂钩等于花钱购买失真信息。(evidence: [T01-S098, T01-S099])
- **为什么进隐性池而非正式榜**：其代表人物（Jeremy Hope、Robin Fraser、Bjarte Bogsnes）的公开长材料在中文可及范围内稀薄，且 Hope 已故；机构本身比个人更可引用。
- **surrogate 入口**：https://bbrt.org/ (evidence: [T01-S098])

---

---

## 10. Borderline / 已考察但未进核心榜

> 记录判定理由，供 Phase 1.5 复议。**被刷掉不等于不重要**，多数是「重叠」或「材料形态不合」。

| 候选 | 判定 | 理由 |
|------|------|------|
| **Ben Murray**（The SaaS CFO） | BORDERLINE，未进榜 | 材料厚（own site + SaaS Metrics School 播客，单集 10 分钟讲透一个指标口径），但其核心贡献是**指标口径标准化与模板**，不是独立的思维体系；与 CJ Gustafson 覆盖高度重叠。建议留在 Track 05 的 sources 维度。(evidence: [T01-S095, T01-S096]) |
| **Jason Lemkin**（SaaStr） | 未进榜 | 影响力真实且长材料充足，但主轴是**销售与增长（GTM）**，财务内容为二级派生；与本 skill 的「内部财务判断」范围偏离。(evidence: [T01-S097]) |
| **Thomas Ittelson** | 未进榜 | 《Financial Statements》是极好的入门书（Track 04 已收录），但**几乎没有长访谈 / 演讲 / 持续输出**，不构成可蒸馏的思维方式。 |
| **Stephen Clapham**（Behind the Balance Sheet） | BORDERLINE | 取证读表的现役实践者，周更 + 课程，材料很厚；但视角是**二级市场分析师**（我怎么发现这家上市公司有问题），不是创始人的内部判断。与 Schilit 重叠。 |
| **Steve Cooper**（前 IASB 理事）+ Dennis Jullens（Footnotes Analyst） | BORDERLINE | 罕见的「准则制定者转做公开分析」组合，一手价值高；但内容面向卖方/买方分析师读附注，对创始人的日常判断距离较远。**建议作为隐性 figure 池 §9.1 的补充观察对象。** |
| **The Secret CFO / OnlyCFO**（匿名） | 需要规则裁决 → 本 track 给出规则 | **匿名 figure 的处理规则**：可作为 Track 05 的**信息源**引用，但**不进 figures 榜**。理由有三：① endorsement 无法独立验证（无法确认任职、无法确认利益关系）；② 无法核实其自述经历；③ Phase 2 蒸馏「思维方式」时，无法把观点归因到一个可追责的人。The Secret CFO 有一篇自述身份与动机的长文，可作为理解其立场偏差的材料，但仍不足以支撑 figure 卡片。(evidence: [T01-S100]) |
| **Bjarte Bogsnes / Jeremy Hope / Robin Fraser**（Beyond Budgeting） | 转入隐性池 §9.5 | 观点极其对口（预算与滚动预测是本 skill 的核心支柱之一），但个人公开长材料在本次检索中稀薄，Hope 已故；改用 BBRT 机构页 + Jensen 论文作 surrogate。(evidence: [T01-S098, T01-S099]) |
| **Jack Sweeney**（CFO Thought Leader）、**Paul Barnhurst**（The FP&A Guy）、**Jack McCullough**、**Hannah Munro**、**Wassia Kamon**、**Josh Aharonoff**、**Ray Rike**、**Jamin Ball** | 未进榜 | 均为**主持人 / 数据提供者 / 模板作者**角色，价值在于「把别人的观点带出来」或「提供基准数据」，而非自己持有一套可蒸馏的判断体系。全部保留在 Track 05。 |
| **投行 / 并购 / VC 投资人侧的知名人物** | 范围外，主动排除 | 本 skill 明确不做卖方并购执行与 VC 看项目视角。 |
| **中文财会考证名师** | 范围外，主动排除 | 内容为准则背诵与应试，与「经营判断」无关；且其一手材料多分布在营销页与被禁平台。 |

### 中文 figure 的诚实结论（必须原样进入 SKILL.md 诚实边界节）

- 本 track 只找到 **2 位**中文 figure（肖星、张新民），**两人都是学院派教授，都以课程与教材为主要输出，都未检索到近 12 个月的公开动态，且都没有 ≥ 30 分钟的深度长访谈**。
- **中文圈缺的不是学者，是「面向创业者的经营财务实操者」的公开一手材料。** Track 05 已独立得出同一结论（中文的经营判断类实务一手源为 0 条）。两个 track 独立收敛到同一结论，说明这是行业结构性事实而非检索失败。
- 造成这一缺口的直接原因之一是：中文实务内容的主要载体（个人公众号、知乎专栏、财会网校营销页）**全部在本次调研的黑名单内**——不是因为内容一定错，而是因为**无法验证作者身份与利益关系**。本 track 宁可留白，不用无法追溯的材料凑数。

---

## Phase 2 提炼提示

### A. 反复出现 ≥ 3 位 figures 的关键词（候选行业心智模型）

| # | 候选心智模型 | 出现于 | 证据 |
|---|------------|-------|------|
| 1 | **报告利润 ≠ 可支配现金**：利润是估计出来的，现金是数出来的；折旧是真实费用，只是先花掉了 | Buffett/Munger、Berman & Knight、肖星、Crabtree、Michalowicz、Skok | evidence: [T01-S021, T01-S039, T01-S079, T01-S048, T01-S065] |
| 2 | **口径决定结论**：ROIC、成本、LTV/CAC、资产质量——同一家公司换个口径可以从赚钱变亏钱，所以先定义再讨论 | Mauboussin、Kaplan、Schilit、Skok、张新民 | evidence: [T01-S011, T01-S034, T01-S029, T01-S064, T01-S086] |
| 3 | **资本配置是第一决策，运营是第二**：钱往哪儿放决定长期结果，且用途是有限的几种 | Buffett、Thorndike、Mauboussin | evidence: [T01-S021, T01-S025, T01-S010] |
| 4 | **增长本身不是好消息，要先问增长的代价**：增长越快现金越紧；ROIC 低于资本成本时增长毁灭价值；烧多少钱换一元新增收入 | Skok、Mauboussin、Sacks、Crabtree | evidence: [T01-S065, T01-S011, T01-S069, T01-S048] |
| 5 | **近似正确胜过精确错误**：与其做一个依赖长期外推的精密模型，不如用一个当期就能改善、不需要预测的粗指标 | Buffett、Penman、Sacks、Crabtree | evidence: [T01-S021, T01-S019, T01-S069, T01-S050] |
| 6 | **框架作者自己划失败边界**（元层面，非常罕见，值得单独提炼成「怎么用别人的框架」）：Kaplan 承认 ABC 常被放弃；Damodaran 写自己方法的十大误区 | Kaplan、Damodaran | evidence: [T01-S035, T01-S007] |

> 上述 6 条**全部满足「≥ 2 个不同 source_id 且跨 ≥ 2 位 figure」**，可直接进入 Phase 2 的 mental model 候选池。

### B. 显著分歧 / 流派分裂（保留矛盾，不和稀泥）

| # | 争的是什么 | A 方 | B 方 | 为什么创始人必须知道 |
|---|-----------|------|------|-------------------|
| **1** | **资本成本这个数字存不存在？** | Damodaran、Mauboussin、公司金融教科书：可以估、必须估，WACC 是投资决策的裁判线 | Penman：把风险压缩成一个数字是虚构；门槛率是你自己的要求回报，不是市场参数 | 决定你要不要花几周去算 WACC。对没有可比上市公司的中小企业，B 方立场更省力也更诚实 (evidence: [T01-S007, T01-S019, T01-S020]) |
| **2** | **提高理解力 vs 绕开理解力** | Berman & Knight、肖星、张新民、Crabtree：教你读懂，然后你自己判断 | Michalowicz：读不懂也没关系，改银行账户结构，用行为约束替代理解 | 决定你的第一步是「上课」还是「改流程」。批评者认为 B 方把利润重新定义成现金存款，在有负债或重资产时会给出错误信号 (evidence: [T01-S039, T01-S053, T01-S056, T01-S057]) |
| **3** | **预测型指标 vs 不预测型指标** | Skok：LTV/CAC、CAC 回收期 —— 建立在流失率外推之上 | Sacks：burn multiple —— 不预测未来，不惩罚沉没成本，当期可改善 | 早期公司数据量下 LTV 几乎不可靠；这不是技术分歧，是「你有没有资格做长期外推」的分歧 (evidence: [T01-S064, T01-S069]) |
| **4** | **准则的可比性 vs 自制口径的相关性** | IASB / FASB / 财政部会计司、准则合规派：口径必须统一才能比较；IFRS 18 把管理层自定义指标拉进附注 | Mauboussin（资本化无形资产）、张新民（资产质量）、整个 non-GAAP 生态：报表口径掩盖了真实经济 | 你自己的管理报表可以自制口径，但对外融资时的口径战争会真实影响估值 (evidence: [T01-S088, T01-S011, T01-S086]) |
| **5** | **精密成本核算 vs 粗颗粒经验比率** | Kaplan：ABC / TDABC，按作业与产能成本率精确分摊 | Crabtree：LER 2:1、税前利润 10-15% 这类可记住的经验阈值 | Kaplan 自己承认 ABC 大规模实施常被放弃；中小企业更可能在 B 方拿到实际收益，但 B 方阈值跨行业不可移植 (evidence: [T01-S035, T01-S049, T01-S051]) |
| **6** | **EBITDA 有没有用** | Munger（广泛转述）：应该读作「狗屁盈利」；Buffett 2000 年信正面批评 | PE 与杠杆融资圈：EBITDA 是偿债能力与经营现金生成的可用近似 | 争的其实是「用在哪个问题上」——衡量所有者回报时它有害，衡量能扛多少债时它有用 (evidence: [T01-S023, T01-S021]) |

### C. 阵营地图（供 Phase 2 分章）

- **准则合规派** → 隐性池 §9.1-9.3（IASB / FASB / 财政部会计司）+ Schilit（从反面用准则）
- **管理会计决策派** → Kaplan、张新民、BBRT（预算反对派）
- **公司金融估值派** → Damodaran、Mauboussin ／ 内部反对派：Penman
- **价值投资资本配置派** → Buffett & Munger、Thorndike
- **创业与 SaaS 指标派** → Skok、Sacks、CJ Gustafson（+ borderline Ben Murray）
- **中小企业现金实操派** → Crabtree（会计框架内）／ Michalowicz（行为规则，争议）
- **财务素养普及派** → Berman & Knight、肖星

### D. 冷僻 / 信号薄弱判定

| 检查项 | 阈值 | 实际 | 判定 |
|-------|------|------|------|
| figure 总数 | ≥ 10 | **16** | ✅ 充足 |
| 每位 ≥ 3 条来源 | 必须 | 16/16 达标 | ✅ |
| source 总数 | 65-90（本次任务设定） | **108** | ⚠️ **超出上限 20%**，见 checklist 说明 |
| verified_primary 占比 | ≥ 40% | **42.6%**（46/108） | ✅ 达标；+ surrogate_primary 合计 **73%** |
| 「近 12 个月动态」填充率 | ≥ 80% | **有动态者 8/16 = 50%** | ⚠️ **未达标** |
| 可信度 low 比例 | < 30% | **0%**（high 5 / medium-high 5 / medium 6） | ✅ |
| 中文 figure 数 | — | **2**，且均无 ≥ 30 分钟长访谈 | ⚠️ **中文维度薄** |

**关于「近 12 个月动态只有 50%」的解释（这不是检索失败，是行业结构）**：本行业的思想领袖有两类。一类是**在职实操者**（Crabtree、CJ Gustafson、Sacks、Damodaran），他们靠持续输出维持影响力，动态密集。另一类是**已完成的经典作者**（Kaplan、Penman、Skok、Berman & Knight、Schilit、肖星、张新民），他们的影响力来自一本书或一篇论文，写完就不再需要发声——**这类人的「沉默」不是失效，是这一行的知识半衰期长**。会计恒等式和 owner earnings 不会因为作者停更而过期。Phase 2 与 SKILL.md 的诚实边界节应当这样表述，而不是简单标注「信息过时风险」。

**必须进入 SKILL.md 诚实边界节的三条**：
1. 中文 figure 只有 2 位，均为学院派教授，均无长访谈，均无近 12 个月动态；**中文的「创业者经营财务实操」一手源为 0**（Track 05 独立得出同一结论）。
2. 隐性 figure 池（IASB / FASB / 财政部会计司 / IMA / AICPA）**全部是机构官方页 surrogate，未直接听到任何个人发声**；关于这些机构方向的判断（如「Sam Woods 的监管背景意味着更偏披露纪律」）是本 track 的推断，已逐条标注。
3. 榜上 16 位有 8 位在近 12 个月内无公开动态；其思想仍然有效，但**任何涉及具体数字、阈值、准则状态的引用都必须回到原始出处核对年份**。

---

## 完成 checklist

### 数量

- **Source 总数**：**108**（T01-S001 ~ T01-S108，无重复 ID）
- **bucket 分布**：
  - `verified_primary`：**46**（42.6%）
  - `surrogate_primary`：**33**（30.6%）— 全部标注了 `own site` / `own publication` / `publisher official page` / `originator` / `official` 之一
  - `secondary`：**29**（26.9%）
  - `dead`：**0**
  - `blacklisted`：**0**
  - 一手合计（verified + surrogate）：**79/108 = 73%**
- **Figures 数**：**16**（+ 隐性 figure 池 5 组机构角色 + borderline 名单 9 类）
- **每位 figure 都有「争议 / 非主流立场」栏**：✅ **16/16**
- **每位 figure ≥ 3 条来源**：✅ 16/16
- **每位 figure 都有「最近 12 个月动态」栏**：✅ 16/16（其中 8 位如实写明「未检索到近 12 个月公开动态」，未编造）
- **每位 figure 都有 endorsement 证据 ≥ 2 独立来源**：✅ 16/16
- **manifest 中被正文引用的 source 比例**：✅ **108/108 = 100%**（无挂着不用的条目）

### ⚠️ 与任务设定的偏差（如实记录，不掩饰）

- **source 总数 108 超出「65-90」的设定上限约 20%。** 原因：16 位 figure × （3 件推荐材料 + 2 条独立 endorsement）已构成约 80 条的下限，加上隐性 figure 池的 5 组机构官方页（IFRS × 3、FASB、财政部会计司 × 3、IMA、AICPA、BBRT）与批评方来源（Profit First 的两篇会计师批评、Outsiders 的幸存者偏差批评、Penman 的学界评议）。**未做删减的理由是：108 条全部被正文引用，删任何一条都会削弱一条 evidence 链。** 若 Phase 1.5 要求严格收敛到 90，建议优先删除 T01-S014 / T01-S068 / T01-S047 / T01-S058 / T01-S078 这类与同组内其他条目高度重叠的补充证据。
- **「近 12 个月动态」有实质内容者仅 8/16（50%），低于模板的 80% 建议值。** 已在 Phase 2 提炼提示 §D 给出结构性解释，并要求原样写入 SKILL.md 诚实边界节。
- **voice_samples 字段未采集。** 本次任务的字段规范由调用方指定为 6 项（核心一句话 / 身份与阵营 / 3 件事 / 争议 / 近 12 个月动态 / endorsement），未包含 voice_samples；且本 track 的检索以文本材料为主，未做音视频转录。**Phase 4 的 voice check 会因此把 voice_confidence 降为 low，这是预期内的。** 若需补齐，优先转录 Damodaran（Meb Faber #619）、Crabtree（Ten Golden Rules #116）、CJ Gustafson（Run the Numbers 任意集）三条长音频。

### 合规

- **黑名单自检**：对全部六个被禁域名（问答社区、公众号、百科、技术博客站、写作社区、股票社区）跑正则检索 → **0 命中**（既不在 manifest 中，也不在正文引用中）。检索过程中确有这些平台的结果返回，**全部主动丢弃**，未用于任何一条 claim。
- **数字纪律**：所有百分比 / 金额 / 阈值均已挂 source_id，或在同句内标注「业内」「据搜索结果」「其个人经验值」「约」「官方」等限定词。特别标注的三处：Crabtree 的 LER 2:1、Sacks 的 burn multiple 分档、Damodaran 对 SpaceX 的估值量级 —— **均已明示为个人经验值 / 个人估算，非行业基准**。
- **版权安全**：全文无超过单句的连续引用，无 transcript 粘贴，全部为结构化摘要 + 链接。
- **未编造**：未给任何 figure 安上没说过的话或没写过的书；无法核实的内容（Munger EBITDA 语录的官方原文出处、财政部会计司领导姓名、Damodaran「被打脸」的归纳）均已逐条标注为「转述」「推断」或「未采信」。

### 状态

✅ **完成** — 2026-09-02
