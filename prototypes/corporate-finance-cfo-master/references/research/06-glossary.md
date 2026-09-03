# Track 06 — Glossary / 术语 · 标准 · 法规 · 认证
# 行业：企业财务与 CFO 视角（Corporate Finance & the CFO Lens）

> locale: `zh-CN`（术语中英对照，URL 保留原文） · 调研日期 `2026-09-02`
> 范围锚定：面向创业公司与中小企业主 / 创始人的**内部财务判断** —— 三张表、预算与滚动预测、现金流与营运资金、成本核算与定价、融资结构与股权稀释。
> 明确排除：投行并购术语细节、VC 投资人内部术语、个人理财术语、考证大纲。
>
> **合规声明**：本文件描述术语与制度事实。涉及中国税务的部分，只指向官方公告原文与持证税务师，**不提供任何税收规避、发票操作或收入隐瞒的方法**。历史实务（如「两套账」）仅作为风险现象被描述，不作为可行做法。

---

## Source Manifest

> bucket 由 `python3 tools/research/source_verifier.py classify <URL>` 机械判定；
> 准则 / 协会发布机构与四大解读按 Track 06 规范人工升级为 `surrogate_primary`（note 中逐字带 `originator` / `vendor docs` / `own publication` / `official`）。

| source_id | url | bucket | last_checked | author/host | one-line note |
|-----------|-----|--------|--------------|-------------|---------------|
| T06-S001 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-18-presentation-and-disclosure-in-financial-statements/ | surrogate_primary | 2026-09-02 | IASB / IFRS Foundation | originator：IFRS 18 准则主页与生效安排 |
| T06-S002 | https://www.ifrs.org/news-and-events/news/2024/04/new-ifrs-accounting-standard-will-aid-investor-analysis-of-companies-financial-performance/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator：2024-04 IFRS 18 发布公告 |
| T06-S003 | https://www.ifrs.org/content/dam/ifrs/publications/amendments/english/2024/effect-analysis-ifrs18-april2024.pdf | surrogate_primary | 2026-09-02 | IASB | originator：IFRS 18 影响分析，含 MPM 设计意图 |
| T06-S004 | https://www.ifrs.org/content/ifrs/home/projects/work-plan/management-defined-performance-measures-hypothetical-income-and-expenses-ifrs-18/tads-and-cls.html | surrogate_primary | 2026-09-02 | IFRS IC | originator：MPM 议题的暂定议程决定 |
| T06-S005 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-15-revenue-from-contracts-with-customers/ | surrogate_primary | 2026-09-02 | IASB | originator：IFRS 15 收入准则主页 |
| T06-S006 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-16-leases/ | surrogate_primary | 2026-09-02 | IASB | originator：IFRS 16 租赁准则主页 |
| T06-S007 | https://www.ifrs.org/issued-standards/ifrs-sustainability-standards-navigator/ifrs-s1-general-requirements/ | surrogate_primary | 2026-09-02 | ISSB | originator：IFRS S1 一般要求 |
| T06-S008 | https://www.ifrs.org/issued-standards/ifrs-sustainability-standards-navigator/ifrs-s2-climate-related-disclosures/ | surrogate_primary | 2026-09-02 | ISSB | originator：IFRS S2 气候相关披露 |
| T06-S009 | https://www.ifrs.org/news-and-events/news/2023/06/issb-issues-ifrs-s1-ifrs-s2/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator：2023-06 S1/S2 发布公告 |
| T06-S010 | https://www.ifrs.org/ifrs-sustainability-disclosure-standards-around-the-world/use-by-jurisdiction/ | surrogate_primary | 2026-09-02 | IFRS Foundation | originator：各法域采用进度追踪页 |
| T06-S011 | https://www.sec.gov/corpfin/non-gaap-financial-measures | verified_primary | 2026-09-02 | SEC Corp Fin | official：非 GAAP 指标 C&DI 官方解释 |
| T06-S012 | https://storage.fasb.org/ASU%202014-09_Section%20A.pdf | surrogate_primary | 2026-09-02 | FASB | originator：ASU 2014-09 原文（ASC 606） |
| T06-S013 | https://storage.fasb.org/Comparison%20of%20Topic%20606%20and%20IFRS%2015.pdf | surrogate_primary | 2026-09-02 | FASB | originator：606 与 IFRS 15 官方对照 |
| T06-S014 | https://kjs.mof.gov.cn/zt/kjzzss/kuaijizhunzeshishi/201709/t20170907_2694006.htm | verified_primary | 2026-09-02 | 财政部会计司 | official：企业会计准则第 14 号——收入 |
| T06-S015 | https://kjs.mof.gov.cn/zt/kjzzss/kuaijizhunzeshishi/201910/t20191028_3411190.htm | verified_primary | 2026-09-02 | 财政部会计司 | official：企业会计准则第 21 号——租赁 |
| T06-S016 | http://kjs.mof.gov.cn/zhengcefabu/201812/t20181213_3092629.htm | verified_primary | 2026-09-02 | 财政部 | official：修订印发新租赁准则的通知与施行日 |
| T06-S017 | http://m.mof.gov.cn/zcfb/201707/t20170719_2653110.htm | verified_primary | 2026-09-02 | 财政部 | official：修订印发新收入准则的通知与分批施行 |
| T06-S018 | http://kjs.mof.gov.cn/zhengcefabu/201905/t20190510_3254992.htm | verified_primary | 2026-09-02 | 财政部会计司 | official：一般企业财务报表格式（三张表口径） |
| T06-S019 | https://fgk.chinatax.gov.cn/zcfgk/c102416/c5210453/content.html | verified_primary | 2026-09-02 | 财政部 / 税务总局 | official：2023 年第 12 号，小微税费政策延至 2027-12-31 |
| T06-S020 | https://fgk.chinatax.gov.cn/zcfgk/c102416/c5201978/content.html | verified_primary | 2026-09-02 | 财政部 / 税务总局 | official：2023 年第 7 号，研发费加计扣除 100% |
| T06-S021 | https://fgk.chinatax.gov.cn/zcfgk/c100022/c5215324/content.html | verified_primary | 2026-09-02 | 税务总局 / 科技部 | official：研发费用加计扣除政策执行指引 2.0 |
| T06-S022 | https://www.gov.cn/zhengce/zhengceku/202411/content_6989164.htm | verified_primary | 2026-09-02 | 国务院 / 税务总局 | official：全国推广数电发票公告（2024-12-01 起） |
| T06-S023 | https://www.gov.cn/zhengce//202411/content_6989160.htm | verified_primary | 2026-09-02 | 中国政府网 | official：数电发票公告的官方解读 |
| T06-S024 | https://fgk.chinatax.gov.cn/zcfgk/c100012/c5236067/content.html | verified_primary | 2026-09-02 | 国家税务总局 | official：数电发票推广公告法规库原文 |
| T06-S025 | https://www.chinatax.gov.cn/chinatax/n810356/n3010387/c5220435/content.html | verified_primary | 2026-09-02 | 国家税务总局 | official：小型微利企业减免企业所得税政策口径 |
| T06-S026 | https://www.irs.gov/publications/p538 | verified_primary | 2026-09-02 | IRS | official：Pub 538 会计期间与方法（cash vs accrual） |
| T06-S027 | https://www.ycombinator.com/blog/announcing-the-safe-a-replacement-for-convertible-notes | verified_primary | 2026-09-02 | Y Combinator | own publication：SAFE 发明者自述其取代可转债 |
| T06-S028 | https://www.ycombinator.com/documents | surrogate_primary | 2026-09-02 | Y Combinator | originator：post-money SAFE 标准文本与 primer |
| T06-S029 | https://pages.stern.nyu.edu/~adamodar/ | verified_primary | 2026-09-02 | Aswath Damodaran / NYU | 估值教学与数据集，DCF / WACC / ERP 一手 |
| T06-S030 | https://ocw.mit.edu/courses/15-401-finance-theory-i-fall-2008/ | verified_primary | 2026-09-02 | MIT OpenCourseWare | 课程 syllabus：NPV / IRR / WACC 讲义 |
| T06-S031 | https://www.cfainstitute.org/programs/cfa | verified_primary | 2026-09-02 | CFA Institute | official：CFA 项目覆盖范围 |
| T06-S032 | https://www.sba.gov/business-guide/manage-your-business/manage-your-finances | verified_primary | 2026-09-02 | US SBA | official：小企业现金流与财务管理官方指引 |
| T06-S033 | https://www.berkshirehathaway.com/letters/1986.html | verified_primary | 2026-09-02 | Warren Buffett | 「业主收益」owner earnings 的原始定义（1986 年报附录） |
| T06-S034 | https://sacks.substack.com/p/the-burn-multiple-51a7e43cb200 | verified_primary | 2026-09-02 | David Sacks | own publication：burn multiple 提出者本人原帖（2020-04） |
| T06-S035 | https://feld.com/archives/2015/02/rule-40-healthy-saas-company/ | surrogate_primary | 2026-09-02 | Brad Feld | own site：Rule of 40 原始博文（2015-02） |
| T06-S036 | https://www.bvp.com/atlas/cloud-computing-metrics | surrogate_primary | 2026-09-02 | Bessemer (BVP) | own publication：云公司五个会计指标 |
| T06-S037 | https://www.bvp.com/atlas/scaling-to-100-million | surrogate_primary | 2026-09-02 | Bessemer (BVP) | own publication：CAC 回本期分客群基准 |
| T06-S038 | https://www.bvp.com/atlas/cfo-playbook-mastering-metrics-and-managing-boards-for-saas-finance-success | surrogate_primary | 2026-09-02 | Bessemer (BVP) | own publication：SaaS CFO 指标与董事会沟通手册 |
| T06-S039 | https://carta.com/learn/equity/glossary/ | surrogate_primary | 2026-09-02 | Carta | vendor docs：股权与私募术语表 |
| T06-S040 | https://carta.com/learn/startups/equity-management/409a-valuation/ | surrogate_primary | 2026-09-02 | Carta | vendor docs：409A 估值定义与流程 |
| T06-S041 | https://carta.com/learn/equity/liquidity-events/liquidation-preferences/ | surrogate_primary | 2026-09-02 | Carta | vendor docs：参与型 / 非参与型优先清算权 |
| T06-S042 | https://carta.com/learn/startups/fundraising/priced-rounds/ | surrogate_primary | 2026-09-02 | Carta | vendor docs：定价轮 vs SAFE |
| T06-S043 | https://hbr.org/1991/05/profit-priorities-from-activity-based-costing | verified_primary | 2026-09-02 | Cooper & Kaplan / HBR | 作业成本法 ABC 的奠基文章（1991-05） |
| T06-S044 | https://hbswk.hbs.edu/item/rethinking-activity-based-costing | verified_primary | 2026-09-02 | HBS Working Knowledge | Kaplan 本人反思 ABC 的落地成本 |
| T06-S045 | https://bbrt.org/ | surrogate_primary | 2026-09-02 | Beyond Budgeting Institute | originator：超越预算 12 原则的发布机构 |
| T06-S046 | https://stripe.com/resources/more/essential-saas-metrics | surrogate_primary | 2026-09-02 | Stripe | vendor docs：SaaS 核心指标口径 |
| T06-S047 | https://stripe.com/resources/more/net-revenue-retention | surrogate_primary | 2026-09-02 | Stripe | vendor docs：NRR / NDR 定义 |
| T06-S048 | https://stripe.com/resources/more/what-is-annual-recurring-revenue-a-guide-for-saas-businesses | surrogate_primary | 2026-09-02 | Stripe | vendor docs：ARR 定义与常见误算 |
| T06-S049 | https://www.ifrs.org/issued-standards/list-of-standards/ias-7-statement-of-cash-flows/ | surrogate_primary | 2026-09-02 | IASB | originator：IAS 7 现金流量表三分类 |
| T06-S050 | https://www.ifrs.org/issued-standards/list-of-standards/ias-36-impairment-of-assets/ | surrogate_primary | 2026-09-02 | IASB | originator：IAS 36 资产减值与商誉测试 |
| T06-S051 | https://www.ifrs.org/issued-standards/list-of-standards/ias-38-intangible-assets/ | surrogate_primary | 2026-09-02 | IASB | originator：IAS 38 资本化 vs 费用化的判定 |
| T06-S052 | https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datacurrent.html | verified_primary | 2026-09-02 | Damodaran / NYU Stern | 行业 beta / WACC / 股权风险溢价公开数据集 |
| T06-S053 | https://www.court.gov.cn/zixun/xiangqing/199691.html | verified_primary | 2026-09-02 | 最高人民法院 | official：九民纪要全文 —— 对赌协议效力与可履行性 |
| T06-S054 | https://www.gov.cn/zhengce/zhengceku/202505/content_7022105.htm | verified_primary | 2026-09-02 | 六部门（央行牵头） | official：规范供应链金融业务通知，2025-06-15 施行 |
| T06-S055 | https://www.gov.cn/zhengce/202505/content_7022108.htm | verified_primary | 2026-09-02 | 中国政府网 | official：央行负责人就供应链金融通知答记者问 |
| T06-S056 | https://www.pbc.gov.cn/tiaofasi/144941/144979/3941920/5579680/2025020516345014304.pdf | verified_primary | 2026-09-02 | 中国人民银行 | official：供应链金融通知 PDF 原文 |
| T06-S057 | https://www.gov.cn/zhengce/zhengceku/2020-09/22/content_5546142.htm | verified_primary | 2026-09-02 | 八部门（央行牵头） | official：2020 年规范发展供应链金融的意见 |
| T06-S058 | https://www.imanet.org/certifications/cma-certification | surrogate_primary | 2026-09-02 | IMA | originator：CMA 覆盖的管理会计知识域 |
| T06-S059 | https://www.accaglobal.com/gb/en/qualifications/glance/acca/overview.html | surrogate_primary | 2026-09-02 | ACCA | originator：ACCA 资格覆盖范围 |
| T06-S060 | https://www.cicpa.org.cn/ | verified_primary | 2026-09-02 | 中国注册会计师协会 | official：中国 CPA 的法定主管协会 |
| T06-S061 | https://www.aicpa-cima.com/resources/landing/cpa-exam | surrogate_primary | 2026-09-02 | AICPA | originator：US CPA 考试范围 |
| T06-S062 | https://www.investopedia.com/terms/c/cashconversioncycle.asp | secondary | 2026-09-02 | Investopedia | 现金转换周期通用定义（仅作交叉参考，不作一手） |
| T06-S063 | https://www.npc.gov.cn/ | verified_primary | 2026-09-02 | 全国人大 | official：公司法等法律原文检索入口 |
| T06-S064 | https://fgk.chinatax.gov.cn/ | verified_primary | 2026-09-02 | 国家税务总局 | official：税收法规库，核查现行税率与优惠的唯一入口 |
| T06-S065 | https://venturehacks.com/option-pool-shuffle | surrogate_primary | 2026-09-02 | Venture Hacks (Nivi / Naval) | own site：「option pool shuffle」一词的原始出处与算例 |
| T06-S066 | https://sacks.substack.com/p/the-saas-metrics-that-matter | verified_primary | 2026-09-02 | David Sacks | own publication：SaaS 指标全景与优先级 |
| T06-S067 | https://www.bvp.com/atlas/state-of-the-cloud-2023 | surrogate_primary | 2026-09-02 | Bessemer (BVP) | own publication：云行业年度基准数据 |
| T06-S068 | https://www.law.cornell.edu/uscode/text/26/409A | verified_primary | 2026-09-02 | Cornell LII | 美国税法 IRC §409A 法条原文 |
| T06-S069 | https://www.ifrs.org/issued-standards/list-of-standards/ifrs-3-business-combinations/ | surrogate_primary | 2026-09-02 | IASB | originator：IFRS 3 企业合并与商誉的初始确认 |

---

## A. 高频术语 / 黑话（中英对照）

> 每条格式：**中文名 / 英文名（缩写）** → 一句话定义 → **真实使用场合** → **外行最容易搞错的地方**。
> 数字纪律：本节中出现的经验门槛均标注「业内经验值」并挂 source；无 source 的一律不给具体数字。

### A1. 三张表与勾稽（Financial Statements & Articulation）

**1. 权责发生制 / Accrual basis（权责）**
定义：收入在「赚到」的时点确认、费用在「发生」的时点确认，与钱什么时候进出账无关。
用在哪：对外报表、审计、投资人尽调一律用这个口径；准则要求的就是它 (evidence: [T06-S014, T06-S012])。
外行误区：以为「账上有多少钱」就是「赚了多少钱」。权责制下利润和现金可以长期背离 —— 这是所有后续误解的总源头。

**2. 收付实现制 / Cash basis（收付实现）**
定义：钱到账才算收入，钱付出才算费用。
用在哪：小微企业内部管钱、个体户税务口径、创始人自己算「这个月够不够发工资」。美国税法明确规定哪些纳税人可以用 cash method (evidence: [T06-S026])。
外行误区：以为「用收付实现制」是不正规。它在特定规模与特定用途下是合法且合适的；错的是**在需要权责口径的场合（对外报表、融资材料）拿收付实现的数字充数**。

**3. 毛利 / 毛利率 — Gross Profit / Gross Margin（GM）**
定义：收入减去「与收入直接相关的成本（COGS）」。毛利率 = 毛利 ÷ 收入。
用在哪：判断「这门生意本身成不成立」的第一道关；SaaS 公司算毛利率时必须把云成本、客户成功（支持性人力）、支付通道费算进 COGS，Bessemer 专门强调云公司的 COGS 口径 (evidence: [T06-S036])。
外行误区：把毛利率当成行业标签（「软件就是 80%」）。真正的问题是**你自己把什么放进了 COGS** —— 把实施团队、客服、服务器都挪到费用里，毛利率能凭空高 20 个百分点，而生意没变。

**4. EBIT / 息税前利润 — Earnings Before Interest and Taxes**
定义：利润表上剔除利息和所得税影响后的经营结果，近似于「主营业务本身赚的钱」。
用在哪：跨公司比较经营能力时用，因为资本结构（借了多少钱）和税率差异被剔除了。
外行误区：把 EBIT 当作「税前利润」。税前利润还含利息，EBIT 不含。

**5. EBITDA / 息税折旧摊销前利润**
定义：EBIT 再加回折旧与摊销。
用在哪：重资产行业估值、并购报价、银行看偿债能力时的通用语言。IFRS 18 生效后，「调整后 EBITDA」这类自定义小计将作为管理层定义的业绩指标（MPM）被强制披露口径并纳入审计 (evidence: [T06-S001, T06-S003])。
外行误区：**「EBITDA 就是现金流」是本行最经典的外行破绽。** EBITDA 完全不扣营运资金变动、不扣资本开支、不扣利息和税。一家应收账款暴涨、每年要换设备的公司，EBITDA 很好看，现金却在往外流。Buffett 在 1986 年就用「业主收益」这个概念点破了这一点：当维持性资本开支超过折旧摊销时，会计利润会**实质性高估**所有者实际赚到的钱 (evidence: [T06-S033])。

**6. 净利润 / Net Income（净利、税后利润）**
定义：所有收入减所有费用、利息、税之后的最终数字。
用在哪：分红基数、所得税汇算、股东回报口径。
外行误区：把净利润当成「可以拿走的钱」。净利润里含着还没收回的应收账款、还没卖掉的存货；能不能拿走要看现金流量表。

**7. 三类现金流 — 经营 / 投资 / 筹资（Operating / Investing / Financing Cash Flow, CFO / CFI / CFF）**
定义：IAS 7 规定现金流量表必须按经营、投资、筹资三类列报 (evidence: [T06-S049])；中国的一般企业财务报表格式同样如此 (evidence: [T06-S018])。
用在哪：看一家公司「靠什么活着」。经营现金流为正 = 生意自己造血；长期靠筹资现金流为正撑着 = 靠融资活着。
外行误区：只看「现金净增加额」这一个总数。总数为正可能是刚融了一笔钱，而经营现金流其实在大幅流出 —— 这两件事的含义天差地别。

**8. 自由现金流 / Free Cash Flow（FCF）**
定义：最常用的口径是经营现金流减去资本开支（CapEx）。注意这是一个**没有会计准则统一定义**的指标。
用在哪：估值（DCF 折的就是它）、判断公司有没有「真正可自由支配的钱」。
外行误区：以为 FCF 有唯一标准算法。不同人算的 FCF（是否扣利息、是否扣股权激励、是否扣租赁付款）差别巨大。SEC 的 Reg G 体系正是为了约束这类自定义指标的披露 (evidence: [T06-S011])。**问别人 FCF 数字时，正确的第一句话是「你的口径是什么」。**

**9. 业主收益 / Owner Earnings**
定义：Buffett 1986 年报附录给的定义 ——「(a) 报告的利润 加 (b) 折旧、折耗、摊销及若干其他非现金费用 减 (c) 年均资本化支出」 (evidence: [T06-S033])。
用在哪：老板视角判断「这门生意每年真正能给我多少可支配的钱」；小企业主评估收购标的时特别好用。
外行误区：把它和 EBITDA 混为一谈。两者的差别正好在最关键的一项 —— 业主收益**减去**维持性资本开支，EBITDA **加回**折旧摊销。方向完全相反。

**10. 递延收入 / 合同负债 — Deferred Revenue / Contract Liability**
定义：钱已经收了但服务还没提供完，这部分挂在**负债**里，随着履约逐期转成收入。新收入准则下中国报表科目称「合同负债」(evidence: [T06-S014, T06-S005])。
用在哪：所有预收模式（年费 SaaS、健身卡、教育培训、装修预付款）的公司每月关账都要算。
外行误区：**把递延收入当收入**。「我们今年签了 1200 万年费」和「我们今年确认了 1200 万收入」是两件事；如果合同是 12 月签的，当年只能确认一个月。反过来，把递延收入当「已经到手的利润」去发奖金，是中小企业现金崩盘的常见起点。

**11. 应计与预提 / Accruals（应计费用、预提费用）**
定义：服务已经消耗但账单还没到（如当月电费、当月已发生未结算的推广费），要在当期先计入费用并挂应付。
用在哪：月度关账的核心动作之一；不做应计，月度利润会被账单到达的节奏随机扰动。
外行误区：以为「没收到发票就不用记账」。这会导致月度利润忽高忽低，让所有的月度对比失去意义。

**12. 资本化 vs 费用化 / Capitalize vs Expense**
定义：一笔支出计入资产（分期摊到以后各期）还是一次性计入当期损益。IAS 38 规定了无形资产（含内部开发支出）的确认条件 (evidence: [T06-S051])。
用在哪：研发投入、自建软件、装修支出的会计处理。
外行误区：以为可以自由选择来「调节利润」。准则对资本化条件有明确限制；且这只影响利润的时间分布，**完全不改变现金流出**。把开发人员工资资本化能让今年利润好看，但公司账上的钱一分不多。

**13. 折旧与摊销 / Depreciation & Amortization（D&A）**
定义：把已经花掉的长期资产成本，按受益期分摊到各期的费用。
用在哪：制造业、有大量设备与门店装修的公司；也是 EBITDA 里被加回的那两项。
外行误区：把折旧当成「假费用」。折旧对应的现金**已经在过去付掉了**，而且未来还要再付一次（设备总要换）。这正是业主收益要减维持性资本开支的原因 (evidence: [T06-S033])。

**14. 商誉与减值 / Goodwill & Impairment**
定义：收购付出的价格超过被收购方可辨认净资产公允价值的部分记为商誉；商誉不摊销，但要定期做减值测试，IAS 36 规定了测试要求 (evidence: [T06-S050])。
用在哪：做了并购之后每年年末；也是上市公司「业绩暴雷」最常见的科目。
外行误区：把商誉当成一项「值钱的资产」。商誉是**买贵了的记账痕迹**，不能变现、不能抵押；它的唯一命运是要么被证明合理，要么被减值冲掉。

---

### A2. 营运资金与现金（Working Capital & Cash）

**15. 营运资金 / Working Capital（WC；营运资本）**
定义：流动资产减流动负债；日常口径更常用「经营性营运资金」= 应收 + 存货 − 应付。
用在哪：解释「为什么增长越快越缺钱」—— 增长意味着先垫应收和存货，钱回来在后面。
外行误区：以为「有利润就有钱」。营运资金占用是**利润与现金之间最大的那道闸门**。一家毛利健康、订单增长 100% 的公司，可能正因为营运资金被拉大而现金断裂。

**16. 现金转换周期 / Cash Conversion Cycle（CCC；现金周期）**
定义：CCC = DSO + DIO − DPO，即一块钱从变成存货到最终收回现金要多少天 (evidence: [T06-S062])。
用在哪：贸易、零售、制造、跨境电商的老板每月盯的核心数字。
外行误区：只盯毛利率不盯 CCC。同样的毛利率，CCC 从 90 天压到 45 天，等于凭空多出一半的经营资金 —— **这是不用融资的融资**。

**17. DSO / 应收账款周转天数 — Days Sales Outstanding**
定义：平均要多少天才能把卖出去的东西收回钱。
用在哪：销售政策与回款考核；给大客户的账期直接体现在这里。
外行误区：把 DSO 变差解释成「客户临时慢了」。DSO 系统性上升通常意味着**销售为了签单在偷偷放宽账期**，是收入质量下降的先行信号。

**18. DIO / 存货周转天数 — Days Inventory Outstanding**
定义：存货平均在仓库里躺多少天。
用在哪：任何有实物的生意；也是滞销与减值风险的先行指标。
外行误区：认为「有货才安全」。存货是**用现金买来的、还可能跌价的资产**；DIO 拉长几乎总是先于减值损失出现。

**19. DPO / 应付账款周转天数 — Days Payable Outstanding**
定义：你平均多少天付供应商的钱。
用在哪：与供应商谈判、CCC 优化。
外行误区：把「拖供应商」当成免费融资。拖账期通常会被供应商以更高的报价、更差的优先级和更低的配合度收回去 —— 成本只是从财务费用挪到了采购价里。

**20. 账龄 / Aging（账龄分析、账龄表）**
定义：按逾期时长把应收账款分档（如 30 天内 / 30-60 / 60-90 / 90 天以上）。
用在哪：每月催收会议、坏账准备计提。
外行误区：只看应收总额不看账龄结构。1000 万应收里有 300 万超过 90 天，和 1000 万全在 30 天内，是两家完全不同的公司。

**21. 烧钱率 / Burn Rate（净烧钱 net burn / 总烧钱 gross burn）**
定义：gross burn 是每月总的现金支出；net burn 是每月净减少的现金（支出减收到的钱）。
用在哪：创业公司董事会第一页；也是 burn multiple 的分子 (evidence: [T06-S034])。
外行误区：报数时不说是 gross 还是 net。两个数字可能差好几倍，投资人会立刻追问 —— **含糊其辞本身就是破绽**。

**22. 现金跑道 / Runway（跑道、还能活几个月）**
定义：账上现金 ÷ 月净烧钱率 = 还能撑几个月。
用在哪：融资节奏决策、招聘冻结决策。
外行误区：用「上个月的烧钱率」外推。跑道要用**未来的**烧钱率算，而未来的烧钱率会因为已经签下的合同、已经发出的 offer 而变。而且跑道要留出融资本身需要的时间（业内经验：融资从启动到到账通常按季度而非按周计）。

**23. 十三周滚动现金流 / 13-Week Cash Flow（13周表）**
定义：以周为颗粒度、滚动向前推 13 周（约一个季度）的现金收支预测，每周更新，滚掉最旧一周、补上最新一周。
用在哪：现金紧张期、重组期、银行或投资人要求加强监控时的标准工具；业内把它当作短期流动性管理的通行做法。美国小企业管理局（SBA）的官方小企业财务指引同样把现金流管理而非利润列为小企业存续的首要事项 (evidence: [T06-S032])。
外行误区：把它当成「月度预算的周版本」。13 周表的目的**不是准确，而是提前发现哪一周会见底**；它只记确定性的收支（已开票的应收、已签的付款、工资社保、税），不记乐观的销售预测。

**24. 保理 / Factoring 与供应链金融 / Supply Chain Finance**
定义：把应收账款转让或质押给金融机构提前拿到钱（保理）；或依托核心企业信用为其上下游中小企业融资（供应链金融）。
用在哪：账期长、下游是大企业的中小供应商。
中国监管现状：2025 年由中国人民银行牵头六部门发布《关于规范供应链金融业务 引导供应链信息服务机构更好服务中小企业融资有关事宜的通知》，**自 2025-06-15 起施行**，明确应收账款电子凭证付款期限原则上在 6 个月以内、最长不超过 1 年，融资须在央行征信中心动产融资统一登记公示系统登记，并规定供应链信息服务机构**未依法获得许可不得开展保理融资、贷款等金融业务**，设两年过渡期 (evidence: [T06-S054, T06-S055, T06-S056])。更早的框架性文件为 2020 年八部门《关于规范发展供应链金融 支持供应链产业链稳定循环和优化升级的意见》 (evidence: [T06-S057])。
外行误区：把保理成本只算利息。真实成本要算上手续费、追索权安排（有追索权 = 客户不付你还得还）、以及对客户关系的影响。

**25. 资金池 / Cash Pooling（资金归集）**
定义：集团把多个法人主体的账户资金集中调度，减少整体的闲置与借款。
用在哪：多主体、多店、多区域的公司。
外行误区：把资金池当成「钱可以随便调」。跨法人主体的资金往来涉及**关联方往来、利息定价、税务与法律合规**，处理不当会被认定为抽逃出资或产生税务风险。具体安排必须由持证专业人士设计，本文件不提供操作方法。

---

### A3. 成本与定价（Costing & Pricing）

**26. 固定成本 / 变动成本 — Fixed Cost / Variable Cost**
定义：变动成本随业务量同比例变化（原材料、支付通道费），固定成本在一定区间内不随业务量变（房租、管理人员工资）。
用在哪：所有「这单要不要接」「这个价能不能报」的判断。
外行误区：以为固定成本永远固定。它只在**一定业务量区间内**固定；超出产能就会阶梯式跳升（要多租一层楼、多开一条产线）。业内叫这种为阶梯式成本。

**27. 贡献边际 / Contribution Margin（CM；边际贡献）**
定义：收入减去**变动成本**。它衡量的是「每多做一单，能给固定成本和利润贡献多少」。
用在哪：淡季要不要接低价单、要不要停掉某条产品线、促销折扣的底线在哪。
外行误区：**把贡献边际和毛利混着说。** 毛利扣的是 COGS（里面通常含固定的制造费用、折旧、厂房），贡献边际扣的只有变动成本。用毛利做「接不接单」的决策会系统性拒绝掉本该接的单。

**28. 盈亏平衡点 / Break-even Point（BEP；保本点）**
定义：固定成本 ÷ 单位贡献边际 = 需要卖多少才不亏；或固定成本 ÷ 贡献边际率 = 需要多少收入才不亏。
用在哪：开新店、上新品、做产能决策时的第一个数。
外行误区：只算一个「保本销量」就完事。真正要问的是**保本点离你现在有多远**（安全边际），以及**保本点对价格的敏感度**（降价 10% 会让保本销量涨多少）。

**29. 经营杠杆 / Operating Leverage（经营杠杆度）**
定义：固定成本占比越高，收入的小幅波动会被放大成利润的大幅波动。
用在哪：解释「为什么我们收入只掉了 15%，利润就没了」；也解释软件公司在规模化后利润率的陡峭上升。
外行误区：只在顺风时理解它。高经营杠杆在下行期是同等强度的**放大器**，这是重资产、重团队公司在需求下滑时崩得特别快的原因。

**30. 标准成本与差异分析 / Standard Costing & Variance Analysis（标准成本法）**
定义：先设定单位产品的标准用料、标准工时、标准价格，实际发生后拆解差异（价格差异 vs 用量差异）。
用在哪：制造业、餐饮连锁（标准菜谱成本）、代工厂的月度成本复盘。
外行误区：把总成本超支笼统归因为「原材料涨价了」。差异分析的价值恰恰在于**把「买贵了」和「用多了」拆开** —— 前者是采购的问题，后者是生产的问题，处理方式完全不同。

**31. 作业成本法 / Activity-Based Costing（ABC）**
定义：不按销量或工时这类单一标准分摊间接费用，而是识别真正驱动费用发生的「作业」与「成本动因」，再按耗用量分摊 (evidence: [T06-S043])。
用在哪：产品线多、客户服务强度差异大的公司 —— 典型场景是「小客户订单量小但占用了大部分客服和物流资源」。
外行误区：以为 ABC 是「更精确所以更好」，忽略实施成本。Kaplan 本人后来公开反思过传统 ABC 在企业里维护成本过高、难以持续更新的问题 (evidence: [T06-S044])。中小企业更现实的做法是**只对少数关键决策做一次性的作业成本分析**，而不是重建整套核算体系。

**32. 成本加成定价 vs 价值定价 / Cost-plus vs Value-based Pricing**
定义：前者按成本加一个目标毛利率定价；后者按客户获得的价值 / 愿付价格定价。
用在哪：所有报价场景。
外行误区：把成本加成当成「公平」和「安全」。成本加成的隐含假设是「我的成本结构代表市场」，这在软件、设计、咨询这类边际成本极低的业务上会**系统性低估价格**；反过来在成本很高但价值有限的业务上又会报出卖不掉的价。

**33. 增量成本与沉没成本 / Incremental Cost & Sunk Cost**
定义：增量成本 = 因为做这个决策而额外多花的钱；沉没成本 = 已经花掉且无论如何都收不回的钱。
用在哪：要不要继续投一个项目、要不要清仓一批滞销货。
外行误区：**「我们已经投了 200 万，不能就这么算了」** —— 这是全世界最贵的一句话。已投入的 200 万与「接下来该怎么做」在逻辑上完全无关；唯一相关的是从现在往前看的增量收入与增量成本。同样，「用全成本分摊算下来淡季每单都亏，所以淡季停产」也是同一个错误的变体：**淡季只要单价高于变动成本，多做一单就多覆盖一分固定成本。**

---

### A4. 预算与 FP&A（Budgeting & Financial Planning and Analysis）

**34. 年度预算 / Annual Budget**
定义：把下一年的收入、成本、费用、投资、人力按月排成一张有约束力的计划表。
用在哪：年底的预算季；也是各部门费用审批的依据。
外行误区：把预算当成「目标」或「预测」。三者是三件事（见 D 节对照）。预算的本质是**资源分配的承诺**。

**35. 滚动预测 / Rolling Forecast（滚动预测、12 个月滚动）**
定义：不再只在年底做一次预测，而是每月或每季更新一次，永远向前看固定长度（如 12 个月）。
用在哪：变化快的行业、现金紧张期。Beyond Budgeting 的原则 7 与 9 主张动态、精简、无偏的预测过程，但**滚动预测只是实现方式之一，不是该框架规定的唯一做法** (evidence: [T06-S045])。
外行误区：以为滚动预测能取代预算。它取代的是「年度预测」，不是「资源分配的承诺」；很多公司上了滚动预测后费用失控，就是因为把承诺一起取消了。

**36. 零基预算 / Zero-Based Budgeting（ZBB）**
定义：每一期预算都从零开始论证每一笔支出的必要性，而不是在去年基础上加减百分比。
用在哪：成本结构需要一次性重构时（被收购后、大幅降本时）。
外行误区：把 ZBB 当成常规做法。它的论证成本极高，业内普遍的用法是**周期性地对特定费用类别做一次 ZBB**，而不是每年对所有科目做。

**37. 超越预算 / Beyond Budgeting（BB）**
定义：由 Beyond Budgeting Institute 提出的管理框架，共 12 条原则（6 条关于领导力、6 条关于管理流程），主张去中心化领导 + 自适应管理流程，反对把固定年度财务目标同时当成目标、预测和资源分配 (evidence: [T06-S045])。
用在哪：讨论「为什么我们的预算每年都是一场博弈」时的理论参照。
外行误区：以为它就是「不做预算」。它反对的是**把三种功能捆绑在一个数字上**，不是反对计划本身。

**38. 驱动因素模型 / Driver-based Model（驱动模型）**
定义：不直接拍收入数字，而是把它拆成可观测、可干预的业务驱动量（销售人数 × 人均线索 × 转化率 × 客单价）。
用在哪：任何要跟业务部门对齐的预算与预测。
外行误区：模型层数越多越好。层数多到业务负责人自己都说不清哪个数是他能管的，模型就失去了作用 —— **驱动模型的价值是「谁对哪个数负责」说得清**，不是精度。

**39. 方差分析 / Variance Analysis（差异分析、预实差异）**
定义：比较实际数与预算 / 预测数，逐项拆解差异原因（量差、价差、结构差、时间差）。
用在哪：月度经营分析会的主体内容。
外行误区：只报差异百分比不报原因归类。「营销费用超支 18%」是没有信息量的；「超支 18% 中，12% 是提前投放了下季度的预算（时间差），6% 是单次获客成本上升（价差）」才是能行动的。

**40. 预测准确度 / Forecast Accuracy（预测偏差 / bias）**
定义：预测值与实际值的偏离程度，通常同时看绝对误差与**系统性偏向**（长期偏乐观还是偏悲观）。
用在哪：评估 FP&A 团队与业务负责人的预测质量。
外行误区：只追求误差小。持续的**单向偏差**（永远高估收入）比误差大更危险，因为它会让所有基于预测的决策系统性地朝一个方向错。

**41. 月度关账 / Month-end Close（关账、结账）**
定义：每月固定时间内完成入账、应计、对账、调整，产出当期正式财务数据的流程。
用在哪：所有有财务团队的公司。业内常用「关账天数」作为财务基础能力的量化指标。
外行误区：以为关账慢只是财务效率问题。关账慢的真实后果是**管理层看到的永远是过时的数字**，做的所有决策都滞后一个周期。

**42. 管理报表包 / Management Reporting Pack（管报、月报包）**
定义：给管理层看的内部报表集合，通常包含损益、现金、关键经营指标、预实差异、以及一页文字解读。
用在哪：每月经营会。
外行误区：把管报做成法定报表的复制品。管报的口径**可以也应该**与法定报表不同（比如按业务线拆分、把股权激励和一次性项目单列），前提是口径稳定且可对账回法定报表。Bessemer 面向 SaaS CFO 的指标与董事会沟通手册给出了这类管报包的典型结构 (evidence: [T06-S038])。

**43. 财务 BP / Business Partnering（业务财务、财务 BP）**
定义：嵌到业务团队里、参与决策而不只是事后记账的财务角色。
用在哪：有一定规模后的组织设计。CMA（IMA 的管理会计师认证）覆盖的正是这类规划、预算与预测、绩效管理、决策分析的知识域 (evidence: [T06-S058])。
外行误区：以为 BP 就是「给业务做表的人」。BP 的核心职责是**在决策发生前提供反对意见**；一个从不说「不」的 BP 等于没有。


---

### A5. 单位经济与 SaaS 指标（Unit Economics & SaaS Metrics）

**44. 客户终身价值 / Lifetime Value（LTV，也写 CLV / CLTV）**
定义：一个客户在整个生命周期内预计带来的价值总和。
用在哪：判断获客花多少钱是划算的；决定要不要做长期合同。
外行误区：用**收入**而不是**毛利**算 LTV。正确做法是「毛利调整后的 LTV」（见第 53 条）。用收入口径算出来的 LTV/CAC 可能是真实值的三到五倍，会直接导致过度投放。

**45. 客户获取成本 / Customer Acquisition Cost（CAC）**
定义：获取一个新客户的平均成本。
用在哪：投放决策、销售团队扩编决策。
外行误区：CAC 分母里混入了**老客户续费带来的收入对应的销售成本**，或分子里漏掉了销售人员的工资与提成。CAC 只能用「获取新客户」的花费除以「新客户数」；把客户成功团队的成本算进 CAC 还是算进留存成本，业内本身有分歧，**关键是自己口径一致并说明**。

**46. CAC 回本周期 / CAC Payback Period（回本期）**
定义：要多久才能用这个客户贡献的毛利把获取他的成本赚回来。Bessemer 的表述是：**只有在 CAC 收回之后，这个客户才开始产生利润；在回本期内你只是在把花出去的钱收回来** (evidence: [T06-S037])。
用在哪：现金视角下最实用的单位经济指标 —— 它直接决定你需要多少营运资金来支撑增长。
业内经验基准（Bessemer 给云公司的目标值，**非普适标准**）：面向 SMB 客群 < 12 个月；面向中端市场 < 18 个月；面向企业级 < 24 个月 (evidence: [T06-S037])。
外行误区：只看 LTV/CAC 比值不看回本期。LTV/CAC = 3 但回本期 30 个月的生意，在现金上是**极度耗血**的；比值好看不代表你撑得到那一天。

**47. ARR / MRR — 年度经常性收入 / 月度经常性收入（Annual / Monthly Recurring Revenue）**
定义：订阅制业务中可预期重复发生的收入的年化 / 月度口径 (evidence: [T06-S048])。
用在哪：SaaS 公司对内对外沟通增长的默认单位。
外行误区：把一次性收入（实施费、定制开发费、硬件）算进 ARR。ARR 的全部意义在于「经常性」；掺进一次性收入后，这个数字既不能用来预测明年，也不能用来支撑估值倍数。另一个常见错误是**把 ARR 当成会计收入** —— ARR 是运营指标，不受收入准则约束，与利润表上的收入通常对不上 (evidence: [T06-S046])。

**48. 净收入留存 / 毛留存 — Net Dollar Retention（NDR / NRR）与 Gross Revenue Retention（GRR）**
定义：GRR 只看老客户流失和降级后还剩多少（上限 100%）；NDR 在此基础上加上老客户的扩容与升级（可以超过 100%） (evidence: [T06-S047], [T06-S036])。
用在哪：投资人尽调里权重最高的单一指标之一；David Sacks 在其 SaaS 指标全景中也把留存类指标排在优先级前列 (evidence: [T06-S066])，Bessemer 的年度云行业基准报告则提供了跨公司的对照区间 (evidence: [T06-S067])。Bessemer 的表述是毛留存理想上应在 90% 以上、净留存应在 100% 以上（**业内经验目标，非普适标准**） (evidence: [T06-S036])。
外行误区：只报 NDR 不报 GRR。NDR 130% 可能是「少数大客户疯狂扩容，同时一半小客户流失」；GRR 会把这个真相暴露出来。**只给 NDR 是行业内公认的选择性披露信号。**

**49. 流失 / Churn（客户流失率 vs 收入流失率）**
定义：客户流失率看走掉多少个客户；收入流失率看走掉多少钱 (evidence: [T06-S046])。
用在哪：留存分析、产品优先级。
外行误区：两者混用。走掉 30% 的客户但只丢了 5% 的收入（流失的都是小客户），和走掉 5% 的客户丢了 30% 的收入（流失的是头部客户），是完全不同的两种病。

**50. Rule of 40 / 四十法则**
定义：增长率 + 利润率 ≥ 40%。Brad Feld 在 2015 年的博文里把它写成「你的增长率加上利润应该等于 40%」，并明确说这是他从一位后期投资人那里听来的快速判断法 (evidence: [T06-S035])。
用在哪：后期融资、并购定价时的快速健康检查。
外行误区：**把它当成准则或标准去套早期公司。** Feld 本人写明这条规则是给**有规模的**公司用的（他的表述是假设至少 5000 万美元收入量级） (evidence: [T06-S035])。用它去评价一家 ARR 200 万的公司没有意义。另外「利润率」用哪个口径（EBITDA？FCF？经营利润？）本身就没有统一答案 —— **说 Rule of 40 时不说口径，就是外行。**

**51. 烧钱倍数 / Burn Multiple**
定义：David Sacks 提出，净烧钱 ÷ 净新增 ARR，衡量「每换来 1 块钱的新增经常性收入要烧掉几块钱」 (evidence: [T06-S034])。
用在哪：2022 年之后的融资环境里，这是替代「唯增长论」的核心效率指标。
外行误区：把它和 CAC 混同。CAC 只算获客花费，burn multiple 算的是**公司全部的净烧钱**（含研发、管理、一切）—— 它衡量的是整个公司的资本效率，而不只是市场营销的效率。

**52. Magic Number / 魔法数字（销售效率比）**
定义：本季度净新增 ARR ÷ 上季度销售与市场费用，衡量每投入 1 元销售市场费用带来多少新增 ARR；也有用季度收入增量年化的变体算法。
用在哪：判断销售组织该踩油门还是该修引擎。
外行误区：不注明用的是哪个变体。两种常见算法（季度 ARR 增量年化 ÷ 上季 S&M vs 净新增 ARR ÷ 上季 S&M）结果差 4 倍。**报这个数字必须同时报公式。**

**53. 毛利调整后的 LTV / Gross-margin-adjusted LTV**
定义：LTV = 客户平均月度收入 × **毛利率** ÷ 月度流失率（而不是用收入直接算）。
用在哪：所有严肃的单位经济讨论。
外行误区：见第 44 条。补充一点：**低毛利业务（硬件、履约密集型电商、有大量人力交付的服务）用收入口径算 LTV 会得出彻底失真的结论** —— 一个毛利率 20% 的生意，收入口径 LTV 会把真实值放大 5 倍。

---

### A6. 融资与股权（Financing & Equity）

**54. 投前估值 / 投后估值 — Pre-money / Post-money Valuation**
定义：投后估值 = 投前估值 + 本轮融资额。投资人拿到的比例 = 投资额 ÷ **投后**估值。
用在哪：每一次谈估值。
外行误区：说「我们估值 1 个亿」而不说是投前还是投后。融 2000 万时，投前 1 亿意味着让出约 16.7%，投后 1 亿意味着让出 20% —— **同一句话，两个结果**。这是本行最基础、也最常被外行漏掉的限定词。

**55. 稀释 / Dilution（摊薄）**
定义：新发股份导致原有股东持股比例下降。
用在哪：每一轮融资、每一次扩期权池。
外行误区：把稀释当成损失。**比例变小但绝对价值可能变大** —— 关键问题永远是「这次融资带来的价值增长，是否大于我让出的比例」。反过来，只盯着「不能被稀释」而错过必要的融资，是同一个错误的另一面。

**56. 期权池 / Option Pool 与「期权池洗牌」/ Option Pool Shuffle**
定义：预留给员工的股份池。「期权池洗牌」指投资人要求**在投前**（pre-money）就把扩大后的期权池放进股权表，这样扩池带来的稀释全部由创始人和老股东承担，新投资人不承担 —— 这个说法与算例最早由 Venture Hacks 系统化提出 (evidence: [T06-S065])。
用在哪：Term sheet 谈判的第二轮（第一轮谈估值，第二轮才发现期权池的位置改变了实际估值）。
外行误区：只看 term sheet 上的估值数字。期权池放在投前还是投后，会实质性改变创始人的有效估值。**正确的对抗方式不是砍池子大小，而是用具体的招聘计划来论证池子该多大，并争取把增量部分放到投后。**

**57. 优先股 / Preferred Stock（优先股、A 轮优先股）**
定义：投资人通常持有的股份类别，带有清算优先、反稀释、保护性条款、董事席位等一系列优于普通股的权利。
用在哪：所有机构融资。
外行误区：以为「一股就是一股」。创始人和员工持有的是**普通股**，投资人持有的是优先股，两者在退出时的分配次序完全不同 —— 这正是「公司卖了 1 亿，创始人一分钱没拿到」这类新闻的机制。

**58. 优先清算权 / Liquidation Preference（清算优先权）**
定义：公司清算或被出售时，优先股股东先按约定金额拿回钱，剩下的才轮到普通股 (evidence: [T06-S041])。
关键区分：
- **非参与型 / Non-participating**：投资人**二选一** —— 要么拿回优先金额，要么转成普通股按比例分，不能兼得 (evidence: [T06-S041])。
- **参与型 / Participating**：投资人先拿回优先金额，**然后还能**按比例参与剩余分配，业内直接叫「double dip（双重分配）」 (evidence: [T06-S041])。
- **带上限的参与型 / Capped participation**：参与部分封顶在优先金额的某个倍数（如 2 倍、3 倍） (evidence: [T06-S041])。
用在哪：Term sheet 里对退出结果影响最大的一条。
外行误区：只看倍数（1x / 2x）不看参与型与否。**1x 参与型在很多退出情形下比 2x 非参与型对创始人更不利** —— 只比倍数就是没看懂条款。

**59. 反稀释条款 / Anti-dilution Provision**
定义：下一轮估值低于本轮（down round）时，保护早期投资人不被贱价新股稀释的机制，常见有「完全棘轮 full ratchet」与「加权平均 weighted average」两类，后者又分广义与狭义。
用在哪：Term sheet；在下行周期里从睡眠条款变成活条款。
外行误区：签的时候觉得「反正我们不会降价融资」。完全棘轮在下行轮里对创始人的杀伤力极大，业内默认可接受的通常是**广义加权平均**。

**60. SAFE 与可转换债 / SAFE and Convertible Note**
定义：SAFE 由 Y Combinator 于 2013 年创设，是一份短合同：投资人现在出钱，换取未来在定价轮时按约定条件拿到股份的权利；YC 在 2018 年把标准形式改为 **post-money SAFE**，其好处是**能立刻精确算出卖掉了多少股权** (evidence: [T06-S027, T06-S028])。可转债则是先作为债务存在，到期或触发条件时转股。
用在哪：早期融资（种子轮及更早）。
外行误区：把 SAFE 当成「没稀释」。SAFE 的稀释是**延迟发生**的，一旦定价轮到来，之前所有 SAFE 一起转股，创始人常在这一刻才第一次看到真实的股权表。**多张不同估值上限的 SAFE 叠加，是创始人低估自身稀释最常见的原因。** 另一个误区：pre-money SAFE 与 post-money SAFE 在多轮叠加时结果差别很大 (evidence: [T06-S028, T06-S042])。

**61. 对赌 / 估值调整机制 — Valuation Adjustment Mechanism（VAM，业绩承诺、对赌协议）**
定义：投融资双方就未来业绩、上市时间等设定条件，未达成则由融资方回购股权或作现金补偿。
中国司法口径（这一条是中国特有的关键知识）：最高人民法院《全国法院民商事审判工作会议纪要》（法〔2019〕254 号，业内俗称「九民纪要」）区分了**协议效力**与**可履行性** —— 与目标公司对赌的协议在无法定无效事由时**有效**，但投资方请求目标公司回购股权的，法院要审查是否完成了减资程序，未完成则驳回；请求金钱补偿的，要按公司法关于利润分配的规定审查公司是否有可分配利润，没有或不足的应驳回或部分支持，公司未来有利润时可另行起诉 (evidence: [T06-S053])。九民纪要本身不是司法解释、不能直接作为裁判依据援引，但法院可在说理部分参照 (evidence: [T06-S053])。
外行误区：以为「签了对赌就一定要赔」或者「对赌一律无效」。真实答案是**有效但未必能执行，取决于程序与公司财务状况**。任何具体案件必须由执业律师判断。

**62. 回购条款 / Redemption Right（回购权）**
定义：投资人在约定期限内未实现退出时，要求公司或创始人按约定价格回购其股份的权利。
用在哪：中国市场的融资协议中极为常见。
外行误区：把「公司回购」和「创始人个人回购」当成一回事。前者受公司法减资程序与可分配利润限制（见上条；公司法原文可在全国人大官网检索 (evidence: [T06-S063])），后者是**创始人个人的无限责任**，两者的风险性质完全不同。签字前必须由律师逐字确认回购义务主体。

**63. 股权结构表 / Cap Table（Capitalization Table）**
定义：记录谁持有多少股份、什么类别、什么价格、什么时候取得的表格 (evidence: [T06-S039])。
用在哪：融资、期权授予、退出分配的唯一事实来源。
外行误区：以为 cap table 就是一张持股比例饼图。真正的 cap table 必须是**按类别、按轮次、含所有可转换工具（SAFE、可转债、期权、认股权证）的完全稀释口径**。只算已发行普通股的比例，在定价轮那天会被打脸。

**64. 退出瀑布 / Exit Waterfall（分配瀑布）**
定义：退出对价按清算优先权、参与条款、转股选择等规则逐层分配的计算过程。Carta 的表述是：**瀑布是估值中最重要的一块，因为它捕捉了内嵌的清算优先权** (evidence: [T06-S040])。
用在哪：任何一次「如果按 X 亿卖掉，我能拿多少」的严肃计算。
外行误区：用持股比例乘以售价。在有清算优先权的结构下，这个算法只在售价足够高时才近似成立；在中低价位退出时，普通股股东的实际所得可能远低于比例值，甚至为零。

**65. 409A 估值 / 409A Valuation**
定义：对私有公司**普通股**公允市场价值（FMV）的独立评估，主要用途是确定员工期权的最低行权价，以满足美国税法 §409A 的要求 (evidence: [T06-S040, T06-S068])。
用在哪：有美国实体、要给员工发期权的公司。
外行误区：把 409A 估值当成公司估值。409A 估的是**普通股**，通常显著低于投资人买优先股的价格；两者本来就应该不同，差价来自优先股的各项权利。**「我们 409A 只有融资价的三分之一，是不是被低估了」是典型外行提问。**

**66. ESOP 与员工持股平台 / ESOP and Employee Holding Vehicle（代持平台、持股平台）**
定义：ESOP 泛指员工股权激励计划；在中国常见的落地方式是设立有限合伙企业作为持股平台，由创始人担任 GP 控制投票权，员工作为 LP 享受经济利益。
用在哪：中国架构下的股权激励。
外行误区：把「代持」和「持股平台」混为一谈。**个人代持**（写在某人名下、靠一纸协议约定）存在继承、离婚、债务执行、代持人反悔等一系列风险；**有限合伙持股平台**是有工商登记的正式结构。另外，股权激励涉及个人所得税处理与工商登记，具体方案必须由律师与税务师设计 —— 本文件不提供具体操作方案。

---

### A7. 估值与资本（Valuation & Cost of Capital）

**67. 现金流折现 / Discounted Cash Flow（DCF）**
定义：把未来各期的自由现金流按折现率折回今天，加总得到内在价值。
用在哪：并购定价、重大投资决策、内部项目评估。
外行误区：以为 DCF 是「算出来的客观价值」。DCF 的结果对增长率假设和折现率高度敏感，**改两个小数点可以让估值翻倍**。内行用 DCF 的方式是反过来的：先看市场价格，再倒推「市场隐含了什么假设」，然后判断这些假设是否合理。

**68. 终值 / Terminal Value（TV）**
定义：预测期之后所有现金流的现值，通常用永续增长法（Gordon 模型）或退出倍数法估算。
用在哪：每一个 DCF 模型。
外行误区：不知道**终值通常占 DCF 总价值的绝大部分**。也就是说，一个五年期的 DCF，其结论主要由第五年之后的假设决定，而不是由你精心搭建的前五年明细决定。

**69. 加权平均资本成本 / Weighted Average Cost of Capital（WACC）**
定义：股权成本与债务成本按市值权重加权，得到公司整体的资金成本；DCF 中用作折现率。Damodaran 每年公开各行业的资本成本、beta 与股权风险溢价数据集 (evidence: [T06-S052, T06-S029])。
用在哪：折现率的确定、判断一个项目「值不值得做」的门槛收益率。
外行误区：以为「自有资金没有成本」。**股权是最贵的钱**（股东要求的回报高于债权人）。用「反正是自己的钱」来论证一个低回报项目，是中小企业最常见的资本配置错误。

**70. 股权风险溢价 / Equity Risk Premium（ERP）**
定义：投资股票相对无风险利率所要求的额外回报，是股权成本的核心组成部分 (evidence: [T06-S052])。
用在哪：算股权成本、算 WACC。
外行误区：直接照搬美国的数字用在中国或新兴市场标的上。Damodaran 的数据集专门区分了国别风险溢价 (evidence: [T06-S052])。

**71. Beta / β（贝塔系数）**
定义：衡量一项资产相对整体市场的系统性风险，用于 CAPM 计算股权成本。
用在哪：算折现率时。非上市公司通常取可比上市公司的 beta 去杠杆后再按自身资本结构加杠杆。
外行误区：给一家非上市中小企业硬套一个 beta 然后号称算出了「科学的折现率」。在实务中，中小企业的折现率更多是**由可获得的资金成本和机会成本决定的**，beta 只是参考。

**72. 可比公司倍数 / Comparable Company Multiples（EV/EBITDA、EV/Revenue、P/E）**
定义：用同类公司的市场定价倍数给标的定价。EV（企业价值）= 股权价值 + 净债务。
用在哪：快速定价、验证 DCF 结果是否离谱。
外行误区：**把 EV 倍数和股权价值倍数混用。** EV/EBITDA 得出的是企业价值，要减净债务才是股东能拿到的价值；P/E 得出的直接是股权价值。用 EV/EBITDA 算出 5 亿就说「我的公司值 5 亿」，忽略了 2 亿负债，是常见的自我高估。另一个误区是拿上市公司倍数直接套非上市公司，忽略流动性折价与规模折价。

**73. 净现值 / 内部收益率 / 回收期 — NPV / IRR / Payback Period**
定义：NPV 是按折现率折现后的净值（> 0 才做）；IRR 是让 NPV 为零的折现率；回收期是收回初始投资需要的时间 (evidence: [T06-S030])。
用在哪：设备投资、开新店、上新产线的立项评审。
外行误区：只看回收期不看 NPV。回收期完全忽略回本之后的现金流，会系统性偏向短平快项目。另一个误区是**在项目现金流正负交替时迷信 IRR** —— 那种情况下 IRR 可能有多个解或没有意义。

**74. 投入资本回报率 / 净资产收益率 — ROIC / ROE**
定义：ROIC 衡量公司用全部投入资本（股权 + 有息负债）创造的税后经营回报；ROE 衡量股东权益的回报。
用在哪：判断一门生意本身好不好（ROIC），以及杠杆对股东回报的影响（ROE）。
外行误区：只看 ROE 高就认为公司优秀。**ROE 可以靠加杠杆做高**，同时风险也在上升；ROIC 才是剥离了资本结构后的经营质量。**核心判断句：只有当 ROIC 持续高于 WACC 时，增长才在创造价值；ROIC < WACC 时，增长越快，毁灭的价值越多。**

**75. 经济增加值 / Economic Value Added（EVA，经济利润）**
定义：税后经营利润减去全部投入资本的机会成本（资本 × WACC）。
用在哪：事业部绩效考核、判断某块业务是否真的赚钱。
外行误区：把会计利润当成「赚钱」。会计利润里**不扣股权资本的成本**；一门年利润 500 万、占用了 1 亿资本的业务，在会计上赚钱，在经济上很可能在亏。这是「我们公司很赚钱」这句话最容易翻车的地方之一。

---

## B. 准则、法规与合规框架

> 每条标 `last_checked: 2026-09-02` 与 `Decay risk`。**税务与优惠政策 = high；IFRS / ASC 已生效准则 = low；IFRS 18 与 ISSB 的落地 = medium。**

### B1. 国际与美国（IFRS / ISSB / US GAAP / SEC）

#### B1-1. IFRS 15《客户合同收入》 / Revenue from Contracts with Customers

- **Type**: standard · **发布机构**: IASB（国际会计准则理事会）
- **Issued**: 2014-05 · **Effective**: 2018-01-01 起的年度期间
- **一句话**: 用「五步法」（识别合同 → 识别履约义务 → 确定交易价格 → 分摊交易价格 → 履约时确认收入）统一了全球收入确认口径 (evidence: [T06-S005, T06-S012])
- **对创始人真正的影响**: 「客户打款」不等于「可以确认收入」。年费预收、里程碑交付、多要素捆绑销售（软件 + 实施 + 服务）都要拆成履约义务分别确认 —— 这是递延收入科目在 SaaS 公司资产负债表上巨大的根本原因。
- **与 ASC 606 的关系**: IASB 与 FASB 联合项目，条文高度趋同，FASB 官方出过逐条对照 (evidence: [T06-S013])
- `last_checked: 2026-09-02` · **Decay risk: low**（已稳定生效 8 年以上）

#### B1-2. IFRS 16《租赁》 / Leases

- **Type**: standard · **发布机构**: IASB
- **Issued**: 2016-01 · **Effective**: 2019-01-01 起的年度期间
- **一句话**: 取消承租人的「经营租赁 / 融资租赁」二分，绝大多数租赁一律上表，确认使用权资产（right-of-use asset）与租赁负债 (evidence: [T06-S006])
- **对创始人真正的影响**: 长租办公室 / 门店 / 设备后，资产负债表会同时长出一块资产和一块负债，**资产负债率被动上升**，EBITDA 反而变好看（租金从经营费用变成折旧 + 利息）。跟银行谈贷款契约（covenant）时这一条经常引发误会。
- `last_checked: 2026-09-02` · **Decay risk: low**

#### B1-3. IFRS 18《财务报表列报和披露》 / Presentation and Disclosure in Financial Statements ★重点

- **Type**: standard · **发布机构**: IASB
- **Issued**: 2024-04 · **Effective**: **2027-01-01 起的年度报告期间**，允许提前采用；取代 IAS 1 (evidence: [T06-S001, T06-S002])
- **三个核心变化**:
  1. **利润表强制分类为经营 / 投资 / 融资三大类**，并强制列报规定的小计（如 operating profit），终结了各家自定义「营业利润」的乱象 (evidence: [T06-S001, T06-S003])
  2. **管理层定义的业绩指标（MPM, management-defined performance measures）必须披露并进入审计范围** —— 即企业在对外沟通中使用的、不由 IFRS 规定的收入费用小计（典型如「调整后 EBITDA」），必须在附注中说明口径、说明为什么用它、并与最接近的 IFRS 小计做调节 (evidence: [T06-S001, T06-S003])
  3. 对费用的汇总与分解（aggregation / disaggregation）提出更明确要求
- **为什么创始人要在意**: 这是把「调整后 EBITDA」从营销话术拉回准则约束的一步。IASB 明确说目的是提升 MPM 的**纪律性与透明度并使其可审计** (evidence: [T06-S002])。生效前这几年，融资材料里的「调整后」口径仍属自定义地带，**这正是外行最容易被数字牵着走的窗口期**。
- **落地仍在推进中**: IFRS 解释委员会对 MPM 的具体边界（如「假设性收入与费用」）仍在出暂定议程决定 (evidence: [T06-S004])
- `last_checked: 2026-09-02` · **Decay risk: medium**（未到生效日，实施指引仍在增补）

#### B1-4. IFRS S1 / IFRS S2（ISSB 可持续披露准则）

- **Type**: standard · **发布机构**: ISSB（国际可持续准则理事会，IFRS 基金会下设）
- **Issued**: 2023-06 · **Effective**: 2024-01-01 起的年度报告期间，需 S1 与 S2 同时采用 (evidence: [T06-S007, T06-S008, T06-S009])
- **一句话**: S1 是可持续相关财务信息的一般要求（治理 / 战略 / 风险管理 / 指标与目标四支柱），S2 专门讲气候，并整合了 TCFD 建议 (evidence: [T06-S009])
- **关键限定**: 准则本身**不自动具有法律强制力**，是否强制、从哪一年开始强制，由各法域自行立法 —— IFRS 基金会有专门页面按法域追踪采用进度 (evidence: [T06-S010])
- **对创始人真正的影响**: 短期不是中小企业的直接义务，但**通过供应链传导** —— 大客户 / 上市公司客户被要求披露范围三排放（Scope 3，即上下游价值链排放）时，会向供应商索要数据。这是「合规成本从大公司下渗到小供应商」的典型路径。
- `last_checked: 2026-09-02` · **Decay risk: medium**（法域采用状态每季度变化）

#### B1-5. US GAAP ASC 606（Topic 606，收入）

- **Type**: standard · **发布机构**: FASB（美国财务会计准则委员会）
- **Issued**: ASU 2014-09（2014-05） · 后续有 2016-08 / 2016-12 / 2016-20 等多个修订 ASU (evidence: [T06-S012])
- **一句话**: 美国版的五步法收入准则，核心原则是「按预期有权取得的对价金额确认收入」 (evidence: [T06-S012])
- **术语提醒**: 中国团队常把 ASC 606 与 IFRS 15 混着说。两者条文趋同但**不完全等同**，FASB 出过官方对照文件；做 VIE 架构 / 准备美股上市时这一差异会被审计师逐条追 (evidence: [T06-S013])
- `last_checked: 2026-09-02` · **Decay risk: low**

#### B1-6. SEC Regulation G 与非 GAAP 指标的合规边界

- **Type**: regulation · **发布机构**: 美国证券交易委员会（SEC）
- **Issued**: 2003（Sarbanes-Oxley 法案第 401(b) 条的落地规则） · 持续通过 C&DI（合规与披露解释）更新 (evidence: [T06-S011])
- **一句话**: 只要公开披露里出现非 GAAP 指标（调整后 EBITDA、调整后净利、自由现金流的自定义版本等），就必须**同时给出最接近的 GAAP 指标、给出逐项调节表、并说明为什么用它**；且不得让非 GAAP 指标比 GAAP 指标更突出 (evidence: [T06-S011])
- **对创始人真正的影响**: 这是全世界「调整后数字」的事实纪律模板。即使公司远没到上市，**投资人尽调时会拿 Reg G 的逻辑来质问你的调整项**：这笔调整是一次性的吗？未来还会发生吗？把经常性支出（如持续的招聘费、持续的市场投放）调出 EBITDA 是最常被抓的动作。
- **与 IFRS 18 的关系**: Reg G 管的是「披露时怎么说」，IFRS 18 的 MPM 是把同一件事写进会计准则本身 (evidence: [T06-S001, T06-S011])
- `last_checked: 2026-09-02` · **Decay risk: medium**（C&DI 不定期更新）

#### B1-7. IRS Publication 538 — 会计方法（收付实现 vs 权责发生）

- **Type**: regulation（税务口径） · **发布机构**: 美国国税局（IRS）
- **一句话**: 规定什么规模 / 什么类型的纳税人可以用收付实现制（cash method）、什么情况必须用权责发生制（accrual method） (evidence: [T06-S026])
- **为什么放进来**: 这是「同一家公司可以有两套合法口径」的最清晰例证 —— **会计口径与税务口径本来就不必相同**。中国同理（会计利润 vs 应纳税所得额需要纳税调整）。外行听到「两套账」就以为一定违法，其实合法的口径差异（税会差异）是常态，违法的是隐瞒收入与虚假凭证。
- `last_checked: 2026-09-02` · **Decay risk: high**（税法条款按年更新，门槛金额逐年通胀调整，必须查当年版本）

### B2. 中国（企业会计准则 / 税务 / 征管）

#### B2-1. 企业会计准则（CAS, Chinese Accounting Standards）体系

- **Type**: standard · **发布机构**: 中华人民共和国财政部会计司
- **一句话**: 由基本准则 + 40 余项具体准则 + 应用指南 + 解释构成，是中国境内执行企业会计准则的主体框架 (evidence: [T06-S014, T06-S015])
- **报表格式的官方口径**: 财政部单独发文规定「一般企业财务报表格式」，即资产负债表 / 利润表 / 现金流量表的具体行项 —— **中国的三张表长什么样是有法定模板的**，不是各家自己设计 (evidence: [T06-S018])
- `last_checked: 2026-09-02` · **Decay risk: low**（框架稳定，个别准则修订）

#### B2-2. CAS 14《收入》（修订版）

- **Type**: standard · **Issued**: 2017-07 修订印发
- **分批施行时间表** (evidence: [T06-S017]):
  - 境内外同时上市 + 境外上市且采用 IFRS / CAS 编表的企业：2018-01-01
  - 其他境内上市企业：2020-01-01
  - 执行企业会计准则的非上市企业：2021-01-01
- **一句话**: 中国版五步法，与 IFRS 15 趋同 (evidence: [T06-S014])
- **对创始人真正的影响**: 非上市公司从 2021 年起也在这套口径下了。「合同负债」（旧称预收账款）科目变大，是新准则下预收模式企业的正常现象，不是经营变差。
- `last_checked: 2026-09-02` · **Decay risk: low**

#### B2-3. CAS 21《租赁》（修订版）

- **Type**: standard · **Issued**: 2018-12 修订印发
- **分批施行** (evidence: [T06-S016]):
  - 境内外同时上市 + 境外上市且采用 IFRS / CAS 编表的企业：2019-01-01
  - 其他执行企业会计准则的企业：2021-01-01
- **一句话**: 与 IFRS 16 趋同，承租人单一模型，使用权资产与租赁负债入表 (evidence: [T06-S015])
- `last_checked: 2026-09-02` · **Decay risk: low`

#### B2-4. 《小企业会计准则》

- **Type**: standard · **发布机构**: 财政部 · **Issued**: 2011（财会〔2011〕17 号），2013-01-01 起施行
- **一句话**: 面向小企业的简化准则体系 —— 大量取消公允价值计量、简化减值处理，且**刻意向税法口径靠拢以降低税会差异的核算成本**
- **对创始人真正的影响**: 这是很多创业公司代账实际执行的准则。它的简化换来低成本，代价是**报表对内部管理的信息量偏低**（不做详细成本核算、不做递延处理），所以「用小企业会计准则出的报表」经常不足以支撑定价和产能决策，需要单独搭一套管理口径。
- **注意**: 融资时投资人常要求切换到《企业会计准则》并做追溯调整，这是尽调阶段常见的一笔隐藏成本。
- `last_checked: 2026-09-02` · **Decay risk: low`

#### B2-5. 小型微利企业所得税优惠（**有明确年限，务必按年核查**）

- **Type**: regulation · **发布机构**: 财政部 + 国家税务总局
- **政策依据**: 《关于进一步支持小微企业和个体工商户发展有关税费政策的公告》（**财政部 税务总局公告 2023 年第 12 号**） (evidence: [T06-S019])
- **口径（截至本文 last_checked 2026-09-02 的官方表述）**:
  - 小型微利企业**减按 25% 计算应纳税所得额，按 20% 税率**缴纳企业所得税，**执行至 2027-12-31** (evidence: [T06-S019, T06-S025])
  - 「小型微利企业」的官方三条件：从事国家非限制和禁止行业，且年度应纳税所得额 ≤ 300 万元、从业人数 ≤ 300 人、资产总额 ≤ 5000 万元 (evidence: [T06-S019, T06-S025])
  - 对增值税小规模纳税人、小型微利企业和个体工商户，2023-01-01 至 2027-12-31 减半征收资源税（不含水资源税）、城市维护建设税、房产税、城镇土地使用税、印花税（不含证券交易印花税）、耕地占用税和教育费附加、地方教育附加 (evidence: [T06-S019])
- **硬提醒**: 上述比例与门槛**均带有效期**，且历史上多次延长与调整。任何时点使用前必须回查 `fgk.chinatax.gov.cn` 法规库原文的最新公告，并由持证税务师确认适用性。**不要把这些数字写死在模型里而不注明年份与出处。**
- `last_checked: 2026-09-02` · **Decay risk: high**

#### B2-6. 研发费用加计扣除

- **Type**: regulation · **发布机构**: 财政部 + 国家税务总局（+ 科技部）
- **政策依据**: 《关于进一步完善研发费用税前加计扣除政策的公告》（**财政部 税务总局公告 2023 年第 7 号**） (evidence: [T06-S020])
- **口径（官方表述，2023-01-01 起，作为制度性安排长期实施）**:
  - 未形成无形资产计入当期损益的研发费用，在据实扣除基础上，**再按实际发生额的 100% 税前加计扣除**；形成无形资产的，按无形资产成本的 **200%** 税前摊销 (evidence: [T06-S020])
  - 可加计范围：人员人工、直接投入、折旧费用、无形资产摊销、新产品设计费 / 新工艺规程制定费 / 新药临床试验费 / 勘探开发现场试验费，以及其他相关费用 (evidence: [T06-S020, T06-S021])
  - **负面清单行业不适用**：烟草制造业、住宿和餐饮业、批发和零售业、房地产业、租赁和商务服务业、娱乐业 (evidence: [T06-S020])
- **对创始人真正的影响**: 这是技术型中小企业最实在的一项税收支持，但它对**费用归集的颗粒度**有硬要求 —— 研发工时、研发领料、研发人员名单要能拆出来。很多公司拿不到，不是不符合条件，而是**账做得太粗，事后无法归集**。执行指引 2.0 版是官方给的归集口径手册 (evidence: [T06-S021])
- `last_checked: 2026-09-02` · **Decay risk: high**（归集口径与申报表随年度更新）

#### B2-7. 全面数字化的电子发票（数电发票）与征管数字化

- **Type**: regulation · **发布机构**: 国家税务总局
- **时间线** (evidence: [T06-S022, T06-S023, T06-S024]):
  - 2021-12-01 广东、上海、内蒙古率先试点
  - 试点逐步扩至全国
  - **自 2024-12-01 起在全国正式推广应用**
- **官方定义**: 数电发票是《发票管理办法》中「电子发票」的一种，票面要素全面数字化、**号码全国统一赋予、开票额度智能授予**、信息通过税务数字账户在征纳双方之间自动流转；与纸质发票具有同等法律效力；号码为 20 位 (evidence: [T06-S023])
- **术语说明 —「金税四期」**: 这是业内与媒体的通俗叫法，指税务征管信息化的新阶段（以数治税、发票全面电子化、数据比对）。**它不是一份可以引用的官方文件名**，官方文件是上述数电发票公告与各项征管规定。用这个词时应意识到它是俗称。
- **对创始人真正的影响（合规视角，非规避视角）**: 额度由系统智能授予、进销项自动比对，意味着**收入与成本的证据链必须从一开始就真实一致**。历史上民营中小企业存在「两套账」（内账 / 外账口径不一致）的实务现象，其本质是账实不符，在征管数字化下暴露概率显著上升，且构成税务与法律风险。**正确路径是一套真账 + 合法的税会差异调整**，具体处理必须由持证税务师按当年法规判断。本文件不提供任何规避方法。
- `last_checked: 2026-09-02` · **Decay risk: high**

#### B2-8. 社保费征收职责划转（俗称「社保入税」）

- **Type**: regulation · **背景**: 2018 年《国税地税征管体制改革方案》确定将各项社会保险费交由税务部门统一征收，此后各地分步落地
- **对创始人真正的影响**: 工资总额与社保缴费基数的一致性成为可核查项。这直接影响**人力成本的真实口径** —— 很多早期公司的「人均成本」模型低估，是因为只算了到手工资，没算全额社保公积金与用工附加成本。做预算时人力成本应按**全成本口径（cost-to-company）**建模。
- **合规红线**: 缴费基数如何确定、有无过渡安排，属地差异大且按年变化，一律以当年当地税务机关公告为准并咨询持证专业人士。
- `last_checked: 2026-09-02` · **Decay risk: high**

#### B2-9. 高新技术企业认定对财务口径的要求

- **Type**: certification · **发布机构**: 科技部 + 财政部 + 国家税务总局（《高新技术企业认定管理办法》及工作指引）
- **一句话**: 通过认定的企业减按 15% 税率征收企业所得税（法定基准税率为 25%），认定有效期 3 年
- **对财务的真正要求**（这是它进入 glossary 的原因）: 认定标准包含**研发费用占销售收入的比例**（按销售收入规模分档）与**高新技术产品（服务）收入占企业当年总收入的比例**，两项都要求企业能在账上把研发费用与高新收入**单独归集并出具专项审计报告**。也就是说，高企认定实际上是一个**倒逼财务核算颗粒度**的制度。
- **硬提醒**: 具体比例分档、认定流程与后续管理条款随办法与指引修订，使用前查科技部 / 火炬中心与税务总局的现行文本。
- `last_checked: 2026-09-02` · **Decay risk: high**

#### B2-10. 增值税与企业所得税的基本框架（创始人需要的最小认知）

- **增值税（VAT）**: 中国的主体流转税，实行**销项税额 − 进项税额**的抵扣机制；纳税人分为一般纳税人与小规模纳税人两类，适用不同的计税方法。
  - **对创始人真正的影响**: 增值税**不是你的成本，是你代收代付的过手税**（除非你拿不到进项发票，那部分就变成真实成本）。把含税价当收入、把增值税当利润的减项，是最常见的两个方向相反的错误。**具体税率、征收率与优惠一律以当年官方公告为准。**
- **企业所得税（CIT）**: 法定基准税率 25%；符合条件的小型微利企业、高新技术企业等适用优惠（见 B2-5 / B2-9）。
  - **核心概念 — 税会差异**: 会计利润 ≠ 应纳税所得额。业务招待费、广告费、职工福利费等有扣除限额；罚款、部分捐赠不得税前扣除；亏损可结转弥补（结转年限有法定上限且特定类型企业有专门规定）。**这就是「账上赚钱但要交的税更多」的来源。**
- **硬提醒**: 本节**刻意不写具体税率与限额比例**，因为它们按年份与企业类型变化。查询入口：`https://fgk.chinatax.gov.cn/`（税收法规库）与 `https://www.chinatax.gov.cn/`。任何具体处理由持证税务师判断。
- `last_checked: 2026-09-02` · **Decay risk: high**

### B3. 职业资格与知识体系（仅作术语与体系来源，不做考证攻略）

| 资格 | 全称 | 发证 / 主办 | 覆盖什么 | 与本行业的关系 |
|------|------|------------|---------|---------------|
| **CPA（中国注册会计师）** | 注册会计师 | 中国注册会计师协会（CICPA） (evidence: [T06-S060]) | 会计、审计、财务成本管理、税法、经济法、战略 | **唯一拥有中国法定审计签字权**的资格。看重「对外报表的真实公允」 |
| **US CPA** | Certified Public Accountant | 美国各州会计委员会（州发证），AICPA 主管考试 (evidence: [T06-S061]) | US GAAP、审计、税法、商业环境 | 美股上市 / 美国实体架构时的对口资格 |
| **ACCA** | Association of Chartered Certified Accountants | ACCA（英国特许公认会计师公会） (evidence: [T06-S059]) | IFRS 体系为主，财务管理、审计、税务、战略商业报告 | 国际准则（IFRS）口径最强，跨境业务常见 |
| **CMA** | Certified Management Accountant | IMA（美国管理会计师协会） | **管理会计**：规划、预算与预测、绩效管理、成本管理、内控、财务分析、决策分析 | **与本文件范围最贴合的一张证** —— 它考的就是 FP&A、成本、内部决策，而非对外审计 |
| **CFA** | Chartered Financial Analyst | CFA Institute | 投资分析、估值、资产组合管理、道德准则 (evidence: [T06-S031]) | 覆盖 DCF / WACC / 可比公司倍数等估值语言，但**站在投资人视角而非企业内部视角** |

- **关键区分（这条本身就是一个外行破绽）**: CPA 是「对外证明报表可信」，CMA 是「对内帮管理层做决策」，CFA 是「站在外部投资人角度给资产定价」。三者不是难度阶梯，是**三个不同的岗位视角**。说「我们财务总监是 CPA，所以预算做得好」在逻辑上就是错位的 —— 审计训练和 FP&A 训练不是一回事。
- `last_checked: 2026-09-02` · **Decay risk: low**（资格体系稳定；具体科目设置有修订）

---

---

## C. 「一听就是外行」的破绽

> 这一节是给 Phase 2.5「行业表达 DNA」提取用的：外行说出下面这些话，行内人当场就知道对方没管过钱。每条给**正确说法**。

**C1. 把「利润」和「现金」当同一件事**
外行说法：「我们这个月赚了 30 万。」（指的是账上多了 30 万）
为什么露馅：权责发生制下利润和现金天然背离；一个月的利润数和一个月的现金变动数是两个独立的量 (evidence: [T06-S014, T06-S026])。
正确说法：「这个月确认了 30 万利润，但经营现金流是负的，因为应收增加了 50 万。」—— 内行永远把这两个数**分开报**。

**C2.「我们公司很赚钱，就是没钱」说不出下一句**
外行说法：说完这句就摊手，当成一个无解的怪现象。
为什么露馅：这句话描述的是一个有名字、有解法的问题 —— **营运资金占用**。
正确说法：「利润是正的但现金是负的，因为增长把钱压在了应收和存货里。看 CCC：DSO 从 45 天涨到 78 天，这就是钱去的地方。」问题定位到 DSO / DIO / DPO 三个数上，就变成可行动的了。

**C3.「EBITDA 就是现金流」**
外行说法：拿 EBITDA 当经营现金流用，或者说「我们 EBITDA 转正了，所以不烧钱了」。
为什么露馅：EBITDA 不扣营运资金变动、不扣资本开支、不扣利息和税。Buffett 早在 1986 年就指出，当维持性资本开支超过折旧摊销时，会计口径会**实质性高估**所有者真正赚到的钱 (evidence: [T06-S033])。IFRS 18 之所以要把这类自定义小计纳入强制披露与审计范围，动机正是提升其纪律性与透明度 (evidence: [T06-S001, T06-S002])。
正确说法：「EBITDA 转正了，但净烧钱还有每月 80 万，差额在营运资金和资本开支上。」

**C4. 把估值当身价**
外行说法：「他公司估值 5 个亿，他身价 5 个亿。」或者「我们估值 2 亿，所以我值 8000 万。」
为什么露馅：估值是**上一轮少数几个人在特定条件下、买特定股份类别（优先股）的边际定价**，不是全部股份都能按这个价卖出去。创始人持有的是普通股，退出时要走完清算优先权的瀑布 (evidence: [T06-S041, T06-S040])。409A 估值（普通股公允价值）系统性低于优先股融资价，正是这件事的制度化体现 (evidence: [T06-S040, T06-S068])。
正确说法：「上一轮投后估值 2 亿，我持有 40% 普通股；但按当前的清算优先权结构，如果按 8000 万卖掉，我实际能拿到的接近零。」

**C5. 把递延收入当收入 / 把预收款当利润**
外行说法：「我们今年签了 1200 万，收入 1200 万。」
为什么露馅：收入准则要求按履约进度确认，预收部分挂在合同负债（负债）里 (evidence: [T06-S014, T06-S005])。
正确说法：「我们今年签约额（bookings）1200 万，确认收入 380 万，合同负债余额 820 万。」—— **内行会自然地把签约额、确认收入、现金收款三个数分开说。**

**C6. 用全成本分摊得出「淡季停产」**
外行说法：「淡季每单摊下来都亏，所以停产 / 不接单。」
为什么露馅：把固定成本摊到单位上再和单价比，是**决策场景下用错了成本口径**。只要单价高于**变动成本**，多做一单就多覆盖一分固定成本。
正确说法：「淡季单价 80 元，单位变动成本 55 元，贡献边际 25 元。停产的话这 25 元也没有了，固定成本照样要付。所以只要不冲击旺季定价和产能，接。」

**C7.「融了一轮就安全了」**
外行说法：拿到 TS 或到账就当危机解除。
为什么露馅：融资只改变了跑道长度，没改变烧钱效率。而且这一轮带来的条款（清算优先权、回购权、对赌）会在未来某天变成新的约束 —— 在中国，回购与对赌的可执行性还受减资程序与可分配利润的司法审查 (evidence: [T06-S053])。
正确说法：「这一轮给了我们 18 个月跑道，按当前 burn multiple 2.8x 算，我们必须在第 9 个月前把它压到 1.5x 以内，否则下一轮谈不到更好的价。」

**C8. 报数字不带口径**
外行说法：「我们 ARR 1000 万」「毛利率 70%」「跑道 12 个月」——报完就停。
为什么露馅：这些指标全都没有统一定义。ARR 是否含一次性收入、毛利率的 COGS 边界在哪、跑道用的是 gross burn 还是 net burn，都会让同一家公司的数字差出几倍。SEC 的 Reg G 之所以要求非 GAAP 指标必须附调节表与最接近的 GAAP 指标，就是因为口径不明本身就是误导 (evidence: [T06-S011])。
正确说法：报数字时**主动**加限定 ——「ARR 1000 万，不含实施费；毛利率 70%，COGS 含云成本和客户成功团队；跑道 12 个月，按 net burn 算，不含已签未付的那笔设备款。」

**C9. 混用投前 / 投后估值**
外行说法：「我们估值 1 个亿。」
为什么露馅：融 2000 万时，投前 1 亿让出约 16.7%，投后 1 亿让出 20%。少一个词，结果差 3.3 个百分点的公司。
正确说法：永远说「投前 1 亿」或「投后 1.2 亿」。

**C10. 把「有订单」当成「有钱」**
外行说法：「我们手上有 3000 万订单，不缺钱。」
为什么露馅：订单要经过生产 / 交付 / 开票 / 账期才变成现金；订单越多，营运资金缺口反而越大。这正是「增长把公司拖死」的机制。
正确说法：「在手订单 3000 万，但按当前 CCC 108 天，执行这批订单需要先垫进去约 X 万营运资金，这是我们要融资的原因。」

**C11.「税后利润就是能分的钱」**
外行说法：「今年净利 500 万，分了吧。」
为什么露馅：净利里含未收回的应收和未卖出的存货；分红还要看**可分配利润**、法定公积金提取、以及公司未来的资本开支需要。在中国，公司向投资方作现金补偿时法院也要审查是否有可分配利润 (evidence: [T06-S053])。
正确说法：「净利 500 万，但经营现金流只有 180 万，明年还有一笔设备更新。今年先不分。」

**C12.「我们财务是 CPA，所以预算做得准」**
外行说法：把会计 / 审计能力和 FP&A 能力当成一回事。
为什么露馅：CPA 训练的是「对外证明报表可信」，CMA 训练的是「对内做规划、预算与决策分析」，CFA 训练的是「站在外部给资产定价」(evidence: [T06-S058, T06-S060, T06-S031])。三者是三种岗位视角，不是难度阶梯。
正确说法：「我们的会计核算很扎实，但没人做过驱动因素模型和滚动预测，这块要单独补。」

**C13.（中国特有）把「两套账」当成一种财务技巧**
外行说法：把内外账差异当作可以随意设计的东西来讨论。
为什么露馅：账实不符本身就是风险，且在征管数字化（数电发票全国推广、进销项自动比对、开票额度智能授予）下暴露概率显著上升 (evidence: [T06-S022, T06-S023])。内行会立刻把话题转向合规路径。
正确说法：「一套真账，税会差异在纳税调整里合法处理。具体适用哪些扣除和优惠，按当年官方公告由持证税务师确认。」—— **本文件不提供任何规避性操作方法。**

---

## D. 同名不同义 / 易混淆对照

**D1. 毛利 vs 贡献边际（Gross Profit vs Contribution Margin）**
- 毛利 = 收入 − COGS（COGS 里通常含固定的制造费用、折旧、场地）。
- 贡献边际 = 收入 − **变动成本**。
- 用途不同：毛利回答「这门生意的结构好不好」，贡献边际回答「这一单接不接、这个价降不降」。
- 混用后果：用毛利做接单决策会系统性拒掉本该接的单（见 C6）。

**D2. 现金流 vs 自由现金流 vs EBITDA**
- 现金流（通常指经营现金流 CFO）：IAS 7 定义的三类之一，实打实的现金进出 (evidence: [T06-S049])。
- 自由现金流 FCF：常见口径是 CFO − 资本开支，但**没有准则统一定义**，各家算法不同。
- EBITDA：利润表口径，不扣营运资金变动、不扣资本开支、不扣利息和税。
- 关系：三者依次离「真钱」越来越远。EBITDA 是最容易被包装的一个，也正因如此被 IFRS 18 的 MPM 规则和 SEC Reg G 盯上 (evidence: [T06-S001, T06-S011])。

**D3. 预算 vs 预测 vs 目标（Budget vs Forecast vs Target）**
- 预算：**资源分配的承诺** —— 你被批准可以花多少。
- 预测：**对现实的最好估计** —— 不带愿望，会随信息更新。
- 目标：**想达成的水平** —— 通常故意定得有挑战性。
- 混用后果：三者绑在一个数字上时，预测会被目标污染（永远偏乐观），预算会被当成目标（花不完就被砍，于是年底突击花钱）。Beyond Budgeting 的核心主张正是把这三种功能拆开 (evidence: [T06-S045])。

**D4. 估值 vs 市值 vs 身价（Valuation vs Market Cap vs Net Worth）**
- 估值：一级市场里少数投资人对**优先股**的边际定价。
- 市值：二级市场上全部流通股按当前价计算的总值，有真实的连续交易支撑。
- 身价：个人可变现的净资产，要经过清算优先权瀑布、锁定期、税、以及能否真的卖掉。
- 混用后果：见 C4。

**D5. 成本 vs 费用（Cost vs Expense）**
- 成本：与产出对象直接相关、可对象化的耗费（进入 COGS 或存货）。
- 费用：期间性耗费，与产出对象无直接关系（销售费用、管理费用、研发费用）。
- 关键：**同一笔支出放在成本还是费用里，毛利率会剧变，净利不变。** 这就是「毛利率不可跨公司直接比较」的根本原因（见 A1-3）。
- 相关的第三个概念：**资本化 vs 费用化** 决定的是同一笔支出**什么时候**进损益，与成本 / 费用的分类是两个独立的维度 (evidence: [T06-S051])。

**D6. 投前估值 vs 投后估值（Pre-money vs Post-money）**
- 投后 = 投前 + 本轮融资额；投资人比例 = 投资额 ÷ 投后。
- 延伸：**期权池放在投前还是投后**会实质改变创始人的有效估值 —— 这就是 option pool shuffle (evidence: [T06-S065])。
- 延伸二：pre-money SAFE 与 post-money SAFE 在多张叠加时的稀释结果差别很大；YC 2018 年改用 post-money 的理由就是**能立刻精确算出卖掉了多少股权** (evidence: [T06-S028])。

**D7. 参与型 vs 非参与型优先清算权（Participating vs Non-participating）**
- 非参与型：投资人**二选一** —— 拿回优先金额，或转普通股按比例分 (evidence: [T06-S041])。
- 参与型：先拿回优先金额，**再**按比例参与剩余分配，业内叫 double dip (evidence: [T06-S041])。
- 带上限的参与型：参与部分封顶在优先金额的若干倍 (evidence: [T06-S041])。
- 关键提醒：**只比 1x / 2x 的倍数而不看参与型与否，是看错了变量。** 在不少退出价位上，1x 参与型对创始人比 2x 非参与型更不利。

**D8. ARR vs 收入 vs 签约额（ARR vs Revenue vs Bookings）**
- ARR / MRR：运营指标，年化的经常性收入，不受会计准则约束 (evidence: [T06-S048])。
- 收入：会计指标，按 IFRS 15 / ASC 606 / CAS 14 的五步法在履约时确认 (evidence: [T06-S005, T06-S012, T06-S014])。
- 签约额 bookings：合同签下来的总金额，可能跨多年、可能还没开始履约。
- 混用后果：见 C5。**投资人尽调时会同时要这三个数并做交叉验证，三者对不上就是深挖信号。**

**D9. DSO / DIO / DPO 与 CCC**
- 三个是分项，CCC = DSO + DIO − DPO 是合成指标 (evidence: [T06-S062])。
- 常见混淆：把 CCC 改善归功于「回款变好了」，实际是靠拖长 DPO 拖出来的 —— **同样的 CCC 数字，来源不同，含义完全相反**（前者是能力，后者是在透支供应商关系）。

**D10. 商誉 vs 无形资产 vs 品牌价值**
- 商誉：收购对价超过可辨认净资产公允价值的差额，只在**企业合并**中产生，不摊销、要做减值测试 (evidence: [T06-S069], [T06-S050])。
- 无形资产：可辨认的（专利、软件、商标权），有确认条件，通常要摊销 (evidence: [T06-S051])。
- 品牌价值：**自创品牌不能入账**。一家公司账上没有品牌资产，不代表品牌不值钱；反过来，账上有大额商誉不代表品牌强，只代表以前买贵了。

**D11. 内部收益率 IRR vs 投资回报率 ROI vs 投入资本回报率 ROIC**
- IRR：带时间维度的年化收益率，用于项目立项 (evidence: [T06-S030])。
- ROI：不带时间维度的简单比值，说「回报 3 倍」时必须补上「用了几年」才有意义。
- ROIC：衡量存量业务用全部投入资本创造的经营回报，与 WACC 比较才有意义。
- 判断句：**ROIC > WACC，增长才创造价值；ROIC < WACC，增长越快毁灭越多。**

---

## Phase 2 提炼提示

**「行业表达 DNA」直接素材**：
- 高频黑话 top 10：现金跑道 runway、烧钱率 burn、贡献边际、CCC / DSO、递延收入（合同负债）、投前投后、清算优先权、稀释、burn multiple、关账。
- 行业拒绝的话术 top 5：「EBITDA 就是现金流」、「估值等于身价」、「融了就安全了」、「有订单就不缺钱」、无口径的「毛利率 70%」。
- 外行破绽 top 10：见 C 节 C1-C13，其中 C1 / C3 / C4 / C5 / C6 是最高频。

**「智识谱系」线索**：
- 准则演变路径：IAS 1 → **IFRS 18（2027 生效）**，反映的是「把管理层自定义指标纳入准则约束」这一范式转向 (evidence: [T06-S001])；ISSB S1/S2 反映「非财务信息进入财务报告体系」(evidence: [T06-S009])。
- 中国路径：分批施行的 CAS 14 / CAS 21 趋同于 IFRS (evidence: [T06-S017, T06-S016])，叠加征管数字化（数电发票全国推广）(evidence: [T06-S022])，方向是「口径国际化 + 征管数据化」两条腿。
- 流派之争：预算派 vs Beyond Budgeting 派 (evidence: [T06-S045])；增长优先 vs 效率优先（burn multiple / Rule of 40 的流行本身就是周期信号）(evidence: [T06-S034, T06-S035])。

**「时效性」信号（喂给诚实边界节）**：
- 预计 12-24 个月内会变的：中国税收优惠（小微政策现行执行至 2027-12-31）(evidence: [T06-S019])、研发费加计扣除的归集口径与申报表 (evidence: [T06-S021])、供应链金融通知的两年过渡期安排 (evidence: [T06-S054])、IFRS 18 的实施指引与 MPM 边界 (evidence: [T06-S004])、ISSB 各法域采用状态 (evidence: [T06-S010])。
- **本文件所有具体税率、门槛、比例都带年份与出处；使用者必须回查 `fgk.chinatax.gov.cn` 现行文本** (evidence: [T06-S064])。

**「工作流变化触发」种子（喂给 Track 03）**：
- 数电发票全国推广（2024-12-01 起）→ 开票、进项管理、月度关账流程重构 (evidence: [T06-S022])。
- 供应链金融通知（2025-06-15 施行，含 6 个月 / 最长 1 年付款期限与登记要求）→ 应收账款融资与账期管理流程重构 (evidence: [T06-S054])。
- IFRS 18（2027-01-01 生效）→ 采用 IFRS 的企业的利润表结构与「调整后」指标披露流程重构 (evidence: [T06-S001])。

**冷僻 / 信号薄弱评估**：**不冷僻。** 本行业术语总数 75 条（远超 40 的下限），准则法规条目 18 条且绝大多数有政府或准则机构原文，verified_primary 占比高。glossary 维度信号充分。

---

## 完成 checklist

- **Source 总数**：69 条（目标 50-80，达标）
- **术语条数**：**75 条**（A1 三张表 14 · A2 营运资金 11 · A3 成本定价 8 · A4 预算 FP&A 10 · A5 单位经济 10 · A6 融资股权 13 · A7 估值资本 9）—— 目标 40-60，超额完成
- **准则 / 法规 / 认证条数**：**18 条**（B1 国际与美国 7 · B2 中国 10 · B3 职业资格 5 张证并列为 1 条对照表），全部标注 `last_checked: 2026-09-02` 与 `Decay risk`
- **外行破绽条数**：**13 条**（目标 8-12，达标）
- **易混淆对照组数**：**11 组**（目标 6-10，达标）
- **bucket 分布**：`verified_primary` **34 条（49%）** · `surrogate_primary` **34 条** · `secondary` **1 条**（仅 Investopedia，作交叉参考，未单独支撑任何 claim） · `reference` 0 · `dead` 0
- **黑名单自检**：按 Track 06 规范的 7 个禁用平台正则全文扫描，**0 命中**（问答社区 / 公众号 / 百科 / 技术博客农场 / 短文平台 / 股票社区 / 财会网校营销页 均未出现在 manifest 或正文引用中）
- **合规红线**：涉及中国税务、发票、社保、两套账的部分，仅描述制度事实与风险，**未提供任何规避操作方法**，且全部指向官方公告与持证专业人士
- **数字纪律**：所有百分比 / 金额 / 天数均挂 source_id 或带「业内经验值」「约」「官方」等限定词；税率与门槛均写明公告文号与有效年份
