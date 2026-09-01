# Track 02 — 工具地图：供应链与生产运营

> 蒸馏主题：制造业与消费品的实体供应链「计划—制造—交付」。
> 受众 locale：zh-CN。覆盖国际主流栈与中国本土栈两套。
> 最后核对：2026-09-02。所有来源见文末 Source Manifest。

---

## 0. 先说清楚：这行的「工具」不是一个软件清单

如果你把供应链与生产运营的工具地图画成「ERP / APS / MES / WMS 四个方框」，你会漏掉这行一半的工作量。这个领域的工具实际上分三层，而且三层是并列的、互相不能替代的：

**第一层是系统软件。** ERP 管账和主数据，MES（制造执行系统，管车间里每张工单实际发生了什么）管现场，APS（高级计划与排程）算什么时候做什么，WMS/TMS 管仓和运。这层是 IT 采购、有合同、有实施周期。

**第二层是方法工具。** 价值流图（VSM，把一个产品从下单到交付的每个物料流与信息流步骤画在一张纸上）、A3 报告、看板卡、标准作业票、SMED 换模记录表。这层几乎不花钱，用纸笔和白板就能做，但它决定了第一层的系统喂进去的是什么逻辑。一个没做过价值流图的工厂上 APS，等于把混乱自动化。Lean Enterprise Institute（精益企业研究院，精益方法在西方的主要传承机构）到今天仍然把 VSM 的模板做成可下载的表格发布，而不是做成一个软件产品——这本身就是一个信号：这层工具的价值在于强迫人走一遍思考流程，不在于工具本身 [T02-S007][T02-S009]。

**第三层是分析工具。** SQL、Python（pandas）、Excel、Power BI/Tableau、以及运筹优化求解器与仿真软件。这层是计划员和供应链分析师每天真正打字的地方。

一个常见的误判：以为「上了 ERP 就有计划能力了」。ERP 提供的是记账口径的物料需求计划（MRP），它假设产能无限、提前期固定。真正的产能约束、换型顺序、瓶颈保护，ERP 原生功能基本不解决，那是 APS 和方法工具的地盘。

**本文的分层口径**：必备层 = 这行 80% 以上从业者会碰到；场景特化层 = 特定履行模式、特定规模、特定职能才需要；新兴层 = 2025–2026 出现或大幅变化，还没有稳定的最佳实践。

---

## 1. 必备层（≥80% 从业者用到）

### 1.1 ERP / MRP —— 主数据与物料需求计划的底座

**SAP S/4HANA（PP 生产计划 + MM 物料管理）**

大型离散制造和流程制造的事实标准。S/4HANA 相对于老 ECC 最实质的变化是 MRP Live：物料需求净算直接在 HANA 内存数据库里完成，展开多层 BOM（物料清单）生成计划订单与采购申请，不再依赖过夜批处理 [T02-S001][T02-S002]。这句话的运营含义比技术含义大——它意味着计划员可以在一天里跑多次 MRP，而不是「今天下的单，明天早上才看到影响」。

MRP Live 还能和 PP/DS（生产计划与详细排程模块）混跑：在 location product 主数据上打了 advanced planning 标记的物料走 PP/DS 的有限产能算法，其余走标准 MRP [T02-S002]。这是 SAP 体系里「一部分产线要精细排程、一部分不需要」的标准做法。产品仍在演进——例如 MRP Live 生成的计划订单、采购申请、计划协议与库存转储申请可以触发业务事务事件（BTE），供外部系统订阅 [T02-S003]。

- **用在什么场景**：多工厂、多组织、需要合并报表与审计追溯的中大型制造企业；对流程合规要求高的行业（汽车、医药、航空）。
- **相对优劣**：主数据模型完整、行业方案深、生态大。代价是实施与变更成本高，任何流程变动都要经过配置与测试。
- **什么时候不该用**：单厂、产品线少于几百个 SKU、IT 团队不到 3 人的企业。这种规模上 SAP，实施费通常远超软件本身价值，且后续没人维护主数据，系统会在两年内退化成一个昂贵的库存台账。

**Oracle（Fusion Cloud SCM）/ NetSuite**

Oracle 在 2025 年 Gartner Supply Chain Planning Solutions 魔力象限中连续第三年被列为 Leader（Oracle 官方新闻稿口径，Gartner 原报告需付费获取）[T02-S018]。NetSuite 是 Oracle 体系里给中小企业的云 ERP，制造能力比 Fusion 弱得多，适合装配型、BOM 层数少的业务。

- **什么时候不该用 NetSuite**：多级 BOM 超过 4–5 层、有大量共用件与替代料、需要按工序排程的离散制造。NetSuite 的制造模块在这类场景会很快撞墙。

**Odoo**

开源起家的模块化 ERP，MRP 模块可用，二次开发门槛低。适合 50–300 人、有一两个愿意写 Python 的 IT、且愿意用「够用 + 自己改」换掉商业软件许可费的工厂。风险在于版本升级时自定义模块的兼容性，以及社区版与企业版功能差异。

值得注意的一个能力边界，官方文档说得很直白：Odoo 的主生产计划（MPS）是一个**手工工具**——把产品加进 MPS 不会自动触发生产或采购，它只给出建议数量，仍需人工创建制造单/采购单 [T02-S042]。而且官方明确建议**不要对同一个产品同时使用 MPS 和再订货规则（reordering rules）**，因为再订货规则是自动化流程，会与 MPS 的手工补货方式冲突 [T02-S042][T02-S043]。这类「两套补货逻辑打架」的坑在所有 ERP 里都存在，Odoo 只是把它写进了文档而已。

**关于实施周期与成本的诚实说法**

第三方口径（非厂商、非同行评议）给出的区间大致是：ERP 项目通常 6–18 个月，中型市场部署平均约 18 个月，比企业内部最初预估的时间线长约 30% [T02-S056]。成本方面，200 人规模的制造企业上中端 ERP，第三方咨询内容给出的区间是 20 万–50 万美元 [T02-S056]。预算超支是常态而非例外，Statista 汇总的全球调查显示相当比例的 ERP 项目超预算 [T02-S055]。

这些数字全部来自**咨询公司或厂商生态的内容营销**（包括 NetSuite 自己整理的 ERP 统计合集 [T02-S057]），样本口径不透明，**只能当作数量级参考，不能当作预算依据**。你自己的报价要向实施商索要同规模、同行业的三个可回访客户，那比任何行业均值有用。

**中国本土栈：用友、金蝶、鼎捷**

- **用友 U9 cloud**：定位中型及中大型制造业云 ERP，官方口径覆盖机械、电子、汽配、家具、整车、军工等细分行业，主打多组织多工厂的集团制造场景 [T02-S031]。
- **金蝶云·星空**：云原生架构，覆盖面广，中型制造与商贸混合业务的常见选择。
- **鼎捷（T100 / E10 / 易飞）**：三条产品线分别对应集团级、中大型、中小型，在台资背景的电子与精密制造圈子里渗透率高。

**关于市占率数字的诚实提示**：中文市场几乎每一家 ERP/MES 厂商都宣称自己在某个细分口径下「第一」。这些数字通常引用 IDC 或赛迪的付费报告，但公开可查的原始报告链接几乎都不存在，且口径互相排斥（「云化 MES」「SaaS MES」「制造业 ERP」是三个不同的分母）。**在选型文档里引用这些数字之前，先要求厂商提供原始报告页码。** 本文对所有此类数字一律标注为「厂商自报」，不作为事实使用。

**选型上的一个硬约束**：ERP 的选择在很大程度上决定了你后续能上什么 APS。SAP 生态里 IBP/PP-DS 的集成成本最低；用友/金蝶生态里，国产 APS 与本土 MES 的接口更成熟。跨生态集成（比如用友 ERP + Kinaxis）不是不能做，但主数据映射与增量同步的工作量往往被低估两到三倍。

### 1.2 Excel / 表格 —— 别装作它不存在

这行大量的需求计划、产能粗排、库存分析、供应商比价，今天仍然跑在 Excel 上。这不是从业者落后，是有结构性原因的：

1. **计划工作的本质是反复试算。** 计划员一天要问二十次「如果这批料晚三天到会怎样」。在 Excel 里改一个单元格三秒钟出结果；在 ERP 里改一个参数要走审批、跑批、等结果。
2. **计划的逻辑变化比 IT 排期快。** 一条新产线的排产规则可能一个月改三次，任何需要提工单的系统都跟不上。
3. **Excel 是唯一一个跨公司通用的界面。** 你的供应商不会为了给你交货计划去登录你的系统。

**什么时候必须迁走**：出现下面任何一条，Excel 就已经是负债而不是资产了。

- 同一个数据有两个以上版本的表在流通，且没人说得清哪个是最新的。
- 关键计算逻辑只存在于一个人的表里，这个人休假业务就停摆（业内俗称「Excel 单点故障」）。
- 数据量超过几十万行，或需要跨表关联超过三层，打开一次要几分钟。
- 需要审计追溯：谁在什么时候、基于什么假设改了这个计划。Excel 没有可信的版本与权限模型。
- 需要多人同时编辑同一个计划版本。

**迁移的正确姿势不是把 Excel 搬进 ERP。** 见第 5 节避坑清单第 2 条。中间态通常更现实：把数据层（取数、清洗、汇总）迁到 SQL + Python/Power BI，把试算层暂时留在 Excel，直到试算逻辑稳定到值得固化成系统功能为止。

### 1.3 方法工具（纸笔层）

这层工具的共同点：便宜、快、强迫跨部门当面对齐。它们在这行的地位和 ERP 一样是「工具」，不是「培训内容」。

**价值流图（Value Stream Mapping, VSM）**

把一个产品族从下单到交付的全部物料流与信息流步骤画在一张纸上，标出每步的加工时间、等待时间、库存量、良率、换型时间。LEI 的定义强调 VSM 比流程图和布局图更有力的地方在于它同时捕获信息流，而不只是物料流 [T02-S007][T02-S068]。这一点在计划场景里尤其关键——很多交期问题的根源不在加工慢，在于信息在哪里停住了（等审批、等确认、等排产会议）。这类等待在流程图上完全看不见。

- **用在什么场景**：改善项目立项前；上 MES/APS 前的现状盘点；交期长但说不清时间花在哪里的时候。
- **什么时候不该用**：产品种类极多且工艺路线各不相同的小批量多品种场景，画一个产品族的 VSM 得到的结论无法外推。这时候更该做的是按工艺路线聚类，或直接做瓶颈分析。
- **常见误用**：画完就挂墙上。VSM 的产出是「未来状态图 + 落地行动计划」，不是一张现状图。

**A3 报告**

丰田发源的做法：把问题、分析、对策、行动计划压缩到一张 A3 纸上，常配图表 [T02-S008]。它的价值不在纸的尺寸，在于它是一个**通过具体问题进行对话的管理过程**——上级不是批准 A3，而是通过追问帮下属把逻辑想通 [T02-S008]。

- **什么时候不该用**：当组织的真实决策发生在别的地方（比如老板一句话），A3 会退化成事后补的文档，纯浪费。

**看板卡（Kanban）**

物理卡片或电子信号，用于拉动式补货。适用于需求相对平稳、消耗频繁、品种数量可控的物料。
- **什么时候不该用**：需求极度不稳定、或单件价值极高且需求稀疏的物料。看板的前提是「消耗触发补货」，需求断续时会导致要么长期缺货要么长期压库。这类物料应该走 MRP 或者按订单采购。

**标准作业（Standard Work）与 SMED 换模记录表**

标准作业票记录节拍时间、作业顺序、在制品标准手持量。SMED（Single-Minute Exchange of Die，快速换模）的核心工具就是一张按秒记录的换模动作表，把动作分成「内部作业」（必须停机做的）与「外部作业」（可以在机器运行时做的），再想办法把内部转外部。

- **为什么在计划里重要**：换型时间是排程模型里最关键的参数之一。换型时间从 4 小时降到 40 分钟，经济批量、库存水位、可承诺交期全部要重算。**很多公司在没做 SMED 的情况下上 APS，结果 APS 算出的排程为了避开长换型而把批量做得巨大，然后大家抱怨系统「不智能」。** 问题不在系统。

**5S**

现场整理整顿。放在工具地图里的理由是：库存准确率和 5S 强相关。一个物料随手乱放的车间，ERP 里的库存数永远是错的，而库存准确率是上 APS 的前置条件（见第 4 节）。

### 1.4 流程参考模型：SCOR

SCOR（Supply Chain Operations Reference，供应链运作参考模型）不是软件，是一套**流程与指标的共同语言**。它由供应链协会提出、1996 年建立，2014 年供应链协会与 APICS 合并后由 ASCM 维护 [T02-S026][T02-S032]。当前的 SCOR Digital Standard 把供应链拆成六个一级流程：Plan、Order、Source、Transform、Fulfill、Return [T02-S027]。

**它在实务里的用法只有两个，而且都不是「照着做」**：

1. **对齐口径。** 当销售说的「交货周期」和工厂说的「生产周期」不是一件事时，SCOR 提供一套现成的定义，省掉三个月的扯皮。
2. **定指标体系。** SCOR 把流程、指标、最佳实践、技术挂在同一个框架上 [T02-S026]，可以直接拿来搭 KPI 树，而不用从零发明。

**什么时候不该用**：不要把 SCOR 当作流程再造的蓝图去逐条对标。它是参考模型不是标准答案，逐条落地会产生大量没人看的文档。

### 1.5 分析层：SQL / Python / BI

- **SQL**：从 ERP 数据库或数仓取数。这行的分析工作 70% 是取数与对数，不是建模。
- **Python + pandas**：做 ABC/XYZ 分类、库存健康度分析、预测误差分解、供应商交期分布分析。相对于 Excel 的优势是可复现、可版本管理、可处理百万行级。
- **Power BI / Tableau**：给管理层看的计划达成率、库存周转、OTIF（准时足量交付率）看板。
- **什么时候不该用 BI**：当你需要的是「让人做决定」而不是「让人知道现状」。BI 只呈现，不给建议、不写回系统。把控制塔当 BI 仪表盘用是这行最常见的浪费之一（见第 5 节）。

---

## 2. 场景特化层

### 2.1 APS 高级计划与排程

APS 与 ERP 的 MRP 的根本区别：MRP 假设产能无限、提前期是固定参数；APS 把产能、换型、物料齐套当作约束，算出的是有限产能下可执行的计划。

**Kinaxis（RapidResponse / Maestro）**

技术上的差异化是并发计算引擎：在一份实时数据模型上同时跑多个场景，让 S&OP（销售与运营计划，月度层面对齐销量、产能、财务）、S&OE（销售与运营执行，周/日层面处理偏差）、IBP 三个时间尺度共用一套数据。厂商与媒体口径都强调它的场景模拟（what-if）速度显著快于传统 ERP 的 MRP 重跑。Kinaxis 称自己是 2025 年 Gartner Supply Chain Planning Solutions 魔力象限里连续第十一次进 Leader 象限（厂商自报，Gartner 原报告付费）[T02-S015]。

- **用在什么场景**：多工厂、多层供应网络、需求波动大且需要频繁重排的离散制造（电子、汽车、工业设备、半导体）。特别适合合约制造（EMS/ODM）这种「客户天天改单」的业务。
- **什么时候不该用**：单厂、需求稳定、SKU 少的场景。并发引擎的价值在于「频繁重算 + 多方案对比」，需求稳定时这个能力用不上，你付的是没用到的钱。

**o9 Solutions**

用企业知识图谱（把供应链、商务、财务数据连成一张图）作为底层数据模型，把需求预测、供应计划、库存优化、收入管理、IBP 放在同一个平台上 [T02-S053]。o9 称在 2025 年 Gartner 魔力象限中被列为 Leader（厂商自报）[T02-S016]。求解侧 o9 自述使用启发式、线性规划、混合整数规划以及第三方求解器的组合 [T02-S053]——这句话值得注意，它意味着「优化」在这类平台里不是一个黑盒，而是一组可以被追问的算法选择。

- **相对 Kinaxis 的差别**：o9 更强调「商业侧与供应侧共用一个模型」，所以在需要销售、市场、财务深度参与计划的消费品与零售场景更顺；Kinaxis 在制造侧的物料与产能约束建模上历史更久。
- **什么时候不该用**：知识图谱建模需要企业先想清楚自己的业务对象关系。数据治理没做过的企业上 o9，最大的风险是建模阶段无限延长。

**Blue Yonder**

零售与消费品出身，强在需求预测、补货、以及计划到执行（WMS/TMS）的连续性。厂商自述平台架构是微服务 + Snowflake 数据底座，把计划、执行、商务放在一个多企业网络上 [T02-S039][T02-S038]。生产计划模块也有，但它的重心历史上一直偏向零售侧 [T02-S061]。第三方评测普遍提到学习曲线陡峭 [T02-S035]。

- **用在什么场景**：门店/DC 多级补货、促销驱动的需求、需要计划与仓配执行打通的消费品与零售。
- **什么时候不该用**：离散制造的工序级排程。这不是它的强项。

**SAP IBP**

SAP 生态内的计划平台（需求、库存、供应、S&OP、控制塔模块）。最大优势是与 S/4HANA 的主数据同源，集成成本最低。

技术上值得知道的一个区分，官方文档写得很清楚：IBP 的时间序列供应计划提供**启发式（heuristic）**与**优化器（optimizer）**两种引擎 [T02-S040]。启发式按规则逐层展开、速度快、结果可解释；优化器求解一个带成本项的数学模型，会给出目标函数值与下界，官方甚至提供「优化器运行详情」界面来看解质量随时间的收敛情况以及各成本项对结果的影响 [T02-S041]。

**这个区分是所有 APS 选型的通用问题，不只是 SAP 的**：

- **启发式**：结果可解释、计划员能看懂「为什么是这个答案」，但不保证最优。
- **优化器**：结果更优，但计划员往往说不清为什么，且成本参数（缺货成本、延迟成本、加班成本）一旦设错，会得到数学上最优、业务上荒谬的计划。
- **实务经验**：绝大多数企业上线第一年该用启发式。等计划员建立了对系统的信任、成本参数被现实校准过，再考虑优化器。**反过来做的项目，通常在第三个月被业务部门集体抵制。**

- **决策要点**：如果你已经是 S/4HANA 用户且计划逻辑不特别复杂，IBP 通常是总拥有成本最低的选择；如果你的计划逻辑是竞争优势的一部分，专业 APS 更值得。

**OMP**

流程行业（化工、造纸、金属、食品）的专精玩家。OMP 宣称在 2026 年 Gartner「流程行业供应链计划解决方案」魔力象限中在两个轴上都位置最高（厂商自报）[T02-S017]。流程行业的排程约束（连续生产、序列相关换型、联产品/副产品、罐容约束）与离散制造非常不同，通用 APS 往往建模困难，这是 OMP 长期存在的原因。

**Siemens Opcenter APS（原 Preactor）**

Preactor 被西门子收购后改名 Opcenter Advanced Planning and Scheduling。支持有限产能与无限产能两种模式，计划周期可按天、周、月或混合；排程侧是交互式多约束排程，排序算法考虑资源可用性与订单附带的约束 [T02-S022][T02-S023]。产品仍在活跃迭代（Preactor APS 17.1 版本说明见西门子官方博客）[T02-S024]。

- **用在什么场景**：单厂或少数几个厂的**车间级有限产能排程**，特别是换型时间显著、需要人工干预甘特图的场景。价格与实施复杂度远低于 Kinaxis/o9 这一档。
- **什么时候不该用**：跨厂、跨国的网络级供应计划。Opcenter APS 是排程工具，不是供应链网络计划平台。**这是一个非常常见的误配**：企业想解决「网络层的物料与产能平衡」，却买了一个车间排程器。

**中国本土 APS / 排产**

- **黑湖智造（Blacklake）**：云端制造协同系统，SaaS 交付，功能覆盖计划排产、生产执行、质量、仓储、资源管理与数据分析 [T02-S030]。定位上更接近「MES + 轻排产」，不是重型 APS。
- **新核云**：融合 ERP 与 MES，在汽车零部件与装备制造垂直行业积累较深，强调打通设备层到企业层的数据 [T02-S034]。

  关于这两家的市场份额，公开可见的两组数字互相矛盾（一组称黑湖在「云化 MES」细分占 52.7% 居首，另一组称在「SaaS MES」子市场新核云 19.6%、黑湖 18.9% 分列前二）。这两组数字都来自厂商引用的付费报告，分母口径不同且无公开原始报告可核。**一律按厂商自报处理，不要写进选型报告当作事实。**

- **国产 APS 的真实定位**：多数国产排产产品的强项是「把车间的实际约束建准 + 快速上线 + 服务响应快」，弱项是多级供应网络的建模能力与场景模拟深度。对于单厂或几个厂的国内制造企业，国产方案的性价比通常明显更好；对于跨国多基地网络，目前仍缺乏能替代 Kinaxis/o9 的国产选项。

### 2.2 MES / 车间执行

MES 解决的是「计划下发之后，车间实际发生了什么」：工单派工、工序报工、设备数据采集、质量记录、批次追溯。

- **Siemens Opcenter Execution**：与西门子自动化设备生态深度整合，离散与流程都有版本。
- **Rockwell FactoryTalk ProductionCentre**：北美制造业与 Rockwell PLC（可编程逻辑控制器，产线上的控制主机）生态绑定紧，设备层数据采集是强项。厂商自述覆盖制药、汽车、快消、电子、电动车电池、时尚、轮胎、金属矿业，并提供单厂、多厂与行业套件三种交付形态 [T02-S046][T02-S047]。它同时把质量管理与业务分析整合进无纸化车间执行 [T02-S046]——**这是选型时要警觉的地方**：MES 厂商越来越倾向于把 QMS（质量管理系统）打包进来，如果你已经有独立 QMS，需要提前划清边界，否则会出现两套不合的质量记录。
- **AVEVA（原 Wonderware）**：流程工业、能源、公用事业侧渗透率高，强在实时数据与操作可视化。
- **黑湖智造**：中国中小制造企业的云 MES 常见选择，实施周期短是主要卖点 [T02-S030]。

**MES 选型的核心分岔不是功能表，是三个问题**：

1. 你的车间数据是**人工报工**还是**设备自动采集**？前者选型重点是易用性（工人愿不愿意用手机/平板报工），后者重点是设备协议兼容性（OPC UA、Modbus、各家 PLC 私有协议）。
2. 你需要**批次追溯**到什么粒度？医药、食品、汽车安全件需要单件或批次级全链追溯，这会大幅提高 MES 的数据模型复杂度。
3. MES 和 ERP 的**边界怎么划**？最常见的失败是两边都做工单管理，导致数据双写、口径打架。

### 2.3 WMS / TMS

- **WMS（仓储管理系统）**：管理上架、拣选、波次、库位。ERP 的库存模块与 WMS 的分界很清楚：ERP 记录「有多少」，WMS 记录「在哪个库位、由谁在什么时候动过、下一步该怎么走」。WMS 特有的能力包括库位级实时库存、按存储规则与周转率导向的上架与拣选、任务交织、波次与批量拣选优化、每笔交易的条码/RF/语音校验、货位优化与劳动力标准管理 [T02-S062]。当仓库 SKU 数上千、有批次/效期管理、或引入自动化设备（AGV、立体库）时，ERP 自带的库存模块就不够了。
- **TMS（运输管理系统）**：管理装车、路线、运费结算、承运商绩效。国内中小制造企业上 TMS 的比例远低于 WMS，因为运输多外包给货代。

**判断是否需要 WMS 的经验门槛（业内经验，非硬标准）**：日出库单量超过几百单、或库位数超过几千、或库存准确率长期低于 95% 且盘点找不出原因——三条中占两条就该认真评估 WMS。

**集成上的一条实务原则**：ERP 与 WMS 的接口应当是**单向权威**的——销售单与采购单从 ERP 流向 WMS，库存移动、收货与发货确认从 WMS 流回 ERP [T02-S062]。任何一方都不应该去改对方的主数据。这条原则听起来显然，但违反它是仓库对账工作量爆炸的头号原因。

### 2.4 需求预测

- **ForecastPro**：老牌统计预测软件，界面友好，适合计划团队没有编程能力但需要正经统计预测的场景。
- **SAP APO / IBP 统计引擎**：SAP 生态内的预测模块，好处是与后续供应计划同源。
- **开源栈**：
  - **Nixtla StatsForecast**：统计与计量预测模型库，速度是主要卖点，开源在 GitHub 上维护 [T02-S013]。对供应链最有价值的是它把断续需求（intermittent demand，大量为零、偶尔来一单的备件类需求）模型做全了：CrostonClassic、ADIDA、IMAPA、TSB [T02-S012][T02-S014]。文档明确提示这些断续需求模型目前只能给点预测，不给区间 [T02-S012]——**这一点在做安全库存时很关键**，因为安全库存的计算需要的是需求分布（尤其是分布的上尾），不是一个点估计。ASCM 对安全库存的定位也是「应对需求变异的应急计划」而不是「补预测误差的固定量」[T02-S029]。实务上的做法：断续需求用点预测定补货量，用历史需求的经验分布（而非正态假设）定安全库存。
  - **Prophet**：处理季节性与节假日效应方便，但在断续需求和短历史序列上表现通常不如专门的统计方法。
  - **statsmodels**：ETS、ARIMA 等经典方法的实现，适合做基线对照。

**关于「用深度学习做需求预测」的冷水**：StatsForecast 项目自己的对比文档就在做统计方法、机器学习方法与神经网络方法的横向比较 [T02-S058]。在供应链的典型数据条件下（每个 SKU 只有两三年月度或周度历史、序列数量多但每条都很短），统计方法通常是很难被超越的基线，而且训练成本低几个数量级。**先把统计基线跑出来，再决定要不要上更复杂的模型**——很多团队跳过这一步，结果是花了半年做的模型跑不赢一个季节性朴素预测（naive seasonal，直接拿去年同期当预测）。

**预测工具选型的真实分岔**：不是「哪个模型准」，是「你的需求是什么形态」。
- 连续、有季节性、历史长 → 统计方法（ETS/ARIMA）+ 促销/事件调整。
- 断续、稀疏（备件、长尾 SKU）→ Croston 系方法，或者干脆放弃预测改用缓冲（见 DDMRP）。
- 新品、无历史 → 预测在数学上无解，只能靠类比法 + 快速反应机制。**给新品做统计预测是这行最普遍的自欺行为之一。**

### 2.5 运筹优化与仿真

**优化求解器**

- **Gurobi**：商业求解器，混合整数规划（MIP，一部分决策变量必须取整数、另一部分可取任意实数的优化问题）性能领先。Gurobi 自己的技术资料把 MIP 的求解路径讲得很清楚：基于线性规划的分支定界，性能提升主要来自预处理（presolve）、割平面、启发式与并行 [T02-S052]。第三方采购平台的估算是每年 1 万美元起，企业级部署常在 2 万–10 万美元以上（第三方估算，非厂商报价，实际价格按用途与规模谈判）[T02-S033]。学术免费。
- **IBM CPLEX**：另一家老牌商业求解器，能力接近 Gurobi。
- **Google OR-Tools（含 CP-SAT）**：开源免费。CP-SAT 是约束规划求解器（把问题描述成变量 + 约束，让求解器自己找可行解），在**排程类问题**（车间排程、人员排班）上表现优异。官方文档直接提供 job shop（车间作业排程，目标是最小化 makespan 即从最早开工到最晚完工的总跨度）与 flexible job shop（同一道工序可在多台机器上做）的完整实现，代码覆盖 Python、C++、Java、C#、Go [T02-S010][T02-S011][T02-S060]。排程建模的基本积木（可变工期、可选任务、互斥资源、时序关系）在官方 scheduling 文档里有系统说明 [T02-S011]。局限是 CP-SAT 原生不支持连续变量（除非能推导为整数），涉及连续量的问题（如混合配料、连续产能分配）要用 MIP 求解器 [T02-S033]。
- **PyJobShop**：在 CP-SAT 之上封装的开源排程建模库，把 job shop / flow shop / flexible job shop 这些标准问题类型做成现成 API [T02-S059]。**如果你的问题就是标准车间排程，从这里起步比自己从 CP-SAT 裸写快一个数量级。**
- **Pyomo / PuLP**：Python 建模层，不是求解器。写模型用它们，底下换求解器（CBC、HiGHS、Gurobi、CPLEX）只改一行。这个分层的实务价值是：**先用免费求解器把模型写对，规模撑不住了再花钱换商业求解器**，而不是一开始就买。

**什么时候该用优化，什么时候不该**：

优化的前提是你能把目标和约束写成数学式子，并且数据准确。现实中失败的优化项目里，绝大多数不是模型不对，是**约束没写全**——排程模型没建模的那个「李师傅只会开三号机」的隐性约束，会让优化结果在车间被直接否决。**先用 Excel 或手工排一版，把所有被忽略的约束逼出来，再上优化。**

**仿真软件**

- **AnyLogic**：同时支持离散事件、系统动力学、多智能体三种建模范式，且可以在一个模型里混用 [T02-S050]。这是它在供应链网络仿真上的核心优势——网络层用多智能体（每个工厂、DC、港口是一个有自己行为的个体），产线层用离散事件，需求与政策层用系统动力学。有配套的供应链仿真教材可下载（作者 Dmitry Ivanov，书由厂商网站托管）[T02-S051]。
- **FlexSim**：3D 离散事件仿真，覆盖制造、物料搬运、医疗、仓储与供应链 [T02-S063]。产线与仓储布局仿真直观，**做给管理层看时说服力强**——这不是玩笑，产能投资决策常常卡在「决策者想象不出来」，3D 动画在这个环节真的有用。
- **Simul8**：轻量离散事件仿真，学习门槛低。
- **SimPy**：基于标准 Python 的**过程式**离散事件仿真框架，开源免费。进程用 Python 生成器函数定义，可以建模顾客、车辆、代理这类主动实体；同时提供多种共享资源类型来建模有限产能的拥堵点（服务台、收银台、通道）[T02-S037]。仿真可以「尽可能快」地跑、按实际时钟跑、或手工逐事件推进 [T02-S037]。
  - **什么时候用 SimPy 而不是商业仿真软件**：模型要嵌进已有的 Python 数据流水线、要跑几万次参数扫描、或者要进版本控制被同事 review。
  - **什么时候不该用**：需要 3D 可视化说服管理层、或者建模的人不写代码。

**仿真 vs 优化的分工**：优化回答「最好的方案是什么」，仿真回答「这个方案在随机波动下会怎样」。产能投资决策、缓冲区大小、AGV 数量这类问题，仿真比优化更合适，因为关键变量是波动而不是均值。

**两者结合的一个真实用法**：约束理论的 DBR（鼓-缓冲-绳）需要给瓶颈前的缓冲定一个大小，这个参数没有解析解，通常靠仿真扫描。已有学术工作专门研究如何在 DBR 参数化中管理仿真预算、减少计算量 [T02-S049]——这类问题在教科书里被一句「设定合适的缓冲」带过，在现实里是要跑几千次仿真的。

### 2.6 多级供应链风险可视

2020 年之后这个品类才真正被采购。核心能力是把你的一级供应商往上追到二级、三级乃至更深，再叠加地理、天气、地缘、财务风险事件。

- **Resilinc**：主打多级映射（multi-tier mapping），厂商称可追溯到 sub-tier 10 层，并做成供应网络的数字孪生 [T02-S025]。
- **Everstream Analytics**：Discover / Explore / Reveal 三个产品，覆盖供应商风险评估到实时监控与全球事件告警 [T02-S064][T02-S065]。
- **Interos**：AI 驱动的关系映射，覆盖实体与数字供应链风险，强调对风险的发现与排序 [T02-S066]。

**诚实的判断**：这类平台的深层数据（三级以上）主要靠三个来源——供应商自主填报、公开贸易与工商数据推断、以及厂商自建数据库。**填报覆盖率决定一切**。如果你没有商务筹码逼供应商填问卷，买回来的多级地图会有大量空白，而空白处恰恰是风险所在。

- **什么时候不该买**：供应商数量少于几十家、且你对每一家都很熟的企业。这时候一张 Excel 表加一次季度电话比平台有用。
- **什么时候值得买**：受法规驱动的场景（欧盟供应链尽职调查、冲突矿产、强迫劳动合规），因为这时候你需要的是可审计的证据链而不是洞察。

### 2.7 PLM / BOM 管理

- **Siemens Teamcenter**：大型制造业 PLM 的主流，与 NX/CAD 生态紧密。
- **PTC Windchill**：另一大主流，在配置管理与变更管理上历史深。
- **Arena PLM**（现属 PTC）：云原生，中小型电子与医疗器械企业常用，上手快。

**为什么 PLM 在供应链工具地图里**：BOM 是 MRP 的输入。工程 BOM（EBOM）与制造 BOM（MBOM）不一致，是计划系统出错的头号根因之一。西门子官方文档对两者的区分说得最简洁：**EBOM 强调物料和零件如何服务于产品的功能设计，MBOM 反映这些物料和零件如何被装配成一个完整产品，MBOM 是从 EBOM 派生出来的** [T02-S044]。差异来自哪里很具体——包装材料、辅料、工装、装配顺序、外购件与自制件的划分，这些在设计视角里不存在，在生产视角里必须有。

PLM 的价值在于管住这层派生关系与工程变更（ECO/ECN）的发布节奏，让计划知道「哪个版本从哪张工单开始生效」。Teamcenter 提供 EBOM 到 MBOM 的可视化实时比对（reconciliation），以及基于可配置规则框架的双向更新 [T02-S044][T02-S045]。

**给计划岗的实用提醒**：当你发现「系统说料齐了但车间开不了工」反复出现，先查的不是 MRP 参数，是 EBOM/MBOM 是否同步。这条经验能省掉很多无效的参数调整。

- **什么时候不该单独上 PLM**：产品结构简单、变更频率低的企业，ERP 自带的 BOM 版本管理够用。
- **什么时候必须上**：一年工程变更几百次以上、或者有客户强制的配置管理要求（航空、医疗器械、汽车）。

---

## 3. 新兴 / 实验层（2025–2026）

**这一节的写法：厂商说了什么、有没有可验证的客户案例、我的判断分开写。**

### 3.1 计划系统里的 AI 代理（agentic AI）

**厂商侧发生了什么**：2025 年 10 月 Kinaxis 发布 Maestro Agents，定位是嵌在计划环境里的「有上下文的数字同事」，帮计划员从发现问题更快走到行动 [T02-S020][T02-S019]。2026 年进一步发布 Maestro Agent Studio，提供无代码方式让供应链团队用自己的数据、流程和工具组合 AI 代理 [T02-S021]。o9 的做法是在企业知识图谱上跑跨职能的组合式代理（composite agents），厂商描述的循环是「感知—建模—决策—执行—学习」[T02-S054]。

两家的共同叙事是同一句话：**代理是在真实的计划模型内推理，而不是外挂一个聊天框。** 这个区分本身是对的、也是重要的——外挂式的助手拿不到约束和权衡，只能复述数据。

**有没有可验证案例**：目前公开可查的具名客户表述很少。Kinaxis 的发布稿里引用了 Jabil（大型电子合约制造商）高级总监的说法，称 Kinaxis 代理已经在帮他们的计划团队与客户和代工厂协作 [T02-S020]。这是**厂商发布稿里的客户引言**，属于厂商自报口径，不是独立验证的效果数据——没有给出量化的效率或准确率提升。

**我的判断**：

- 真实且有价值的部分：把「查询 + 汇总 + 生成解释」这类计划员每天占大量时间的重复劳动自动化。计划员一天里有相当比例的时间在回答「这个订单为什么会晚」，而这个问题的答案本来就藏在系统数据里。
- 目前站不住的部分：「AI 自主决策并执行」。这两家的代理都强调在计划模型内推理，而跨系统的行动能力仍在建设中。也就是说，宣传里的「控制塔自动处理异常」目前主要是在自家计划平台的边界内成立。
- **给采购方的建议**：把 AI 代理当作**已购平台的增值功能**评估，不要当作换平台的理由。要求厂商演示的不是 demo 数据，是拿你自己的一个月真实数据跑一遍。

### 3.2 需求感知（demand sensing）

用短周期的下游信号（POS 销量、经销商出货、在途库存、天气、搜索热度）修正短期预测。厂商普遍宣称短期（1–4 周）预测误差可降低两位数百分比。

**诚实的说法**：这类改善在**下游数据可得且颗粒度足够**的消费品与零售场景是可信的；在数据只能到经销商一级、且经销商压货行为主导出货节奏的场景，需求感知修正的往往是渠道行为噪声而不是真实需求。**先问自己能不能拿到 POS 数据，再评估工具。**

### 3.3 数字孪生与网络设计自动化

供应链数字孪生的含义在不同厂商嘴里差异极大，从「一张动态的网络图」到「一个可以跑仿真的完整模型」都有人叫这个名字。可验证的部分是：AnyLogic 这类仿真工具做的网络仿真是实打实的模型；供应链风险平台做的「数字孪生」通常指的是供应网络的关系图谱，不含动态仿真能力 [T02-S025]。**买之前问清楚：能不能跑蒙特卡洛？能不能给出分布而不只是一个数？**

### 3.4 GPU 加速的优化求解

NVIDIA cuOpt 等把线性规划与混合整数规划的部分算法搬到 GPU 上。对于超大规模的路径规划与网络流问题，加速效果有公开的技术说明。对典型的工厂排程问题（规模中等、约束结构复杂），CP-SAT 这类 CPU 求解器仍然更实用。**这是 2026 年值得观察但不值得赌的方向。**

---

## 4. 选型决策树

**关键分岔不是厂商功能清单。** 功能表上每家都打勾。真正决定成败的是下面五个问题，按顺序回答。

### 第一步：定履行模式（这一步没定，后面全白做）

```
你的产品在收到客户订单之前，做到哪一步？
│
├─ 已经做成成品放在仓库里 → MTS 备货生产
│   需要：需求预测 + 主生产计划 MPS + MRP + 安全库存策略
│   计划的主战场在「预测准不准」和「库存放在哪一级」
│   工具重点：预测工具 + 库存优化 + 补货规则
│
├─ 通用件做成半成品，收到订单后组装 → ATO 订单装配
│   需要：两级计划——半成品按预测做，成品按订单组装
│   核心是「解耦点」放在哪一层 BOM
│   工具重点：可承诺量 ATP/CTP 计算 + 通用件预测 + 组装排程
│   这是 APS 价值最大的场景之一
│
├─ 收到订单才开始做，但设计是现成的 → MTO 订单生产
│   需要：有限产能排程 + 可靠的交期承诺
│   计划的主战场是「排程」和「报交期」，不是预测
│   工具重点：APS 排程器（Opcenter APS 这一档就够）+ 长周期料的预投策略
│
└─ 收到订单才开始设计 → ETO 订单设计
    需要：项目式排程（不是 MPS+MRP）
    BOM 在项目进行中才逐步成型，MRP 的前提「BOM 已知」不成立
    工具重点：项目管理 + 工程进度与采购进度联动 + PLM
    强行套 MPS/MRP 是 ETO 企业上 ERP 失败的最常见原因
```

ASCM（原 APICS，供应链管理领域的主要行业协会与认证机构）的 CPIM 体系把履行策略正式列为：MTS、ATO、CTO（配置生产）、MTO、ETO、延迟制造、再制造 [T02-S028]。多数真实企业是混合的——**这时候正确做法是按产品族分开定，而不是找一个「兼顾所有模式」的系统。**

### 第二步：看需求变异度与产品生命周期

```
需求可预测吗？产品活多久？
│
├─ 需求平稳 + 生命周期长（工业标准件、基础耗材）
│   → 统计预测有效。ETS/ARIMA + 安全库存公式够用
│
├─ 需求波动大 + 生命周期长（工业设备备件、长尾 SKU）
│   → 预测准确率天花板很低，别在预测上砸钱
│   → 走缓冲逻辑：DDMRP（需求驱动的物料需求计划）
│      在关键节点设「解耦点」放缓冲库存，用实际消耗触发补货
│      DDI（提出这套方法的机构）的适用条件说得很清楚：
│      当「客户能接受的等待时间远短于累计生产提前期」时最有价值 [T02-S004]
│      配套的运营模型除了库存缓冲，还包含时间缓冲与产能缓冲 [T02-S005]
│      —— 只做库存缓冲不做另外两种，是 DDMRP 落地失败的常见形态
│
├─ 需求波动大 + 生命周期短（时尚、消费电子、促销品）
│   → 预测在数学上不可能准。核心能力是「快速反应」
│   → 工具重点：短周期补货 + 需求感知 + 产能弹性
│   → 不要买重型 APS 去优化一个本来就不确定的输入
│
└─ 全新产品无历史
    → 统计预测无意义。类比法 + 小批量试产 + 快速迭代
```

DDMRP 的六个组成部分是：战略解耦、缓冲档案与水位、动态缓冲调整、需求驱动的计划、可视化协同执行、战术适应 [T02-S004]。它明确定位为「结合 MRP/DRP 中仍然有效的部分 + 精益与约束理论的拉动与可视 + 六西格玛的变异削减」[T02-S004]。DDI 网站上列了 A2A（意大利公用事业）与 JELD-WEN（建材制造）等案例，但主页面上没有给出量化指标 [T02-S004][T02-S006]——**引用 DDMRP 效果时要注意这一点，公开的量化证据比方法的流行度弱。**

### 第三步：看产品结构复杂度

```
多级 BOM 有几层？共用件比例多高？
│
├─ 1–3 层，共用件少 → ERP 原生 MRP 够用，不需要 APS
│
├─ 4–8 层，共用件多 → MRP 展开的连锁效应显著
│   一个顶层需求变动会在下面几层引发大量调整
│   → 这是 APS 的场景模拟能力真正值钱的地方
│   → 也是 PLM 管住 BOM 版本变得必要的地方
│
└─ 8 层以上或大量替代料/工程变更 → PLM 必需
    先解决 EBOM/MBOM 一致性，再谈计划系统
```

### 第四步：看工厂约束类型

```
瓶颈在哪里？稳不稳？
│
├─ 瓶颈固定且明确（一台关键设备、一道关键工序）
│   → 约束理论 TOC 的 DBR 逻辑比全局优化更实用
│   → DBR 三个词的意思：「鼓」是当前约束，它的节奏就是全线节奏；
│      「缓冲」是喂给约束的物料存量，作用是不让约束停机待料；
│      「绳」是把投料速度和缓冲水位绑起来的信号链 [T02-S048]
│   → 把排程精力全部集中在瓶颈，其余工序跟着瓶颈走
│   → 一个 Excel + 一个瓶颈甘特图往往就够，别急着买 APS
│   → 缓冲要设多大没有解析解，靠仿真扫参数 [T02-S049]
│
├─ 瓶颈随产品组合漂移
│   → 这是 APS 有限产能排程的核心价值场景
│   → 因为瓶颈位置本身是排程结果的函数，人算不出来
│
├─ 换型时间长且与顺序相关（换 A→B 和换 B→A 时间不同）
│   → 需要支持序列相关换型（sequence-dependent setup）的排程器
│   → 这是选型时必须实测的功能点，不能只看功能表打勾
│   → 同时：先做 SMED 把换型时间压下来，收益通常大于上系统
│
└─ 约束不在产能在物料（长周期进口件）
    → 问题在采购与供应商管理，不在排程
    → 上 APS 解决不了物料到不了的问题
```

### 第五步：看公司规模与 IT 承载力（上 APS 前的数据体检）

**这是最容易被跳过、也最致命的一步。** APS 的输入全部来自 ERP：订单、库存、BOM、工艺路线。输入错了，输出必然错，而且错得更快更自信。

上 APS 前必须先测的三个准确率（下列门槛为业内常用经验值，非任何标准机构的强制规定）：

| 数据项 | 常用经验门槛 | 怎么测 | 不达标的后果 |
|---|---|---|---|
| 库存准确率 | ≥ 95%（关键料 ≥ 98%） | 循环盘点，按库位+批次比对 | 排程基于不存在的库存，齐套判断全错 |
| BOM 准确率 | ≥ 98% | 抽样拆解实物比对 BOM | 缺料在开工时才发现 |
| 工艺路线与工时准确率 | ≥ 95% | 实测工时 vs 系统标准工时 | 排程算出的产能是假的，交期承诺不可信 |

行业侧的经验说法之一是「相当比例的生产延误可追溯到 BOM 数据不准而非真实缺料」（第三方厂商内容口径，非同行评议研究，仅作方向参考）[T02-S036]。

```
数据体检结果
│
├─ 三项都达标 + IT 有专职团队 + 多厂
│   → 可以上重型 APS（Kinaxis / o9 / SAP IBP / OMP）
│
├─ 三项都达标 + IT 只有 1–3 人 + 单厂或少数厂
│   → 上轻量排程器（Opcenter APS 这一档）或国产 APS
│   → 或者先用 Python + OR-Tools 做一个针对性排程模型
│
├─ 有一项不达标
│   → 先做数据治理，6–12 个月，别买 APS
│   → 这期间用 Excel + 方法工具（VSM/瓶颈分析）挖收益
│
└─ 三项都不达标
    → 问题不在计划，在现场管理
    → 先做 5S、循环盘点、BOM 清理，别谈系统
```

---

## 5. 避坑清单

新任计划经理或跨行进来的人最容易踩的坑，按踩中频率排序。

**坑 1：数据没治理就上 APS。**
最贵的错误。APS 把错误数据变成看起来很专业的错误计划，而且因为界面漂亮，比 Excel 的错误更难被质疑。正确顺序：库存准确率 → BOM 准确率 → 工艺路线 → 再谈 APS。见第 4 节第五步。

**坑 2：把 Excel 计划直接搬进 ERP。**
Excel 里的计划逻辑通常包含大量隐性判断（「这个客户的单要优先」「这台机器周三下午保养」），这些判断在 Excel 里由人每次现场决定。搬进 ERP 后，隐性判断要么丢失（计划变差），要么被硬编码成规则（失去灵活性）。**正确做法是先把隐性判断显性化写下来，判断哪些该固化成规则、哪些必须保留人工干预，再决定系统边界。**

**坑 3：买控制塔当仪表盘用。**
控制塔（control tower）的价值在于「发现异常 → 评估影响 → 给出方案 → 执行并回写」这个闭环。如果买回来只用了第一步的可视化，那你买的是一个非常昂贵的 BI。判断标准很简单：**上线半年后，有没有任何一个决策是因为控制塔而改变的？** 如果没有，它就是仪表盘。

**坑 4：用 MRP 解决瓶颈问题。**
MRP 假设产能无限。当交期问题的根因是某道工序排不过来时，无论 MRP 参数怎么调（改提前期、加安全库存、改批量），都只是把问题挪到别处。瓶颈问题的解法是：识别瓶颈 → 保护瓶颈（在其前面放缓冲）→ 让其他工序服从瓶颈节奏 → 提升瓶颈产能。这是约束理论 TOC 的基本逻辑，与买什么系统无关。

**坑 5：上系统前不定履行模式。**
ETO 企业买了 MTS 逻辑的 ERP，或者 MTS 企业上了项目式管理，是最难挽回的错配，因为它错在数据模型层面而不是配置层面。**先定履行模式，再选系统。** 见第 4 节第一步。

**坑 6：把预测准确率当作 KPI 去优化。**
预测准确率有天花板，由需求本身的变异度决定。在一个本质上不可预测的品类上死磕预测准确率，投入产出比极差。正确的问题是「在这个准确率水平下，我需要多少缓冲/多快的反应速度才能达成服务水平」。

**坑 7：先买 APS 再做 SMED。**
换型时间是排程的关键输入。换型时间没压下来，APS 只能通过放大批量来规避换型，结果是库存上升、柔性下降，然后大家怪系统。SMED 的投入通常是几周的人力，收益是长期的。**顺序反了，钱就白花了。**

**坑 8：多级供应链风险平台买了但不逼供应商填报。**
平台的深层数据依赖供应商自主填报。没有商务压力配合，覆盖率会低到没有决策价值。买之前先确认：谁负责催填、催不动怎么办。

**坑 9：MES 和 ERP 都做工单管理。**
边界不清导致数据双写、口径打架、对账变成日常工作。常见的清晰划法：ERP 管工单的创建、成本、结算；MES 管工单在车间的执行、报工、质量记录；两边的接口只传状态和数量，不双向改主数据。

**坑 10：给新品做统计预测然后相信它。**
无历史数据时统计预测在数学上无意义。这时候该做的是类比法定一个粗略量级、小批量投放、然后把资源投在「发现卖爆了或卖不动之后能多快调整」上。

**坑 11：以为国际大厂方案在中国工厂能原样落地。**
差异不在软件功能，在配套条件：主数据维护的人力配置、车间工人的系统使用习惯、供应商的信息化水平、以及本地实施顾问的可得性。一个在欧洲总部跑得很好的 APS 模板，搬到国内工厂常常因为「没人维护工艺路线主数据」而失效。

**坑 12：把 Gartner 魔力象限当选型结论。**
魔力象限评的是厂商综合能力，不是「适合你」。象限里的 Leader 可能因为规模不匹配、行业不对口、或本地服务能力不足而完全不适合你。**本文引用的所有魔力象限位置都来自厂商自己的新闻稿或落地页 [T02-S015][T02-S016][T02-S017][T02-S018][T02-S067]，原报告需付费获取，且各家只会公布对自己有利的那一张图。** 注意到 2026 年 Gartner 把这个品类拆成了「离散与流程行业」与「流程行业」不同的象限，这本身说明一件事：**不存在一个通吃的最优 APS，品类分岔就是承认场景分岔。**

**坑 13：把 MES 厂商附带的质量模块当成 QMS 用，或反过来。**
MES 厂商越来越倾向于把质量管理打包进产品 [T02-S046]。如果企业已有独立 QMS（尤其是受法规约束的医药、医疗器械），两套系统都存质量记录会导致审计时说不清哪份是权威版本。**边界必须在合同签之前划清。**

---

## 6. 一页速查

| 你的问题 | 该拿起的工具 | 不该拿起的工具 |
|---|---|---|
| 交期长但说不清时间花在哪 | 价值流图 VSM | APS |
| 某道工序永远排不过来 | TOC 瓶颈分析 + DBR | 调 MRP 参数 |
| 换型太久导致批量做不小 | SMED 换模记录表 | APS |
| 库存高但还缺货 | ABC/XYZ 分类 + 解耦点重设（DDMRP 思路） | 加安全库存 |
| 备件类需求断断续续 | Croston/ADIDA/TSB（StatsForecast） | Prophet、ARIMA |
| 瓶颈随产品组合漂移 | APS 有限产能排程 | 人工甘特图 |
| 客户天天改单，要快速重排 | Kinaxis 这类并发场景引擎 | Excel |
| 要判断加一条产线能提多少产出 | 仿真（AnyLogic/FlexSim/SimPy） | 优化求解器 |
| 排程要考虑序列相关换型 | CP-SAT 或支持该约束的 APS | 通用 MIP 模型 |
| 工程变更多导致计划频繁出错 | PLM（Teamcenter/Windchill/Arena） | 加强人工核对 |
| 要向监管证明供应链尽调 | 多级风险平台（Resilinc 等） | 内部 Excel 表 |

---

## Source Manifest

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T02-S001 | https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/f899ce30af9044299d573ea30b533f1c/86e15c58eb021f60e10000000a44147b.html | surrogate_primary | 2026-09-02 | SAP | vendor docs, first-hand product doc on Working with MRP Live |
| T02-S002 | https://learning.sap.com/courses/exploring-business-processes-in-sap-s-4hana-production-planning/outlining-material-requirements-planning-with-mrp-live | surrogate_primary | 2026-09-02 | SAP | vendor docs, official training material on MRP Live and PP/DS |
| T02-S003 | https://community.sap.com/t5/enterprise-resource-planning-blog-posts-by-sap/what-s-new-for-production-planning-in-sap-s-4hana-private-cloud-2025/ba-p/14267254 | secondary | 2026-09-02 | SAP Community | vendor-hosted community blog, author-written, not official documentation |
| T02-S004 | https://www.demanddriveninstitute.com/ddmrp | verified_primary | 2026-09-02 | Demand Driven Institute | originator of the DDMRP method, six components and applicability conditions |
| T02-S005 | https://www.demanddriveninstitute.com/demand-driven-operating-model | verified_primary | 2026-09-02 | Demand Driven Institute | originator, decoupling and control point buffer model |
| T02-S006 | https://www.demanddriveninstitute.com/case-studies | verified_primary | 2026-09-02 | Demand Driven Institute | originator, self-reported case list (A2A, JELD-WEN), no quantified metrics on page |
| T02-S007 | https://www.lean.org/lexicon-terms/value-stream-mapping/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | association, lexicon definition of value stream mapping |
| T02-S008 | https://www.lean.org/lexicon-terms/a3-report/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | association, lexicon definition of the A3 report and A3 management process |
| T02-S009 | https://www.lean.org/events-training/forms-templates/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | association, downloadable A3 / standard work / VSM templates |
| T02-S010 | https://developers.google.com/optimization/scheduling/job_shop | verified_primary | 2026-09-02 | Google OR-Tools | project own documentation, job shop scheduling with CP-SAT |
| T02-S011 | https://github.com/google/or-tools/blob/stable/ortools/sat/docs/scheduling.md | verified_primary | 2026-09-02 | Google OR-Tools | project own documentation, CP-SAT scheduling primitives |
| T02-S012 | https://nixtlaverse.nixtla.io/statsforecast/docs/tutorials/intermittentdata.html | verified_primary | 2026-09-02 | Nixtla | project own documentation, intermittent demand models and point-forecast-only limitation |
| T02-S013 | https://github.com/Nixtla/statsforecast | verified_primary | 2026-09-02 | Nixtla | project own documentation, StatsForecast repository |
| T02-S014 | https://nixtlaverse.nixtla.io/statsforecast/docs/models/adida.html | verified_primary | 2026-09-02 | Nixtla | project own documentation, ADIDA model reference |
| T02-S015 | https://www.kinaxis.com/en/blog/kinaxis-named-leader-2025-gartner-magic-quadrant-supply-chain-planning-solutions | secondary | 2026-09-02 | Kinaxis | vendor press post citing a paywalled Gartner analyst report; vendor-selected framing |
| T02-S016 | https://o9solutions.com/news/o9-named-a-leader-in-the-2025-gartner-magic-quadrant-for-supply-chain-planning-solutions | secondary | 2026-09-02 | o9 Solutions | vendor press post citing a paywalled Gartner analyst report |
| T02-S017 | https://omp.com/news-events/news/2026/omp-positioned-highest-in-2026-gartner-magic-quadrant-for-supply-chain-planning-solutions | secondary | 2026-09-02 | OMP | vendor press post citing a paywalled Gartner analyst report, process industries quadrant |
| T02-S018 | https://www.oracle.com/news/announcement/oracle-once-again-named-a-leader-in-2025-gartner-magic-quadrant-for-supply-chain-planning-solutions-2025-05-16/ | secondary | 2026-09-02 | Oracle | vendor press release citing a paywalled Gartner analyst report |
| T02-S019 | https://www.kinaxis.com/en/solutions/ai-agents | surrogate_primary | 2026-09-02 | Kinaxis | vendor docs, Maestro Agents product page |
| T02-S020 | https://www.kinaxis.com/en/news/press-releases/2025/kinaxis-accelerates-agentic-era-supply-chain-orchestration-launch-maestro | surrogate_primary | 2026-09-02 | Kinaxis | vendor docs, launch announcement containing the Jabil customer quote |
| T02-S021 | https://www.kinaxis.com/en/news/press-releases/2026/kinaxis-introduces-maestro-agent-studio-unlocking-next-level-decision | surrogate_primary | 2026-09-02 | Kinaxis | vendor docs, Maestro Agent Studio announcement |
| T02-S022 | https://www.siemens.com/en-us/products/opcenter/advanced-planning-scheduling-aps/advanced-planning-software/ | surrogate_primary | 2026-09-02 | Siemens | vendor docs, Opcenter APS finite/infinite capacity planning description |
| T02-S023 | https://www.plm.automation.siemens.com/global/en/products/manufacturing-operations-center/preactor-aps.html | surrogate_primary | 2026-09-02 | Siemens | vendor docs, Preactor to Opcenter APS product page |
| T02-S024 | https://blogs.sw.siemens.com/opcenter/Preactor-APS-version-17-1/ | surrogate_primary | 2026-09-02 | Siemens | vendor docs, Preactor APS 17.1 release notes on the official Opcenter blog |
| T02-S025 | https://resilinc.ai/products/multi-tier-mapping/ | surrogate_primary | 2026-09-02 | Resilinc | vendor docs, multi-tier mapping and sub-tier depth claims |
| T02-S026 | https://www.ascm.org/corporate-solutions/standards-tools/scor-ds/ | verified_primary | 2026-09-02 | ASCM | association, SCOR Digital Standard overview |
| T02-S027 | https://www.ascm.org/globalassets/ascm_website_assets/docs/scor/intro-and-front-matter-scor-digital-standard-2025.pdf | verified_primary | 2026-09-02 | ASCM | association, SCOR DS 2025 front matter, Plan/Order/Source/Transform/Fulfill/Return processes |
| T02-S028 | https://www.ascm.org/globalassets/ascm_website_assets/docs/ecm/ecm-CPIM9.pdf | verified_primary | 2026-09-02 | ASCM | association, CPIM 9.0 exam content manual listing fulfillment strategies MTS/ATO/CTO/MTO/ETO |
| T02-S029 | https://www.ascm.org/ascm-insights/safety-stock-a-contingency-plan-to-keep-supply-chains-flying-high/ | verified_primary | 2026-09-02 | ASCM | association, safety stock under demand variability |
| T02-S030 | https://www.blacklake.cn/ | surrogate_primary | 2026-09-02 | 黑湖智造 Blacklake | vendor docs, cloud MES product scope (planning, execution, quality, warehouse) |
| T02-S031 | https://u9cloud.yonyou.com/ | surrogate_primary | 2026-09-02 | 用友 Yonyou | vendor docs, U9 cloud manufacturing ERP positioning and target industries |
| T02-S032 | https://scor.ascm.org/ | verified_primary | 2026-09-02 | ASCM | association, SCOR model reference site |
| T02-S033 | https://www.vendr.com/marketplace/gurobi | secondary | 2026-09-02 | Vendr | third-party procurement marketplace price estimate, not a vendor list price |
| T02-S034 | https://36kr.com/p/1724910436353 | secondary | 2026-09-02 | 36Kr | tech media profile of 新核云 cloud ERP + MES positioning |
| T02-S035 | https://www.omniful.ai/blog/top-blue-yonder-alternatives-2026 | secondary | 2026-09-02 | Omniful | vendor-adjacent comparison blog, used only for the widely-repeated "steep learning curve" observation |
| T02-S036 | https://www.agsdevices.com/bom-inventory-management/ | secondary | 2026-09-02 | AGS Devices | third-party vendor content claiming a share of production delays trace to BOM inaccuracy; directional only, not peer-reviewed |
| T02-S037 | https://simpy.readthedocs.io/en/latest/ | verified_primary | 2026-09-02 | SimPy | project own documentation, process-based discrete-event simulation framework overview |
| T02-S038 | https://blueyonder.com/solutions/supply-chain-planning | surrogate_primary | 2026-09-02 | Blue Yonder | vendor docs, supply chain planning solution page |
| T02-S039 | https://blueyonder.com/solutions/blue-yonder-platform | surrogate_primary | 2026-09-02 | Blue Yonder | vendor docs, platform architecture (microservices, Snowflake data foundation) |
| T02-S040 | https://help.sap.com/docs/SAP_INTEGRATED_BUSINESS_PLANNING/feae3cea3cc549aaa9d9de7d363a83e6/68be40553ebe8518e10000000a423f68.html | surrogate_primary | 2026-09-02 | SAP | vendor docs, IBP time-series-based supply planning heuristic |
| T02-S041 | https://help.sap.com/docs/SAP_INTEGRATED_BUSINESS_PLANNING/feae3cea3cc549aaa9d9de7d363a83e6/6ae8504591574271acb4fe7658e3e910.html | surrogate_primary | 2026-09-02 | SAP | vendor docs, IBP optimizer run details, objective function value and bound |
| T02-S042 | https://www.odoo.com/documentation/19.0/applications/inventory_and_mrp/manufacturing/workflows/use_mps.html | surrogate_primary | 2026-09-02 | Odoo | vendor docs, MPS is a manual tool and conflicts with reordering rules |
| T02-S043 | https://www.odoo.com/documentation/19.0/applications/inventory_and_mrp/inventory/warehouses_storage/replenishment/reordering_rules.html | surrogate_primary | 2026-09-02 | Odoo | vendor docs, reordering rules behaviour |
| T02-S044 | https://www.siemens.com/en-us/technology/manufacturing-bill-of-materials-mbom/ | surrogate_primary | 2026-09-02 | Siemens | vendor docs, EBOM vs MBOM definition and derivation |
| T02-S045 | https://www.siemens.com/en-us/solutions/bom-management/ | surrogate_primary | 2026-09-02 | Siemens | vendor docs, Teamcenter integrated BOM and change management |
| T02-S046 | https://www.rockwellautomation.com/en-us/products/software/factorytalk/operationsuite/mes/productioncentre.html | surrogate_primary | 2026-09-02 | Rockwell Automation | vendor docs, FactoryTalk ProductionCentre MES capabilities |
| T02-S047 | https://www.rockwellautomation.com/en-us/products/software/factorytalk/operationsuite/mes.html | surrogate_primary | 2026-09-02 | Rockwell Automation | vendor docs, MES portfolio and deployment shapes |
| T02-S048 | https://www.tocico.org/ | verified_primary | 2026-09-02 | TOCICO | association, Theory of Constraints body of knowledge and drum-buffer-rope definition |
| T02-S049 | https://arxiv.org/pdf/2402.14832 | verified_primary | 2026-09-02 | arXiv | academic preprint on simulation budget management in drum-buffer-rope parametrization |
| T02-S050 | https://www.anylogic.com/supply-chains/ | surrogate_primary | 2026-09-02 | AnyLogic | vendor docs, supply chain simulation and multi-paradigm modeling |
| T02-S051 | https://www.anylogic.com/upload/pdf/operations-and-supply-chain-simulation-with-anylogic72.pdf | secondary | 2026-09-02 | AnyLogic / D. Ivanov | academic textbook hosted on the vendor site, not independently published here |
| T02-S052 | https://www.gurobi.com/resources/faq/mixed-integer-programming-mip | surrogate_primary | 2026-09-02 | Gurobi | vendor docs, MIP definition and branch-and-bound solution path |
| T02-S053 | https://o9solutions.com/digital-brain | surrogate_primary | 2026-09-02 | o9 Solutions | vendor docs, Digital Brain platform and solver mix (heuristics, LP, MIP, third-party) |
| T02-S054 | https://o9solutions.com/news/o9-enhances-its-digital-brain-platform-with-generative-ai-powered-composite-agents-to-execute-complex-cross-functional-planning/ | surrogate_primary | 2026-09-02 | o9 Solutions | vendor docs, generative-AI composite agents announcement |
| T02-S055 | https://www.statista.com/statistics/526423/worldwide-erp-implementation-projects-cost-overrun/ | secondary | 2026-09-02 | Statista | aggregator statistic on worldwide ERP project cost overruns |
| T02-S056 | https://www.erpresearch.com/en-us/erp-implementation-cost-breakdown | secondary | 2026-09-02 | ERP Research | third-party consultancy content on ERP implementation duration and cost ranges |
| T02-S057 | https://www.netsuite.com/portal/resource/articles/erp/erp-statistics.shtml | secondary | 2026-09-02 | NetSuite (Oracle) | vendor marketing article aggregating third-party ERP statistics |
| T02-S058 | https://nixtlaverse.nixtla.io/statsforecast/docs/tutorials/statisticalneuralmethods.html | verified_primary | 2026-09-02 | Nixtla | project own documentation, statistical vs ML vs neural forecasting comparison |
| T02-S059 | https://github.com/PyJobShop/PyJobShop | verified_primary | 2026-09-02 | PyJobShop | project own documentation, constraint-programming scheduling library on top of CP-SAT |
| T02-S060 | https://developers.google.com/optimization/cp | verified_primary | 2026-09-02 | Google OR-Tools | project own documentation, constraint optimization overview |
| T02-S061 | https://blueyonder.com/solutions/supply-chain-planning/production-planning | surrogate_primary | 2026-09-02 | Blue Yonder | vendor docs, production planning module |
| T02-S062 | https://supplychainmath.com/en/supply-chain-software-guide.html | secondary | 2026-09-02 | SupplyChainMath | third-party guide distinguishing ERP vs APS vs WMS vs TMS scope and integration direction |
| T02-S063 | https://www.flexsim.com/ | surrogate_primary | 2026-09-02 | FlexSim | vendor docs, 3D discrete-event simulation scope across manufacturing and warehousing |
| T02-S064 | https://www.everstream.ai/ | surrogate_primary | 2026-09-02 | Everstream Analytics | vendor docs, supply chain risk intelligence platform |
| T02-S065 | https://www.everstream.ai/platform/global-monitoring/ | surrogate_primary | 2026-09-02 | Everstream Analytics | vendor docs, global monitoring and alerting module |
| T02-S066 | https://www.interos.ai/ | surrogate_primary | 2026-09-02 | Interos | vendor docs, multi-tier supply chain risk discovery and ranking |
| T02-S067 | https://www.kinaxis.com/en/about-us/gartner-magic-quadrant-supply-chain-planning-solutions | secondary | 2026-09-02 | Kinaxis | vendor landing page for the 2026 Gartner quadrant, paywalled original report |
| T02-S068 | https://www.lean.org/the-lean-post/articles/understanding-the-fundamentals-of-value-stream-mapping/ | verified_primary | 2026-09-02 | Lean Enterprise Institute | association, why VSM captures information flow and not just material flow |
