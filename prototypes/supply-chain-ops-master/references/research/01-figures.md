# Track 01 — 行业大佬 / Figures
## 供应链与生产运营（Supply Chain & Production Operations）

> **蒸馏范围**：制造业与消费品的实体供应链「计划—制造—交付」运营判断。含精益/TPS、约束理论 TOC、六西格玛与统计质量、工厂物理学（用排队论看运营的科学）、S&OP 产销协同与需求计划、库存与交期、多级 BOM 与供应商管理。
> **不含**：跨境电商卖家发货物流、纯采购谈判技巧。
> **受众 locale**：zh-CN。正文中文散文；人名、书名、术语、URL 保留原文（英/日）。
> **`last_checked` 基准日**：2026-09-02　|　**收录人物**：15 位（含 4 个稳定的双人组合）　|　**来源**：94 条

**入选标准**：不按知名度排，按「有没有提出一套可以被反驳的判断方式」排。所以这里没有 CEO，没有咨询品牌，只有流派奠基人和当代最好的拆解者。

---

## 谱系速览

### 一、六大流派归位

| 流派 | 代表人物（本文编号） | 一句话主张 | 它的核心机制 | 它最擅长的场景 | 它的盲区 |
|------|--------------------|-----------|-------------|---------------|---------|
| **精益 / TPS 派** | 大野耐一 (01)、新乡重夫 (02)、Womack & Jones (03)、Liker (04)、Spear (05)、Rother (06) | 把「流」做顺，浪费和问题会自己浮出水面 | 用**低库存**逼出问题 + 用**停线权**让问题不可隐藏 + 用**每天的改善练习**让人自己解决 | 品种相对稳定、量大、可反复练习的重复性生产 | 需求剧烈波动、工序时间高度不稳、一次性项目 |
| **约束理论 TOC 派** | Goldratt (07) | 系统产出只由一个约束决定，约束之外的改善全是幻觉 | 五步聚焦 + Drum-Buffer-Rope（用**时间缓冲**保护瓶颈） + Throughput Accounting | 有明确物理瓶颈、订单驱动、多品种小批量 | 瓶颈漂移的车间；进不了主流财务语言 |
| **统计质量 / 六西格玛派** | Deming (08)、Wheeler (09) | 先分清「系统固有波动」和「特殊原因」，否则一切改善都是瞎折腾 | 过程行为图 / 控制图；系统 94%、个人 6%；渊博知识体系 | 任何有重复测量数据的过程；供应商绩效判读 | 只教你「该不该动」，不教你「怎么把流做顺」 |
| **运营科学 / 工厂物理学派** | Hopp & Spearman (10) | 精益和 TOC 都是同一组数学定律的特例 | Little's Law；**变异必被库存 / 产能 / 时间三者之一吸收**；CONWIP | 定产能、定在制品上限、定交期承诺、判断哪种缓冲最便宜 | 对人、学习、供应商关系与需求端行为几乎无话可说 |
| **需求驱动 DDMRP 派** | Ptak & Smith (11) | MRP 的确定性假设已失效；别追预测精度，去降低对预测的依赖 | 在 BOM 关键层级设**战略解耦缓冲**，切断变异的逐级放大 | 多层 BOM、长提前期、高品种的制造与分销 | 缓冲规则是启发式而非最优解；方法-认证-软件三位一体的角色冲突 |
| **韧性 / 风险派** | Hau Lee (12)、Sheffi (13)、Simchi-Levi (14) | 效率最优的链条最脆；要为「断」而设计 | 牛鞭四因；Triple-A；探测时间与恢复时间（TTR/TTS）；Risk Exposure Index | 网络级风险敞口、单一来源、深层供应商暴露 | 投入回报是「没发生的事故」，财务上无法证明，预算永远最先被砍 |
| **中文语境转译** | 刘宝红 (15) | 高成本高库存的根子在计划能力，不在采购砍价 | 需求预测 → 库存计划 → 供应链执行「三道防线」 | 中国制造/零售企业的计划职能从零建设 | 是高质量转译与实战注释，不是原创流派，理论主张需回一手核对 |

### 二、他们互相攻击的点（争议 > 共识）

这套 OS 最有价值的部分不是六派各自的正确，而是**它们在哪里互不相容**。下面每一条都是真实的、有文本可查的对立，不是「各有千秋」。

1. **Goldratt 打精益：「等浪费自己浮现」是把诊断权交给运气。**
   精益的机制是降低库存、让问题暴露，然后改善。Goldratt 的立场是——为什么要等？直接指出约束在哪就行。TOC 圈广为流传的这句嘲讽有其文本基础：他在 2008 年的《Standing on the Shoulders of Giants》里以 Hitachi Tool Engineering 为例，明确论证**精益实施失败不是执行不力，而是前提条件不成立**——福特用传送带的物理长度限制在制品，大野用看板数量限制在制品，两者都要求环境相对稳定；在品种多、需求波动、工序时间不稳的环境里，这个前提不存在，所以必须改用**时间缓冲**。〔T01-S063 / T01-S064〕
   *精益方的反击*：约束会漂移、会被指错，而且真实工厂里大量瓶颈是**政策造成的（policy constraint）**而非设备；TOC 假设你能看清瓶颈，这个假设本身才是运气。

2. **工厂物理学派同时打精益和 TOC：你们都是特例，不是理论。**
   Hopp & Spearman 在《To Pull or Not to Pull: What Is the Question?》(M&SOM, 2004) 里做了一次概念清洗：**pull 的定义不是「按需求触发生产」，而是「显式给在制品设上限」**；按这个定义，很多自称 pull 的系统其实是 push，而 MRP 加一个 WIP 上限就变成了 pull。看板的好处主要来自「在制品被封顶」这个事实，而不是「处处拉动」这个仪式——所以一个总量上限（CONWIP）在更一般的环境里能拿到同样的好处。他们进一步定义 **lean 的本质是「用成本最低的缓冲吸收变异」**，而不是「消除浪费」。〔T01-S066〕
   对 TOC 同样处理：五步聚焦是「容量约束下最优化」的直觉版本，DBR 是一种带 WIP 上限的投料策略；TOC 的贡献是传播力而非理论新意。
   *反击*：Factory Physics 的定律刻画的是稳态、单一产品族、机器为中心的车间，对多层供应网络、需求端行为、供应商关系与人几乎无话可说。定律告诉你物理上限在哪，不告诉你一群人怎样每天逼近它——那正好是 Rother 与 Spear 的领域。

3. **工厂物理学派打六西格玛：变异消灭不完，问题是谁来付账。**
   变异缓冲定律说，系统里的变异**必然**被**库存 / 产能 / 时间（交期）**三者之一吸收。所以把全部资源投进「降低变异」，常常不如用同样的钱买一点产能缓冲。同理，「零库存」不是好坏问题，是**记账位置转移**问题——你把变异从库存挪到了交期或备用产能上。〔T01-S066 / T01-S068〕

4. **新乡重夫打统计质量派：统计抽样从设计上就接受不良。**
   新乡主张用 100% 源流检查加 poka-yoke 取代统计抽样检验，理由是抽样在数学上就承认「一定比例的不良会流出去」，因此永远到不了零缺陷。这与 Deming「不理解变异就无法改进」是正面对立。〔T01-S033 / T01-S034〕
   *Wheeler 一侧的反击*：防错装置解决的是可被防错的错误，解决不了过程本身的漂移；没有过程行为图，你根本不知道该往哪装防错。两人各自击中对方的盲区——这条裂缝至今贯穿制造业质量部门的组织架构。

5. **统计派内战：Wheeler 打六西格玛的度量基础。**
   sigma level 与 DPMO 的换算依赖 **1.5σ 位移假设** + 正态分布假设。Wheeler 的判断是：「假设一个不可预测的过程漂移不会超过 1.5σ，是完全站不住脚的」——不可预测的定义就是你不知道它会漂多远。他并指出 sigma level 的估计跨越九个数量级，使不合格品率的估计不可靠。这个数字的来源本身也有问题：它原本是 Motorola 内部做设计仿真的一个测试值，不是过程度量。〔T01-S081 / T01-S084〕
   *六西格玛方的官方解释见* 〔T01-S086〕（把它当成长期过程漂移的经验保守值）；*第三方在临床检验领域要求为它提供证据的论文见* 〔T01-S085〕。

6. **Deming 打六西格玛的组织形态（隔代交火）。**
   Deming 1993 年去世，未直接评价六西格玛（1986 年起于 Motorola，1995 年经 GE 规模化）。但两派长期互不认账：Deming 派认为「黑带项目 + 财务收益挂钩」是把改进重新包装成个人绩效游戏，恰恰违背了「94% 属于系统」的核心；六西格玛派认为 Deming 只有哲学、没有可部署的项目方法论。Deming 的 14 点第 11、12 条直接要求废除数量指标、MBO 与年度绩效评级——这是他被引用最多、执行最少的部分。〔T01-S043 / T01-S047〕

7. **断链之后：「JIT 是不是元凶」之争。**
   *控方*：just-in-time 假设环境相对稳定、扰动小而少，因此吸收不了疫情级别的大冲击；几十年来企业被市场纪律训练成低库存，冲击一来就集体断供。美国 CEA 的官方 issue brief 与多项同行评议研究都在这个框架下论述效率-韧性权衡。〔T01-S088 / T01-S089 / T01-S090〕
   *辩方（Sheffi 一派与精益方）*：出问题的是**单一来源（single sourcing）与对深层供应商的无知**，不是低库存本身——很多囤了大量库存的公司照样断供，因为他们囤错了东西。真正的变量是**探测时间与恢复时间**，不是库存天数。把 JIT 当元凶，是把「短期主义的成本削减」误认成「丰田的 JIT」。〔T01-S023 / T01-S091〕
   *第三方立场（工厂物理学派）*：这场争论本身问错了问题——变异总要被某种缓冲吸收，疫情只是把账单从库存挪到了交期与产能上；问「JIT 好不好」不如问「你选的缓冲对不对」。

8. **DBR 的假设被批：瓶颈会漂移。**
   Drum-Buffer-Rope 假设约束相对稳定且可识别。在真实的多品种小批量车间里，瓶颈随产品组合漂移（wandering bottleneck），鼓点需要不断重设，收益急剧下降。TOC 内部对此的回应是 **Simplified DBR (S-DBR)**；工厂物理学派的回应更狠——这些排程结论本来就能直接由排队论定律推出。〔T01-S065 / T01-S066〕

9. **精益 vs. DDMRP：库存到底是不是万恶之源。**
   精益的第一戒律是库存掩盖问题；DDMRP 明确主张**有些库存是资产**（战略解耦库存），并要求把它放在 BOM 的特定层级。精益纯粹派视之为倒退回推式生产；DDMRP 的回应是——不解耦，变异就沿 BOM 逐级放大，你在最下游看到的是一个被放大了十倍的鬼影。〔T01-S012〕

10. **TOC vs. DDMRP：缓冲该放在哪。**
    DDMRP 的红黄绿缓冲管理直接继承自 TOC，但把缓冲从**约束前面**搬到了**解耦点**。这不是细节差异——它等于承认在多层 BOM 的复杂供应链里，单一约束模型不够用了。这是 TOC 谱系内部最重要的一次分化。〔T01-S012 / T01-S060〕

11. **Hau Lee 划的一条界：结构性变化 ≠ 突发中断。**
    Triple-A 里的 adaptability 处理的是市场迁移、成本曲线变化这类**结构性长期变化**，与 Sheffi / Simchi-Levi 关心的**突发中断**不是一回事。为地震准备和为需求结构迁移准备，是两套不同的投资——把两者混为一谈是韧性讨论里最常见的偷换。〔T01-S020〕

12. **韧性派内部：韧性能不能被算出来。**
    同在 MIT，Sheffi 走组织能力与案例路线（探测时间、恢复文化、深层供应商可视化），Simchi-Levi 走优化模型路线（TTR / TTS / REI）。Simchi-Levi 最大胆的简化是**只用 impact 维度、放弃 likelihood 维度**——因为低频高损事件的概率根本估不出来，硬估只会带来虚假的精确。批评者说这会让你为极不可能的事过度投资。〔T01-S036 / T01-S023〕

13. **精益内部：文化可不可移植。**
    Liker 主张丰田模式可以在非日本、非汽车的组织里建立，为此写了两本讲精益领导力培养的书；Rother 与相当一部分实践者认为 14 条原则是**对结果的描述**，照着结果清单去建设是典型的因果倒置——你只能复制丰田「试的方式」，复制不了它的解。Liker 在 2021 年第二版《The Toyota Way》里把重心从工具移到科学思维、吸收了 Toyota Kata，可视为对这个批评的部分让步。〔T01-S050 / T01-S010〕

14. **一条贯穿六派的共同敌人：成本会计。**
    这是唯一让大野耐一、Goldratt 和 Ptak & Smith 站在同一边的东西。大野认为把设备开动率当 KPI 制造了过量生产（七大浪费里最坏的一个，因为它掩盖其他所有浪费）；Goldratt 认为「产品成本」在共享资源的系统里根本不存在，用它决策必然错；Ptak & Smith 在《Demand Driven Performance》里直接攻击吸收成本法（absorption costing）逼着工厂多生产。三派方法互相攻击，但都指认同一个凶手。〔T01-S029 / T01-S060 / T01-S012〕

---

## 人物档案

### 01 · 大野耐一 Taiichi Ohno（1912–1990）— TPS 的立法者

**核心一句话.** 「我们做的全部事情，就是盯住从接到客户订单到收到现金这段时间线，然后把里面不增值的浪费砍掉。」——他把「降低成本」这个模糊目标，重写成一条**可测量的时间轴**，这是二十世纪运营管理最重要的一次问题重述。

**他到底立了什么法.** 丰田官方把 TPS 定义为「以彻底消除浪费为哲学、追求最有效率生产方式的生产体系」，两根支柱是 **jidoka（自働化 / automation with a human touch，异常自动停线）** 与 **Just-in-Time（只在需要的时候、按需要的量、做需要的东西）**。Jidoka 的血脉来自丰田佐吉 1896 年的自动停机织机与 1924 年 G 型自动织机，Just-in-Time 的概念来自丰田喜一郎；大野耐一的贡献是在 Eiji Toyoda（丰田英二）的支持下，把这两条祖训**变成车间里可运行的机制**——看板（kanban）、超市式后工程领取、少人化、七大浪费的分类、五个为什么。

**代表作品 / 观点**

- 丰田官方对 TPS 的定义、两大支柱与起源叙述（含大野耐一角色的官方措辞） —— 〔一手〕 https://global.toyota/en/company/vision-and-philosophy/production-system/
- 《トヨタ生産方式——脱規模の経営をめざして》(1978)；英译《Toyota Production System: Beyond Large-Scale Production》(Productivity Press, 1988) —— 〔一手·本人著作〕 https://www.routledge.com/Toyota-Production-System-Beyond-Large-Scale-Production/Ohno/p/book/9780915299140
- 英译本全文 PDF（可核对原始措辞，非商用转载） —— 〔一手·著作原文〕 https://www.almendron.com/tribuna/wp-content/uploads/2021/12/toyota-production-system-beyond-large-scale-production.pdf
- 学术教材式传记条目（生平、时间线核对） —— 〔二手〕 https://uen.pressbooks.pub/ompeople/chapter/taiichi-ohno/

**值得读 / 听 / 看的 3 件事**

1. 《Toyota Production System: Beyond Large-Scale Production》全书 —— 这本书不厚、不好读，语气近乎训人，但它是唯一的一手宪法。特别读他讲**为什么先做「后工程领取」而不是先做看板**：看板只是那个原则的载体，不是原则本身。很多人抄走了看板，丢掉了原则。
2. 丰田官方的 TPS 页面 —— 用来校准：西方转述里 TPS 常被写成「消除浪费的工具集」，丰田自己的措辞里 jidoka（停线权）和 JIT 是并列的两根柱子，而停线权往往被中国和西方工厂第一个砍掉。
3. 《Workplace Management》（大野口述整理，另一本一手材料） —— 里面有他最锋利的那些短句，例如把「合理化」和「改善」区分开：改善必须由做事的人自己做。

**争议 / 非主流立场**

- **他自己承认 TPS 是「反常识」的，且极不受欢迎。** 大野在书里直言，减少在制品、把机器停下来、让人闲着而不是让机器满负荷，在当时的丰田内部被视为疯子行为；他被叫作「暴君」「大野的鬼」。他对「让人接受」这件事毫无兴趣，靠的是强制与权力，不是共识——这一点在今天所有讲「精益要靠文化」的教材里被系统性地美化掉了。
- **他公开否认 TPS 可以被复制**：TPS 是丰田在**没有钱、市场小、品种多、量小**的战后条件下逼出来的答案，福特式大批量在那个条件下不可行。他认为脱离条件抄结论毫无意义。这是后来 Rother、Spear 反复重申的同一句话。
- **对成本会计的敌意**：大野认为把机器开动率（设备稼働率）当 KPI 是制造过量生产的元凶——过量生产是七大浪费里最坏的一个，因为它**掩盖所有其他浪费**。这一条与 DDMRP 攻击吸收成本法是同一条战线。
- **「库存降下来，问题自己浮出水面」**：这是他最著名也最被 Goldratt 嘲讽的一条（「等浪费自己浮现」，见下文 TOC 部分）。TOC 认为这是把系统的诊断权交给运气。
- **他与新乡重夫的功劳之争**：西方文献常把 SMED 与 poka-yoke 直接算在新乡名下、把 TPS 算在大野名下；日本方面的叙述里两人角色更纠缠，新乡是外部顾问/讲师，大野是内部执行者。功劳归属至今没有统一口径。

**其思想的当代承载机构 / 传人.** 官方口径由 Toyota Motor Corporation 自己维护（global.toyota 的 TPS 页面 + 各地 Toyota Production System Support Center）；西方的翻译与传播由 Lean Enterprise Institute（Womack 创办）与 Lean Global Network 承载；学术性重述由 Steven Spear（MIT）与 Mike Rother（Michigan）两条线继承——前者解释「规则」，后者解释「练法」。

### 02 · 新乡重夫 Shigeo Shingo（1909–1990）— 把「不可能」变成工程问题的人

**核心一句话.** 「检验不产生质量，只确认不良；要让不良根本不可能发生。」——他拒绝在「良率 99.9%」上做优化，直接把目标定成**零缺陷（Zero Quality Control）**，并且给出了达成它的机制：源流检查 + poka-yoke（防错装置）+ 100% 自动检查 + 即时反馈。

**为什么重要.** 大野耐一给了 TPS 的宪法，新乡重夫给了让宪法能落地的两项关键技术：
- **SMED（Single-Minute Exchange of Die，单分钟换模）**：把换模时间从几小时压到 10 分钟以内。这不是「省时间」的小改善——它是 JIT 的**前提条件**：换模贵，批量就必须大；批量大，就不可能小批量拉动。SMED 的核心洞见是把换模动作分成「内部作业（必须停机做）」与「外部作业（可在运行中做）」，然后不断把内部转成外部。
- **poka-yoke（ポカヨケ，防错）**：他 1960 年代把这个词用于工业流程，主张用物理装置让错误动作做不出来，而不是靠工人「更小心」。

**代表作品 / 观点**

- 《A Study of the Toyota Production System from an Industrial Engineering Viewpoint》(1981/1989 英译) —— 从 IE（工业工程）视角对 TPS 的系统化重构，与大野的第一人称叙事互补 —— 〔一手·本人著作〕
- 《Zero Quality Control: Source Inspection and the Poka-Yoke System》(1986 英译) —— 〔一手·本人著作〕
- 《A Revolution in Manufacturing: The SMED System》(1985 英译) —— 〔一手·本人著作〕
- Shingo Institute（Utah State University Jon M. Huntsman School of Business 下属），Shingo Model® 与 Shingo Prize® 的守护机构 —— 〔一手·冠名机构〕 https://shingo.org/
- 生平、著作年表与术语来源核对 —— 〔二手〕 https://en.wikipedia.org/wiki/Shigeo_Shingo ；https://en.wikipedia.org/wiki/Poka-yoke

**值得读 / 听 / 看的 3 件事**

1. 《A Revolution in Manufacturing: The SMED System》—— 读它的正确姿势不是学换模，是学**他的问题重构方式**：所有人都在问「怎么换得快一点」，他问「哪些动作根本不该在停机时做」。这个动作在任何领域都可以复用。
2. 《Zero Quality Control》—— 尤其他对统计抽样检验（statistical sampling inspection）的正面攻击，见下。
3. Shingo Institute 的 Shingo Model 材料 —— 注意：这是**后人以他命名的体系**，不是他本人写的，读的时候要分清哪些是新乡、哪些是 Utah State 的加工。

**争议 / 非主流立场**

- **他公开反对统计质量控制（SQC）**：这是他最激烈也最被回避的一条。新乡认为统计抽样检验从设计上就接受了「一定比例的不良」，因而永远达不到零缺陷；他主张用 100% 源流检查 + 防错装置取代抽样统计。**这与 Deming / 六西格玛统计派是正面对立的立场**——统计派认为不理解变异就无法改进，新乡派认为统计是在给不良找台阶。这条裂缝至今贯穿制造业质量部门。
- **「改善是工程问题，不是意识问题」**：他对「提高质量意识」「加强培训」这类回答几乎是鄙视的态度，认为凡是靠人的注意力维持的质量都会失效。
- **功劳归属争议**：西方（尤其 Productivity Press 与 Norman Bodek 的推广）把新乡塑造成「TPS 的共同创造者」，日本内部叙述则更强调他是外部 IE 顾问与讲师，很多机制的实际推动者是大野和丰田内部人员。他本人从未在丰田任职。
- **Shingo Prize 的通货膨胀问题**：Shingo Prize 曾出现过获奖企业随后业绩恶化甚至工厂关闭的案例，促使 Shingo Institute 在 2008 年后把评审重心从「工具实施程度」改为「文化与原则」（即今天的 Shingo Model）。这次改版本身就是对「精益工具化」最有力的自我批评。

**其思想的当代承载机构 / 传人.** Shingo Institute（Utah State University）持有 Shingo Model® 与 Shingo Prize®；SMED 与 poka-yoke 已被吸收进几乎所有精益与 TPM 教材，成为无需署名的通用知识——这本身是最高级的传承，也让他本人的原始论证（尤其反 SQC 那一段）被普遍遗忘。

### 03 · James P. Womack & Daniel T. Jones — 把 TPS 翻译成西方能学的「精益」

**核心一句话.** 「Lean thinking 的本质不是少用人，是用一半的一切做出两倍的东西——因为价值只由终端客户定义，其余全是浪费。」他们做的事，是把丰田车间里一套默会的手艺，拆成五步可教的语法：identify value → map the value stream → create flow → establish pull → seek perfection。

**为什么重要.** 「lean」这个词本身是 MIT 的 International Motor Vehicle Program (IMVP) 造出来的（研究员 John Krafcik 首用，Womack 与 Jones 把它写进《The Machine That Changed the World》并推向全球）。没有这两个人，丰田生产方式在西方只会停留在「日本人的怪癖」层面。Womack 1997 年创办 Lean Enterprise Institute（非营利），Jones 在英国办 Lean Enterprise Academy，两家共同催生 2007 年的 Lean Global Network。

**代表作品 / 观点**

- 《The Machine That Changed the World》(1990, 与 Daniel Roos 合著)，IMVP 五年、五百万美元研究的产物 —— 〔一手〕（作者本人机构页收录）https://www.lean.org/about-lei/senior-advisors-staff/james-womack/
- 《Lean Thinking: Banish Waste and Create Wealth in Your Corporation》(1996；2003 修订；2nd Edition 仍在 LEI 书店在售) —— 〔一手〕 https://www.lean.org/store/book/lean-thinking-2nd-edition/
- 《Lean Solutions》(2005) —— 把镜头从工厂转向「消费的浪费」：客户为了消费你的产品所浪费的时间，也是你的浪费 —— 〔一手〕 https://www.lean.org/store/book/lean-solutions/
- LEI 的机构自述与沿革 —— 〔一手〕 https://www.lean.org/about-lei/news/background-what-is-the-lean-enterprise-institute/
- Dan Jones 在 LEI 的 thought-leader 页（英国 Lean Enterprise Academy 创办人、LEI 高级顾问） —— 〔一手〕 https://www.lean.org/about-lei/thought-leader/daniel-jones/

**值得读 / 听 / 看的 3 件事**

1. 《Lean Thinking》全书 —— 不要只读五原则那一章，真正的养分在后半部的企业改造案例（Pratt & Whitney、Porsche、Lantech），它们展示了「流」被打通时组织会怎样痛。
2. 「Lean Thinking at 20: A Q&A with Jim Womack and Dan Jones」—— 两位作者二十年后自评哪里说对了、哪里说错了。〔一手〕 https://www.lean.org/the-lean-post/articles/lean-thinking-at-20-a-qa-with-jim-womack-and-dan-jones/
3. 「Jim Womack and Dan Jones on the Evolution and Future of Lean」—— 他们对「精益已死 / 精益被工具化」批评的正面回应。〔一手〕 https://www.lean.org/the-lean-post/articles/jim-womack-and-dan-jones-on-the-evolution-and-future-of-lean/

**争议 / 非主流立场**

- **他们自己承认最大的失败**：《Lean Thinking》把精益写成了一套「工具清单」，结果全世界的公司买了工具、跳过了管理体系。Womack 后来反复说，价值流图（value stream map）被画成了墙上的壁纸，而不是改变行为的契约。他晚期几乎所有文章都在补这一课（hoshin kanri 方针管理、管理系统而非工具）。
- **「lean」这个词本身是个战略性误译**：它强调「瘦」，于是被 HR 和财务部门理解成裁员授权。丰田内部从不说 lean。Womack 承认这个词让精益背上了「lean = mean」的骂名，但他不打算改。
- **和学界的紧张关系**：《The Machine That Changed the World》的方法论（跨厂对标生产率）被后来的学者批评为口径不可比、把丰田的成绩部分归因于车型组合与本土供应链结构，而非纯管理方法。IMVP 的结论至今是运营管理领域引用最多也争议最多的实证之一。
- **他们与工厂物理学派的分歧**：Womack/Jones 认为精益是一套「看得见浪费」的实践哲学；Hopp & Spearman 认为这只是排队论定律的一个特例，而且是被丰田的具体环境（高量、稳定、低品种）过度拟合的那个特例。

**最近 12 个月（2025-09 ~ 2026-09）动态.** Womack 仍以 LEI 创办人兼高级顾问身份写 The Lean Post 专栏，近期主题集中在 hoshin kanri（方针管理）与「目标—行动对齐」，即他一贯的「工具没用，管理体系才有用」的续篇；文章列表见 https://www.lean.org/the-lean-post/articles/?written_by=811 〔一手〕。Jones 主要活动在英国 Lean Enterprise Academy 与 Lean Global Network 体系内，近年重心偏医疗与零售的端到端流。

### 04 · Jeffrey K. Liker — 把「丰田为什么行」拆成 14 条可讨论的原则

**核心一句话.** 「丰田的优势不在工具，在一套 4P 结构：Philosophy（长期理念）→ Process（流程消除浪费）→ People and Partners（培养人与伙伴）→ Problem Solving（持续解决问题与学习）。大多数公司只抄了 Process 那一层，然后困惑为什么不灵。」

**为什么重要.** Liker 是密歇根大学工业与运营工程系的教授（现已荣休），从 1980 年代起做日美汽车业对比研究，是学界里对丰田观察时间最长的人之一。《The Toyota Way》(2004) 是把 TPS 从「车间技术」提升为「管理体系」的那本书——它让 CEO 而不只是厂长开始读精益。2021 年他出了大改的第二版。

**代表作品 / 观点**

- 《The Toyota Way: 14 Management Principles from the World's Greatest Manufacturer》(McGraw-Hill, 2004；**Second Edition 2021**) —— 〔一手·本人著作〕 出版社官方页 https://www.mheducation.com/highered/mhp/product/toyota-way-second-edition-14-management-principles-world-s-greatest-manufacturer.html
- 第二版前言与「Praise for」页（可核对第二版到底改了什么，由出版社官方技术库放出） —— 〔二手·出版社〕 https://www.accessengineeringlibrary.com/content/book/9781260468519/front-matter/preface2
- 《The Toyota Way to Lean Leadership》(2011, 与 Gary Convis)、《Toyota Under Fire》(2011, 与 Timothy Ogden)、《Developing Lean Leaders at All Levels》(2014) —— 〔一手·本人著作〕
- 长访谈：Liker 谈第二版为什么要重写（Lean Blog 第 400 期播客，含文字稿） —— 〔二手·播客媒体〕 https://www.leanblog.org/2021/02/s1e400-jeff-liker-on-the-second-edition-of-the-toyota-way/

**值得读 / 听 / 看的 3 件事**

1. **《The Toyota Way》第二版（2021），不是 2004 版**。第二版的改动本身就是最有信息量的部分：他把重心从「14 条原则」移到**科学思维（scientific thinking）而非工具**，吸收了 Rother 的 Toyota Kata，扩写了 **Hoshin Kanri（方针管理）**，加进了服务业与医疗案例，并重构了领导力模型。也就是说，写出「精益工具圣经」的人，十七年后自己说重点不是工具。
2. 《Toyota Under Fire》—— 2009-2010 年丰田大规模召回危机的内部视角。这本书最有价值的地方在于它是一次**对自己研究对象的压力测试**：如果丰田真那么好，为什么会出这事？Liker 的回答（增长过快超出了培养人的速度）比结论本身更值得学。
3. Lean Blog 第 400 期的长访谈 —— 听他亲口讲第一版哪里被误读了。

**争议 / 非主流立场**

- **他被批评「离丰田太近」**：Liker 长期与丰田及其供应商合作、获多次 Shingo Award，批评者认为他的叙述接近官方口径，对丰田的阴暗面（供应商压价、日本国内的严苛工时、海外工厂与本土的落差）着墨不足。《Toyota Under Fire》被一部分人视为辩护书而非批判。
- **「文化可以被移植」vs.「文化不可移植」**：Liker 的核心主张之一是丰田模式**可以**在非日本、非汽车的组织里建立（他花了两本书讲怎么培养精益领导者）；Rother 与相当一部分实践者认为 14 条原则是**对结果的描述**，照着结果清单去建设，是典型的因果倒置。Liker 在第二版里部分吸收了这个批评。
- **对「精益 = 裁员」的立场**：他一贯坚持长期雇用是 4P 里 People 那一层的前提，没有雇用安全感就没有人会暴露问题；这使他与把精益当成本削减工具的咨询实践公开对立。
- **对丰田电动化转型的判断**：近年丰田在纯电动车上的保守路线（押注混动与多路径）被资本市场长期批评；Liker 属于少数公开为丰田这一决策的**方法论**辩护的学者（认为这是长期理念与实证决策的体现），这是他当前最有争议的立场。

**最近 12 个月动态.** 已从密歇根大学荣休，仍以顾问与作者身份活跃（Liker Lean Advisors 体系），近年输出集中在精益领导力培养与丰田在电动化/智能化转型中的管理体系论述；《The Toyota Way》第二版（2021）仍是其立场的最新完整表述。

### 05 · Steven J. Spear — 「丰田不是有一套好流程，是有一套不断做实验的方法」

**核心一句话.** 「丰田工厂里每一个动作、每一次交接、每一条流路都被写死到近乎僵硬——恰恰因为写死了，任何偏离都立刻可见，于是整个工厂变成一台连续做受控实验的机器。刚性是柔性的前提。」

**为什么重要.** 1999 年他与 H. Kent Bowen 在《Harvard Business Review》发表《Decoding the DNA of the Toyota Production System》，基于对 40 多家工厂四年的实地研究。这篇文章解决了一个悖论：为什么丰田的规范极其严格，产出却极其灵活？答案是四条**未被言明的规则（tacit rules）**：所有工作在内容、顺序、时间、结果上必须高度规定；每一个客户-供应者连接必须直接、是非分明（yes/no）；每条产品与服务的流路必须简单直接；任何改进必须由**做这件事的人**、在**老师的指导下**、按**科学方法**进行。前三条让问题**立刻暴露**，第四条让问题**被就地解决**。这是对 TPS 最好的一次机理性解释——比任何工具清单都更接近「为什么」。

**代表作品 / 观点**

- 《Decoding the DNA of the Toyota Production System》(HBR, 1999-09, 与 H. Kent Bowen)，获 HBR 的 McKinsey Award —— 〔一手〕 https://hbr.org/1999/09/decoding-the-dna-of-the-toyota-production-system
- 《The High-Velocity Edge》（原名《Chasing the Rabbit》，2009）—— 把丰田的机理推广到核潜艇（美国海军核动力项目）、Alcoa、医疗系统等高风险高速组织 —— 〔一手·本人著作〕
- **《Wiring the Winning Organization: Liberating Our Collective Greatness through Slowification, Simplification, and Amplification》(IT Revolution, 2023, 与 Gene Kim)** —— 获 Shingo Publication Award —— 〔一手·本人著作〕；出版社页 https://itrevolution.com/product/wiring-the-winning-organization/ ；获奖公告（Utah State University / Shingo Institute 官方） https://www.usu.edu/today/story/gene-kim-and-steven-j-spear-earn-shingo-publication-award-for-wiring-the-winning-organization
- MIT Sloan 官方教员页（现任高级讲师；同时是 Institute for Healthcare Improvement 高级研究员） —— 〔一手〕 https://mitsloan.mit.edu/faculty/directory/steven-spear
- MIT Sloan 官方对新书核心机制的解读文章 —— 〔一手·所属机构〕 https://mitsloan.mit.edu/ideas-made-to-matter/how-to-wire-your-organization-to-excel-problem-solving
- MIT Industrial Liaison Program 的相关条目 —— 〔一手·所属机构〕 https://ilp.mit.edu/node/64085
- 长访谈（Lean Blog，2023，与 Gene Kim 同场） —— 〔二手·播客媒体〕 https://www.leanblog.org/2023/11/gene-kim-and-steve-spear-discussing-wiring-the-winning-organization/

**值得读 / 听 / 看的 3 件事**

1. **《Decoding the DNA of the Toyota Production System》原文**（15 页）—— 这套 OS 里性价比最高的一次阅读。读的时候重点看它举的**反例**：一家自称做了精益的工厂，看板齐全、5S 干净，但没有任何一条规则被满足，所以问题从不暴露。这是识别「假精益」最锋利的一把尺。
2. 《The High-Velocity Edge》—— 尤其海军核动力（Rickover 体系）那部分。他要证明的是：TPS 的机理与汽车无关，与**高风险复杂系统里如何积累知识**有关。这本书让 TPS 的适用范围从工厂扩展到医院、航空、软件。
3. 《Wiring the Winning Organization》—— 他最新的抽象层：**slowification（把问题从高压现场挪到低压场景解决）、simplification（把大问题切成可独立处理的小块）、amplification（让问题的信号响到不可能被忽略）**。这是四条规则的第三代表述，也是他向软件/DevOps 世界的正式接口（与 Gene Kim 合著即是明证）。

**争议 / 非主流立场**

- **「所有失败的精益，都是因为抄了做法没抄机理」**：他的四条规则是**元规则**，不指定任何工具。这在实践上意味着：一家没有看板、没有 andon 灯的公司可以是精益的，一家两样俱全的公司可以完全不是。这个立场让大量以工具审计为业的咨询与认证体系尴尬。
- **「刚性产生柔性」是反直觉的核心主张**：主流管理话语推崇授权、灵活、少约束；Spear 说没有严格规定就没有基线，没有基线就检测不到偏离，检测不到偏离就无法学习。这与敏捷/自组织话语正面冲突（虽然他后来与 Gene Kim 合作，把它翻译成了 DevOps 能接受的语言）。
- **对医疗行业的严厉判断**：他长期在医疗系统做研究（IHI 高级研究员），公开主张医疗差错主要不是个人能力问题而是**系统未被设计成能暴露问题**，并批评医院的「不追责文化」在没有配套的问题暴露机制时只是纵容。这在医疗质量圈子里争议不小。
- **与工厂物理学派的分歧**：Spear 的框架里几乎没有数学。Hopp/Spearman 会说他描述的是组织学习机制而非系统行为定律，无法预测产能与交期；Spear 一派会说定律告诉你上限在哪，但不告诉你一群人怎样每天逼近上限——两者其实互补，但从不互相引用。

**最近 12 个月动态.** 仍任 MIT Sloan 高级讲师，重心在《Wiring the Winning Organization》体系的传播与在医疗、软件组织中的应用；该书已获 Shingo Publication Award，是他把 TPS 机理推向非制造业的最新一次尝试。

### 06 · Mike Rother — 从「画图」到「练招式」：把改善变成可训练的科学思维

**核心一句话.** 「你复制不了丰田的解，因为解是丰田在它自己的路上逐次试出来的；你能复制的只有它试的方式。」——所以他把改善从「找出浪费」重新定义为「在不确定中用科学方法逼近一个目标状态」。

**两次转向，一个人.** 1999 年他与 John Shook 合著《Learning to See》，把 value stream mapping（价值流图）交到全世界工程师手里，这本书是精益工具化浪潮的引爆点之一。十年后他自己成了这股浪潮最严厉的批评者：2009 年的《Toyota Kata》公开说，画图和照搬工具解释不了丰田的持续力，真正的机制是一套每天重复的行为套路——Improvement Kata（设定挑战 → 把握现状 → 定下一个目标状态 → 逐个撞障碍）和 Coaching Kata（上级用固定五问带下级练）。

**代表作品 / 观点**

- 《Learning to See: Value Stream Mapping to Add Value and Eliminate MUDA》(1999, 与 John Shook)，LEI 出版 —— 〔一手〕（LEI 为作者所属机构出版）https://www.lean.org/store/book/learning-to-see/
- 《Creating Continuous Flow》(2001, 与 Rick Harris) —— 〔一手〕
- 《Toyota Kata: Managing People for Improvement, Adaptiveness and Superior Results》(2009, McGraw-Hill) —— 〔一手〕
- 《The Toyota Kata Practice Guide》(2017) 与《Toyota Kata Culture》(2017, 与 Gerd Aulinger) —— 〔一手〕
- 作者本人维护的免费资料站（Improvement Kata Handbook、幻灯片、练习卡，全部可下载） —— 〔一手〕 http://www-personal.umich.edu/~mrother/Homepage.html
- 二手概览与书目核对 —— 〔二手〕 https://en.wikipedia.org/wiki/Toyota_Kata

**值得读 / 听 / 看的 3 件事**

1. 《Toyota Kata》全书 —— 尤其第 1 部分（丰田到底在管什么）与第 3 部分（Coaching Kata 的五问）。这本书回答了《Learning to See》回答不了的问题。
2. 他本人站点上免费放出的 **Improvement Kata Handbook** —— 这是极罕见的「作者把自己书的可执行部分免费开源」，直接可用于车间。〔一手〕
3. 《The Toyota Kata Practice Guide》—— 如果你只想要「明天早上怎么做」，读这本，不读 2009 那本。

**争议 / 非主流立场**

- **他公开反对自己成名的东西**：Rother 认为西方的精益推行大面积失败，根因是把 TPS 当「最佳实践清单」抄，而 TPS 是一套「在未知里前进的方法」。价值流图只是描述现状的工具，本身不产生能力。这在精益咨询业里等于砸自家招牌。
- **「持续改进不是文化问题，是练习问题」**：主流说法是「要先建立改善文化」，Rother 说这是因果倒置——行为套路反复练到自动化之后，文化是它的副产品。他要求的是像练琴一样每天 20 分钟的刻意重复，很多管理者接受不了这种「幼稚」的形式化。
- **反对目标管理式的 KPI 驱动改善**：Kata 的核心是「目标状态（target condition）」而非「目标数字（target）」——前者描述流程应该怎么运转，后者只描述结果。他认为 KPI 驱动必然导致造假与局部优化。
- **与 TOC 的暗线冲突**：Kata 假设瓶颈与障碍是逐次涌现、不可预知的，所以只能试；TOC 假设瓶颈可被识别并集中攻击。两者对「你到底知不知道该改哪」的判断相反。

**最近 12 个月动态.** Rother 现已入选 Association for Manufacturing Excellence (AME) Hall of Fame，主要产出形态从新书转为线上工作坊与自有站点的免费资料迭代；Toyota Kata 的社群化承载体是每年的 KataCon 与各国 Kata 实践者网络，不再由他一人推动。

### 07 · Eliyahu M. Goldratt（1947–2011）— 「系统的产出只由一个环节决定，其余全是噪音」

**核心一句话.** 「任何系统的产出都受限于极少数（通常是一个）约束；在约束之外做的任何改善都是幻觉——它不增加产出，只增加库存和自我感觉。」

**为什么重要.** Goldratt 是物理学家出身（这一点决定了他的全部风格：找那条支配方程，其余忽略）。他做了三件在管理学里罕见的事：(1) 用**小说**（《The Goal》，1984）而不是教科书传播方法；(2) 提出一套刺刀见红的**替代会计口径**——Throughput（有效产出）/ Inventory（库存）/ Operating Expense（运营费用），直接对抗成本会计的「局部效率」；(3) 给出一个可执行的循环：**五步聚焦法（Five Focusing Steps）**——识别约束 → 最大化利用约束 → 让其余一切迁就约束 → 提升约束 → 约束被打破后回到第一步，别让惰性成为新约束。生产排程上对应 **Drum-Buffer-Rope（鼓-缓冲-绳）**：鼓是瓶颈的节拍，缓冲保护瓶颈不断料，绳把投料速度绑在瓶颈上。项目管理上对应 **Critical Chain（关键链）**。

**代表作品 / 观点**

- 《The Goal: A Process of Ongoing Improvement》(1984) —— 商业小说，运营管理领域销量最大的书 —— 〔一手·本人著作〕
- 《It's Not Luck》(1994)、《Critical Chain》(1997)、《The Haystack Syndrome》(1990)、《Theory of Constraints》(1990) —— 〔一手·本人著作〕
- **《Standing on the Shoulders of Giants: Production concepts versus production applications — The Hitachi Tool Engineering example》(2008)** —— 他晚年最重要、也最有攻击性的一篇论文，见下 —— 〔一手·本人论文〕；学术期刊版（Gestão & Produção, SciELO）https://www.scielo.br/j/gp/a/nw43nPSMWtFFqr4x5jhJkJn/?lang=en ；全文 PDF（政府机构托管）https://businesswales.gov.wales/sites/main/files/documents/Standing-on-the-Shoulders-of-Giants.pdf
- Dr. Eliyahu M. Goldratt Foundation（其遗产与研究资助机构，挂靠 TOCICO） —— 〔一手·本人遗产机构〕 https://www.tocico.org/mpage/goldratt_foundation
- TOCICO 收录的 Goldratt「What is TOC」原始材料 —— 〔一手·协会〕 https://www.tocico.org/page/EliyahuGoldrattWhatisTOC
- Goldratt Foundation 授权的会议材料（TOC 与 TPS 的关系讨论） —— 〔一手·协会/基金会〕 https://cdn.ymaws.com/www.tocico.org/resource/resmgr/2012_foundation_pdfs/kohls,_kevin_final_toc_&_tmp.pdf
- Goldratt Consulting / Goldratt Group 官方站点（他本人创办的咨询机构，goldratt.com 现重定向至此；设有 Goldratt House——「TOC 的活体中心，其创立者最后的工作场所」） —— 〔一手·本人创办机构〕 http://goldrattgroup.com/
- 学术界对 TOC 的系统性文献回顾（用于校正他本人的自述） —— 〔二手〕 https://en.wikipedia.org/wiki/Theory_of_constraints

**值得读 / 听 / 看的 3 件事**

1. **《Standing on the Shoulders of Giants》(2008)** —— 如果只读一篇，读这篇，不是《The Goal》。他在文中把 Ford、大野耐一和自己放在同一条线上：三人遵循的是同一组「流」的原则，只是**环境不同导致应用不同**。他的核心论断是：福特用**空间**限制在制品（传送带的物理长度），大野用**库存量**限制在制品（看板数量），而这两种机制都要求**环境相对稳定**；在 Hitachi Tool Engineering 那种品种多、需求波动大、工序时间不稳的环境里，精益实施失败不是因为执行不力，而是**方法的前提条件不成立**。TOC 用**时间缓冲**替代空间/数量缓冲，因此不受这个前提约束。这是对精益最有分量的一次学理攻击。
2. 《The Goal》—— 读它是为了理解**为什么它有效**：Goldratt 明白管理者不接受「你错了」，只接受「你也可以像 Alex Rogo 一样自己想明白」。这是方法传播史上的一次范式创新。
3. 《The Haystack Syndrome》—— 讲 Throughput Accounting 的那本，是他攻击成本会计最系统的表达，也是最少人读完的一本。

**争议 / 非主流立场**

- **对精益最著名的嘲讽**：TOC 圈广为流传的表述是，精益让你**降低库存，然后等问题（浪费）自己浮出水面**——Goldratt 认为这是把系统的诊断权交给运气与时间，而 TOC 是**直接指出问题在哪**（约束），不用等。精益方面的回应是：约束会漂移、会被误认，而且大量真实工厂的瓶颈是**由策略造成的（policy constraint）**而非物理设备，指认往往指错。
- **对成本会计的全面否定**：他认为「产品成本」在多工序共享资源的系统里是**不存在的东西**，用它做决策必然错。这一立场至今未被主流会计与 ERP 采纳，是 TOC 无法进入财务语言体系的根本原因。
- **DBR 的核心假设被质疑**：Drum-Buffer-Rope 假设约束**相对稳定、可识别**。在真实的多品种小批量车间里，瓶颈随产品组合漂移（wandering bottleneck），此时 DBR 的鼓点会不断重设，收益急剧下降。后来的 Simplified DBR（S-DBR）就是对这个批评的回应。工厂物理学派进一步说，TOC 的排程结论可以直接由排队论定律推出，是**特例而非新理论**。
- **风格上的树敌**：Goldratt 公开表示学界对 TOC 的实证研究「大多问错了问题」，并长期与咨询同行、软件厂商冲突。他的方法论传播依赖个人权威与认证体系，而非同行评议——这既是 TOC 扩散快的原因，也是它在学术界地位不稳的原因。
- **与 DDMRP 的血缘**：DDMRP 的缓冲管理直接继承自 TOC，但把缓冲从「约束前」搬到「解耦点」，等于承认在多层 BOM 的复杂供应链里，单一约束的模型不够用了。这是 TOC 内部最重要的一次分化。

**其思想的当代承载机构 / 传人.** TOCICO（Theory of Constraints International Certification Organization，认证与知识体系的守护者）与挂靠其下的 Dr. Eliyahu M. Goldratt Foundation；商业实施侧由 Goldratt Consulting / Goldratt Group（goldrattgroup.com，业务分 Innovation / Strategy / Operational Excellence / Training 四块，并设 Goldratt House 作为 TOC 的实体中心）及各国 TOC 咨询机构承载。方法本身已扩散进项目管理（Critical Chain，被 PMI 体系部分吸收）与零售补货（TOC replenishment）。

### 08 · W. Edwards Deming（1900–1993）— 「你的员工不是问题，你的系统才是」

**核心一句话.** 「94% 的麻烦与改进机会属于系统，属于管理层的责任；只有 6% 属于个人。」（《Out of the Crisis》第 315 页）——这句话是他全部主张的压缩包：**只要你还在考核个人，你就没在管理系统。**

**为什么他属于供应链而不只是质量.** Deming 提供的是这套运营 OS 的**认识论层**：在你判断任何一个数字（本月交付率下降、这条线良率波动、这个供应商延迟）之前，你必须先回答一个问题——这是**系统固有的共同原因变异（common cause）**，还是**特殊原因（special cause）**？答错了这一步，后面所有动作都是有害的：对共同原因做干预（tampering）会**放大**波动，这就是他用漏斗实验（funnel experiment）演示的东西；而对特殊原因不追根因，则永远解决不了问题。所有做需求计划、库存策略、供应商绩效的人，每天都在犯这个错。

**代表作品 / 观点**

- The W. Edwards Deming Institute（他 1993 年亲手创办的非营利机构，是其思想的法定承载者） —— 〔一手·本人创办机构〕 https://deming.org/
- 《Out of the Crisis》(MIT CAES, 1982/1986)、《The New Economics for Industry, Government, Education》(1993) —— 〔一手·本人著作〕
- **System of Profound Knowledge™（渊博知识体系）**：系统观（appreciation for a system）、变异知识（knowledge about variation）、知识理论（theory of knowledge）、心理学 —— 四者缺一不可 —— 〔一手〕 https://deming.org/explore/red-bead-experiment/
- **Red Bead Experiment（红珠实验）** 官方页与影像 —— 〔一手〕 https://deming.org/deming-red-bead-experiment/ ；https://deming.org/lessons-from-the-red-bead-experiment-with-dr-deming/
- Deming 本人讲 14 点的原始影像（Deming Library） —— 〔一手·本人影像〕 https://deming.org/deming-library-video-with-dr-deming-discussing-the-14-points/
- 视频资料总入口 —— 〔一手〕 https://deming.org/w-edwards-deming-videos-on-demand/
- 红珠实验的学术整理（教学用，可作为交叉印证） —— 〔二手〕 https://maaw.info/DemingsRedbeads.htm

**值得读 / 听 / 看的 3 件事**

1. **Red Bead Experiment 的原始录像**（不是文字转述）—— 六个「志愿工人」用同一把勺子从同一桶珠子里舀，产出的红珠数必然不同；「厂长」照着这个差异做奖惩、贴光荣榜、开除末位，全程荒谬。看完你会永远无法直视一张供应商绩效排名表。这是全套材料里最值得投入的 40 分钟。
2. 《Out of the Crisis》的「Seven Deadly Diseases（七大恶疾）」与「14 Points」——尤其第 4 点：**停止以价格为唯一标准做采购决策，转向与单一供应商建立长期忠诚与信任关系**。这是供应链专业里最被引用也最被违反的一条。
3. 《The New Economics》第 4 章 System of Profound Knowledge —— 他晚年把 14 点收敛成的理论内核，比 14 点更本质。

**争议 / 非主流立场**

- **废除绩效考核、目标管理与年度评级**：14 点里的第 11、12 点直接要求取消数量指标（quotas）、取消 MBO、取消年度绩效评级。这在今天任何一家公司都近乎不可执行，也是 Deming 被引用最多、执行最少的部分。
- **反对 Six Sigma 的正统解释**：Deming 本人在世时未评价 Six Sigma（1993 年去世，Six Sigma 1986 年起于 Motorola、1995 年经 GE 大规模化），但 Deming 学派与 Six Sigma 阵营长期互相不认账：Deming 派认为 Six Sigma 的「黑带项目 + 财务收益挂钩」是把改进重新包装成个人绩效游戏，恰恰违背了系统观；Six Sigma 派认为 Deming 只有哲学、没有可部署的项目方法论。
- **反对「零缺陷」口号**：14 点第 10 点明确要求「消除对员工的口号、劝诫和目标」，因为口号把责任推给工人而不改变系统——这和新乡重夫的 Zero Quality Control **在口号层面对立、在机制层面其实同盟**（两人都反对靠人小心）。但新乡反对统计抽样，Deming 认为不懂统计就不配谈改进——这是真正的裂缝。
- **对日本奇迹的归因争议**：主流叙事说 Deming 教会了战后日本质量管理（日本科学技术连盟 JUSE 以他命名戴明奖）；批评者认为这一叙事被美国方面放大，日本本土的 TQC/CWQC 发展有其独立脉络（石川馨、田口玄一等）。

**其思想的当代承载机构 / 传人.** The W. Edwards Deming Institute（deming.org，本人 1993 年创办）是唯一的法定承载者，持有 System of Profound Knowledge™ 与红珠/漏斗实验的官方材料；统计过程控制这条线的当代最尖锐继承者是 Donald J. Wheeler（见下一条）。

### 09 · Donald J. Wheeler — 统计派内部的持刀者：「六西格玛的那个 1.5σ 位移，站不住脚」

**核心一句话.** 「在你判断一个过程好不好之前，先回答它是不是**可预测（predictable）**的。对不可预测的过程谈能力指数、谈 DPMO、谈 sigma level，全是把数字算给自己看。」

**为什么在这份名单里.** Deming 给了「共同原因 vs 特殊原因」的哲学，Wheeler 是把它变成日常可操作工具、并且**用它去打六西格玛正统**的人。他坚持把 control chart 叫作 **process behavior chart（过程行为图）**——因为它的用途不是「控制」，是**判断这个过程的行为是否稳定**。他是 SPC Press 的核心作者，长期在《Quality Digest》写专栏。任何做供应商质量、良率管理、交付准时率追踪的人，他的那套判断法是最低成本的防蠢工具：一张过程行为图能立刻告诉你，这个月的波动值不值得开会。

**代表作品 / 观点**

- 《Understanding Variation: The Key to Managing Chaos》(2nd ed.) —— 一百多页，是这套 OS 里最短、最该先读的统计书 —— 〔一手·本人著作〕
- 《Understanding Statistical Process Control》(3rd ed., 与 David S. Chambers) —— 完整技术版 —— 〔一手·本人著作〕
- **《The Six-Sigma Zone》(Manuscript No. 177)** —— 他对 1.5σ 位移的正式拆解 —— 〔一手·本人论文〕 https://www.spcpress.com/pdf/DJW177.pdf
- SPC Press 上他的全部文章索引（数百篇，免费） —— 〔一手·本人出版渠道〕 https://www.spcpress.com/djw_articles.php
- 研讨班资料 —— 〔一手·本人站点〕 https://www.spcpress.com/seminars.php
- 《The Problem With Sigma Levels》(Quality Digest, 2026-03-26)，本人署名专栏 —— 〔一手·本人专栏〕 https://www.qualitydigest.com/inside/statistics-article/problem-sigma-levels-032626.html
- 1.5σ 位移在临床检验领域被要求提供证据的学术论文（第三方对同一争议的独立检视） —— 〔一手·学术〕 https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6999184/
- 六西格玛阵营对 1.5σ 位移的标准解释（用于看清对立面怎么说） —— 〔二手·行业站〕 https://www.isixsigma.com/dmaic-methodology/15-sigma-process-shift/
- 其 USPC 研讨班的第三方笔记 —— 〔二手〕 https://www.leansixsigmadefinition.com/summary-of-donald-wheelers-understanding-statistical-process-control-uspc-seminar/

**值得读 / 听 / 看的 3 件事**

1. 《Understanding Variation》全书 —— 两三个小时能读完，回报极高。核心训练是：拿到任何一列月度数字，先画图看它是不是可预测，再决定要不要解释它。绝大多数管理会议上的「同比下降 3%」根本不值得解释。
2. 《The Six-Sigma Zone》—— 他把 1.5σ 位移的来龙去脉拆开：这个数字原本是 Motorola 内部做设计仿真时用的一个测试值，后来被当成「所有过程漂移的最坏情况」写进了 sigma level 与 DPMO 的换算表。他的判断是：**「假设一个不可预测的过程漂移不会超过 1.5σ，是完全站不住脚的」**——不可预测意味着你不知道它会漂多远，这正是「不可预测」的定义。
3. SPC Press 上他的文章索引 —— 免费、量大、按主题组织。任何一个具体的统计困惑（要不要剔除异常点、样本量多大、能力指数怎么算）都能在里面找到一篇短文。

**争议 / 非主流立场**

- **直接攻击六西格玛的度量基础**：sigma level 与 DPMO 的换算依赖 1.5σ 位移假设 + 正态分布假设，两者他都认为不可辩护；他指出 sigma level 的估计跨越九个数量级，导致不合格品率的估计根本不可靠。这在一个以 sigma level 为品牌名的方法论面前，是掀桌子级别的批评。
- **反对「先做正态性检验」**：主流教科书要求先验证数据服从正态分布再用控制图；Wheeler 用大量实证主张过程行为图对分布形态**极其稳健**，正态性检验反而会把人引向错误的复杂化。这是 SPC 圈子里的长期论战。
- **反对能力指数（Cp/Cpk）的滥用**：他的立场是过程不可预测时能力指数没有意义，因为它描述的是一个不存在的稳定状态。而现实中绝大多数 Cpk 报告来自不可预测的过程。
- **与新乡重夫的对立**：新乡认为统计抽样从设计上就接受不良、应当被 poka-yoke 取代；Wheeler 认为不理解变异就无法判断该改什么，防错装置解决的是可被防错的错误，解决不了过程本身的漂移。两人各自击中对方的盲区。
- **他不属于任何咨询体系**：没有认证、没有黑带、没有方法论品牌——这既是他保持攻击性的原因，也是他影响力远小于六西格玛体系的原因。

**最近 12 个月动态.** 仍在持续产出：2026 年 3 月 26 日于《Quality Digest》发表《The Problem With Sigma Levels》，延续其对 sigma level 被系统性误读的批评（一手核实：文章署名 Donald J. Wheeler，日期 2026-03-26）。SPC Press 仍是其著作与文章的宿主。

### 10 · Wallace J. Hopp & Mark L. Spearman — 「精益和 TOC 都是同一组定律的特例」

**核心一句话.** 「制造系统的行为不由管理哲学决定，由**数学定律**决定：Little's Law、变异传播、容量-在制品-周期时间之间的权衡。所有有效的方法之所以有效，是因为它们碰巧遵守了这些定律；所有失效的实施，是因为它们违反了定律而不自知。」

**为什么重要.** 1996 年的《Factory Physics: Foundations of Manufacturing Management》做了一件在当时几乎没人做的事：**不讲哲学，讲定律**。它把 MRP、JIT、TOC、六西格玛全部放进同一个分析框架里，逐一说明各自在什么条件下成立。核心积木包括：
- **Little's Law**：WIP = Throughput × Cycle Time。三者只能定两个，第三个是结果——这一条就足以证伪大量「既要短交期又要高稼动率又不许增加在制品」的管理要求。
- **变异定律（Variability Law / Buffering Law）**：系统里的变异**必然**被三种缓冲之一吸收——**库存、产能、时间（交期）**。你不能消灭变异的影响，只能选择用哪种缓冲付账。这是全书最有力的一条判断工具：任何一个运营决策，都可以问「你在用哪种缓冲，代价是谁承担」。
- **拥塞与稼动率的非线性**：稼动率趋近 100% 时，周期时间趋向无穷。所以「设备开动率越高越好」在数学上是错的。
- **CONWIP（Constant Work In Process）**：Spearman 与 Zazanis 提出的推拉混合机制——他们证明，看板的好处主要来自**在制品被封顶**这个事实，而不是来自「处处拉动」这个仪式；因此一个覆盖整条线的总量上限（CONWIP）可以在更一般的环境里拿到同样的好处。

**代表作品 / 观点**

- 《Factory Physics》(1996；3rd Edition, Waveland Press) —— 〔一手·本人著作〕；出版社官方页 https://www.waveland.com/browse.php?t=587
- **《To Pull or Not to Pull: What Is the Question?》(Manufacturing & Service Operations Management, 2004, 6(2):133–148)** —— 本条最重要的一篇，见下 —— 〔一手·学术论文〕；.edu 托管全文 https://www2.isye.gatech.edu/~jvandeva/Classes/6203/2007/PushPull.pdf ；机构转载 https://projectproduction.org/journal/reprint-to-pull-or-not-to-pull-what-is-the-question/
- 《Factory Physics for Managers: How Leaders Improve Performance in a **Post-Lean Six Sigma** World》(Pound, Bell & Spearman, McGraw-Hill, 2014) —— 副标题本身就是宣战 —— 〔一手·本人著作〕；出版社技术库页 https://www.accessengineeringlibrary.com/content/book/9780071822503
- CONWIP 机制说明与文献索引 —— 〔二手〕 https://en.wikipedia.org/wiki/CONWIP
- 《Factory Physics》一书的结构与定位（三部分：basics / intuition / synthesis） —— 〔二手〕 https://en.wikipedia.org/wiki/Factory_Physics
- 「To Pull or Not to Pull」的后续学术讨论（POMS 会议论文，「概念在翻译中丢失了吗」） —— 〔一手·学会会议论文〕 https://pomsmeetings.org/confpapers/051/051-1344.pdf
- Factory Physics 方法的官方站点（Factory Physics® 现为 Strategic Project Solutions, Inc. 注册商标；提供 digital twin 诊断工具、认证教育与书目，含 Hopp 的《Supply Chain Science》） —— 〔一手·方法创立方站点〕 https://www.factoryphysics.com/

**值得读 / 听 / 看的 3 件事**

1. **《To Pull or Not to Pull: What Is the Question?》** —— 不到 20 页，是本领域最锋利的一次概念清洗。他们的论断：**pull 的定义不是「按需求触发生产」，而是「显式地给在制品设上限」**；push 是「按计划投料，在制品无上限」。按这个定义，很多自称做 pull 的系统其实是 push，而很多被骂成 push 的 MRP 加个 WIP 上限就变成了 pull。他们进一步说：**lean 的本质是「用最低成本吸收变异的缓冲」**——不是消灭浪费，是**买最便宜的缓冲**。
2. 《Factory Physics》第 II 部分（intuition）—— 尤其变异缓冲定律那几章。这是全书里最值得记住的部分，而且不需要读懂公式也能用。
3. 《Factory Physics for Managers》—— 如果你不做数学，读这本。副标题「Post-Lean Six Sigma World」就是他们的立场声明：精益与六西格玛已经过了它们的历史时刻，需要一个能解释它们为何有时有效有时无效的更底层框架。

**争议 / 非主流立场**

- **对精益的降维打击**：他们不说精益错，说精益是**特例**。精益的所有做法（小批量、拉动、快速换模、平准化）都可以从变异与排队论定律推导出来，而定律还能告诉你**什么时候不该那么做**——精益本身做不到这一点，因为它的表述是规范性（应该消除浪费）而非条件性的。
- **对 TOC 的同样处理**：约束理论的五步聚焦在他们看来是「容量约束下的最优化」的一个直觉版本，DBR 是一种带 WIP 上限的投料策略；TOC 的贡献是传播力，不是理论新意。
- **对六西格玛的批评**：把变异当成需要被消灭的敌人是错的，**变异永远消灭不完，关键是决定用哪种缓冲吸收它**；把所有资源投进降低变异，往往不如用同样的钱买一点产能缓冲。这一条直接冲撞六西格玛的方法论根基。
- **「零库存」是伪目标**：既然变异必须被三种缓冲之一吸收，把库存压到零只意味着变异会跑去时间（交期变长）或产能（备用产能成本）。因此「零库存」不是好坏问题，是**记账位置转移**问题。
- **他们自己被反批评的地方**：批评者指出，Factory Physics 的定律主要刻画**稳态、单一产品族、机器为中心**的车间，对多层供应网络、需求端行为、供应商关系与人的因素几乎无话可说；把它当成完整的运营 OS 会丢掉精益里关于**人与学习**的那一半（Rother、Spear 的领域）。定律告诉你物理上限在哪，不告诉你怎么让一群人每天逼近它。

**最近 12 个月动态.** Hopp 长期任教于密歇根大学（Ross School of Business / 工业与运营工程），研究已扩展到医疗运营与服务系统；Spearman 从学界转向实业，Factory Physics® 现由 Strategic Project Solutions, Inc. 持有商标并运营（官网 2026 年仍在更新），主要形态已从书变成**数字孪生（digital twin）式的运营诊断与产能/在制品仿真工具**加认证教育；书目线上另有 Hopp 的《Supply Chain Science》作为 Factory Physics 的精简版。方法本身已被大量 APS（高级排程）与 IBP（集成业务计划）产品吸收为底层假设。

### 11 · Carol Ptak & Chad Smith — DDMRP：宣布 MRP 的确定性假设已经死了

**核心一句话.** 「MRP 是 1960 年代为『需求可预测、提前期稳定、BOM 不变』的世界设计的；今天这三条全不成立，所以 MRP 的问题不是参数没调好，是它的世界观过期了。」他们的解不是更准的预测，而是**在关键位置放战略性库存缓冲，把长链切成几段解耦的短链**（decoupling），让波动在缓冲处被吸收而不是沿 BOM 逐级放大。

**为什么重要.** 这是极少数「敢直接改教科书」的流派：他们把 DDMRP 写进了 Joseph Orlicky 的经典《Material Requirements Planning》第 3 版（2011）与第 4 版（2023）——即接管了 MRP 正典本身的编者身份。Carol Ptak 曾任 APICS 主席（2000 年），Chad Smith 出身 TOC 咨询体系；DDMRP 因此是 TOC 缓冲思想 + MRP 数据结构 + 精益拉动的一次杂交。2011 年他们成立 Demand Driven Institute（DDI）作为方法的宿主机构。

**代表作品 / 观点**

- Demand Driven Institute 官方机构自述与方法定位 —— 〔一手〕 https://www.demanddriveninstitute.com/about-us
- 《Orlicky's Material Requirements Planning》3/E (2011) 与 4/E (2023)，Ptak & Smith 为改版编者 —— 〔一手〕（DDI 官方书目页）
- 《Demand Driven Material Requirements Planning (DDMRP) V3》(2019) —— 方法的规范文本 —— 〔一手〕
- 《Precisely Wrong》(2017) —— 书名即立场：宁可大致正确，不要精确地错
- 《The Demand Driven Adaptive Enterprise》(2018)、《Adaptive Sales and Operations Planning》(2022) —— 把方法从物料层推到 S&OP 与战略层 —— 〔一手〕
- 《Demand Driven Performance – Using Smart Metrics》(2013) —— 攻击成本会计式绩效指标（吸收成本法逼着工厂多生产）
- 认证体系 Demand Driven Planner (DDP) / Demand Driven Leader (DDL)，与 ASCM 的 PDP 学分互认 —— 〔一手〕 https://www.demanddriveninstitute.com/demand-driven-planner-ddp ；https://www.demanddriveninstitute.com/demand-driven-leader-ddl
- 作者页与视频资料 —— 〔一手〕 https://www.demanddrivenmrp.com/meet-the-authors ；https://www.demanddrivenmrp.com/ddmrp-videos
- ASCM 分会公开的 DDMRP 课程说明（协会侧材料，可用于核对认证口径） —— 〔一手·协会〕 https://bc.ascm.org/meetinginfo.php?id=64&ts=1455916293

**值得读 / 听 / 看的 3 件事**

1. 《Orlicky's MRP 4/E》第 1-6 章 —— 读他们怎么在 Orlicky 的坟头上解释「Orlicky 本人如果活到今天会怎么改」。这是全书最好看的部分，也是方法合法性的全部来源。
2. 《Demand Driven Performance》—— 对「吸收成本法（absorption costing）导致过量生产」的攻击，比 DDMRP 本身更有普适价值，任何做工厂 KPI 的人都该读。
3. DDI 官方的 DDMRP 视频与方法规范页 —— 因为 DDMRP 已被大量 ERP 厂商包装成模块，先看原方，再看厂商版本。

**争议 / 非主流立场**

- **最尖锐的一条：他们说「提高预测精度」是死路。** 主流需求计划（demand planning）整个行业的存在理由就是把 forecast accuracy 做高；DDMRP 说在长尾、高品种的现实里，预测误差有一个不可压缩的下限，投钱在那上面的边际回报趋零，正确的做法是**降低对预测的依赖**（缩短「需要被预测的时间窗」）。这直接得罪了半个行业。
- **学术界的反击**：多篇运营管理论文指出 DDMRP 的缓冲计算规则（buffer profiles、平均日用量 × 提前期 × 变异系数）是**启发式（heuristic）而非最优解**，在若干情境下会被经典的 (s, S) 库存策略或 base-stock 策略稳稳打败；批评者说 DDMRP 是「好的工程实践包装成理论突破」。DDI 的回应是：最优解建立在参数已知的假设上，而现实中参数本身不可知。
- **与精益的紧张**：精益要「库存是万恶之源」，DDMRP 明确说**有些库存是资产**（战略性解耦库存），并要求把它放在 BOM 的特定层级。这在精益纯粹派看来是倒退回推式生产。
- **与 TOC 的血缘和分歧**：Chad Smith 出身 TOC，DDMRP 的缓冲管理（红黄绿）直接继承自 TOC 的 buffer management；但 TOC 把缓冲放在**约束前面**，DDMRP 把缓冲放在**解耦点**——两者对「系统的关键位置在哪」判断不同。
- **商业模式质疑**：方法 + 认证 + 软件合规标记（DDMRP compliant）三位一体，批评者认为这让 DDI 既当规则制定者又当裁判。

**最近 12 个月动态.** DDI 持续以 DDP / DDL / DDPP 认证与 ERP 厂商合规认证为主要输出形态，方法的规范文本仍以《Orlicky's MRP 4/E》(2023) 与 DDMRP V3 为准；Ptak 与 Smith 近年重心已从物料层的 DDMRP 上移到「Demand Driven Adaptive Enterprise」与 Adaptive S&OP，即把缓冲逻辑接到产销协同与战略回路上。

### 12 · Hau L. Lee — 牛鞭效应的解剖者，与「效率不等于优秀」的最早发难者

**核心一句话.** 「供应链里的需求放大不是人性贪婪造成的，是**理性的人在错误的信息结构里做的正确决策**造成的。」——牛鞭效应（bullwhip effect）有四个可被工程化消除的成因，不是道德问题。

**为什么重要.** Lee 是斯坦福 GSB 的 Thoma Professor of Operations, Information and Technology，供应链管理成为一门学科时最早的一批建构者。他与 V. Padmanabhan、Seungjin Whang 的 1997 年论文《Information Distortion in a Supply Chain: The Bullwhip Effect》在 2004 年被票选为 Management Science 创刊以来最有影响力的十篇论文之一。他把牛鞭归因为四条：需求信号处理（demand signal processing）、批量订货（order batching）、价格波动与促销（price fluctuation）、短缺博弈（rationing and shortage gaming）——每一条都有对应的制度性解法。

**代表作品 / 观点**

- 《Information Distortion in a Supply Chain: The Bullwhip Effect》(Management Science, 1997；2004 年 50 周年重刊) —— 〔一手·学术〕 https://pubsonline.informs.org/doi/pdf/10.1287/mnsc.1040.0305
- 《The Bullwhip Effect in Supply Chains》(Sloan Management Review, 1997) —— 面向管理者的版本 —— 〔一手·学术〕 https://www2.isye.gatech.edu/~jvandeva/Classes/6203/2006/TheBullWhipEffectinSCsLee.pdf
- 《The Triple-A Supply Chain》(Harvard Business Review, 2004；McKinsey Award 第二名) —— Agility / Adaptability / Alignment —— 〔一手〕 https://www.gsb.stanford.edu/faculty-research/publications/triple-supply-chain
- 斯坦福官方教员页（研究方向、在研项目、Value Chain Innovation Initiative） —— 〔一手〕 https://gsb.stanford.edu/faculty-research/faculty/hau-l-lee
- POMS 2021 的 Hau Lee 学术生涯致敬文集（可用作其思想脉络与影响力的结构化索引） —— 〔一手·学会〕 https://pomsmeetings.org/conf-2021/documents/Honoring-Hau-Lee-POMS-2021.pdf

**值得读 / 听 / 看的 3 件事**

1. 1997 年 Sloan Management Review 版的牛鞭论文 —— 全篇不到 20 页，四个成因 + 每个成因的对策表，是三十年来没被超越的运营诊断清单。
2. 《The Triple-A Supply Chain》—— 读它的正确方式是把它当**反驳文**：Lee 在文章开头直接说「速度快、成本低的供应链并不会带来持久优势」，这句话在 2004 年是异端。
3. 斯坦福 GSB 的 Value Chain Innovation Initiative 相关材料 —— 他后期把供应链问题接到可持续与发展中国家小农供应链上，这条线比牛鞭那条线更能看出他的判断方式。

**争议 / 非主流立场**

- **「效率型供应链是陷阱」**：Triple-A 的核心论断是——大多数公司拼命优化的成本与速度，恰恰不产生竞争优势，因为它们可被复制；真正稀缺的是三个 A。这个说法在精益/成本削减主导的年代属于逆流。
- **对 information sharing 万灵药的怀疑**：牛鞭的四因里只有一条能靠共享 POS 数据解决，另外三条（批量、促销、短缺博弈）是**激励结构问题**，共享数据不但无效，还可能因为下游知道上游要缺货而加剧抢单。这一点至今被大量「数据透明化」项目忽略。
- **与韧性派的分工线**：Lee 的框架里 adaptability 处理的是**结构性长期变化**（市场迁移、成本曲线变化），不是 Sheffi/Simchi-Levi 关心的**突发中断**。他明确反对把两者混为一谈——为地震准备和为需求结构迁移准备，是两套投资。
- **对促销（price fluctuation）的态度**：他实质上认为高低促销（Hi-Lo pricing）是自己给自己制造牛鞭，倾向 EDLP（everyday low price）。这在消费品行业是长期争议，销售端几乎不可能接受。

**最近 12 个月动态.** 仍任斯坦福 GSB 教席教授，学术输出重心在价值链创新（Value Chain Innovation Initiative）、社会责任与可持续供应链；官方教员页为其近况的权威口径。

### 13 · Yossi Sheffi — 韧性（resilience）不是买保险，是把中断变成竞争优势

**核心一句话.** 「你无法预测下一次中断是什么，所以别在预测上花钱；要花在**缩短探测时间和恢复时间**上——韧性是一种可以被工程化的组织能力。」

**为什么重要.** Sheffi 是 MIT Center for Transportation & Logistics (MIT CTL) 的主任，也是把「供应链韧性」从风险管理的边角料变成董事会议题的人。他的思路核心是把中断按「发生概率 × 影响」画到一张图上，但重点不是那张图，而是**恢复时间目标（time-to-recovery, TTR）**与**探测时间（detection window）**这两个可管理变量。他的一贯立场是：真正区分公司的不是有没有被打中，而是被打中之后的曲线形状。

**代表作品 / 观点**

- 《The Resilient Enterprise: Overcoming Vulnerability for Competitive Advantage》(MIT Press, 2005) —— 〔一手〕 https://sheffi.mit.edu/book/resilient-enterprise
- 《The Power of Resilience: How the Best Companies Manage the Unexpected》(MIT Press, 2015) —— 深层供应商（deep-tier）风险、网络安全、长期中断、应急指挥中心 —— 〔一手〕 https://sheffi.mit.edu/book/power-resilience
- 本人 MIT 官方站点（书目、文章、演讲全集） —— 〔一手〕 https://sheffi.mit.edu/
- 早期 MIT 个人页（《The Resilient Enterprise》专页） —— 〔一手〕 https://web.mit.edu/sheffi/www/resilientEnterprise.html
- 出版社官方书页 —— 〔二手·出版社〕 https://mitpress.mit.edu/9780262693493/the-resilient-enterprise/
- 面向从业者的长访谈（Supply Chain Management Review） —— 〔二手·媒体〕 https://www.scmr.com/article/the_power_of_resilience_a_qa_with_yossi_sheffi

**值得读 / 听 / 看的 3 件事**

1. 《The Power of Resilience》第 2-4 部分 —— 深层供应商风险那几章是全书最硬的部分：你的一级供应商没事，不代表你没事；2011 年日本地震后大量车企才发现自己的四级供应商是同一家。
2. 《The Resilient Enterprise》里的 Nokia vs. Ericsson 案例（2000 年 Philips 芯片厂火灾） —— 这是韧性文献的创世案例，一个厂着火，两家公司命运分岔。要读原书版本，不要读被转述二十手的段子版。
3. 他本人 MIT 站点上的文章与演讲档案 —— 相比书，他的短文更能看出判断在最近几年的迁移（从「为中断准备」到「为 AI 与劳动力结构变化准备」）。

**争议 / 非主流立场**

- **他反对「去全球化就是韧性」**：在疫情后 reshoring / 本土化成为政治正确时，Sheffi 一贯的立场是本土化只是把风险换了一种形态（把地缘风险换成集中度风险和成本风险），并不天然更韧。他对「囤库存 = 韧性」也持保留态度——库存只买来时间，不解决结构。
- **他不认为 JIT 是疫情断链的元凶**：这是供应链圈子里最激烈的一场争论。一派认为 just-in-time 把系统的所有缓冲都榨干了，所以一有扰动就散架；Sheffi 这一派认为，出问题的是**单一来源（single sourcing）和对深层供应商的无知**，而不是低库存本身——很多囤了大量库存的公司照样断供，因为他们囤错了东西。
- **韧性投资的悖论**：他直言韧性投入的回报是「没发生的事故」，这在财务上无法证明，所以韧性预算永远在灾后三个月最容易批、三年后最先被砍。他对企业能否长期维持韧性投入是悲观的。
- **对 AI 与自动化的立场偏乐观**：在多数人担心自动化削减岗位时，他的近期论述倾向于「技术改变任务而非消灭职业」，这在物流劳动力议题上属于少数派。

**最近 12 个月动态.** 仍任 MIT CTL 主任（该中心是他的机构载体），近年著作与文章重心从「中断韧性」转向 AI、自动化与供应链劳动力的未来；其 MIT 官方站点是核实其最新产出的权威入口。

### 14 · David Simchi-Levi — 把「你不知道自己有多脆」变成一个可算的数

**核心一句话.** 「不要去猜下一次中断的概率，那是猜不到的；去算**假设某个节点停了，你多久能恢复（TTR）、在这段时间里你能撑多久（TTS）、以及你会亏多少钱**——把风险从概率问题改写成影响问题。」

**为什么重要.** 这是韧性领域里最工程化的一支。Simchi-Levi（MIT，运筹与统计）与 Ford 从 2013 年开始合作，起因是 2011 年日本地震与泰国洪水暴露了一个事实：**车企对自己的深层供应商一无所知**。他们提出 **Risk Exposure Index (REI)**：不问「这个供应商出事的可能性多大」（数据根本不存在），而是给每个节点设一个 **time-to-recover (TTR)**，然后用优化模型算出如果它停摆 TTR 那么久，全网络的财务影响（performance impact）是多少。结果往往反直觉：**风险最高的节点常常是采购金额最小的那些**——一个几毛钱的零件可以停掉一条整车线。后来他又把这套方法扩展成 **time-to-survive (TTS)** 与 2020 年的「supply chain stress test（供应链压力测试）」。

**代表作品 / 观点**

- 《Find the Weak Link in Your Supply Chain》(Harvard Business Review, 2015) —— REI 面向管理者的正式表述 —— 〔一手〕 https://hbr.org/2015/06/find-the-weak-link-in-your-supply-chain
- MIT 官方对该研究被企业采用情况的报道（Ford 等） —— 〔一手·所属机构〕 https://news.mit.edu/2022/companies-use-mit-research-identify-respond-supply-chain-risks-0615
- 《Disruption Risk Mitigation in Supply Chains — The Risk Exposure Index Revisited》(Gao, Simchi-Levi, Teo, Yan) —— 方法的学术修订版 —— 〔一手·学术〕 https://www.ssrn.com/abstract=2875596 ；全文 https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=7218&context=lkcsb_research
- 生平与著作年表核对 —— 〔二手〕 https://en.wikipedia.org/wiki/David_Simchi-Levi
- 行业媒体对 REI 早期扩散的记录 —— 〔二手·媒体〕 https://www.scdigest.com/assets/on_target/13-04-24-1.php?cid=6971 ；https://www.scdigest.com/assets/newsviews/15-06-10-1.php?cid=9398

**值得读 / 听 / 看的 3 件事**

1. HBR 2015《Find the Weak Link in Your Supply Chain》—— 八页，把整套方法讲完，且带 Ford 的真实数字。这是过去二十年供应链风险领域最实用的一篇。
2. REI Revisited 那篇学术论文 —— 如果你要真的实现它，管理版讲不清楚约束条件；这篇讲清楚了模型形态与它的局限（单点中断假设、TTR 的估计误差）。
3. 他 2020 年 4 月在 INFORMS 关于疫情期间供应链恢复的公开演讲/文章 —— 这是「压力测试」概念第一次被用在一次真实的全球中断上。

**争议 / 非主流立场**

- **「概率不可知，所以别用概率」**：主流风险管理教你画 likelihood × impact 矩阵；他的立场是 likelihood 那一维在低频高损事件上根本估不出来，硬估只会带来虚假的精确。**只用 impact 维度**是他方法论上最大胆也最被质疑的简化（批评者说这会让你为极不可能的事过度投资）。
- **「采购额和风险无关」**：这条结论直接否定了绝大多数公司按支出（spend）分层管理供应商的做法。多数采购组织的组织结构就是按支出建的，所以这个结论在企业内部推行阻力极大。
- **单点中断假设的局限**：REI 的经典形式一次只让一个节点失效；疫情这种**全网同时受损**的情形超出了模型的原始设定，这也是 2020 年后他扩展到 stress test 的原因。批评者认为这暴露了方法的边界。
- **与 Sheffi 的分工与竞争**：同在 MIT，Sheffi 走的是组织能力与案例路线（探测时间、恢复文化、深层供应商可视化），Simchi-Levi 走的是优化模型路线。两人对「韧性能否被算出来」的信念不同——这是韧性派内部最主要的方法论分歧。

**最近 12 个月动态.** 仍在 MIT（工程系统 / 运筹中心）主持相关研究，近年方向已从纯风险模型扩展到需求预测、动态定价与「AI + 运筹」在供应链决策中的结合；MIT 官方新闻页是其成果被企业采用的权威记录入口。

### 15 · 刘宝红 Bob Liu — 中文圈里少数把「计划」讲成技术活而不是态度问题的人

**核心一句话.** 「高成本、高库存、重资产，根子不在采购砍价不够狠，在**需求预测、库存计划、供应链执行**这三道防线一道都没建起来。」——他把中国制造业与零售业的通病，从「供应商不给力 / 销售不靠谱」的归因，扭回到计划职能的能力缺失上。

**为什么在这份名单里.** 前面十四位定义了这套运营 OS，但他们的语境是欧美日的成熟制造体系。刘宝红的价值在于**语境转换**：他在北美做了十多年采购与供应链实践，回到中文语境后处理的是一批特定病灶——需求端极度不确定的电商/新零售、供应商管理靠关系而非流程、计划部门在组织里没有话语权、「小批量多品种」被当借口而不是设计约束。他的方法论不是原创流派，而是把 S&OP、安全库存、ABC 分类、供应商分层这些标准动作，翻译成中国企业能落地的版本。他的一手阵地是自己 2000 年代起经营的「供应链管理专栏」（scm-blog.com），据其自述已积累 600 多篇原创文章，书是文章的沉淀，不是反过来。

**代表作品 / 观点**

- 「供应链管理专栏」官网（本人创办并持续更新的博客，一手阵地） —— 〔一手·本人站点〕 https://scm-blog.com/
- 作者自述与背景（西斯国际执行总监） —— 〔一手·本人站点〕 https://scm-blog.com/about.html
- 著作总览页 —— 〔一手·本人站点〕 https://scm-blog.com/book.html
- 《采购与供应链管理：一个实践者的角度》（第 4 版）——中文供应链领域长期销量领先的实务书 —— 〔一手·本人著作〕；官网放出的同名讲义 PDF https://scm-blog.com/Supplier%20and%20Supply%20Chain%20Management.pdf
- 《供应链的三道防线：需求预测、库存计划和供应链执行》（第 2 版）——他最有结构的一本，「三道防线」是其核心框架 —— 〔一手·本人著作〕
- 《供应链管理：高成本、高库存、重资产的解决方案》（第 2 版） —— 〔一手·本人著作〕
- 《供应链的全局观：跨职能协作、成本控制和库存优化》，官网讲义 PDF —— 〔一手·本人著作〕 https://scm-blog.com/9a667a0bf0faae11924d08b87a23d72d8e2e2f2f.pdf
- 供应链管理分类归档（可核对其近期论述主题与更新频率） —— 〔一手·本人站点〕 https://scm-blog.com/cat-5/

**值得读 / 听 / 看的 3 件事**

1. 《供应链的三道防线》全书 —— 这是他体系性最强的一本：第一道防线是**需求预测**（不是「预测要准」，而是「预测必须由一个明确的人负责，并且有一套从判断到数字的流程」），第二道是**库存计划**（安全库存不是拍脑袋，是服务水平 × 需求变异 × 提前期变异的函数），第三道是**供应链执行**（催单、加急、协同）。他的核心判断是：**大多数公司把 90% 的力气花在第三道防线上，因为前两道没人会做。**
2. 官网上的长文归档（scm-blog.com/cat-5/）—— 免费、量大、按主题分类。读博客比读书能更直接看到他处理具体案例的方式。
3. 官网放出的两份讲义 PDF（供应商与供应链管理 / 供应链的全局观）—— 这是他培训体系的骨架，比书更浓缩。

**争议 / 非主流立场**

- **「采购降本是最没用的降本」**：他反复主张，采购谈判能拿到的降幅远小于设计、需求管理与计划带来的降幅，但企业习惯性把压力全给采购，因为那是唯一「看得见对手」的地方。这直接得罪了以年降（annual cost reduction）为 KPI 的采购体系。
- **反对「预测无用论」**：中文圈流行「预测总是不准，所以别做预测，做柔性就行」，他明确反驳：**没有预测就没有计划，柔性也需要预测来决定柔到什么程度**；不准不是不做的理由，是要给预测配一个可改进的流程与责任人。这与 DDMRP「降低对预测的依赖」的取向形成有意思的张力（DDMRP 是缩短需要被预测的时间窗，而不是取消预测——两者其实不矛盾，但在中文语境里常被对立化）。
- **对「小批量多品种是中国特色」的否定**：他把品种爆炸看作**内部治理失败**（谁都能提新料号、没人负责清理），而不是市场逼出来的宿命。这条主张在业务部门极不受欢迎。
- **需要提醒的边界**：他是**实务作者与培训者**，不是流派奠基人，也不产出可被同行评议的原创方法。读他的正确定位是「把前十四位的东西翻成中文语境的高质量转译与实战注释」，而不是把他当成与 Goldratt、Deming 同层的理论来源。对于其书中的具体数字与案例，仍需按一手材料核对。

**最近 12 个月动态.** 「供应链管理专栏」仍在持续更新（可核对的最近归档到 2025 年 12 月，例如《供应商有选择，没管理，注定绩效不好》一文，https://scm-blog.com/2025/12/post-914.html ），主题延续供应商管理与计划职能建设；主要活动形态为企业内训与著作再版。


---

## Source Manifest

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T01-S001 | https://www.lean.org/about-lei/senior-advisors-staff/james-womack/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute founded by Womack; own site bio |
| T01-S002 | https://www.lean.org/about-lei/thought-leader/daniel-jones/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute page for Dan Jones |
| T01-S003 | https://www.lean.org/about-lei/news/background-what-is-the-lean-enterprise-institute/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute self-description |
| T01-S004 | https://www.lean.org/the-lean-post/articles/lean-thinking-at-20-a-qa-with-jim-womack-and-dan-jones/ | verified_primary | 2026-09-02 | Womack & Jones / LEI | own publication, authors self-assessing their book |
| T01-S005 | https://www.lean.org/the-lean-post/articles/jim-womack-and-dan-jones-on-the-evolution-and-future-of-lean/ | verified_primary | 2026-09-02 | Womack & Jones / LEI | own publication |
| T01-S006 | https://www.lean.org/store/book/lean-thinking-2nd-edition/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute publisher page, own publication |
| T01-S007 | https://www.lean.org/store/book/lean-solutions/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute publisher page, own publication |
| T01-S008 | https://www.lean.org/the-lean-post/articles/?written_by=811 | verified_primary | 2026-09-02 | James Womack / LEI | own publication archive, recent-activity check |
| T01-S009 | https://www.lean.org/store/book/learning-to-see/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | originator institute publisher of Rother & Shook, own publication |
| T01-S010 | http://www-personal.umich.edu/~mrother/Homepage.html | verified_primary | 2026-09-02 | Mike Rother (U. Michigan) | own site, free Improvement Kata Handbook by the originator |
| T01-S011 | https://en.wikipedia.org/wiki/Toyota_Kata | secondary | 2026-09-02 | Wikipedia | encyclopedia, bibliography cross-check only |
| T01-S012 | https://www.demanddriveninstitute.com/about-us | verified_primary | 2026-09-02 | Demand Driven Institute | originator institute for DDMRP, founded by Ptak & Smith |
| T01-S013 | https://www.demanddriveninstitute.com/demand-driven-planner-ddp | verified_primary | 2026-09-02 | Demand Driven Institute | originator institute certification page |
| T01-S014 | https://www.demanddriveninstitute.com/demand-driven-leader-ddl | verified_primary | 2026-09-02 | Demand Driven Institute | originator institute certification page |
| T01-S015 | https://www.demanddrivenmrp.com/meet-the-authors | verified_primary | 2026-09-02 | Ptak & Smith / DDI | own site, author page for the DDMRP book |
| T01-S016 | https://www.demanddrivenmrp.com/ddmrp-videos | verified_primary | 2026-09-02 | Ptak & Smith / DDI | own site, originator method videos |
| T01-S017 | https://bc.ascm.org/meetinginfo.php?id=64&ts=1455916293 | verified_primary | 2026-09-02 | ASCM (BC chapter) | association page, CDDP course scope cross-check |
| T01-S018 | https://pubsonline.informs.org/doi/pdf/10.1287/mnsc.1040.0305 | verified_primary | 2026-09-02 | INFORMS / Management Science | academic journal of record, Lee et al. bullwhip paper |
| T01-S019 | https://www2.isye.gatech.edu/~jvandeva/Classes/6203/2006/TheBullWhipEffectinSCsLee.pdf | verified_primary | 2026-09-02 | Georgia Tech ISyE | .edu hosted copy of Lee's Sloan Management Review paper |
| T01-S020 | https://www.gsb.stanford.edu/faculty-research/publications/triple-supply-chain | verified_primary | 2026-09-02 | Hau L. Lee / Stanford GSB | own publication record on the author's own institution site |
| T01-S021 | https://gsb.stanford.edu/faculty-research/faculty/hau-l-lee | verified_primary | 2026-09-02 | Hau L. Lee / Stanford GSB | own site (institution faculty page), current activity |
| T01-S022 | https://pomsmeetings.org/conf-2021/documents/Honoring-Hau-Lee-POMS-2021.pdf | verified_primary | 2026-09-02 | POMS (Production and Operations Management Society) | association conference document honoring Hau Lee |
| T01-S023 | https://sheffi.mit.edu/ | verified_primary | 2026-09-02 | Yossi Sheffi / MIT | own site, book and article archive |
| T01-S024 | https://sheffi.mit.edu/book/resilient-enterprise | verified_primary | 2026-09-02 | Yossi Sheffi / MIT | own site, own publication page |
| T01-S025 | https://sheffi.mit.edu/book/power-resilience | verified_primary | 2026-09-02 | Yossi Sheffi / MIT | own site, own publication page |
| T01-S026 | https://web.mit.edu/sheffi/www/resilientEnterprise.html | verified_primary | 2026-09-02 | Yossi Sheffi / MIT | own site (legacy MIT page) |
| T01-S027 | https://mitpress.mit.edu/9780262693493/the-resilient-enterprise/ | secondary | 2026-09-02 | MIT Press | publisher/bookstore page |
| T01-S028 | https://www.scmr.com/article/the_power_of_resilience_a_qa_with_yossi_sheffi | secondary | 2026-09-02 | Supply Chain Management Review | trade media interview |
| T01-S029 | https://global.toyota/en/company/vision-and-philosophy/production-system/ | verified_primary | 2026-09-02 | Toyota Motor Corporation | company official page of the method originator; TPS definition and Ohno's role in Toyota's own words |
| T01-S030 | https://www.routledge.com/Toyota-Production-System-Beyond-Large-Scale-Production/Ohno/p/book/9780915299140 | secondary | 2026-09-02 | Routledge / Productivity Press | publisher listing for Ohno's own book |
| T01-S031 | https://www.almendron.com/tribuna/wp-content/uploads/2021/12/toyota-production-system-beyond-large-scale-production.pdf | secondary | 2026-09-02 | almendron.com (hosted copy) | third-party hosted full text of Ohno's book; wording check only |
| T01-S032 | https://uen.pressbooks.pub/ompeople/chapter/taiichi-ohno/ | secondary | 2026-09-02 | Utah Education Network / Pressbooks (OER textbook) | open textbook biography, timeline cross-check |
| T01-S033 | https://shingo.org/ | verified_primary | 2026-09-02 | Shingo Institute, Utah State University | originator institute of the Shingo Model and Shingo Prize (.edu affiliated) |
| T01-S034 | https://en.wikipedia.org/wiki/Shigeo_Shingo | secondary | 2026-09-02 | Wikipedia | encyclopedia, dates and bibliography cross-check |
| T01-S035 | https://en.wikipedia.org/wiki/Poka-yoke | secondary | 2026-09-02 | Wikipedia | encyclopedia, term origin cross-check |
| T01-S036 | https://hbr.org/2015/06/find-the-weak-link-in-your-supply-chain | verified_primary | 2026-09-02 | Harvard Business Review / Simchi-Levi | own publication, authors' canonical statement of the Risk Exposure Index |
| T01-S037 | https://news.mit.edu/2022/companies-use-mit-research-identify-respond-supply-chain-risks-0615 | verified_primary | 2026-09-02 | MIT News | own institution reporting on its own research adoption |
| T01-S038 | https://www.ssrn.com/abstract=2875596 | verified_primary | 2026-09-02 | SSRN / Gao, Simchi-Levi, Teo, Yan | academic working paper by the originators, own publication |
| T01-S039 | https://ink.library.smu.edu.sg/cgi/viewcontent.cgi?article=7218&context=lkcsb_research | verified_primary | 2026-09-02 | Singapore Management University institutional repository | .edu repository full text of the REI Revisited paper |
| T01-S040 | https://en.wikipedia.org/wiki/David_Simchi-Levi | secondary | 2026-09-02 | Wikipedia | encyclopedia, bibliography cross-check |
| T01-S041 | https://www.scdigest.com/assets/on_target/13-04-24-1.php?cid=6971 | secondary | 2026-09-02 | Supply Chain Digest | trade media, diffusion of REI |
| T01-S042 | https://www.scdigest.com/assets/newsviews/15-06-10-1.php?cid=9398 | secondary | 2026-09-02 | Supply Chain Digest | trade media, time-to-survive explainer |
| T01-S043 | https://deming.org/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute founded by Deming himself in 1993 |
| T01-S044 | https://deming.org/explore/red-bead-experiment/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute, System of Profound Knowledge and Red Bead source |
| T01-S045 | https://deming.org/deming-red-bead-experiment/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute, official Red Bead Experiment page |
| T01-S046 | https://deming.org/lessons-from-the-red-bead-experiment-with-dr-deming/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute, lessons page |
| T01-S047 | https://deming.org/deming-library-video-with-dr-deming-discussing-the-14-points/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute, Deming's own footage of the 14 Points |
| T01-S048 | https://deming.org/w-edwards-deming-videos-on-demand/ | verified_primary | 2026-09-02 | The W. Edwards Deming Institute | originator institute, video archive index |
| T01-S049 | https://maaw.info/DemingsRedbeads.htm | secondary | 2026-09-02 | MAAW (Management And Accounting Web) | academic teaching site summary, cross-check |
| T01-S050 | https://www.mheducation.com/highered/mhp/product/toyota-way-second-edition-14-management-principles-world-s-greatest-manufacturer.html | secondary | 2026-09-02 | McGraw-Hill Education | publisher page for Liker's book, edition and scope check |
| T01-S051 | https://www.accessengineeringlibrary.com/content/book/9781260468519/front-matter/preface2 | secondary | 2026-09-02 | McGraw-Hill AccessEngineering | publisher-hosted front matter of The Toyota Way 2nd ed |
| T01-S052 | https://www.leanblog.org/2021/02/s1e400-jeff-liker-on-the-second-edition-of-the-toyota-way/ | secondary | 2026-09-02 | Lean Blog (Mark Graban) | podcast interview, practitioner media |
| T01-S053 | https://scm-blog.com/ | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own site, author's primary Chinese-language outlet |
| T01-S054 | https://scm-blog.com/about.html | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own site, author self-description and credentials |
| T01-S055 | https://scm-blog.com/book.html | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own site, own publication list |
| T01-S056 | https://scm-blog.com/Supplier%20and%20Supply%20Chain%20Management.pdf | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own site, own publication (course handout PDF) |
| T01-S057 | https://scm-blog.com/9a667a0bf0faae11924d08b87a23d72d8e2e2f2f.pdf | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own site, own publication (course handout PDF) |
| T01-S058 | https://scm-blog.com/cat-5/ | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own site, topic archive for recent-activity check |
| T01-S059 | https://scm-blog.com/2025/12/post-914.html | verified_primary | 2026-09-02 | 刘宝红 / 供应链管理专栏 | own publication, dated post used to verify recent activity |
| T01-S060 | https://www.tocico.org/mpage/goldratt_foundation | verified_primary | 2026-09-02 | TOCICO / Dr. Eliyahu M. Goldratt Foundation | association page for the originator's own legacy foundation |
| T01-S061 | https://www.tocico.org/page/EliyahuGoldrattWhatisTOC | verified_primary | 2026-09-02 | TOCICO | association, Goldratt's own "What is TOC" material |
| T01-S062 | https://cdn.ymaws.com/www.tocico.org/resource/resmgr/2012_foundation_pdfs/kohls,_kevin_final_toc_&_tmp.pdf | surrogate_primary | 2026-09-02 | TOCICO / Goldratt Foundation | association conference PDF on TOC vs TPS |
| T01-S063 | https://www.scielo.br/j/gp/a/nw43nPSMWtFFqr4x5jhJkJn/?lang=en | verified_primary | 2026-09-02 | SciELO / Gestao & Producao | peer-reviewed journal record of Goldratt's "Standing on the Shoulders of Giants" |
| T01-S064 | https://businesswales.gov.wales/sites/main/files/documents/Standing-on-the-Shoulders-of-Giants.pdf | secondary | 2026-09-02 | Business Wales (gov.wales) | government-hosted copy of Goldratt's paper; text check only |
| T01-S065 | https://en.wikipedia.org/wiki/Theory_of_constraints | secondary | 2026-09-02 | Wikipedia | encyclopedia, TOC toolset and critique index |
| T01-S066 | https://www2.isye.gatech.edu/~jvandeva/Classes/6203/2007/PushPull.pdf | verified_primary | 2026-09-02 | Georgia Tech ISyE | .edu hosted full text of Hopp & Spearman, "To Pull or Not to Pull" (M&SOM 2004) |
| T01-S067 | https://projectproduction.org/journal/reprint-to-pull-or-not-to-pull-what-is-the-question/ | secondary | 2026-09-02 | Project Production Institute | institute reprint of the authors' paper |
| T01-S068 | https://www.waveland.com/browse.php?t=587 | secondary | 2026-09-02 | Waveland Press | publisher page for Factory Physics 3rd ed |
| T01-S069 | https://www.accessengineeringlibrary.com/content/book/9780071822503 | secondary | 2026-09-02 | McGraw-Hill AccessEngineering | publisher-hosted record of Factory Physics for Managers |
| T01-S070 | https://en.wikipedia.org/wiki/CONWIP | secondary | 2026-09-02 | Wikipedia | encyclopedia, CONWIP mechanism cross-check |
| T01-S071 | https://en.wikipedia.org/wiki/Factory_Physics | secondary | 2026-09-02 | Wikipedia | encyclopedia, book structure cross-check |
| T01-S072 | https://pomsmeetings.org/confpapers/051/051-1344.pdf | verified_primary | 2026-09-02 | POMS | association conference paper revisiting the push/pull definition |
| T01-S073 | https://hbr.org/1999/09/decoding-the-dna-of-the-toyota-production-system | verified_primary | 2026-09-02 | Harvard Business Review / Spear & Bowen | own publication, the canonical article of record |
| T01-S074 | https://mitsloan.mit.edu/faculty/directory/steven-spear | verified_primary | 2026-09-02 | Steven Spear / MIT Sloan | own site (institution faculty page), current role |
| T01-S075 | https://mitsloan.mit.edu/ideas-made-to-matter/how-to-wire-your-organization-to-excel-problem-solving | verified_primary | 2026-09-02 | MIT Sloan | own institution article explaining Spear's latest framework |
| T01-S076 | https://ilp.mit.edu/node/64085 | verified_primary | 2026-09-02 | MIT Industrial Liaison Program | own institution record |
| T01-S077 | https://www.usu.edu/today/story/gene-kim-and-steven-j-spear-earn-shingo-publication-award-for-wiring-the-winning-organization | verified_primary | 2026-09-02 | Utah State University / Shingo Institute | .edu awarding body announcing its own Shingo Publication Award |
| T01-S078 | https://itrevolution.com/product/wiring-the-winning-organization/ | secondary | 2026-09-02 | IT Revolution | publisher/bookstore page |
| T01-S079 | https://www.leanblog.org/2023/11/gene-kim-and-steve-spear-discussing-wiring-the-winning-organization/ | secondary | 2026-09-02 | Lean Blog (Mark Graban) | podcast interview, practitioner media |
| T01-S080 | https://www.lean.org/the-lean-post/articles/decoding-the-dna-of-the-toyota-production-system/ | secondary | 2026-09-02 | Lean Enterprise Institute | LEI commentary reposting a third party's HBR article |
| T01-S081 | https://www.spcpress.com/pdf/DJW177.pdf | verified_primary | 2026-09-02 | Donald J. Wheeler / SPC Press | own publication, "The Six-Sigma Zone" manuscript |
| T01-S082 | https://www.spcpress.com/djw_articles.php | verified_primary | 2026-09-02 | Donald J. Wheeler / SPC Press | own site, complete article index |
| T01-S083 | https://www.spcpress.com/seminars.php | verified_primary | 2026-09-02 | Donald J. Wheeler / SPC Press | own site, seminar materials |
| T01-S084 | https://www.qualitydigest.com/inside/statistics-article/problem-sigma-levels-032626.html | surrogate_primary | 2026-09-02 | Donald J. Wheeler (Quality Digest column) | own publication, bylined column dated 2026-03-26; verified author and date; author's own publication (signed column) |
| T01-S085 | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6999184/ | verified_primary | 2026-09-02 | NIH / PubMed Central | peer-reviewed paper questioning the 1.5 SD shift assumption |
| T01-S086 | https://www.isixsigma.com/dmaic-methodology/15-sigma-process-shift/ | secondary | 2026-09-02 | iSixSigma | industry site stating the Six Sigma camp's own defense of the 1.5 sigma shift |
| T01-S087 | https://www.leansixsigmadefinition.com/summary-of-donald-wheelers-understanding-statistical-process-control-uspc-seminar/ | secondary | 2026-09-02 | leansixsigmadefinition.com | third-party seminar notes |
| T01-S088 | https://bidenwhitehouse.archives.gov/cea/written-materials/2023/11/30/issue-brief-supply-chain-resilience/ | verified_primary | 2026-09-02 | US Council of Economic Advisers (White House) | government official issue brief on efficiency-vs-resilience |
| T01-S089 | https://pmc.ncbi.nlm.nih.gov/articles/PMC8771080/ | verified_primary | 2026-09-02 | NIH / PubMed Central | peer-reviewed study of supply chain resilience during COVID-19 |
| T01-S090 | https://www.cfr.org/articles/what-happened-supply-chains-2021 | secondary | 2026-09-02 | Council on Foreign Relations | think-tank analysis of the 2021 disruption |
| T01-S091 | https://www.leanblog.org/2021/06/should-we-blame-just-in-time-or-short-term-thinking-for-supply-chain-problems/ | secondary | 2026-09-02 | Lean Blog (Mark Graban) | practitioner blog arguing the lean camp's rebuttal on JIT |
| T01-S092 | https://www.bcg.com/publications/2021/building-resilience-strategies-to-improve-supply-chain-resilience | secondary | 2026-09-02 | BCG | consultancy analysis piece |
| T01-S093 | https://www.factoryphysics.com/ | verified_primary | 2026-09-02 | Factory Physics (Strategic Project Solutions, Inc.) | originator site for the Factory Physics method; own site, live 2026 |
| T01-S094 | http://goldrattgroup.com/ | verified_primary | 2026-09-02 | Goldratt Consulting / Goldratt Group | originator's own firm (goldratt.com redirects here); own site, steward of Goldratt's TOC legacy |

---

## 附：本轮调研的方法说明与缺口

- **人物筛选标准**：不按知名度排，按「是否定义了一套可被反驳的判断方式」排。因此 CEO（如 Tim Cook）与咨询品牌不入选；已故者若其思想仍有明确的机构承载（Toyota / LEI / Deming Institute / Shingo Institute / TOCICO），按现役处理。
- **已核实的近况**：Wheeler（2026-03 专栏，一手核实日期与署名）、刘宝红（2025-12 博文，一手核实）、Spear（MIT Sloan 现任高级讲师 + 2023 新书获 Shingo Publication Award，一手核实）、Ptak & Smith（Orlicky's MRP 4/E, 2023，机构页核实）。
- **未能一手核实、按推断标注的部分**：Womack / Jones / Liker / Rother / Hopp / Spearman / Hau Lee / Sheffi / Simchi-Levi 的「最近 12 个月」具体动态，只核实到其现任机构与最新公开著作层级，未逐条核实 2025-09 之后的新发表。文中相关表述已限定为「重心 / 形态」而非具体事件。〔推断〕
- **明确未纳入的候选**（避免硬凑）：Joseph Juran、Walter Shewhart、石川馨、田口玄一（统计质量的更早源头，但离「供应链运营判断」较远）；Michael Porter（价值链，属战略而非运营）；Martin Christopher（Cranfield，敏捷供应链，可作为下一轮扩展位）；Bill Smith / Mikel Harry（六西格玛创立者，一手材料稀缺且争议由 Wheeler 一条线已覆盖）。
