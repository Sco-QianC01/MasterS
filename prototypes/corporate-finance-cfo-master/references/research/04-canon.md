# Track 04 — Canon 知识正典：企业财务与 CFO 视角（Corporate Finance & the CFO Lens）

> **调研日期**: 2026-09-02 · **locale**: zh-CN · **Track**: 04 (canon)
> **范围锚定**: 面向创业公司与中小企业主/创始人的「看懂钱、管住钱、用好钱」的内部财务判断 —— 读懂三张表、预算与滚动预测、现金流与营运资金、成本核算与定价、融资结构与股权稀释。
> **明确排除**: 投行卖方并购执行与交易建模、VC 投资人的看项目视角、个人理财与二级市场投资、注册会计师/中级职称的考证准则背诵。
>
> **状态**: ✅ 完成

---

## Source Manifest

> bucket 判定：`python3 tools/research/source_verifier.py classify <URL>` 自动结果，只做「升级到 surrogate_primary」的人工调整（准则机构 / 出版社官方 / 作者本人站 / 事务所出版物），不私自降级。
> 403 状态码的条目（Morgan Stanley、FASB）是反爬拦截而非死链，内容经搜索结果与二次来源交叉确认。

| source_id | url | bucket | last_checked | author/host | one-line note |
|-----------|-----|--------|--------------|-------------|---------------|
| T04-S001 | https://store.hbr.org/product/financial-intelligence-revised-edition-a-manager-s-guide-to-knowing-what-the-numbers-really-mean/10833 | verified_primary | 2026-09-02 | Harvard Business Review Press | publisher official page — Financial Intelligence 修订版书页 |
| T04-S002 | https://financialintelligencebook.com/reviews/ | surrogate_primary | 2026-09-02 | Business Literacy Institute | own site — 作者自营书站与评价页 |
| T04-S003 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/ | verified_primary | 2026-09-02 | Aswath Damodaran / NYU Stern | Damodaran Online 主站，估值教材与数据总入口 |
| T04-S004 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datacurrent.html | verified_primary | 2026-09-02 | Aswath Damodaran / NYU Stern | 免费行业数据集：beta / WACC / margins / ROIC |
| T04-S005 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/webcastvalonline.htm | verified_primary | 2026-09-02 | Aswath Damodaran / NYU Stern | 免费估值公开课 25 讲 webcast + slides |
| T04-S006 | https://www.morganstanley.com/im/publication/insights/articles/article_returnoninvestedcapital.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — Counterpoint Global ROIC 计算与常见坑 |
| T04-S007 | https://www.morganstanley.com/im/publication/insights/articles/article_capitalallocation.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — 资本配置五大用途与评估框架 |
| T04-S008 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-18-presentation-and-disclosure-in-financial-statements/ | surrogate_primary | 2026-09-02 | IASB / IFRS Foundation | originator official standard page — IFRS 18，2027-01-01 生效 |
| T04-S009 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-15-revenue-from-contracts-with-customers/ | surrogate_primary | 2026-09-02 | IASB / IFRS Foundation | originator official standard page — IFRS 15 收入五步法 |
| T04-S010 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-16-leases/ | surrogate_primary | 2026-09-02 | IASB / IFRS Foundation | originator official standard page — IFRS 16 租赁上表 |
| T04-S011 | https://www.sec.gov/rules-regulations/staff-guidance/corporation-finance-interpretations/non-gaap-financial-measures | verified_primary | 2026-09-02 | US SEC Corp Fin | 非 GAAP 指标 C&DI 官方解释，Reg G 执法口径 |
| T04-S012 | https://kjs.mof.gov.cn/zt/kjzzss/ | verified_primary | 2026-09-02 | 中国财政部会计司 | 企业会计准则 CAS 官方专题页 |
| T04-S013 | https://www.berkshirehathaway.com/letters/1986.html | verified_primary | 2026-09-02 | Warren Buffett / Berkshire | owner earnings 定义与「现金流谬误」附录原文 |
| T04-S014 | https://book.douban.com/subject/34810876/ | verified_primary | 2026-09-02 | 豆瓣读书 | 肖星《一本书读懂财报》修订版书目权威条目 |
| T04-S015 | https://www.mheducation.com/highered/mhp/product/financial-shenanigans-fourth-edition-how-detect-accounting-gimmicks-fraud-financial-reports.html | surrogate_primary | 2026-09-02 | McGraw-Hill Education | publisher official page — Financial Shenanigans 第 4 版 |
| T04-S016 | https://www.venturedeals.com/ | surrogate_primary | 2026-09-02 | Brad Feld & Jason Mendelson | own site — Venture Deals 官方书站 |
| T04-S017 | https://profitfirstbook.com/ | surrogate_primary | 2026-09-02 | Mike Michalowicz | own site — Profit First 官方书站 |
| T04-S018 | https://simplenumbers.me/ | surrogate_primary | 2026-09-02 | Greg Crabtree | own site — Simple Numbers 官方站与 LER 工具 |
| T04-S019 | https://sbo.financial/blog/accountants/accountants-review-profit-first/ | secondary | 2026-09-02 | SBO Financial | 会计师视角对 Profit First 的系统性批评 |
| T04-S020 | https://wanderwellconsulting.com/why-i-dont-recommend-profit-first/ | secondary | 2026-09-02 | Wanderwell Consulting | 记账事务所「为什么我不推荐 Profit First」 |
| T04-S021 | https://valueandopportunity.com/2016/04/19/capital-allocation-capital-mangement-what-is-good-and-what-is-bad/ | secondary | 2026-09-02 | value and opportunity | 指出 The Outsiders 的幸存者偏差 |
| T04-S022 | https://cup.columbia.edu/book/accounting-for-value/9780231151184/ | verified_primary | 2026-09-02 | Columbia University Press | publisher official page — Penman《Accounting for Value》 |
| T04-S023 | https://cup.columbia.edu/book/narrative-and-numbers/9780231180481/ | verified_primary | 2026-09-02 | Columbia University Press | publisher official page — Damodaran《Narrative and Numbers》 |
| T04-S024 | https://www.degruyterbrill.com/document/doi/10.1515/ael-2013-0026/html | secondary | 2026-09-02 | Accounting, Economics & Law | 学界对 Penman 反 DCF 立场的正式评议 |
| T04-S025 | https://www.mheducation.com/highered/product/Principles-of-Corporate-Finance-Brealey.html | surrogate_primary | 2026-09-02 | McGraw-Hill Education | publisher official page — Brealey/Myers/Allen/Edmans 第 14 版 |
| T04-S026 | https://en.wikipedia.org/wiki/Principles_of_Corporate_Finance | secondary | 2026-09-02 | Wikipedia | 版次沿革与作者更替（Edmans 加入）交叉核对 |
| T04-S027 | https://www.jstor.org/stable/1809766 | secondary | 2026-09-02 | JSTOR / AER | Modigliani-Miller 1958 原文归档页 |
| T04-S028 | https://onlinelibrary.wiley.com/doi/10.1111/j.1540-6261.1984.tb03646.x | verified_primary | 2026-09-02 | Journal of Finance / Wiley | Myers 1984《The Capital Structure Puzzle》原文 |
| T04-S029 | https://www.sciencedirect.com/science/article/abs/pii/0304405X84900230 | verified_primary | 2026-09-02 | JFE / Elsevier | Myers & Majluf 1984 融资优序理论原文 |
| T04-S030 | https://www.nber.org/papers/w1396 | secondary | 2026-09-02 | NBER | Myers & Majluf 工作论文免费全文 |
| T04-S031 | https://hbr.org/1988/09/measure-costs-right-make-the-right-decisions | verified_primary | 2026-09-02 | Cooper & Kaplan / HBR | 作业成本法 ABC 的奠基文章 |
| T04-S032 | https://hbr.org/2004/11/time-driven-activity-based-costing | verified_primary | 2026-09-02 | Kaplan & Anderson / HBR | Kaplan 自陈 ABC 实施常被放弃，提出 TDABC |
| T04-S033 | https://bbrt.org/ | surrogate_primary | 2026-09-02 | Beyond Budgeting Round Table | originator official site — BBRT 12 原则 |
| T04-S034 | https://www.sciencedirect.com/science/article/abs/pii/S0304405X19301692 | verified_primary | 2026-09-02 | JFE / Elsevier | Gornall & Strebulaev 独角兽估值虚高 48% |
| T04-S035 | https://www.nber.org/papers/w23895 | secondary | 2026-09-02 | NBER | 同上论文的免费工作论文版 |
| T04-S036 | https://www.wiley.com/en-us/Venture+Deals:+Be+Smarter+Than+Your+Lawyer+and+Venture+Capitalist,+4th+Edition-p-9781119594840 | surrogate_primary | 2026-09-02 | Wiley | publisher official page — Venture Deals 第 4 版 |
| T04-S037 | https://www.icourse163.org/course/UIBE-1003252013 | secondary | 2026-09-02 | 对外经济贸易大学 / 中国大学MOOC | 张新民《财务报表分析》慕课，配套教材体系 |
| T04-S038 | https://book.douban.com/subject/36285053/ | verified_primary | 2026-09-02 | 豆瓣读书 | 张新民《财务报表分析》第 6 版书目条目 |
| T04-S039 | https://hbr.org/2001/11/corporate-budgeting-is-broken-lets-fix-it | verified_primary | 2026-09-02 | Michael C. Jensen / HBR | 预算与奖金挂钩 = 花钱买谎话 |
| T04-S040 | https://aswathdamodaran.blogspot.com/2015/02/dcf-myth-1-if-you-have-ddiscount-rate.html | verified_primary | 2026-09-02 | Aswath Damodaran | own site — DCF 十大误区系列开篇 |
| T04-S041 | https://pages.stern.nyu.edu/~adamodar/pdfiles/country/DCFmythsTemasek.pdf | verified_primary | 2026-09-02 | Aswath Damodaran / NYU | DCF 十大误区讲义 PDF |
| T04-S042 | https://www.forentrepreneurs.com/saas-metrics-2/ | verified_primary | 2026-09-02 | David Skok | own site — SaaS Metrics 2.0，创业单位经济学奠基 |
| T04-S043 | https://www.ecfr.gov/current/title-17/chapter-II/part-244 | verified_primary | 2026-09-02 | eCFR / 17 CFR Part 244 | Regulation G 法规原文 |
| T04-S044 | https://www.fasb.org/standards | surrogate_primary | 2026-09-02 | FASB | originator official page — US GAAP 准则总入口（含 ASC 606） |
| T04-S045 | https://kjs.mof.gov.cn/zt/kjzzss/kuaijizhunzeshishiwenda/ | verified_primary | 2026-09-02 | 中国财政部会计司 | 企业会计准则实施问答，中国口径的判断依据 |
| T04-S046 | https://www.gsb.stanford.edu/faculty-research/publications/squaring-venture-capital-valuations-reality | verified_primary | 2026-09-02 | Stanford GSB | 独角兽估值虚高论文的机构页 |
| T04-S047 | https://www.semanticscholar.org/paper/A-Cash-Conversion-Cycle-Approach-to-Liquidity-Richards-Laughlin/6f0a861d27e59ce73f8b8207121e52980248a0c2 | secondary | 2026-09-02 | Semantic Scholar | Richards & Laughlin 1980 现金转换周期原始论文索引 |
| T04-S048 | https://czj.sh.gov.cn/zys_8908/zcfg_8983/zcfb_8985/hj_9035/cwhjjbzdgf/20120208/0017-156925.html | verified_primary | 2026-09-02 | 上海市财政局转发财会〔2011〕17号 | 《小企业会计准则》全文（政府门户转发） |
| T04-S049 | https://www.forentrepreneurs.com/saas-economics-1/ | verified_primary | 2026-09-02 | David Skok | own site — SaaS 现金流低谷，越快增长越缺钱 |
| T04-S050 | https://www.wiley.com/en-us/Investment+Valuation:+Tools+and+Techniques+for+Determining+the+Value+of+Any+Asset,+3rd+Edition-p-9781394254606 | surrogate_primary | 2026-09-02 | Wiley | publisher official page — Damodaran《Investment Valuation》 |
| T04-S051 | https://www.wiley.com/en-nl/The+Little+Book+of+Valuation:+How+to+Value+a+Company,+Pick+a+Stock+and+Profit-p-9781118064146 | surrogate_primary | 2026-09-02 | Wiley | publisher official page — Damodaran《The Little Book of Valuation》 |
| T04-S052 | https://www.morganstanley.com/im/publication/insights/articles/article_valuationmultiples.pdf | surrogate_primary | 2026-09-02 | Mauboussin & Callahan | own publication — 倍数法本质是简化的 DCF |
| T04-S053 | https://www.eatonvance.com/content/dam/im/assets/publication/thought-leadership/consilient-observer/article_everythingisadcfmodel_us.pdf | secondary | 2026-09-02 | Eaton Vance（MSIM 分发） | 《Everything Is a DCF Model》全文可下载副本 |
| T04-S054 | https://aswathdamodaran.substack.com/ | verified_primary | 2026-09-02 | Aswath Damodaran | own site — 现行主力发文渠道（blogspot 已并行） |
| T04-S055 | https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/ | surrogate_primary | 2026-09-02 | MIT OpenCourseWare | official course syllabus — 公司金融理论 reading list |
| T04-S056 | https://www.simonandschuster.co.uk/books/Financial-Statements/Thomas-Ittelson/9781632652072 | surrogate_primary | 2026-09-02 | Career Press / Red Wheel Weiser | publisher official page — Ittelson《Financial Statements》 |
| T04-S057 | https://www.iasplus.com/en/standards/ifrs/ifrs15 | surrogate_primary | 2026-09-02 | Deloitte IAS Plus | vendor docs — IFRS 15 五步法与实务要点 |
| T04-S058 | https://www.iasplus.com/en/standards/ifrs/ifrs-16 | surrogate_primary | 2026-09-02 | Deloitte IAS Plus | vendor docs — IFRS 16 使用权资产与租赁负债 |
| T04-S059 | https://kpmg.com/xx/en/what-we-do/services/audit/corporate-reporting-institute/ifrs/presentation-and-disclosure/ifrs18.html | verified_primary | 2026-09-02 | KPMG | vendor docs — IFRS 18 三大变化与过渡安排 |
| T04-S060 | https://www.sec.gov/rules/final/33-8176.htm | verified_primary | 2026-09-02 | US SEC | Regulation G 与 Item 10(e) 最终规则发布文 |
| T04-S061 | https://www.ifrs.org/issued-standards/ifrs-for-smes/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator official page — 中小企业简化准则 IFRS for SMEs |
| T04-S062 | https://feld.com/archives/2011/07/venture-deals-be-smarter-than-your-lawyer-and-venture-capitalist/ | secondary | 2026-09-02 | Brad Feld | 作者自述本书源于 term sheet 博客连载 |
| T04-S063 | https://www.xuetangx.com/course/THU08091000367 | secondary | 2026-09-02 | 学堂在线 / 清华大学 | 肖星《财务分析与决策》国家精品课 |
| T04-S064 | https://en.wikipedia.org/wiki/Pecking_order_theory | secondary | 2026-09-02 | Wikipedia | 融资优序理论的谱系（Donaldson 1961 → Myers 1984） |
| T04-S065 | https://en.wikipedia.org/wiki/Owner_earnings | secondary | 2026-09-02 | Wikipedia | owner earnings 定义与出处交叉核对 |
| T04-S066 | https://cas.xmu.edu.cn/zkjs/zzzdzlk/CAS/b1__zghjzzsl/qyhjzzd14h__sr_2017_.htm | verified_primary | 2026-09-02 | 厦门大学会计发展研究中心 | CAS 14 收入（2017 修订）准则全文 |
| T04-S067 | https://kjs.mof.gov.cn/zt/kjzzss/qykjzz/ | verified_primary | 2026-09-02 | 中国财政部会计司 | 企业会计准则具体准则目录（含 14 号 / 21 号） |
| T04-S068 | https://papers.ssrn.com/sol3/papers.cfm?abstract_id=267651 | verified_primary | 2026-09-02 | Michael C. Jensen / SSRN | 《Paying People to Lie》预算与奖金的完整论文版 |
| T04-S069 | https://maaw.info/ArticleSummaries/ArtSumJensen2001.htm | secondary | 2026-09-02 | Management & Accounting Web | Jensen 预算论文的学术摘要与批评脉络 |
| T04-S070 | https://en.wikipedia.org/wiki/Valuation:_Measuring_and_Managing_the_Value_of_Companies | secondary | 2026-09-02 | Wikipedia | Koller/Goedhart/Wessels《Valuation》版次与定位 |
| T04-S071 | https://www.morganstanley.com/im/en-us/individual-investor/insights/consilient-observer/return-on-invested-capital.html | surrogate_primary | 2026-09-02 | Michael Mauboussin / MSIM | own publication — ROIC 系列文章落地页 |
| T04-S072 | https://www.iasplus.com/en/standards/ifrs/ifrs-18 | surrogate_primary | 2026-09-02 | Deloitte IAS Plus | vendor docs — IFRS 18 变化要点与生效安排 |
| T04-S073 | https://www.thecasecentre.org/products/view?id=41919 | secondary | 2026-09-02 | The Case Centre | Jensen 预算文章的教学案例发行页 |
| T04-S074 | https://www.oreilly.com/library/view/venture-deals-4th/9781119594826/ | secondary | 2026-09-02 | O'Reilly | Venture Deals 第 4 版被技术教育平台收录 |
| T04-S075 | https://www.avalonaccounting.ca/books/simple-numbers-straight-talk-big-profits | secondary | 2026-09-02 | Avalon Accounting（会计事务所） | 从业会计师对 Simple Numbers 四把钥匙的应用复盘 |

---

## 总览（按类型分组）

### Textbook / 系统性著作（必读 14 本）

| # | 书名 | 作者 | 年份/版本 | 难度 | 它立的规矩（一句话） |
|---|------|------|-----------|------|---------------------|
| 1 | Financial Intelligence | Berman, Knight, Case | 2006 / rev. 2013 | 入门 | 利润是估计出来的，现金是数出来的 |
| 2 | Financial Statements: A Step-by-Step Guide | Thomas Ittelson | 1998 / 3rd 2020 | 入门 | 说你懂财报，标准是你能自己把三张表做平 |
| 3 | Principles of Corporate Finance | Brealey, Myers, Allen, Edmans | 1981 / 14th 2022 | 进阶-高阶 | NPV 是一切投资决策的唯一裁判 |
| 4 | Investment Valuation / Little Book of Valuation | Aswath Damodaran | 1996– / 持续更新 | 进阶 | 估值的门槛不是数据垄断，是假设的诚实 |
| 5 | Narrative and Numbers | Aswath Damodaran | 2017 | 进阶 | 故事没有数字是空想，数字没有故事是伪精确 |
| 6 | Simple Numbers, Straight Talk, Big Profits! | Greg Crabtree | 2011 / 2.0 | 入门-进阶 | 老板先拿市场行情工资，剩下的才叫利润 |
| 7 | Profit First | Mike Michalowicz | 2014 / rev. 2017 | 入门 | 收入 − 利润 = 费用（行为规矩，非会计规矩） |
| 8 | Venture Deals | Feld & Mendelson | 2011 / 4th 2019 | 进阶 | 每张 term sheet 是经济与控制两场谈判叠加 |
| 9 | Financial Shenanigans | Schilit, Perler, Engelhart | 1993 / 4th 2018 | 进阶 | 看财报不是阅读，是质询 |
| 10 | The Outsiders | William Thorndike | 2012 | 入门-进阶 | CEO 的第一职责是资本配置 |
| 11 | Berkshire 致股东信（1986 附录） | Warren Buffett | 1977– | 进阶 | owner earnings：折旧是真实费用，维持性资本开支必须扣 |
| 12 | Accounting for Value | Stephen Penman | 2011 | 高阶 | 锚定已知（会计），把推测放在最后 |
| 13 | 《一本书读懂财报》 | 肖星 | 2014 / 修订版 | 入门 | 利润表看能力，资产负债表看家底，现金流量表看死活 |
| 14 | 《财务报表分析》第 6 版 | 张新民、钱爱民 | 2019 / 6th 2023 | 进阶 | 同样的数字，质量可以完全不同 |

### 准则与规则原文（Standards as Canon，5 组）

| 准则 | 发布机构 | 关键时点 | 它立的规矩 |
|------|---------|---------|-----------|
| IFRS 15 / ASC 606 收入 | IASB / FASB | 中国 CAS 14 于 2017 修订趋同，2018/2020/2021 分批实施 | 收入确认统一到五步法；收到钱 ≠ 确认收入 |
| IFRS 16 租赁 | IASB | 中国 CAS 21 趋同 | 消灭经营租赁的表外藏身处；EBITDA 被系统性抬高 |
| IFRS 18 列报 | IASB | **2024-04-09 发布，2027-01-01 生效**，取代 IAS 1 | 规定损益表结构；把管理层自定义指标 MDPM 拉进附注 |
| SEC Reg G / Item 10(e) | US SEC | 现行 + C&DI 持续更新 | 非 GAAP 指标可用，但必须调节、不得误导 |
| CAS 与《小企业会计准则》 | 中国财政部 | 小准则财会〔2011〕17 号，**2013-01-01 施行** | 给小企业一条合法的简化路径；选哪套是战略选择 |

### Seminal Papers / 研究 / 数据集（10 条）

| # | 标题 | 作者 / 年 | 核心 idea |
|---|------|----------|-----------|
| 1 | The Cost of Capital, Corporation Finance and the Theory of Investment | Modigliani & Miller, 1958 | 完美市场下资本结构与企业价值无关；倒过来用于定位现实中的摩擦 |
| 2 | Corporate Financing and Investment Decisions...（pecking order） | Myers & Majluf, 1984 | 信息不对称导致融资偏好：留存 > 债务 > 股权 |
| 3 | Measure Costs Right: Make the Right Decisions | Cooper & Kaplan, HBR 1988 | 传统分摊扭曲产品成本；改按作业消耗分摊 |
| 4 | Corporate Budgeting Is Broken / Paying People to Lie | Jensen, HBR 2001 | 预算挂钩奖金 = 花钱购买失真信息 |
| 5 | Squaring Venture Capital Valuations with Reality | Gornall & Strebulaev, JFE 2020 | 独角兽报告估值平均虚高 48%，普通股虚高 56% |
| 6 | ROIC / Capital Allocation / Everything Is a DCF Model 系列 | Mauboussin & Callahan, 2021– | ROIC > 资本成本时增长才创造价值；倍数是压缩的 DCF |
| 7 | Damodaran Online 数据集 + 25 讲免费估值课 | Damodaran, NYU Stern | 免费 beta / ERP / 行业 ROIC 与倍数；每年更新 |
| 8 | Beyond Budgeting 12 原则与研究 | Hope, Fraser, Bunce / BBRT 1998– | 拆开目标、预测、资源分配三件事 |
| 9 | A Cash Conversion Cycle Approach to Liquidity Analysis | Richards & Laughlin, 1980 | 流动性从静态清算视角改为动态循环速度 |
| 10 | SaaS Metrics 2.0 / SaaS 现金流低谷 | David Skok | 增长越快现金越差；关键是单客户能否回本 |

### Courses（4 门，全部含 last_updated）

| 课程 | 讲师 / 机构 | 格式 | Last_updated | 一句话 |
|------|-----------|------|--------------|--------|
| Valuation Online Class（25 讲 webcast） | Aswath Damodaran / NYU Stern | 视频 + 讲义 + 课后测验，**rolling**（随学期更新） | rolling，配套数据集每年 1 月刷新；使用前必须核对页面数据年份 (evidence: [T04-S005, T04-S004]) | 免费复刻其学期估值课的完整路径 |
| 《财务分析与决策》 | 肖星 / 清华大学，学堂在线 | 中文 MOOC，国家精品课，配套《一本书读懂财报》 | 平台按学期开课滚动（自 2016 秋首开，长期重复开设） (evidence: [T04-S063, T04-S014]) | 中文圈财报入门的默认公开课 |
| 《财务报表分析》 | 张新民 / 对外经济贸易大学，中国大学 MOOC | 中文 MOOC，配套人大社教材（第 6 版 2023） | 平台滚动开课；教材第 6 版 2023-01 (evidence: [T04-S037, T04-S038]) | 「财务状况质量」体系的作者亲授版 |
| MIT 15.401 Finance Theory I | MIT / OpenCourseWare | 讲义 + 作业 + 考题（存档式） | **2008 秋季版存档，未再更新** — 仅作 syllabus / reading list 参考 (evidence: [T04-S055]) | 公司金融理论骨架（NPV / CAPM / MM）的免费 syllabus |

> **课程时效提醒**：MIT 15.401 是 2008 存档版，准则相关内容（收入、租赁）已完全过时，只能用于理论骨架；两门中文 MOOC 需按平台当期开课情况核对；Damodaran 的数据每年必须重取。

### Core Concepts（26 个）

见 [第四节](#四核心概念26-个)。tier-1 共 20 个（所有创始人必懂），tier-2 共 6 个（资深者熟知）。

---

## 一、必读正典（书）

> 每本按：作者/年份/版本 → **它到底立了什么规矩** → 为什么是正典（≥3 独立来源）→ **局限 / 被批评之处**（写实，不只写优点）。
> 「立了什么规矩」= 这本书让这行的人从此怎么想问题，不是内容摘要。

---

### 📖 1. Financial Intelligence: A Manager's Guide to Knowing What the Numbers Really Mean

- **Author**: Karen Berman, Joe Knight, with John Case
- **Year**: 2006 初版 / **Revised Edition 2013**（Harvard Business Review Press）
- **Type**: 面向非财务管理者的系统性入门
- **难度**: 入门
- **它立了什么规矩**：把「财务是一门带有判断的艺术，不是一组客观事实」这句话变成非财务人的默认起点。它明确教一件事——**利润是估计出来的，现金是数出来的**（accrual 下的收入确认、坏账计提、折旧年限全是选择），所以看到利润数字第一反应应该是「这个数是怎么估出来的」，而不是「这个数是多少」。它同时定死了非财务管理者的最低门槛：能读懂三张表 + 知道自己日常决策（给客户宽松账期、囤库存、加人）会砸到哪张表的哪一行 (evidence: [T04-S001, T04-S002])
- **核心论点**：① 财务数字含有大量假设与偏好，「财务智商」就是识别这些假设的能力；② 利润 ≠ 现金，理解两者背离是管理者的第一课；③ 比率不是答案，是提问的起点；④ 营运资金是经营决策的直接后果，不是财务部门的事 (evidence: [T04-S001])
- **读完得到什么**：能拿到一份自己公司的三张表，说出「这家公司是靠什么赚钱的、钱卡在哪里、哪些数字是被会计政策做出来的」
- **Endorsement evidence**：
  - `[course_syllabus]` 长期作为 HBR Press 面向管理者的财务素养标准读物在售并出修订版，被大量 MBA/EMBA 非财务模块采用 (evidence: [T04-S001])
  - `[figure_long]` 作者自营 Business Literacy Institute 长期以此书为培训教材，累计培训大量企业管理者 (evidence: [T04-S002])
  - `[blog_secondary]` 中英文创业者书单反复出现，2013 修订版本身是「持续被读」的市场证据 (evidence: [T04-S001])
- **局限 / 被批评之处**：
  - **深度天花板明显**：为了可读性牺牲了准确度，涉及收入确认、租赁、递延所得税等真正难的判断题时只点到为止，靠它无法处理 IFRS 15 五步法这类实际难题 (evidence: [T04-S009])
  - **案例偏美国大中型上市公司**，中小企业主关心的「老板工资怎么算」「税负如何影响留存」几乎不涉及，需要 Crabtree 补 (evidence: [T04-S018])
  - **修订版仍停在 2013**，对 SaaS/订阅制的递延收入与合同资产、以及 IFRS 16 后租赁上表的影响没有覆盖 (evidence: [T04-S010])
- **替代品**: Ittelson《Financial Statements》（更偏机械操作，教你逐笔造表）
- **如果只读 1 章**: 讲「利润是估计值 / Profit is an estimate」的那部分——这是全书唯一不可替代的观念
- **可信度**: high · **Decay risk**: low（观念不过时）/ medium（准则细节已旧）

---

### 📖 2. Financial Statements: A Step-by-Step Guide to Understanding and Creating Financial Reports

- **Author**: Thomas R. Ittelson
- **Year**: 1998 初版 / **Third Edition 2020**（Career Press，20 周年版，累计 20 万册以上）
- **Type**: 操作型教程
- **难度**: 入门
- **它立了什么规矩**：把「三张表勾稽」从抽象概念变成可以手动跑一遍的机械动作。全书用一家虚构公司的连续交易，逐笔演示每一笔业务同时打在资产负债表、利润表、现金流量表上的位置。它立的规矩是：**你说你懂财报，标准是你能自己把三张表连起来做平**——做不平就是没懂 (evidence: [T04-S056])
- **核心论点**：① 每笔交易都同时影响多张表，孤立看单表必然误判；② 现金流量表是三张表里唯一「无处躲藏」的表；③ 创业者要能自己搭出预计报表，而不是等会计给结果
- **读完得到什么**：能从一堆流水自己搭出三张表并做平；看别人的表时知道每个数字应该在别的表里对应到哪
- **Endorsement evidence**：
  - `[course_syllabus]` 长期被创业课程与 MBA 预修（accounting bootcamp）作为动手材料使用，第 3 版由出版社按 20 周年重排说明持续采用 (evidence: [T04-S056])
  - `[figure_short]` 出版方与经销渠道明确定位读者为「entrepreneurs, non-financial managers, lawyers, lenders, investors」，20 万册销量是持续被读的证据 (evidence: [T04-S056])
  - `[blog_secondary]` 在英文创业财务书单中与 Berman & Knight 长期成对出现，扮演「动手篇」角色 (evidence: [T04-S056])
- **局限 / 被批评之处**：
  - **只到「怎么做」，不到「怎么判断」**：教你把表做平，但不教你判断这套数字质量好不好、有没有被粉饰；要判断得转 Schilit 或张新民 (evidence: [T04-S015, T04-S038])
  - **纯 US GAAP 语境**，中国的增值税、发票制、CAS 与《小企业会计准则》差异完全没有，中国用户直接照搬会出错 (evidence: [T04-S048])
  - 对已经会做账的人价值低，是典型的「零基础专属」书
- **如果只读 1 章**: 三表联动的那组连续交易演示
- **可信度**: high · **Decay risk**: low

---

### 📖 3. Principles of Corporate Finance

- **Author**: Richard A. Brealey, Stewart C. Myers, Franklin Allen, **Alex Edmans**（第 14 版新增作者）
- **Year**: 1981 初版 / **14th Edition 2022**（McGraw-Hill）
- **Type**: 研究生级教科书
- **难度**: 进阶 → 高阶
- **它立了什么规矩**：确立了「公司金融是一套可以推导的理论，不是经验汇编」这个立场，并把**净现值 NPV 作为一切投资决策的唯一裁判**写进了全球商学院的默认语言。它的关键主张是：懂理论不是为了套公式，是为了在遇到教科书没写过的非常规情况时还能判断——所以它先解释「公司和市场为什么这么行为」，再给工具 (evidence: [T04-S025, T04-S026])
- **核心论点**：① 价值来自现金流与风险，不来自会计利润；② 机会成本是资本预算的真正标尺；③ 资本结构在无摩擦世界里不影响价值（MM 定理），现实中的偏离来自税盾、破产成本、信息不对称；④ 市场有效性是基准假设而非信仰 (evidence: [T04-S025, T04-S027])
- **读完得到什么**：能对任一投资/融资决策给出一个有理论依据的判断框架，并说清自己的假设错在哪会翻盘
- **Endorsement evidence**：
  - `[course_syllabus]` 全球 MBA/MSF 公司金融课的长期标准教材，40 余年连续改版本身是采用证据 (evidence: [T04-S025, T04-S026])
  - `[course_syllabus]` MIT OpenCourseWare 15.401 Finance Theory I 等公开课的公司金融部分沿用同一理论骨架（NPV / CAPM / MM） (evidence: [T04-S055])
  - `[conf_citation]` Damodaran 的估值教学与 Mauboussin 的资本配置研究都建立在这套 NPV + 资本成本框架之上 (evidence: [T04-S003, T04-S007])
- **局限 / 被批评之处**：
  - **对中小企业主几乎不可直接使用**：假设有公开市场定价、可估 beta、可发债，而绝大多数中小企业这三条都不成立；照搬 CAPM 算折现率是最常见的误用 (evidence: [T04-S040])
  - **百科全书式，篇幅巨大**，非全职学生很难读完；实践中多作查阅书而非通读书
  - **理论与现实的缝隙被批评**：MM 定理的前提（无税、无破产成本、信息对称）在现实中全部不成立，教科书虽有讨论，但学生容易把结论当成「资本结构不重要」误用 (evidence: [T04-S027, T04-S029])
  - 价格高、版次更新频繁被指有教材经济学的商业动机（这一点是行业普遍批评，不针对本书独有）
- **替代品**: Berk & DeMarzo《Corporate Finance》（更结构化、更偏教学法）；只想要判断力不想要推导的读者应直接读 Damodaran
- **如果只读 1 章**: 资本预算与 NPV 那一组章节 + 资本结构章
- **可信度**: high · **Decay risk**: low

---

### 📖 4. Investment Valuation（及配套 The Little Book of Valuation）

- **Author**: Aswath Damodaran
- **Year**: Investment Valuation 初版 1996，最新版由 Wiley 持续更新；The Little Book of Valuation 2011 初版，2024 出新版 (evidence: [T04-S050, T04-S051])
- **Type**: 估值参考书（大部头）+ 面向普通投资者的精简版
- **难度**: 进阶（Little Book 入门）
- **它立了什么规矩**：把估值从「投行的黑箱手艺」变成**公开、可复现、带公开数据的公共方法论**。Damodaran 把行业 beta、股权风险溢价、各行业利润率与 ROIC 全部免费公开在 NYU 站点上，等于宣布：**估值的门槛不是数据垄断，是假设的诚实**。他立的第二条规矩是「估值是有偏见的（bias）、不确定的（uncertainty）、且复杂度并不带来准确度」——所以模型越大越可疑 (evidence: [T04-S003, T04-S004, T04-S040])
- **核心论点**：① 任何资产的价值 = 预期现金流按风险折现；② 相对估值（倍数法）不是 DCF 的替代品，是压缩版的 DCF；③ 折现率不是最重要的输入，现金流与再投资才是；④ 复杂度是偏见的藏身处 (evidence: [T04-S040, T04-S041, T04-S052])
- **读完得到什么**：能对一家非上市公司给出一个自己敢为其假设辩护的价值区间，并说出哪个假设变动会推翻结论
- **Endorsement evidence**：
  - `[figure_long]` 作者本人在 NYU 免费公开 25 讲估值课 + 全部讲义与课后测验，是本书的官方配套 (evidence: [T04-S005])
  - `[course_syllabus]` NYU Stern 正式学位课与 Executive Education 15 周估值课均以其教材与数据为核心 (evidence: [T04-S003])
  - `[conf_citation]` Mauboussin 的 Counterpoint Global 系列在讨论倍数与 DCF 关系时与 Damodaran 同一立场并互相呼应 (evidence: [T04-S052])
- **局限 / 被批评之处**：
  - **对早期公司的适用性被反复质疑**：现金流为负、无可比公司、生存概率本身不确定时，DCF 的输出区间大到近乎无信息；Damodaran 自己承认「不确定性大」不是不做 DCF 的理由，但这恰是批评者的分歧点 (evidence: [T04-S040])
  - **学术侧的正面反对**：Penman 认为 DCF 把估值押在最不可知的远期预测和无法观测的资本成本上，主张改用会计利润与账面价值锚定 (evidence: [T04-S022, T04-S024])
  - **公开数据集的滥用**：NYU 行业均值被大量使用者当成「标准答案」直接套到自己公司，忽略样本是上市公司、规模与流动性完全不同 (evidence: [T04-S004])
  - 大部头版本对中小企业主性价比低，Little Book 版信息密度更合适
- **如果只读 1 章**: 关于估值中的偏见与不确定性那一章；或直接读 DCF 十大误区讲义 (evidence: [T04-S041])
- **可信度**: high · **Decay risk**: low（方法）/ medium（数据须每年重取）

---

### 📖 5. Narrative and Numbers: The Value of Stories in Business

- **Author**: Aswath Damodaran
- **Year**: 2017（Columbia University Press / Columbia Business School Publishing）
- **Type**: 方法论专著
- **难度**: 进阶
- **它立了什么规矩**：把「讲故事」和「算数字」从对立关系改判为**必须互相约束的一对**。它立的规矩是：任何估值数字都必须能翻译回一个可以被质疑的商业叙事（这家公司要成为什么、多大市场、多高份额、多少利润率），而任何叙事都必须能落成一组具体数字并接受**可能性 / 合理性 / 概率**三重检验。故事没有数字是空想，数字没有故事是伪精确 (evidence: [T04-S023])
- **核心论点**：① 估值分歧的根源通常是叙事分歧，不是折现率分歧；② 叙事必须经过「possible / plausible / probable」三道筛；③ 公司历史既滋养也约束叙事（Uber / Twitter / Facebook / Amazon 案例）；④ 叙事改变时要显式承认并重估，而不是偷偷改参数 (evidence: [T04-S023])
- **读完得到什么**：面对创始人的增长故事，能立刻把它翻译成收入规模、利润率、再投资率三个数，并指出哪一步在数学上不成立
- **Endorsement evidence**：
  - `[figure_long]` 作者在自有博客与 Substack 长期用同一框架公开做估值案例，形成持续教学 (evidence: [T04-S040, T04-S054])
  - `[course_syllabus]` Columbia Business School Publishing 出版并纳入其商学院出版体系 (evidence: [T04-S023])
  - `[blog_secondary]` 被估值行业媒体（Business Valuation Resources 等）作为方法论书评长期引用 (evidence: [T04-S023])
- **局限 / 被批评之处**：
  - **落地手续少**：框架好记，但把叙事转成数字的中间步骤依赖大量个人判断，书里没有可复制的机械流程
  - **案例集中在高关注度科技公司**，中小企业与传统行业读者的迁移成本比预期高
  - 部分书评认为它更像是给已经会做 DCF 的人加一层纪律，不适合作为估值入门 (evidence: [T04-S023])
- **如果只读 1 章**: Uber 估值那组「同一公司、不同叙事、不同数字」的对照
- **可信度**: high · **Decay risk**: low

---

### 📖 6. Simple Numbers, Straight Talk, Big Profits!（及 Simple Numbers 2.0）

- **Author**: Greg Crabtree（with Beverly Blair Harzog）
- **Year**: 2011 初版；后续 Simple Numbers 2.0 扩展
- **Type**: 中小企业现金与利润实操
- **难度**: 入门 → 进阶
- **它立了什么规矩**：给中小企业主定了两条会被反复引用的硬规矩——**① 老板必须先给自己发市场行情的工资，再谈利润**（否则利润是假的，只是把老板工资藏进了利润里）；**② 税前净利率 10% 是「还活着」的及格线，15% 以上才算好**。第三条是它真正的贡献：**劳动效率比（Labor Efficiency Ratio）**——用「毛利 ÷ 直接人工成本」衡量每投 1 元人工产出多少毛利，把「人效」从口号变成可跨行业比较的数字 (evidence: [T04-S018])
- **核心论点**：① 老板工资必须先做市场化还原，否则所有利润指标失真；② 人是大多数服务型企业最大的成本，人效比营收增速更重要；③ 现金、利润、税三者必须同时规划；④ 增长要用现金买，规模不等于安全 (evidence: [T04-S018, T04-S075])
- **读完得到什么**：能把自己公司的报表重算成「老板工资还原后的真实利润」，并算出各团队的人效比
- **Endorsement evidence**：
  - `[figure_long]` 作者本人是执业 CPA，长期以此体系为中小企业与 EO/Vistage 类企业家组织授课，官方站点提供配套工具 (evidence: [T04-S018])
  - `[blog_secondary]` 被大量会计事务所与行业从业者作为客户咨询框架采用并公开复盘（如建筑装修行业的实践笔记） (evidence: [T04-S018])
  - `[blog_secondary]` 在英文中小企业财务书单中与 Profit First 并列出现，扮演「更严谨的那一本」角色 (evidence: [T04-S017, T04-S019])
- **局限 / 被批评之处**：
  - **基准值的适用边界没有交代清楚**：10% 税前净利率、LER 1.8–2.2 这些数字来自作者服务的美国服务型中小企业样本，重资产、低毛利、长账期行业照搬会得出荒谬结论 (evidence: [T04-S018])
  - **美国税制与实体结构强绑定**（S-corp / pass-through 的税务规划贯穿全书），中国读者需要整体重译才能用 (evidence: [T04-S048])
  - LER 把福利与税费排除在「直接人工」之外的定义是作者自定义口径，与通用管理会计口径不一致，跨公司比较前必须先统一定义 (evidence: [T04-S018])
- **替代品**: Berman & Knight（更中性、更少美国税制）
- **如果只读 1 章**: 老板工资还原 + 劳动效率比那两章
- **可信度**: medium-high（框架 high，基准值 medium） · **Decay risk**: medium（税制相关内容衰减快）

---

### 📖 7. Profit First

- **Author**: Mike Michalowicz
- **Year**: 2014 初版 / 2017 修订版（Portfolio / Penguin）
- **Type**: 行为型现金管理方法
- **难度**: 入门
- **它立了什么规矩**：把会计恒等式**故意倒过来**：不是「收入 − 费用 = 利润」，而是「**收入 − 利润 = 费用**」。做法是每笔收入进账后立刻按固定比例分拨到几个独立银行账户（利润 / 老板工资 / 税 / 运营），运营账户里剩多少就只能花多少。它立的规矩不是会计规矩，是**行为规矩**：用账户物理隔离制造人为稀缺，逼老板先兑现利润再谈开销 (evidence: [T04-S017, T04-S019])
- **核心论点**：① 帕金森定律在企业开支上成立——有多少花多少，所以要先把钱拿走；② 小企业主不看报表、只看银行余额，所以工具要顺应这个习惯而不是纠正它；③ 税和老板工资必须预先扣留，不能事后补 (evidence: [T04-S017, T04-S019])
- **读完得到什么**：一套当天就能开始执行的现金纪律；对现金失控型小企业见效快
- **Endorsement evidence**：
  - `[figure_long]` 作者建立了 Profit First Professionals 认证会计师网络并持续布道，官方站点是一手渠道 (evidence: [T04-S017])
  - `[blog_secondary]` 大量独立会计/记账事务所公开撰文评价（正反都有），说明它已进入专业圈的讨论议程 (evidence: [T04-S019, T04-S020])
  - `[blog_secondary]` 在小企业主群体中形成事实上的通用词汇（「Profit First 账户」），传播广度本身构成 canon 资格 (evidence: [T04-S017])
- **局限 / 被批评之处（这本必须写足）**：
  - **专业会计师的核心批评：它把症状管理当成了病因治疗**。分账户不改变企业的真实经济状况——毛利不够、定价过低、成本结构错误的企业，分完账户后只是更早发现付不起账单，问题本身没解决 (evidence: [T04-S019, T04-S020])
  - **越过了适用条件却从不声明**：方法的成立高度依赖定价能力、固定成本占比、资本密集度、需求弹性；作者把在自己那类轻资产服务业里有效的做法推广成普适法则，却没有说明前提 (evidence: [T04-S019])
  - **与权责发生制冲突**：银行余额法忽略应收应付与递延，对有大额在手订单/预收款的企业会给出严重误导的「利润」信号；对项目制、长周期收款企业尤其危险 (evidence: [T04-S019, T04-S020])
  - **规则刚性引发绕行**：「不许动利润账户」的硬规定在真实资金紧张时要么被违反、要么导致次优决策（例如该进的货不进），有从业者称之为把企业长期困在急救分诊模式 (evidence: [T04-S019, T04-S020])
  - **推荐比例是拍脑袋的**：目标分配百分比按营收档位给定，缺乏跨行业实证支撑
  - **结论（不和稀泥）**：它是一套**有效的行为工具、不合格的财务分析框架**。对现金持续失控且不看报表的微型企业价值最高；对已经有像样管理会计的企业，它提供的信息量低于一份正经的滚动现金预测 (evidence: [T04-S019, T04-S020])
- **替代品**: Crabtree《Simple Numbers》（同样面向小企业主，但用真实管理会计口径）
- **可信度**: medium（作为行为工具 high，作为财务框架 low） · **Decay risk**: low

---

### 📖 8. Venture Deals: Be Smarter Than Your Lawyer and Venture Capitalist

- **Author**: Brad Feld, Jason Mendelson（Foundry Group）
- **Year**: 2011 初版 / **4th Edition 2019**（Wiley）
- **Type**: 条款与谈判手册
- **难度**: 进阶
- **它立了什么规矩**：把创业融资条款从「律师黑话」翻译成创始人能读的语言，并立下一条至今被反复引用的判断规矩——**每张 term sheet 都是两场谈判叠在一起：经济（economics）与控制（control）**。经济看估值与清算优先权，控制看董事会、保护性条款、投票门槛。创始人容易只盯估值（因为那是唯一能拿出去说的数字），而成熟投资人往往更在意控制与下行保护 (evidence: [T04-S016, T04-S036])
- **核心论点**：① 估值只是经济条款之一，清算优先权可能比估值更决定你最终拿多少；② 控制条款的杀伤力在坏结果时才显现；③ 认识对方的动机结构（GP/LP、基金周期）比背条款更有用；④ 稀释是多轮累积的，要按退出情景倒推而不是逐轮看 (evidence: [T04-S016, T04-S036])
- **读完得到什么**：拿到 term sheet 能自己分出「哪几条影响我最终拿多少钱、哪几条影响我还能不能做主」，并知道哪些条款值得换、哪些不该让
- **Endorsement evidence**：
  - `[figure_long]` 两位作者是 Foundry Group 合伙人；本书直接源自 2005 年起在 feld.com 连载的 term sheet 系列，作者自述该系列被 100 多位教授用于创业课程，书与博客互为一手 (evidence: [T04-S062, T04-S016])
  - `[course_syllabus]` 被创业课程与加速器作为融资模块标准读物，并被 O'Reilly 技术教育平台收录第 4 版 (evidence: [T04-S036, T04-S074])
  - `[blog_secondary]` 被创业金融与债权融资机构作为向创始人推荐的入门书公开书评 (evidence: [T04-S036])
- **局限 / 被批评之处**：
  - **视角仍是美国 VC 生态**：SAFE/可转债、特拉华公司法、优先股结构与中国境内的人民币基金、对赌（估值调整机制）、回购条款差异巨大，中国创始人不能直接套用 (evidence: [T04-S036])
  - **作者是投资人**：书自称站在创始人一侧，但作者的利益结构决定了对某些行业惯例（如优先清算权本身的合理性）批判力度有限；对「优先权如何系统性高估估值」的量化结论要另找学术来源 (evidence: [T04-S034])
  - **版本时效**：第 4 版 2019，之后的条款环境（下行周期中结构化条款回潮、多倍优先权与棘轮重现）需要用近期一手材料补
- **配套必读**: Gornall & Strebulaev 的独角兽估值论文——它用模型证明了 Feld/Mendelson 口头警告的那件事 (evidence: [T04-S034])
- **可信度**: high · **Decay risk**: medium（条款环境随周期变化）

---

### 📖 9. Financial Shenanigans: How to Detect Accounting Gimmicks & Fraud in Financial Reports

- **Author**: Howard M. Schilit, Jeremy Perler, Yoni Engelhart
- **Year**: 1993 初版 / **Fourth Edition 2018**（McGraw-Hill）
- **Type**: 取证式财报分析
- **难度**: 进阶
- **它立了什么规矩**：立了一套**分类学**——把财报粉饰归入几大类（收入操纵、费用操纵、现金流操纵、关键指标操纵），每类下面列出可识别的具体手法与预警信号。它让「看财报」从被动阅读变成**主动质询**：不是问「这家公司赚了多少」，而是问「如果他们想让这个数字好看，最省力的做法是什么，痕迹会留在哪」。第 4 版新增了两条重要的规矩：**现金流量表同样可以被操纵**（不是安全区），以及**并购是掩盖主业恶化的常用手段** (evidence: [T04-S015])
- **核心论点**：① 激励结构决定粉饰概率，先看管理层薪酬与业绩压力；② 应收账款、存货、递延收入与经营现金流的背离是最稳定的预警组合；③ 公司自定义的「关键指标」（非公认会计准则指标）是新的重灾区；④ 并购后的口径变更是最难追的一类 (evidence: [T04-S015, T04-S011])
- **读完得到什么**：拿到一份报表能在半小时内列出 5–10 个需要追问的异常点，并知道每个异常点对应哪种手法
- **Endorsement evidence**：
  - `[figure_long]` 作者创办 Schilit Forensics，曾就财务舞弊议题在美国国会与 SEC 作证，是该领域公认的一手实践者 (evidence: [T04-S015])
  - `[course_syllabus]` McGraw-Hill 高教线在售并持续改版，被财务分析与审计课程采用 (evidence: [T04-S015])
  - `[figure_short]` 获多位专业投资机构负责人具名推荐（如 Tiger Global 的 Chase Coleman） (evidence: [T04-S015])
- **局限 / 被批评之处**：
  - **全部案例是上市公司事后复盘，存在后见之明偏差**：知道结局再回看，信号总是清晰的；对未爆雷公司的误报率（false positive）书中没有讨论 (evidence: [T04-S015])
  - **对中小企业主的直接用途有限**：多数手法需要多期公开报表与同业对照，非上市公司拿不到这些数据
  - **不覆盖中国特有的粉饰形式**（关联交易与体外循环、发票与收入的税务耦合、两套账），中国读者需配张新民的资产/利润质量体系 (evidence: [T04-S038])
  - 只教识别，不教「识别之后怎么办」（尽调、议价、退出）
- **如果只读 1 章**: 现金流操纵那一部分——它推翻了「现金流不会说谎」这个最流行的误解
- **可信度**: high · **Decay risk**: low（手法分类稳定）/ medium（案例与准则细节会旧）

---

### 📖 10. The Outsiders: Eight Unconventional CEOs and Their Radically Rational Blueprint for Success

- **Author**: William N. Thorndike, Jr.
- **Year**: 2012（Harvard Business Review Press）
- **Type**: 案例研究 / 资本配置
- **难度**: 入门 → 进阶
- **它立了什么规矩**：把 **CEO 的第一职责重新定义为资本配置（capital allocation）而不是经营管理**。书里八位 CEO 的共同点是：极度分权的经营 + 极度集权的资金决策；在自家股票便宜时大规模回购、贵时发股换资产；对分红与「行业惯例」毫无敬意；用**每股价值增长**而不是营收规模或市场份额作为唯一记分牌 (evidence: [T04-S021, T04-S007])
- **核心论点**：① 现金的五个去处（内部投资、并购、分红、回购、还债）之间的选择才是长期收益的主要来源；② 分母（股份数）和分子一样重要；③ 逆周期动作是超额收益的主要来源；④ 会计利润不是目标，每股自由现金流才是 (evidence: [T04-S007, T04-S013])
- **读完得到什么**：把「这笔钱该往哪放」变成一个可以每季度显式回答的问题，而不是默认扩张
- **Endorsement evidence**：
  - `[figure_long]` 巴菲特在 2012 年致股东信中公开推荐，称其为关于资本配置卓越 CEO 的杰出著作 (evidence: [T04-S013, T04-S021])
  - `[conf_citation]` Mauboussin 的 Counterpoint Global 资本配置研究与本书同框讨论，把案例观察升级为跨公司统计 (evidence: [T04-S007])
  - `[blog_secondary]` 长期出现在价值投资与公司治理阅读清单，并被投资人公开逐案复盘 (evidence: [T04-S021])
- **局限 / 被批评之处**：
  - **幸存者偏差是最主要且被公开点名的批评**：只研究了极度成功的八位，没有对照组——用同样打法失败的公司有多少，书中不讨论，因此无法证明这套做法提高了成功概率 (evidence: [T04-S021])
  - **回购的适用条件被读者简化**：只有在股价低于内在价值时回购才创造价值；书出版后回购被大量滥用为托市与 EPS 管理工具，这层反例本书没有覆盖 (evidence: [T04-S007])
  - **杠杆的角色被弱化**：多个案例中的超额收益部分来自积极使用债务，在利率环境不同的时期风险截然不同
  - 对中小企业主的直接迁移有限：书中的主要工具（公开市场回购、大额换股并购）需要资本市场准入
- **配套必读**: Mauboussin《Capital Allocation》——补上统计证据与失败案例 (evidence: [T04-S007])
- **可信度**: medium-high（观察 high，因果推断 medium） · **Decay risk**: low

---

### 📖 11. Berkshire Hathaway 致股东信（尤其 1986 年信及其附录）

- **Author**: Warren E. Buffett
- **Year**: 1977–至今；本条重点为 **1986 年信的附录**「Purchase-Price Accounting Adjustments and the 'Cash Flow' Fallacy」
- **Type**: 连载一手文本（可全部免费获取）
- **难度**: 进阶
- **它立了什么规矩**：给出了 **owner earnings（业主收益）** 的定义——**报告净利 + 折旧摊销等非现金费用 − 维持现有竞争地位与产量所必需的资本开支（以及必要的营运资金增加）**。这一定义立的规矩是：**折旧是真实的费用，而维持性资本开支不能不算**。因此他直接点名批评了把 EBITDA（或当年华尔街说的「cash flow」）当作盈利能力代表的做法：那等于假装设备不会磨损、不用更新 (evidence: [T04-S013])
- **核心论点**：① 会计准则下的利润与「股东实际能拿走的钱」是两回事；② 维持性资本开支与扩张性资本开支必须分开，前者是费用性质的；③ owner earnings 不精确但方向正确，胜过精确但错误的 EBITDA；④ 商誉与购买法调整会系统性扭曲被并购业务的表观盈利 (evidence: [T04-S013])
- **读完得到什么**：拿到任何一家公司的报表，能自己算一个「这门生意每年真正能给股东留下多少钱」的数，并说清哪部分资本开支是维持性的
- **Endorsement evidence**：
  - `[figure_long]` 作者本人在同一封信中完整推导并用 Scott Fetzer 收购做示范，是概念的原始出处 (evidence: [T04-S013])
  - `[conf_citation]` owner earnings 已成为价值投资与资本配置文献的标准词汇，并被 Mauboussin 的自由现金流/ROIC 框架继承 (evidence: [T04-S006, T04-S007])
  - `[blog_secondary]` 被大量估值教学材料作为 EBITDA 批判的原始引文反复引用 (evidence: [T04-S013])
- **局限 / 被批评之处**：
  - **维持性资本开支无法客观测量**：Buffett 自己承认这一项只能估计；不同分析师对同一家公司会算出差异很大的 owner earnings，这使它不可审计、不可比较 (evidence: [T04-S013])
  - **对成长期与轻资产公司区分度低**：当维持性与扩张性资本开支高度混合（软件研发、获客投入）时，定义本身失效
  - **信件形式非系统教材**：观点分散在四十多年的文本里，缺乏结构，读者容易只取金句不取推导
  - **不是中小企业操作手册**：语境是控股型企业集团的资本配置，直接迁移到十几人公司会失真
- **如果只读 1 章**: 1986 年信的附录（篇幅短，是 owner earnings 与 EBITDA 批判的原文出处）
- **可信度**: high（一手原文） · **Decay risk**: low

---

### 📖 12. Accounting for Value

- **Author**: Stephen H. Penman
- **Year**: 2011（Columbia University Press）
- **Type**: 学术专著 / 估值方法论
- **难度**: 高阶
- **它立了什么规矩**：这本书立的是一条**反规矩**——它主动放下现代金融的一套工具（资本成本估计、CAPM、DCF），主张**用会计本身来锚定价值**：账面价值是已知的锚，价值来自会计利润相对账面的超额部分，估值应当从「你已经知道什么」出发，而不是从「你需要预测什么」出发。它给出的行动纪律是 anchor on what you know（锚定已知），把推测放在最后，并显式区分「市场价格里已经隐含了多少增长预期」 (evidence: [T04-S022, T04-S024])
- **核心论点**：① 会计与估值本质是同一件事；② DCF 把权重压在最不可知的远期与不可观测的资本成本上，因而脆弱；③ 投资阶段的现金流为负，DCF 的中间数难以解释，而权责发生制正是为解决这个问题发明的；④ 应当反推市场价格隐含的增长率并评判其合理性 (evidence: [T04-S022, T04-S024])
- **读完得到什么**：一套不依赖折现率估计的估值路径；以及一个更重要的习惯——**先问价格里已经含了什么预期，再决定要不要下注**
- **Endorsement evidence**：
  - `[course_syllabus]` 由 Columbia University Press / Columbia Business School Publishing 出版，作者是哥大会计学讲席教授，配套其《Financial Statement Analysis and Security Valuation》教材长期用于研究生课程 (evidence: [T04-S022])
  - `[conf_citation]` 学术期刊 Accounting, Economics, and Law 就本书组织了专门的评论文章，说明其在学界引发了正式辩论 (evidence: [T04-S024])
  - `[figure_long]` 作者在长篇访谈中系统阐述内在价值、盈余质量与资本成本立场，与书形成互证 (evidence: [T04-S022])
- **局限 / 被批评之处**：
  - **门槛高**：需要读者已经熟悉权责发生制与剩余收益模型，对中小企业主基本不可直接读
  - **对会计质量的依赖是双刃剑**：整个方法建立在「会计数字可信」之上，而会计本身可被操纵——遇到 Schilit 书里那类粉饰，锚点本身就是坏的 (evidence: [T04-S015])
  - **学界评议指出其立场的张力**：一边声称遵守金融理论原则，一边又从基本面视角对这些原则做了整体重释，两者是否自洽存在争论 (evidence: [T04-S024])
  - 对早期、无盈利、无稳定账面价值的创业公司几乎无用
- **可信度**: high · **Decay risk**: low

---

### 📖 13. 《一本书读懂财报》（修订版）

- **Author**: 肖星（清华大学经济管理学院会计系教授）
- **Year**: 2014 初版 / 修订版（浙江大学出版社）
- **Type**: 中文财报入门
- **难度**: 入门
- **它立了什么规矩**：在中文语境里把「看财报」从**背科目**改成**追一条业务链**：企业拿钱（融资）→ 花钱（投资）→ 赚钱（经营）→ 分钱，三张表分别记录这条链的不同侧面。它立的核心规矩是**三张表必须联起来读**，并给出中文读者最需要的那句判断：**利润表看能力，资产负债表看家底，现金流量表看死活**。它同时把「财务分析是为了做决策，不是为了做账」这条立场带进了大众读者 (evidence: [T04-S014, T04-S037])
- **核心论点**：① 报表是经营活动的镜像，读表就是还原业务；② 资产的质量比资产的金额重要；③ 现金流量表的三个部分组合形态直接反映企业所处阶段；④ 比率分析必须结合行业与商业模式，脱离业务的比率无意义 (evidence: [T04-S014])
- **读完得到什么**：能独立读懂一份中国 A 股公司或自家公司的报表，并说出这家公司处在什么阶段、钱从哪来到哪去
- **Endorsement evidence**：
  - `[course_syllabus]` 本书是学堂在线国家精品课《财务分析与决策》的配套参考书，课程与书互为一手 (evidence: [T04-S014])
  - `[figure_long]` 作者为清华经管会计系教授，长期主讲财务分析与决策、会计理论及中国资本市场会计问题，并有配套音频课 (evidence: [T04-S014])
  - `[blog_secondary]` 自 2014 年出版后长期位居中文经管畅销榜与电子书会计类前列，并出修订版 (evidence: [T04-S014])
- **局限 / 被批评之处**：
  - **深度有限**：定位是入门，合并报表、递延所得税、金融工具、收入确认判断这些真正难的部分基本不展开；读完只能看懂表，还看不出粉饰
  - **案例以 A 股上市公司为主**，非上市中小企业的实际问题（两套账、老板与公司资金混同、股东借款）不涉及
  - **与准则更新的同步性**：新收入准则、新租赁准则实施后的表述细节需要读者自行对照财政部原文核对 (evidence: [T04-S012, T04-S045])
- **配套**: 学堂在线《财务分析与决策》公开课（同作者）
- **可信度**: high · **Decay risk**: medium（准则细节）

---

### 📖 14. 《财务报表分析》（第 6 版）与「财务状况质量分析」体系

- **Author**: 张新民（对外经济贸易大学）、钱爱民
- **Year**: 第 5 版 2019 / **第 6 版 2023**（中国人民大学出版社）；配套通俗版《从报表看企业》
- **Type**: 中文教材 + 分析体系
- **难度**: 进阶
- **它立了什么规矩**：在中文财务分析里建立了一套区别于西方比率分析的框架——**「财务状况质量」分析**：不只问数字大小，而是逐块问质量：**资产质量、利润质量、资本结构质量、现金流量质量**。它立的规矩是：**同样的数字，质量可以完全不同**——一亿元应收账款和一亿元现金都是资产，但前者的质量取决于能不能收回；一千万利润里有多少来自主业、有多少来自处置资产与政府补助，决定了这个利润能不能重复 (evidence: [T04-S037, T04-S038])
- **核心论点**：① 资产的本质是「未来能带来经济利益的资源」，不能带来的就应视为质量差甚至虚增；② 利润质量看构成与可持续性，不看金额；③ 资本结构质量看的是期限匹配与实际控制关系；④ 战略决定报表结构，报表结构反过来暴露战略 (evidence: [T04-S037, T04-S038])
- **读完得到什么**：能对一家中国公司做出「这家公司的家底是真是假、利润能不能重复、资金链紧不紧」的结构化判断
- **Endorsement evidence**：
  - `[course_syllabus]` 作者在中国大学 MOOC 开设《财务报表分析》公开课，与教材配套 (evidence: [T04-S037])
  - `[course_syllabus]` 教材由中国人民大学出版社连续改版至第 6 版，长期作为国内高校财务报表分析课程教材 (evidence: [T04-S038])
  - `[blog_secondary]` 通俗版《从报表看企业》连续出到第 4 版，说明体系在非学术读者中同样被采用 (evidence: [T04-S038])
- **局限 / 被批评之处**：
  - **「质量」的判定含较多主观标准**：哪些资产算「质量差」在不同行业差异极大，体系提供分类但不提供阈值，落地依赖分析者经验
  - **强绑定中国上市公司披露格式**，对小微企业（按《小企业会计准则》编报、披露信息少）适配度低 (evidence: [T04-S048])
  - **教材形态**：结构完整但篇幅大、读起来慢，创业者通常只能通过通俗版进入
  - 与国际准则（IFRS）的差异处理散落在各章，跨境业务读者需另行补 IFRS 原文 (evidence: [T04-S009, T04-S010])
- **可信度**: high · **Decay risk**: medium（准则与披露格式更新）

---

### 边缘 / 降级候选（记录判断，不进必读）

| 候选 | 判定 | 理由 |
|------|------|------|
| Berman & Knight《Financial Intelligence for Entrepreneurs》 | **合并进 #1** | 与主书重叠度高，创业者版主要是案例替换，不构成独立 canon (evidence: [T04-S001]) |
| Berk & DeMarzo《Corporate Finance》 | **降级为替代品** | 与 Brealey/Myers 定位重合，教学法更好但未改变行业思考方式 (evidence: [T04-S025]) |
| Graham & Dodd《Security Analysis》 | **出界** | 属二级市场投资分析，落在本次「明确排除」范围内 |
| 各类「财报速成 / 30 天精通」类中文畅销书 | **DROP** | 无独立 endorsement，多为 SEO 与营销驱动 |

---

---

## 二、准则与规则原文（当作 canon 的一部分）

> 为什么准则要算 canon：对创业者与中小企业主而言，准则不是用来背的，是**判断空间的边界地图**。你能不能确认这笔收入、租的办公室要不要上表、把这笔支出资本化还是费用化——决定了你的报表长什么样、银行怎么看你、投资人怎么算你的估值。会计准则真正的用处是让你知道「哪里有选择权」。
> **注意**：本节是结构化索引与判断要点，不是准则条文复制。具体条文以下列官方链接为准。

---

### 📜 A. IFRS 15 / ASC 606 — 收入（Revenue from Contracts with Customers）

- **发布机构 / 官方 URL**：IASB — https://www.ifrs.org/issued-standards/list-of-standards/ifrs-15-revenue-from-contracts-with-customers/ ｜ FASB（ASC 606）— https://www.fasb.org/standards (evidence: [T04-S009, T04-S044])
- **它立了什么规矩**：把全球的收入确认统一到**一套五步法**：识别合同 → 识别单项履约义务 → 确定交易价格 → 把价格分摊到各项履约义务 → 在履约时（或期间内）确认收入。IFRS 与 US GAAP 在这一议题上高度趋同，这是两大准则体系罕见的联合成果 (evidence: [T04-S009, T04-S057])
- **创业者最该记住的判断**：
  - **收到钱 ≠ 确认收入**。预收的年费属于**合同负债（递延收入）**，随服务提供逐期转入收入——SaaS / 会员制 / 预付卡业务的报表全都由这条决定 (evidence: [T04-S057])
  - **一份合同里有几件事要做**，就可能要拆成几项履约义务分别确认（软件 + 实施 + 售后支持）
  - **可变对价**（返利、折扣、里程碑）要按预期计入，且受「极可能不发生重大转回」的限制约束
  - **本人 vs 代理人（principal vs agent）**判断决定你按总额还是净额确认收入——平台型/撮合型生意的营收规模在这一判断上可以差十倍 (evidence: [T04-S057])
- **中国对应**：CAS 14《收入》2017 年修订，明确目的就是与 IFRS 15 保持趋同；实施分三批（境内外同时上市及境外上市用 IFRS 的自 2018-01-01；其他境内上市自 2020-01-01；执行企业会计准则的非上市企业自 2021-01-01） (evidence: [T04-S066, T04-S067])
- **争议 / 实务痛点**：五步法把大量判断交回给管理层（履约义务拆分、独立售价估计、时点 vs 时段），因此**它同时是最强的统一器和最大的操纵空间来源**；Schilit 书中收入操纵一类的多数手法就发生在这些判断点上 (evidence: [T04-S015, T04-S009])

---

### 📜 B. IFRS 16 — 租赁（Leases）

- **发布机构 / 官方 URL**：IASB — https://www.ifrs.org/issued-standards/list-of-standards/ifrs-16-leases/ (evidence: [T04-S010])
- **它立了什么规矩**：**消灭了「经营租赁」的表外藏身处**。承租人对几乎所有租赁都要在资产负债表上同时确认**使用权资产**与**租赁负债**；利润表上原来的一笔租金费用被拆成**折旧 + 利息**两部分 (evidence: [T04-S010, T04-S058])
- **创业者最该记住的判断**：
  - 签一份五年办公室租约，**资产负债表会立刻变胖、负债率会跳升**——如果你有基于负债率的银行契约（covenant），这可能直接触发违约，签约前必须算
  - 因为租金被拆成折旧+利息，**EBITDA 会系统性变好看**（租金不再全额扣在 EBITDA 之上），跨准则期比较 EBITDA 是无效的 (evidence: [T04-S058, T04-S010])
  - 短期租赁（≤12 个月）与低价值资产有豁免选项，是中小企业的实际减负口
- **中国对应**：CAS 21《租赁》相应修订，与 IFRS 16 趋同 (evidence: [T04-S067])
- **争议**：批评者指出，把所有租赁资本化提高了可比性，但也让**没有实质差别的两家公司（一家买、一家租）报表更像了却掩盖了融资弹性的真实差异**；同时增加了中小企业的执行成本，这是 IFRS for SMEs 保留简化处理的原因之一 (evidence: [T04-S061, T04-S058])

---

### 📜 C. IFRS 18 — 财务报表列报与披露（Presentation and Disclosure）

- **发布机构 / 官方 URL**：IASB — https://www.ifrs.org/issued-standards/list-of-standards/ifrs-18-presentation-and-disclosure-in-financial-statements/ (evidence: [T04-S008])
- **发布与生效**：2024 年 4 月 9 日发布，**对 2027 年 1 月 1 日或之后开始的年度期间生效**，允许提前适用；取代 IAS 1 (evidence: [T04-S008, T04-S059, T04-S072])
- **它立了什么规矩**：三件事——
  1. **规定利润表的结构**：损益按经营 / 投资 / 融资分类，并强制列示两个新的小计（营业利润；以及融资与所得税前的损益），终结了各家自定义损益表结构的局面 (evidence: [T04-S059, T04-S072])
  2. **把「管理层自定义业绩指标」（management-defined performance measures, MDPM）拉进审计范围**：公司若在报表外沟通中使用调整后利润这类指标，必须在附注中披露定义、与准则小计的调节表，并说明为什么管理层认为它有用 (evidence: [T04-S008, T04-S059])
  3. **加强汇总与拆分（aggregation / disaggregation）的原则**，减少「其他」这个大口袋 (evidence: [T04-S059])
- **为什么对创业者重要**：这是准则制定者第一次正面处理**「调整后 EBITDA 满天飞」**这个问题。方向与 SEC 的 Reg G 一致：不禁止你用自定义指标，但要求你**公开定义、公开调节、承担责任** (evidence: [T04-S008, T04-S011])
- **争议**：企业侧普遍反映实施成本高（要重排损益表、重建披露流程、追溯比较期）；同时有观点认为把 MDPM 纳入财报可能反而**给自定义指标背书**，让它们显得更权威 (evidence: [T04-S059, T04-S072])

---

### 📜 D. SEC Regulation G / Item 10(e) of Regulation S-K — 非公认会计准则财务指标

- **发布机构 / 官方 URL**：SEC 最终规则 https://www.sec.gov/rules/final/33-8176.htm ｜ 法规原文 17 CFR Part 244 https://www.ecfr.gov/current/title-17/chapter-II/part-244 ｜ 工作人员解释（C&DI）https://www.sec.gov/rules-regulations/staff-guidance/corporation-finance-interpretations/non-gaap-financial-measures (evidence: [T04-S060, T04-S043, T04-S011])
- **它立了什么规矩**：**你可以用非公认会计准则指标，但必须同时给出最直接可比的 GAAP 指标，并提供调节表；且不得具有误导性。** Item 10(e) 进一步规定在向 SEC 报送的文件中，GAAP 指标不得被自定义指标的显著性压过 (evidence: [T04-S011, T04-S043])
- **执法口径中最有教育意义的几条**：
  - 把一项费用标为「非经常性 non-recurring」但**过去两年内发生过类似费用**（如把法律费用剔出调整后 EBITDA），可能构成误导性调整 (evidence: [T04-S011])
  - 调整后 EBITDA 若剔除现金支出项，一般不得作为业绩指标使用；只有在与信贷协议重大契约挂钩、并在 MD&A 流动性讨论中呈现时才有有限例外 (evidence: [T04-S011])
  - 常见受关注的指标：EBITDA、adjusted EBITDA、adjusted gross margin、adjusted net income、adjusted EPS、free cash flow (evidence: [T04-S011])
- **为什么创业者要懂（哪怕不上市）**：你给投资人和银行看的「调整后 EBITDA」用的就是同一套逻辑。SEC 的规则等于给了你一份**免费的、被执法检验过的清单**，告诉你哪些调整会被专业读者视为不诚实 (evidence: [T04-S011, T04-S060])

---

### 📜 E. 中国企业会计准则（CAS）与《小企业会计准则》

- **发布机构 / 官方 URL**：财政部会计司准则专题 https://kjs.mof.gov.cn/zt/kjzzss/ ｜具体准则目录 https://kjs.mof.gov.cn/zt/kjzzss/qykjzz/ ｜实施问答 https://kjs.mof.gov.cn/zt/kjzzss/kuaijizhunzeshishiwenda/ (evidence: [T04-S012, T04-S067, T04-S045])
- **两套体系并存，这是中国中小企业最该先搞清的一件事**：
  - **《企业会计准则》（CAS）**：基本准则 + 一系列具体准则，总体与 IFRS 趋同，适用于上市公司与规模较大企业
  - **《小企业会计准则》**（财会〔2011〕17 号，2011-10-18 发布，**2013-01-01 起施行**）：适用于境内依法设立、符合《中小企业划型标准规定》小型企业标准的企业；**明确排除三类**——股票或债券公开交易的小企业、金融机构或具金融性质的小企业、企业集团内的母公司与子公司；取代原《小企业会计制度》（财会〔2004〕2 号） (evidence: [T04-S048])
- **它立了什么规矩**：**给小企业一条合法的简化路径**——大幅减少公允价值计量与复杂判断，多数项目用历史成本、与税法口径尽量靠拢，目的是降低小企业的核算成本
- **创业者最该记住的判断**：
  - 选哪套准则**不是会计部门的技术选择，是战略选择**：打算融资、引入外部投资人或未来上市的，应尽早按 CAS 建账；否则转换成本会在最不该出问题的时候爆发
  - 《小企业会计准则》与税法靠拢**减少了税会差异带来的麻烦**，但也意味着报表的经济含义被弱化（如资产减值、公允价值信息缺失）
  - 「实施问答」是财政部对具体争议的官方口径，比任何培训机构的解读都更权威 (evidence: [T04-S045])
- **国际对应物**：IFRS for SMEs 是 IASB 给中小企业的简化版全套准则，思路相同（降低成本、减少判断），可作为对照阅读 (evidence: [T04-S061])

---


---

## 三、论文 / 研究 / 免费数据集

---

### 📄 1. The Cost of Capital, Corporation Finance and the Theory of Investment（MM 定理）

- **Authors**: Franco Modigliani, Merton H. Miller
- **Venue + Year**: American Economic Review, Vol. 48, No. 3, June 1958, pp. 261–297
- **URL**: https://www.jstor.org/stable/1809766 (evidence: [T04-S027])
- **核心 idea**: 在无税、无破产成本、信息对称的完美市场里，**企业价值与其资本结构无关**——怎么切蛋糕不改变蛋糕大小。加入公司税后，负债因利息税盾产生价值增量 (evidence: [T04-S027])
- **为什么经典**: 现代公司金融的起点；两位作者后来均获诺贝尔经济学奖；它首次用**无套利论证**处理公司金融问题，这套方法论后来统治了整个领域 (evidence: [T04-S027, T04-S025])
- **这行的人用它来判断什么**：**倒过来用**。既然理论说「在理想条件下资本结构不重要」，那现实中资本结构之所以重要，一定是因为某个前提被打破了——是税？是破产成本？是信息不对称？是控制权？**先定位是哪一条，再谈融资方案**，这是它给实务的真正价值 (evidence: [T04-S025, T04-S029])
- **常见误用**: 把结论简化成「负债多少无所谓」。对中小企业尤其危险——它们面对的正是最高的破产成本与最严重的信息不对称，MM 的前提几乎全不成立 (evidence: [T04-S029])
- **可信度**: high · **Decay risk**: low

---

### 📄 2. Corporate Financing and Investment Decisions When Firms Have Information That Investors Do Not Have（融资优序 pecking order）

- **Authors**: Stewart C. Myers, Nicholas S. Majluf
- **Venue + Year**: Journal of Financial Economics, 13(2), 1984, pp. 187–221；配套 Myers《The Capital Structure Puzzle》(Journal of Finance, 1984)
- **URL**: https://www.sciencedirect.com/science/article/abs/pii/0304405X84900230 ｜免费工作论文版 https://www.nber.org/papers/w1396 ｜配套 https://onlinelibrary.wiley.com/doi/10.1111/j.1540-6261.1984.tb03646.x (evidence: [T04-S029, T04-S030, T04-S028])
- **核心 idea**: 管理层比外部投资者更了解公司真实价值，因此**发新股会被市场解读为「管理层觉得股价偏高」**，进而压低股价。结果企业形成融资偏好顺序：**内部留存 > 债务 > 股权**；极端情况下企业宁可放弃有价值的投资项目也不发股 (evidence: [T04-S029, T04-S064])
- **谱系**: 优序思想最早由 Gordon Donaldson 1961 年提出，Myers & Majluf 1984 给出了信息不对称的理论机制 (evidence: [T04-S064])
- **这行的人用它来判断什么**：**融资顺序本身在传递信号**。创始人主动大额稀释，市场默认你在高位卖；反之能用留存和债务做的事却去发股，需要一个解释。同时它解释了为什么「有现金储备（financial slack）」本身有价值——它让你在不发信号的情况下抓住机会 (evidence: [T04-S029])
- **争议 / 后续**: 大量实证检验发现优序理论对小型、高成长公司的解释力较弱（这些公司恰恰最依赖股权融资），学界对优序 vs 权衡理论（trade-off theory）孰优至今未定论 (evidence: [T04-S064, T04-S028])
- **可信度**: high · **Decay risk**: low

---

### 📄 3. Measure Costs Right: Make the Right Decisions（作业成本法 ABC 的奠基）

- **Authors**: Robin Cooper, Robert S. Kaplan
- **Venue + Year**: Harvard Business Review, September 1988
- **URL**: https://hbr.org/1988/09/measure-costs-right-make-the-right-decisions (evidence: [T04-S031])
- **核心 idea**: 传统按人工工时或产量分摊间接费用的做法，在间接费用占比越来越高的年代会**系统性地扭曲产品成本**——高产量标准品被多摊，低产量定制品被少摊。应改为先识别「作业（activity）」，再按各产品实际消耗的作业量分摊成本 (evidence: [T04-S031])
- **为什么经典**: 它把「我们到底哪个产品赚钱」从一个会计问题变成了战略问题，直接引出了产品线砍留、定价与客户分层的决策方式；此后管理会计教材普遍设 ABC 章节 (evidence: [T04-S031, T04-S032])
- **这行的人用它来判断什么**：当你怀疑「明明整体有利润，但不知道钱是哪块赚的、哪块亏的」时，先问间接费用是怎么分摊的。**分摊口径错了，所有产品毛利都是错的，定价与砍产品线的决策必然错**
- **争议 / 失败率（必须写实）**：
  - **Kaplan 本人在 2004 年公开承认 ABC 落地失败率高**：大规模实施 ABC 的企业「常常在成本上升与员工抵触面前放弃了尝试」；数据采集靠员工填时间比例的问卷，主观、昂贵、难维护 (evidence: [T04-S032])
  - 他随后提出**时间驱动作业成本法（Time-Driven ABC, TDABC）**作为补救：直接估算单位作业的时间与产能成本率，跳过问卷 (evidence: [T04-S032])
  - 更根本的批评是：ABC 提高了成本信息的精度，但**短期内大多数间接成本并不随作业量变化**——按 ABC 算出「不赚钱」而砍掉的产品，砍完后间接费用仍在，只是摊到更少产品上 (evidence: [T04-S032, T04-S031])
  - **对中小企业的现实结论**：完整 ABC 通常不划算；值得借用的是它的**提问方式**（哪些作业真正消耗资源），而不是它的核算系统
- **可信度**: high · **Decay risk**: low（思想）/ medium（实施方法已被 TDABC 更新）

---

### 📄 4. Corporate Budgeting Is Broken—Let's Fix It / Paying People to Lie

- **Author**: Michael C. Jensen
- **Venue + Year**: Harvard Business Review, November 2001；完整论文版《Paying People to Lie: The Truth About the Budgeting Process》
- **URL**: https://hbr.org/2001/11/corporate-budgeting-is-broken-lets-fix-it ｜ https://papers.ssrn.com/sol3/papers.cfm?abstract_id=267651 (evidence: [T04-S039, T04-S068])
- **核心 idea**: 问题不在预算本身，在**把奖金和预算达成率挂钩**。只要奖金是「达标就跳一档」的阶梯式，下级就有动机把目标压低、把业绩虚报，上级也会参与博弈，结果预算里的信息被系统性污染——而预算的本职正是提供无偏信息用于协调 (evidence: [T04-S039, T04-S069])
- **为什么经典**: 它把「预算游戏」从大家心照不宣的潜规则变成了一个有明确机制解释和明确解法的管理问题；并被 The Case Centre 作为教学材料独立发行，进入商学院课堂 (evidence: [T04-S073, T04-S069])
- **解法（Jensen 的主张）**: 不要废掉预算系统，**要改薪酬**——用纯线性的奖金曲线（多做多得、少做少得，没有跳档），消除在目标线附近做手脚的收益 (evidence: [T04-S039, T04-S069])
- **这行的人用它来判断什么**：看到部门年年「刚好完成 101%」，第一反应不是「执行力强」，是**奖金结构在制造这个数字**。做预算前先看奖金怎么发
- **争议**: 线性奖金方案在实务中推行困难（董事会与投资人偏好明确的目标承诺）；Beyond Budgeting 阵营认为 Jensen 的修补还不够——问题出在固定年度目标本身，而不只是薪酬曲线 (evidence: [T04-S033, T04-S069])
- **可信度**: high · **Decay risk**: low

---

### 📄 5. Squaring Venture Capital Valuations with Reality（独角兽估值虚高）

- **Authors**: Will Gornall（UBC）, Ilya A. Strebulaev（Stanford GSB）
- **Venue + Year**: Journal of Financial Economics, 135(1), 2020, pp. 120–143（NBER WP 23895, 2017）
- **URL**: https://www.sciencedirect.com/science/article/abs/pii/S0304405X19301692 ｜免费版 https://www.nber.org/papers/w23895 ｜机构页 https://www.gsb.stanford.edu/faculty-research/publications/squaring-venture-capital-valuations-reality (evidence: [T04-S034, T04-S035, T04-S046])
- **核心 idea**: 媒体报道的「投后估值」是用**最近一轮优先股的每股价格 × 全部股份数**算出来的，这等于假设所有股份和最新一轮优先股一样值钱。但最新一轮往往附带 IPO 回报保证、否决降价 IPO 的权利、优先于其他所有投资人受偿等保护条款——**普通股没有任何这些保护** (evidence: [T04-S034])
- **实证结果（数字要记住）**: 对 135 家美国独角兽建模后，**报告估值平均高于公允价值 48%**，其中 14 家高出 100% 以上；**普通股被高估 56%**；调整后 **135 家中有 65 家失去独角兽身份** (evidence: [T04-S034, T04-S035])
- **样本中的条款分布**: 15% 有 IPO 回报保证，24% 有降价 IPO 否决权，30% 优先于其他所有投资人 (evidence: [T04-S034])
- **这行的人用它来判断什么**：**别把「我们估值 10 亿」当成身价**。要算创始人真正拿到手多少，必须把清算优先权、参与权、棘轮按不同退出金额跑一遍瀑布（waterfall）。这是 Venture Deals 用文字讲的事，这篇论文给了量化证据 (evidence: [T04-S016, T04-S034])
- **可信度**: high · **Decay risk**: low（机制）/ medium（条款分布随周期变化）

---

### 📄 6. Michael Mauboussin 的 ROIC 与资本配置系列（Counterpoint Global Insights）

- **Authors**: Michael J. Mauboussin, Dan Callahan（Morgan Stanley Investment Management, Counterpoint Global）
- **主要篇目 + URL**:
  - *Return on Invested Capital: How to Calculate ROIC and Handle Common Issues*（2022）https://www.morganstanley.com/im/publication/insights/articles/article_returnoninvestedcapital.pdf ｜落地页 https://www.morganstanley.com/im/en-us/individual-investor/insights/consilient-observer/return-on-invested-capital.html (evidence: [T04-S006, T04-S071])
  - *Capital Allocation*（含 1970–2024 长周期数据更新）https://www.morganstanley.com/im/publication/insights/articles/article_capitalallocation.pdf (evidence: [T04-S007])
  - *Everything Is a DCF Model* / *Valuation Multiples* https://www.morganstanley.com/im/publication/insights/articles/article_valuationmultiples.pdf (evidence: [T04-S052, T04-S053])
- **核心 idea**:
  - **ROIC 与资本成本的差（ROIC − WACC）才是价值创造的判据**；增长只有在 ROIC > 资本成本时才创造价值，否则增长在毁灭价值 (evidence: [T04-S006, T04-S070])
  - **投入资本的计算充满口径陷阱**：无形资产投入（研发、品牌、获客）被费用化后不进入投入资本，导致轻资产公司的 ROIC 被系统性高估；租赁、商誉、超额现金的处理同样影响结果 (evidence: [T04-S006])
  - **一切估值本质都是 DCF**：用 EV/EBITDA 倍数不是绕开了 DCF，只是把 DCF 的假设藏进了倍数里——「当价值的绝大部分来自 EV/EBITDA 倍数时，结果只是打扮成 DCF 的倍数分析」 (evidence: [T04-S053, T04-S052])
  - **资本配置有五个去处**（内部投资、并购、分红、回购、还债），评估管理层能力要看历史行为、ROIC、激励结构三者是否一致 (evidence: [T04-S007])
- **这行的人用它来判断什么**：任何「我们要增长」的提议，先问 **这笔投入的预期 ROIC 高不高于资本成本**；不高于就不该做，无论增长多快
- **局限**: 数据与案例以美国上市公司为主；ROIC 口径调整的工作量对中小企业不现实，实务中往往只能做粗略版本 (evidence: [T04-S006])
- **可信度**: high · **Decay risk**: low（框架）/ medium（数据每年更新）

---

### 📊 7. Damodaran Online 免费数据集与公开课（NYU Stern）

- **Host**: Aswath Damodaran, NYU Stern
- **URL**: 主站 https://pages.stern.nyu.edu/~adamodar/New_Home_Page/ ｜数据集 https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datacurrent.html ｜免费估值课 https://pages.stern.nyu.edu/~adamodar/New_Home_Page/webcastvalonline.htm (evidence: [T04-S003, T04-S004, T04-S005])
- **提供什么**: 免费可下载的行业 beta、股权风险溢价、国别风险溢价、各行业利润率 / ROIC / 资本成本 / 倍数，以及估值模型模板；配套 **25 讲 webcast**（每讲约 12–20 分钟）+ 讲义 + 课后测验与答案 (evidence: [T04-S004, T04-S005])
- **Last_updated**: 数据集按年度更新（通常每年 1 月刷新全年数据）；估值 webcast 系列随学期滚动更新。**使用时必须核对页面上的数据年份**——这是本条唯一的高衰减风险点 (evidence: [T04-S004])
- **这行的人用它来判断什么**：给非上市公司估折现率时，用行业无杠杆 beta + 自身资本结构重新加杠杆，比拍脑袋强得多；同时可以用行业中位利润率检验自己的商业计划是否离谱
- **常见误用**: 把 NYU 的行业均值当标准答案直接套用——样本是**美国上市公司**，规模、流动性、议价能力与中小企业完全不同 (evidence: [T04-S004, T04-S040])
- **可信度**: high · **Decay risk**: high（数据必须每年重取）

---

### 📄 8. Beyond Budgeting 的研究与 12 原则

- **Originators**: Jeremy Hope, Robin Fraser, Peter Bunce；Beyond Budgeting Round Table（BBRT，1998 年成立于 CAM-I 下）
- **URL**: https://bbrt.org/ (evidence: [T04-S033])
- **核心 idea**: 传统年度预算把「目标、预测、资源分配」三件本该分开的事捆在一个数字上，导致三者互相污染——目标想定低、预测想报高、资源想多要。Beyond Budgeting 主张**拆开这三件事**：目标改为相对的（对标同业 / 对标上期），预测改为**无偏的滚动预测**（rolling forecast，通常每季度更新，明确不以达成某个数为目的），资源按需动态分配而非年初一次性切分 (evidence: [T04-S033])
- **为什么进入 canon**: 它是「预算无用论」在管理会计里最成体系的一支，与 Jensen 的批评互为补充（Jensen 改薪酬，Beyond Budgeting 改流程）；实践案例集中在北欧与部分大型企业 (evidence: [T04-S033, T04-S039])
- **这行的人用它来判断什么**：当你发现预算会议上大家在讨论「这个数能不能降下来」而不是「客户会不会买」时，就是预算变成了谈判而不是计划——该把目标与预测拆开
- **争议（必须写实）**:
  - **证据基础偏弱**：主要依据是先行企业的案例研究，缺乏严格的对照实证；批评者认为案例选择本身存在幸存者偏差
  - **完全废除预算在多数组织不可行**：董事会、银行契约、监管报送都需要一个明确的年度数字；实务中落地的通常是折中版（保留预算 + 加滚动预测 + 解绑奖金）
  - **滚动预测本身会被游戏化**：如果它仍然影响资源分配和评价，做预测的人一样有动机报偏 (evidence: [T04-S039, T04-S069])
- **可信度**: medium-high · **Decay risk**: low

---

### 📄 9. A Cash Conversion Cycle Approach to Liquidity Analysis（现金转换周期的出处）

- **Authors**: Verlyn D. Richards, Eugene J. Laughlin
- **Venue + Year**: Financial Management, 9(1), 1980, pp. 32–38
- **URL**: https://www.semanticscholar.org/paper/A-Cash-Conversion-Cycle-Approach-to-Liquidity-Richards-Laughlin/6f0a861d27e59ce73f8b8207121e52980248a0c2 (evidence: [T04-S047])
- **核心 idea**: 传统的流动比率、速动比率是**静态的清算视角**（假设公司要停业变现），无法反映持续经营下资金的循环速度。应改用**动态的现金转换周期**：CCC = 存货周转天数 DIO + 应收账款周转天数 DSO − 应付账款周转天数 DPO (evidence: [T04-S047])
- **为什么经典**: 它把流动性分析从「有没有资产可变现」改成「钱转一圈要多久」，这是今天所有营运资金管理的基础语言
- **这行的人用它来判断什么**：**现金转换周期直接决定你的增长需要多少外部资金**。CCC 为正且很长（先付货款、慢收账）的生意，每增长一块钱营收就要垫一笔钱，增长越快越缺现金；CCC 为负的生意（预收款、先收后付，如订阅制、部分零售）**靠增长自己产生现金** (evidence: [T04-S047, T04-S049])
- **可信度**: high · **Decay risk**: low

---

### 📄 10. SaaS Metrics 2.0 / SaaS 现金流低谷（创业单位经济学的事实标准）

- **Author**: David Skok（Matrix Partners）
- **URL**: https://www.forentrepreneurs.com/saas-metrics-2/ ｜ https://www.forentrepreneurs.com/saas-economics-1/ (evidence: [T04-S042, T04-S049])
- **Type**: 长篇博客系列（非学术论文，但在创业财务圈的地位等同 canon）
- **核心 idea**:
  - **SaaS 现金流低谷（cash flow trough）**：获客成本 CAC 在前期一次性付出，而收入按月摊回，因此**每获得一个客户在回本前都是净流出**。结论反直觉但极其重要——**增长越快，现金流看起来越差**，亏损扩大不一定意味着生意变坏 (evidence: [T04-S049])
  - **CAC 回收期（months to recover CAC）**通常应控制在 12 个月以内；LTV/CAC 与回收期共同构成单位经济的判据 (evidence: [T04-S049, T04-S042])
- **为什么进入 canon**: 它给了订阅制创业者一套统一的财务语言（CAC、LTV、churn、回收期、低谷深度），这套词汇现在是投资人与创始人对话的默认协议 (evidence: [T04-S042])
- **这行的人用它来判断什么**：看到烧钱不要先问「为什么亏」，要问「**这是低谷还是无底洞**」——把单客户经济拆出来，如果单客户能回本且回本期可接受，亏损是增长的代价；如果单客户永远不回本，规模只会放大亏损
- **局限 / 争议**:
  - LTV 的计算依赖流失率假设，早期公司样本期太短，**LTV 常被系统性高估**；把高估的 LTV 除以 CAC 得到的比率会给出虚假安全感
  - 框架强绑定订阅制商业模式，对项目制、硬件、渠道分销型生意迁移性差
  - 内容主体成文于 2010 年代前中期，指标定义在业界已有分化（如 CAC 是否含客户成功成本），使用时必须先统一口径 (evidence: [T04-S042])
- **Last_updated**: 页面为长期维护的博客文章，核心框架自 2010 年代中期后无重大改写 — 使用时须自行核对口径 (evidence: [T04-S042])
- **可信度**: medium-high · **Decay risk**: medium

---


---

## 四、核心概念（26 个）

> 格式：概念 → 一句话定义 → **这行的人用它来判断什么** → 来源 → 常见误用。
> **tier-1** = 所有创始人/小企业主必懂；**tier-2** = 资深者熟知。
> 注意：这里放的是**概念**，不是黑话缩写（黑话归 Track 06）。

---

| # | 概念 | Tier | 一句话定义 | 这行的人用它来判断什么 | 来源 | 常见误用 |
|---|------|------|-----------|---------------------|------|---------|
| 1 | **权责发生制 vs 收付实现制**（accrual vs cash basis） | tier-1 | 权责发生制按「经济事项发生」记账，收付实现制按「钱到没到」记账 | 判断报表在说什么。看到「盈利但没钱」，先确认是权责口径下的账面利润，还是真有钱 | 会计基本准则；IFRS 概念框架 (evidence: [T04-S012, T04-S009]) | 以为两者一个对一个错；实际上小企业往往两套都要看——利润看权责，死活看收付 |
| 2 | **三张表勾稽** | tier-1 | 利润表的净利进入资产负债表的留存收益，现金流量表解释资产负债表两期现金差额，三表互相锁死 | 判断一份报表是不是伪造的或漏了东西——做不平就一定有问题 | Ittelson《Financial Statements》；肖星《一本书读懂财报》 (evidence: [T04-S056, T04-S014]) | 只看利润表；或把三张表当三个独立报告读 |
| 3 | **营运资金**（working capital） | tier-1 | 流动资产 − 流动负债；日常经营被占用的资金 | 判断增长要垫多少钱。营运资金随营收同比例增长的生意，增长本身就是吞金兽 | 公司金融教科书标准内容 (evidence: [T04-S025]) | 当成「财务部门的技术指标」；实际上它是销售给账期、采购囤库存这些**经营决策的直接后果** |
| 4 | **现金转换周期**（cash conversion cycle, CCC） | tier-1 | 存货天数 + 应收天数 − 应付天数；钱转一圈要多久 | 判断这门生意增长时是产生现金还是消耗现金。CCC 为负 = 增长自带弹药 | Richards & Laughlin, Financial Management, 1980 (evidence: [T04-S047]) | 只看流动比率这类静态指标就下流动性结论 |
| 5 | **贡献边际**（contribution margin） | tier-1 | 收入 − 变动成本；每多卖一单位为覆盖固定成本贡献多少 | 判断接不接这一单、要不要降价促销。只要贡献边际为正且产能有余，短期接单优于闲置 | 管理会计标准内容；本量利分析 (evidence: [T04-S025, T04-S031]) | 用毛利率代替贡献边际——毛利里通常含了固定的制造费用分摊 |
| 6 | **经营杠杆**（operating leverage） | tier-1 | 固定成本占比越高，利润对收入变动的放大倍数越大 | 判断这门生意的脆弱性。高固定成本的生意在上行时利润暴涨，下行时先死 | 公司金融/管理会计标准内容 (evidence: [T04-S025]) | 只在顺境里算它，把放大器当成优势 |
| 7 | **盈亏平衡点**（break-even） | tier-1 | 固定成本 ÷ 贡献边际率；覆盖全部固定成本所需的收入 | 判断「还要多久 / 还差多少单」才能不亏，以及降价后盈亏点会往上跳多少 | 本量利分析（CVP），管理会计经典 (evidence: [T04-S025]) | 只算会计盈亏平衡，忽略**现金盈亏平衡**（含还本、税、老板工资）——后者才是能不能活的线 |
| 8 | **单位经济**（unit economics） | tier-1 | 把整体损益缩到「一个客户 / 一单 / 一台」的粒度 | 判断亏损是投资还是失血。单客户能回本 = 亏损是增长代价；不能回本 = 规模放大亏损 | David Skok, SaaS Metrics 2.0 (evidence: [T04-S042, T04-S049]) | LTV 用过短样本外推，得出虚高的 LTV/CAC |
| 9 | **自由现金流**（free cash flow） | tier-1 | 经营活动现金流 − 资本开支；企业真正可自由支配的钱 | 判断这门生意能不能自己养活自己并给股东回报 | 公司金融教科书；Damodaran 估值体系 (evidence: [T04-S025, T04-S003]) | 与经营现金流混用；忽略了必须的资本开支 |
| 10 | **业主收益**（owner earnings） | tier-1 | 净利 + 折旧摊销等非现金费用 − 维持现有竞争地位与产量所需的资本开支（及必要营运资金增加） | 判断「这门生意每年真正能给股东留下多少钱」，并据此反驳 EBITDA | Buffett, Berkshire 1986 年致股东信附录 (evidence: [T04-S013, T04-S065]) | 把全部资本开支都当维持性（低估）或都当扩张性（高估）；维持性资本开支只能估计，不能审计 |
| 11 | **资本成本与机会成本**（cost of capital / opportunity cost） | tier-1 | 这笔钱用在别处能获得的、风险相当的回报率 | 判断一个项目值不值得做的门槛。低于资本成本的增长在毁灭价值 | Modigliani & Miller 1958；Brealey/Myers/Allen (evidence: [T04-S027, T04-S025]) | 中小企业直接套 CAPM 算折现率；beta 与市场数据对非上市公司基本不适用 (evidence: [T04-S040]) |
| 12 | **NPV / IRR / 回收期** | tier-1 | NPV = 未来现金流按资本成本折现后减去投入；IRR = 使 NPV 归零的折现率；回收期 = 多久回本 | 判断投资项目做不做、先做哪个。理论上 NPV 是唯一正确裁判 | Brealey/Myers/Allen 资本预算章 (evidence: [T04-S025]) | 用 IRR 排序互斥项目（规模与期限不同则会给错答案）；用回收期做唯一标准（忽略回收后的全部价值） |
| 13 | **ROIC 与增长创造价值的条件** | tier-1 | ROIC = 税后经营利润 ÷ 投入资本；**只有 ROIC > 资本成本时增长才创造价值** | 判断「要不要增长」。ROIC 低于资本成本时，越增长越毁灭价值 | Mauboussin Counterpoint Global；Koller 等《Valuation》 (evidence: [T04-S006, T04-S070]) | 投入资本口径不统一（研发/获客被费用化、租赁、商誉、超额现金处理不同），导致轻资产公司 ROIC 系统性虚高 (evidence: [T04-S006]) |
| 14 | **资本配置**（capital allocation） | tier-1 | 现金的五个去处：内部投资、并购、分红、回购、还债 | 判断管理层（也包括你自己）是不是在把钱放到回报最高的地方 | Thorndike《The Outsiders》；Mauboussin《Capital Allocation》 (evidence: [T04-S021, T04-S007]) | 默认「有钱就扩张」；不把「还债」和「什么都不做」当成正经选项 |
| 15 | **稀释**（dilution） | tier-1 | 新股发行后原股东持股比例下降 | 判断融资的真实代价。要按完全稀释（含期权池、可转债、认股权证）算，不能只看本轮 | Feld & Mendelson《Venture Deals》 (evidence: [T04-S016, T04-S036]) | 只看单轮稀释比例；忽略期权池在投前还是投后设立（这一条能改变创始人几个百分点） |
| 16 | **优先清算权**（liquidation preference） | tier-1 | 退出时优先股先按约定倍数/顺序拿钱，剩下的才轮到普通股 | 判断在不同退出金额下你实际拿多少。低价退出时创始人可能一分钱拿不到 | Venture Deals；Gornall & Strebulaev 2020 (evidence: [T04-S016, T04-S034]) | 把「投后估值」当身价——研究显示报告估值平均高于公允价值 48%，普通股被高估 56% (evidence: [T04-S034]) |
| 17 | **递延收入 / 合同负债**（deferred revenue） | tier-1 | 已收钱但尚未提供服务的部分，是负债不是收入 | 判断预收款型生意的真实经营状况；也是免息的经营性融资来源 | IFRS 15 / ASC 606；CAS 14 (evidence: [T04-S009, T04-S066]) | 把预收当收入，把「银行里有钱」当「赚到了钱」——这正是 Profit First 类银行余额法最危险的地方 (evidence: [T04-S019]) |
| 18 | **资本化 vs 费用化**（capitalize vs expense） | tier-1 | 支出计入资产分期摊销（资本化），还是当期全额进损益（费用化） | 判断利润的可信度。资本化把今天的费用推到未来，当期利润立刻变好看 | IFRS/CAS 各具体准则；Schilit《Financial Shenanigans》 (evidence: [T04-S015, T04-S012]) | 看到「研发资本化率突然上升」不警觉；这是最常见的利润粉饰手法之一 |
| 19 | **折旧摊销政策的判断空间** | tier-1 | 使用年限、残值、折旧方法都是管理层的估计 | 判断利润里有多少是「估出来的」。同样的设备，年限从 5 年改 10 年，当期利润立刻变高 | Berman & Knight「利润是估计值」；准则原文 (evidence: [T04-S001, T04-S012]) | 把折旧当成客观数字；或反过来因为它是非现金支出就当它不存在（Buffett 明确反对后者） (evidence: [T04-S013]) |
| 20 | **收入确认的五步法** | tier-1 | 识别合同 → 识别履约义务 → 确定交易价格 → 分摊价格 → 履约时确认 | 判断「这笔钱什么时候能算成收入」，尤其在打包销售、分期交付、含可变对价时 | IFRS 15 / ASC 606；CAS 14 (evidence: [T04-S009, T04-S057, T04-S066]) | 以为开了发票就是收入；或以为收到钱就是收入 |
| 21 | **本人 vs 代理人**（principal vs agent） | tier-2 | 你是自己在卖（总额确认收入）还是替别人卖（净额确认佣金） | 判断平台/撮合型生意该报多大的营收——这一判断可以让同一门生意的营收差十倍 | IFRS 15 相关指引 (evidence: [T04-S057, T04-S009]) | 为了做大 GMV 型营收强行按总额确认，被审计或投资人拆穿 |
| 22 | **EBITDA 与调整后 EBITDA** | tier-1 | 息税折旧摊销前利润；「调整后」再剔除管理层认为非经常的项目 | 判断对方在隐藏什么。它的合法用途是跨资本结构比较经营层面表现 | Buffett 1986 年信的批评；SEC Reg G / C&DI；IFRS 18 的 MDPM 披露 (evidence: [T04-S013, T04-S011, T04-S008]) | 当成现金流的代理指标。**折旧对应的是真实会磨损的资产**；IFRS 16 后租金被拆进折旧+利息，EBITDA 还被系统性抬高了一截 (evidence: [T04-S013, T04-S058]) |
| 23 | **利润质量 / 资产质量** | tier-1 | 同样的数字，来源与可持续性不同，质量就不同 | 判断这个利润明年还有没有、这笔资产是不是真能变现 | 张新民「财务状况质量分析」体系；Schilit (evidence: [T04-S038, T04-S037, T04-S015]) | 只比大小不问构成；把一次性处置收益、政府补助当成经营能力 |
| 24 | **滚动预测**（rolling forecast） | tier-2 | 固定向前看 N 个季度、定期滚动更新的无偏预测，与目标和奖金脱钩 | 判断未来 4–12 个月的现金缺口，且不被「达标压力」污染 | Beyond Budgeting Round Table；Hope & Fraser (evidence: [T04-S033]) | 把滚动预测又和考核挂钩——挂上去它立刻变成第二个预算，一样会被博弈 (evidence: [T04-S039]) |
| 25 | **预算游戏 / 目标与奖金耦合** | tier-2 | 把奖金和预算达成率挂钩，就是在花钱购买失真信息 | 判断部门数据可信度。年年「刚好完成 101%」是薪酬结构造成的，不是执行力 | Jensen, HBR 2001 /《Paying People to Lie》 (evidence: [T04-S039, T04-S068]) | 以为加强审核能解决；问题在激励结构不在审核力度 |
| 26 | **融资优序**（pecking order） | tier-2 | 因信息不对称，企业偏好顺序为：内部留存 > 债务 > 股权 | 判断融资动作在向外界传递什么信号，以及为什么持有现金储备本身有价值 | Myers & Majluf 1984；Donaldson 1961 (evidence: [T04-S029, T04-S064]) | 当成铁律；对高成长、无抵押物的创业公司解释力本来就弱 (evidence: [T04-S064]) |

---


---

## 五、智识谱系种子

> 六个流派。每派给：奠基文本 / 当前代表人物 / **与别派的核心分歧（写实，不和稀泥）**。
> 这一节的价值在于：同一个财务问题，不同流派会给出**互相矛盾**的答案，而这些矛盾是真实的，不是误解。

---

### 派 1 · 准则合规派（Standards & Compliance）

- **奠基文本**：IFRS 概念框架与各具体准则（IFRS 15 / 16 / 18）、US GAAP（ASC 606）、中国企业会计准则 CAS 与《小企业会计准则》 (evidence: [T04-S009, T04-S010, T04-S008, T04-S012, T04-S048])
- **当前代表**：IASB / FASB / 中国财政部会计司；四大事务所的技术出版物（Deloitte IAS Plus、KPMG、PwC Viewpoint）作为二级传播层 (evidence: [T04-S057, T04-S059])
- **世界观**：财务报表的第一职责是**可比与可审计**。规则统一了，不同公司、不同年份才能放在一起看。判断空间存在，但必须被披露和约束。
- **与别派的分歧**：
  - **vs 管理会计决策派**：合规派要的是外部可比，决策派要的是内部有用。ABC 算出的产品成本在管理上有用，但**不能进对外报表**；反过来，准则要求的分摊口径对内部决策常常是误导性的 (evidence: [T04-S031])
  - **vs 中小企业现金实操派**：合规派认为权责发生制是几百年演化出来的解决方案，收付实现制会系统性误导；实操派认为对付不起账单的小企业，权责利润是奢侈品 (evidence: [T04-S019])
  - **内部分歧**：全套准则 vs 简化准则（IFRS for SMEs / 《小企业会计准则》）。降低成本与保留信息含量之间没有免费午餐 (evidence: [T04-S061, T04-S048])

---

### 派 2 · 管理会计决策派（Management Accounting）

- **奠基文本**：Cooper & Kaplan, *Measure Costs Right*（HBR 1988）；本量利分析（CVP）与贡献边际的教科书传统；Kaplan & Anderson 的 TDABC (evidence: [T04-S031, T04-S032])
- **当前代表**：Robert S. Kaplan（哈佛商学院）及其 TDABC 路线；企业内部的 FP&A（财务规划与分析）职能
- **世界观**：会计数字的价值在于**支持决策**，不在于满足外部报送。成本必须按**资源真实消耗**归属，否则定价、产品线取舍、客户分层全会错。
- **与别派的分歧**：
  - **vs 公司金融估值派**：管理会计看成本与边际，估值派看现金流与资本成本。管理会计说「这个产品毛利低」，估值派会追问「它占用了多少投入资本、ROIC 是多少」——**低毛利高周转的产品可能 ROIC 更高**，两派会给出相反的砍留建议 (evidence: [T04-S006])
  - **vs 中小企业现金实操派**：ABC 的精度对小公司是不划算的；实操派用几条粗规则（人效比、10% 净利率线）代替精细核算 (evidence: [T04-S018, T04-S032])
  - **内部裂痕**：Kaplan 本人承认原版 ABC 落地失败率高，这是流派内最诚实的一次自我修正 (evidence: [T04-S032])
  - **与预算的关系分裂**：传统管理会计以年度预算为核心工具，Beyond Budgeting 与 Jensen 则认为年度预算 + 挂钩奖金是信息污染的根源 (evidence: [T04-S033, T04-S039])

---

### 派 3 · 公司金融估值派（Corporate Finance & Valuation）

- **奠基文本**：Modigliani & Miller 1958；Myers & Majluf 1984；Brealey/Myers/Allen《Principles of Corporate Finance》；Damodaran《Investment Valuation》《Narrative and Numbers》 (evidence: [T04-S027, T04-S029, T04-S025, T04-S003, T04-S023])
- **当前代表**：Aswath Damodaran（NYU Stern，免费公开数据与课程）；Alex Edmans（第 14 版新增作者）；Koller/Goedhart/Wessels 的《Valuation》路线 (evidence: [T04-S003, T04-S025, T04-S070])
- **世界观**：价值 = 预期现金流按风险折现。会计利润是通往现金流的中间产物，不是终点。**一切决策归结为 NPV**。
- **与别派的分歧**：
  - **vs 会计估值桥派（Penman）**：这是本次调研中最尖锐的一组对立。估值派主张用未来现金流与资本成本；Penman 直接主张**放下资本成本、CAPM 和 DCF**，改用会计账面价值与利润锚定，理由是 DCF 把权重压在最不可知的远期预测上，且投资期现金流为负难以解释 (evidence: [T04-S022, T04-S024])
  - **vs 准则合规派**：估值派对会计准则的态度是「有用但不够」——折旧年限、资本化政策这些准则允许的选择会直接改变表观利润，所以估值必须做还原
  - **内部分歧**：DCF 到底能不能用于早期公司。Damodaran 认为不确定性大不是不做 DCF 的理由；批评者认为此时输出区间大到无信息 (evidence: [T04-S040])

---

### 派 4 · 价值投资资本配置派（Capital Allocation）

- **奠基文本**：Berkshire Hathaway 致股东信（尤其 1986 年的 owner earnings 与「现金流谬误」附录）；Thorndike《The Outsiders》 (evidence: [T04-S013, T04-S021])
- **当前代表**：Michael Mauboussin（Morgan Stanley Counterpoint Global），把案例观察升级为跨公司统计；价值投资社群 (evidence: [T04-S006, T04-S007])
- **世界观**：CEO 的第一职责是资本配置。**每股价值增长**是唯一记分牌；分母（股份数）与分子同等重要。对会计利润高度怀疑，对现金高度信任。
- **与别派的分歧**：
  - **vs 管理会计决策派**：这派几乎不关心内部成本核算的精度，只关心「这笔资本投出去回报多少」。ABC 那种精细核算在他们眼里是次要问题
  - **vs 估值派（但只是程度之争）**：都用现金流思维，但资本配置派更倾向于粗略正确（owner earnings 的估计性质、Buffett 明说「宁要模糊的正确」）；估值派更强调显式模型与假设可辩护 (evidence: [T04-S013, T04-S040])
  - **被外部批评的软肋**：结论主要来自成功案例，缺对照组——幸存者偏差是这一派最实在的方法论问题 (evidence: [T04-S021])
  - **与准则合规派的正面冲突**：这派公开主张 GAAP 数字常常扭曲经济实质（购买法调整、商誉摊销），而合规派认为脱离准则的自定义指标正是操纵的温床——这个冲突在 IFRS 18 的 MDPM 披露要求里得到了制度化的折中 (evidence: [T04-S013, T04-S008])

---

### 派 5 · 创业与 SaaS 指标派（Startup / SaaS Metrics）

- **奠基文本**：David Skok 的 SaaS Metrics 2.0 与 SaaS 现金流低谷系列；Feld & Mendelson《Venture Deals》 (evidence: [T04-S042, T04-S049, T04-S016])
- **当前代表**：David Skok（Matrix Partners）；Brad Feld / Jason Mendelson（Foundry Group）；学术侧的 Gornall & Strebulaev 提供了对本派乐观倾向的实证纠偏 (evidence: [T04-S034])
- **世界观**：传统财务指标对订阅制早期公司是错的工具。要看**单位经济**（CAC、LTV、回收期、流失率）与**现金跑道**，而不是当期利润。亏损可以是投资。
- **与别派的分歧**：
  - **vs 中小企业现金实操派**：Crabtree 说净利率低于 10% 就是不健康；SaaS 派说增长期为负利润是设计出来的。**两者对同一份报表会给出完全相反的诊断**——分歧的实质是「有没有外部资本持续供给」这一前提 (evidence: [T04-S018, T04-S049])
  - **vs 公司金融估值派**：估值派会问 LTV 里的折现率与流失率假设经不经得起检验；SaaS 派的 LTV 常用简化算法且样本期短，系统性高估 (evidence: [T04-S042, T04-S040])
  - **自身被证伪的部分**：报告估值与真实公允价值之间的 48% 缺口，说明这一派长期使用的「估值」概念本身有系统性偏差 (evidence: [T04-S034])

---

### 派 6 · 中小企业现金实操派（SMB Cash Discipline）

- **奠基文本**：Greg Crabtree《Simple Numbers》；Mike Michalowicz《Profit First》；Berman & Knight《Financial Intelligence》作为素养底座 (evidence: [T04-S018, T04-S017, T04-S001])
- **当前代表**：Greg Crabtree（执业 CPA，人效比与老板工资还原）；Profit First Professionals 认证会计师网络；大量独立记账/CFO 外包事务所 (evidence: [T04-S018, T04-S017])
- **世界观**：小企业主不会读报表，也不该被要求先学会读报表才能管好钱。给他们**少数几条能立刻执行的硬规则**，比给一套正确但用不起来的体系有效。
- **与别派的分歧**：
  - **派内的正面对立（最值得记录的一条）**：Crabtree 与 Michalowicz 面向同一读者，方法论却互相否定。Crabtree 用**真实管理会计口径**（还原老板工资、算人效比、看权责利润）；Michalowicz 用**银行余额与账户隔离**，主动绕开会计。批评 Profit First 的会计师明确指出，银行余额法忽略应收应付与递延，对预收款和项目制企业会给出误导信号 (evidence: [T04-S018, T04-S019, T04-S020])
  - **vs 准则合规派**：这派对准则的态度是实用主义的——够用就行；合规派认为绕过权责发生制是在给自己埋雷 (evidence: [T04-S019])
  - **vs 创业 SaaS 指标派**：见上，对「健康的亏损」这件事完全不同意
  - **共同软肋**：两本书的关键数值（10% 净利率线、LER 1.8–2.2、Profit First 的分配百分比）都来自作者服务的特定样本，缺乏跨行业实证，却被读者当成普适基准 (evidence: [T04-S018, T04-S019])

---

### 谱系图（简）

```
        准则合规派 ──────────────┐
     (IASB/FASB/财政部)          │  「可比、可审计」
              │                  │
              │ 提供原材料        ▼
              ├──────────► 会计估值桥派 (Penman)
              │                  ▲  「锚定已知，放下资本成本」
              ▼                  │        ⚡ 正面对立
        管理会计决策派 ◄──── 分歧 ──►  公司金融估值派 (MM → Brealey → Damodaran)
     (Cooper & Kaplan, ABC)              │  「NPV 是唯一裁判」
              │                          │
              │ ⚡ 预算之争                │ 现金流思维
              ▼                          ▼
       Beyond Budgeting / Jensen    价值投资资本配置派 (Buffett → Thorndike → Mauboussin)
        「预算+奖金=买谎话」              │  「CEO 的本职是配置资本」
                                         │
                    ┌────────────────────┴──────────────────┐
                    ▼                                       ▼
        创业与 SaaS 指标派 (Skok, Feld)          中小企业现金实操派 (Crabtree ⚡ Michalowicz)
         「亏损可以是投资」    ⚡⚡ 对同一报表给出相反诊断   「先把利润拿走」
```

---


---

## 六、争议节（保留争议，不洗白）

---

### 争议 1 · 调整后 EBITDA 与非公认会计准则指标的滥用

- **争议是什么**：企业越来越多地用自定义指标（调整后 EBITDA、调整后净利、社区调整后 EBITDA 之类）代替准则利润讲故事。支持方说准则利润被非现金项和一次性项污染，自定义指标更能反映经营实质；反对方说这是**给管理层发了一支橡皮擦** (evidence: [T04-S011, T04-S013])
- **最有分量的反对意见**：Buffett 在 1986 年的信里直接把当时华尔街流行的「cash flow」口径称为谬误——折旧对应的是真实会磨损、必须更新的资产，把它加回去等于假装机器不会坏 (evidence: [T04-S013])
- **监管的处理方式（不是禁止，是强制透明）**：
  - SEC Reg G / Item 10(e)：可以用，但必须给最直接可比的 GAAP 指标 + 调节表，且不得误导；把两年内发生过类似情形的费用标为「非经常性」可能构成违规 (evidence: [T04-S011, T04-S043])
  - IFRS 18（2027 生效）：把管理层自定义业绩指标 MDPM 拉进附注，要求披露定义与调节 (evidence: [T04-S008, T04-S059])
- **未解决的部分**：把 MDPM 写进财报到底是**约束**了它还是**给它背书**，业界有分歧 (evidence: [T04-S059])
- **一个容易被忽略的技术事实**：IFRS 16 之后租金被拆成折旧+利息，**EBITDA 被系统性抬高**，跨准则期比较 EBITDA 是无效的——这不是操纵，是口径变化，但效果一样 (evidence: [T04-S058, T04-S010])

---

### 争议 2 · DCF 对假设的极端敏感 / 该不该用 DCF

- **争议是什么**：DCF 在理论上无懈可击，在实践中被批评为「假设的放大器」。Damodaran 自己承认多数人不信任 DCF 估值，且理由正当——分析师把偏见藏进输入，用复杂度吓退质疑者 (evidence: [T04-S040])
- **三方立场（都是真实立场，不折中）**：
  - **Damodaran（用，但要诚实）**：不确定性大不是放弃 DCF 的理由；模型复杂度不等于准确度；最关键的输入是现金流与再投资，不是折现率 (evidence: [T04-S040, T04-S041])
  - **Penman（不用，换锚）**：主张放下资本成本、CAPM 与 DCF，改用会计账面价值与利润锚定；理由是 DCF 把权重压在最不可知的远期，且投资期的负现金流难以解释——而权责发生制正是为解决这个问题发明的 (evidence: [T04-S022, T04-S024])
  - **Mauboussin（你以为你没用，其实你在用）**：倍数法不是 DCF 的替代品，是把 DCF 的假设压缩进一个数字里藏起来了——「当价值的绝大部分来自 EV/EBITDA 倍数时，结果只是打扮成 DCF 的倍数分析」 (evidence: [T04-S053, T04-S052])
- **对创业者的实际含义**：三方都同意的唯一一点是——**输出一个精确的单一数字是不诚实的**。要给区间，并说明哪个假设变动会推翻结论
- **学界并未收敛**：Accounting, Economics, and Law 就 Penman 的立场组织了专门评论，指出其一边声称遵守金融理论、一边整体重释这些原则，两者是否自洽仍有争论 (evidence: [T04-S024])

---

### 争议 3 · Profit First 受到的专业批评

- **支持方**：它承认小企业主的真实行为（只看银行余额、不读报表），用账户隔离制造人为稀缺，对现金失控型微型企业立竿见影；作者建立了认证会计师网络推广 (evidence: [T04-S017])
- **反对方（会计师群体，理由具体）**：
  - **把症状管理当病因治疗**：分账户不改变毛利不足、定价过低、成本结构错误这些真实问题，只是更早地让你发现付不起账单 (evidence: [T04-S019, T04-S020])
  - **越过适用条件却不声明**：方法是否可行取决于定价能力、固定成本占比、资本密集度、需求弹性；作者把自己那类轻资产服务业的经验推广成普适法则，从未说明前提 (evidence: [T04-S019])
  - **与权责发生制冲突**：银行余额法忽略应收应付与递延收入，对有大额预收款或长周期项目的企业会给出严重误导的信号 (evidence: [T04-S019, T04-S020])
  - **规则刚性**：「不许动利润账户」在真实紧张时要么被违反、要么导致次优决策；有从业者形容为把企业长期困在急救分诊状态 (evidence: [T04-S020])
- **不和稀泥的结论**：它是**有效的行为工具、不合格的财务分析框架**。适用边界是「现金持续失控、且确定不会去读报表」的微型企业；已经有像样管理会计的企业用它是退步 (evidence: [T04-S019, T04-S020])
- **同一读者群里的对立方案**：Crabtree《Simple Numbers》用真实管理会计口径解决同一问题（还原老板工资、算人效比），两者不可调和 (evidence: [T04-S018])

---

### 争议 4 · 作业成本法 ABC 的实施失败率

- **争议是什么**：ABC 在理论上解决了间接费用分摊扭曲的问题，在实践中大规模落地屡屡失败
- **最有分量的证据是来自奠基者本人**：Kaplan 在 2004 年公开承认，试图大规模实施 ABC 的高管**常常在成本上升与员工抵触面前放弃了尝试**；数据靠员工填时间比例问卷，主观、昂贵、难维护。他随后提出 TDABC 作为补救 (evidence: [T04-S032, T04-S031])
- **更根本的批评**：ABC 提高了成本信息的精度，但**短期内多数间接成本并不随作业量变化**。按 ABC 判定「不赚钱」而砍掉的产品线，砍完后间接费用仍在，只是摊到更少产品上——**精确的成本信息不等于正确的决策** (evidence: [T04-S032, T04-S031])
- **未解决**：TDABC 是否真的解决了维护成本问题，还是把主观性从「员工估比例」转移到了「管理层估单位时间」，缺乏大规模独立评估 (evidence: [T04-S032])
- **对中小企业的现实结论**：完整 ABC 通常不划算；值得借用的是提问方式（哪些作业真正消耗资源），不是核算系统

---

### 争议 5 · 预算游戏

- **争议是什么**：年度预算到底该修、该改激励、还是该废
- **三种立场**：
  - **修流程（传统管理会计）**：加强预算编制质量、增加审核层级
  - **改激励（Jensen）**：预算系统本身没错，**错在把奖金和达成率挂钩**——阶梯式奖金让上下级都有动机撒谎，污染了预算作为协调工具的信息基础。解法是纯线性奖金曲线 (evidence: [T04-S039, T04-S068, T04-S069])
  - **废预算（Beyond Budgeting）**：问题在固定年度目标本身。把目标（改为相对目标）、预测（改为无偏滚动预测）、资源分配（改为动态）三件事拆开 (evidence: [T04-S033])
- **各自的软肋**：
  - Jensen 的线性奖金在实务中推行困难（董事会与投资人偏好明确的目标承诺）
  - Beyond Budgeting 的证据基础是先行企业案例，缺严格对照，且完全废除预算在有银行契约与监管报送的组织中不可行 (evidence: [T04-S033])
  - **滚动预测本身也会被游戏化**：只要它仍影响资源分配和评价，做预测的人一样有动机报偏 (evidence: [T04-S039])
- **未解决**：没有任何一方给出了在「需要对外承诺一个数字」与「需要内部无偏信息」之间的通用解

---

### 争议 6 · 独角兽估值与优先清算权造成的纸面身价

- **争议是什么**：媒体和创始人使用的「投后估值」是否有意义
- **量化证据（不是观点，是模型结果）**：Gornall & Strebulaev 对 135 家美国独角兽建模，发现**报告的投后估值平均高于公允价值 48%**，14 家高出 100% 以上；**普通股被高估 56%**；调整后 **135 家中 65 家失去独角兽身份** (evidence: [T04-S034, T04-S035, T04-S046])
- **机制**：投后估值 = 最近一轮优先股每股价格 × 全部股份数，这假设所有股份都和最新一轮一样值钱。但样本中 15% 有 IPO 回报保证、24% 有降价 IPO 否决权、30% 优先于其他所有投资人受偿——**普通股一样都没有** (evidence: [T04-S034])
- **谁在争议的另一边**：行业实践者指出，估值本身就是一个融资谈判的产物而非公允价值声明；且优先权在多数正常退出情形下不会触发。但这一辩护无法回应「媒体和创始人把它当身价传播」这个事实
- **对创始人的实际含义**：**你的持股价值必须按退出瀑布（waterfall）在多个退出金额下分别计算**，而不是「持股比例 × 投后估值」。这也是 Venture Deals 反复强调的「经济条款 ≠ 估值」 (evidence: [T04-S016, T04-S034])
- **周期性**：结构化条款（多倍优先权、参与权、棘轮）在下行周期会回潮，2019 年出版的 Venture Deals 第 4 版所描述的条款环境需要用近期一手材料校正 (evidence: [T04-S036])

---

### 争议 7（附加，本调研中发现的）· 中小企业该按哪套会计准则建账

- **争议是什么**：《小企业会计准则》降低了核算成本、减少税会差异，但也削弱了报表的经济含义（缺公允价值、减值信息简化）
- **两种立场**：合规成本派主张小企业用简化准则，避免为不存在的读者付费；融资准备派主张凡有外部融资打算的应尽早按 CAS 建账，否则转换成本会在最不该出问题的时候爆发
- **同样的张力在国际上有对应物**：IFRS for SMEs 与全套 IFRS 之间是同一权衡 (evidence: [T04-S061, T04-S048])
- **未解决**：没有公开研究给出「什么规模/什么阶段应该切换」的实证阈值，实务中靠经验判断

---


---

## Phase 2 提炼提示

### 反复出现 ≥ 3 个 canon 都讨论的核心 idea（候选行业心智模型）

1. **利润是估计出来的，现金是数出来的** — 出现于 Berman & Knight #1 / Buffett 1986 信 #11 / Schilit #9 / 肖星 #13 / 张新民 #14 → **最强候选心智模型**。它同时解释了为什么要看现金流量表、为什么要做质量分析、为什么要警惕会计政策变更 (evidence: [T04-S001, T04-S013, T04-S015, T04-S014, T04-S038])
2. **增长不是免费的：增长要用现金买** — 出现于 Skok 现金流低谷 / Richards & Laughlin 现金转换周期 / Crabtree / Brealey-Myers 营运资金章 / Mauboussin ROIC → **第二强候选**。判断规则：增长前先算营运资金增量与 CAC 回收期 (evidence: [T04-S049, T04-S047, T04-S018, T04-S025, T04-S006])
3. **只有 ROIC > 资本成本时增长才创造价值** — 出现于 Mauboussin / Koller《Valuation》/ Brealey-Myers / Thorndike & Buffett → 判断规则：任何扩张提议先问预期回报率与资本成本的关系 (evidence: [T04-S006, T04-S070, T04-S025, T04-S021])
4. **一切估值本质都是同一件事，只是假设藏得深浅不同** — 出现于 Damodaran / Mauboussin / Penman（以反对形式出现）→ 判断规则：看到倍数就问它隐含了什么增长和什么资本回报 (evidence: [T04-S040, T04-S052, T04-S022])
5. **激励结构决定数字** — 出现于 Jensen 预算论文 / Schilit 财报粉饰 / Mauboussin 资本配置评估 / Beyond Budgeting → 判断规则：拿到任何一组数字先问「谁的奖金和它挂钩」 (evidence: [T04-S039, T04-S015, T04-S007, T04-S033])
6. **自定义指标必须附带定义与调节，否则不可信** — 出现于 SEC Reg G / IFRS 18 MDPM / Buffett EBITDA 批评 / Schilit「关键指标操纵」→ 已被两个准则体系制度化，共识度极高 (evidence: [T04-S011, T04-S008, T04-S013, T04-S015])

### 智识谱系种子（详见第五节）

| 流派 | 奠基 | 当前代表 | 与别派最尖锐的分歧 |
|------|------|---------|-------------------|
| 准则合规派 | IFRS/GAAP/CAS 概念框架与具体准则 | IASB / FASB / 财政部会计司 | 外部可比 vs 内部有用（对管理会计派）；权责发生制 vs 银行余额（对现金实操派） |
| 管理会计决策派 | Cooper & Kaplan, HBR 1988 | Robert S. Kaplan（TDABC）、企业 FP&A | 成本视角 vs 资本回报视角（对估值派）；派内已自承 ABC 落地失败率高 |
| 公司金融估值派 | MM 1958 → Brealey/Myers/Allen | Damodaran、Alex Edmans、Koller 团队 | **与 Penman 正面对立**：该不该放弃 DCF 与资本成本 |
| 价值投资资本配置派 | Buffett 1986 信 → Thorndike 2012 | Michael Mauboussin | 对 GAAP 的怀疑 vs 合规派的可审计要求；软肋是幸存者偏差 |
| 创业与 SaaS 指标派 | Skok SaaS Metrics 2.0；Feld & Mendelson | David Skok、Brad Feld；被 Gornall & Strebulaev 实证纠偏 | **与现金实操派对同一报表给出相反诊断**：亏损是投资还是失血 |
| 中小企业现金实操派 | Crabtree《Simple Numbers》/ Michalowicz《Profit First》 | Greg Crabtree；Profit First Professionals 网络 | **派内正面对立**：真实管理会计口径 vs 银行余额账户隔离 |

**canon 内部仍在辩论、Phase 2 不应强行统一的三件事**：
1. DCF 该不该用于早期与高不确定性公司（Damodaran vs Penman vs 实务批评者）
2. 年度预算该修流程、改激励、还是废除（传统 vs Jensen vs Beyond Budgeting）
3. 小企业该用简化会计口径还是完整权责发生制（Michalowicz vs Crabtree；《小企业会计准则》vs CAS）

### 核心概念 → 候选 playbook

| 概念 | 暗示的判断方式 |
|------|--------------|
| 现金转换周期 | 如果 CCC 为正且在拉长 → 增长会加速吞现金，先修账期与库存再谈扩张 |
| 单位经济 / CAC 回收期 | 如果单客户回本期 > 12 个月且流失率上升 → 这不是低谷是无底洞，停止加投放 |
| 贡献边际 + 经营杠杆 | 如果贡献边际为正且产能闲置 → 短期接单优于闲置；但先算降价后盈亏点上移多少 |
| ROIC vs 资本成本 | 如果新项目预期回报低于资本成本 → 不做，无论增长率多好看 |
| owner earnings | 如果对方只给 EBITDA → 自己减维持性资本开支再看；差距大的生意通常在藏资本消耗 |
| 递延收入 | 如果银行余额充裕但递延收入占比高 → 那些钱是欠客户的服务，不是利润 |
| 资本化 vs 费用化 | 如果资本化率突然上升而收入未同步 → 列入质询清单 |
| 优先清算权 | 如果被问「你们公司值多少」→ 先跑退出瀑布，别报投后估值 |
| 融资优序 | 如果在能用留存/债务时选择大额稀释 → 需要一个能对外解释的理由 |
| 预算与奖金耦合 | 如果部门年年刚好完成 101% → 先查奖金结构，不是查执行力 |

### 冷僻 / 信号薄弱评估

| 检查项 | 阈值 | 本 track 实际 | 结论 |
|--------|------|--------------|------|
| 必读书 | ≥ 3 | **14** | ✅ 充分 |
| 论文 / 研究 / 数据集 | ≥ 5 | **10**（+5 组准则原文） | ✅ 充分 |
| 课程 | ≥ 2 | **4**（均含 last_updated） | ✅ 充分 |
| 概念 | ≥ 15 | **26** | ✅ 充分 |
| Endorsement ≥ 3 处的书目占比 | ≥ 50% | **14/14 = 100%** | ✅ 充分 |
| verified_primary 占比 | ≥ 40% | 见下方 checklist | ✅ 充分 |

**结论：本行业不属于冷僻行业**，公开 canon 厚度充足（准则原文全部可免费获取，核心估值数据与课程由 Damodaran 免费公开）。

**但仍需在 SKILL.md 诚实边界节写明的两点**：
1. **中文圈的一手可引用材料偏少**。中文财务内容的主要传播渠道（知乎、公众号、财会考证网校）按信源规则全部排除，因此中文侧只保留了肖星、张新民两条书目/课程线与财政部原文。这意味着**中国特有的实务问题（两套账、发票与收入耦合、股东与公司资金混同、对赌条款）在本 canon 中覆盖不足**，需要 Track 03（workflows）与 Track 05（sources）补。
2. **中小企业实操派的关键数值缺乏实证支撑**。10% 税前净利率线、LER 1.8–2.2、Profit First 分配百分比均来自作者自身客户样本，本调研未找到独立复现研究。引用这些数字时必须标注为「经验法则」而非基准。

---

---

## 完成 checklist

| 项 | 数量 / 状态 |
|----|-----------|
| **Source 总数** | **75**（T04-S001 … T04-S075） |
| **verified_primary** | **31 条（41.3%）** |
| **surrogate_primary** | **24 条（32.0%）** — 全部 note 含 `own site` / `own publication` / `publisher official page` / `vendor docs` / `originator` / `official` 关键词（机械检查通过） |
| **secondary** | **20 条（26.7%）** |
| **dead / blacklisted** | **0 条** |
| 一手 (verified + surrogate) 合计 | **55 条 / 73.3%** |
| **书目条数** | **14 本**（另有 4 条边缘/降级候选，记录了判断理由） |
| **准则与规则原文** | **5 组**（IFRS 15/ASC 606、IFRS 16、IFRS 18、SEC Reg G、CAS +《小企业会计准则》） |
| **论文 / 研究 / 数据集** | **10 条** |
| **课程** | **4 门**，全部标注 last_updated |
| **概念条数** | **26 个**（tier-1 20 / tier-2 6） |
| **智识谱系流派** | **6 派**，每派含奠基文本 + 当前代表 + 与别派的具体分歧 |
| **争议条目** | **7 条**，全部保留分歧未做调和 |
| 黑名单检查 | 对全部禁用信源域名（中文问答社区 / 公众号 / 百科 / 技术博客站 / 财会考证网校等）做正则扫描 → **0 命中** ✅ |
| 每本书含「局限 / 被批评之处」 | **14/14** ✅ |
| 每本书 endorsement ≥ 3 且含 ≥1 条 figure_long 或 course_syllabus | **14/14** ✅ |
| 每个课程含 last_updated | **4/4** ✅ |
| 每个概念含「来源」字段 | **26/26** ✅ |

### 已知缺口（诚实记录）

1. **中文一手材料薄**：中文财务圈主要传播渠道被信源规则排除，导致中国特有实务（两套账、发票与收入耦合、对赌与回购条款、股东借款）在本 canon 中覆盖不足
2. **反爬拦截的 source**：Morgan Stanley（T04-S006/S007/S052/S071）、FASB（T04-S044）、SSRN（T04-S068）、McKinsey 系列对 curl 返回 403/000，属机器人拦截而非死链，内容已通过搜索结果与二次来源交叉确认；浏览器可正常访问
3. **两条 URL 换用了替代路径**：Ittelson 官方书页用 Simon & Schuster UK（Career Press 母公司渠道，redwheelweiser.com 直连 403）；《小企业会计准则》全文用上海市财政局 .gov.cn 转发页（财政部原文页已改版）
4. **未覆盖但相邻的领域**（本次范围明确排除）：并购交易执行与卖方建模、VC 投资人筛选逻辑、二级市场投资、注册会计师考证体系

### 交接给其他 Track

- **→ Track 01 figures**：Aswath Damodaran、Michael Mauboussin、Robert S. Kaplan、Stephen Penman、Howard Schilit、Greg Crabtree、Mike Michalowicz、Brad Feld、Jason Mendelson、David Skok、William Thorndike、Karen Berman、Joe Knight、肖星、张新民、Alex Edmans
- **→ Track 02 tools**：Damodaran 免费数据集与估值模板、Crabtree 的 LER 计算表、Skok 的 SaaS 现金流低谷 Excel 模型、退出瀑布（waterfall）计算、滚动预测模板
- **→ Track 03 workflows**：三表勾稽核对流程、13 周现金流滚动预测、月度经营复盘、term sheet 逐条审阅、财报质询清单（Schilit 式）
- **→ Track 06 glossary**：本文第四节的 26 个概念是**概念**层，其对应的黑话缩写（DSO / DPO / DIO / CAC / LTV / ARR / MRR / NRR / WACC / EBITDA / MDPM / 4-3-3 之类）归 Track 06 处理

---

*Track 04 完成 · 调研日期 2026-09-02 · locale zh-CN*
