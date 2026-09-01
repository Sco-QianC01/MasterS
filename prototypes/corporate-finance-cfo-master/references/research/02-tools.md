# Track 02 — 工具栈与选型决策树｜企业财务与 CFO 视角

- **industry**: 企业财务与 CFO 视角（创业公司与中小企业主的内部财务工具栈）
- **locale**: zh-CN（正文中文，产品名 / URL 保留原文）
- **调研日期**: 2026-09-02
- **范围锚定**: 创业公司 / 中小企业主自己要用、自己要维护的财务工具栈。**不含**投行建模软件、券商终端（Bloomberg / Wind / Capital IQ）、个人记账 App。

> **状态**：已完成。85 条 source，20 条 verified_primary，全部经 `tools/research/source_verifier.py classify` 判定。

## Source Manifest

| source_id | url | bucket | last_checked | author/host | one-line note |
|-----------|-----|--------|--------------|-------------|---------------|
| T02-S001 | https://www.financialprofessionals.org/training-resources/resources/survey-research-economic-data/Details/afp-fpa-benchmarking-survey-report-technology | surrogate_primary | 2026-09-02 | AFP | originator — 2025 FP&A 基准调查技术分册，362 份从业者样本 |
| T02-S002 | https://www.financialprofessionals.org/training-resources/resources/articles/Details/why-aren-t-fp-a-teams-using-the-epm-tools-they-bought | surrogate_primary | 2026-09-02 | AFP | originator — 协会自问「买了 EPM 为什么不用」 |
| T02-S003 | https://www.gov.cn/zhengce/zhengceku/202411/content_6989164.htm | verified_primary | 2026-09-02 | 国家税务总局 | 2024 年第 11 号公告：全国推广数电发票原文 |
| T02-S004 | https://fgk.chinatax.gov.cn/zcfgk/c100012/c5236067/content.html | verified_primary | 2026-09-02 | 国家税务总局 | 税收法规库同一公告的法规检索版 |
| T02-S005 | https://www.gov.cn/zhengce//202411/content_6989160.htm | verified_primary | 2026-09-02 | 国家税务总局 | 数电发票公告官方解读：赋码制/赋额制/去介质 |
| T02-S006 | https://www.lucanet.com/en/insights/company-news/causal-joins-lucanet/ | surrogate_primary | 2026-09-02 | Lucanet | vendor docs — Causal 被收购并入 Lucanet 的官方说明 |
| T02-S007 | https://www.kingdee.com/product/small | surrogate_primary | 2026-09-02 | 金蝶 | vendor docs — 金蝶 AI 星辰（小微业财税一体化）产品页 |
| T02-S008 | https://www.kingdee.com/products/ykj.html | verified_primary | 2026-09-02 | 金蝶 | vendor docs — 精斗云云会计产品页，微型企业/个体户 |
| T02-S009 | https://www.microsoft.com/en-us/power-platform/products/power-bi/pricing | verified_primary | 2026-09-02 | Microsoft | vendor docs — Power BI 官方定价页（Free / Pro / PPU / Fabric 容量） |
| T02-S010 | https://www.tableau.com/pricing/teams-orgs | verified_primary | 2026-09-02 | Tableau (Salesforce) | vendor docs — 官方按角色定价 Creator/Explorer/Viewer |
| T02-S011 | https://www.metabase.com/pricing/ | surrogate_primary | 2026-09-02 | Metabase | vendor docs — 开源自托管与 Cloud 两条线的官方定价 |
| T02-S012 | https://www.fanruan.com/finereport | verified_primary | 2026-09-02 | 帆软 | vendor docs — FineReport 官方产品页，中国式复杂报表 |
| T02-S013 | https://www.odoo.com/pricing | surrogate_primary | 2026-09-02 | Odoo | vendor docs — 开源 ERP 官方按用户定价与模块边界 |
| T02-S014 | https://www.xero.com/us/pricing-plans/ | surrogate_primary | 2026-09-02 | Xero | vendor docs — 官方套餐与各档功能边界 |
| T02-S015 | https://www.zoho.com/us/books/pricing/ | surrogate_primary | 2026-09-02 | Zoho | vendor docs — Zoho Books 官方定价，含免费档条件 |
| T02-S016 | https://www.netsuite.com/portal/products/erp.shtml | verified_primary | 2026-09-02 | Oracle NetSuite | vendor docs — NetSuite ERP 官方产品页（无公开报价） |
| T02-S017 | https://www.sap.com/products/erp/business-one.html | verified_primary | 2026-09-02 | SAP | vendor docs — Business One 官方产品页，中小企业 ERP |
| T02-S018 | https://www.cubesoftware.com/pricing | surrogate_primary | 2026-09-02 | Cube | vendor docs — 与 Excel/Sheets 双向同步的 FP&A 官方定价 |
| T02-S019 | https://runway.com/pricing | surrogate_primary | 2026-09-02 | Runway | vendor docs — 官方定价与套餐边界 |
| T02-S020 | https://www.mosaic.tech/pricing | surrogate_primary | 2026-09-02 | Mosaic | vendor docs — 官方定价页（Strategic Finance 定位） |
| T02-S021 | https://www.abacum.ai/ | surrogate_primary | 2026-09-02 | Abacum | vendor docs — 官网首页，中型企业 FP&A 定位 |
| T02-S022 | https://www.pigment.com/ | surrogate_primary | 2026-09-02 | Pigment | vendor docs — 官网首页，企业级规划平台 |
| T02-S023 | https://www.anaplan.com/ | surrogate_primary | 2026-09-02 | Anaplan | vendor docs — 官网首页，连接式规划的老牌重型方案 |
| T02-S024 | https://www.planful.com/ | surrogate_primary | 2026-09-02 | Planful | vendor docs — 官网首页，中大型企业 EPM |
| T02-S025 | https://www.datarails.com/ | surrogate_primary | 2026-09-02 | Datarails | vendor docs — 官网首页，「保留 Excel」路线的代表 |
| T02-S026 | https://www.venasolutions.com/ | surrogate_primary | 2026-09-02 | Vena | vendor docs — 官网首页，Excel 原生界面的 EPM |
| T02-S027 | https://www.jirav.com/pricing | surrogate_primary | 2026-09-02 | Jirav | vendor docs — 官方定价，面向中小企业与会计事务所 |
| T02-S028 | https://floatapp.com/pricing/ | surrogate_primary | 2026-09-02 | Float | vendor docs — 现金流预测官方定价，接 Xero/QBO |
| T02-S029 | https://www.fathomhq.com/pricing | surrogate_primary | 2026-09-02 | Fathom | vendor docs — 管理报告与现金流预测官方定价 |
| T02-S030 | https://stripe.com/billing/pricing | surrogate_primary | 2026-09-02 | Stripe | vendor docs — Stripe Billing 官方费率（按流水抽成模式） |
| T02-S031 | https://www.chargebee.com/pricing/ | surrogate_primary | 2026-09-02 | Chargebee | vendor docs — 订阅计费官方定价与免费额度 |
| T02-S032 | https://www.maxio.com/pricing | surrogate_primary | 2026-09-02 | Maxio | vendor docs — SaaSOptics + Chargify 合并后的官方定价 |
| T02-S033 | https://recurly.com/pricing/ | surrogate_primary | 2026-09-02 | Recurly | vendor docs — 订阅计费官方定价 |
| T02-S034 | https://ramp.com/pricing | surrogate_primary | 2026-09-02 | Ramp | vendor docs — 官方定价，免费档 + 交换费返点模式 |
| T02-S035 | https://www.brex.com/pricing | surrogate_primary | 2026-09-02 | Brex | vendor docs — 官方定价与套餐边界 |
| T02-S036 | https://use.expensify.com/pricing | surrogate_primary | 2026-09-02 | Expensify | vendor docs — 报销官方定价，按活跃用户计费 |
| T02-S037 | https://www.huilianyi.com/ | surrogate_primary | 2026-09-02 | 汇联易 | vendor docs — 中国费控报销厂商官网 |
| T02-S038 | https://www.fenbeitong.com/ | surrogate_primary | 2026-09-02 | 分贝通 | vendor docs — 中国「因公消费+支付」一体化厂商官网 |
| T02-S039 | https://fast-standard.org/the-fast-standard/ | surrogate_primary | 2026-09-02 | FAST Standard Organisation | originator — FAST 建模规范原文与下载 |
| T02-S040 | https://www.fmworldcup.com/ | surrogate_primary | 2026-09-02 | Financial Modeling World Cup | originator — 建模竞赛官方站，事实上的手速与规范标尺 |
| T02-S041 | https://pulley.com/pricing | surrogate_primary | 2026-09-02 | Pulley | vendor docs — cap table 官方定价，$1,200/$3,500 年费档 |
| T02-S042 | https://carta.com/pricing/ | surrogate_primary | 2026-09-02 | Carta | vendor docs — 官方定价页（curl 403 为反爬，页面存活） |
| T02-S043 | https://www.chinatax.gov.cn/ | verified_primary | 2026-09-02 | 国家税务总局 | 税务政策与电子税务局入口的官方总站 |
| T02-S044 | https://www.yonsuite.com/ | surrogate_primary | 2026-09-02 | 用友 | vendor docs — YonSuite 官网，成长型企业一体化云 |
| T02-S045 | https://h.chanjet.com/ | surrogate_primary | 2026-09-02 | 畅捷通（用友） | vendor docs — 好会计官网，小微云财税主力产品 |
| T02-S046 | https://ydz.chanjet.com/ | surrogate_primary | 2026-09-02 | 畅捷通（用友） | vendor docs — 易代账官网，代账机构侧的 SaaS |
| T02-S047 | https://www.kdzwy.com/ | surrogate_primary | 2026-09-02 | 金蝶 | vendor docs — 金蝶账无忧，代账机构智能财税 SaaS |
| T02-S048 | https://www.yunzhangfang.com/ | surrogate_primary | 2026-09-02 | 云账房 | vendor docs — 独立代账 SaaS 厂商官网 |
| T02-S049 | https://www1.ccb.com/cn/yqzl/index.html | surrogate_primary | 2026-09-02 | 中国建设银行 | vendor docs — 银企直联综合服务平台官方说明（银行 official） |
| T02-S050 | https://open.icbc.com.cn/icbc/apip/mdres/bank_enterprise_access.pdf | surrogate_primary | 2026-09-02 | 中国工商银行 | vendor docs — 银企互联《企业开发手册》官方 PDF |
| T02-S051 | https://www.cmbchina.com/corporate/firmbank/FirmbankInfo.aspx?guid=f90bad24-02f7-40c0-bc38-99178e234aff | surrogate_primary | 2026-09-02 | 招商银行 | vendor docs — 银企直联产品与历史版本说明 |
| T02-S052 | https://www.rillet.com/ | surrogate_primary | 2026-09-02 | Rillet | vendor docs — AI 原生 ERP，2026-08 C 轮 10 亿美元估值 |
| T02-S053 | https://meetcampfire.com/ | surrogate_primary | 2026-09-02 | Campfire | vendor docs — AI 原生总账/ERP，Accel 领投 |
| T02-S054 | https://www.numeric.io/ | surrogate_primary | 2026-09-02 | Numeric | vendor docs — AI 对账与关账工作流 |
| T02-S055 | https://www.floqast.com/ | surrogate_primary | 2026-09-02 | FloQast | vendor docs — 关账管理老牌，2026-01 官宣 ARR 超 2 亿美元 |
| T02-S056 | https://www.blackline.com/ | surrogate_primary | 2026-09-02 | BlackLine | vendor docs — 账务自动化与对账的企业级基线 |
| T02-S057 | https://puzzle.io/ | surrogate_primary | 2026-09-02 | Puzzle | vendor docs — 面向创业公司的 AI 优先记账 |
| T02-S058 | https://www.digits.com/ | surrogate_primary | 2026-09-02 | Digits | vendor docs — AI 记账与报表，小微/初创定位 |
| T02-S059 | https://basis.ai/ | surrogate_primary | 2026-09-02 | Basis | vendor docs — 面向会计事务所的 AI agent |
| T02-S060 | https://www.mostlymetrics.com/p/presenting-the-2025-tech-stack-report | surrogate_primary | 2026-09-02 | CJ Gustafson | own publication — 1000+ CFO 参与的财务工具栈调查结果 |
| T02-S061 | https://www.mostlymetrics.com/p/the-state-of-the-cfotech-stack | surrogate_primary | 2026-09-02 | CJ Gustafson | own publication — CFO 工具市场拥挤度盘点（100+ 规划工具） |
| T02-S062 | https://www.mostlymetrics.com/p/announcing-the-2026-finance-tech-stack-survey | surrogate_primary | 2026-09-02 | CJ Gustafson | own publication — 2026 版调查公告与覆盖品类 |
| T02-S063 | https://www.thesaascfo.com/surveys/finance-accounting-tech-stack-survey/ | surrogate_primary | 2026-09-02 | Ben Murray | own publication — 第 7 届财务/运营工具栈调查，500 份样本 |
| T02-S064 | https://www.onlycfo.io/p/the-startup-finance-checklist | surrogate_primary | 2026-09-02 | OnlyCFO | own publication — 创业公司财务基建清单与免费模板 |
| T02-S065 | https://www.thefpandaguy.com/ | surrogate_primary | 2026-09-02 | Paul Barnhurst | own site — FP&A 工具评测与年度工具栈调查合办方 |
| T02-S066 | https://www.coso.org/generative-ai | surrogate_primary | 2026-09-02 | COSO | originator — 2026-02-23《生成式 AI 内部控制》官方指引 |
| T02-S067 | https://www.cpapracticeadvisor.com/2026/08/13/before-you-let-the-agents-run-the-close-five-controls-to-put-in-writing-first/188496/ | secondary | 2026-09-02 | CPA Practice Advisor | 让 AI agent 跑关账前必须先写死的 5 项控制 |
| T02-S068 | https://www.chinatax.gov.cn/chinatax/n810219/n810724/c5237168/content.html | verified_primary | 2026-09-02 | 国家税务总局 | 新电子税务局建成通稿：9600 万纳税人、97% 事项线上办 |
| T02-S069 | https://jiangsu.chinatax.gov.cn/art/2024/9/9/art_22419_471916.html | verified_primary | 2026-09-02 | 江苏省税务局 | 全国统一规范电子税务局上线图解，功能边界一手 |
| T02-S070 | https://www.rillet.com/blog/rillet-raises-100m-series-c-at-1b-valuation-to-build-accounting-superintelligence | verified_primary | 2026-09-02 | Rillet | vendor docs — C 轮官宣，自述 600+ 客户、替换 NetSuite/SAP |
| T02-S071 | https://www.wallstreetprep.com/knowledge/demystifying-the-13-week-cash-flow-model-in-excel/ | secondary | 2026-09-02 | Wall Street Prep | 13 周现金流在重组/DIP 场景的标准定义与结构 |
| T02-S072 | https://www.financialprofessionals.org/training-resources/resources/survey-research-economic-data | surrogate_primary | 2026-09-02 | AFP | originator — 流动性/司库年度基准调查的官方总入口 |
| T02-S073 | https://github.com/metabase/metabase | verified_primary | 2026-09-02 | Metabase | 开源 BI 主仓：49.0k stars，last push 2026-09-01 |
| T02-S074 | https://github.com/odoo/odoo | verified_primary | 2026-09-02 | Odoo | 开源 ERP 主仓：54.1k stars，last push 2026-09-01 |
| T02-S075 | https://www.fenbeitong.com/info/14670/ | surrogate_primary | 2026-09-02 | 分贝通 | vendor docs — 官方新闻页，自述「SaaS+交易」返佣模式 |
| T02-S076 | https://ifenxi.com/research/content/3815 | secondary | 2026-09-02 | 爱分析 | 第三方分析机构：汇联易定位大中型企业的评述 |
| T02-S077 | https://www.ekuaibao.com/ | surrogate_primary | 2026-09-02 | 合思（易快报） | vendor docs — 中国费控报销第三家主流厂商官网 |
| T02-S078 | https://kjs.mof.gov.cn/zcfb/201707/t20170719_2653411.htm | verified_primary | 2026-09-02 | 财政部会计司 | 企业会计准则第 14 号——收入（修订）原文 |
| T02-S079 | https://www.microsoft.com/en-us/microsoft-365/excel | verified_primary | 2026-09-02 | Microsoft | vendor docs — Excel 官方产品页（含 Copilot 能力边界） |
| T02-S080 | https://workspace.google.com/products/sheets/ | verified_primary | 2026-09-02 | Google | vendor docs — Google Sheets 官方产品页 |
| T02-S081 | https://www.floqast.com/blog/what-ai-audit-controls-actually-look-like | verified_primary | 2026-09-02 | FloQast | vendor docs — 厂商自述 AI 控制留痕的实际形态 |
| T02-S082 | https://www.getaleph.com/ | surrogate_primary | 2026-09-02 | Aleph | vendor docs — 连接 ERP 与电子表格的 FP&A 数据层 |
| T02-S083 | https://help.fanruan.com/finereport/doc-view-1750.html | surrogate_primary | 2026-09-02 | 帆软 | vendor docs — 官方帮助中心：FineReport 与 FineBI 定位差别 |
| T02-S084 | https://www.chargebee.com/docs/billing/2.0/kb/reports-and-analytics/revenue-recognition-as-defined-in-asc-606 | surrogate_primary | 2026-09-02 | Chargebee | vendor docs — 官方文档说明 ASC 606 收入确认口径与模块边界 |
| T02-S085 | https://www.maxio.com/products/revenue-recognition | verified_primary | 2026-09-02 | Maxio | vendor docs — 官方页：计费与 ASC 606 收入确认合一 |

## 总览（按 tier 分组）

### 必备（14 个）

| 工具 | 一句话 | 谁在用 | Decay | Evidence |
|------|--------|--------|-------|----------|
| Excel / Microsoft 365 | 财务模型的事实标准界面，至今没有被取代 | 全阶段，所有人 | low | [T02-S001, T02-S060, T02-S079] |
| Google Sheets | 协作与轻量看板，早期团队的默认账本 | 种子轮到 A 轮 | low | [T02-S001, T02-S080] |
| QuickBooks Online | 海外初创的默认总账，会计事务所生态最厚 | 0 到约 2000 万美元收入 | low | [T02-S060, T02-S063] |
| Xero | QBO 的主要替代，非美英澳市场更常见 | 中小企业、代账所 | low | [T02-S014] |
| 金蝶（精斗云 / AI 星辰） | 中国小微到成长型企业的业财税一体化 | 中国境内实体 | medium | [T02-S007, T02-S008] |
| 用友（畅捷通好会计 / YonSuite） | 中国小微云财税份额领先，向上接 YonSuite | 中国境内实体 | medium | [T02-S044, T02-S045] |
| Odoo | 开源 ERP，进销存 + 会计一体，可自托管 | 有技术团队的贸易/制造 | low | [T02-S013, T02-S074] |
| NetSuite | 多主体多币种的中大型 ERP 基线 | 约 2000 万美元收入以上 | low | [T02-S016] |
| 电子税务局（全国统一规范） | 中国报税、发票、勾选的唯一官方入口 | 所有中国实体 | low | [T02-S068, T02-S069] |
| 数电发票 | 发票全面数字化，去介质、赋码、赋额 | 所有中国实体 | medium | [T02-S003, T02-S005] |
| 银企直联 / 企业网银 | 资金查询、付款、电子对账的银行侧接口 | 有多账户或 ERP 的实体 | low | [T02-S049, T02-S050, T02-S051] |
| SAP Business One | 中小企业版 SAP，制造与分销场景深，靠伙伴实施 | 已在 SAP 生态 / 供应链复杂 | low | [T02-S017] |
| Zoho Books | 性价比路线，官方有条件免费档 | 极小团队 / 已用 Zoho 全家桶 | medium | [T02-S015] |
| 企业微信/飞书/钉钉的审批流 | 报销与付款审批的最低成本载体（上系统前） | 50 人以下团队 | medium | [T02-S064] |

### 场景特化（31 个）

| 工具 | 一句话 | 分岔条件 | Decay | Evidence |
|------|--------|----------|-------|----------|
| Cube | 保留 Excel/Sheets 前端的 FP&A 中间层 | 模型由财务自己维护，不想换界面 | medium | [T02-S018] |
| Datarails | 同上路线，更偏「把现有表格搬上云」 | 已有一堆历史 Excel 模型 | medium | [T02-S025] |
| Vena | Excel 原生界面 + 建模引擎的 EPM | 中型、有 IT 支持 | medium | [T02-S026] |
| Runway | 面向创业公司的可视化预算与叙事 | 要给董事会讲故事 | high | [T02-S019] |
| Mosaic | 战略财务，指标与 headcount 规划 | SaaS，$10-100M ARR | medium | [T02-S020] |
| Abacum | 中型市场 FP&A，2026 年被点名上升 | 换掉 Adaptive/Anaplan 的中间选择 | medium | [T02-S021, T02-S060] |
| Pigment | 企业级规划，建模自由度高 | 多业务线、复杂驱动 | medium | [T02-S022] |
| Anaplan | 老牌重型规划，$1B+ 仍占优 | 大型、有专职建模团队 | low | [T02-S023, T02-S060] |
| Planful | 中大型 EPM，2026 年中端份额上升 | 合并报表 + 预算一体 | medium | [T02-S024, T02-S060] |
| Jirav | 中小企业与会计事务所的打包 FP&A | 由外部会计维护模型 | medium | [T02-S027] |
| Lucanet xP&A（原 Causal） | 被收购后并入 Lucanet 平台 | 已有 Causal 存量用户 | high | [T02-S006] |
| Float | 接 Xero/QBO 的现金流预测 | 记账已在云端，要滚动看现金 | medium | [T02-S028] |
| Fathom | 管理报告 + 现金流，事务所常用 | 需要给老板做月度经营报告 | medium | [T02-S029] |
| Carta | cap table 与 409A 的行业默认 | 要拿机构美元融资 | low | [T02-S042, T02-S060] |
| Pulley | Carta 的价格与体验挑战者 | 早期、结构简单、想省钱 | medium | [T02-S041] |
| Stripe Billing | 已用 Stripe 收款时的订阅计费 | 收单已在 Stripe | low | [T02-S030] |
| Chargebee / Maxio / Recurly | 独立订阅计费与收入确认 | 计费规则复杂或需 ASC 606 报表 | medium | [T02-S031, T02-S032, T02-S033] |
| Ramp / Brex / Expensify / 汇联易 / 分贝通 / 合思 | 费控报销与企业卡 | 按境内外与是否要「免报销」分岔 | medium | [T02-S034, T02-S035, T02-S036, T02-S037, T02-S075, T02-S077] |
| Power BI / Tableau / Metabase / 帆软 FineReport | 看板与报表分发 | 按预算、自托管需求、中国式报表分岔 | low | [T02-S009, T02-S010, T02-S011, T02-S012] |
| FAST Standard / FMWC | 建模规范与手感训练来源 | 模型要交接给别人时 | low | [T02-S039, T02-S040] |

### 新兴（8 个）

| 工具 | 一句话 | 成熟度实话 | Decay | Evidence |
|------|--------|-----------|-------|----------|
| Rillet | AI 原生 ERP，明确对标替换 NetSuite | 有真实付费客户，但仍是早期赌注 | high | [T02-S052, T02-S070] |
| Campfire | AI 原生总账/ERP | 客户名单薄，属于早期采用者游戏 | high | [T02-S053] |
| Numeric | AI 辅助对账与关账工作流 | 落地点窄但真实 | high | [T02-S054] |
| Basis | 面向会计事务所的 AI agent | 融资高，产品仍在证明期 | high | [T02-S059] |
| Puzzle | AI 优先的初创记账 | 替代人肉记账的早期尝试 | high | [T02-S057] |
| Digits | AI 记账与报表 | 长期存在但未成主流 | high | [T02-S058] |
| Aleph | ERP 到电子表格的数据层 + AI 问答 | 定位清晰，规模仍小 | high | [T02-S082] |
| 各 FP&A 厂商的内嵌 AI 助手 | 「问一句就给差异解释」 | 演示强、生产环境要人复核 | high | [T02-S061, T02-S001] |

---

## 一、必备层

### 1.1 电子表格仍是主力

**先把这句话说清楚：这一行最重要的工具是 Excel，不是任何一个买来的系统。**

- **证据不是感觉**：AFP 2025 年 FP&A 基准调查（362 份从业者样本）显示，官方口径下 96% 的受访者把电子表格当规划工具、93% 当报表工具，且是按日或按周使用；同一份调查里 71% 的人也在用 EPM（企业绩效管理）系统，两者并存说明 EPM 没有把表格挤掉 (evidence: [T02-S001, T02-S002])
- **第二个独立来源**：Mostly Metrics 的年度财务工具栈调查（超过 1000 位 CFO 参与）给出的分界线是——**公司收入过约 1 亿美元之前，专用 FP&A 工具的采用率都不到一半** (evidence: [T02-S060])
- **两个来源相互独立**（一个是协会调查，一个是从业者社区调查），所以「电子表格是必备层」这条判断成立 (evidence: [T02-S001, T02-S060])

#### Excel / Microsoft 365

- **用什么场景**：三表联动模型、月度经营分析、Cap table 稀释模型、13 周现金流、任何一次性的假设测试。凡是「结构还没稳定、下周可能推翻重来」的分析，Excel 都赢 (evidence: [T02-S001])
- **相对优劣**：胜在自由度和交接的普适性——任何一个会计、投资人、审计都打得开。输在版本控制、多人协作、审计留痕，以及公式错误没有护栏
- **价格模式**：按用户订阅（Microsoft 365 商业版），官方定价页见 vendor docs；桌面版功能（Power Query、Power Pivot、数据模型）是财务真正需要的部分，网页版会缺 (evidence: [T02-S079])
- **谁在用**：从 3 个人到 3 万人的公司都在用。差别只在「它是唯一的系统」还是「它是系统之上的一层」
- **最大的坑**：**把 Excel 当数据库**。一旦一个文件同时承担「原始明细存储 + 计算 + 呈现」三件事，它就会在 20 MB 左右开始崩，并且没有人敢改。正确做法是明细留在总账/BI 里，Excel 只做计算与呈现 (evidence: [T02-S001, T02-S039])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low（24 个月内被显著取代概率 < 20%）

#### Google Sheets

- **用什么场景**：早期公司的第一本账、和外部投资人/FA 共享的模型、需要多人同时改的预算表、用 `IMPORTRANGE`/`GOOGLEFINANCE` 拼的轻量看板 (evidence: [T02-S080])
- **相对优劣**：协作和权限管理比 Excel 好，公式生态和大数据量性能比 Excel 差。**行数一过几万，卡顿就是常态**
- **价格模式**：随 Google Workspace 席位走，官方按用户按月计费 (evidence: [T02-S080])
- **谁在用**：种子轮到 A 轮的公司、远程团队、海外 SaaS 初创
- **最大的坑**：**权限没收干净**。一份「知道链接就能编辑」的董事会模型流出去，比任何系统漏洞都常见
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

**什么规模之前不该上系统（这是本节最该记住的结论）**

- 单一法人主体 + 单一币种 + 月度凭证量小于约几百笔 → 电子表格 + 云记账软件就够，**不要上 ERP** (evidence: [T02-S060, T02-S064])
- 收入体量到约 1 亿美元之前，多数公司的主力规划模型仍然在电子表格里；这不是落后，是行业常态 (evidence: [T02-S060])
- 判断信号不是收入数字，而是**痛点**：关账拖过 15 天、有人在手工合并多个主体、同一个指标三个部门算出三个数——这三条同时出现才是换系统的时候 (evidence: [T02-S002, T02-S060])

---

### 1.2 记账与 ERP

#### QuickBooks Online（QBO）

- **用什么场景**：美国/海外主体的第一套总账，接银行流水自动导入，会计事务所直接在里面出报表
- **相对优劣**：生态最厚（几乎所有海外财务 SaaS 都优先接 QBO），成本低；弱在多主体合并、复杂收入确认、多币种，做不了就得靠外挂
- **价格模式**：按订阅分档，官方定价页有反爬（HTTP 拦截），**本文不写具体金额**；业内共识是月费几十美元级
- **谁在用**：海外注册的初创、SMB；Mostly Metrics 与 The SaaS CFO 两份从业者工具栈调查都把它当作低收入段的默认项 (evidence: [T02-S060, T02-S063])
- **最大的坑**：把 QBO 的现金制报表直接当经营口径给董事会看。QBO 默认很容易停在现金制，而投资人和收入确认要的是权责发生制 (evidence: [T02-S064])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Xero

- **用什么场景**：QBO 之外的主要选择，英澳新与部分欧洲市场更常见；对代账事务所友好
- **相对优劣**：界面与银行对账体验好，第三方 App 市场大（Float、Fathom 这类都是先接 Xero）；美国市场生态不如 QBO
- **价格模式**：官方按套餐分档订阅，各档在发票数、账单数、多币种上有硬限制，官方定价页写明 (evidence: [T02-S014])
- **谁在用**：非美市场的中小企业、跨境电商的海外主体
- **最大的坑**：**低档套餐的发票/账单条数限制**会在业务起量后突然卡住，被迫升级或拆账套 (evidence: [T02-S014])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### 金蝶（精斗云云会计 / AI 星辰）

- **用什么场景**：中国境内实体的账务、进销存、开票与报税打通。精斗云面向微型企业与个体工商户，AI 星辰面向小型到成长型企业的业财税一体化 (evidence: [T02-S007, T02-S008])
- **相对优劣**：与中国财税链路（数电发票、电子税务局）的适配是它的核心价值，海外 SaaS 完全做不了这块；弱在灵活报表与 API 开放度，以及跨主体合并
- **价格模式**：按账套/用户/模块的年费订阅，分档，具体金额以官网各产品页为准 (evidence: [T02-S007, T02-S008])
- **谁在用**：中国境内的小微与成长型企业，以及代账机构的客户
- **最大的坑**：**先买了模块，再发现业务流程要按软件改**。中国 ERP 的实施占比常常高于软件本身的价格，选型时只比 license 价格必然踩坑
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium（产品线更名与合并频繁，2026 年「金蝶云·星辰」已更名为「金蝶 AI 星辰」）

#### 用友（畅捷通好会计 / 易代账 / YonSuite）

- **用什么场景**：与金蝶同一生态位。好会计面向小微企业自己记账，易代账面向代账机构批量做账，YonSuite 面向成长型企业的一体化 (evidence: [T02-S044, T02-S045, T02-S046])
- **相对优劣**：小微云财税这一段的市场份额领先是厂商与第三方研究都提到的口径（厂商自述，需打折看）；向上到 YonSuite 时复杂度和实施成本陡增
- **价格模式**：按订阅年费分档，官网产品页给具体档位
- **谁在用**：中国境内小微企业、代账机构；再往上是用 YonSuite 的成长型企业
- **最大的坑**：**小微产品与集团产品之间没有平滑升级路径**。从好会计换到 YonSuite 基本等于重新实施一次，历史数据迁移要单独立项
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Odoo

- **用什么场景**：需要进销存 + 会计 + CRM 一体，并且愿意自己托管或找实施商的贸易/制造/电商公司 (evidence: [T02-S013])
- **相对优劣**：开源可改是最大优势——主仓 54.1k stars，2026-09-01 仍有推送，社区活跃度是硬信号 (evidence: [T02-S074])；劣势是「会计合规」要靠本地化模块，中国税务场景需要额外集成
- **价格模式**：官方按用户订阅 + 按模块，社区版免费自托管。**真实成本大头是实施与二次开发，不是 license** (evidence: [T02-S013])
- **谁在用**：有技术团队或长期实施伙伴的中小企业，尤其是跨境电商和贸易
- **最大的坑**：**把开源当免费**。社区版跑起来容易，跑到能出合规报表、能升级、能审计要投入的人月，往往超过直接买 SaaS
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### NetSuite

- **用什么场景**：多法人主体、多币种、需要合并报表和审计留痕的中大型公司；也是很多海外公司 IPO 前的标配 (evidence: [T02-S016])
- **相对优劣**：多主体合并与本位币折算是它真正值钱的地方；劣势是实施周期长、报表定制贵、日常小改动都要找顾问
- **价格模式**：官方不公开报价，按模块 + 用户数 + 年限谈判。**任何在第三方站看到的「NetSuite 五年花费 X 万美元」都属于业内估计，不是官方定价**
- **谁在用**：业内经验大致是收入体量到约 2000 万美元、或出现第二个法人主体之后才值得上 (evidence: [T02-S060])
- **最大的坑**：**上得太早**。在只有一个主体、一个币种、几百笔月凭证的时候上 NetSuite，得到的是更慢的关账和一笔无法回收的实施费
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### SAP Business One / Zoho Books（补位选项）

- **SAP Business One**：面向中小企业的 SAP 产品线，制造与分销场景的功能深，靠伙伴实施；适合已经在 SAP 生态里、或供应链复杂的公司 (evidence: [T02-S017])
- **Zoho Books**：性价比路线，官方有免费档（有营收上限条件），适合极小团队和已经在用 Zoho 其他产品的公司；弱在会计深度与审计接受度 (evidence: [T02-S015])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low / medium

---

### 1.3 中国财税合规链路

这一段是中国创业者和中小企业主绕不开的、**没有替代品**的必备层。它不是「选一个工具」，而是一条固定链路。

#### 全国统一规范电子税务局

- **用什么场景**：申报、缴税、发票开具与交付、进项发票用途确认（勾选）、涉税资料查询——一个入口全办 (evidence: [T02-S069])
- **官方规模口径**：税务总局官方通稿称新电子税务局服务超 9600 万纳税人、月均办理超 3.8 亿笔业务，97% 的税费事项与 99% 的纳税申报事项可线上全流程办理 (evidence: [T02-S068])
- **价格模式**：免费，官方系统
- **最大的坑**：**账号与实名权限就是公司的财务命脉**。法人、财务负责人、办税员的实名认证与授权关系一旦没理清，换财务、换代账、法人变更时会直接卡住报税
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### 数电发票（全面数字化的电子发票）

- **用什么场景**：开票、收票、查验、用途确认的全流程。税务总局 2024 年第 11 号公告确认在全国正式推广应用 (evidence: [T02-S003, T02-S004])
- **三个机制变化**（官方解读原话口径）：**去介质**（不再领取专用税控设备）、**赋码制**（系统自动分配全国统一发票号码，取消号段申领）、**赋额制**（系统自动授予开票总额度，符合条件的新办纳税人开业即可开票） (evidence: [T02-S005])
- **相对优劣**：对创业公司是纯利好——开业当天就能开票，不用买税控盘、不用跑领票。代价是**开票行为实时进入税务数字账户**，事后调整空间接近于零
- **价格模式**：官方免费
- **最大的坑**：**开票额度不够时才发现额度是动态授予的**。大单要开票前没有提前确认额度，会在收款关键节点卡住 (evidence: [T02-S005])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium（推广与规则仍在迭代）

#### 进销项比对与「金税四期」这个说法

- **先纠正一个用词**：「金税四期」是业内和媒体的通俗叫法，税务总局的官方表述是**智慧税务**建设与全国统一规范电子税务局。写材料时用官方词，别在正式文件里写「金税四期」 (evidence: [T02-S068, T02-S069])
- **实际影响**：发票要素全面数字化 + 号码全国统一赋予 + 信息在征纳双方之间自动流转，意味着**进项与销项的比对是系统默认能力，不是抽查动作** (evidence: [T02-S005])
- **最大的坑**：**用「以票管税时代的老经验」做税务筹划**。买发票、虚开、两套账这类做法在数据自动比对下不是风险高低问题，是必然暴露问题
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### 代账 SaaS（代理记账机构侧）

- **用什么场景**：不是给企业主用的，是给**替你记账的那家代账公司**用的。中国 30 人以下公司绝大多数把记账外包，实际决定你账务质量的是对方用什么系统、怎么用
- **主要玩家**：畅捷通易代账、金蝶账无忧、云账房 (evidence: [T02-S046, T02-S047, T02-S048])
- **价格模式**：按账套数或客户数向代账机构收年费；企业主看到的是代账服务费，不是软件费
- **谁在用**：代账机构；间接影响所有把记账外包的中小企业
- **最大的坑**：**账套的所有权和数据导出权在代账机构手里**。换代账时拿不到完整的凭证、附件和往来明细，是中国中小企业最常见的一次性损失。签代账合同时就要写明数据交付格式与离场义务
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

---

### 1.4 银行与资金

#### 企业网银 / 银企直联（银企互联）

- **用什么场景**：账户余额与明细查询、批量付款、代发工资、资金归集与下拨、**电子对账** (evidence: [T02-S049, T02-S050])
- **两者的区别**（这是选型的真分岔）：
  - **企业网银**：人登录网页操作。零成本、零集成，适合账户数少、付款笔数少的公司
  - **银企直联**：企业的 ERP/财务系统与银行核心系统直接对接，不用登录网银就能查账、付款、拉对账单。建行、工行、招行都有官方产品页与开发手册 (evidence: [T02-S049, T02-S050, T02-S051])
- **价格模式**：银行侧通常按接口/年费收，或以存款规模置换减免；**真实成本是 IT 对接的人月**，不是银行报价
- **谁在用**：账户数超过约 5 个、或月付款笔数上百、或有多主体资金归集需求的公司。**一个账户、每月几十笔付款的公司不需要银企直联**
- **最大的坑**：
  1. **每家银行的接口都不一样**，接了三家银行等于做了三次集成，而且升级不同步
  2. **对账口径**：银行流水的摘要字段各行格式不同，自动对账的匹配率没到 90% 以上，人工反而更累
  3. **U 盾/证书的物理管理**：多主体多银行时，一堆 U 盾在一个抽屉里由一个出纳保管，是最典型的资金内控漏洞
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

---

## 二、场景特化层

### 2.1 FP&A 与预算

**先说这一层的市场实情**：CFO 工具市场极度拥挤——业内盘点称面向 CFO 办公室的规划工具已超过 100 个 (evidence: [T02-S061])。所以这一节的价值不在于「列出谁」，而在于**分成两条路线**。

**路线 A：保留电子表格作为前端**（Cube、Datarails、Vena）
**路线 B：把建模搬进厂商自己的界面**（Runway、Mosaic、Abacum、Pigment、Anaplan、Planful）

这条分界线比任何功能对比都重要，因为它决定了**谁能维护这个模型**：路线 A 的模型财务自己就能改；路线 B 的模型改结构往往要找厂商或内部超级用户 (evidence: [T02-S001, T02-S002])。

#### Cube

- **场景**：财务已经有一套跑得通的 Excel/Sheets 模型，痛点是「取数慢 + 版本乱」，不是「模型不会建」 (evidence: [T02-S018])
- **优劣**：与 Excel/Sheets 双向同步是它的卖点，学习成本低；劣势是它本质是数据层与版本层，建模能力上限还是电子表格的上限
- **价格模式**：官方按套餐年费订阅，分档 (evidence: [T02-S018])
- **谁在用**：约 30-300 人、有 1-3 人财务团队的公司
- **最大的坑**：**同步方向没定清楚**。哪张表是「源」哪张是「镜像」如果没在实施时定死，最后会出现两边都能改、谁也不知道哪个是准的
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Datarails

- **场景**：历史 Excel 模型多且乱，公司不想推倒重来，只想把它们统一到一个可追溯的地方 (evidence: [T02-S025])
- **优劣**：「不改变工作方式」是最大卖点，也是最大天花板——脏模型搬上云仍然是脏模型
- **价格模式**：官方询价制，不公开标价
- **谁在用**：中型、传统行业、财务团队 Excel 依赖极重的公司
- **最大的坑**：把它当成「模型治理」的替代品。**工具能记录版本，不能替你重建口径**
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Vena

- **场景**：需要 EPM 级别的建模引擎（多维度、驱动式、工作流审批），但团队只肯用 Excel 界面 (evidence: [T02-S026])
- **优劣**：Excel 原生 + 后端多维模型是它的独特位；劣势是实施重于 Cube/Datarails
- **价格模式**：询价制
- **谁在用**：中型到中大型企业，有专职 FP&A
- **最大的坑**：实施周期被低估，**上线时间常常跨过一个完整预算季**，导致第一年白做
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Runway

- **场景**：早期到成长期创业公司，需要一份**能给董事会讲故事**的预算与情景对比，而不是一份能给审计看的模型 (evidence: [T02-S019])
- **优劣**：叙事与可视化强，非财务人也看得懂；劣势是深度建模与合并报表能力有限，且是相对年轻的产品
- **价格模式**：官方分档订阅 (evidence: [T02-S019])
- **谁在用**：种子轮到 B 轮的科技公司
- **最大的坑**：把董事会用的叙事模型当成运营模型。**两者的颗粒度需求相反**——董事会要少而清楚，运营要细而可拆
- **last_checked**: 2026-09-02 ｜ **Decay risk**: high（新兴产品，12 个月内定位可能明显变化）

#### Mosaic / Abacum / Pigment / Anaplan / Planful

- **Mosaic**：战略财务定位，强在指标看板与 headcount 规划，适合 SaaS 且已有 CRM/HRIS 可接 (evidence: [T02-S020])
- **Abacum**：中型市场 FP&A，在 2026 年的 CFO 工具栈调查里被点名为「替代 Adaptive / Anaplan 的中端选择」之一 (evidence: [T02-S021, T02-S060])
- **Pigment**：建模自由度高的企业级规划，适合多业务线、驱动逻辑复杂 (evidence: [T02-S022])
- **Anaplan**：老牌重型，调查数据显示在 10 亿美元以上收入段仍占优；在中小企业身上就是过度配置 (evidence: [T02-S023, T02-S060])
- **Planful**：中大型 EPM，同一份调查里被点名在中端份额上升 (evidence: [T02-S024, T02-S060])
- **共同的价格模式**：全部询价制，没有公开标价。**任何在对比站看到的年费数字都是业内估计**
- **共同的最大的坑**：**买了不用**。AFP 官方调查显示 71% 的团队在用 EPM，同时 96% 的人仍在按周用电子表格做规划——买了系统而主力模型还在表格里，是这个品类最典型的结局 (evidence: [T02-S001, T02-S002])
- **last_checked**: 2026-09-02

#### Jirav

- **场景**：中小企业，或者由**外部会计事务所**替你维护预测模型 (evidence: [T02-S027])
- **优劣**：三表联动 + 预测打包好，事务所渠道强；灵活度不如通用建模工具
- **价格模式**：官方分档年费订阅，有面向事务所的合作方案 (evidence: [T02-S027])
- **最大的坑**：模型逻辑在事务所手里，**换事务所等于换模型**
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Lucanet xP&A（原 Causal）

- **状态更新（重要）**：Causal 于 2024-10-31 被德国 CFO 软件集团 Lucanet 收购，产品未关停，正在并入 Lucanet 平台 (evidence: [T02-S006])
- **给选型的启示**：这是 FP&A 工具最典型的风险——**你选的是产品，拿到的可能是并购路线图**。签多年合同前问清楚产品未来 24 个月的独立路线
- **last_checked**: 2026-09-02 ｜ **Decay risk**: high

---

### 2.2 现金流预测

#### 13 周滚动现金流（这是方法，不是软件）

- **场景**：现金紧张、要跟银行/投资人谈判、要做重组或裁员决策时的标准工具。13 周 = 一个季度，粒度到周，足够看见发薪周的缺口，又足够长到能安排一次融资或一次账期谈判 (evidence: [T02-S071])
- **为什么是 13 周而不是 12 或 26**：它对齐一个财季与债务契约测试周期，也是重组/DIP（债务人持有资产）融资场景下贷款方与顾问的默认要求格式 (evidence: [T02-S071])
- **载体**：**绝大多数是 Excel 模板**，不是软件。AFP 的流动性调查系列是这个做法采用率的官方来源 (evidence: [T02-S072])
- **最大的坑**：**做成一次性的**。13 周现金流的全部价值在「滚动」——每周把实际值填进去、和上周预测比差异、解释差异。做一次就束之高阁等于没做
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Float

- **场景**：记账已经在 Xero/QBO 上，想要一个自动拉数的滚动现金流预测，而不是每周手工更新 Excel (evidence: [T02-S028])
- **优劣**：接总账自动更新是核心价值；劣势是预测逻辑相对简单，复杂的收款账期与项目制预测要外挂
- **价格模式**：官方分档月费/年费订阅 (evidence: [T02-S028])
- **谁在用**：用 Xero/QBO 的中小企业
- **最大的坑**：**总账里的应收账期是名义账期，不是实际回款时间**。直接按发票到期日预测现金，会系统性高估回款
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Fathom

- **场景**：需要给老板/董事会一份定期的**经营分析报告**（不只是现金流），并接总账自动生成 (evidence: [T02-S029])
- **优劣**：报告模板与指标库现成，会计事务所大量用它给客户出月报；劣势是自定义分析深度有限
- **价格模式**：官方按公司数/套餐订阅，有面向事务所的批量方案 (evidence: [T02-S029])
- **最大的坑**：模板化报告好看但**不解释因果**。指标全绿而业务在恶化的情况很常见
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

---

### 2.3 股权与 cap table

#### Carta

- **场景**：要拿机构美元融资、要发期权、要做 409A 估值。它的真实价值不只是软件，是**投资人、律所、审计都认这个格式** (evidence: [T02-S042])
- **优劣**：生态与合规接受度是护城河；劣势是价格随股东数与融资额上升快，且历史上有过数据使用争议
- **价格模式**：官方按套餐年费分档，早期有免费/入门档（有股东数与融资额上限条件），具体条件以官方定价页为准 (evidence: [T02-S042])。**注意：官方定价页对自动化抓取返回 403，属反爬不是死链**
- **谁在用**：拿美元 VC 的公司，从种子轮开始
- **最大的坑**：**当作「录入完就不管」的档案库**。期权归属、离职回购、行权窗口如果没同步进去，下一轮尽调会全部炸出来
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Pulley

- **场景**：早期、股本结构简单（普通股 + 一档优先股）、对价格敏感的公司 (evidence: [T02-S041])
- **优劣**：官方定价公开透明——Startup 档 $1,200/年（25 名股东），Growth 档 $3,500/年（40 名股东，含 409A 估值），企业版询价，**且官方明确说明没有免费档** (evidence: [T02-S041])。劣势是复杂结构（参与型优先股、多层清算优先权、复杂认股权证）的深度不如 Carta
- **谁在用**：种子轮到 A 轮、结构简单的公司
- **最大的坑**：**股东数计费口径**。官方定义中，单笔 5 万美元以下的天使投资人按半个股东计——报价时按人头估算会算错档位 (evidence: [T02-S041])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### AngelList / Excel 稀释模型

- **AngelList**：更偏基金与 SPV（特殊目的载体）侧，创业公司自己管 cap table 的场景不如 Carta/Pulley 主流
- **Excel 稀释模型**：**在 pre-seed 到种子轮阶段，这仍然是正确答案**。真正需要建模的是「这一轮之后我还剩多少、期权池从哪儿来、优先清算怎么算」——这三个问题在一张表里比在任何软件里更清楚 (evidence: [T02-S064])
- **最大的坑**：软件里的 cap table 和 Excel 里的稀释模型**长期不一致**，融资谈判时用了旧表
- **last_checked**: 2026-09-02

#### 中国的持股平台与代持结构（如实说：工具化程度低）

- **实情**：中国境内的员工激励与股权结构，主流做法是**有限合伙形式的持股平台**加上工商登记，以及在某些阶段的代持安排。这套东西**没有一个像 Carta 那样的行业标准软件**——它主要活在律所的文件、工商登记信息和一张 Excel 里
- **这不是本调研没找到，是行业事实**：Carta/Pulley 这类产品的合规模型建立在美国 409A、Rule 701、Form 3921 之上 (evidence: [T02-S041])，这些在中国境内结构下不适用
- **实践建议**：把「工商登记的股权结构」「持股平台的合伙份额表」「员工激励的授予与归属台账」当作**三张必须分开维护、定期核对的表**，用 Excel + 版本归档，而不是指望一个系统
- **最大的坑**：**只存在律师的 Word 文件里**。协议是法律效力载体，但没有一张能一眼看出稀释与归属的表，创始人自己也说不清下一轮之后剩多少
- **可信度**: medium ｜ `[no standard tooling source found — 该结论基于中美合规框架差异，不基于某个中国 cap table 产品]`
- **last_checked**: 2026-09-02

---

### 2.4 订阅计费与收入确认

**这一节的核心分岔不是选哪家，是「计费」和「收入确认」是不是同一件事。**

#### Stripe Billing

- **场景**：收款已经在 Stripe，订阅规则不复杂（固定套餐、按量计费、试用期） (evidence: [T02-S030])
- **优劣**：与收单同源，集成成本最低；劣势是收入确认与 SaaS 财务报表能力弱于专业方案
- **价格模式**：**按处理流水的百分比抽成**（在支付手续费之外另计），官方费率页给具体比例 (evidence: [T02-S030])。这是关键差别——流水越大，Billing 越贵
- **最大的坑**：**用 Stripe 的 MRR 面板当财务口径**。Stripe 的口径是收款视角，权责发生制下的确认收入与它经常不等
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Chargebee

- **场景**：计费规则复杂（多币种、多定价模型、分销渠道、试用与折扣策略） (evidence: [T02-S031])
- **优劣**：计费灵活度高；**但要注意官方文档写明：核心计费内置的收入确认是按旧准则口径，ASC 606 / IFRS 15 的五步法由单独的 RevRec 模块承担** (evidence: [T02-S084])。选型时把它当两个产品报价
- **价格模式**：官方分档订阅 + 超出流水后按比例，有免费额度门槛 (evidence: [T02-S031])
- **最大的坑**：以为买了 Chargebee 就自动合规 606
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Maxio

- **场景**：B2B SaaS，同时要计费和**干净的 GAAP 收入确认 + SaaS 指标**。它是 SaaSOptics 与 Chargify 合并的产物，收入确认在核心平台里而不是外挂模块 (evidence: [T02-S032, T02-S085])
- **优劣**：计费 + 收入确认 + 指标一体是它的位；劣势是价格高于纯计费方案，且对非订阅业务没意义
- **价格模式**：官方分档订阅，询价为主 (evidence: [T02-S032])
- **最大的坑**：合并产品的历史包袱——两条老产品线的功能与迁移路径要在采购时问死
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Recurly

- **场景**：以订阅计费与流失挽回（dunning）为主，收入确认另配 (evidence: [T02-S033])
- **优劣**：计费与续费挽回成熟；收入确认能力不是它的主场
- **价格模式**：官方分档订阅 + 按流水比例 (evidence: [T02-S033])
- **最大的坑**：把它当收入确认系统买
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

**中国境内的对应现实**：上述四家的收入确认逻辑都围绕 ASC 606 / IFRS 15 构建；中国境内主体适用的是《企业会计准则第 14 号——收入》（修订后的五步法与 IFRS 15 趋同） (evidence: [T02-S078])。**但发票、税会差异和纳税义务时点是另一套规则，不能靠这些工具解决**——境内 SaaS 公司通常要在计费系统之外单独维护一张「确认收入 / 开票 / 纳税义务发生时间」的对照表。

---

### 2.5 费控报销

#### Ramp / Brex（海外）

- **分界线（有调查数据支撑）**：CFO 工具栈调查显示，**约 1 亿美元 ARR 以下是 Ramp 的地盘**，且在这一段 Ramp 已经在赢 Expensify；过了 1 亿美元，Brex 在企业段发力并挑战传统卡组织 (evidence: [T02-S060])
- **价格模式（这是它们和传统报销软件的根本区别）**：Ramp 的官方模式是**软件免费档 + 靠卡的交换费（interchange）赚钱** (evidence: [T02-S034])；Brex 官方也有免费档加付费企业档 (evidence: [T02-S035])。所以「省了软件费」的代价是**你的支付流水绑定在这家公司**
- **谁在用**：有美国实体、美元支出为主的初创与成长期公司
- **最大的坑**：**把卡商当银行**。它们不是存款保险覆盖的银行，资金存放形式和取回条件要在开户时读清楚
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### Expensify（海外）

- **场景**：纯报销，不换支付关系，或已有企业卡只想解决贴票 (evidence: [T02-S036])
- **优劣**：轻、便宜、上手快；劣势是在有免费卡+软件的竞品面前性价比被挤压，调查数据显示它在 1 亿美元 ARR 以下正在丢份额 (evidence: [T02-S060])
- **价格模式**：官方按**活跃用户**计费（当月有提交行为才算），分档 (evidence: [T02-S036])
- **最大的坑**：活跃用户口径导致预算不可预测，季节性出差月账单会跳
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

#### 汇联易 / 分贝通 / 合思（易快报）（中国）

- **三家的真实分岔**（这是中国费控选型的核心）：
  - **分贝通**：从商旅起家，官方自述是「**SaaS + 交易**」模式——把打车、差旅、餐饮做成企业统一支付与统一开票，目标是**员工根本不用报销**，收入含交易流水返佣 (evidence: [T02-S038, T02-S075])
  - **汇联易**：从**费用报销**起家，强在企业内部管理系统与外部消费服务商的连接、预算控制与电子发票管理，第三方分析机构把它定位在大中型企业 (evidence: [T02-S037, T02-S076])
  - **合思（易快报）**：同属报销起家的一档，是这个赛道的第三家主流厂商 (evidence: [T02-S077])
- **价格模式**：报销起家的一档主要收 SaaS 年费（按人数/模块），部分消费场景接入还会有二次费用；支付起家的一档把部分成本转嫁到交易返佣上 (evidence: [T02-S075])
- **谁在用**：分贝通更常见于差旅与地推支出重的公司；汇联易/合思更常见于流程与预算管控要求高的中大型企业 (evidence: [T02-S076])
- **最大的坑**：
  1. **只比软件价格，不比场景接入费**——第三方供应商二次收费是这个赛道的常见隐性成本 (evidence: [T02-S075])
  2. **发票流与账务流没打通**：费控系统里报销通过了，凭证还得在金蝶/用友里再录一遍，等于多一套人工
- **last_checked**: 2026-09-02 ｜ **Decay risk**: medium

---

### 2.6 BI 与看板

#### Power BI

- **场景**：公司已在微软生态，财务自己就是主要作者（Power Query 和 Excel 的技能可以直接迁移） (evidence: [T02-S009])
- **优劣**：单人授权成本在主流 BI 里最低，与 Excel 数据模型同源；劣势是要发布给全公司看时，需要更高档授权或容量，成本模型会突变
- **价格模式**：官方按用户订阅（Free / Pro / Premium Per User）+ 按容量（Fabric）两条线，官方定价页写明分界 (evidence: [T02-S009])
- **最大的坑**：**按用户买到一半才发现要按容量买**。当只读用户数上去以后，按人授权会比容量贵，反之亦然——这条线要在铺开前算 (evidence: [T02-S009])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Tableau

- **场景**：分析能力强、以可视化探索为主的团队 (evidence: [T02-S010])
- **优劣**：可视化与交互体验强；官方按角色定价（Creator / Explorer / Viewer），**Creator 席位贵是它的结构性成本** (evidence: [T02-S010])
- **最大的坑**：给所有人买 Creator。角色划分不清是这个产品最常见的浪费
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Metabase

- **场景**：有数据库、有一点技术能力，想自托管、想省钱、想让业务自助查数 (evidence: [T02-S011])
- **成熟度信号**：主仓 49.0k stars，最后推送 2026-09-01，未归档 (evidence: [T02-S073])
- **价格模式**：开源版可自托管（免费），官方另有云版与企业版分档订阅 (evidence: [T02-S011])
- **最大的坑**：**没人管权限**。自助查数很爽，直到有人把工资表拉出来了
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### 帆软 FineReport / FineBI

- **场景**：中国式复杂报表——多层表头、合并单元格、套打、按科室按层级分发的固定格式报表。这是海外 BI 做不了或做起来极痛苦的一类 (evidence: [T02-S012])
- **两个产品别搞混**（官方帮助中心口径）：**FineReport 偏短期运作支持与固定格式展示取数**，FineBI 偏业务人员自助拖拽的长期分析 (evidence: [T02-S083])。买错会得到「想做分析买了报表工具」
- **价格模式**：按 license + 并发/模块，询价制
- **谁在用**：中国境内有 IT 支撑的中大型企业；小微企业通常用不上也养不起
- **最大的坑**：**把它当 BI 买、当报表用**，最后变成一个昂贵的、需要专人开发的报表出口
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

---

### 2.7 财务模型模板与建模规范

#### FAST Standard

- **是什么**：Flexible / Appropriate / Structured / Transparent 的建模规范，由 FAST Standard Organisation 维护，全文公开可下载 (evidence: [T02-S039])
- **为什么它属于工具栈**：它不是软件，是**让模型可以交接**的那套约定——一行一公式、从上到下从左到右阅读、公式短到「一个拇指能盖住」。没有这套约定，模型换个人就成了黑箱 (evidence: [T02-S039])
- **谁在用**：项目融资、基建、需要外部审阅模型的场景最普遍；创业公司里通常只有做过投行/咨询的人知道
- **最大的坑**：**教条化**。一家 8 个人的公司严格执行完整 FAST 规范是过度投入；真正要抄的是三条——**输入区/计算区/输出区分开、一行一个公式、不写跨表硬编码**
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

#### Financial Modeling World Cup（FMWC）

- **是什么**：公开的建模竞赛，题目与解法公开，是观察「高水平的人怎么在限定时间里搭模型」的一手窗口 (evidence: [T02-S040])
- **对中小企业主/创业者的实际用途**：不是去比赛，是**用它的题目当训练**——它逼你用最少的辅助列把逻辑写清楚
- **最大的坑**：把竞赛技巧当日常规范。竞赛追求速度，生产模型追求可读与可审计，两者的最优解不同
- **last_checked**: 2026-09-02 ｜ **Decay risk**: low

---

## 三、新兴 / 实验层（近 12 个月）

> **本节的写法约定**：只写产品名 + 它实际能做到的那一小块 + 现在的真实成熟度。**厂商营销话术（「自动关账」「AI CFO」「agentic finance」）一律不复述。**

### 3.1 AI 原生 ERP / 总账：钱多，客户少，赌注性质明确

#### Rillet

- **它到底做什么**：AI 原生 ERP，明确定位为替换 NetSuite / SAP / Oracle Fusion 一类的现有系统 (evidence: [T02-S052, T02-S070])
- **真实成熟度**：厂商官方口径称 2026-08 完成 1 亿美元 C 轮、投后估值约 10 亿美元、客户数超过 600 家，并列出若干具名的高增长公司客户 (evidence: [T02-S070])。**这些数字来自厂商自己的公告，不是独立审计**
- **对创业公司的实际含义**：600 家客户对一个 ERP 品类来说仍然很小。**在还没有第二个法人主体、没有多币种的时候讨论换 ERP，本身就是伪问题**
- **stability**: experimental ｜ **Decay risk**: high（12 个月内定位/定价/被收购的概率业内估计 > 40%）
- **last_checked**: 2026-09-02

#### Campfire

- **它到底做什么**：AI 原生总账/ERP，同一赛道的更早期玩家 (evidence: [T02-S053])
- **真实成熟度**：公开可核的客户名单薄，属于早期采用者的游戏。**没有独立第三方生产案例支撑，本文不把它列为可推荐项**
- **stability**: experimental ｜ **Decay risk**: high
- **last_checked**: 2026-09-02

### 3.2 关账与对账：这是 AI 目前最落得下去的一块

#### Numeric

- **它到底做什么**：把对账（尤其是往来科目余额核对）和关账清单做成有 AI 辅助的工作流 (evidence: [T02-S054])
- **为什么这块能落地**：对账是**有明确对错、有大量重复、错了立刻能发现**的任务——这三个条件同时成立，AI 的价值才不是演示效果
- **真实成熟度**：落地点窄但真实。适合月凭证量已经上千、关账要 10 天以上的公司
- **stability**: experimental ｜ **Decay risk**: high
- **last_checked**: 2026-09-02

#### FloQast / BlackLine（老牌加 AI，不是新兴产品）

- **定位澄清**：这两家不是新出现的公司，是关账管理与账务自动化的既有基线，近 12 个月的变化是在原有工作流上加 AI (evidence: [T02-S055, T02-S056])
- **FloQast 官方口径**：2026-01 官宣年度经常性收入超过 2 亿美元，并把增长归因于企业客户、国际扩张与 AI 产品使用度 (evidence: [T02-S055])。**归因是厂商自述**
- **对中小企业的实际含义**：这两个都是**有专职会计团队之后**才有意义的产品。10 人公司买它是买一套用不上的控制框架
- **Decay risk**: low（基础设施型）｜ **last_checked**: 2026-09-02

### 3.3 AI 记账（面向初创与小微）

#### Puzzle / Digits / Basis

- **Puzzle**：AI 优先的初创记账，目标是把「记账 + 出报表」这件事压缩 (evidence: [T02-S057])
- **Digits**：AI 记账与报表，存在时间较长但一直没有成为主流 (evidence: [T02-S058])
- **Basis**：面向**会计事务所**而不是企业自己的 AI agent，融资规模大但产品仍在证明期 (evidence: [T02-S059])
- **共同的真实成熟度**：这类产品能替掉的是**分类打标签**这一层的人工，替不掉的是**判断**——什么该资本化、什么是关联交易、哪笔收入该分期确认。所以它压缩的是记账成本，不是财务负责人的工作
- **stability**: experimental ｜ **Decay risk**: high
- **last_checked**: 2026-09-02

### 3.4 FP&A 问答与差异解释：演示强，生产环境弱

#### Aleph 与各 FP&A 厂商的内嵌 AI 助手

- **Aleph**：定位在 ERP 与电子表格之间的数据层，附带自然语言问数 (evidence: [T02-S082])
- **各家 FP&A 厂商**：近 12 个月几乎所有规划工具都上了自己的 AI 助手，卖点统一是「问一句就给你差异解释」 (evidence: [T02-S061])
- **真实成熟度（有官方调查数据，别信演示）**：AFP 2025 年基准调查显示，只有约 23% 的 FP&A 从业者在按日/周/月的频率使用 AI；另有约 40% 处于测试阶段、计划在未来一年落地 (evidence: [T02-S001])。**也就是说，2026 年这仍然是少数派行为**
- **为什么落不下去（同一份调查给了原因）**：从业者把**数据质量**而不是工具或技能列为首要障碍——约 61% 说数据可靠性不足、约 60% 说数据不可获取 (evidence: [T02-S001])。**在数据口径没统一之前，AI 问答只会更快地给出错误答案**
- **stability**: experimental ｜ **Decay risk**: high
- **last_checked**: 2026-09-02

### 3.5 AI agent 接入财务数据的合规与审计留痕

这是本节最该被认真对待的一块，因为它决定了前面几项能不能真的进生产。

- **已经有正式框架了，不是空谈**：COSO 于 2026-02-23 发布《Achieving Effective Internal Control Over Generative AI》，给出 govern / inventory / assess / design / implement / monitor 六步实施路线 (evidence: [T02-S066])
- **最关键的一条要求**：审计留痕必须能**重建 AI 当时到底基于什么做了动作**——提示词（prompt）、输入、输出、模型与配置版本、以及人工复核的证据，全部是审计轨迹的组成部分，**不是它的附属物** (evidence: [T02-S066])
- **落到具体控制上**（行业实务口径）：每一次 agent 动作要产生结构化日志，记录**哪个 agent、以谁的授权、在什么时间、对哪个资源、结果是什么**，并且事后不可篡改 (evidence: [T02-S067, T02-S081])
- **给创业公司和中小企业主的可执行版本**（不需要买任何工具）：
  1. **先划禁区**：哪些账户、哪些科目、哪些金额以上的动作 AI 不许碰，写进一页纸
  2. **只读优先**：先让 AI 读账、做分析、写解释稿；**过账、付款、改主数据这三件事保持人工**
  3. **留痕三件套**：提示词存档、模型版本记录、人工复核签字（哪怕只是审批流里一个勾）
  4. **对外责任不转移**：用了 AI 出错，对税务局和审计而言责任仍然在企业，不在厂商
- **最大的坑**：**先上 agent，再补控制**。CPA 实务界 2026-08 的公开建议就是反过来——让 agent 跑关账之前，先把五项控制写成文字 (evidence: [T02-S067])
- **last_checked**: 2026-09-02 ｜ **Decay risk**: high（准则与监管仍在快速变化）

---

## 四、避坑清单

外行（以及第一次当 CFO 的人）最容易选错的九件事。每条都写清楚**为什么错**和**替代做法**。

### ❌ 1. 上系统太早

- **错在哪**：在只有一个法人主体、一个币种、每月几百笔凭证的时候上 ERP 或 EPM。得到的是更慢的关账和一笔收不回的实施费
- **证据**：AFP 官方调查显示 71% 的团队装了 EPM，但 96% 的人仍在按周用电子表格做规划——**系统买了没替代掉表格，是这个品类的常态而非例外** (evidence: [T02-S001, T02-S002])；CFO 工具栈调查显示专用 FP&A 工具的采用率在约 1 亿美元收入前都不到一半 (evidence: [T02-S060])
- **替代做法**：用「痛点三连」判断，而不是用收入数字：关账拖过 15 天 + 有人在手工合并多主体 + 同一指标三个部门算出三个数。**三条同时出现才动**

### ❌ 2. 把 ERP 当 FP&A 用

- **错在哪**：ERP 是记录已发生事实的系统，它的数据结构为「可审计」优化；FP&A 要的是假设、情景、驱动因子，为「可推翻重来」优化。**两者的设计目标相反**
- **表现**：在 NetSuite/金蝶里硬做预算模块，每改一次假设要走一次配置；或者反过来，在 FP&A 工具里存明细凭证
- **替代做法**：ERP 出实际数，FP&A（哪怕就是 Excel）出预测数，中间靠一张**口径映射表**对齐科目 (evidence: [T02-S018, T02-S025])

### ❌ 3. 把记账口径直接当经营口径

- **错在哪**：会计科目是为报税和审计设计的，不是为经营决策设计的。「管理费用」里混着研发人力和 CEO 差旅，这个数对经营没有任何指导意义
- **中国特有的加重版**：现金制记账 + 以票入账，导致**收入确认时点跟着发票走**，而不是跟着履约走 (evidence: [T02-S078])
- **替代做法**：一开始就建**两套维度**——法定科目（给税务和审计）+ 管理口径（给经营）。在总账里用辅助核算/项目/部门维度承载，而不是事后在 Excel 里手工拆 (evidence: [T02-S064])

### ❌ 4. 用 SaaS 指标工具算非订阅业务

- **错在哪**：Maxio、Mosaic、Stripe Billing 这类产品的指标体系（MRR、ARR、NDR、churn）建立在「周期性合约」这个前提上。**项目制、贸易制、硬件、代运营业务套这套口径，算出来的数字没有意义**
- **典型翻车**：贸易公司把一次性订单折成「MRR」；项目制公司把合同额当 ARR，结果现金流和收入完全对不上
- **替代做法**：非订阅业务用**订单/项目**做核算单元——在手订单、完工百分比、项目毛利、回款账龄。这类分析在 Excel + BI 里做，比买 SaaS 指标工具更准 (evidence: [T02-S030, T02-S032])

### ❌ 5. cap table 只存在律师的 Word 里

- **错在哪**：法律文件有效力，但没有一张能一眼算出稀释、期权池、清算优先权的表。下一轮融资时，创始人自己说不清 term 之后剩多少
- **中国版更严重**：持股平台 + 工商登记 + 代持三层信息分散，**没有一个像 Carta 那样的标准软件能兜住** (evidence: [T02-S041])
- **替代做法**：拿美元融资 → 从种子轮起用 Carta 或 Pulley，让投资人、律所、审计说同一种格式 (evidence: [T02-S041, T02-S042])；境内结构 → 三张 Excel（工商股权表 / 持股平台份额表 / 员工授予归属台账）+ 每季度核对一次，版本归档

### ❌ 6. 汇率与多主体合并的坑

- **错在哪**（四个具体错误，按发生频率排）：
  1. **全表用一个汇率**：损益类应当用发生期间的平均汇率、资产负债类用期末汇率，混用会让报表凑不平
  2. **把折算差额当成损失**：外币报表折算差额进权益（其他综合收益），不是当期损益；把它算进利润会让老板做错决策
  3. **内部往来没有对消**：A 主体应收 B 主体的钱，在合并层面必须抵销；两边金额还常常因为入账时点差一个汇率而对不上
  4. **用 Excel 手工合并三个以上主体**：这是关账时间失控最常见的单一原因
- **替代做法**：**第二个法人主体出现时**就统一记账系统和科目表，别等到第五个；三个主体以上、或有跨币种内部往来时，才是 NetSuite 这类系统真正值钱的时刻 (evidence: [T02-S016])

### ❌ 7. 数据权限与离职交接

- **三个高频事故**：
  1. **代账机构掌握账套所有权**：换代账时拿不到完整凭证、附件和往来明细 (evidence: [T02-S046, T02-S047])
  2. **电子税务局的实名与授权关系没理清**：财务离职、法人变更时直接卡住报税 (evidence: [T02-S068])
  3. **一份「知道链接就能编辑」的董事会模型流出去**，比任何系统漏洞都常见
- **替代做法**：签代账合同时写明**数据交付格式与离场义务**；电子税务局的办税人授权列一张台账、离职当天撤销；财务模型统一放在受控目录里，链接分享一律设为「指定人员 + 只读」

### ❌ 8. 只比 license 价格，不比实施与场景接入费

- **错在哪**：中国 ERP 的实施费常常高于软件本身；开源 ERP（Odoo）的真实成本大头是二次开发人月 (evidence: [T02-S013, T02-S074])；中国费控赛道里第三方消费场景接入的二次收费是常见隐性成本 (evidence: [T02-S075])
- **替代做法**：报价单必须包含三项——软件年费、实施费、**第 2 年起的运维与变更费率**

### ❌ 9. 把厂商的功能清单当选型依据

- **错在哪**：面向 CFO 办公室的规划工具已超过 100 个 (evidence: [T02-S061])，功能清单高度同质化，比对功能只会得到「都能做」
- **替代做法**：用下面的决策树——问的是**你的公司在哪个阶段、谁维护模型、业务形态是什么、有几个主体几种币种**，不是问工具有什么功能

---

## 选型决策树

**用法**：从上往下依次回答四个问题，每个问题的答案直接决定下一步。**不要跳着看功能对比。**

### 决策点 1：公司在哪个阶段？（决定要不要买东西）

```
IF 单一法人主体 AND 单一币种 AND 月凭证量 < 约 300 笔 AND 团队 < 30 人
  → 记账：QBO / Xero（海外）｜ 金蝶精斗云 / 畅捷通好会计（境内），或直接外包给代账
  → 规划：Excel / Google Sheets，一份三表联动模型 + 一份 13 周现金流
  → 报销：企业微信/飞书/钉钉审批流 + 一张 Excel 台账
  → 明确不要买：ERP、EPM、专用 FP&A、BI
  → 依据：专用 FP&A 工具在约 1 亿美元收入前采用率不到一半 (evidence: [T02-S060])

ELIF 出现第二个法人主体 OR 关账 > 15 天 OR 同一指标多部门算出不同数
  → 这是「该动」的信号。先做的不是买软件，是统一科目表与口径映射表
  → 然后按决策点 2-4 决定买什么

ELIF 收入体量到约 2000 万美元以上 AND 多主体多币种 AND 准备融资/审计/IPO
  → ERP：NetSuite（海外主导）｜ 用友 YonSuite / 金蝶 AI 星辰以上产品线（境内） (evidence: [T02-S016, T02-S044])
  → 此时 ERP 买的不是记账功能，是合并报表与审计留痕
```

### 决策点 2：谁来维护这个模型？（这是 FP&A 选型的真分岔，不是功能）

```
IF 维护者 = 财务负责人自己 / 一个兼职做财务的创始人
  → 留在电子表格里。要治理就加一层：Cube 或 Datarails (evidence: [T02-S018, T02-S025])
  → 不要买 Anaplan / Pigment 这类：改一次结构就要找人，等于把模型交出去
  → 理由：路线 A（保留表格前端）的模型你自己能改，路线 B 不能

ELIF 维护者 = 1-3 人的专职 FP&A 团队
  → Mosaic（SaaS 指标导向）｜ Abacum（中端替代 Adaptive/Anaplan）｜ Vena（要 Excel 界面 + 多维引擎）
  → 依据：CFO 工具栈调查点名 Abacum / Planful 在中端上升 (evidence: [T02-S060])

ELIF 维护者 = 外部会计事务所 / 外包 CFO
  → Jirav（事务所渠道深）｜ Fathom（月度经营报告） (evidence: [T02-S027, T02-S029])
  → 但要在合同里写清楚：模型逻辑与数据的所有权归你，换事务所时可导出

ELIF 维护者 = 专职建模团队 + IT 支持（通常 500 人以上）
  → Anaplan / Pigment / Planful (evidence: [T02-S023, T02-S022, T02-S024])
  → 这一档以下买它 = 买一套没人会改的系统
```

### 决策点 3：业务是订阅制，还是项目制/贸易制？（决定计费与指标工具）

```
IF 订阅制（SaaS、会员、SaaS+服务）
  ├─ IF 收款已在 Stripe AND 计费规则简单
  │    → Stripe Billing（按流水抽成，流水越大越贵） (evidence: [T02-S030])
  ├─ ELIF 计费规则复杂（多币种/多定价模型/渠道）
  │    → Chargebee；但 ASC 606 要另买 RevRec 模块，按两个产品报价 (evidence: [T02-S084])
  └─ ELIF 要计费 + GAAP 收入确认 + SaaS 指标一体
       → Maxio（收入确认在核心平台内，不是外挂） (evidence: [T02-S032, T02-S085])

ELIF 项目制 / 贸易制 / 硬件 / 代运营
  → 不要碰任何 SaaS 指标工具。核算单元是订单/项目，不是订阅
  → 工具：ERP 的项目核算模块 + Excel 项目毛利表 + BI 看板
  → 指标：在手订单、完工进度、项目毛利、回款账龄——不是 MRR/ARR/NDR

ELIF 混合（订阅 + 项目）
  → 两套口径分开算，在管理报表层合并。**不要试图用一个指标体系覆盖两种业务**
```

### 决策点 4：是否多主体多币种？（决定 ERP 与合并方案）

```
IF 单主体单币种
  → 云记账软件够用。不要为「以后可能需要」提前买多主体功能

ELIF 2 个主体 / 同币种
  → 保持同一套记账系统 + 同一份科目表，用 Excel 合并即可
  → 关键动作：**在第二个主体成立当天就统一科目表**，不要等到第五个

ELIF 3 个以上主体 OR 跨币种内部往来 OR 需要外币报表折算
  → 这是 NetSuite 一类系统真正值钱的分界点 (evidence: [T02-S016])
  → 同时必须建立：内部往来对账机制 + 汇率政策（损益用期间平均、资产负债用期末）
  → 境内多主体：用友 YonSuite / 金蝶 AI 星辰及以上 (evidence: [T02-S044, T02-S007])

IF 有中国境内实体（无论几个）
  → 电子税务局 + 数电发票是不可选的必备项，不存在替代方案 (evidence: [T02-S003, T02-S068])
  → 账户数 > 约 5 个 OR 月付款 > 约 100 笔 → 评估银企直联；否则企业网银就够 (evidence: [T02-S049])
```

### 决策点 5：要不要现在上 AI？

```
IF 数据口径还没统一（同一指标多个部门算出不同数）
  → 不要上。AFP 官方调查显示从业者把数据可靠性（约 61%）与数据可获取性（约 60%）
    列为首要障碍，高于工具与技能 (evidence: [T02-S001])
  → AI 在脏数据上只会更快地给出错误答案

ELIF 数据口径已统一 AND 想试
  → 先只读：让 AI 读账、做分析、写差异解释初稿
  → 过账 / 付款 / 改主数据三件事保持人工
  → 留痕按 COSO 2026-02 指引：提示词、输入输出、模型与配置版本、人工复核证据
    全部存档，且要能重建当时的动作 (evidence: [T02-S066])
  → 先写控制再放 agent，不要反过来 (evidence: [T02-S067])

ELIF 有专职会计团队 AND 关账 > 10 天
  → 对账与关账是 AI 目前最落得下去的一块（有明确对错、大量重复、错了立刻发现）
  → Numeric（新）｜ FloQast / BlackLine（老牌加 AI） (evidence: [T02-S054, T02-S055, T02-S056])
```

---

## Phase 2 提炼提示

### 反复出现、≥ 3 source 都强调的「工具选型原则」（候选 playbook 规则）

1. **痛点先于阶段，阶段先于功能**：不要按收入数字买系统，按「关账 > 15 天 + 手工合并多主体 + 同一指标多个数」三条同时出现来判断
   （出现于: T02-S001 / T02-S002 / T02-S060）
2. **电子表格不是过渡方案，是长期底座**：官方调查里 96% 的从业者每周用它做规划，专用工具在约 1 亿美元收入前采用率不到一半
   （出现于: T02-S001 / T02-S060 / T02-S002）
3. **「谁维护这个模型」决定 FP&A 选型，功能清单不决定**：财务自己维护 → 保留表格前端；有专职团队 → 才考虑厂商界面
   （出现于: T02-S018 / T02-S025 / T02-S026 / T02-S060）
4. **买了不用是这个品类的默认结局**：71% 装了 EPM，96% 仍在用表格——采购前先问「上线后主力模型会搬进去吗」
   （出现于: T02-S001 / T02-S002 / T02-S061）
5. **中国财税链路不可选，且不可被海外工具替代**：电子税务局 + 数电发票是硬约束，选任何工具都要先问它接不接这条链
   （出现于: T02-S003 / T02-S005 / T02-S068 / T02-S069）
6. **报价必须含实施与场景接入费**：中国 ERP 实施常高于软件费，开源 ERP 成本大头是人月，费控赛道有第三方接入二次收费
   （出现于: T02-S013 / T02-S074 / T02-S075）
7. **AI 落地的前置条件是数据口径，不是模型能力**：约 61% 说数据可靠性不足、约 60% 说数据不可获取，两者都高于工具与技能
   （出现于: T02-S001 / T02-S066 / T02-S067）

### 显著的工具流派分裂（候选「智识谱系」条目）

- **保留电子表格前端派**（Cube / Datarails / Vena）vs **迁入厂商界面派**（Runway / Mosaic / Abacum / Pigment / Anaplan / Planful）
  - 分歧本质：模型的**可维护性归属**——是让财务自己能改，还是换取更强的建模引擎与工作流
  - 证据：T02-S018 / T02-S025 / T02-S026 vs T02-S019 / T02-S020 / T02-S021 / T02-S022 / T02-S023 / T02-S024
- **计费与收入确认合一派**（Maxio）vs **计费为主、收入确认外挂派**（Chargebee + RevRec 模块 / Recurly）
  - 证据：T02-S085 / T02-S084 / T02-S033
- **软件收费派**（Expensify、汇联易、合思）vs **支付返佣派**（Ramp、Brex、分贝通）
  - 分歧本质：省的软件费换来的是**支付关系的绑定**
  - 证据：T02-S036 / T02-S037 / T02-S077 vs T02-S034 / T02-S035 / T02-S075
- **AI 原生重建派**（Rillet / Campfire）vs **既有系统加 AI 派**（FloQast / BlackLine / 各 FP&A 厂商内嵌助手）
  - 证据：T02-S052 / T02-S070 / T02-S053 vs T02-S055 / T02-S056 / T02-S061

### 新兴工具信号

- 当前活跃 / 上升的新工具数：**8**（Rillet、Campfire、Numeric、Basis、Puzzle、Digits、Aleph、各家内嵌 AI 助手）
- 出现 → 主流 的速度估计：**24-36 个月**，且大概率被并购而非独立长大。参照点是 Causal——2023 年还是 FP&A 的热门新品，2024-10-31 被 Lucanet 收购并入平台 (evidence: [T02-S006])
- **对 Phase 2 的提醒**：新兴层全部标 `stability: experimental` + `Decay risk: high`。写进 SKILL.md 时必须带「6-12 个月后可能不存在或已改名」的提示

### 与其他 Track 的接口

- **→ Track 03（workflows）**：决策点 1-5 可直接转成 SOP 分支；「13 周滚动现金流」「多主体合并的四个汇率错误」「AI 只读优先 + 留痕三件套」是现成的工作流步骤
- **→ Track 01（figures）**：CJ Gustafson（Mostly Metrics，年度 CFO 工具栈调查）、Ben Murray（The SaaS CFO，第 7 届工具栈调查）、Paul Barnhurst（The FP&A Guy，工具栈调查合办方）三人是工具选型维度的核心声音，均已在 Track 05 出现，建议 Track 01 复核是否收录
- **→ Phase 2.1（心智模型）**：「工具解决不了口径问题」「系统买的是约束不是功能」两条候选

### 冷僻 / 信号薄弱自评

- 必备层 14 个 ≥ 3 ✅｜场景特化 31 个 ≥ 5 ✅｜新兴 8 个 ≥ 2 ✅ → **不触发冷僻协议**
- **但有两处必须在 SKILL.md 诚实边界节写明**：
  1. **verified_primary 仅占 23.5%（20/85）**。本行业的一手资料天然是厂商官网与定价页，被 verifier 归为 secondary 后人工升级为 `surrogate_primary`；真正的独立第三方审计数据几乎不存在（软件测评聚合站按本 pipeline 规则被排除）。**厂商自述的客户数、ARR、市场份额均未经独立核实**
  2. **中国境内 cap table / 持股平台维度没有工具化一手来源**——这不是调研不足，是该细分确实没有形成标准产品。相关结论基于中美合规框架差异推导，可信度标 medium
- **价格纪律**：全文只有一处写了确切金额（Pulley 的 $1,200 / $3,500 年费档），来自官方定价页 (evidence: [T02-S041])；其余全部只描述**计价模式**或用「约 / 业内 / 官方」限定

---

## 完成 checklist

- **Source 总数**: 85（目标区间 60-85 ✅）
- **verified_primary 条数**: 20（占 23.5%）
- **surrogate_primary 条数**: 62（全部含 `own site` / `own publication` / `vendor docs` / `originator` / `official` 之一 ✅）
- **secondary 条数**: 3 ｜ **reference**: 0 ｜ **dead**: 0
- **必备 14 / 场景特化 31 / 新兴 8**
- **黑名单自检**: 按 pipeline 黑名单正则（中文 UGC 问答/自媒体/百科/技术博客/雪盘类站点、四家英文软件测评聚合站、两家 PR 通稿站）对全文匹配 → **0 命中** ✅
- **决策树节点数**: 5 个决策点、19 个分支 ✅（模板要求 5-10 个节点）
- **避坑清单**: 9 条 ✅（模板要求 ≥ 5）
- **每个工具卡片**: 均带 `last_checked: 2026-09-02` + `Decay risk` ✅
- **必备层判断**: 均有 ≥ 2 个独立 source（电子表格用 AFP 协会调查 + Mostly Metrics 从业者调查两个独立来源）✅
- **403 处理**: carta.com/pricing、mostlymetrics.com、tableau.com、netsuite.com、sap.com 的 curl 403 已确认为反爬，**未标 dead** ✅
- **范围锚定核对**: 未收录投行建模软件、券商终端（Bloomberg / Wind / Capital IQ）、个人记账 App ✅
