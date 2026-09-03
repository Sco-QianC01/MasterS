# Track 02 — 谈判与议价：工具地图

调研日期：2026-09-02 · locale：zh-CN · 行业范围：谈判与议价的**通用**工具栈（排除单一行业销售话术工具、投行并购执行系统、招聘 ATS、诉讼案件管理）

> **这一 track 的核心判断**：谈判这一行最重要的工具是**纸笔工具与结构化模板**，不是软件。
> 一张 SaaS 产品清单不是谈判工具地图。软件只占三层里的一层，而且是**流程层**，不是**思考层**。
> 下面的必备层里没有一个是软件——它们是十几张表和几套问题清单，用 Excel、Word 甚至笔记本就能落地。

## Source Manifest

> HTTP 存活抽查（2026-09-02）：`acquisition.gov`、`knowledge.insead.edu`、`support.ironcladapp.com`、
> `first.army.mil`、`levels.fyi` 返回 403/405，属反爬拦截而非死链，页面在浏览器可正常打开；
> 其余抽查项均返回 200。bucket 一栏按 `tools/research/source_verifier.py classify` 的结果填写，
> 纯商业 SaaS 的产品页与帮助中心一律降为 `surrogate_primary` 并在 note 标 `vendor docs`。

| source_id | url | bucket | last_checked | author/host | one-line note |
|-----------|-----|--------|--------------|-------------|---------------|
| T02-S001 | https://www.pon.harvard.edu/daily/negotiation-skills-daily/negotiation-preparation-checklist/ | verified_primary | 2026-09-02 | Harvard PON | 谈判准备清单的标准条目与顺序 |
| T02-S002 | https://www.pon.harvard.edu/daily/negotiation-training-daily/negotiating-for-continuos-improvement-use-a-negotiation-preparation-worksheet/ | verified_primary | 2026-09-02 | Harvard PON | 准备表格用于持续改进，而非一次性填写 |
| T02-S003 | https://www.pon.harvard.edu/tag/scoring-system/ | verified_primary | 2026-09-02 | Harvard PON | 议题打分表（scoring system）的教学用法合集 |
| T02-S004 | https://www.pon.harvard.edu/teaching-materials-publications/ | verified_primary | 2026-09-02 | Harvard PON | 课程 教材 — 角色扮演模拟与教案总目录 |
| T02-S005 | https://www.pon.harvard.edu/store/ | verified_primary | 2026-09-02 | Harvard PON TNRC | 课程 教材 — 谈判教学资源中心在售清单 |
| T02-S006 | https://www.pon.harvard.edu/daily/dealmaking-daily/the-benefits-of-multiple-offers/ | verified_primary | 2026-09-02 | Harvard PON | MESO 多个等值同时报价的定义与好处 |
| T02-S007 | https://www.kellogg.northwestern.edu/academics-research/research/detail/2005/putting-more-on-the-table-how-making-multiple-offers/ | verified_primary | 2026-09-02 | Kellogg / Northwestern | Medvec & Galinsky 的 MESO 原始研究摘要 |
| T02-S008 | https://www.pon.harvard.edu/daily/teaching-negotiation-daily/teaching-negotiation-exercises-idecisiongames/ | verified_primary | 2026-09-02 | Harvard PON | PON 对在线角色扮演平台的官方说明 |
| T02-S009 | https://idecisiongames.com/promo-education | surrogate_primary | 2026-09-02 | iDecisionGames | vendor docs — 谈判模拟平台的功能与教学定位 |
| T02-S010 | https://www.first.army.mil/Portals/102/FM%207-0%20Appendix%20K.pdf | verified_primary | 2026-09-02 | US Army First Army | 监管 — FM 7-0 附录 K，复盘（AAR）的官方四问法 |
| T02-S011 | https://www.nwcg.gov/wfldp/toolbox/aars | verified_primary | 2026-09-02 | US NWCG | 监管 — 联邦机构版复盘工具箱与实施要点 |
| T02-S012 | https://www.esd.whs.mil/portals/54/documents/dd/issuances/dodi/500073p.pdf | verified_primary | 2026-09-02 | US DoD | 监管 — DoDI 5000.73 成本分析与 should-cost 审查程序 |
| T02-S013 | https://www.acquisition.gov/far/15.404-1 | verified_primary | 2026-09-02 | US Acquisition.gov | 监管 — FAR 15.404-1 成本分析与价格分析的法定方法 |
| T02-S014 | https://www.acquisition.gov/dlad/15.407-90-reverse-auction. | verified_primary | 2026-09-02 | US Acquisition.gov | 监管 — 反向拍卖在联邦采购中的条款定义 |
| T02-S015 | https://www.gao.gov/assets/d14108.pdf | verified_primary | 2026-09-02 | US GAO | 监管 — 反向拍卖审计：无竞争时省钱效果消失 |
| T02-S016 | https://www.gao.gov/assets/700/693406.pdf | verified_primary | 2026-09-02 | US GAO | 监管 — 反向拍卖后续审计，单一供应商比例问题 |
| T02-S017 | https://www.federalregister.gov/documents/2024/07/30/2024-16281/federal-acquisition-regulation-reverse-auction-guidance | verified_primary | 2026-09-02 | US Federal Register | 监管 — FAR 反向拍卖指引最终规则（2024-07-30） |
| T02-S018 | https://learning.sap.com/learning-journeys/introducing-projects-within-sap-ariba-sourcing/understanding-auction-attributes | surrogate_primary | 2026-09-02 | SAP | vendor docs — Ariba 三种反向拍卖形式的官方定义 |
| T02-S019 | https://compass.coupa.com/en-us/products/product-documentation/supplier-resources/for-suppliers/coupa-supplier-portal/set-up-the-csp/sourcing/sourcing-events-types-for-suppliers | surrogate_primary | 2026-09-02 | Coupa | vendor docs — 寻源事件类型：RFx / 英式 / 荷式反向拍卖 |
| T02-S020 | https://support.keelvar.com/hc/en-us/articles/4417361154322-Autonomous-Sourcing-overview | surrogate_primary | 2026-09-02 | Keelvar | vendor docs — 自动化寻源机器人的角色与审批流 |
| T02-S021 | https://www.keelvar.com/sourcing-automation | surrogate_primary | 2026-09-02 | Keelvar | vendor docs — 厂商自报可减少 90% 战术工作量 |
| T02-S022 | https://support.ironcladapp.com/hc/en-us/articles/30659446762647-Clause-Library-Overview | surrogate_primary | 2026-09-02 | Ironclad | vendor docs — 条款库的数据结构与维护方式 |
| T02-S023 | https://support.ironcladapp.com/hc/en-us/articles/12275685560215-Ironclad-AI-Playbooks-Overview | surrogate_primary | 2026-09-02 | Ironclad | vendor docs — playbook 是决策层，条款库是语言层 |
| T02-S024 | https://support.ironcladapp.com/hc/en-us/articles/36782585702807-Manage-Playbooks-in-Your-Playbook-Library | surrogate_primary | 2026-09-02 | Ironclad | vendor docs — 超过 30 本 playbook 后性能下降 |
| T02-S025 | https://pactum.com/clients | surrogate_primary | 2026-09-02 | Pactum | vendor docs — 自动化议价 agent 的客户成效自报 |
| T02-S026 | https://thunderbird.asu.edu/thought-leadership/journals-case-series/case-series-listing/pactums-ai-contract-negotiations | verified_primary | 2026-09-02 | ASU Thunderbird | 课程 — 高校案例研究，独立复述沃尔玛/马士基部署 |
| T02-S027 | https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32023L0970 | verified_primary | 2026-09-02 | EUR-Lex | 监管 — 欧盟薪酬透明指令原文，含招聘前披露义务 |
| T02-S028 | https://www.cac.gov.cn/2004-08/28/c_126468489.htm | verified_primary | 2026-09-02 | 中央网信办 | 监管 — 《电子签名法》原文，可靠电子签名四要件 |
| T02-S029 | https://gongbao.court.gov.cn/Details/ae403b9e6030a2b7c450fad89bdf76.html | verified_primary | 2026-09-02 | 最高人民法院公报 | 监管 — 私自录音证据效力的司法批复原文 |
| T02-S030 | https://www.cietac.org/en/articles/15778 | surrogate_primary | 2026-09-02 | CIETAC | 协会 — 在线立案系统上线公告与适用范围 |
| T02-S031 | https://kt.cietac.org/portal/main/domain/index.htm | surrogate_primary | 2026-09-02 | CIETAC | 协会 — 智慧庭审平台入口 |
| T02-S032 | https://arxiv.org/abs/2401.04536 | verified_primary | 2026-09-02 | Bianchi et al. | 用谈判博弈评测语言模型自主性的方法论论文 |
| T02-S033 | https://www.levels.fyi/ | secondary | 2026-09-02 | Levels.fyi | 用户自报薪酬，非雇主披露，选择性偏差明显 |
| T02-S034 | https://support.docusign.com/s/document-item?language=en_US&bundleId=pxt1643324456371&topicId=oro1670948103764.html | surrogate_primary | 2026-09-02 | Docusign | vendor docs — 自定义条款库的管理员配置说明 |
| T02-S035 | https://www.fadada.com/about | surrogate_primary | 2026-09-02 | 法大大 | vendor docs — 中国电子签与合同管理服务范围自述 |
| T02-S036 | https://www.esign.cn/product/platform | surrogate_primary | 2026-09-02 | e签宝 | vendor docs — 签管一体化平台的功能边界自述 |
| T02-S037 | https://juro.com/learn/contract-playbook | surrogate_primary | 2026-09-02 | Juro | vendor docs — 条款库与谈判 playbook 的实践说明 |
| T02-S038 | https://linksquares.com/ai-legal-assistant/contract-playbooks/ | surrogate_primary | 2026-09-02 | LinkSquares | vendor docs — playbook 内嵌到起草与谈判流程 |
| T02-S039 | https://www.agiloft.com/blog/scaling-your-legal-expertise-why-contract-playbooks-are-essential | surrogate_primary | 2026-09-02 | Agiloft | vendor docs — 标准条款 / fallback 条款的两级分类 |
| T02-S040 | https://www.salesforce.com/blog/sales/deal-desk/ | surrogate_primary | 2026-09-02 | Salesforce | vendor docs — deal desk 的组成：审批矩阵 + 负责人 + 时限 |
| T02-S041 | https://www.salesforce.com/sales/cpq/what-is-cpq/ | surrogate_primary | 2026-09-02 | Salesforce | vendor docs — CPQ 的定义与它不做的事 |
| T02-S042 | https://arxiv.org/html/2508.03080 | verified_primary | 2026-09-02 | ContractEval 作者 | 条款级法律风险识别的 LLM 基准与失败率 |
| T02-S043 | https://dho.stanford.edu/wp-content/uploads/Legal_RAG_Hallucinations.pdf | verified_primary | 2026-09-02 | Stanford RegLab / HAI | 法律检索增强产品仍有可观幻觉率的实证研究 |
| T02-S044 | https://www.frontiersin.org/journals/artificial-intelligence/articles/10.3389/frai.2026.1782405/full | secondary | 2026-09-02 | Frontiers in AI | 合同条款抽取/分类/摘要的模型评测综述 |
| T02-S045 | https://dol.ny.gov/pay-transparency | verified_primary | 2026-09-02 | 纽约州劳工厅 | 监管 — 招聘启事必须写薪酬区间的法定要求 |
| T02-S046 | https://www.harvey.ai/blog/contract-intelligence-benchmark | surrogate_primary | 2026-09-02 | Harvey | vendor docs — 厂商自建合同理解基准，自报对比人类专家 |
| T02-S047 | https://levels.fyi/offerings/data/radford-comparison | surrogate_primary | 2026-09-02 | Levels.fyi | vendor docs — 自报数据与传统薪酬调研的口径差异 |
| T02-S048 | https://arxiv.org/pdf/2605.16575 | verified_primary | 2026-09-02 | arXiv 作者 | 「会建模对手 ≠ 会谈判」——LLM 谈判者的能力上限 |
| T02-S049 | https://pure.hud.ac.uk/ws/files/17720891/accepted_manuscript.pdf | verified_primary | 2026-09-02 | Univ. of Huddersfield | 微表情训练工具（METT）独立检验：不提升测谎表现 |
| T02-S050 | https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2020.613410/full | secondary | 2026-09-02 | Frontiers in Psychology | 非语言线索测谎研究综述：「一条死胡同」 |
| T02-S051 | https://www.pon.harvard.edu/daily/business-negotiations/negotiation-preparation-strategies/ | verified_primary | 2026-09-02 | Harvard PON | 准备阶段的标准动作顺序与常见遗漏 |
| T02-S052 | https://www.pon.harvard.edu/tag/reservation-price/ | verified_primary | 2026-09-02 | Harvard PON | 保留价的定义与它与 BATNA 的换算关系 |
| T02-S053 | https://www.pon.harvard.edu/daily/batna/batna-negotiators-how-you-can-avoid-striking-out-and-create-mutual-gains-in-your-next-business-negotiation/ | verified_primary | 2026-09-02 | Harvard PON | BATNA 四步评估法：列→评→定→算保留价 |
| T02-S054 | https://www.hbs.edu/ris/Publication%20Files/17-055_878a070d-7972-4ce3-95ce-73f424a38900.pdf | verified_primary | 2026-09-02 | Sebenius / HBS | 工作论文：BATNA 估算的常见错误与三种「不」 |
| T02-S055 | https://www.pon.harvard.edu/daily/business-negotiations/how-to-use-mesos-in-business-negotiations | verified_primary | 2026-09-02 | Harvard PON | MESO 的具体设计步骤与等值校准 |
| T02-S056 | https://www.pon.harvard.edu/daily/conflict-resolution/dealing-with-an-uncooperative-counterpart/ | verified_primary | 2026-09-02 | Harvard PON | 对手不肯交换信息时用 MESO 反推其偏好 |
| T02-S057 | https://www.pon.harvard.edu/uncategorized/making-concessions-in-negotiation-best-practices/ | verified_primary | 2026-09-02 | Harvard PON | 让步阶梯的教学口径：幅度递减传递什么信号 |
| T02-S058 | https://knowledge.insead.edu/strategy/negotiators-should-decrease-concessions-across-rounds | verified_primary | 2026-09-02 | INSEAD Knowledge | 课程 — 递减让步的实验结论（7 项研究，2311 人） |
| T02-S059 | https://www.sciencedirect.com/science/article/abs/pii/S0749597821000613 | secondary | 2026-09-02 | OBHDP (Elsevier) | 递减让步论文的期刊条目，摘要可读、全文付费 |
| T02-S060 | https://www.pon.harvard.edu/tag/logrolling | verified_primary | 2026-09-02 | Harvard PON | 跨议题交换（log-rolling）的教学页 |
| T02-S061 | https://www.pon.harvard.edu/daily/win-win-daily/get-off-on-the-right-foot/ | verified_primary | 2026-09-02 | Harvard PON | 用交换而非折中来创造价值的做法 |
| T02-S062 | https://link.springer.com/content/pdf/10.1023%2FA%3A1011262625052.pdf | secondary | 2026-09-02 | Group Decision & Negotiation | 多议题交换的形式化流程（学术全文 PDF） |
| T02-S063 | https://www.kellogg.northwestern.edu/academics-research/dispute-resolution-research-center/teaching-resources.aspx | verified_primary | 2026-09-02 | Kellogg DRRC | 课程 教材 — 200+ 谈判练习案例官方目录 |
| T02-S064 | https://teachwithkellogg.com/resource-center/royalty-free-exercises/ | surrogate_primary | 2026-09-02 | Kellogg | 教材 — 免版税练习，可直接组局对练 |
| T02-S065 | https://casestudies.law.harvard.edu/program-on-negotiation-1/ | verified_primary | 2026-09-02 | Harvard Law School | 课程 — PON 角色扮演与案例的官方购买入口 |
| T02-S066 | https://www.bls.gov/ppi/ | verified_primary | 2026-09-02 | 美国劳工统计局 | 监管 — 生产者价格指数，调价条款的官方锚 |
| T02-S067 | https://www.bls.gov/oes/ | verified_primary | 2026-09-02 | 美国劳工统计局 | 监管 — 职业就业与工资统计，薪酬谈判的公共基准 |
| T02-S068 | https://www.ismworld.org/supply-management-news-and-reports/reports/ism-pmi-reports/ | verified_primary | 2026-09-02 | ISM | association — 月度 PMI，含可引用的 Prices Index |
| T02-S069 | https://www.stats.gov.cn/ | verified_primary | 2026-09-02 | 国家统计局 | 监管 — 中文侧 PPI/CPI 官方发布方 |
| T02-S070 | https://cicc.court.gov.cn/html/1/218/149/192/2436.html | verified_primary | 2026-09-02 | 最高人民法院 | 监管 — 一站式国际商事纠纷平台工作指引（试行） |
| T02-S071 | https://cicc.court.gov.cn/html/1/259/263/index.html | verified_primary | 2026-09-02 | 最高人民法院 CICC | 监管 — 一站式平台准入的调解与仲裁机构名录 |
| T02-S072 | https://siac.org.sg/siac-simc-arb-med-arb-model-clause | surrogate_primary | 2026-09-02 | SIAC | 协会 — 仲裁-调解-仲裁示范条款官方页 |
| T02-S073 | https://simc.com.sg/arb-med-arb | surrogate_primary | 2026-09-02 | SIMC | 协会 — 三段式流程与 8 周调解时限 |
| T02-S074 | https://www.hkiac.org/mediation/rules/hkiac-mediation-rules | surrogate_primary | 2026-09-02 | HKIAC | 协会 — 香港调解规则官方页 |
| T02-S075 | https://www.cietac.org/en/articles/25161 | surrogate_primary | 2026-09-02 | CIETAC | 协会 — 贸仲调解中心《调解规则》全文 |
| T02-S076 | https://execed.business.columbia.edu/programs/negotiation-strategies-online | verified_primary | 2026-09-02 | Columbia Exec Ed | 课程 — 正式课程里已含 AI 对手模拟 |
| T02-S077 | https://pll.harvard.edu/course/negotiation-mastery | verified_primary | 2026-09-02 | Harvard (PLL) | 课程 — 官方页写明含 AI 驱动的互动谈判模拟 |
| T02-S078 | https://www.coursera.org/learn/negotiation-skills | surrogate_primary | 2026-09-02 | Coursera / Michigan | 课程 — Siedel 四步流程（准备/谈判/收口/复盘） |
| T02-S079 | https://online.umich.edu/content/george-siedel-qa-successful-negotiation/ | verified_primary | 2026-09-02 | Michigan Online | 课程 — 校方访谈：准备清单为何是第一位 |
| T02-S080 | https://www.pon.harvard.edu/daily/negotiation-skills-daily/negotiation-research-you-can-use-why-displays-of-anger-can-backfire-nb | verified_primary | 2026-09-02 | Harvard PON | 假装愤怒等情绪战术在实验中反噬的综述 |
| T02-S081 | https://www.spp.gov.cn/spp/ssmfdyflvdtpgz/202008/t20200831_478413.shtml | verified_primary | 2026-09-02 | 最高人民检察院 | 监管 — 民法典合同编全文（要约/承诺/缔约过失） |
| T02-S082 | https://www.court.gov.cn/zixun/xiangqing/419382.html | verified_primary | 2026-09-02 | 最高人民法院 | 监管 — 合同编通则解释：预约合同与诚信义务 |
| T02-S083 | https://corpgov.law.harvard.edu/2025/07/30/when-term-sheet-provisions-survive-the-execution-of-definitive-agreements/ | verified_primary | 2026-09-02 | Harvard Law School | 条款清单里哪些条款会在正式合同后仍存续 |
| T02-S084 | https://www.ismworld.org/globalassets/pub/docs/210_ethics_book.pdf | verified_primary | 2026-09-02 | ISM | association — 采购从业者道德准则原文，约束议价手段 |
| T02-S085 | https://www.thegappartnership.com/insights/ | surrogate_primary | 2026-09-02 | The Gap Partnership | vendor docs — 采购侧谈判咨询公司官方文章库 |
| T02-S086 | https://www.scientificamerican.com/article/humans-are-pretty-lousy-lie-detectors/ | secondary | 2026-09-02 | Scientific American | 测谎准确率略高于随机的科普综述 |
| T02-S087 | https://artofprocurement.com/podcast | verified_primary | 2026-09-02 | Philip Ideson | own site — 采购实战播客，AI 落地与投资回报专题 |
| T02-S088 | https://www.pon.harvard.edu/publications/negotiation-data-repository/ | verified_primary | 2026-09-02 | Harvard PON | 谈判实验数据仓库，可核对教学结论的原始数据 |

## 三层工具

分层的判据不是「软件 vs 非软件」，而是**这场谈判的胜负手在哪一层**：
必备层管**你自己想清楚了没有**，场景特化层管**流程和信息差**，新兴层管**还没定论的东西**。

### 必备层（10 项）

必备层十项**全部是纸笔工具**——Excel、Word、笔记本都能落地，不需要采购任何软件。
它们的共同点是：**在谈判开始之前就得填完**。临场想不出来的东西，工具救不了。

| # | 工具 | 它解决什么问题 | 怎么用（最小可行版） | 最常见的做错方式 | evidence |
|---|------|--------------|------------------|---------------|----------|
| 1 | **谈判准备清单 + 议题矩阵**（issue × 双方优先级） | 把「我要谈什么」从一句模糊目标拆成一张可核对的表，并强迫你写出**对方**的优先级 | 一列写全部议题（价格、账期、量、交付、责任、排他、续约……），两列分别打「我方重要度」和「我方猜的对方重要度」，第三列写「这个猜测的依据是什么」。空着的依据格就是你的调研任务清单 | ① 只列自己关心的议题，把对方那一列留空或凭感觉填；② 把清单当成一次性文件填完就扔，而不是每轮谈完回来改 | evidence: [T02-S001, T02-S002, T02-S051, T02-S079] |
| 2 | **替代方案与保留价估算表**（BATNA / WATNA / reservation price / target） | 回答「谈崩了我怎么办」和「低于多少我就走」这两个问题——这是全部谈判筹码的来源 | 四步：列出所有替代方案 → 逐个估值（含时间成本与不确定性）→ 取最好的那个作为 BATNA → 把 BATNA 折算成桌面上的**保留价**。再单独写一行 target（想要的价），它和保留价是两个数 | ① 把「我希望的价格」当成保留价，两个数混成一个；② 只估自己的 BATNA 不估对方的；③ 把 BATNA 当成一个静止的数字，忽略它在谈判期间会变（对方的替代方案在流失、你的期权在到期） | evidence: [T02-S052, T02-S053, T02-S054] |
| 3 | **议题打分表**（scoring system） | 把多议题谈判变成可算总分的数字问题，让你在桌上能**当场比较**两个结构完全不同的方案 | 给每个议题分配点数（总和 100），每个议题内的各档位再给分。对方给的任何一个报价都能算出一个总分，和你的保留价（也是一个分数）直接比 | ① 分配点数时按「重要」拍脑袋，没有和保留价挂钩，导致算出来的分没有决策意义；② 只给自己建打分表，不去反推对方的打分表——反推对方的分才是找交换空间的入口 | evidence: [T02-S003, T02-S063] |
| 4 | **可交换筹码与打包方案表**（log-rolling / trade matrix） | 把「我让一步你让一步」的对切，换成「我在你不在乎的地方让、你在我不在乎的地方让」的交换 | 用第 1 项的议题矩阵，找出**双方优先级排序不同**的议题对，一对一对写下来：「我给你 X（我便宜、你贵），换你给我 Y（你便宜、我贵）」。永远**成对**报价，不单独让 | ① 逐个议题依次谈（sequential），这会杀掉全部交换空间——多议题必须**同时**摆上桌；② 议题数堆得过多，超过双方能同时处理的范围反而降低协议质量；③ 把「折中」当成「交换」——对半砍是没有创造价值的 | evidence: [T02-S060, T02-S061, T02-S062] |
| 5 | **多个等值同时报价表**（MESO，Multiple Equivalent Simultaneous Offers） | 同时抛出 2-3 个**对你价值相同、结构不同**的方案。对方挑哪个，就暴露了他的优先级——这是不靠提问就能拿到对方偏好信息的办法 | 用第 3 项的打分表，构造 2-3 个总分相同（对你等值）但议题组合不同的包。同时给出，说明「这三个对我一样，你更喜欢哪个」 | ① 三个方案对你其实不等值（有一个是你偷偷偏好的），一旦被识破就是明显的诱导；② 一次给五六个，对方直接过载放弃选择；③ 把 MESO 当成「多给几个折扣档」——它的价值在**结构不同**，不在价格档位不同 | evidence: [T02-S006, T02-S007, T02-S055, T02-S056] |
| 6 | **让步阶梯与让步理由库** | 预先写好「我准备让几步、每步多大、每步换回什么、每步的说法是什么」，避免临场被时间压力推着乱让 | 一张表：轮次 / 我方让步内容 / 幅度 / 换回什么 / 对外的理由。**幅度逐轮递减**是默认设计 | ① 让步不换东西（单方面让步会被读作「还有空间」）；② 幅度不递减甚至放大，等于告诉对方再压还有；③ 只准备自己的阶梯，不准备**接收方对策**——实验证据显示，面对递减让步的一方会形成对方已到底线的错觉，从而报出更保守的还价、拿到更差的结果，唯一有效的自保是**入场前先定死自己的 target** | evidence: [T02-S057, T02-S058, T02-S059] |
| 7 | **授权与升级路径表**（谁能批到哪一档） | 让谈判桌上的人清楚知道自己能签什么、超过哪条线要回去请示、请示要多久 | 三列：条款/金额档位 → 谁能批 → 承诺的回复时限。谈判前和内部对齐，谈判中直接对照 | ① 没有这张表，谈判者要么越权承诺、要么什么都答应不了；② 把「有限授权」当纯战术（假装要请示）而忘了它首先是**内部治理**；③ 只写审批人不写时限，结果每一档都变成无限期拖延 | evidence: [T02-S040, T02-S023, T02-S039] |
| 8 | **开场脚本与校准问题清单** | 前十分钟决定了议程和锚点。脚本管你不把开场浪费掉；校准问题清单管你在对方发言时问出结构性信息而不是是非题 | 脚本写三样：议程提议、你希望先谈哪个议题、第一个数字（如果你决定先报价）。问题清单写 8-10 个开放式问句（「这个交付期对你们意味着什么」「如果预算不动，哪一块可以调整」），全部避免可以用「是/否」回答 | ① 把脚本写成逐字话术，一旦对方不按剧本走就失灵——脚本要写**目标**不写台词；② 问了开放式问题却不留白，自己接着说下去；③ 相信「必胜开场白」这类东西存在 | evidence: [T02-S051, T02-S079, T02-S078] |
| 9 | **复盘表**（after-action review） | 把一次谈判变成可复用的经验。没有复盘的人谈十年也只是把第一年重复了十遍 | 四问，逐字照抄军方版本即可：① 本来应该发生什么？② 实际发生了什么？③ 为什么有差异？④ 哪些要保持、哪些要改？谈完 48 小时内做，参与者按角色而非职级发言 | ① 变成追责会——复盘的规矩是「把军衔留在门外」，一旦开始找人背锅就再也拿不到真话；② 只复盘输掉的谈判，赢的不复盘（赢的那次可能只是对方犯错）；③ 不落成文档，下次准备时无从调取 | evidence: [T02-S010, T02-S011, T02-S078] |
| 10 | **会议纪要与书面确认模板** | 谈完之后 24 小时内发出的那封确认信，往往比谈判本身更决定最终条款——因为它定义了「我们谈成了什么」 | 固定四段：已达成共识的点 / 仍有分歧的点 / 双方各自的下一步动作与时限 / 明确写「本函为纪要，不构成有约束力的最终协议」（或相反，视你的意图而定） | ① 不发，靠记忆和口头；② 发了但没写清楚有没有约束力——中国法下预约合同与善意磋商义务是真实存在的，一份写法草率的纪要可能被认定产生缔约拘束；③ 把对方没同意的点写成「已达成」，一次就烧掉信任 | evidence: [T02-S081, T02-S082, T02-S083] |

**必备层的整体判断**：这十项里面，**第 1、2、3 项是硬地基**——没有议题矩阵、保留价和打分表，第 4-6 项（交换、MESO、让步阶梯）根本没法构造，因为它们全部要用到打分表里的数字。
第 9、10 项是**唯二能让水平随时间上升**的工具，也是最常被跳过的两项。

`last_checked: 2026-09-02` · Decay risk: **low**（这十项的形态在过去三十年基本没变，教学口径稳定）


### 场景特化层（11 项）

这一层才开始出现软件。判断标准是：**只有当你的谈判量大到人手管不过来，或者你的胜负手在信息与流程上，这些工具才有意义**。
单次、高价值、非重复的谈判（比如一次融资、一次跳槽）用不到这一层的任何一项。

| # | 工具 / 类别 | 适用场景（什么时候才上） | 关键事实 | 注意 / 不适合 | evidence |
|---|-----------|---------------------|---------|-------------|----------|
| 1 | **合同全生命周期管理与条款库**（Ironclad、Docusign CLM、Juro、LinkSquares、Agiloft） | 每月几十份以上同类合同，且法务人手不够逐份看 | 条款库存的是「已审批语言」；**playbook 是叠在条款库之上的决策层**——什么时候用哪条、先给哪个 fallback、越过哪条线必须升级。Agiloft 的做法是把条款直接分成 standard 与 fallback 两级；Ironclad 的 playbook 库有实操上限，官方文档写明超过 30 本后性能开始下降 | 条款库**不是**谈判工具，它是**执行一致性**工具。它让一百个销售给出同样的让步，但不会让任何一次让步更聪明。买了不维护是这一层最贵的失败 | evidence: [T02-S022, T02-S023, T02-S024, T02-S034, T02-S037, T02-S038, T02-S039] |
| 2 | **中国侧电子签与合同管理**（法大大、e签宝） | 中国境内签署、需要存证与出证的场景 | **电子签名与条款库是两件事，必须分开看**。《电子签名法》规定的是「可靠的电子签名」四要件（专有、签署时仅签名人控制、签名改动可发现、文件改动可发现），满足即与手写签名或盖章同等法律效力——这解决的是**签得成不成立**，不是**条款谈得好不好**。两家厂商近年都在电子签之上叠加合同模板、智能审阅与合同管理模块（厂商自报，无第三方审计） | 采购时最常见的错误是把电子签平台当成条款库买。**先问一句：我要的是「签得快」还是「条款不失控」**——前者买电子签，后者要的是 playbook 与授权表，很多时候一张 Excel 就够 | evidence: [T02-S028, T02-S035, T02-S036] |
| 3 | **采购电子寻源平台**（SAP Ariba、Coupa、Jaggaer） | 规格清晰、供应商多、需要留下合规记录的重复性采购 | 主流平台的寻源事件类型大同小异：RFI/RFQ/RFP 加上英式反向拍卖（价格逐步走低）与荷式反向拍卖（价格自动上抬直到有人接）。Ariba 另有日式拍卖与带出价换算的变体。官方文档一致强调：拍卖前要先跑 RFI/RFP 把规格问清楚 | 平台本身不产生议价能力，**竞争才产生议价能力**。规格模糊、供应商稀少的品类放进电子寻源只会把关系谈坏 | evidence: [T02-S018, T02-S019] |
| 4 | **反向拍卖**（作为一种机制，而非某个产品） | 商品化程度高、切换成本低、真有 3 家以上能供的品类 | 美国联邦采购法规里有专门条款定义它，2024-07-30 联邦公报发布了最终指引规则。但**审计证据是负面的**：美国政府问责局（GAO）两份报告指出，当参与竞标者过少（相当比例的联邦反向拍卖最终只有一个报价者）或标的是复杂服务时，反向拍卖的节约效果消失甚至为负 | 这是本层里**厂商宣称与独立审计分歧最大**的一项。买之前先数一数你这个品类真实有几家能供；数不到三家就不要用 | evidence: [T02-S014, T02-S015, T02-S016, T02-S017] |
| 5 | **自动化寻源机器人**（Keelvar） | 长尾、低金额、高频次的战术性采购（例如运费询价） | 按品类配置机器人，自动完成请求接收、标书生成、供应商邀请、催办、比价、场景建模与授标建议；超出预设参数（异常报价、供应商不响应、节约未达阈值）时抛给人工。**厂商自报可减少至多 90% 的战术工作量、至多 25% 成本，无第三方审计** | 它自动化的是**流程**不是**判断**。护栏（邀请谁、审批阈值、什么算有效报价）仍然全部由人预先写死——这些护栏本身就是一张授权表，回到必备层第 7 项 | evidence: [T02-S020, T02-S021] |
| 6 | **自动化议价 agent**（Pactum） | 长尾供应商数量以千计、单个供应商谈判的人力成本高于收益 | 已在大型零售与航运企业部署。**成效数据全部为厂商与其客户自报，无独立审计**，且不同来源口径互相矛盾：达成率有 64%、68%、72% 三个不同数字在流传，平均收益「约 3%」，账期平均延长约 35 天，供应商体验满意度 83%。可交叉核验的独立材料是高校案例研究，但它复述的仍是同一批企业口径 | 它谈的是**参数**（价格档、账期、返点），不是**结构**。一切需要重新定义交易结构的谈判都不在它的能力范围内。详见新兴层第 3 项 | evidence: [T02-S025, T02-S026] |
| 7 | **销售侧折扣审批矩阵与 deal desk**（CPQ 类） | 销售团队规模大到折扣开始失控 | 一个能运转的 deal desk 需要四样东西：**书面的审批矩阵、指定的负责人、请求进入的固定渠道、承诺的回复时限**。CPQ（配置-定价-报价）软件做的是按折扣幅度、合同额、条款、产品组合自动路由审批 | **CPQ 不是谈判工具**，把它当谈判工具是本 track 最常见的外行错误之一。它执行你已经定好的定价政策；如果政策本身错了，CPQ 只会让错误执行得更快更一致 | evidence: [T02-S040, T02-S041] |
| 8 | **薪酬与职级数据**（Levels.fyi、Mercer、Radford、官方披露与统计） | 个人求职/涨薪谈判，以及雇主侧定薪 | 三类数据的口径完全不同：<br>① **法定披露**——欧盟薪酬透明指令要求在招聘启事或首次面试前给出薪酬或至少区间，并禁止询问薪酬史，成员国转化截止 2026-06-07（截至该日仅意大利、斯洛伐克、立陶宛、马耳他完成完整立法）；纽约州要求 4 人以上雇主在招聘启事写明区间，违规罚款按次递增至 3,000 美元。**这是唯一「对方必须给你」的数据**<br>② **官方统计**——美国劳工统计局职业工资统计等，覆盖广但滞后、颗粒度粗<br>③ **商业调研与自报**——Mercer / Radford 由参与企业提交数据、年度周期、同业聚合值；Levels.fyi 是用户自报、每日更新、精确到公司+职级+地点 | Levels.fyi 类数据有明显的**选择性偏差**（愿意上报的人和不愿上报的人不是同一批），且自报无法核验。用它定锚点可以，用它当谈判依据引用给对方会被打回。先查一遍你所在法域有没有强制披露——**有的话那才是最好用的一手** | evidence: [T02-S027, T02-S033, T02-S045, T02-S047, T02-S067] |
| 9 | **可比交易与市场价数据 / 调价指数** | 长约的调价条款、原材料波动的价格重谈 | 把调价绑定到**公开可核验的第三方指数**，而不是绑定到任何一方自己的成本口径。常用锚：美国生产者价格指数（PPI）、ISM 月度采购经理指数中的 Prices Index、中国国家统计局 PPI/CPI | 指数选错比不选更糟——绑到一个与你的实际成本结构相关性弱的指数，等于给自己或对方开了一张免费的期权。签之前用过去 3-5 年的数据回算一遍 | evidence: [T02-S066, T02-S068, T02-S069] |
| 10 | **争议解决机构的在线立案与调解平台**（CIETAC、SIAC/SIMC、HKIAC、最高法一站式平台） | 谈判可能谈崩、需要在合同里预先写好退路时 | 这些不是「谈判工具」，是**估算 BATNA 的工具**——「谈崩要花多少钱、多久」的唯一可靠答案在这些机构的规则与收费表里。CIETAC 自 2019-01-01 起有在线立案系统，并已升级为含在线立案、文件交换、线上开庭与裁决送达的平台；SIAC-SIMC 的仲裁-调解-仲裁示范条款走三段式，调解须在启动日起 8 周内完成；HKIAC 有独立的调解规则；中国最高法一站式国际商事纠纷平台自 2021-07 上线，可在线完成立案、调解、证据交换与庭审，并有准入机构名录 | 在合同起草阶段就要选定机构与规则，谈崩之后再选已经晚了。**跨境合同要注意中国仲裁法自 2026-03-01 施行后，各机构的配套规则修订需要复核** | evidence: [T02-S030, T02-S031, T02-S070, T02-S071, T02-S072, T02-S073, T02-S074, T02-S075] |
| 11 | **谈判模拟与教学材料**（PON 教学资源中心、Kellogg DRRC、iDecisionGames） | 要训练一个团队，或者要在真谈之前做一次带对手的演练 | PON 的教学资源中心有 25 年以上的角色扮演模拟、教案与课程大纲积累，另有 11 份按主题编的简明课纲；Kellogg 争议解决研究中心有 200 多个练习案例，并有一批免版税练习可直接取用；iDecisionGames 是把这些角色扮演搬到线上的平台（自动分角色、自动分组、可录像），素材来自 PON、Kellogg DRRC 等作者方 | 模拟练的是**流程与话术的肌肉记忆**，不是行业知识。你自己行业的真实条款和真实对手，模拟案例里没有——练完还是要回到必备层第 1-3 项自己填表 | evidence: [T02-S004, T02-S005, T02-S008, T02-S009, T02-S063, T02-S064, T02-S065] |

#### 场景特化层附条：录音与转写做复盘

把谈判录下来、转写成文字再逐句复盘，是提升最快的做法之一。**但它的第一约束是法律，不是工具选型。**
市面上的会议转写工具（会议软件自带的、或独立的转写服务）技术上都够用，真正会出事的是合法性：

- **中国大陆**：现行民事证据规则的排除标准是三条红线——以**严重侵害他人合法权益、违反法律禁止性规定、或严重违背公序良俗**的方法形成或获取的证据，不能作为认定事实的依据。早年最高人民法院曾有批复对未经对方同意私录采取更严的一刀切口径，后被上述标准取代。**实务含义**：在自己参与的、非私密场所的商务会谈中录音，通常不当然违法；但涉及私密空间、私密活动、他人隐私或商业秘密的录制风险显著上升，且《个人信息保护法》另有告知-同意要求。 (evidence: [T02-S029, T02-S081])
- **美国**：联邦与多数州采「一方同意」——你自己是对话参与者即可录；但有十余个州要求**全体同意**，且部分州对电话通话与面对面对话适用不同规则。**本条无法用一手来源逐州确认，属必须自查项**：请直接查目标州的成文法条，不要用汇总榜单或转写厂商的合规博客——这类页面更新滞后且没有法律责任。
- **欧盟 / GDPR**：录音属处理个人数据，需要一条合法性基础。在雇佣关系中**同意通常被认为不是有效基础**（因权力不对等），实务上多依赖「合法利益」，并须做利益衡量与事先告知。**本条同样缺一手来源，需以目标国数据保护机关的官方指引为准。**

**跨法域的安全默认做法**：开场就明说「我这边会做记录，方便会后确认，可以吗」。这既解决合法性，也把它变成第 10 项书面确认模板的输入。想靠偷录拿到「证据」的人，通常既承担了法律风险，又没拿到能用的东西。

`last_checked: 2026-09-02` · Decay risk：条款库/寻源平台/CPQ **medium**（产品迭代快但形态稳定）；法域合规部分 **high**（薪酬披露与录音规则每年都在变）


### 新兴 / 实验层（5 项）

全部标 `Decay risk: high` · `last_checked: 2026-09-02`。
这一层的写法与前两层不同：不写「怎么用」，写**现在可信到什么程度、已知怎么失败、厂商说的和能核实的差多少**。

| # | 工具 / 做法 | 现在可信到什么程度 | 已知失败模式 | 宣称 vs 可核实证据 | evidence |
|---|-----------|-----------------|------------|-----------------|----------|
| 1 | **大模型做对手模拟陪练与谈判前立场推演** | **可信度：中等，但仅限「陪练」用途。** 作为一个不知疲倦、随叫随到的对手来练开场、练异议应对、练把方案讲清楚，它是有用的；作为「预测真实对手会怎么反应」的推演引擎，没有证据支持 | ① 模型会顺着你的框架走，你把自己的假设喂进去，它把同样的假设还给你，你误以为得到了验证——这是最危险的一种失败，因为体验非常好；② 学术评测显示，模型能相当好地建模对手（推断偏好、追踪立场），但**建模对手不等于会谈判**，在需要构造让步顺序与承诺策略的地方仍然弱；③ 对同一情境重跑会给出不同建议，缺乏稳定性 | 厂商与课程宣传把它说成「AI 对手」；可核实的部分是**评测方法学已经建立**（用谈判博弈来评估模型自主性已是标准做法），而**「它能替代真人陪练」没有独立证据**。这一层最诚实的说法是：拿它练嘴，不要拿它做决策 | evidence: [T02-S032, T02-S048] |
| 2 | **AI 合同审查与 redline 建议** | **可信度：中等偏低，仅作第一遍筛查。** 用来「把 200 页里可能有问题的 12 处标出来给人看」是站得住的；用来「直接接受它的改条建议」不行 | ① 同一条款重复输入会给出不同判断——基准研究测到同一模型在相同输入上的自洽性只有约 0.81（Jaccard 相似度），在措辞相同的条款上有约 14.7% 的判断变动；② **漏检高危风险**：有基准报告主流通用模型漏掉约 18.2% 的高严重度风险；③ 检索增强（RAG）并不能消灭幻觉——斯坦福的实证研究显示，专门面向法律的检索增强产品仍有可观比例的幻觉输出；④ 通用模型在法律语料上的表现明显弱于领域训练模型 | 厂商侧的证据是**自建基准**（例如一家法律 AI 厂商公布的合同理解基准，四千多个数据点，自报与人类专家对比）——**这是厂商自报，无第三方审计，且基准由被测方设计**。独立学术侧的结论一致更保守。两边的差距本身就是本条的核心信息 | evidence: [T02-S042, T02-S043, T02-S044, T02-S046] |
| 3 | **自动化采购议价 agent 的规模化落地** | **可信度：部署是真的，收益数字不是。** 大型零售与航运企业确有千级供应商规模的部署，这一点有高校案例研究可交叉；具体百分比全部来自部署方与厂商 | ① 只适用于**参数化**的谈判（价格档、账期、返点、量），一旦需要重新定义交易结构就失效；② 长尾供应商未必有议价意愿，达成率高不代表价值高——同意一个本来就该同意的条件不产生收益；③ 供应链关系的长期影响没有任何公开数据 | **矛盾必须保留**：达成率在不同公开材料里是 64% / 68% / 72% 三个数字，取决于分母怎么算；平均收益「约 3%」与账期延长「约 35 天」没有对照组，无法区分「agent 谈出来的」和「同期市场条件本来就在变」。**全部为厂商与客户自报，无第三方审计** | evidence: [T02-S025, T02-S026, T02-S087] |
| 4 | **AI 生成让步信、还价邮件与谈判文书** | **可信度：中等，且用途要限死在「润色」。** 把你已经想清楚的立场写得更清楚、更得体、更短，它做得很好。让它替你想让步的**内容**，它会给你一堆听起来专业但没有依据的理由 | ① 生成的让步理由往往是**编造的外部约束**（「由于供应链成本上升」），如果对方追问细节，你手上没有支撑材料，这是当场失信的典型场景；② 语气过于圆滑，在需要传递「这是我的底线」的场合会削弱信号；③ 生成的书面确认函最容易在「有没有约束力」这一句上出错，而这一句的法律后果最大 | 没有任何独立研究测量过「AI 写的让步信是否拿到更好条款」。厂商与咨询侧的公开文章同样只谈效率与「不要丢掉什么」，不给结果数据；效率与谈判结果之间没有被验证的因果链 | evidence: [T02-S043, T02-S082, T02-S083, T02-S085] |
| 5 | **把 AI 写进正式谈判课程的高校做法** | **可信度：高——这是可核实的事实，不是宣称。** 顶尖商学院已经把 AI 对手模拟写进在售的正式课程页面 | 目前公开材料只说「课程包含 AI 互动模拟」，**没有公开供应商、没有公开教学效果评估、没有对照组**。「学校用了」不等于「有效」——它首先是一个课程差异化信号 | 课程页是校方一手（不是厂商宣称），所以「存在」这件事可信；「有效」这件事无证据。这是本层里唯一一条**事实可信、效果不可信**的条目，值得作为判断其他四条的参照系 | evidence: [T02-S076, T02-S077] |

**新兴层的整体判断**：这五项里，只有第 5 项的「存在」是硬事实。其余四项的共同结构是——**能力宣称在上升，独立验证没跟上**。
一个可操作的判据：**凡是宣称能改善「谈判结果」的 AI 工具，问它有没有对照组；凡是宣称能改善「谈判效率」的，直接试用两周看你自己的感受**。前者目前一个都拿不出对照组。

## 避坑清单

外行在这一行选错工具，几乎总是同一个根因：**把「管理谈判的系统」当成「做好谈判的能力」**。前者是流程，后者是准备。

1. **把 CRM / CPQ 当谈判工具。** CPQ 做的是按折扣幅度自动路由审批，CRM 做的是记录客户与商机。它们执行你已经定好的定价政策，不会让任何一次让步更聪明。政策错了，CPQ 只是把错误执行得更快更一致。判断法：**问这个系统有没有帮你想清楚「对方的优先级是什么」——没有，它就不是谈判工具。** (evidence: [T02-S040, T02-S041])
2. **买了条款库却没人维护。** 条款库的价值来自「这条语言是最新的、真的被批准过的」。一旦法务改了标准条款而库里没同步，销售拿着过期的 fallback 去谈，比没有库更糟——因为所有人都以为它是对的。上线前先定三件事：**谁负责更新、多久审一次、旧版本怎么下线**。Ironclad 官方文档还提示 playbook 数量超过 30 本后性能开始下降，说明这类系统本身也不适合无限膨胀。 (evidence: [T02-S022, T02-S023, T02-S024, T02-S039]) 
3. **用 AI 生成话术代替准备。** 准备的产出是**议题矩阵、保留价和打分表里的数字**，这些数字只能从你自己的调研里来，模型不知道你的成本结构、也不知道对方的替代方案。AI 能把你想清楚的东西写漂亮，不能替你想。已知的具体失败：它倾向于编造外部约束当让步理由，一旦对方追问细节你就当场失信。 (evidence: [T02-S043, T02-S048])
4. **迷信微表情 / 测谎 / 「读心术」类产品——这一类必须直接归入伪科学风险。** 实证证据是清楚的：跨越两万五千次以上真伪判断的元分析显示，人的测谎平均正确率约 54%，接近抛硬币；被普遍认为该擅长测谎的职业（警察调查员、精神科医生、面试官）成绩没有超过普通人。针对微表情识别训练工具（METT）的独立检验也**没有**发现它提升测谎表现。任何以「三秒看穿谎言」「微表情识别」为卖点的课程或软件，都应按虚假宣称处理。**它的实际危害不只是浪费钱，而是让人产生对自己判断力的错误信心，从而跳过真正有效的准备工作。** 同一类别里还应包括「表演愤怒施压」这类情绪战术的培训——实验综述显示它经常反噬。 (evidence: [T02-S049, T02-S050, T02-S080, T02-S086])
5. **用录音取证却踩了法域红线。** 中国大陆的排除标准是「严重侵害他人合法权益 / 违反法律禁止性规定 / 严重违背公序良俗」三条红线，涉及私密空间、私密活动、他人隐私或商业秘密的录制风险显著上升；美国有十余个州要求全体同意且部分州对通话与面谈规则不同；欧盟下同意在雇佣关系中通常不被认为是有效的合法性基础。**安全默认：开场就说「我这边会做记录，方便会后确认」。** (evidence: [T02-S029, T02-S081])
6. **把电子签平台当条款库买。** 电子签解决的是「签得成不成立」（可靠电子签名四要件、与手写签名同等效力），条款库解决的是「条款会不会失控」。两者的采购预算、维护责任人和成功标准完全不同。 (evidence: [T02-S028, T02-S035, T02-S036])
7. **在没有竞争的品类上跑反向拍卖。** 政府审计的结论是：竞标者过少（相当比例的联邦反向拍卖最后只有一个报价者）或标的是复杂服务时，节约效果消失甚至转负，还会损伤长期供应关系。**上拍之前先数一遍这个品类真实有几家能供，少于三家就不要用。** 另外，采购从业者的行业道德准则对「拿假报价压价」这类做法有明确约束，跑拍卖前值得对一遍。 (evidence: [T02-S015, T02-S016, T02-S084])
8. **逐个议题依次谈。** 这是纸笔层面最贵的错误：一次只谈一个议题，会把全部跨议题交换的空间杀死，把一场本可以双赢的谈判压成零和的价格战。多议题必须**同时**摆上桌。但也别走到另一个极端——议题堆得过多同样会降低协议质量。 (evidence: [T02-S060, T02-S061, T02-S062])
9. **把 target 和保留价混成一个数。** 保留价是「低于此就走」，target 是「我要争取的」。合成一个数的直接后果：你会把 target 当底线守，谈崩本可以成交的交易；或者把保留价当目标追，白送掉全部剩余价值。实验证据还显示，**入场前先定死 target 是抵御对方递减让步战术的唯一有效手段**。 (evidence: [T02-S052, T02-S053, T02-S058])
10. **相信厂商公布的成效百分比。** 本 track 收集到的所有 AI 议价与自动化寻源的收益数字（3% 收益、35 天账期、64%/68%/72% 达成率、90% 工作量削减、25% 成本削减）**全部是厂商或其客户自报，没有一个有第三方审计或对照组**。且同一件事在不同材料里的数字互相矛盾。看到百分比先问两句：**分母是什么？有没有对照组？** (evidence: [T02-S021, T02-S025, T02-S026])
11. **用比价站和分析师榜单选工具。** 这类站点的排序由付费与搜索优化决定。要对比就读厂商官方文档（知道产品边界）加独立学术或监管材料（知道效果上限），两边的差距本身就是你要的信息。

## 选型决策树

一句话判据：**这场谈判赢在信息、赢在替代方案、还是赢在流程设计？** 三条分叉对应三套完全不同的工具。

```
起点：这场谈判的胜负手在哪？
│
├─ 【分叉 A】赢在信息 —— 我不知道对方要什么、也不知道市场价在哪
│   │
│   ├─ A1. 不知道「对方要什么」（多议题、结构可变）
│   │      → 必备层 #1 议题矩阵 + #3 议题打分表 + #5 MESO
│   │        MESO 是这条分叉的主力：不靠提问，用对方挑哪个包来读出他的优先级
│   │      → 不要上：任何软件。这一步的产出是几个数字，软件不产出数字
│   │        evidence: [T02-S003, T02-S006, T02-S055, T02-S056]
│   │
│   ├─ A2. 不知道「市场价在哪」——薪酬场景
│   │      → 先查法定披露（欧盟指令 / 纽约州等法域要求雇主给区间），这是唯一「对方必须给你」的数据
│   │      → 再叠官方统计（劳工统计局职业工资）打底
│   │      → 商业调研与自报数据（Mercer / Radford / Levels.fyi）只当锚点，不当引用依据（选择性偏差 + 不可核验）
│   │        evidence: [T02-S027, T02-S045, T02-S047, T02-S067]
│   │
│   └─ A3. 不知道「市场价在哪」——采购场景
│          → should-cost（自下而上的工程成本测算）> 横向比价
│            联邦采购法规把成本分析与价格分析分成两件事，前者才有说服力
│          → 长约要绑公开指数（PPI / PMI Prices Index / 国家统计局），不要绑任何一方的自报成本
│            evidence: [T02-S012, T02-S013, T02-S066, T02-S068, T02-S069]
│
├─ 【分叉 B】赢在替代方案 —— 谁更耗得起，谁就赢
│   │
│   ├─ B1. 我的替代方案不清楚
│   │      → 必备层 #2 BATNA / 保留价估算表，四步走完，把 BATNA 折算成桌面上的一个数
│   │      → 常见错误：把「希望的价格」当保留价；只估自己不估对方；当成静态数字
│   │        evidence: [T02-S053, T02-S054]
│   │
│   ├─ B2. 我的替代方案是「打官司 / 仲裁」
│   │      → 去查争议解决机构的规则与收费表，这是「谈崩要花多少钱多久」的唯一可靠答案
│   │        CIETAC / SIAC-SIMC（三段式，调解 8 周内完成）/ HKIAC / 最高法一站式平台
│   │      → 这件事必须在**起草合同时**做完，谈崩之后再选机构已经晚了
│   │        evidence: [T02-S070, T02-S071, T02-S072, T02-S073, T02-S074, T02-S075]
│   │
│   └─ B3. 我想通过增加对方的成本来改善我的相对位置
│          → 采购侧：引入竞争（电子寻源 / 反向拍卖）——但先数供应商数量，少于三家不要用
│          → 不要上：任何「施压话术」类产品。位置差是靠替代方案改的，不是靠说话方式改的
│            evidence: [T02-S015, T02-S016, T02-S018, T02-S019]
│
└─ 【分叉 C】赢在流程设计 —— 我知道该谈什么，问题是量太大 / 人太多 / 守不住
    │
    ├─ C1. 同一类谈判每月几十次以上，条款失控
    │      → 条款库（standard / fallback 两级）+ playbook（决策层：何时用哪条、何时升级）
    │        Ironclad / Docusign CLM / Juro / LinkSquares / Agiloft 形态趋同，先定谁维护再选谁家
    │      → 前置条件：先有一张手写的授权表（必备层 #7）。没有授权表，条款库只是一堆文本
    │        evidence: [T02-S022, T02-S023, T02-S037, T02-S038, T02-S039]
    │
    ├─ C2. 销售折扣失控
    │      → deal desk 四件套：书面审批矩阵 + 指定负责人 + 固定请求渠道 + 承诺回复时限
    │      → CPQ 只在你已经有了上面四件套之后才有意义。反过来做必然失败
    │        evidence: [T02-S040, T02-S041]
    │
    ├─ C3. 长尾采购人力不够
    │      → 自动化寻源机器人（Keelvar 一类）跑流程；护栏参数由人预先写死
    │      → 自动化议价 agent（Pactum 一类）只在**参数化**谈判上成立（价格档 / 账期 / 返点）
    │        收益数字全部厂商自报、无对照组，按「先跑一个品类看真实数字」的方式引入
    │        evidence: [T02-S020, T02-S021, T02-S025, T02-S026]
    │
    ├─ C4. 团队水平参差，要把能力抬上来
    │      → 角色扮演模拟（PON 教学资源中心 / Kellogg DRRC 免版税练习 / iDecisionGames 在线跑）
    │      → 加必备层 #9 复盘表：模拟练流程，复盘长本事，两个都要
    │        evidence: [T02-S005, T02-S063, T02-S064, T02-S009, T02-S010]
    │
    └─ C5. 谈完之后总是「说好的不算数」
           → 必备层 #10 书面确认模板：共识点 / 分歧点 / 各自下一步与时限 / 有无约束力
           → 中国法下预约合同与善意磋商义务是真实的，「有无约束力」这一句必须写明
             evidence: [T02-S081, T02-S082, T02-S083]
```

**决策树的元规则**：三条分叉里，**A 和 B 只用纸笔层，C 才用软件层**。
如果你发现自己在给一场 A 类或 B 类谈判采购软件，说明你把准备工作的缺口误诊成了工具的缺口。

## Phase 2 提炼提示

**反复出现、跨来源一致的工具选型原则**（候选 playbook 规则）：

- **准备的产出是数字，不是文档。** 议题矩阵、保留价、打分表最终都要落成可比较的数值，否则桌上无法当场判断（出现于 T02-S003 / T02-S052 / T02-S053 / T02-S063）
- **软件管一致性，纸笔管判断力。** 条款库让一百个人给出同样的让步，不会让任何一次让步更聪明（出现于 T02-S023 / T02-S039 / T02-S041）
- **一切自动化都需要先有一张人写的授权表。** 寻源机器人的护栏、CPQ 的审批路由、条款库的 fallback 分级，本质上都是必备层第 7 项的机器可读版本（出现于 T02-S020 / T02-S039 / T02-S040）
- **看到百分比先问分母和对照组。** 本 track 收集到的全部效能数字无一有第三方审计（出现于 T02-S021 / T02-S025 / T02-S026 / T02-S046）

**显著的工具流派分裂**（候选智识谱系条目）：

- **准备派 vs 流程派**：准备派认为谈判水平由入场前填的几张表决定（PON / Kellogg 教学口径、Siedel 四步流程），流程派认为大规模商业谈判的收益来自把重复动作系统化（采购与法务侧的平台厂商）。两派不冲突但资源分配上真实竞争——预算给了条款库就不会给谈判培训
- **人谈 vs 机器谈**：自动化议价 agent 主张长尾谈判可以完全交给机器；学术侧的评测结论是模型「会建模对手但不会构造策略」。分歧点不在技术乐观程度，而在**「谈判」这个词指的是参数优化还是结构设计**

**新兴工具信号**：

- 当前新兴层条目：5 项，其中只有 1 项（高校课程含 AI 模拟）是可核实的事实，其余 4 项是「部署为真、收益存疑」
- 从出现到进主流的速度估计：AI 合同审查约 24-36 个月（已在筛查环节站住，但审查决策权仍在人手里）；自动化议价 agent 不确定，取决于是否出现第一份独立审计

**冷僻 / 信号薄弱**：

- 中文一手材料在**工具层面明显薄**：中国侧只有电子签厂商的自述和争议解决机构的官方页，**没有中文的谈判工具独立评测或学术评估**。这一节的判断绝大部分基于英文一手材料
- 美国各州录音法与欧盟录音合法性两条，**本轮未能取得一手来源逐条确认**，已在正文中显式标为「需自查项」，Phase 2 请勿把它们当作已核实事实使用
- 必备层十项全部来自教学机构口径（PON / Kellogg / Michigan），**缺少「从业者实际使用率」的调查数据**——没有找到任何一份可信的「多少比例的谈判者真的填了准备表」的统计。「≥80% 认真谈判的人都会用到」是从教学口径与课程覆盖面推断的，不是实测。若 Phase 2 需要更硬的支撑，PON 的谈判实验数据仓库是目前唯一能拿到原始实验数据的公开入口 (evidence: [T02-S088])

---

**统计**：必备层 10 项 · 场景特化层 11 项 · 新兴/实验层 5 项 · Source Manifest 88 条
