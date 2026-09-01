# Track 06 — 术语 + 标准 / Glossary
## 供应链与生产运营（Supply Chain & Production Operations）

> 蒸馏主题：制造业与消费品的实体供应链「计划 - 制造 - 交付」。
> 受众 locale：zh-CN。术语一律给出英文/日文原词。
> last_checked：2026-09-02

**怎么用这份文件**：A 段是术语表，按八个场景分组，每条的最后一列写的是**外行最常见的误解**——那一列比定义更值钱。B 段是标准与认证，凡带 `(Decay risk: high)` 的条目都在近两年内改过版本或时间线，用之前必须回官方页面现查。C 段是「说错就露馅」清单，可当面试题或自查表用。

---

## A. 高频术语 / 黑话

### A1. 计划与需求（Planning & Demand）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 物料需求计划 | MRP (Material Requirements Planning) | 由主生产计划出发，按多级 BOM 逐层展开、扣减在手库存与在途、再按提前期倒推，算出每个物料「什么时候下多少单」的**需求计算逻辑** | APICS/ASCM 体系（Orlicky 1975 起）；CPIM 主考内容 | 以为 MRP 是排产系统。MRP 只算「要多少、什么时候要」，**默认产能无限**，不解决「哪台机器几点干」；那是 APS/排程的事 [T06-S002] |
| 主生产计划 | MPS (Master Production Schedule) | 对最终产品（或计划物料）逐周/逐日的可执行生产承诺，是 MRP 的输入源 | APICS/ASCM CPIM | 以为 MPS 就是销售预测。MPS 是**已经和产能、库存策略打过架之后的承诺**，预测只是它的输入之一 |
| 制造资源计划 | MRP II (Manufacturing Resource Planning) | 在 MRP 的物料闭环上再挂产能计划（RCCP/CRP）和财务口径，让物料计划和钱、和产能对上账 | APICS/ASCM | 以为 MRP II 只是 MRP 的版本号升级；它多的是**产能校验与财务映射**这两条腿 |
| 企业资源计划 | ERP (Enterprise Resource Planning) | 把订单、库存、财务、采购、生产等主数据与事务放在一个共享数据库上的事务型系统 | 行业通用；SAP/Oracle 等厂商实现 | 以为 ERP 会自动「优化」。ERP 是**记账与执行的系统**，优化能力弱，所以才要外挂 APS [T06-S002] |
| 高级计划排程 | APS (Advanced Planning and Scheduling) | 在**有限产能**约束下用优化/启发式算法排出可执行序列与时间的系统 | 供应链软件流派（i2/SAP APO/Kinaxis 等） | 以为上了 APS 就不用维护数据。APS 对 BOM、工艺路线、产能日历的数据质量极度敏感，脏数据出来的排程没人敢用 |
| 产销协同 / 销售与运营计划 | S&OP (Sales and Operations Planning) | 月度节奏的跨职能决策会议链：需求评审 → 供应评审 → 产销平衡 → 高管定案，把销售、生产、财务口径拉到同一套数字上 | APICS/ASCM；Oliver Wight 流派 | 以为 S&OP 是一场会。S&OP 是**一条有固定日历和交接物的流程**，会议只是最后一格；只开会不改计划等于没做 |
| 集成业务计划 | IBP (Integrated Business Planning) | S&OP 的升级形态：把产品组合/新品、财务预算、战略假设都纳进同一套滚动计划，输出以金额与量双口径呈现 | Oliver Wight 提出；SAP 以此命名产品 | 把 IBP 当成一个软件模块。IBP 首先是**治理与决策流程**，软件只是承载 |
| 需求感知 | Demand Sensing | 用近端高频信号（POS 销售、渠道库存、订单流、天气/促销）修正短周期（未来 1-8 周）预测的做法 | 供应链软件/咨询流派 | 以为它能提升长周期预测。需求感知只在**短周期**有效，对 6 个月以后的产能投资毫无帮助 |
| 平均绝对百分比误差 | MAPE (Mean Absolute Percentage Error) | 预测误差 = 平均( \|实际-预测\| / 实际 )，最常被引用的预测精度指标 | 预测学界通用 | 低销量 SKU 上 MAPE 会爆炸（分母接近 0），且对预测偏低有系统性偏袒；不能拿它跨 SKU 直接比 |
| 加权绝对百分比误差 | WMAPE / WAPE | 用销量或金额加权后的绝对误差率 = Σ\|实际-预测\| / Σ实际 | 需求计划实务 | 以为它和 MAPE 只是换了个算法。WMAPE 让大 SKU 说了算，**更贴近业务损失**，是组合层面的正确默认口径 |
| 偏差 | Bias (Forecast Bias) | 误差的**方向**：长期系统性偏高或偏低 | 预测学界 | 只盯 MAPE 不看 bias。误差可以很小但一直偏低，结果就是长期缺货；bias 是比精度更该先修的病 |
| 预测增值 | FVA (Forecast Value Added) | 拿每一道人工干预后的预测，与朴素基准（如「上期即下期」）对比，衡量这道工序到底加没加价值 | Michael Gilliland / SAS 推广的实务方法 | 以为流程越多越准。FVA 常常证明**某些人工调整是负增值**，删掉反而更准 |
| 时界 | Time Fence | 计划期上划出的分界线：界内变更需要人工审批或禁止自动改单 | APICS/ASCM；ERP 通用参数 | 把时界当成「死线」。时界是**变更权限的分界**，不是不能改，是改要付代价、要走人 [T06-S002] |
| 冻结区 | Frozen Zone / Demand Time Fence | 时界中最靠近当下、原则上不允许系统自动改动的一段（常为提前期内） | APICS/ASCM | 以为冻结区越长越稳。冻结区越长，响应真实需求的能力越差，这是**稳定 vs 柔性**的直接交易 |
| 计划神经质 | MRP Nervousness / System Nervousness | 上层需求或参数的微小变动，经 BOM 层层放大成下层大量改单、催单与推迟 | APICS/ASCM 术语 | 以为是系统 bug。它是**批量规则 + 时界设置 + 重跑频率**共同造成的结构性现象 [T06-S002] |
| 批量规则 | Lot Sizing (LFL / FOQ / POQ / Wagner-Whitin) | MRP 把净需求凑成实际订单量的规则：按需批量、固定批量、周期批量、动态最优等 | 运筹学 + APICS 实务 | 以为批量只影响库存。批量规则同时决定了**计划的稳定性**，是神经质的头号来源 |
| 滚动计划 | Rolling Horizon Planning | 每期只执行最近一段、然后把计划期整体向前推一格重算 | 运筹学/生产计划学界 | 以为「重算 = 重来」。滚动的意义是**只锁定近端、远端保持粗颗粒**，把决策推迟到信息更好的时候 [T06-S003] |
| 需求计划 | Demand Planning | 把统计预测、销售输入、促销与新品假设合成一份跨职能认可的需求共识 | APICS/ASCM | 以为它归销售。需求计划归属需求计划职能，**销售提供输入而不是拍板**，否则永远偏乐观 |
| 粗能力需求计划 | RCCP (Rough-Cut Capacity Planning) | 在 MPS 层面对关键资源做快速产能校验，判断计划是否根本不可行 | APICS/ASCM CPIM | 以为可以跳过它直接跑 MRP。跳过的结果是 MRP 产出一份**产能上不可能实现**的完美计划 |
| DDMRP 需求驱动物料需求计划 | DDMRP (Demand Driven MRP) | 在供应链上选点设置解耦缓冲，用缓冲状态（红黄绿）而非未来预测触发补货 | Demand Driven Institute（Ptak & Smith） | 以为是 MRP 的替代品。DDMRP 主要是**在哪儿放缓冲 + 拿什么信号触发**的重构，仍需 BOM 与提前期数据 |

### A2. 库存（Inventory）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 安全库存 | Safety Stock | 为吸收**需求波动与供应波动**而多备的量，按目标服务水平和波动的统计量算出来 | 库存理论（经典公式 z·σ·√L） | 以为是「多备一点」的经验值。它是**服务水平 z 值 × 需求/提前期标准差**算出来的数，波动不变、只加库存并不会提升服务水平 [T06-S007] |
| 再订货点 | ROP (Reorder Point) | 库存降到该水位就触发补货：ROP = 提前期内平均需求 + 安全库存 | 库存理论 | 以为 ROP 是库存下限。ROP 是**触发线**，触发后库存还会继续往下走一个提前期 [T06-S007] |
| 经济订货批量 | EOQ (Economic Order Quantity) | 在订货成本与持有成本之间取平衡的批量：√(2DS/H) | Harris 1913 起的经典库存理论 | 把它当放之四海的最优解。EOQ 假设需求恒定、提前期确定、无数量折扣，现实里更多是**用来讲清批量的权衡结构** |
| 报童模型 | Newsvendor Model | 单周期、卖不掉就报废的场景下，用缺货成本与过剩成本之比（临界比）定订货量 | 库存理论经典模型 | 以为只适用于报纸和生鲜。任何**只有一次订货机会**的场景（时装季、演唱会周边、疫苗）都是报童问题 [T06-S007] |
| 服务水平（周期） | Cycle Service Level (CSL / Type-1) | 一个补货周期内**不发生缺货**的概率 | 库存理论 | 和满足率混用。CSL 说的是「有没有缺过」，不管缺了多少 [T06-S007] |
| 满足率 | Fill Rate (Type-2 Service Level) | 需求中被现货直接满足的**比例** | 库存理论 | 以为 95% 服务水平 = 95% 满足率。同一套库存下 fill rate 通常**明显高于** CSL，两者不能互换汇报 [T06-S007] |
| 缺货率 | Stockout Rate | 缺货发生的频次或缺货需求占比 | 库存实务 | 只统计「货架空了」的次数，忽略**被替代品吸收的隐性缺货**，从而低估损失 |
| 库存周转率 | ITO (Inventory Turnover) | 年销货成本 / 平均库存，衡量库存一年翻几次 | 财务与运营通用 | 以为越高越好。周转率被极限拉高的代价通常是缺货率和加急运费飙升 |
| 库存天数 | DOS / DOH / DIO (Days of Supply / Days on Hand) | 现有库存按当前消耗速度能撑多少天 | 运营与财务通用 | 用哪个分母（历史消耗还是未来预测）不说清，两个部门算出的天数能差一倍 |
| 呆滞库存 / 呆料 | Excess & Obsolete (E&O) / Slow-Moving Inventory | 超出可预见需求、或已无需求的存货 | 财务与运营 | 以为呆滞是仓库的锅。呆滞主要来自**预测偏乐观、最小起订量、工程变更**，仓库只是它最终待的地方 |
| ABC 分类 | ABC Analysis | 按金额贡献（帕累托）把物料分 A/B/C，管理精度分级投入 | 库存管理经典 | 只按金额分。金额高但需求极稳的 A 类未必需要重管 |
| ABC-XYZ 分级 | ABC-XYZ Segmentation | 在 ABC（金额）之外再加 XYZ（需求波动性/可预测性）两维分类 | 需求计划实务 | 以为 XYZ 是销量高低。XYZ 是**波动/可预测性**，它决定用什么补货策略，比金额更能决定方法 |
| 供应商管理库存 | VMI (Vendor Managed Inventory) | 由供应商依据客户提供的库存与消耗数据，自主决定补货时间与数量 | 快消/汽车行业实践 | 以为 VMI = 供应商替我扛库存成本。VMI 的核心是**信息共享减少牛鞭效应**，所有权与结算另有约定 |
| 寄售 | Consignment Stock | 货放在客户/经销商处，所有权仍归供应商，领用（或销售）时才结算 | 采购与渠道实务 | 把寄售和 VMI 当同义词。VMI 讲**谁来决定补货**，寄售讲**货权什么时候转移**，两件事可以任意组合 |
| 协同计划预测与补货 | CPFR (Collaborative Planning, Forecasting and Replenishment) | 零售商与供应商共享促销日历、共同做一份预测并据此补货的协作框架 | GS1 / VICS 起源的行业标准框架 | 以为是给对方发个 Excel。CPFR 要求**共同的例外处理规则和一份共识预测**，否则就是两份预测互相打架 [T06-S018] |
| 风险池化 | Risk Pooling | 把多个需求源的波动合并（集中库存/延迟差异化/共用部件），总波动小于各自波动之和 | 运筹/供应链学界（√N 规则） | 以为集中仓一定省钱。集中降低的是**库存**，但常常抬高**运输成本与交付时效**，是一个交易不是免费午餐 [T06-S006] |
| 牛鞭效应 | Bullwhip Effect | 需求波动沿供应链向上游逐级放大的现象 | Forrester 提出、Lee/Padmanabhan/Whang 1997 系统化 | 以为是下游在瞎报。四大成因是**需求信号处理、批量订货、价格波动/促销、短缺博弈配额**，多数是激励结构造成的 [T06-S005] |
| 循环盘点 | Cycle Counting | 按分级频率持续小批量盘点，而不是年终一次性大盘 | 库存管理实务 | 以为盘点是为了对账。循环盘点的真正目的是**找出数据不准的根因**并修流程 |
| 库存准确率 | Inventory Record Accuracy (IRA) | 系统账面数量与实物数量一致的比例（通常按 SKU-库位计） | APICS/ASCM 实务 | 用金额准确率糊弄。MRP 吃的是**数量**，金额对得上但数量错，MRP 照样算错 |

### A3. 精益 / 丰田生产方式（Lean / TPS）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 浪费 | ムダ / muda | 一切消耗资源却不为客户创造价值的活动 | TPS / 丰田官方 | 以为砍浪费就是砍人。丰田的原意是**把腾出的时间还给改善和产量**，裁员会让现场再也不肯说真话 [T06-S010][T06-S048] |
| 不均 | ムラ / mura | 生产量、工作量在时间上的忽高忽低 | TPS / 丰田官方 | 只盯 muda 不管 mura。**不均是浪费和超负荷的共同上游**，不平准化，砍浪费砍不动 [T06-S009][T06-S048] |
| 超负荷 | ムリ / muri | 让人或设备在超出合理能力的状态下工作 | TPS / 丰田官方 | 把 muri 当成「加把劲」。持续 muri 直接产出质量缺陷、工伤和设备故障 [T06-S009] |
| 七大浪费 | Seven Wastes（过量生产/等待/搬运/加工本身/库存/动作/不良） | 大野耐一归纳的浪费分类，其中**过量生产是万恶之首**，因为它掩盖其他所有浪费 | TPS / 大野耐一 | 以为库存是最大的浪费。TPS 排第一的是**过量生产**，库存只是它的表现形式 |
| 看板 | かんばん / kanban | 在拉动系统里传递「补多少、什么时候补」的**实体或电子信号卡**，卡不回来就不许生产 | TPS / 丰田官方 | 把 kanban 当成一块白板贴便利贴。kanban 是**限制在制品数量的授权信号**，没有数量上限的板子不是看板 [T06-S053] |
| 准时化 | ジャストインタイム / JIT (Just-in-Time) | 只在需要的时候、按需要的量、生产需要的东西 | TPS 两大支柱之一 / 丰田官方 | 以为 JIT = 零库存。丰田自己在关键点保有**标准在制品与缓冲**，JIT 反对的是**过量与提前**，不是反对一切库存 [T06-S009][T06-S053] |
| 自働化（带人字旁） | 自働化 / jidoka（autonomation） | 让设备或作业者在检出异常时**立刻停线**，把质量做进工序里 | TPS 两大支柱之一 / 丰田官方；LEI 词典 | 以为是「自动化」。日文特意用带人字旁的「働」，重点是**异常自己会喊停**，不是无人化 [T06-S009][T06-S011] |
| 安灯 | アンドン / andon | 现场的异常显示装置（灯/板），谁发现问题都能拉绳点亮、呼叫支援 | TPS / 丰田官方 | 以为安灯是给管理层看的报警屏。安灯的价值在于**一线有权喊停并被立刻响应**，没人来支援的安灯没人再拉 [T06-S009] |
| 防错 | ポカヨケ / poka-yoke | 用便宜的物理或逻辑装置，让错误**做不出来**或立刻被发现 | 新乡重夫；LEI 词典 | 以为防错是加检验。检验是事后抓，防错是**事前让错误不可能发生**，优先级高得多 [T06-S054] |
| 快速换模 | SMED (Single-Minute Exchange of Die) | 把换型时间压到个位数分钟的方法：先分内外作业，再把内作业转成外作业 | 新乡重夫 | 以为是买台快换设备。SMED 的主要收益来自**把能在机器运转时做的事挪出去**，不花钱的部分先做 |
| 平准化 | 平準化 / heijunka | 在固定周期内把产品**种类和数量**都摊平，避免批量与波峰 | TPS；LEI 词典 | 只平准数量不平准品种。真正的 heijunka 要求**混线小批量轮转**，否则换型压力全压在下游 [T06-S052] |
| 节拍时间 | タクトタイム / takt time | 可用生产时间 ÷ 客户需求量，即「客户每隔多久要一件」 | TPS；LEI 词典 | 以为 takt 是自己的产能。takt **由客户需求决定**，产能是拿来对齐它的，方向反了就会一直过量生产 [T06-S051] |
| 周期时间 | Cycle Time | 同一工序连续产出两件之间的间隔（工序自己的节奏） | 工业工程 / 精益 | 和 lead time 混用，这是本行最常见的露馅点。cycle time 是**一道工序的节奏**，不含排队等待 |
| 交付提前期 | Lead Time | 从客户下单（或触发点）到拿到东西之间的**全部日历时间**，含排队、审批、运输 | 工业工程 / 精益 / APICS | 以为把 cycle time 加起来就是 lead time。真实工厂里 **90% 以上的 lead time 是等待**，加工时间只占很小一块 |
| 通过时间 | Throughput Time / Flow Time | 一件产品从投料到完工穿过整条流程所花的时间 | 工业工程 | 和 lead time 混为一谈。throughput time 只覆盖**车间内部**，lead time 通常还要加上订单处理与发运 |
| 单件流 | One-Piece Flow / Continuous Flow | 一次只做、只传一件，不攒批 | TPS；LEI 词典 | 以为单件流一定效率更低。单件流牺牲的是局部设备利用率，换来的是**大幅缩短的通过时间和早期暴露缺陷** |
| 现地 | 現場 / gemba | 价值实际发生的地方（车间、仓库、门店） | TPS；LEI 词典 | 把「去现场」当成视察。gemba 的要求是**去看事实、不带结论**，看完还要跟一线一起改 |
| 现地现物 | 現地現物 / genchi genbutsu | 亲自到现场、亲眼看实物再做判断 | 丰田之道两大支柱之一 / 丰田官方 | 以为看照片和报表也算。丰田的原则明确是**亲自去、亲眼看**，报表只是二手信息 [T06-S010] |
| 改善 | 改善 / kaizen | 由一线主导、小步快跑、持续不断的改进 | TPS / 丰田官方 | 把 kaizen 当成大项目。kaizen 的本体是**每天一点、由做这件事的人自己改** [T06-S010] |
| 方针管理 | 方針管理 / hoshin kanri (Policy Deployment) | 把少数几个战略目标层层展开成各层的目标与对策，并按月/季 catchball 对齐 | TPS / 精益管理体系 | 以为是 KPI 分解表。hoshin 的关键是**上下反复议价（catchball）以及聚焦到极少数目标**，目标一多就退化成 KPI 摊派 |
| A3 报告 | A3 Report | 用一张 A3 纸走完「背景-现状-目标-根因-对策-计划-跟进」的问题解决与沟通格式 | TPS / 精益 | 当成汇报模板。A3 是**思维训练与带教工具**，写的人和辅导的人对话才是价值所在 |
| 5S | 5S（整理/整顿/清扫/清洁/素养） | 现场基础的目视化与秩序管理法 | TPS / 精益 | 以为 5S 就是大扫除。5S 的目的是**让异常一眼可见**，看不出异常的整洁只是好看 |
| 标准作业 | Standardized Work | 围绕 takt time 定义的作业顺序、标准在制品与时间，是改善的基线 | TPS；LEI 词典 | 以为标准作业是束缚。没有标准就**没有改善的基准线**，改完也无法判断好坏 [T06-S012] |
| 横展 | 横展 / yokoten | 把一处验证有效的对策横向复制到其他线、其他厂 | TPS | 以为横展就是发文件。yokoten 要求接收方**自己去看、自己适配**，照抄常常水土不服 |
| 价值流图 | VSM (Value Stream Mapping) | 画出一个产品族从原料到客户的物流与信息流，标出各段增值时间与等待时间 | LEI（Rother & Shook《Learning to See》） | 以为是流程图。VSM 必须带**时间线与信息流**，只画工序框就退化成普通流程图 [T06-S049] |

### A4. 约束理论（TOC）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 约束 / 瓶颈 | Constraint / Bottleneck | 决定整个系统产出上限的那一个环节；系统产出 = 约束的产出 | TOC（Goldratt《目标》） | 把「最忙的工位」当瓶颈。瓶颈的判据是**产能 < 需求**，最忙可能只是批量或排班烂，不是真瓶颈 [T06-S014] |
| 鼓-缓冲-绳 | DBR (Drum-Buffer-Rope) | 用约束（鼓）定全线节拍，在约束前放时间缓冲，用绳子把投料速度绑到约束节奏上 | TOC | 以为要给每道工序都做详细排程。DBR 只**详细排约束**，其余工序跟着走就行 [T06-S014] |
| 简化鼓缓绳 | S-DBR (Simplified DBR) | 把约束默认设在市场需求侧，只用一条订单交付缓冲驱动 | TOC 后期发展 | 以为 S-DBR 是 DBR 的省事版。它换了个前提：**约束在市场而非车间** |
| 缓冲管理 | Buffer Management | 按缓冲消耗比例（绿/黄/红）决定该催谁、该改什么，用红区原因做持续改进 | TOC | 只看红区催货，不做**红区原因统计**，等于放弃了 TOC 最有价值的改善输入 |
| 五步聚焦 | Five Focusing Steps（识别-挖尽-迁就-提升-回头再来） | 找到约束 → 榨干现有约束产能 → 全系统迁就它 → 再投资扩它 → 约束转移后回到第一步 | TOC | 直接跳到第 4 步买设备。**第 2、3 步通常不花钱就能拿到大部分收益**，且跳过后新瓶颈会立刻冒出来 [T06-S014] |
| 有效产出 | Throughput (T) | 系统通过**销售**产生钱的速率 = 销售额 − 完全变动成本 | TOC 三指标 | 以为 throughput 就是产量。没卖出去的产出在 TOC 里**记为库存不记为有效产出** [T06-S014] |
| 库存 / 投资 | Inventory / Investment (I) | 系统为了将来卖出而投入的、被套住的钱 | TOC 三指标 | 把 I 只理解成原材料。TOC 的 I 含设备与在制品，是**所有被套住的资金** [T06-S014] |
| 运营费用 | OE (Operating Expense) | 把 I 转换成 T 所花的钱（工资、水电、折旧等） | TOC 三指标 | 以为降 OE 是首选。TOC 的排序明确是 **T 优先、其次 I、最后 OE**，因为 T 无上限而 OE 有下限 [T06-S014] |
| 关键链项目管理 | CCPM (Critical Chain Project Management) | 把各任务的个人安全时间抽出来汇总成项目缓冲，按缓冲消耗管进度 | TOC 在项目管理的应用 | 以为是关键路径改个名。CCPM 额外考虑**资源争用**，并把安全时间从任务里剥出来集中管理 |
| 迁就 / 从属 | Subordination | 让所有非约束环节都为约束的节奏服务，哪怕自己看起来在闲置 | TOC | 最难被接受的一步：非约束工位闲置在 TOC 里是**正确的**，逼它满负荷只会堆在制品 [T06-S014] |

### A5. 质量与过程（Quality & Process）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 统计过程控制 | SPC (Statistical Process Control) | 用统计方法监控过程输出，把「正常波动」和「有原因的异常」区分开，在异常发生时及时干预 | ASQ；AIAG & VDA SPC 手册 | 以为 SPC 就是画图。SPC 的意义是**区分普通原因与特殊原因**，对普通原因做逐点调整（过度调整）反而会把波动放大 [T06-S015] |
| 控制图 | Control Chart | 把过程数据按时间序列打点，配上由**过程自身数据**算出的控制限 | Shewhart；ASQ | 把控制限当成规格限。控制限来自**过程实际表现**，规格限来自客户要求，两者画在一张图上是典型错误 |
| 过程能力指数 | Cp | 规格公差宽度 ÷ 6 倍过程标准差，衡量过程「潜在」能力（假设居中） | ASQ | Cp 很高不代表合格。Cp **不看中心是否偏移**，偏了照样批量超差 [T06-S015] |
| 过程能力指数（含偏移） | Cpk | 规格限到过程均值的距离 ÷ 3 倍标准差，取两侧较小值 | ASQ；AIAG 核心工具 | 以为 Cpk 可以在过程不稳定时算。前提是过程**先处于统计受控状态**，否则这个数没有意义 [T06-S015] |
| 过程性能指数 | Pp / Ppk | 用整体（长期）标准差算的能力指数，反映实际交付表现 | AIAG SPC | 把 Ppk 和 Cpk 混着报。Cpk 用组内短期波动，Ppk 用长期整体波动，**Ppk 通常更低也更诚实** |
| DMAIC | DMAIC (Define-Measure-Analyze-Improve-Control) | 六西格玛改进项目的五阶段路线：定义-测量-分析-改进-控制 | ASQ / 六西格玛 | 跳过 Measure 直接上对策。没有基线数据，Improve 之后**无法证明有没有改好** [T06-S016] |
| 六西格玛 | Six Sigma | 以降低过程变异为核心的改进体系，名字来自「规格限距均值 6 个标准差」的目标水平 | Motorola 起源；ASQ 认证体系 | 以为 6σ 是「几乎零缺陷」的口号。它是**具体的变异水平目标**，配套的是统计工具和项目治理 |
| 每百万机会缺陷数 | DPMO (Defects Per Million Opportunities) | 缺陷数 ÷ (单位数 × 每单位机会数) × 10^6 | ASQ / 六西格玛 | 把 DPMO 和 PPM 当同一件事。DPMO 分母含**每单位的机会数**，复杂产品的 DPMO 会显著低于 PPM [T06-S015] |
| 失效模式与影响分析 | FMEA (Failure Mode and Effects Analysis) | 系统性列出可能的失效模式、后果、原因与现有控制，据此排优先级并定措施 | AIAG & VDA FMEA Handbook（2019 首版，2022 第二次印刷） | 以为还在用 RPN 排序。AIAG-VDA 版**已用 AP（Action Priority）表取代 RPN**，并改成 7 步法，还新增了 FMEA-MSR [T06-S017] |
| 措施优先级 | AP (Action Priority) | AIAG-VDA FMEA 里用严重度/频度/探测度三者组合查表得出的 H/M/L 优先级 | AIAG & VDA FMEA Handbook | 以为 AP 是 RPN 换算。AP 是**查表得出的分级**，不是乘积，目的就是消除 RPN 相乘导致的错误排序 [T06-S017] |
| 测量系统分析 | MSA (Measurement System Analysis) / Gage R&R | 评估量具与测量方法本身带来的变异（重复性与再现性）占比 | AIAG MSA 第 4 版 | 拿到超差数据先怪产线。**先证明量具可信**，否则改的是幻觉 [T06-S017] |
| 首件检验 | FAI (First Article Inspection) / 首件确认 | 换型、换料、换班或工程变更后，对第一件产出做全尺寸/全特性确认再放行批量 | 汽车/航空质量实务；AS9102 有专门标准 | 以为首件是走个形式签字。首件的价值在于**在批量报废之前抓住设置错误** |
| 控制计划 | Control Plan | 逐工序写明控制特性、规格、量具、抽样频率与异常反应计划的文件 | AIAG Control Plan 手册（2024 起独立成册，第 1 版） | 以为控制计划是质量部的文件。它是**产线执行文件**，写了不做等于审核时的直接不符合 [T06-S017] |
| 可接受质量水平 | AQL (Acceptable Quality Level) | 抽样检验方案里被视为可接受的过程平均不良率水平（配套 ISO 2859 / ANSI Z1.4 抽样表） | ISO 2859 系列 | 以为 AQL 1.0 表示「只允许 1% 不良」。AQL 是**抽样方案的设计参数**，反映的是判定风险，不是对交付批的质量承诺 |
| 一次通过率 | FPY (First Pass Yield) / FTT (First Time Through) | 不经任何返工、一次就合格通过的比例 | 精益 / 汽车行业 | 用最终合格率冒充 FPY。返工修好的算合格，会把**返工浪费完全藏起来** |
| 滚动通过率 | RTY (Rolled Throughput Yield) | 各工序 FPY 连乘，反映整条线一次做对的概率 | 六西格玛；ASQ | 只看单工序良率。20 道工序每道 99%，RTY 只有 82%，这才是**客户感知到的质量** [T06-S015] |
| 8D 报告 | 8D (Eight Disciplines) | 客户抱怨处理的八步法：紧急围堵 → 根因 → 永久对策 → 验证 → 防再发 → 横展 | 汽车行业实务（源自福特） | 把围堵措施当成永久对策交差。D3 围堵和 D5/D6 永久对策**必须分开**，否则问题必然复发 |

### A6. 制造与产能（Manufacturing & Capacity）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 设备综合效率 | OEE (Overall Equipment Effectiveness) | 可用率 × 表现性 × 质量合格率，衡量计划生产时间里真正产出合格品的比例 | TPM / JIPM（日本设备保全协会）；LEI 词典 | 用 OEE 跨设备横向比排名。OEE 只在**同一台设备的时间序列**上有意义，也不能对非瓶颈设备追求高 OEE [T06-S019] |
| 六大损失 | Six Big Losses | 故障停机、换型调整、小停机空转、速度降低、过程不良、启动良率损失 | TPM / JIPM | 只统计大故障。**小停机和降速这两类「隐形损失」通常占大头**，恰恰最难被记录 [T06-S019] |
| 产能利用率 | Capacity Utilization | 实际产出 ÷ 可用产能 | 运营管理 / 排队论 | 以为越高越好。排队论里利用率趋近 100% 时**等待时间趋于无穷**，所以高利用率通常意味着长交期 [T06-S020] |
| 瓶颈工序 | Bottleneck Operation | 产能小于其上下游需求、决定全线产出的那道工序 | TOC / 工业工程 | 把在制品堆得最多的工位当瓶颈。堆料可能只是**上游批量太大**造成的，需要看产能对需求的比值 |
| 换型时间 | Changeover Time / Setup Time | 上一款最后一件合格品到下一款第一件合格品之间的时间 | 精益 / SMED | 只算「拧螺丝」的时间。正确口径**含调试与首件合格前的所有时间** |
| 在制品 | WIP (Work in Process) | 已投料尚未完工、被压在流程里的数量 | 工业工程 / 精益 | 把高 WIP 当成「产线很忙」。WIP 越高，**通过时间越长、质量问题暴露越晚** [T06-S020] |
| 利特尔法则 | Little's Law | 在制品 = 产出速率 × 通过时间（WIP = Throughput × Cycle Time） | 排队论（John Little, 1961） | 以为放更多料进去就能多产出。产出由瓶颈决定，多放料**只会等比例拉长通过时间** [T06-S020] |
| VUT 公式 | VUT / Kingman's Equation | 等待时间 ≈ 变异性因子 × 利用率因子 × 单件加工时间；利用率因子为 ρ/(1−ρ) | 排队论（Kingman）；Factory Physics 流派 | 以为交期长是因为人不努力。VUT 说明**变异 × 高利用率**才是排队的数学成因，不消除变异就只能靠降利用率买交期 [T06-S020][T06-S046] |
| 良率 | Yield | 合格产出 ÷ 投入 | 制造通用 | 和 FPY 混用，把返工救回来的算进良率，掩盖返工成本 |
| 节拍与产线平衡 | Line Balancing | 把作业内容重新分配到各工位，使各工位工时尽量接近 takt time | 工业工程 / 精益 | 以为平衡是为了让每个人一样忙。平衡的目的是**把零散的等待集中起来消灭掉**，而不是均摊 |
| 标准在制品 | SWIP (Standard Work in Process) | 为维持流动所必需的最小在制品数量，属于标准作业三要素之一 | TPS；LEI 词典 | 以为 TPS 要求零在制品。SWIP 是**被规定下来的必要在制品**，少于它反而停线 [T06-S012] |
| 计划外停机 | Unplanned Downtime | 非计划的设备或产线停止时间 | TPM | 只统计时长不统计次数。**频次决定了对计划的破坏程度**，两个口径必须一起看 |
| 总生产维护 | TPM (Total Productive Maintenance) | 以操作者自主保全为基础、全员参与的设备管理体系，OEE 是它的核心指标 | JIPM（1971 年提出） | 以为 TPM 是维修部的事。TPM 的第一支柱是**操作者自主保全**，维修部只做专业保全 [T06-S019] |

### A7. 履行与交付（Fulfillment & Delivery）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| 备货生产 | MTS (Make-to-Stock) | 按预测生产并入库，客户从成品库存直接提货 | 生产策略分类；APICS/ASCM | 以为 MTS 一定库存高。MTS 的成败取决于**预测准度与解耦点选得对不对**，而不是备多少 [T06-S018] |
| 订单生产 | MTO (Make-to-Order) | 收到客户订单后才开始生产，成品不备库存 | 生产策略分类 | 以为 MTO 就没有预测。MTO 仍需要**对原材料和产能做预测性准备**，否则交期长到没人下单 |
| 订单装配 | ATO (Assemble-to-Order) | 通用部件按预测备货，收到订单后才做最终装配与配置 | 生产策略分类；SAP/JDE 均有对应流程 | 把 ATO 当 MTO 的快版。ATO 的前提是**产品结构上存在通用件与差异件的清晰分界** [T06-S021] |
| 订单设计 | ETO (Engineer-to-Order) | 收到订单后才做设计，BOM 与工艺随订单产生 | 生产策略分类 | 用 MTS 的 KPI 考核 ETO 业务。ETO 的瓶颈通常在**工程设计资源**而不是产线 |
| 客户订单解耦点 | CODP (Customer Order Decoupling Point) / OPP (Order Penetration Point) | 供应链上「预测驱动」与「订单驱动」的分界点，也是产品被指定给某个客户的那一刻 | 生产策略/供应链设计文献 | 以为解耦点是仓库位置。它是**流程上的一个点**，往下游移就是 MTS，往上游移就是 MTO [T06-S018] |
| 延迟策略 | Postponement (Delayed Differentiation) | 把使产品差异化的工序尽量往后推，在通用状态下保有库存 | 供应链设计（HP 打印机是经典案例） | 以为延迟只是「晚点做」。延迟需要**先重新设计产品与流程**，把差异化工序移到末端，是设计问题不是排程问题 [T06-S018] |
| 可承诺量 | ATP (Available-to-Promise) | 在现有库存与已计划产出中，尚未被承诺出去、可以许给新订单的数量 | APICS/ASCM；ERP/APS 通用功能 | 把在手库存当 ATP。ATP 必须**扣掉已承诺给别人的量**，否则同一批货被卖两次 [T06-S022] |
| 可承诺产能 | CTP (Capable-to-Promise) | 在 ATP 不足时，进一步调用产能与物料可用性校验，算出真正能承诺的交期 | SAP APO/PP-DS 等 APS 功能 | 以为 CTP 只是把 ATP 算得更细。CTP 会**真的去排产能**，因此对主数据质量与响应时间要求高得多 [T06-S047] |
| 准时足量交付 | OTIF (On Time In Full) | 既按承诺日期到、又按承诺数量到的订单（行）占比；两个条件必须同时满足 | 零售/快消行业实务；SCOR 可靠性属性下的同类指标 | 用 OT 和 IF 分别达标来报 OTIF。OTIF 是**逻辑与**，两个 95% 相乘只有 90% |
| 完美订单履行 | Perfect Order Fulfillment | SCOR 可靠性属性下的核心指标：准时 + 足量 + 单证正确 + 无破损，四项全对才计一单 | ASCM SCOR-DS | 以为它等于 OTIF。完美订单还要求**单证与货物状态都对**，通常比 OTIF 低几个点 [T06-S001] |
| 满足率 | Fill Rate（订单行/数量/订单三种口径） | 被现货直接满足的比例，可按订单行、数量或整单计算 | 库存与履行实务 | 不说口径就报数字。按数量算和按整单算能差十几个点，**跨公司比较必须先对口径** |
| 齐套率 | Kitting Rate / Component Availability | 一个订单/工单所需物料全部到齐的比例 | 制造现场实务 | 用平均物料齐套率糊弄。装配是**逻辑与**，缺一件就开不了工，要看的是「整套齐」的比例 |
| 承诺交期 vs 实际交期 | Quoted / Promised Lead Time vs Actual Lead Time | 对外报的交期与实际兑现的交期 | 履行实务 | 只考核实际交期。承诺交期被销售随口改短时，实际再准也叫「延误」 |
| 累计提前期 | Cumulative Lead Time / Aggregate Lead Time | 从最长的一条 BOM 路径上把各级采购与制造提前期加起来的总时长 | APICS/ASCM | 以为交期等于装配时间。累计提前期决定了**你最多能承诺多快**，它通常远长于装配周期 |
| 订单履行周期 | Order Fulfillment Cycle Time | SCOR 响应性属性指标：从客户下单到客户收到货的实际时间 | ASCM SCOR-DS | 从「排产完成」开始掐表。SCOR 口径**从收到订单开始算** [T06-S001] |
| 紧急插单 / 加急 | Expediting / Hot Order | 打破既定序列优先处理某订单 | 现场实务 | 以为加急不花钱。每一次插单都会**推迟其他所有订单并抬高整体变异**，是交期恶化的自我强化循环 |

### A8. 采购与供应商（Sourcing & Supplier Management）

| 中文名 | 英文/日文原名 | 一句话定义 | 出自流派/标准 | 外行最常误解的点 |
|---|---|---|---|---|
| Kraljic 矩阵 | Kraljic Matrix / Purchasing Portfolio Model | 按「利润影响」与「供应风险」两维把采购品类分为战略/瓶颈/杠杆/一般四类，各配不同策略 | Peter Kraljic, HBR 1983《Purchasing Must Become Supply Management》 | 只按金额分类。**低金额高风险的瓶颈件**（一颗停产芯片）才是最容易把整条线打停的那一类 [T06-S023] |
| 单一来源 | Sole Source | 市场上**只有这一家**能供（专利、独占产能、客户指定） | 采购实务 | 和 single source 混用，这是采购最典型的露馅点 |
| 单一供应商 | Single Source | 市场上有多家可选，但公司**主动选择只用一家** | 采购实务 | 把 single 说成 sole 会让风险评估结论完全反过来：sole 只能靠库存和替代设计化解，single 是自己一句话就能改的决策 |
| 双源 / 多源 | Dual Sourcing / Multi-Sourcing | 同一物料由两家或多家供应商按比例供货 | 采购实务 | 以为多源一定更安全。若多家共用**同一个二级供应商或同一片产区**，多源只是账面多源 |
| 总拥有成本 | TCO (Total Cost of Ownership) | 采购价之外，把物流、关税、质量成本、库存持有、切换与报废等全生命周期成本算进来 | 采购与供应管理学界/实务 | 只比单价。低价供应商常靠**更长交期、更高不良、更大 MOQ** 把成本转嫁到你的库存和产线上 |
| 最小起订量 | MOQ (Minimum Order Quantity) | 供应商要求的单次最小订购数量 | 采购实务 | 以为 MOQ 只是谈判问题。MOQ 常常来自**供应商的换型成本或模具产能**，攻它要攻工艺不是攻价格 |
| 最小包装量 | MPQ / SPQ (Minimum/Standard Package Quantity) | 一个包装单位的固定数量，订货必须按它的整数倍 | 采购与物流实务 | 和 MOQ 混用。MOQ 是**一次订多少的下限**，MPQ 是**订量的步长**，两者共同决定实际库存下界 |
| 年降 | Annual Price Reduction / LTA (Long-Term Agreement) 降价条款 | 合同约定每年按一定比例下调单价，通常假设供应商靠学习曲线与规模消化 | 汽车/电子行业实务 | 以为年降是白拿的。年降压到成本线以下，供应商就会**降配、拖交期或退出**，成本转成质量风险 |
| 产品质量先期策划 | APQP (Advanced Product Quality Planning) | 新产品从立项到量产的结构化质量策划流程，含五个阶段与阶段评审 | AIAG APQP 第 3 版（2024 年 3 月） | 以为 APQP 是一套表格。它是**跨职能的阶段门流程**，表格只是证据 [T06-S017] |
| 生产件批准程序 | PPAP (Production Part Approval Process) | 供应商用规定的一套证据（含 PSW 提交保证书）证明其量产过程能稳定造出合格件 | AIAG PPAP 第 4 版 | 以为 PPAP 是首件检验。PPAP 批的是**过程**（在量产工装、量产节拍下的能力），不只是那几个样件 [T06-S017] |
| 提交等级 | PPAP Submission Level 1-5 | 客户指定要提交多少证据（从只交 PSW 到全套资料现场评审） | AIAG PPAP | 默认都是 Level 3。等级由**客户指定**，猜错会直接导致提交被退回 |
| 供应商审核 / 审厂 | Supplier Audit（过程审核 VDA 6.3 / 体系审核） | 到供应商现场按检查表评估其体系、过程或产品的符合性与能力 | VDA 6.3、IATF 16949 体系；行业实务 | 把审厂当成看看厂房干不干净。有效审核看的是**过程能力证据与异常响应记录** |
| 多级供应链可视 | Multi-Tier Visibility / Sub-Tier Mapping | 不只看直接供应商（Tier 1），还要摸清 Tier 2/3 乃至原料产地 | 供应链风险管理；UFLPA/CSDDD 等法规也在倒逼 | 以为 Tier 1 说没问题就行。风险往往**卡在你没听说过的 Tier 3 独家小厂**，且合规责任不因不知情而免除 [T06-S027][T06-S028] |
| 供应商绩效评分卡 | Supplier Scorecard | 用质量（PPM）、交付（OTD）、成本、响应等维度定期给供应商打分并分级 | 采购实务；IATF 16949 明确要求监控 | 只考核价格与到货率。不含**变更通知与异常响应**的评分卡，抓不到最贵的那类风险 [T06-S013] |
| 供应商变更通知 | PCN / SCN (Product / Supply Change Notification) | 供应商在更换材料、工艺、产地或停产前必须提前书面通知客户 | 电子/汽车行业实务；IATF 16949 要求 | 以为「反正是同样的料」。未申报变更是**批量质量事故的头号来源**，也是 PPAP 需要重做的触发条件 |
| 关键件 / 长周期件 | Long-Lead Item | 采购提前期显著长于其他物料、决定整机可承诺交期的物料 | 采购与计划实务 | 按统一策略管所有料号。长周期件必须**单独提前锁定或备货**，否则累计提前期永远压不下来 |

---

## B. 标准 / 框架 / 认证

### B1. 供应链参考模型与职业认证

| 标准/认证 | 发布机构 | 覆盖什么 | 最近一次更新 | 谁需要 |
|---|---|---|---|---|
| **SCOR / SCOR-DS**（Supply Chain Operations Reference – Digital Standard） | ASCM（Association for Supply Chain Management，前身 APICS） | 供应链的**通用过程语言 + 指标 + 实践 + 人员技能**四层参考模型。SCOR-DS 把原来的 Plan/Source/Make/Deliver/Return/Enable 重构为 **Orchestrate（OE）、Plan（P）、Order（O）、Source（S）、Transform（T）、Fulfill（F）、Return（R）** 七个一级过程：Deliver 拆成 Order 与 Fulfill，Make 改称 Transform，Enable 升格为 Orchestrate；并把可持续/循环供应链纳入模型 | SCOR-DS 于 **2022 年 9 月**发布并转为在线开放访问；ASCM 持续发版（最新为 SCOR Version 14.0，2025 年信息模型文档以 CC BY-NC-ND 4.0 发布） | 做供应链诊断、跨公司对标、ERP/APS 蓝图设计的人；写 RFP 与 SOW 时用它做统一过程语言 [T06-S001][T06-S004][T06-S050] |
| **SCOR 性能属性与指标** | ASCM | 五个性能属性：可靠性（Reliability）、响应性（Responsiveness）、敏捷性（Agility）、成本（Costs）、资产管理效率（Asset Management Efficiency）；各挂 Level-1 指标如 Perfect Order Fulfillment、Order Fulfillment Cycle Time | 随 SCOR-DS 同步 | 定 KPI 体系的人。注意：**指标要成组用**，只压成本必然牺牲可靠性 [T06-S001][T06-S004] |
| **CPIM**（Certified in Planning and Inventory Management） | ASCM / APICS | 企业内部的计划与库存：供应链战略、S&OP、需求与供应计划、详细排程、库存与配送管理、质量与技术驱动的持续改进 | **CPIM 8.0（考纲 2023 年 6 月 1 日生效）把原来的 Part 1 + Part 2 合并成一场考试**，7.0 版最后可考日为 2024 年 2 月 1 日 | 计划员、生产计划、库存管理、MRP/ERP 顾问。**中国制造业招计划经理时出现频率最高的一张证** [T06-S008][T06-S055] |
| **CSCP**（Certified Supply Chain Professional） | ASCM / APICS | 端到端的**外部**供应链：全球化、寻源、物流（正向与逆向）、供应链关系、风险管理、优化、可持续与新技术 | 考纲定期换版 | 供应链总监、S&OP/网络设计、跨企业协同岗位 [T06-S008] |
| **CLTD**（Certified in Logistics, Transportation and Distribution） | ASCM / APICS | 物流战略、需求与产能管理、订单履行、仓储与库存、运输、全球物流、逆向物流与风险 | 考纲定期换版 | 物流、仓储、运输、进出口岗位 [T06-S008] |
| **CTSC**（Certified in Transformation for Supply Chain） | ASCM | 供应链**转型**的诊断、设计与落地：把高层战略翻译成可执行的端到端改造 | ASCM 近年新增的认证，是四张证里最新的一张 | 负责供应链变革项目、数字化转型的负责人 [T06-S008] |

### B2. 管理体系标准（ISO / IATF）

| 标准 | 发布机构 | 覆盖什么 | 最近一次更新 | 谁需要 |
|---|---|---|---|---|
| **ISO 9001** 质量管理体系 | ISO（国际标准化组织），TC 176/SC 2 | 组织级质量管理体系要求：过程方法、风险思维、领导作用、供方控制、纠正措施 | ISO 9001:2015 是长期现行版；改版工作 2023 年立项，开发轨道延长到 36 个月并加了第二次委员会草案，**ISO 官方口径为 2026 年 9 月发布 ISO 9001:2026**；已认证组织将获得过渡期（通常按认证周期约三年，以 IAF 决议为准）。**(Decay risk: high — 就在本月切版，务必现查 iso.org 的发布状态与 IAF 过渡决议)** | 几乎所有 B2B 制造与服务供应商；客户审核的最低门槛 [T06-S024][T06-S025] |
| **ISO 14001** 环境管理体系 | ISO | 环境管理体系要求：环境因素识别、合规义务、目标与绩效评价，近年强化气候相关议题 | **ISO 14001:2026 已于 2026 年 4 月发布**，认证组织需在其认证周期设定的时限内完成过渡 | 有环保监管压力、客户 ESG 问卷或 CSDDD/CBAM 上游要求的制造企业 [T06-S026] |
| **ISO 28000** 供应链安全管理体系 | ISO | 供应链**安全与韧性**管理体系要求（防盗、防篡改、货物完整性、场所与运输安全），与 ISO 31000 风险管理、ISO 22301 业务连续性对齐 | **ISO 28000:2022（第二版）** 取代 2007 版；改为「安全与韧性 — 安全管理体系」定位 | 跨境物流、保税与高价值货物运输、需要向客户证明货物完整性的企业 [T06-S029] |
| **IATF 16949** 汽车行业质量管理体系 | IATF（International Automotive Task Force），必须与 ISO 9001 一起实施 | 在 ISO 9001 之上叠加汽车行业要求：核心工具、供应商开发、产品安全、变更管理、防错、总成本 | 标准正文仍是 **IATF 16949:2016**，但通过 **Sanctioned Interpretations（SI，认可解释）** 持续演进；**《Rules for achieving and maintaining IATF Recognition》第 6 版 2024 年 4 月发布、2025 年 1 月 1 日生效**；2025 年 11 月又发布了针对 Rules 6th 与 IATF 16949 的新一批 SI（含 SI 19/20/21 与 IATF 16949 SI #27-30）。**(Decay risk: high — SI 是滚动发布的，审核依据以最新 SI 为准)** | 汽车 OEM 的一级/二级供应商；没有它基本进不了主机厂供应商名录 [T06-S013][T06-S030] |

### B3. AIAG 汽车核心工具

AIAG（Automotive Industry Action Group，美国汽车行业行动集团）发布的「核心工具」是 IATF 16949 落地时客户必然会查的一套手册。**各手册版本近年集中换代，是本行最容易过时的一块知识。**

| 手册 | 发布机构 | 覆盖什么 | 最近一次更新 | 谁需要 |
|---|---|---|---|---|
| **APQP** 产品质量先期策划 | AIAG | 新产品开发的五阶段策划与阶段门评审，从立项、设计、过程开发到试产与量产反馈 | **第 3 版，2024 年 3 月**（引入敏捷产品管理相关更新，并把 Control Plan 拆出去独立成册） | 新项目 PM、SQE、工艺工程师 [T06-S017] |
| **Control Plan** 控制计划 | AIAG | 逐工序的控制特性、规格、测量系统、抽样计划与反应计划 | **第 1 版，2024 年 3 月**（首次独立成册，此前是 APQP 手册的一部分）。**(Decay risk: high — 很多国内教材还按旧结构讲)** | 工艺、质量、产线班组长 [T06-S017] |
| **PPAP** 生产件批准程序 | AIAG | 量产前向客户提交的证据包（含 PSW 提交保证书）与五个提交等级 | **第 4 版** | 供应商质量、SQE、新品导入 [T06-S017] |
| **FMEA**（AIAG & VDA FMEA Handbook） | AIAG 与 VDA（德国汽车工业协会）联合 | DFMEA、PFMEA 与 FMEA-MSR（监控与系统响应）；**7 步法**取代旧流程，**AP（Action Priority）表取代 RPN**，S/O/D 评分表全面重写 | **第 1 版（2019 年发布），2022 年 8 月第二次印刷**；有中文等多语种版本 | 所有汽车链上的设计与工艺工程师。**还在用 RPN>100 作为整改门槛的组织，审核时会被直接开不符合** [T06-S017][T06-S031] |
| **MSA** 测量系统分析 | AIAG | 量具的偏倚、线性、稳定性、重复性与再现性（Gage R&R）评价方法 | **第 4 版** | 质量工程师、计量、实验室 [T06-S017] |
| **SPC** 统计过程控制 | AIAG 与 VDA 联合（AIAG & VDA SPC Manual） | 控制图选择与判异规则、过程能力（Cp/Cpk）与过程性能（Pp/Ppk）的计算与前提 | **AIAG & VDA SPC Manual 第 1 版，2026 年 7 月**，是对旧 AIAG SPC 手册的重大改版。**(Decay risk: high — 刚换版不到两个月)** | 质量工程师、工艺、产线数据分析 [T06-S017] |

### B4. 贸易与物流术语标准

| 标准 | 发布机构 | 覆盖什么 | 最近一次更新 | 谁需要 |
|---|---|---|---|---|
| **Incoterms® 2020** 国际贸易术语解释通则 | ICC（International Chamber of Commerce，国际商会） | 11 条贸易术语（EXW、FCA、CPT、CIP、DAP、DPU、DDP 七条适用任何运输方式；FAS、FOB、CFR、CIF 四条仅适用海运及内河运输），界定买卖双方的**交货点、风险转移点、费用划分与单证义务** | **2020 年 1 月 1 日生效**；相对 2010 版最显著的变化是 DAT 改名并改义为 **DPU（Delivered at Place Unloaded）**，且 CIP 的默认保险等级提高。ICC 通常约每十年修订一次 | 外贸、采购、物流、法务；写合同的人。**Incoterms 只管交货与风险，不管所有权转移、不管付款、不代替买卖合同** [T06-S032] |
| **GS1 标识与条码标准**（GTIN / SSCC / GLN / EPCIS） | GS1 | 全球统一的商品、物流单元、地点标识与事件数据交换标准，是多级追溯与数字护照落地的底层编码 | 持续更新的标准族 | 快消/零售供应链、需要向下游做批次追溯的制造企业 [T06-S033] |

### B5. 精益与六西格玛认证体系

| 体系 | 发布机构 | 覆盖什么 | 最近一次更新 | 谁需要 |
|---|---|---|---|---|
| **Shingo Model / Shingo Prize** | Shingo Institute（美国犹他州立大学 Jon M. Huntsman 商学院下属） | 以**指导原则（Guiding Principles）**而非工具为核心的卓越运营模型，分四个维度：文化促成因素（Cultural Enablers）、持续改进（Continuous Improvement）、企业协同（Enterprise Alignment）、结果（Results）；评审看的是**行为（KBI 关键行为指标）**而不是工具清单 | Shingo Institute 会发布模型更新（见其 Model Changes 页） | 想把精益从「工具项目」推进到「文化与行为」的组织；Shingo Prize 是精益领域国际认可度最高的奖项之一 [T06-S034] |
| **ASQ 六西格玛绿带 CSSGB / 黑带 CSSBB** | ASQ（American Society for Quality，美国质量协会） | 绿带 BoK 按 DMAIC 分章（Overview/Define/Measure/Analyze/Improve/Control）；黑带 BoK 九大领域，另含组织层部署、团队管理与 DFSS | BoK 定期换版（如 2022 版 BoK） | 质量与改进岗位。**黑带必须提交完成的项目（1 个带宣誓书的项目 + 2 个项目的选项）才有报考资格**——这是它和多数「培训机构发的黑带证」最大的区别 [T06-S035][T06-S036] |
| **精益认证的现实** | — | 市面上大量「绿带/黑带」由培训机构自行颁发，不涉及项目审核与统一考纲 | — | 招人时要问清**发证机构 + 是否有项目要求**；只看「黑带」两个字没有信息量 |

### B6. 合规新变量（2024-2026）

> 这一整节 **(Decay risk: high)**：四项法规在 2024-2026 年间都在改，且改的是**生效时间和适用门槛**，不是细节。任何超过三个月的二手总结都可能是错的，用之前必须回官方页面核对。

#### B6.1 欧盟企业可持续尽责指令 CSDDD / CS3D — **(Decay risk: high)**

- **谁发布**：欧盟（Directive (EU) 2024/1760，2024 年 7 月 25 日生效），由各成员国转化为国内法后执行。
- **覆盖什么**：要求在范围内的大企业对**自身经营、子公司以及产业链上下游合作伙伴**的人权与环境不利影响做识别、预防、缓解与救济，并制定气候转型计划。
- **时间线（关键，已被改过两次）**：原本要求成员国 **2026 年 7 月 26 日**前完成转化。经 Omnibus I 简化包（Directive (EU) 2025/794 与 Directive (EU) 2026/470）修订后，转化截止推迟到 **2028 年 7 月 26 日**、自 **2029 年 7 月 26 日**起适用；第 16 条的报告义务适用于 **2030 年 1 月 1 日**及以后开始的财年。适用门槛也被抬高到**员工 > 5000 人且净营业额 > 15 亿欧元**。欧盟理事会已于 2026 年 2 月 24 日为该简化方案背书。
- **对供应商管理的实际影响**：直接受管辖的中国供应商很少，但**你的欧洲客户会把义务通过合同条款下推**——供应商行为准则、尽责问卷、现场审核权、整改期限与终止条款。真正要提前准备的是「**能不能说清楚自己的二三级供应商是谁**」。[T06-S028][T06-S037][T06-S038]

#### B6.2 碳边境调节机制 CBAM — **(Decay risk: high)**

- **谁发布**：欧盟委员会税收与海关总署（DG TAXUD）执行。
- **覆盖什么**：对进口的钢铁、铝、水泥、化肥、电力、氢等高碳产品，按其**内含排放量**要求进口方购买 CBAM 证书，把欧盟碳价延伸到进口环节。
- **时间线**：**过渡期 2023 年 10 月 — 2025 年 12 月**，只需按季度申报内含排放、不付费；**确定期自 2026 年 1 月 1 日起生效**。年进口量超过 **50 吨**单一质量门槛的进口商必须申请「授权 CBAM 申报人」资格（2026 年初已有 4100+ 经营者取得）。2026 年度的申报与购证：证书自 **2027 年 2 月**起可购买，年度申报须在 **2027 年 9 月 30 日**前提交。
- **对供应商管理的实际影响**：欧洲客户会向中国供应商索要**逐产品的内含排放数据与核算方法**，且要能追到冶炼/熟料等上游工序。没有数据的默认值通常更不利，等于变相涨价。**产品碳足迹核算能力正在变成一项供应商准入条件。**[T06-S039][T06-S040]

#### B6.3 美国《维吾尔强迫劳动预防法》UFLPA — **(Decay risk: high)**

- **谁发布**：美国国会立法（2021 年 12 月 23 日签署），由 DHS 下属的强迫劳动执法工作组（FLETF）维护实体清单，CBP（海关与边境保护局）在口岸执法。
- **覆盖什么**：确立**可反驳推定**——凡全部或部分在新疆维吾尔自治区开采/生产/制造，或由实体清单上的企业生产的货物，一律推定为强迫劳动产品，依 19 U.S.C. § 1307 禁止进入美国。推定自 **2022 年 6 月 21 日**起生效。
- **时间线与规模**：实体清单持续扩容，**截至 2026 年 8 月已有 187 家实体在列**（2026 年 7 月 31 日一次性新增 43 家）；自法案实施以来 CBP 已拒绝入境超过 24,300 批货物、货值近 10 亿美元。
- **对供应商管理的实际影响**：这是四项里对**多级供应链可视化**要求最硬的一项。举证责任在进口方，要「清晰且令人信服」地追溯到原料层（棉花、多晶硅、番茄、铝、锂等重点品类），需要的是**逐级采购凭证、生产记录、物流单据的证据链**，而不是一纸供应商声明。**「我不知道我的三级供应商是谁」在这里不是免责事由。**[T06-S027][T06-S041][T06-S042]

#### B6.4 欧盟电池法规与数字电池护照 — **(Decay risk: high)**

- **谁发布**：欧盟（Regulation (EU) 2023/1542，电池与废电池法规），欧盟委员会内部市场总署发布落地指南。
- **覆盖什么**：碳足迹声明、有害物质限制、再生料含量、性能与耐久性、**电池尽责调查义务**（原材料负责任采购），以及**数字电池护照**。
- **时间线**：自 **2027 年 2 月 18 日**起，每一块投放市场的电动汽车电池、轻型交通工具（LMT）电池以及容量 > 2 kWh 的工业电池都必须具备电池护照。欧盟委员会已于 **2026 年 8 月**发布更新版《数字电池护照指南》，逐数据点标明哪些是强制、可选、条件适用或 2027 年 2 月暂不要求。尽责调查义务部分已被 **Regulation (EU) 2025/1561（2025 年 7 月 18 日）** 修订。
- **对供应商管理的实际影响**：电池护照本质是一条**贯穿多级供应商的产品级数据链**（材料来源、碳足迹、再生料比例、生产批次），单靠整车厂或电芯厂自己填不出来。正极材料、电解液、箔材等上游供应商会被要求按统一数据点提供可核验数据，**这是把 GS1 式的标识与 EPCIS 式的事件数据真正逼进生产端的第一个大规模案例**。[T06-S043][T06-S044][T06-S045]

---

## C. 「说这个词就露馅」清单

下面每一条都是**一句话就能让老手判断你没在现场待过**的说法。左边是常见错法，右边是正确说法。

| # | 露馅的说法 | 为什么错 | 正确说法 |
|---|---|---|---|
| C1 | 「我们的 **cycle time** 是 30 天」 | cycle time 是**一道工序连续产出两件之间的间隔**，单位通常是秒或分钟。30 天那个数是 lead time | 「我们的**订单交付提前期（lead time）**是 30 天，其中装配的 **cycle time** 是 45 秒，其余是排队、等料和运输」。要报数就先报口径：从哪个事件开始、到哪个事件结束 |
| C2 | 「这条线**产能利用率 95%**，管理得很好」 | 排队论里等待时间随利用率上升而非线性爆炸（ρ/(1−ρ)），95% 利用率通常意味着交期长、插单频繁、加急成常态 | 「**瓶颈工序**利用率 95%，非瓶颈工序有意留出缓冲」。高利用率只在**瓶颈**上是好事；对非瓶颈追求高利用率只会堆在制品 [T06-S020][T06-S046] |
| C3 | 「**安全库存**我们一般备半个月」 | 安全库存是**按目标服务水平和需求/提前期的波动算出来的**（z·σ·√L 那一类），不是拍脑袋的天数 | 「按 **95% 周期服务水平**、需求标准差 σ 和提前期波动算出来是 X 件，折合 Y 天」。要降库存先降**波动和提前期**，不是直接砍那个天数 [T06-S007] |
| C4 | 「我们搞 **JIT**，目标是**零库存**」 | JIT 是「只在需要的时候、按需要的量做需要的东西」，反对的是**过量与提前**；丰田自己在关键点保有标准在制品与缓冲 | 「我们用 JIT/拉动来**消除过量生产**，在解耦点保留有意设计的缓冲」。把库存归零而不改前置条件，等于把风险转嫁给供应商和加急运费 [T06-S009][T06-S010] |
| C5 | 「我们上了 **kanban**，就是车间那块看板」 | kanban 是**限制在制品数量的补货授权信号**（卡不回来就不许生产）；一块没有数量上限的白板不是看板系统 | 「我们用**看板卡（或电子看板）做拉动补货**，卡数决定在制品上限」。判据是：**卡的数量是不是真的限制了投料** [T06-S011] |
| C6 | 「**瓶颈**就是最忙的那个工位」 | 最忙可能只是批量太大、排班不合理或数据错误。瓶颈的判据是**产能 < 需求**，且它决定全线产出 | 「瓶颈是**需求超过其产能、决定整线产出**的那个资源」。找瓶颈先看产能对需求的比值和缓冲消耗趋势，不是看谁前面料堆得高 [T06-S014] |
| C7 | 「**MRP** 帮我们排产」 | MRP 只算「要什么、要多少、什么时候要」，**默认产能无限**；排产（哪台设备几点做什么）是 APS/详细排程的事 | 「MRP 出**物料需求**，APS/排程在**有限产能**下出可执行序列，两者中间还要过一道产能校验（RCCP/CRP）」 [T06-S002] |
| C8 | 「这个料是 **sole source**，我们打算再开发一家」 | 能再开发一家就说明市场上不止一家，那叫 **single source**（自己选的独家）。**sole source** 是市场上只有这一家（专利、独占产能、客户指定） | 「这是 **single source**，我们计划导入第二家做 dual source」/「这是 **sole source**，只能靠安全库存、长约锁产能或替代设计来化解」。**两个词的风险对策完全不同** |
| C9 | 「我们 **OTIF 95%**，其中准时 97%、足量 98%」 | OTIF 是**逻辑与**：一单必须同时准时且足量才计入。分别报两个数再说 OTIF 95% 往往是算错了 | 「**准时且足量**的订单行占比 95%」，并说明分母是订单、订单行还是数量口径 |
| C10 | 「我们 **FMEA** 做完了，RPN 超过 100 的都整改了」 | AIAG-VDA FMEA 手册已用 **AP（Action Priority）查表分级**取代 RPN 乘积排序，正是为了消除 RPN 相乘造成的错误优先级 | 「按 **AP 表**分出 H/M/L，H 必须有措施、M 需说明理由」。还在用 RPN 门槛的，客户审核会直接问版本 [T06-S017][T06-S031] |
| C11 | 「**PPAP** 就是首件检验」 | PPAP 批准的是**过程**：在量产工装、量产节拍、量产人员条件下能稳定造出合格件，提交的是一整套证据包（含 PSW） | 「PPAP 是**过程批准**，首件检验（FAI）是每次换型后对第一件产品的确认，两者目的和触发条件都不同」 [T06-S017] |
| C12 | 「**Cpk 1.67**，这个过程没问题」 | Cpk 只有在过程**处于统计受控状态**（控制图无异常）时才有意义；不稳定的过程算出的 Cpk 是虚数 | 「过程先经 SPC 判稳，再算 Cpk = 1.67」。另外要说清是 **Cpk（组内短期）还是 Ppk（整体长期）**，两者常差一截 [T06-S015] |
| C13 | 「**Incoterms** 里 FOB，所以货权在装船时转移给买方」 | Incoterms 规定的是**交货点、风险转移与费用划分**，**不规定所有权（货权）转移**，也不规定付款条件 | 「FOB 下**风险**在货物装上船时转移；**所有权**转移按买卖合同和适用法律另行约定」 [T06-S032] |
| C14 | 「我们只用 Tier 1 供应商的合规声明就够了」 | UFLPA 下举证责任在进口方，要求追溯到原料层的证据链；CSDDD/电池法规同样把义务推到多级 | 「我们做了 **sub-tier mapping**，对重点品类保留逐级的采购凭证、生产记录与物流单据」。**不知情不构成免责** [T06-S027][T06-S041] |

---

## Source Manifest

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T06-S001 | https://www.ascm.org/corporate-solutions/standards-tools/scor-ds/ | verified_primary | 2026-09-02 | ASCM | association, SCOR originator |
| T06-S002 | https://docs.oracle.com/cd/A60725_05/html/comnls/us/mrp/gls.htm | surrogate_primary | 2026-09-02 | Oracle | vendor docs, MRP and Supply Chain Planning glossary |
| T06-S003 | https://arxiv.org/pdf/2402.14506 | verified_primary | 2026-09-02 | arXiv | academic preprint, rolling-horizon production planning |
| T06-S004 | https://www.ascm.org/globalassets/ascm_website_assets/docs/scor/information-model-scor-digital-standard-2025.pdf | verified_primary | 2026-09-02 | ASCM | association, SCOR-DS information model (SCOR v14.0) |
| T06-S005 | https://www.gsb.stanford.edu/faculty-research/publications/information-distortion-supply-chain-bullwhip-effect | verified_primary | 2026-09-02 | Stanford GSB | academic, bullwhip-effect originator paper (Lee/Padmanabhan/Whang) |
| T06-S006 | https://dspace.mit.edu/bitstream/handle/1721.1/126955/1191622819-MIT.pdf | verified_primary | 2026-09-02 | MIT DSpace | academic thesis, risk pooling for spare parts |
| T06-S007 | https://ocw.mit.edu/courses/15-760a-operations-management-spring-2002/9c5b7fa103a68eb27bb0c3b62cfd9d6a_lecture7_feb20.pdf | verified_primary | 2026-09-02 | MIT OpenCourseWare | academic course material, MRP/ERP and inventory models |
| T06-S008 | https://www.ascm.org/learning-development/certifications-credentials/ | verified_primary | 2026-09-02 | ASCM | certification body, APICS CPIM/CSCP/CLTD/CTSC |
| T06-S009 | https://global.toyota/en/company/vision-and-philosophy/production-system/ | verified_primary | 2026-09-02 | Toyota Motor Corporation | originator of the Toyota Production System |
| T06-S010 | https://global.toyota/en/company/plant-tours/production-system/index.html | verified_primary | 2026-09-02 | Toyota Motor Corporation | originator, official TPS plant-tour explainer |
| T06-S011 | https://www.lean.org/lexicon-terms/jidoka/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator |
| T06-S012 | https://www.lean.org/explore-lean/lexicon-terms/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (terms index) |
| T06-S013 | https://www.iatfglobaloversight.org/iatf-169492016/iatf-169492016-sis/ | verified_primary | 2026-09-02 | IATF | certification body oversight, IATF 16949 sanctioned interpretations |
| T06-S014 | https://www.tocico.org/page/ref_bank1 | verified_primary | 2026-09-02 | TOCICO | certification body for Theory of Constraints |
| T06-S015 | https://asq.org/quality-resources/process-capability | verified_primary | 2026-09-02 | ASQ | association, process capability Cp/Cpk body of knowledge |
| T06-S016 | https://asq.org/quality-resources/dmaic | verified_primary | 2026-09-02 | ASQ | association, DMAIC reference |
| T06-S017 | https://www.aiag.org/expertise-areas/quality/quality-core-tools | verified_primary | 2026-09-02 | AIAG | association, automotive core tools originator |
| T06-S018 | https://arxiv.org/pdf/2503.05749 | verified_primary | 2026-09-02 | arXiv | academic, Operations & Supply Chain Management: Principles and Practice |
| T06-S019 | https://www.lean.org/lexicon-terms/overall-equipment-effectiveness/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (OEE) |
| T06-S020 | https://arxiv.org/pdf/1901.02926 | verified_primary | 2026-09-02 | arXiv | academic, Little's Law and system performance models |
| T06-S021 | https://help.sap.com/docs/SAP_ERP/a0d3efbac8b14fc89b29bf47a1677c86/cd90b853ff98b44ce10000000a174cb4.html | surrogate_primary | 2026-09-02 | SAP | vendor docs, assemble-to-order process definition |
| T06-S022 | https://help.sap.com/docs/SAP_SUPPLY_CHAIN_MANAGEMENT/15f45255438149fa996da194295b132b/3024fe50b894c557e10000000a44176d.html | surrogate_primary | 2026-09-02 | SAP | vendor docs, Global Available-to-Promise |
| T06-S023 | https://hbr.org/1983/09/purchasing-must-become-supply-management | verified_primary | 2026-09-02 | Harvard Business Review | academic/practitioner journal, Kraljic matrix originator |
| T06-S024 | https://www.iso.org/standard/62085.html | verified_primary | 2026-09-02 | ISO | international standards association, ISO 9001:2015 originator |
| T06-S025 | https://committee.iso.org/sites/tc176sc2/home/news/content-left-area/news-and-updates/Update%20-%20Revision%20of%20ISO%209001.html | verified_primary | 2026-09-02 | ISO/TC 176/SC 2 | association committee, ISO 9001 revision status |
| T06-S026 | https://www.iso.org/news/2026/04/iso-14001-2026-published | verified_primary | 2026-09-02 | ISO | association, ISO 14001:2026 publication announcement |
| T06-S027 | https://www.dhs.gov/uflpa-entity-list | verified_primary | 2026-09-02 | U.S. DHS / FLETF | regulator, UFLPA Entity List |
| T06-S028 | https://eur-lex.europa.eu/eli/dir/2024/1760/oj/eng | verified_primary | 2026-09-02 | EUR-Lex (EU) | regulator, CSDDD Directive (EU) 2024/1760 consolidated text |
| T06-S029 | https://www.iso.org/obp/ui/#!iso:std:79612:en | verified_primary | 2026-09-02 | ISO | association, ISO 28000:2022 online browsing platform entry |
| T06-S030 | https://www.iatfglobaloversight.org/wp/wp-content/uploads/2025/11/IATF-Stakeholder-Communique-SC-2025-003-Release-of-Sanctioned-Interpretations-SIs-and-Frequently-Asked-Questions-FAQs-related-to-Rules-6th-Edition-and-IATF-16949.pdf | verified_primary | 2026-09-02 | IATF | certification body oversight, Nov 2025 SI/FAQ release |
| T06-S031 | https://www.aiag.org/training-and-resources/manuals/details/FMEAAV-1 | verified_primary | 2026-09-02 | AIAG | association, AIAG & VDA FMEA Handbook edition details |
| T06-S032 | https://iccwbo.org/business-solutions/incoterms-rules/incoterms-2020/ | verified_primary | 2026-09-02 | ICC | association, Incoterms rules originator |
| T06-S033 | https://www.gs1.org/standards/traceability | verified_primary | 2026-09-02 | GS1 | association, global identification and traceability standards originator |
| T06-S034 | https://shingo.org/shingo-model/ | verified_primary | 2026-09-02 | Shingo Institute | association, Shingo Model originator |
| T06-S035 | https://www.asq.org/cert/six-sigma-black-belt | verified_primary | 2026-09-02 | ASQ | certification body, CSSBB eligibility and exam |
| T06-S036 | https://www.asq.org/cert/resource/pdf/certification/2022-SSGB-BoK.pdf | verified_primary | 2026-09-02 | ASQ | certification body, Six Sigma Green Belt body of knowledge |
| T06-S037 | https://commission.europa.eu/topics/business-and-industry/doing-business-eu/sustainability-due-diligence-responsible-business/corporate-sustainability-due-diligence_en | verified_primary | 2026-09-02 | European Commission | regulator, CSDDD topic page and amended timeline |
| T06-S038 | https://www.consilium.europa.eu/en/press/press-releases/2026/02/24/council-signs-off-simplification-of-sustainability-reporting-and-due-diligence-requirements-to-boost-eu-competitiveness/ | verified_primary | 2026-09-02 | Council of the European Union | regulator, Omnibus I simplification sign-off |
| T06-S039 | https://taxation-customs.ec.europa.eu/carbon-border-adjustment-mechanism/cbam-definitive-regime_en | verified_primary | 2026-09-02 | European Commission DG TAXUD | regulator, CBAM definitive regime |
| T06-S040 | https://taxation-customs.ec.europa.eu/news/cbam-successfully-entered-force-1-january-2026-2026-01-14_en | verified_primary | 2026-09-02 | European Commission DG TAXUD | regulator, CBAM entry into force 1 Jan 2026 |
| T06-S041 | https://www.cbp.gov/trade/forced-labor/UFLPA | verified_primary | 2026-09-02 | U.S. Customs and Border Protection | regulator, UFLPA enforcement and importer due diligence |
| T06-S042 | https://www.dhs.gov/news/2026/07/31/dhs-announces-addition-43-companies-uflpa-entity-list | verified_primary | 2026-09-02 | U.S. DHS | regulator, Entity List expansion July 2026 |
| T06-S043 | https://eur-lex.europa.eu/eli/reg/2023/1542/oj/eng | verified_primary | 2026-09-02 | EUR-Lex (EU) | regulator, EU Batteries Regulation (EU) 2023/1542 |
| T06-S044 | https://single-market-economy.ec.europa.eu/news/guidance-support-preparations-digital-batteries-passport-2026-08-21_en | verified_primary | 2026-09-02 | European Commission DG GROW | regulator, Digital Batteries Passport guidance (Aug 2026) |
| T06-S045 | https://eur-lex.europa.eu/eli/reg/2025/1561/oj/eng | verified_primary | 2026-09-02 | EUR-Lex (EU) | regulator, amendment on battery due diligence obligations |
| T06-S046 | https://arxiv.org/pdf/2605.27202 | verified_primary | 2026-09-02 | arXiv | academic, Kingman's formula and utilization-variability queueing |
| T06-S047 | https://help.sap.com/docs/SAP_SUPPLY_CHAIN_MANAGEMENT/15f45255438149fa996da194295b132b/1242c95360267614e10000000a174cb4.html | surrogate_primary | 2026-09-02 | SAP | vendor docs, Capable-to-Promise (CTP) |
| T06-S048 | https://www.lean.org/lexicon-terms/muda-mura-muri/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (muda/mura/muri) |
| T06-S049 | https://www.lean.org/lexicon-terms/value-stream-mapping/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (VSM) |
| T06-S050 | https://www.kinaxis.com/en/blog/transform-your-supply-chain-using-ascms-scor-ds-model-peter-bolstorff | surrogate_primary | 2026-09-02 | Kinaxis | vendor docs, interview with ASCM's Peter Bolstorff on SCOR DS |
| T06-S051 | https://www.lean.org/lexicon-terms/takt-time/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (takt time) |
| T06-S052 | https://www.lean.org/lexicon-terms/heijunka/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (heijunka) |
| T06-S053 | https://www.lean.org/lexicon-terms/just-in-time-production/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (JIT / pull) |
| T06-S054 | https://www.lean.org/lexicon-terms/poka-yoke/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | nonprofit association, Lean Lexicon originator (poka-yoke) |
| T06-S055 | https://www.ascm.org/globalassets/ascm_website_assets/docs/ecm/ecm-cpim8.pdf | verified_primary | 2026-09-02 | ASCM | certification body, CPIM 8.0 exam content manual |
