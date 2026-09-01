# Track 04 — 知识正典 / Canon

**主题**：供应链与生产运营（Supply Chain & Production Operations）——制造业与消费品的实体供应链「计划-制造-交付」判断
**受众 locale**：zh-CN（正文中文，书名/人名/术语/URL 保留原文）
**调研日期**：2026-09-02
**版权声明**：本文件只做结构化摘要与极短引用（单句以内），不含任何整章、长段原文或完整目录。

---

## 0. 这个领域的正典长什么样

供应链与生产运营是少数「实务先于理论」的学科。它的正典有三条明显不同的血脉，彼此并不友好：

1. **丰田血脉（日本，1950s-1988）**——大野耐一、新乡重夫。写法是车间笔记 + 哲学格言，几乎没有公式。它立的规矩是：**库存是罪，不是资产**；问题要当场暴露、当场停线。
2. **以色列-管理咨询血脉（1984-）**——Goldratt 的约束理论 TOC。写法是小说和苏格拉底式对话。它立的规矩是：**系统的产出由唯一的瓶颈决定，非瓶颈上的任何局部改善都是幻觉**。
3. **北美学院血脉（1990s-）**——Hopp & Spearman 的《Factory Physics》、MIT/Stanford 的供应链论文流（Lee、Fisher、Graves）。写法是排队论、随机过程、报童模型。它立的规矩是：**变异（variability）是一切交期与库存的根因，前两派都只是特定参数下的特解**。

一个从业者被认为「读过书」的最低门槛，大致是：读过《The Goal》、知道七大浪费、能画一张价值流图、听得懂牛鞭效应。要被认为「专业」，还得能算安全库存、能读 VUT 公式、知道 S&OP 每月开几次会。

---

## A. 必读正典（书）

判定标准：本条书目被至少 3 个彼此独立的来源（创立者机构站 / 学术站 / 认证机构 / 出版社官方页 / 独立媒体）引用为该领域基础读物。下面每条都给出**它到底立了什么规矩**和**它的局限**。

---

### A1.《The Goal: A Process of Ongoing Improvement》（中译《目标：简单而有效的常识管理》）
- **作者/年份**：Eliyahu M. Goldratt & Jeff Cox，1984（North River Press；后有 1992、2004、2014 多个修订版）
- **立了什么规矩**：把工厂的「目标」重新定义为**赚钱**，并给出三个可测指标——有效产出 throughput（系统通过销售产生现金的速率）、库存 inventory（系统投在待售物上的钱）、运营费用 operating expense（把库存变成有效产出所花的钱）。据此推出「聚焦五步骤」（识别约束 → 挖尽约束 → 其他一切迁就约束 → 提升约束 → 回到第一步，防止惰性）。它最反直觉的一句话是：**非瓶颈资源的利用率不是效率，是浪费**。
- **为什么是正典**：它是极少数以小说形式流行的管理书，进入了 MBA 与工厂主管培训的默认书单；TOCICO（Goldratt 本人参与创立的国际认证组织）以它为知识体系起点。
- **局限 / 被批评之处**：
  - 小说体让论证无法被检验——书里的收益是虚构的，没有对照组。
  - TOC 的学术文献长期以案例研究为主，缺少大样本随机对照的证据；已有的综述文章多承认「实证基础薄弱、发表偏差明显」。
  - 「瓶颈是固定的」这个隐含假设在多品种小批量、产品组合频繁变动的工厂里经常不成立——瓶颈会漂移，鼓-缓冲-绳（DBR）排程就会崩。
  - Goldratt 本人对精益/JIT 的态度是竞争性的，导致 TOC 社群与精益社群长期互不引用（详见 F 节）。
- 来源：T04-S001 T04-S002 T04-S003

### A2.《トヨタ生産方式——脱規模の経営をめざして》/《Toyota Production System: Beyond Large-Scale Production》（中译《丰田生产方式》）
- **作者/年份**：大野耐一（Taiichi Ohno），日文原版 1978（ダイヤモンド社），英译 1988（Productivity Press，译本推手 Norman Bodek）
- **立了什么规矩**：TPS 两根支柱——**Just-in-Time**（只在需要的时候、按需要的量、生产需要的东西）与**自働化 jidoka**（带人字旁的自动化：机器发现异常自己停）。提出**七大浪费 muda**：过量生产、等待、搬运、加工本身、库存、动作、不良品；其中「过量生产」被点名为万恶之源。提出**五问法（5 whys）**追根因，以及「超市」比喻催生看板 kanban。
- **为什么是正典**：它是原始文献，不是二手解读；后来所有精益书（Womack、Liker、Rother）都在解释它。
- **局限 / 被批评之处**：
  - 写法是格言体与回忆录，没有可复制的实施步骤——这正是后来《Learning to See》《Toyota Kata》要补的洞。
  - 大量隐含前提是丰田当时的环境：需求相对稳定、供应商地理集中在爱知县、终身雇佣制下工人不怕改善掉自己的岗位。这些条件在多数企业不成立，直接照搬会失败。
  - 劳动社会学一支长期批评 TPS 是「以压力管理」（management by stress）——库存降低意味着缓冲消失，异常直接转化为工人身上的强度。这条批评在英文文献里从 1988 年 Parker & Slaughter 一路延续到今天关于「精益的阴暗面」的研究。
- 来源：T04-S004 T04-S005 T04-S006

### A3.《The Machine That Changed the World》（中译《改变世界的机器》）
- **作者/年份**：James P. Womack, Daniel T. Jones, Daniel Roos，1990（Rawson Associates / Free Press；2007 有增补版）。基于 MIT 的 International Motor Vehicle Program（IMVP）历时五年、约 500 万美元的全球汽车装配厂对标研究。
- **立了什么规矩**：**造出了「lean production 精益生产」这个词**，并用跨厂对标数据把「日本工厂效率高」从传闻变成可比数字（每车装配工时、每百车缺陷数、库存周转、新车开发工时）。它的论点是：精益不是日本文化特产，是一套可迁移的生产组织方式，且会从汽车业扩散到一切价值创造活动。
- **局限 / 被批评之处**：
  - **数据与方法学争议**：装配厂生产率对标依赖大量标准化调整（车型复杂度、垂直整合度、自动化程度、什么算「装配」），不同调整假设会显著改变结论；后续研究者对「日本厂 2 倍效率」这个标志性数字的可比性提出过质疑。
  - **浪漫化丰田**：书把丰田写成理想型，弱化了供应商压价、班组长强度、临时工用工等成本转移；也没有预见丰田自己在 2009-2010 大规模召回中暴露的质量与规模扩张问题。
  - **叙事的宿命论**：「精益必将取代大批量生产」的预言被后来的现实部分证伪——很多行业出现的是精益与大规模定制、模块化外包的混合体，而不是全面精益化。
  - 25 周年回顾类的学术文章普遍承认：这本书成功地传播了词汇，但也让「lean」被简化成裁员和降库存的代名词，与 TPS 原意脱节。
- 来源：T04-S007 T04-S008 T04-S009

### A4.《Lean Thinking: Banish Waste and Create Wealth in Your Corporation》（中译《精益思想》）
- **作者/年份**：James P. Womack & Daniel T. Jones，1996（Simon & Schuster；2003 修订版）
- **立了什么规矩**：把 TPS 抽象成**精益五原则**——定义价值（由终端客户定义）、识别价值流、让价值流动（flow）、由客户拉动（pull）、追求尽善尽美（perfection）。这是把丰田车间实践搬出汽车业、搬进任何行业的翻译层。
- **局限**：五原则是方向而非方法，落地时极容易退化成「办工具活动」（挂看板、贴 5S 标签）而不改变排程与考核逻辑；作者本人后来在 LEI 的文章里反复承认「工具式精益」是最大的失败模式。
- 来源：T04-S010 T04-S011

### A5.《The Toyota Way》（中译《丰田模式》）
- **作者/年份**：Jeffrey K. Liker，2004（McGraw-Hill）；**第二版 2020**（14 原则更新，加入丰田自己 2001 年《The Toyota Way》内部文件之后的演化与召回危机反思）
- **立了什么规矩**：14 条管理原则，分成 4P——Philosophy（长期思维）、Process（正确的流程产生正确的结果）、People/Partners（培养人与伙伴）、Problem Solving（持续解决根本问题驱动组织学习）。它把「精益是文化不是工具箱」这一点写成了可讲授的形式。
- **局限**：14 条原则的可证伪性低——几乎任何成功都能被归因到其中某条；且此书对丰田内部冲突、供应商谈判的强硬面着墨很少，仍属同情性叙述。
- 来源：T04-S012 T04-S013

### A6.《Factory Physics: Foundations of Manufacturing Management》
- **作者/年份**：Wallace J. Hopp & Mark L. Spearman，1996 初版；**第 3 版 2008（Waveland Press，长期重印）**；两位作者后续以《Factory Physics for Managers》(2014) 面向非工程读者
- **立了什么规矩**：把工厂当作**排队网络**来分析，用数学而不是口号解释精益为什么有效。核心工具：
  - **Little's Law**：WIP = 吞吐率 × 周期时间。三者只能定两个。
  - **VUT 公式**（源自 Kingman 近似）：等待时间 ≈ V（变异因子）× U（利用率因子）× T（有效加工时间）。利用率趋近 1 时排队时间发散——**这解释了为什么「机台利用率 95%」是灾难而不是成就**。
  - **最佳情况 / 最差情况 / 实际情况**性能曲线，以及 CONWIP（恒定在制品）作为 kanban 的泛化。
- **为什么是正典**：这是把精益/TOC 从信仰变成可计算的桥；工程院校运营管理课的标准教材之一，也是 Project Production Institute 等工程社群的理论底座。
- **局限**：数学门槛高，对没有随机过程基础的计划员不友好；模型假设（稳态、独立同分布的到达与服务）在需求剧烈非平稳、产品生命周期短的场景（快时尚、消费电子新品）会失真；书对组织行为、供应商关系几乎不谈。
- 来源：T04-S014 T04-S015 T04-S016

### A7.《Learning to See: Value-Stream Mapping to Add Value and Eliminate Muda》（中译《学习观察》）
- **作者/年份**：Mike Rother & John Shook，1998/1999（Lean Enterprise Institute 出版，LEI 的第一个「工具箱」项目）。1999 年 Shingo Research Award。
- **立了什么规矩**：**价值流图 VSM** 的标准画法——从客户订单倒推，把物流与信息流画在同一张纸上，标注每道工序的周期时间 C/T、换型时间 C/O、可动率、在制品、增值时间与总前置时间比。方法是「先画现状图，再画未来状态图，再排改善计划」。用一个虚构的 Acme Stamping 案例贯穿。
- **局限**：VSM 假设产品族清晰、路由相对稳定；在高混合低批量（HMLV）、共享设备、工程订制（ETO）环境里，一张图画不完，容易变成挂在墙上的装饰。LEI 自己的文章也承认 VSM 被大量误用为「一次性活动」而非持续管理机制。
- 来源：T04-S017 T04-S018 T04-S097 T04-S098

### A8.《Toyota Kata: Managing People for Improvement, Adaptiveness and Superior Results》（中译《丰田套路》）
- **作者/年份**：Mike Rother，2009（McGraw-Hill）；后续有《The Toyota Kata Practice Guide》(2017)
- **立了什么规矩**：指出前面所有精益书的共同盲点——它们描述的是**丰田的当前状态（工具与解法）**，而不是**丰田如何持续产生这些解法的行为习惯**。提出两个套路：**改善套路（Improvement Kata）**（把握方向 → 理解现状 → 设定下一个目标状态 → 用 PDCA 快速实验逼近）和**教练套路（Coaching Kata）**（管理者用五个固定问题带教）。
- **局限**：把「科学思维」制度化为固定问答，容易变成仪式；对领导层耐心的要求极高，短周期考核的组织通常撑不到见效。
- 来源：T04-S019 T04-S020

### A9.《Out of the Crisis》（中译《转危为安》）
- **作者/年份**：W. Edwards Deming，1982/1986（MIT CAES；2018 MIT Press 重印版）
- **立了什么规矩**：**变异是管理的对象，不是员工的过错**。区分**普通原因变异（common cause，系统固有）与特殊原因变异（special cause，可指认的外部扰动）**——把普通原因当特殊原因去追责，就是「干预（tampering）」，会让系统更不稳；提出管理十四要点（含「停止依赖大批量检验来保证质量」「停止只按价格选供应商」「破除部门壁垒」「取消对工人的数字定额」）与「七种致命恶疾」。Deming 在日本的讲座是 TPS 与日本质量运动的共同前史。
- **局限**：文风严厉、结构松散，读起来更像布道；十四要点里对绩效考核与目标管理（MBO）的全盘否定在现代实证管理研究里存在争议；书中统计工具（控制图）需要另配教材才能上手。
- 来源：T04-S021 T04-S022

### A10.《The Resilient Enterprise: Overcoming Vulnerability for Competitive Advantage》
- **作者/年份**：Yossi Sheffi，2005（MIT Press）
- **立了什么规矩**：把**中断（disruption）**当作可以事先设计的对象。核心是「脆弱性 = 中断概率 × 后果严重度」的分类图，以及「**灾前做的准备比灾中的反应更决定生死**」这一判断。工具包括：标准化与模块化设计换取零件互换、双源/多源采购、与供应商建立可动员的深度关系、把柔性（flexibility）而不是冗余（redundancy）当作首选投资。经典案例：2000 年 Philips 阿尔伯克基工厂火灾中 Nokia 与 Ericsson 的分野；Aisin Seiki 火灾后丰田供应链网络的自组织恢复。
- **局限**：2005 年成书，早于中美贸易摩擦、疫情、红海航运危机与出口管制时代；对地缘政治、单点国别依赖（如先进制程、稀土、特定原料药）几乎没有框架。Sheffi 后续多本书（含疫情期著作）才补上。案例叙事强、可量化的决策规则少。
- 来源：T04-S023 T04-S024

### A11.《Demand Driven Material Requirements Planning (DDMRP)》
- **作者/年份**：Carol Ptak & Chad Smith，Version 2 (2016)、**Version 3 (2019, Industrial Press)**；配套《Orlicky's Material Requirements Planning, 3rd ed.》(2011) 与 Demand Driven Institute 的认证体系（CDDP / DDPP / DDLP）
- **立了什么规矩**：主张传统 MRP 的名义前置期与依赖需求推算在高变异环境里放大牛鞭效应，改为在**战略解耦点（strategic decoupling points）**放置**库存缓冲**，缓冲分红黄绿三区，用**净流量（net flow position = 在手 + 在途 − 合格需求）**触发补货，并按 ADU（平均日用量）与解耦前置期动态调整缓冲高度。目标是「压缩前置期、抑制紧张（nervousness）」。
- **局限 / 被批评之处（这是本领域最活跃的争议之一）**：
  - **实证基础薄弱**：系统性文献综述普遍指出严肃的学术验证很少，多数「证据」是实施方自述的案例。
  - **基线不公平**：批评者（包括 Lokad 的 Joannes Vermorel 等）指出 DDMRP 常拿「最朴素的 MRP」作对照，而不是拿现代随机优化或概率预测方法作对照，因此「优于 MRP」这个结论没有说服力。
  - **新颖性存疑**：一部分分析认为 DDMRP 本质是「再包装的精益 + 解耦点 + 老式再订货点」，理论增量有限。
  - **形式化不足**：红黄绿分区与经验系数缺乏从损失函数出发的推导，难以做经济性优化。
  - 但它在实务圈（尤其欧洲制造业与 ERP 生态）确实有真实采用率，作为「能被计划员看懂的抗变异方法」有工程价值。写进正典是因为它是当下 MRP 争论的焦点，不是因为它已被证明。
- 来源：T04-S025 T04-S026 T04-S027

### A12.《Orlicky's Material Requirements Planning》
- **作者/年份**：Joseph Orlicky 原著 1975；第 2 版 George Plossl（1994）；**第 3 版 Ptak & Smith（2011, McGraw-Hill）**
- **立了什么规矩**：MRP 的原始逻辑——**独立需求（成品，靠预测）与相关需求（零部件，靠 BOM 展开计算）必须分开处理**；用主生产计划 MPS + 多级 BOM + 提前期偏置 + 批量规则，逐级算出物料需求计划。这是几乎所有 ERP 的计算内核。
- **局限**：假设前置期固定、能力无限（MRP I 不做产能校验，这才有了后来的 MRP II / CRP）、批量规则静态；对预测误差极度敏感，是牛鞭效应在企业内部的放大器。第 3 版由 DDMRP 作者接手改写，本身在学界有「原典被派系接管」的争议。
- 来源：T04-S028 T04-S029

### A13.《Supply Chain Management: Strategy, Planning, and Operation》
- **作者/年份**：Sunil Chopra & Peter Meindl，1st ed. 2001；**7th ed. (2019) / Global Edition，近年由 Chopra 单独署名维护**（Pearson）
- **立了什么规矩**：英语世界供应链课程最通用的教科书。核心框架是**效率-响应性谱系（efficiency-responsiveness spectrum）**与**战略匹配（strategic fit）**：需求不确定性越高，供应链就该越靠响应端。六个驱动因素——设施（facilities）、库存（inventory）、运输（transportation）、信息（information）、采购（sourcing）、定价（pricing）。定量部分覆盖预测、聚合计划、安全库存与服务水平、网络设计（含选址整数规划）、收益管理。
- **局限**：教科书体例，观点温和不锋利；案例更新慢，对中国-东南亚制造网络、跨境电商履约、关税与合规的处理很薄；定价高、版本迭代频繁（被批评为「教科书通胀」）。
- 来源：T04-S030 T04-S031

### A14.《A Study of the Toyota Production System: From an Industrial Engineering Viewpoint》
- **作者/年份**：新乡重夫（Shigeo Shingo），日文 1980s，英译修订版 1989（Productivity Press）。另有《Zero Quality Control: Source Inspection and the Poka-Yoke System》《A Revolution in Manufacturing: The SMED System》(1985)
- **立了什么规矩**：从工业工程角度把 TPS 拆解为**工序（process）与作业（operation）两张网**；创立 **SMED（Single-Minute Exchange of Die，个位分钟换模）**，把换型分成内部作业（必须停机做）与外部作业（可在机器运转时做），先转换后精简——这是「小批量在经济上可行」的技术前提；创立 **poka-yoke 防错**与「源头检验」，主张用 100% 源头检查取代抽样统计检验来实现零缺陷。
- **局限**：新乡与丰田内部对「谁发明了什么」存在长期归属争议（大野系与新乡系的叙述不一致）；他对统计质量控制（SQC）的贬低被质量工程界认为过头——防错与统计方法是互补而非替代；文本翻译生硬，可读性差。
- 来源：T04-S032 T04-S033

### A15.《Critical Chain》
- **作者/年份**：Eliyahu M. Goldratt，1997（North River Press）
- **立了什么规矩**：把 TOC 搬到项目管理。诊断：每个任务估时里都藏着个人安全余量，但这些余量被**学生综合症（拖到最后才开始）**、**帕金森定律（工作填满可用时间）**与多任务切换吃掉，所以任务级的余量保护不了项目。处方：把任务估时砍到 50% 概率水平，把省下的时间集中成**项目缓冲**放在关键链末端，另设**汇入缓冲**保护接入关键链的支链，用**缓冲消耗率**而不是「里程碑是否按时」来管控项目。
- **局限**：50% 估时在合同/外包环境里难以推行（会被当成承诺）；缓冲大小的设定（常见「砍半的一半」）缺乏理论依据；与挣值管理（EVM）、敏捷的关系长期没理清；实证同样以案例为主。
- 来源：T04-S034 T04-S035

---

## B. 必读论文 / 长文

### B1. Spear & Bowen,《Decoding the DNA of the Toyota Production System》
- **出处**：Harvard Business Review, Sept-Oct 1999（Steven J. Spear, MIT Sloan；H. Kent Bowen, HBS）。基于对 40 余家工厂、四年的实地研究。
- **它立了什么规矩**：TPS 的可迁移内核不是看板或安灯，而是**四条使用规则（Rules-in-Use）**：(1) 所有作业在内容、顺序、时间、结果四个维度上被高度规定；(2) 每一组客户-供应者连接必须是直接的、二元的、有明确的是/否请求与应答；(3) 每个产品与服务的流动路径必须简单直接、预先指定；(4) 任何改善必须在指导下、按科学方法、在尽可能低的组织层级上进行。四条规则共同把工厂变成一个**持续做实验的社区**——每次异常都是一次假设被证伪。
- **最反直觉的判断**：**正是操作上的刚性（rigidity）造就了柔性（flexibility）**——因为只有把标准写死，偏差才可见。
- **局限**：规则一的「高度规定」在知识工作、工程订制场景难以照搬；文章没有讨论工人对被高度规定的抵触，也没有对照组。
- 来源：T04-S036 T04-S037

### B2. Lee, Padmanabhan & Whang,《The Bullwhip Effect in Supply Chains》
- **出处**：*Sloan Management Review* 38(3), Spring 1997, pp.93-102。姊妹学术版《Information Distortion in a Supply Chain: The Bullwhip Effect》发表于 *Management Science* 43(4), 1997, pp.546-558（DOI 10.1287/mnsc.43.4.546）；2004 年 *Management Science* 把它选入「最有影响力论文」重刊，三位作者另写了一篇十年回顾《Comments on "Information Distortion in a Supply Chain: The Bullwhip Effect"》，*Management Science* 50(12), 2004, pp.1887-1893（DOI 10.1287/mnsc.1040.0305）——**回顾文本身值得单独读**，作者在其中承认了模型假设的边界并回应了早期批评。
- **它立了什么规矩**：需求波动沿供应链向上游逐级放大，**不是因为人蠢，而是因为局部理性决策的必然结果**。四个成因：
  1. **需求预测更新**（每级都基于上游订单而非终端消费重新预测并加安全库存）
  2. **订单批量化**（凑整车、凑月度处理成本）
  3. **价格波动**（促销与折扣导致提前囤货 forward buying，购买模式与消费模式脱钩）
  4. **配给与短缺博弈**（缺货时超额下单抢配额，供应恢复后集中砍单）
- **对策**：共享 POS 数据、供应商管理库存 VMI、CPFR、每日低价 EDLP 取代促销、按历史销量而非当期订单配货。
- **局限 / 后续**：牛鞭是否普遍存在有实证争议——用行业数据做的复现研究发现制造业层面的放大效应弱于理论预期（存在「牛鞭在零售端明显、在上游被产能平滑」的现象）；此外四因之外还有前置期、批量政策与信息延迟的交互项，后续文献（Chen 等的量化模型、Cachon 等的实证）做了大量修正。
- 来源：T04-S038 T04-S039 T04-S040 T04-S086

### B3. Fisher,《What Is the Right Supply Chain for Your Product?》
- **出处**：Harvard Business Review, March-April 1997（Marshall L. Fisher, Wharton）。基于十余年跨行业（食品、时装、服装、汽车）研究。
- **它立了什么规矩**：先按需求模式给产品分类，再选供应链——**功能型产品（functional：需求可预测、生命周期长、毛利低，如日用杂货）配物理效率型供应链（追求最低成本、高产能利用、库存周转）；创新型产品（innovative：需求不可预测、生命周期短、毛利高、款式多，如时装与消费电子）配市场响应型供应链（追求缓冲产能、快速反应、部署式库存）**。绝大多数供应链病症的根因是**产品类型与供应链类型的错配**——尤其是把创新型产品塞进为功能型产品设计的低成本供应链。
- **配套概念**：Fisher 与 Ananth Raman 的**准确响应（accurate response）**——先小批量试产，用早期真实销售信号更新预测，再决定主要产量（时装业「二次下单」的理论依据）。
- **局限**：二分法过于粗糙，现实中同一 SKU 在生命周期不同阶段会换类；对同时要低成本又要快反的品类（快时尚）没有答案——Zara 的做法其实是两种供应链并联，而非二选一。
- 来源：T04-S041 T04-S042

### B4. Hau Lee,《The Triple-A Supply Chain》
- **出处**：Harvard Business Review, October 2004（Hau L. Lee, Stanford GSB）。基于对 60 余家企业 15 年的观察。
- **它立了什么规矩**：**只追求快和便宜的供应链会随时间劣化**。可持续的优势需要同时具备三个 A：
  - **Agility 敏捷**：对短期需求/供应变化快速反应（数据共享、共同规划、延迟策略、备用应急库存与物流）
  - **Adaptability 适应**：随市场结构与战略变化调整网络本身（监测经济体变化、及时迁移产地与供应基地、设计模块化产品平台）
  - **Alignment 对齐**：让所有伙伴的激励与风险收益一致（信息对等、角色与责任明确、风险与收益共担）
- **局限**：三个 A 之间存在真实取舍（对齐所需的长期合约与适应所需的换供应商自由是冲突的），文章更多是分类而非取舍法则；实证以正例为主，缺失败样本。
- 来源：T04-S043 T04-S044

### B5. Sterman,《Modeling Managerial Behavior: Misperceptions of Feedback in a Dynamic Decision Making Experiment》
- **出处**：*Management Science* 35(3), March 1989, pp.321-339（John D. Sterman, MIT Sloan）。DOI 10.1287/mnsc.35.3.321
- **它立了什么规矩**：这是**啤酒游戏（Beer Distribution Game）**的正式实验报告，也是牛鞭效应的**行为学**基础。Sterman 让被试在一个含时滞与多级反馈的模拟分销系统里下单，发现即使需求只有一次小幅阶跃，订单波动仍会剧烈放大。原因不是信息缺失，而是**对反馈的误认（misperceptions of feedback）**：人们系统性地忽略在途库存（supply line），于是对同一个缺口反复下单。他用锚定-调整（anchoring and adjustment）规则拟合被试行为，拟合优度很高。
- **为什么重要**：B2 的四个成因是结构性的（激励与流程），这篇是认知性的——**即使把四个结构成因全部消除，只要人还在回路里且看不见在途量，牛鞭依然存在**。这直接推出了「让在途可见」这条实务原则。
- **局限**：实验室被试非专业计划员；模拟环境的成本函数与真实企业不同；后续研究表明训练与信息可视化能显著减弱效应但不能消除。
- 来源：T04-S071 T04-S096

### B6. Cachon, Randall & Schmidt,《In Search of the Bullwhip Effect》
- **出处**：*Manufacturing & Service Operations Management* 9(4), 2007, pp.457-479。DOI 10.1287/msom.1060.0149
- **它立了什么规矩**：用美国行业与企业层面的实际数据去找牛鞭，结论是**牛鞭远没有理论和啤酒游戏暗示的那么普遍**——在他们检验的行业里，多数制造业行业**不表现出**订单波动大于销售波动；零售端更明显，上游反而被产能与生产平滑（production smoothing）压平了。
- **为什么必须一起读**：它是本领域少见的「用数据打自己人」的论文。任何声称「我们公司有牛鞭」的诊断，都应该先按这篇的方法算一下方差比，而不是默认存在。
- **局限**：数据聚合层级高（行业/企业而非 SKU），聚合本身会掩盖单品级的放大；季节性调整方法有争议。**结论应读作「牛鞭不是普遍规律，是特定条件下的现象」，而不是「牛鞭不存在」。**
- 来源：T04-S072

### B7. Eppen,《Effects of Centralization on Expected Costs in a Multi-Location Newsboy Problem》
- **出处**：*Management Science* 25(5), May 1979, pp.498-501。DOI 10.1287/mnsc.25.5.498
- **它立了什么规矩**：**风险池化的数学证明**。在需求独立同分布、持有与缺货成本线性的假设下，把 n 个地点的库存集中，期望成本按 **√n** 的比例下降（换句话说，n 个仓合成 1 个仓，安全库存只需原来的 1/√n）。这三页纸是**集中仓、通用零件、延迟策略、跨区域调拨**四类决策的共同理论根。
- **局限（很重要）**：结论对假设极其敏感——需求正相关时收益大幅缩水（极端正相关时归零）；**重尾需求下 √n 法则失效**（后续 Stanford 的研究显示厚尾分布中集中化收益远小于经典结果）；且该模型不计运输成本与响应时间，而集中化恰恰会拉长最后一公里。**不要把 √n 当成免费午餐去论证「关掉区域仓」。**
- 来源：T04-S073 T04-S074

### B8. Fisher & Raman,《Reducing the Cost of Demand Uncertainty Through Accurate Response to Early Sales》
- **出处**：*Operations Research* 44(1), 1996, pp.87-99（Marshall Fisher, Ananth Raman）。DOI 10.1287/opre.44.1.87
- **它立了什么规矩**：**准确响应 / 快速响应**的定量版。把一次性下单拆成**两次**：第一次只投产总量的一小部分，用最初几周的真实销售更新需求分布，第二次再决定剩余产量。文章用滑雪服制造商 Sport Obermeyer 的真实数据展示：即使产能受限、第二次下单要付溢价，两阶段决策仍能显著降低缺货与残值损失。同时给出用**买手预测的离散程度**作为需求不确定性代理变量的方法——买手们意见越分散的款，越不确定，越该留到第二次。
- **为什么重要**：它是 B3（Fisher 1997 HBR）的引擎室；也是今天所有「小单快反」「柔性供应链」话术的学术原型。
- **局限**：要求供应链有真实的二次下单产能与短补货前置期；在产能靠长约锁定、模具开发周期长的品类做不到。
- 来源：T04-S075

### B9. Lee, Billington & Carter,《Hewlett-Packard Gains Control of Inventory and Service through Design for Localization》
- **出处**：*Interfaces* 23(4), 1993, pp.1-11。DOI 10.1287/inte.23.4.1。配套的管理版是 Feitzinger & Lee,《Mass Customization at Hewlett-Packard: The Power of Postponement》, *HBR*, Jan-Feb 1997。
- **它立了什么规矩**：**延迟策略 postponement / 面向本地化的设计**。HP DeskJet 打印机原来在工厂就装好各国电源与说明书，导致每个国别版本各自备库存。改为工厂只做通用机身、把电源模块与本地化物料推迟到区域配送中心装配后，各国需求被汇集成一个通用件的需求（风险池化生效），总制造+运输+库存成本显著下降（公开报道的量级为约 25%）。
- **一句话原则**：**把差异化动作推到需求信号出现之后**——产品设计（模块化、通用平台）与供应链设计必须一起改，只改供应链做不到。
- **局限**：区域 DC 要具备装配与质检能力（成本与合规负担）；通用件本身可能更贵；对差异化在早期工序就锁定的产品（涂装、成型）不适用。
- 来源：T04-S076 T04-S077 T04-S093 T04-S094

### B10. Olhager,《Strategic Positioning of the Order Penetration Point》＋ Harfeldt-Berg & Olhager 的 CODP 系统综述
- **出处**：Jan Olhager, *International Journal of Production Economics* 85(3), 2003, pp.319-329（DOI 10.1016/S0925-5273(03)00119-1）；Harfeldt-Berg & Olhager,《The customer order decoupling point in empirical operations and supply chain management research: a systematic literature review and framework》, *International Journal of Production Research* 62(17), 2024, pp.6380-6399（DOI 10.1080/00207543.2024.2314164）。更早的源头是 Sharman (1984) 与 Hoekstra & Romme (1992)。
- **它立了什么规矩**：**客户订单解耦点 CODP（又名订单穿透点 OPP）**是供应链结构的第一决策变量。CODP **上游按预测补货（MTS 逻辑）、下游按订单履行（MTO 逻辑）**；它的位置由三类因素决定——市场（客户可接受的交期 vs 生产总前置期，即 **P/D 比**）、产品（品种数、模块化程度、BOM 形状）、生产（工艺柔性、换型成本、需求波动）。**当客户可接受交期 < 生产总前置期时，你必然要在某处持有库存——CODP 就是决定「在哪一层持有」的那个选择。**
- **为什么重要**：MTS/MTO/ATO/ETO 不是四种公司类型，是 CODP 的四个位置。多数「库存高又交不出货」的病，本质是 CODP 放错了层级（放在成品，而不是放在通用半成品/关键长周期件）。2024 年的综述把 32 个实证因素归成市场与产品、运营、供应链、绩效四类，是目前最系统的实证盘点。
- **局限**：单一 CODP 的假设在多产品族企业不成立（同一工厂会有多个解耦点）；综述本身指出实证研究在服务业与多解耦点场景仍然稀缺。
- 来源：T04-S078 T04-S079 T04-S095

### B11. Hopp & Spearman,《To Pull or Not to Pull: What Is the Question?》
- **出处**：*Manufacturing & Service Operations Management* 6(2), 2004, pp.133-148。DOI 10.1287/msom.1030.0028
- **它立了什么规矩**：这是工厂物理学派对精益话术的一次正面清算。核心论点：**「推 vs 拉」被普遍误定义**。拉动的本质**不是**「按客户需求生产」也**不是**「用看板卡片」，而是**系统对在制品设置了明确上限**（WIP cap）；推动是按外生计划投料、不设 WIP 上限。据此：MRP 是推、看板是拉、**CONWIP 也是拉且通常比看板更鲁棒**；「拉动优于推动」的真正原因是 WIP 受控带来的周期时间稳定与质量反馈快，与卡片形式无关。
- **为什么重要**：它把一场十几年的口号之争还原成一个可测量的设计参数（WIP 上限设多少），并说明**混合系统（上游推、CODP 下游拉）**通常才是最优解——这与 B10 的解耦点框架完全咬合。
- **局限**：定义之争本身对一线改善帮助有限；文章对组织与人的因素照例不谈。
- 来源：T04-S080

### B12. Holweg,《The Genealogy of Lean Production》
- **出处**：*Journal of Operations Management* 25(2), 2007, pp.420-437（Matthias Holweg）。DOI 10.1016/j.jom.2006.04.001
- **它立了什么规矩**：对《The Machine That Changed the World》叙事的**史学修正**。它追溯 IMVP 研究的实际过程，指出 **「lean」这个词并非 Womack 等人首创，而是出自 IMVP 研究员 John Krafcik 1988 年在 *Sloan Management Review* 的文章《Triumph of the Lean Production System》**；并还原了装配厂对标方法（生产率标准化）的设计与争议，以及为什么这套研究会被压缩成一个高度传播但过度简化的故事。
- **为什么必读**：它是你在被人拿「日本厂效率是美国厂两倍」这类数字说服之前，应该先读的那一篇。
- 来源：T04-S081

### B13. Mehri,《The Darker Side of Lean: An Insider's Perspective on the Realities of the Toyota Production System》
- **出处**：*Academy of Management Perspectives* 20(2), May 2006, pp.21-42（Darius Mehri，作者在日本一家丰田系供应商做过三年工程师）。DOI 10.5465/amp.2006.20591003
- **它立了什么规矩**：内部人视角的负面证据——工程设计上的路径依赖与创新受限、工时与安全问题、供应商层级中的强度转移、性别与外籍员工待遇。它是「精益的阴暗面」文献里被引用最多、也最难被忽视的一篇，因为它不是理论推演而是参与式观察。
- **怎么读**：单一个案、时间与企业特定，不能外推成「精益都这样」；但它足以证伪「TPS 是一个对所有参与者都更好的系统」这种全称命题。**读丰田正典时把这篇当解毒剂。**
- 来源：T04-S082

### B14. Azzamouri, Baptiste, Dessevre & Pellerin,《DDMRP: A Systematic Review and Classification》
- **出处**：*Journal of Industrial Engineering and Management* 14(3), 2021, pp.439-456（开放获取）。DOI 10.3926/jiem.3331
- **它立了什么规矩**：把 2011-2020 年所有 DDMRP 文献做了盘点，结论直白：文献总量小（几十篇量级），**约四成是性能分析、仅约一成提出新的建模方法**；DDMRP **尚未成熟**，其鲁棒性有待检验，多个参数（缓冲区系数、ADU 窗口、解耦点选择）目前靠经验而非推导。主要实施集中在离散制造，流程工业几乎没有证据。
- **怎么用**：这是 F4 争议中**最中立的一份材料**——既不是 Demand Driven Institute 的宣传，也不是竞品厂商的攻击。要判断 DDMRP，先读它。
- 来源：T04-S083

### B15. Dolgui, Ivanov & Simchi-Levi,《Stress Tests for Supply Chains: Towards Resilience and Viability》
- **出处**：*International Journal of Production Research* 63(9), 2025, pp.3254-3258。DOI 10.1080/00207543.2025.2483113。配套背景是 Ivanov 关于**供应链生存力（viability）**与数字孪生压力测试的一系列论文。
- **它立了什么规矩**：把金融业的**压力测试**思路正式移植到供应链——不是问「我们的韧性得分是多少」，而是问「在指定的一组冲击情景（单点断供、区域封锁、需求骤降、运力中断）下，网络还能不能维持关键产出，恢复到 X% 需要多久」。同时区分两个层级：**resilience 韧性 = 受冲击后恢复原状的能力（被动免疫）；viability 生存力 = 通过学习与结构调整长期存续的能力（主动免疫）**。
- **为什么收进来**：这是 A10（Sheffi 2005）的当代续篇，补上了 2005 年没有的东西——可执行的情景测试协议与地缘政治级冲击。欧盟联合研究中心（JRC）已有基于这条线的政策报告。
- **局限**：仍属新兴议程，标准化的压力测试协议尚未形成行业共识；对中小企业的数据要求偏高。
- 来源：T04-S084 T04-S085

---

## C. 课程 / 认证 / 知识体系

### C1. ASCM（原 APICS）三大认证
ASCM（Association for Supply Chain Management）是本领域最被雇主识别的认证机构，2019 年由 APICS 更名而来（APICS 作为其下属品牌保留）。

| 认证 | 全称 | 覆盖范围 | 谁该考 | 结构 |
|---|---|---|---|---|
| **CPIM** | Certified in Planning and Inventory Management | 企业「四面墙以内」：需求管理、MPS 主生产计划、MRP、产能计划、执行与控制、库存、S&OP、精益/质量 | 计划员、物控、生产调度、库存与需求计划、制造运营经理 | 传统为两门考试（Part 1 / Part 2）；ASCM 近年推动向单一考试路径演进，报考前须以官网当期公告为准 |
| **CSCP** | Certified Supply Chain Professional | 端到端延伸供应链：需求、全球网络、寻源采购、内部运营、供应商关系、正向与逆向物流、风险、技术、绩效改进 | 想要跨职能视角的供应链经理、采购、S&OP 主持人、咨询顾问 | 单门考试，150 题 / 3.5 小时；有报考资格门槛（学位或 3 年相关经验或持有指定证书） |
| **CLTD** | Certified in Logistics, Transportation and Distribution | 物流战略、运输、仓储与履约、订单与库存管理、全球物流与合规、可持续与逆向物流、绩效与网络优化 | 物流经理、运输采购、仓配运营、跨境履约 | 单门考试，150 题 / 3.5 小时 |

**怎么选（务实建议）**：做工厂计划、排产、库存 → CPIM；做全链路规划、S&OP、供应商管理、想转咨询 → CSCP；做仓配与运输 → CLTD。三者不互斥，行业内常见路径是 CPIM → CSCP。
来源：T04-S045 T04-S046 T04-S047 T04-S087 T04-S102

### C2. SCOR / SCOR-DS 参考模型
- **是什么**：Supply Chain Operations Reference，1996 年由 Supply Chain Council 发布，后并入 APICS/ASCM。它是供应链的**通用流程语言 + 绩效指标字典 + 对标框架**：把任何供应链拆成标准流程层级（L1 流程 → L2 流程类型 → L3 流程要素），配一套标准 KPI（可靠性 / 响应性 / 敏捷性 / 成本 / 资产管理效率，其中 Perfect Order Fulfillment、Order Fulfillment Cycle Time、Cash-to-Cash Cycle Time 最常被引用）。
- **SCOR-DS（Digital Standard）**：ASCM 称之为 1996 年以来最重大的一次改版，2022 年发布、2025 年更新至 14.0 版。变化：从线性的 Plan-Source-Make-Deliver-Return 五流程，改为包含 **Orchestrate（统筹）/ Plan / Order / Source / Transform / Fulfill / Return** 的网络化七流程；纳入可持续与 ESG 指标；开放获取（CC BY-NC-ND 授权）。配套有 SCOR-P 从业者认证。
- **怎么用**：主要用于跨企业对标、流程梳理与 KPI 定义统一，**不是**一套实施方法论——它告诉你「量什么」，不告诉你「怎么改」。
来源：T04-S048 T04-S049 T04-S050

### C3. MITx MicroMasters in Supply Chain Management（MIT CTL）
- **是什么**：MIT Center for Transportation & Logistics 在 edX / MITx Online 上开设的研究生水平在线项目，五门课 + 一场综合结课考试：
  - CTL.SC0x Supply Chain Analytics（概率统计与优化基础）
  - CTL.SC1x Supply Chain Fundamentals（预测、库存、运输、网络设计的核心数学）
  - CTL.SC2x Supply Chain Design
  - CTL.SC3x Supply Chain Dynamics（系统动力学、啤酒游戏、牛鞭）
  - CTL.SC4x Supply Chain Technology and Systems
- **为什么重要**：这是目前**公开可得、数学严谨度最高**的供应链系统课程，课程负责人 Chris Caplice 与 Eva Ponce 的讲义（Key Concepts 文档）本身就是一份高质量的公式手册。通过 MicroMasters 可申请 MIT SCM 硕士的 Blended 路径（在校学期缩短）。
- **注意**：课程可免费旁听，认证与学分需付费；开课时间按学期滚动排期。
来源：T04-S051 T04-S052 T04-S053 T04-S090

### C4. 精益体系的官方知识源
- **Lean Enterprise Institute (lean.org)**：Womack 1997 年创立，出版《Learning to See》《Lean Thinking》等「工作手册」并办 Lean Summit、教练课程。它是精益知识的原产地机构。
- **Shingo Institute（Utah State University 商学院）**：颁发 **Shingo Prize**（企业卓越奖，评的是文化与行为而非工具部署）与 **Shingo Research and Professional Publication Award**（学术/图书奖，《Learning to See》1999 年得奖）。它提供 Shingo Model 的系列研讨课（DISCOVER / ENABLE / IMPROVE / ALIGN / BUILD EXCELLENCE）。
- **六西格玛绿带/黑带**：注意这是一个**没有单一权威发证方**的领域。相对可信的第三方认证是 **ASQ（American Society for Quality）** 的 CSSGB / CSSBB / CSSYB（有工作经验与项目要求、闭卷考试）与 **IASSC** 的 lean six sigma 考试（只考知识、不要求项目）。企业内训证书与网课「黑带」在含金量上差异极大，简历上应写明发证机构。
来源：T04-S054 T04-S055 T04-S056 T04-S088 T04-S089 T04-S091 T04-S092

### C5. 中文圈系统课程（谨慎结论）
- 中国大陆的正规学位路径主要在**物流工程与管理（专业学位）/ 管理科学与工程**下，代表院校包括北京交通大学、上海海事大学、西南交通大学等；MOOC 平台（中国大学 MOOC / 学堂在线）上有院校开设的「物流与供应链管理」「生产运作管理」课程。
- ASCM 的 CPIM/CSCP 在中国大陆有授权培训机构与中文备考资料，考试本身为英文（部分科目有其他语言版本，须以官网当期为准）。
- **未验证**：坊间「供应链总监班」「精益六西格玛黑带速成」类商业培训的质量与发证效力，本次调研没有找到可核实的独立评价依据，一律标记为**未验证**，不建议在没有查清发证机构的情况下购买。
来源：T04-S057

---

## D. 核心概念清单

| # | 概念（中/英/日） | 一句话定义 | 出自 |
|---|---|---|---|
| 1 | 利特尔法则 Little's Law | 在制品 = 产出率 × 周期时间；三个量只能自由定两个 | Factory Physics（A6），源自 J.D.C. Little 1961 |
| 2 | 瓶颈 / 约束 bottleneck-constraint | 决定整个系统产出上限的那一个资源；非约束的产能富余不是浪费而是必需 | The Goal（A1） |
| 3 | 聚焦五步骤 Five Focusing Steps | 识别 → 挖尽 → 迁就 → 提升 → 回到第一步（防惰性） | The Goal（A1） |
| 4 | 有效产出 / 库存 / 运营费用（TOC 三指标） | Throughput = 通过销售产生现金的速率；Inventory = 压在待售物上的钱；OE = 把库存变成 T 花的钱 | The Goal（A1） |
| 5 | 鼓-缓冲-绳 DBR | 用瓶颈节奏当「鼓」定排程，在瓶颈前留时间「缓冲」，用「绳」把投料速度拴回瓶颈消耗速度 | TOC 体系 / Critical Chain（A15） |
| 6 | 七大浪费 muda | 过量生产、等待、搬运、加工本身、库存、动作、不良；过量生产是万恶之源 | 大野耐一（A2） |
| 7 | 不均 mura / 超负荷 muri | muda 之外的两个 M：mura 是节奏与负荷的波动，muri 是让人或设备超出合理负荷；三者互为因果 | 丰田体系 / The Toyota Way（A5） |
| 8 | 节拍时间 takt time | 可用工作时间 ÷ 客户需求数量，即「客户每隔多久要一件」；是排产的心跳而非产能上限 | Learning to See（A7）；定义见 T04-S101 |
| 9 | 平准化 heijunka | 把品种与数量在时间上摊平（混线小批量循环），用生产端的稳定去吸收需求端的波动 | 大野耐一（A2）/ Lean Thinking（A4）；定义见 T04-S099 |
| 10 | 自働化 jidoka | 「带人字旁的自动化」：设备/人一旦发现异常就自主停止，不把不良往下传 | 大野耐一（A2）；定义见 T04-S100 |
| 11 | 防错 poka-yoke | 用装置或设计让错误物理上做不出来（或立刻可见），取代靠注意力的检验 | 新乡重夫（A14） |
| 12 | SMED | 把换型作业拆成内部（必须停机）与外部（可运转中完成），先外部化再精简，目标个位分钟 | 新乡重夫（A14） |
| 13 | 看板 kanban | 用实物卡片/信号授权补货与生产的拉动机制；无卡不生产，因此在制品有硬上限 | 大野耐一（A2） |
| 14 | 安灯 andon | 一拉即亮的异常呼叫与停线信号，让问题在发生的那一秒变成组织的问题 | 大野耐一（A2）/ Spear & Bowen（B1） |
| 15 | 现地现物 genchi genbutsu | 去现场、看实物、亲自确认，再下判断；反对靠报表隔空管理 | The Toyota Way（A5） |
| 16 | 价值流 value stream | 从原料到客户手中，为某个产品族创造价值所需的全部动作（含增值与不增值） | Lean Thinking（A4）/ Learning to See（A7） |
| 17 | 单件流 one-piece flow | 让一件产品连续流过各工序而不停留成堆，暴露一切不平衡与不良 | Lean Thinking（A4） |
| 18 | 报童模型 newsvendor | 单期一次性订货下的最优订量：让服务水平等于临界比 Cu/(Cu+Co)（缺货成本 / (缺货成本+过剩成本)） | 运营管理经典 / Chopra & Meindl（A13） |
| 19 | 安全库存与服务水平 | 安全库存 ≈ z(服务水平) × 需求与前置期综合波动的标准差；服务水平提升到 99% 以上时库存成本非线性暴涨 | Chopra & Meindl（A13）/ MITx SC1x（C3） |
| 20 | EOQ 经济订货批量 | 在订货成本与持有成本之间取平衡的批量：√(2DS/H)；对参数误差不敏感（成本曲线平坦）是它真正的价值 | Harris 1913 / Orlicky's MRP（A12） |
| 21 | 牛鞭效应 bullwhip effect | 需求波动沿供应链向上游逐级放大，源于四类局部理性决策 | Lee, Padmanabhan & Whang（B2） |
| 22 | 客户订单解耦点 CODP | 供应链上「预测驱动」与「订单驱动」的分界线；它的位置决定了交付前置期与库存形态 | DDMRP（A11）/ MTS-MTO 文献 |
| 23 | 延迟策略 postponement | 把差异化动作（贴标、配置、包装、本地化）推迟到需求信号明确之后，用通用半成品汇集风险 | Lee 等延迟策略文献 / Triple-A（B4） |
| 24 | 风险池化 risk pooling | 把多个独立需求汇总，总需求的变异系数下降（集中库存的安全库存按 √n 缩减），是集中仓与通用件的理论依据 | Eppen 1979 / Chopra & Meindl（A13） |
| 25 | MTS / MTO / ATO / ETO | 按 CODP 位置分的四种交付模式：备货生产 / 订单生产 / 订单装配 / 订单设计 | APICS-ASCM 体系（C1） |
| 26 | OEE 与六大损失 | 设备综合效率 = 时间开动率 × 性能开动率 × 合格品率；六大损失 = 故障、换型调整、空转短停、速度降低、启动不良、加工不良 | TPM 体系（Nakajima） |
| 27 | 过程能力 Cp / Cpk | Cp 只看波动宽度与公差之比，Cpk 还惩罚中心偏移；Cpk 高不代表过程受控，只代表当前有余量 | 统计质量控制 / AIAG SPC 手册 |
| 28 | VUT 公式 | 排队等待 ≈ V(变异) × U(利用率) × T(有效加工时间)；利用率趋近 100% 时等待时间发散 | Factory Physics（A6），源自 Kingman 近似 |
| 29 | CONWIP | 恒定在制品：给整条线设一个 WIP 总上限，出一件才放一件，是 kanban 的泛化，对混合产品更稳健 | Factory Physics（A6） |
| 30 | 普通原因 / 特殊原因变异 | 系统固有的波动 vs 可指认的外部扰动；把前者当后者追责叫「干预」，只会让系统更差 | Out of the Crisis（A9） |
| 31 | 改善套路 / 教练套路 Kata | 目标状态 → 现状 → 障碍 → 下一步实验的固定练习循环，以及管理者带教的五问 | Toyota Kata（A8） |
| 32 | A3 报告 | 一张 A3 纸上完成背景-现状-目标-根因-对策-计划-跟进的结构化思考与共识工具 | 丰田体系 / Managing to Learn (Shook) |

---

## E. 阅读路线图：零基础 → 能上手做计划

**第 1 本《The Goal》（A1）** — 先建立「系统有瓶颈、局部效率是幻觉」这一条直觉。用小说读，两天读完，不需要任何数学。**为什么放第一**：它是唯一一本能让非工科背景的人在毫无痛苦的情况下换掉「越忙越好」这个默认心智模型的书。后面所有的排产讨论都要用到这个直觉。

**第 2 本《Learning to See》（A7）** — 立刻动手画你自己业务的一张价值流图。**为什么是第二**：读完《The Goal》你会有冲动去找瓶颈，但没有工具看见它。VSM 是最便宜的可视化工具，一支笔、一张纸、走一圈车间/仓库就能做。这一步把抽象概念钉在你自己的现场上。

**第 3 本《Lean Thinking》（A4）或《The Toyota Way》（A5）二选一** — 前者给你「怎么改」的五原则骨架，后者给你「为什么改不动」的组织答案。**为什么在这里**：你画完图会遇到第一次改善失败，这时候需要知道自己踩的是哪一类坑。选哪本取决于你的痛点是流程（选 Lean Thinking）还是人和管理层（选 The Toyota Way）。

**第 4 本《Factory Physics》（A6）或 MITx SC1x（C3）二选一** — 开始算。Little's Law、VUT、安全库存、EOQ、报童模型。**为什么必须有这一步**：前三步给的是判断力，但「要不要加一台设备」「安全库存设几天」「服务水平 95% 还是 98%」这类问题只能算，不能悟。跳过这一步的人会长期停留在讲故事阶段，做不了计划岗。如果数学基础薄弱，先上 MITx SC0x/SC1x（有讲解和作业），再回头读 Factory Physics 当参考书。

**第 5 本（可选，按岗位分叉）**：
- 做端到端计划 / S&OP → Chopra & Meindl（A13）+ Fisher HBR 1997（B3）
- 做工厂现场 → Toyota Kata（A8）+ 新乡重夫的 SMED（A14）
- 做供应链风险与网络 → Sheffi《The Resilient Enterprise》（A10）+ Hau Lee Triple-A（B4）
- 做 ERP / MRP 参数与 IT → Orlicky's MRP（A12），并把 DDMRP（A11）当**争议材料**读而不是当教科书读

**顺序的逻辑**：直觉（为什么）→ 可视化（在哪里）→ 方法（怎么改）→ 定量（改多少）→ 领域深化。反过来的顺序（先学公式）在实务中失败率很高——不是因为公式难，而是因为没有现场直觉的人算出来的参数没人信、也没人执行。

---

## F. 争议：正典之间的分歧

### F1. TOC 派 vs 精益派
- **TOC 打精益**：精益追求全线平衡（每个工位节拍相同），但在有变异的真实系统里，平衡线意味着**每个工位都是瓶颈**，任何一次扰动都会立刻传递、无处吸收。TOC 主张**故意不平衡**——留一个明确的约束，其余工位有保护性产能。TOC 还认为精益的「消灭一切浪费」缺少优先级，会把改善资源撒在非约束上，对系统产出零贡献。
- **精益打 TOC**：DBR 假设瓶颈位置稳定；产品组合一变瓶颈就漂移，排程系统立刻失效。而 kanban/CONWIP 这类拉动机制不需要知道瓶颈在哪，就能自动限制在制品——**鲁棒性更好、实施更简单**。此外精益认为 TOC 停在「管理约束」，不追求消除变异本身，是治标。
- **对同一现象的不同话术**：DBR 的缓冲是**时间**，kanban 的缓冲是**空间/数量**；TOC 的「绳」和 CONWIP 的 WIP 上限在数学上高度相似。很多实务上的争吵其实是同一件事的两种记账方式。
- **诚实的结论**：分歧的一部分是真的（是否需要事先定位瓶颈），另一部分是生意——两派各有咨询与认证生态，学界也大致分成拥 Goldratt 与忽视 Goldratt 两个阵营。**要在需求快速增长、瓶颈明确且不动的产线上做排程 → DBR 有优势；要在混乱、变异大、瓶颈会漂的产线上先稳住系统 → kanban/CONWIP 拉动更快见效。**
来源：T04-S035 T04-S058 T04-S059 T04-S080

### F2. 工厂物理学派：「你们都是特例」
Hopp & Spearman 的立场是：TPS 和 TOC 都是**在特定参数区间内正确的经验规则**，而排队论给出的是通用规律。具体的攻击点：
- **JIT/零库存**：Little's Law 说明，在给定产出率下降低 WIP 必然缩短周期时间，但 WIP 不能降到低于「关键 WIP」（= 瓶颈产能 × 原始过程时间），否则产出率必然下降。所以「零库存」是口号不是目标——正确的问题是「在多少变异下、需要多少缓冲」。
- **缓冲定律（buffering law）**：变异一定会以三种形式之一被吸收——**库存、产能、时间（交期）**。你不能三个都不给。精益宣传「消除库存又不失产能又不延长交期」，在数学上要求变异先被消除，而这一点在多数工厂做不到。
- **对 TOC**：瓶颈只在确定性系统里是清晰概念；在随机系统里「谁是瓶颈」随时间波动，所谓约束更像是一个统计上的重心。
- **反批评**：Factory Physics 学派自己的局限是把工厂当稳态排队网络，对**人、组织学习、供应商关系**几乎失语——而这恰是精益真正的护城河。用 Factory Physics 能解释丰田为什么有效，但解释不了为什么别人抄不动丰田。
来源：T04-S014 T04-S060 T04-S061 T04-S080

### F3.《改变世界的机器》的数据与叙事之争
- **方法学**：跨厂生产率对比需要对车型复杂度、垂直整合边界、自动化水平、什么算「装配工时」做大量标准化调整；不同的调整假设会显著改变「日本厂效率优势」的幅度。批评者认为 IMVP 的调整方法透明度不足，标志性倍数被过度传播。
- **浪漫化**：书把丰田写成理想型，弱化了对供应商的持续降价压力、班组高强度、临时工与派遣工在缓冲中的角色；也没有预见 2009-2010 年丰田大规模召回所暴露的「快速扩张 + 全球化供应链」下质量体系的裂缝。
- **词汇的胜利与语义的失守**：25 周年前后的学术回顾普遍承认这本书让「lean」进入全世界的管理词汇表，但也让它在实践中被广泛简化为**裁员与压库存**，与 TPS 强调的「培养人、把问题暴露出来」几乎相反。这一点连 LEI 自己都在反复纠正。
- **劳动关系一支的批评**：社会学与劳资关系学者（「精益的阴暗面」这一系文献）认为精益是「以压力管理」——去掉库存缓冲后，异常直接转化为工人身上的强度与工时；这一支与管理学主流几乎不互相引用。
来源：T04-S009 T04-S062 T04-S063 T04-S064 T04-S081 T04-S082

### F4. DDMRP 的合法性之争
- **拥护方**：Demand Driven Institute 与其认证生态、部分 ERP/APS 厂商，主张 DDMRP 解决了 MRP 的「紧张性（nervousness）」与前置期叠加放大问题，且是计划员真能看懂并执行的方法。
- **质疑方**：
  1. **实证不足**——系统性文献综述明确指出经同行评审的严肃验证很少，多数证据是实施方自述或硕士论文级别。
  2. **基线不公平**——对照组常是「教科书里最朴素的 MRP」，而不是现代随机/概率预测方法；Lokad 等量化派据此认为「优于 MRP」的结论不成立。
  3. **新颖性存疑**——批评者认为它是解耦点 + 再订货点 + 精益缓冲思想的再包装，理论增量有限。
  4. **形式化不足**——红黄绿三区与经验系数没有从损失函数推导，难做经济最优。
- **公允的话**：DDMRP 在「让人能操作」这一维度上有真实工程价值，在「被证明优于最佳替代方案」这一维度上**目前证据不足**。把它当作一种可用的缓冲管理实践没问题，当作被验证的科学则不行。
来源：T04-S065 T04-S066 T04-S067 T04-S083

### F5. JIT 是不是 2020-2022 全球断链的元凶
- **控方**：主流财经媒体在芯片荒、口罩与呼吸机短缺期间大量将 JIT 点名为脆弱性根源；汽车业 2021 财年前后因缺芯的全球减产损失被估计在两千亿美元量级。逻辑是：几十年把库存当浪费砍掉，等于把整个系统的缓冲砍到零。
- **辩方（学界主流）**：
  - Choi、Netland、Sanders、Sodhi、Wagner 等在 *Production and Operations Management*（2023）的论文明确指出学界分裂，并给出「JIT 在适配的供应链段落中即使遭遇中断也能保持优势」的立场——问题在于**在哪些段落用 JIT**，而不是 JIT 本身。
  - 真正实行 TPS 的企业（本地化供应、平准化、内建质量、长期供应商关系）在疫情中表现更好；丰田恰恰因为在福岛地震后建立了芯片安全库存与多级供应商可视化，在缺芯初期比同行扛得更久。
  - 被点名的许多短缺品（卫生纸、家具）从来不是 JIT 供应链——把无关行业的短缺算到 JIT 头上是归因错误。
  - 更可能的根因组合是：需求结构剧变（服务转商品）、单源与单一国别集中、多级供应链可视化缺失、以及**短期主义的成本考核**（把库存当财报负担砍到极限），而不是 JIT 的技术原理。
- **仍未解决的部分**：JIT 与韧性的取舍在**高度集中、长前置期、政治敏感**的品类（先进制程半导体、特定原料药、稀土）上是真实的；这类品类需要战略库存或产能冗余，这一点两方都不否认。争的是范围，不是有无。
来源：T04-S068 T04-S069 T04-S070 T04-S084 T04-S085

---

## Source Manifest

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T04-S001 | https://en.wikipedia.org/wiki/The_Goal_(novel) | secondary | 2026-09-02 | Wikipedia | encyclopedia entry, bibliographic facts only |
| T04-S002 | https://en.wikipedia.org/wiki/Theory_of_constraints | secondary | 2026-09-02 | Wikipedia | encyclopedia overview of five focusing steps |
| T04-S003 | https://www.researchgate.net/publication/272392183_Theory_of_Constraints_A_Literature_Review | secondary | 2026-09-02 | ResearchGate | aggregator hosting of a TOC literature review |
| T04-S004 | https://en.wikipedia.org/wiki/Taiichi_Ohno | secondary | 2026-09-02 | Wikipedia | biography and seven wastes list |
| T04-S005 | https://uen.pressbooks.pub/ompeople/chapter/taiichi-ohno/ | secondary | 2026-09-02 | Utah Education Network / open textbook | academic open-textbook chapter on Ohno |
| T04-S006 | https://books.google.com/books/about/Toyota_Production_System.html?id=7_-67SshOy8C | secondary | 2026-09-02 | Google Books | bibliographic record for the 1988 Productivity Press translation |
| T04-S007 | https://www.lean.org/store/book/the-machine-that-changed-the-world/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S008 | https://en.wikipedia.org/wiki/The_Machine_That_Changed_the_World_(book) | secondary | 2026-09-02 | Wikipedia | encyclopedia entry, IMVP background |
| T04-S009 | https://bear.buckingham.ac.uk/116/8/25%20years%20of%20Lean%20final_pre-print%20copy.pdf | verified_primary | 2026-09-02 | University of Buckingham research repository | academic pre-print reviewing 25 years of lean |
| T04-S010 | https://www.lean.org/lexicon-terms/lean-thinking/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S011 | https://en.wikipedia.org/wiki/James_P._Womack | secondary | 2026-09-02 | Wikipedia | biography, LEI founding |
| T04-S012 | https://www.mheducation.com/highered/mhp/product/toyota-way-second-edition-14-management-principles-world-s-greatest-manufacturer.html | surrogate_primary | 2026-09-02 | McGraw Hill | publisher own page for the 2020 2nd edition, publisher own publication |
| T04-S013 | https://www.lean.org/the-lean-post/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S014 | https://en.wikipedia.org/wiki/Factory_Physics | secondary | 2026-09-02 | Wikipedia | encyclopedia entry on the book and its laws |
| T04-S015 | https://projectproduction.org/resources/glossary/key-terms/ | secondary | 2026-09-02 | Project Production Institute | practitioner glossary applying VUT/operations science |
| T04-S016 | https://books.google.com/books/about/Factory_Physics.html?id=TfcWAAAAQBAJ | secondary | 2026-09-02 | Google Books | bibliographic record, 3rd edition Waveland Press |
| T04-S017 | https://www.lean.org/store/book/learning-to-see/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S018 | https://www.lean.org/the-lean-post/articles/insights-on-why-when-and-how-value-stream-mapping-is-a-vital-part-of-continuous-improvement/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S019 | https://www.lean.org/lexicon-terms/kata/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S020 | https://en.wikipedia.org/wiki/Toyota_Kata | secondary | 2026-09-02 | Wikipedia | encyclopedia entry, bibliographic facts on the 2009 McGraw-Hill book |
| T04-S021 | https://deming.org/explore/fourteen-points/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute own publication |
| T04-S022 | https://mitpress.mit.edu/9780262350037/out-of-the-crisis/ | verified_primary | 2026-09-02 | MIT Press | publisher own page for the 2018 reissue |
| T04-S023 | https://sheffi.mit.edu/book/resilient-enterprise | verified_primary | 2026-09-02 | Yossi Sheffi / MIT | author own site |
| T04-S024 | https://mitpress.mit.edu/9780262693493/the-resilient-enterprise/ | verified_primary | 2026-09-02 | MIT Press | publisher own page |
| T04-S025 | https://www.demanddriveninstitute.com/ | verified_primary | 2026-09-02 | Demand Driven Institute | originator institute own publication |
| T04-S026 | https://www.lokad.com/demand-driven-material-requirements-planning-ddmrp/ | secondary | 2026-09-02 | Lokad | vendor critique of DDMRP, partisan |
| T04-S027 | https://www.brightworkresearch.com/how-convincing-is-the-mit-ddmrp-study/ | secondary | 2026-09-02 | Brightwork Research | independent analyst critique, partisan |
| T04-S028 | https://www.mheducation.com/highered/mhp/product/orlicky-s-material-requirements-planning-third-edition.html | surrogate_primary | 2026-09-02 | McGraw Hill | publisher own page, 3rd edition 2011, publisher own publication |
| T04-S029 | https://en.wikipedia.org/wiki/Material_requirements_planning | secondary | 2026-09-02 | Wikipedia | encyclopedia entry on MRP logic and limits |
| T04-S030 | https://www.pearson.com/en-us/subject-catalog/p/supply-chain-management-strategy-planning-and-operation/P200000005704 | surrogate_primary | 2026-09-02 | Pearson | publisher own page, publisher own publication |
| T04-S031 | https://www.kellogg.northwestern.edu/faculty/directory/chopra_sunil.aspx | verified_primary | 2026-09-02 | Kellogg School, Northwestern University | author institutional faculty page |
| T04-S032 | https://books.google.com/books/about/A_Study_of_the_Toyota_Production_System.html?id=RKWU7WElJ7oC | secondary | 2026-09-02 | Google Books | bibliographic record, Productivity Press 1989 revised English edition |
| T04-S033 | https://en.wikipedia.org/wiki/Shigeo_Shingo | secondary | 2026-09-02 | Wikipedia | biography, SMED and poka-yoke attribution disputes |
| T04-S034 | https://en.wikipedia.org/wiki/Critical_chain_project_management | secondary | 2026-09-02 | Wikipedia | encyclopedia entry on CCPM buffers |
| T04-S035 | https://www.tocico.org/ | verified_primary | 2026-09-02 | TOCICO (Theory of Constraints International Certification Organization) | originator institute own publication; also the TOC certification body co-founded by Goldratt |
| T04-S036 | https://hbr.org/1999/09/decoding-the-dna-of-the-toyota-production-system | verified_primary | 2026-09-02 | Harvard Business Review | journal official article page |
| T04-S037 | https://www.lean.org/the-lean-post/articles/decoding-the-dna-of-the-toyota-production-system/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S038 | https://sloanreview.mit.edu/article/the-bullwhip-effect-in-supply-chains/ | verified_primary | 2026-09-02 | MIT Sloan Management Review | journal official article page |
| T04-S039 | https://doi.org/10.1287/mnsc.43.4.546 | verified_primary | 2026-09-02 | Management Science (INFORMS) | peer-reviewed journal DOI, the 1997 academic version |
| T04-S040 | https://www2.isye.gatech.edu/~jvandeva/Classes/6203/2006/BullWhipRefs.htm | verified_primary | 2026-09-02 | Georgia Tech ISyE | university course reference list |
| T04-S041 | https://hbr.org/1997/03/what-is-the-right-supply-chain-for-your-product | verified_primary | 2026-09-02 | Harvard Business Review | journal official article page |
| T04-S042 | https://store.hbr.org/product/what-is-the-right-supply-chain-for-your-product/97205 | secondary | 2026-09-02 | HBR Store | commerce listing page |
| T04-S043 | https://hbr.org/2004/10/the-triple-a-supply-chain | verified_primary | 2026-09-02 | Harvard Business Review | journal official article page |
| T04-S044 | https://www.gsb.stanford.edu/faculty-research/publications/triple-supply-chain | verified_primary | 2026-09-02 | Stanford Graduate School of Business | author institutional publication record |
| T04-S045 | https://www.ascm.org/learning-development/certifications-credentials/exam-details/ | verified_primary | 2026-09-02 | ASCM | certification body official page |
| T04-S046 | https://www.ascm.org/globalassets/ascm_website_assets/docs/certification-certificates-comparisoncharts.pdf | verified_primary | 2026-09-02 | ASCM | certification body official comparison chart |
| T04-S047 | https://www.apics.org/docs/default-source/certification/apics-certification-comparison-chart.pdf | verified_primary | 2026-09-02 | APICS / ASCM | certification body official document |
| T04-S048 | https://www.ascm.org/corporate-solutions/standards-tools/scor-ds/ | verified_primary | 2026-09-02 | ASCM | association official standard page |
| T04-S049 | https://www.ascm.org/globalassets/ascm_website_assets/docs/scor/intro-and-front-matter-scor-digital-standard-2025.pdf | verified_primary | 2026-09-02 | ASCM | association official SCOR DS 14.0 front matter |
| T04-S050 | https://en.wikipedia.org/wiki/Supply_chain_operations_reference | secondary | 2026-09-02 | Wikipedia | encyclopedia entry on SCOR history |
| T04-S051 | https://micromasters.mit.edu/scm/ | verified_primary | 2026-09-02 | MIT | university official program page |
| T04-S052 | https://ctl.mit.edu/education/online-education/mitx-micromastersr-program-supply-chain-management | verified_primary | 2026-09-02 | MIT Center for Transportation and Logistics | university official program page |
| T04-S053 | https://scx-static-assets.s3.amazonaws.com/SCx%20Key%20Concept%20Documents/MITx_MicroMasters_SCM_KeyConcepts.pdf | secondary | 2026-09-02 | Chris Caplice & Eva Ponce, MIT CTL | course faculty own publication |
| T04-S054 | https://www.lean.org/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication |
| T04-S055 | https://shingo.org/about-the-shingo-institute/ | verified_primary | 2026-09-02 | Shingo Institute, Utah State University | originator institute own publication |
| T04-S056 | https://www.asq.org/cert/six-sigma-black-belt | verified_primary | 2026-09-02 | American Society for Quality | certification body official page |
| T04-S057 | https://www.icourse163.org/ | secondary | 2026-09-02 | 中国大学MOOC (icourse163) | platform index, individual course quality unverified |
| T04-S058 | https://www.allaboutlean.com/drum-buffer-rope/ | secondary | 2026-09-02 | Christoph Roser, AllAboutLean | expert practitioner blog, partisan on DBR vs kanban |
| T04-S059 | https://txm.com/theory-of-constraints-vs-lean-which-makes-sense-for-your-business/ | secondary | 2026-09-02 | TXM Lean Solutions | consultancy blog, partisan |
| T04-S060 | https://www.qualitydigest.com/inside/lean-column/where-ohno-and-vut-intersect-092519.html | secondary | 2026-09-02 | Quality Digest | trade magazine column linking Ohno and VUT |
| T04-S061 | https://metricgate.com/docs/hopp-spearman-factory-physics/ | secondary | 2026-09-02 | Metricgate | third-party documentation of the Kingman/VUT approximation |
| T04-S062 | https://web.mit.edu/esd.83/www/notebook/machine.pdf | secondary | 2026-09-02 | MIT ESD.83 course notebook | student book review hosted on a university site, not peer reviewed |
| T04-S063 | https://michelbaudin.com/2012/01/24/lean-versus-the-toyota-production-system/ | secondary | 2026-09-02 | Michel Baudin | practitioner blog on the lean-vs-TPS semantic drift, partisan |
| T04-S064 | https://www.industryweek.com/the-economy/article/21960853/experts-dont-blame-lean-manufacturing-for-toyotas-problems | secondary | 2026-09-02 | IndustryWeek | trade press coverage of the Toyota recall debate |
| T04-S065 | https://www.demanddriveninstitute.com/ddmrp | verified_primary | 2026-09-02 | Demand Driven Institute | originator institute own publication |
| T04-S066 | https://www.jiem.org/index.php/jiem/article/view/3331 | verified_primary | 2026-09-02 | Journal of Industrial Engineering and Management | peer-reviewed open-access journal official article page |
| T04-S067 | https://www.brightworkresearch.com/how-accurate-is-the-criticism-of-lokad-ddmrp-video/ | secondary | 2026-09-02 | Brightwork Research | independent analyst commentary, partisan |
| T04-S068 | https://onlinelibrary.wiley.com/doi/10.1111/poms.13979 | verified_primary | 2026-09-02 | Production and Operations Management (Wiley) | peer-reviewed journal official page |
| T04-S069 | https://en.wikipedia.org/wiki/2021%E2%80%932023_global_supply_chain_crisis | secondary | 2026-09-02 | Wikipedia | encyclopedia entry, timeline and loss estimates |
| T04-S070 | https://www.leanblog.org/2021/06/should-we-blame-just-in-time-or-short-term-thinking-for-supply-chain-problems/ | secondary | 2026-09-02 | Mark Graban, LeanBlog | practitioner blog defending JIT, partisan |
| T04-S071 | https://doi.org/10.1287/mnsc.35.3.321 | verified_primary | 2026-09-02 | Management Science (INFORMS) | peer-reviewed journal DOI, Sterman 1989 beer game experiment |
| T04-S072 | https://doi.org/10.1287/msom.1060.0149 | verified_primary | 2026-09-02 | Manufacturing & Service Operations Management (INFORMS) | peer-reviewed journal DOI, Cachon Randall Schmidt 2007 |
| T04-S073 | https://doi.org/10.1287/mnsc.25.5.498 | verified_primary | 2026-09-02 | Management Science (INFORMS) | peer-reviewed journal DOI, Eppen 1979 risk pooling |
| T04-S074 | https://stanford.edu/~kostasb/papers/inventory_pooling.pdf | verified_primary | 2026-09-02 | Stanford University (Bimpikis et al.) | university-hosted working paper on pooling under heavy-tailed demand |
| T04-S075 | https://doi.org/10.1287/opre.44.1.87 | verified_primary | 2026-09-02 | Operations Research (INFORMS) | peer-reviewed journal DOI, Fisher & Raman 1996 accurate response |
| T04-S076 | https://doi.org/10.1287/inte.23.4.1 | verified_primary | 2026-09-02 | Interfaces (INFORMS) | peer-reviewed journal DOI, Lee Billington Carter 1993 HP DeskJet |
| T04-S077 | https://hbr.org/1997/01/mass-customization-at-hewlett-packard-the-power-of-postponement | verified_primary | 2026-09-02 | Harvard Business Review | journal official article page |
| T04-S078 | https://doi.org/10.1016/S0925-5273(03)00119-1 | verified_primary | 2026-09-02 | International Journal of Production Economics (Elsevier) | peer-reviewed journal DOI, Olhager 2003 order penetration point |
| T04-S079 | https://doi.org/10.1080/00207543.2024.2314164 | verified_primary | 2026-09-02 | International Journal of Production Research (Taylor & Francis) | peer-reviewed journal DOI, CODP systematic review 2024 |
| T04-S080 | https://doi.org/10.1287/msom.1030.0028 | verified_primary | 2026-09-02 | Manufacturing & Service Operations Management (INFORMS) | peer-reviewed journal DOI, Hopp & Spearman 2004 pull definition |
| T04-S081 | https://doi.org/10.1016/j.jom.2006.04.001 | verified_primary | 2026-09-02 | Journal of Operations Management (Elsevier) | peer-reviewed journal DOI, Holweg 2007 genealogy of lean |
| T04-S082 | https://doi.org/10.5465/amp.2006.20591003 | verified_primary | 2026-09-02 | Academy of Management Perspectives | peer-reviewed journal DOI, Mehri 2006 insider account |
| T04-S083 | https://doi.org/10.3926/jiem.3331 | verified_primary | 2026-09-02 | Journal of Industrial Engineering and Management | peer-reviewed open-access DOI, DDMRP systematic review 2021 |
| T04-S084 | https://doi.org/10.1080/00207543.2025.2483113 | verified_primary | 2026-09-02 | International Journal of Production Research (Taylor & Francis) | peer-reviewed journal DOI, Dolgui Ivanov Simchi-Levi 2025 stress tests |
| T04-S085 | https://publications.jrc.ec.europa.eu/repository/bitstream/JRC139968/JRC139968_01.pdf | verified_primary | 2026-09-02 | European Commission Joint Research Centre | institutional research report on supply chain stress tests |
| T04-S086 | https://doi.org/10.1287/mnsc.1040.0305 | verified_primary | 2026-09-02 | Management Science (INFORMS) | peer-reviewed journal DOI, authors' 2004 retrospective on the bullwhip paper |
| T04-S087 | https://www.ascm.org/learning-development/certifications-credentials/ | verified_primary | 2026-09-02 | ASCM | certification body official landing page |
| T04-S088 | https://www.asq.org/cert/six-sigma-green-belt | verified_primary | 2026-09-02 | American Society for Quality | certification body official page |
| T04-S089 | https://iassc.org/six-sigma-certification/ | verified_primary | 2026-09-02 | International Association for Six Sigma Certification | certification body official page |
| T04-S090 | https://mitxonline.mit.edu/programs/program-v1:MITxT+SCM/ | verified_primary | 2026-09-02 | MITx Online / MIT | university official program enrolment page |
| T04-S091 | https://en.wikipedia.org/wiki/Shingo_Prize | secondary | 2026-09-02 | Wikipedia | encyclopedia entry on the prize categories and history |
| T04-S092 | https://www.usu.edu/today/story/shingo-institute-announces-2025-rising-star-award-recipients-academy-inductees | verified_primary | 2026-09-02 | Utah State University | host university own news publication on the Shingo Institute |
| T04-S093 | https://www.sciencedirect.com/science/article/abs/pii/S027269630400141X | verified_primary | 2026-09-02 | Journal of Operations Management (Elsevier / ScienceDirect) | peer-reviewed journal official page on postponement structures |
| T04-S094 | https://faculty.wharton.upenn.edu/wp-content/uploads/2012/04/Perils.pdf | verified_primary | 2026-09-02 | Wharton School, University of Pennsylvania | author faculty page hosting the paper on perils of delayed differentiation |
| T04-S095 | https://portal.research.lu.se/en/publications/the-customer-order-decoupling-point-in-empirical-operations-and-s/ | verified_primary | 2026-09-02 | Lund University research portal | author institutional publication record |
| T04-S096 | https://www.osti.gov/servlets/purl/2371560 | verified_primary | 2026-09-02 | US Department of Energy OSTI / Argonne National Laboratory | government-hosted research article on the history of the Beer Game |
| T04-S097 | https://www.lean.org/lexicon-terms/value-stream-mapping/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication, VSM definition |
| T04-S098 | https://kresgeguides.bus.umich.edu/Lean-ValueStreams/Value-Streams-VSM-Mapping | verified_primary | 2026-09-02 | Ross School of Business, University of Michigan | university library research guide on value-stream mapping |
| T04-S099 | https://www.lean.org/lexicon-terms/heijunka/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication, heijunka definition |
| T04-S100 | https://www.lean.org/lexicon-terms/jidoka/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication, jidoka definition |
| T04-S101 | https://www.lean.org/lexicon-terms/takt-time/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute own publication, takt time definition |
| T04-S102 | https://www.ascm.org/ | verified_primary | 2026-09-02 | ASCM | association official site, APICS successor body |
