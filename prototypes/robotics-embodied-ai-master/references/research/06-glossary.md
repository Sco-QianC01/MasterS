# Track 06 — Glossary：术语 + 标准 + 法规 · 机器人与具身智能（locale=zh-CN）

> Phase 1 wave 1 · Track 06。供 Phase 2 整合进 skill 的 [Glossary — 术语 + 标准] 节，并支持「行业表达 DNA / 外行破绽」提取。
> 全文 `last_checked = 2026-09-02`。标准与法规一律标版本号、发布日、生效/适用日、法域、适用对象。
> **原话与转述分开标**：`【原文】` = 逐字引用；无标记 = 本文转述。**没有把握的条款号一律不写**，只写标准号 + 节名。

## Source Manifest

> 全部 `last_checked = 2026-09-02`。iso.org / webstore.iec.ch / automate.org(A3)/ UL 的标准页按规范记为 `surrogate_primary` + note `standards body`;政府与监管文件(MIIT / gov.cn / SAMR / EUR-Lex / OSHA / EU-OSHA)记为 `verified_primary` + note `regulator` 或 `监管`;厂商与项目自有文档记 `surrogate_primary` + note `vendor docs` / `own site`;arXiv / DOI 论文记 `verified_primary`。
> **与机械分类器的差异说明**：`source_verifier.py classify` 会把 iso.org / .edu / 部分 vendor 域名直接判为 `verified_primary`；本 track 按 Track 06 的标注约定，把「标准发布/售卖机构页」「厂商与项目自有文档」「协会」「课程/教材官网」一律降标为 `surrogate_primary` 并在 note 写明来源类型，只把政府/监管原文与论文原文留在 `verified_primary`。这是**有意的保守标注**，不是漏标；Phase 4 复核时以本说明为准。

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T06-S001 | https://www.iso.org/standard/75539.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 8373:2021 机器人词汇第 3 版 |
| T06-S002 | https://www.iso.org/standard/73933.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 10218-1:2025 机器人本体安全 |
| T06-S003 | https://www.iso.org/standard/73934.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 10218-2:2025 应用与机器人单元 |
| T06-S004 | https://www.iso.org/standard/62996.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO/TS 15066:2016 协作机器人 TS |
| T06-S005 | https://www.iso.org/standard/41571.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 10218-2:2011 旧版(已被取代) |
| T06-S006 | https://www.iso.org/standard/22244.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 9283:1998 性能规范与试验方法 |
| T06-S007 | https://www.iso.org/standard/51528.html | surrogate_primary | 2026-09-02 | ISO/TC 199 | standards body — ISO 12100:2010 风险评估 A 类标准 |
| T06-S008 | https://www.iso.org/standard/73481.html | surrogate_primary | 2026-09-02 | ISO/TC 199 | standards body — ISO 13849-1:2023 PL 第 4 版 |
| T06-S009 | https://www.iso.org/standard/69883.html | surrogate_primary | 2026-09-02 | ISO/TC 199 | standards body — ISO 13849-1:2015 上一版 |
| T06-S010 | https://www.iso.org/standard/83545.html | surrogate_primary | 2026-09-02 | ISO/TC 110 | standards body — ISO 3691-4:2023 无人驾驶工业车辆 |
| T06-S011 | https://www.iso.org/standard/70660.html | surrogate_primary | 2026-09-02 | ISO/TC 110 | standards body — ISO 3691-4:2020 上一版 |
| T06-S012 | https://www.iso.org/standard/83498.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO/DIS 13482 服务机器人安全修订中 |
| T06-S013 | https://www.iso.org/standard/63127.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 18646-1:2016 轮式服务机器人移动性能 |
| T06-S014 | https://www.iso.org/standard/82643.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO 18646-2:2024 导航性能测试 |
| T06-S015 | https://www.iso.org/standard/90680.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — ISO/CD TR 20218-3 10218-2 使用指南 |
| T06-S016 | https://www.iso.org/sectors/engineering/robotics | surrogate_primary | 2026-09-02 | ISO | standards body — ISO 机器人标准总入口 |
| T06-S017 | https://committee.iso.org/sites/tc299/home/projects/ongoing/iso-10218-2.html | surrogate_primary | 2026-09-02 | ISO/TC 299 | standards body — TC 299 在研项目页 |
| T06-S018 | https://webstore.iec.ch/en/publication/59927 | surrogate_primary | 2026-09-02 | IEC | standards body — IEC 62061:2021 机械 SCS 功能安全 ed.2 |
| T06-S019 | https://webstore.iec.ch/en/publication/112847 | surrogate_primary | 2026-09-02 | IEC | standards body — IEC 62061:2021+AMD1:2024+AMD2:2026 |
| T06-S020 | https://webstore.iec.ch/en/publication/26037 | surrogate_primary | 2026-09-02 | IEC | standards body — IEC 60204-1:2016 机械电气安全 |
| T06-S021 | https://webstore.iec.ch/en/publication/71256 | surrogate_primary | 2026-09-02 | IEC | standards body — IEC 60204-1:2016+AMD1:2021 CSV |
| T06-S022 | https://webstore.iec.ch/en/publication/5515 | surrogate_primary | 2026-09-02 | IEC | standards body — IEC 61508-1:2010 功能安全母标准 |
| T06-S023 | https://webstore.iec.ch/en/publication/22273 | surrogate_primary | 2026-09-02 | IEC | standards body — IEC 61508:2010 CMV 全套 1-7 部分 |
| T06-S024 | https://www.iec.ch/functional-safety | surrogate_primary | 2026-09-02 | IEC | standards body — SIL 体系官方科普页 |
| T06-S025 | https://www.automate.org/robotics/news/new-ansi-a3-r15-06-2025-american-national-standard-for-industrial-robot-safety-now-available-for-purchase | surrogate_primary | 2026-09-02 | A3 | 协会 — R15.06-2025 三部分发布公告与批准日期 |
| T06-S026 | https://www.automate.org/robotics/blogs/updated-iso-10218-faq | surrogate_primary | 2026-09-02 | A3 | 协会 — ISO 10218:2025 官方 FAQ(15066 归并说明) |
| T06-S027 | https://www.automate.org/robotics/news/new-r15-08-part-1-american-national-standard-for-industrial-mobile-robot-safety-requirements-published-by-robotic-industries-association | surrogate_primary | 2026-09-02 | A3/RIA | 协会 — R15.08-1 发布公告 |
| T06-S028 | https://webstore.ansi.org/standards/ria/ansia3r15082023 | surrogate_primary | 2026-09-02 | ANSI Webstore | standards body — R15.08-2-2023 目录页 |
| T06-S029 | https://webstore.ansi.org/standards/ria/ansiriar15082020 | surrogate_primary | 2026-09-02 | ANSI Webstore | standards body — R15.08-1-2020 目录页 |
| T06-S030 | https://webstore.ansi.org/standards/ul/ansiul33002024 | surrogate_primary | 2026-09-02 | ANSI Webstore | standards body — ANSI/CAN/UL 3300:2024 目录与日期 |
| T06-S031 | https://www.ul.com/services/consumer-and-commercial-robots | surrogate_primary | 2026-09-02 | UL Solutions | certification body / 认证机构 — 服务机器人认证范围 |
| T06-S032 | https://blog.ansi.org/ansi/iso-10218-1-2025-robots-and-robotic-devices-safety/ | secondary | 2026-09-02 | ANSI Blog | 10218-1:2025 变化点解读 |
| T06-S033 | https://blog.ansi.org/ansi/ansi-a3-r15-06-2025-robot-safety/ | secondary | 2026-09-02 | ANSI Blog | R15.06-2025 三部分结构解读 |
| T06-S034 | https://blog.ansi.org/ansi/iso-3691-4-2023-driverless-industrial-trucks/ | secondary | 2026-09-02 | ANSI Blog | ISO 3691-4:2023 适用对象解读 |
| T06-S035 | https://eur-lex.europa.eu/eli/reg/2023/1230/oj/eng | verified_primary | 2026-09-02 | EUR-Lex | regulator — 欧盟机械法规 2023/1230 官方文本 |
| T06-S036 | https://eur-lex.europa.eu/eli/reg/2026/1744/oj/eng | verified_primary | 2026-09-02 | EUR-Lex | regulator — Digital Omnibus on AI 官方文本 |
| T06-S037 | https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng | verified_primary | 2026-09-02 | EUR-Lex | regulator — EU AI Act 官方文本 |
| T06-S038 | https://osha.europa.eu/en/legislation/directive/regulation-20231230eu-machinery | verified_primary | 2026-09-02 | EU-OSHA | 监管 — 机械法规立法条目与适用日期 |
| T06-S039 | https://single-market-economy.ec.europa.eu/sectors/mechanical-engineering/machinery_da | verified_primary | 2026-09-02 | 欧盟委员会 | 监管 — 机械立法主页与过渡安排 |
| T06-S040 | https://www.osha.gov/otm/section-4-safety-hazards/chapter-4 | verified_primary | 2026-09-02 | OSHA | regulator — 工业机器人系统检查技术手册 |
| T06-S041 | https://www.osha.gov/enforcement/directives/ted-01-00-015-6 | verified_primary | 2026-09-02 | OSHA | regulator — OTM 该章更新指令记录 |
| T06-S042 | https://www.miit.gov.cn/jgsj/kjs/wjfb/art/2023/art_50316f76a9b1454b898c7bb2a5846b79.html | verified_primary | 2026-09-02 | 工业和信息化部 | 监管 — 人形机器人创新发展指导意见原文 |
| T06-S043 | https://www.gov.cn/zhengce/zhengceku/2023-01/19/content_5738112.htm | verified_primary | 2026-09-02 | 中国政府网 | 监管 — 「机器人+」应用行动实施方案原文 |
| T06-S044 | https://std.samr.gov.cn/search/orgDetailView?tcCode=TC591SC5 | verified_primary | 2026-09-02 | 国家标准委 | 监管 — TC591/SC5 人形机器人分标委职责与委员 |
| T06-S045 | https://std.samr.gov.cn/search/orgDetailView?data_id=CF251D8F517DD1C7E05397BE0A0AD46C | verified_primary | 2026-09-02 | 国家标准委 | 监管 — TC591 全国机器人标委会 |
| T06-S046 | https://std.samr.gov.cn/gb/search/gbDetailed?id=71F772D7DB68D3A7E05397BE0A0AB82A | verified_primary | 2026-09-02 | 国家标准委 | 监管 — GB 11291.1-2011 日期与强制属性 |
| T06-S047 | https://std.samr.gov.cn/gb/search/gbDetailed?id=71F772D7E933D3A7E05397BE0A0AB82A | verified_primary | 2026-09-02 | 国家标准委 | 监管 — GB 11291.2-2013 条目 |
| T06-S048 | https://std.samr.gov.cn/gb/search/gbDetailed?id=71F772D7EE9AD3A7E05397BE0A0AB82A | verified_primary | 2026-09-02 | 国家标准委 | 监管 — GB/T 12642-2013 条目 |
| T06-S049 | https://www.ncsti.gov.cn/kjdt/scyq/bjjjjskfq/jkdt/202504/t20250416_201754.html | verified_primary | 2026-09-02 | 北京市科委 | 监管 — 首批人形机器人系列国家标准立项 |
| T06-S050 | https://www.ncsti.gov.cn/kjdt/tzgg/202409/t20240930_180766.html | verified_primary | 2026-09-02 | 北京市科委 | 监管 — 人形机器人标委会筹建方案公示 |
| T06-S051 | https://open.beijing.gov.cn/html//yizhuang/gzdt/2025/4/1745221749437.html | verified_primary | 2026-09-02 | 北京市政务公开 | 监管 — 首批人形机器人国标立项名单 |
| T06-S052 | https://www.sist.org.cn/xwzx/yndt/202606/t20260609_2511164.html | surrogate_primary | 2026-09-02 | 深圳市标准技术研究院 | standards body — 首批人形机器人国标审定会记录 |
| T06-S053 | https://www.ndls.org.cn/standard/detail/825a275bf8dddc8ded0ffcf92884a705 | surrogate_primary | 2026-09-02 | 国家数字标准馆 | standards body — GB/T 12642-2013 采标关系与指标清单 |
| T06-S054 | https://www.ndls.org.cn/standard/detail/db52097af2f5816c8ead581bb9eb73d1 | surrogate_primary | 2026-09-02 | 国家数字标准馆 | standards body — GB/T 20868-2024 性能试验应用规范 |
| T06-S055 | https://arxiv.org/abs/2303.04137 | verified_primary | 2026-09-02 | Cheng Chi et al. | Diffusion Policy 原论文(2023-03-07) |
| T06-S056 | https://arxiv.org/abs/2304.13705 | verified_primary | 2026-09-02 | Tony Z. Zhao et al. | ACT / ALOHA 原论文(2023-04-23) |
| T06-S057 | https://arxiv.org/abs/2307.15818 | verified_primary | 2026-09-02 | Brohan et al. (Google DM) | RT-2:VLA 一词的出处(2023-07-28) |
| T06-S058 | https://arxiv.org/abs/2212.06817 | verified_primary | 2026-09-02 | Brohan et al. (Google) | RT-1(2022-12-13) |
| T06-S059 | https://arxiv.org/abs/2406.09246 | verified_primary | 2026-09-02 | Moo Jin Kim et al. | OpenVLA(2024-06-13) |
| T06-S060 | https://arxiv.org/abs/2310.08864 | verified_primary | 2026-09-02 | Open X-Embodiment Collab. | 跨本体数据集与 RT-X(2023-10-13) |
| T06-S061 | https://arxiv.org/abs/2410.24164 | verified_primary | 2026-09-02 | Kevin Black et al. (PI) | π0 flow-matching VLA(2024-10-31) |
| T06-S062 | https://arxiv.org/abs/1011.0686 | verified_primary | 2026-09-02 | Ross, Gordon, Bagnell | DAgger 与协变量偏移(2010-11-02) |
| T06-S063 | https://arxiv.org/abs/1703.06907 | verified_primary | 2026-09-02 | Josh Tobin et al. | 域随机化原论文(2017-03-20) |
| T06-S064 | https://arxiv.org/abs/1710.06537 | verified_primary | 2026-09-02 | Xue Bin Peng et al. | 动力学随机化 sim-to-real(2017-10-18) |
| T06-S065 | https://arxiv.org/abs/2010.11251 | verified_primary | 2026-09-02 | Joonho Lee et al. (RSL) | teacher-student 特权学习四足(2020-10-21) |
| T06-S066 | https://arxiv.org/abs/1806.10293 | verified_primary | 2026-09-02 | Kalashnikov et al. | QT-Opt 大规模真机 RL(2018-06-27) |
| T06-S067 | https://docs.ros.org/en/rolling/Concepts/Intermediate/About-Quality-of-Service-Settings.html | surrogate_primary | 2026-09-02 | Open Robotics | vendor docs — ROS 2 QoS 官方概念页 |
| T06-S068 | https://design.ros2.org/articles/ros_on_dds.html | surrogate_primary | 2026-09-02 | ROS 2 Design | originator — 为什么 ROS 2 选 DDS |
| T06-S069 | https://www.omg.org/spec/DDS/ | surrogate_primary | 2026-09-02 | OMG | standards body — DDS 规范主页 |
| T06-S070 | https://www.ethercat.org/en/technology.html | surrogate_primary | 2026-09-02 | EtherCAT Technology Group | association / 协会 — EtherCAT 技术与周期时间 |
| T06-S071 | https://www.can-cia.org/canopen | surrogate_primary | 2026-09-02 | CAN in Automation | association / 协会 — CANopen 与 CiA 402 驱动规范 |
| T06-S072 | https://wiki.linuxfoundation.org/realtime/documentation/start | surrogate_primary | 2026-09-02 | Linux Foundation | originator — PREEMPT_RT 实时补丁官方文档 |
| T06-S073 | https://www.universal-robots.com/products/ | surrogate_primary | 2026-09-02 | Universal Robots | vendor docs — 协作臂重复定位精度标注方式 |
| T06-S074 | https://www.harmonicdrive.net/technology | surrogate_primary | 2026-09-02 | Harmonic Drive | vendor docs — 谐波减速器原理与背隙说明 |
| T06-S075 | https://www.nabtesco.com/en/products/precision.html | surrogate_primary | 2026-09-02 | Nabtesco | vendor docs — RV 摆线针轮减速器 |
| T06-S076 | https://mujoco.readthedocs.io/en/stable/overview.html | surrogate_primary | 2026-09-02 | Google DeepMind | vendor docs — MuJoCo 物理引擎与接触模型 |
| T06-S077 | https://docs.isaacsim.omniverse.nvidia.com/ | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Isaac Sim / Lab 并行仿真 |
| T06-S078 | https://moveit.ai/ | surrogate_primary | 2026-09-02 | PickNik / MoveIt | vendor docs — 运动规划框架 |
| T06-S079 | https://hades.mech.northwestern.edu/index.php/Modern_Robotics | surrogate_primary | 2026-09-02 | Lynch & Park | publisher / 课程 — 《Modern Robotics》官方站与术语定义 |
| T06-S080 | https://underactuated.mit.edu/ | surrogate_primary | 2026-09-02 | Russ Tedrake, MIT | syllabus / 课程 — 欠驱动机器人讲义 |
| T06-S081 | https://lavalle.pl/planning/ | surrogate_primary | 2026-09-02 | Steven M. LaValle | publisher / 出版社 — 《Planning Algorithms》全文 |
| T06-S082 | https://ifr.org/robot-history | surrogate_primary | 2026-09-02 | IFR | association / 协会 — 工业与服务机器人定义口径 |
| T06-S083 | https://ifr.org/free-downloads | surrogate_primary | 2026-09-02 | IFR | association / 协会 — 机器人密度等统计口径 |
| T06-S084 | https://en.wikipedia.org/wiki/ISO_10218 | secondary | 2026-09-02 | — | 10218 版本沿革交叉核对 |
| T06-S085 | https://en.wikipedia.org/wiki/Robot_calibration | secondary | 2026-09-02 | — | 绝对精度 vs 重复精度的通俗界定 |
| T06-S086 | https://www.therobotreport.com/iso-10218-industrial-robot-safety-standard-receives-major-overhaul/ | secondary | 2026-09-02 | The Robot Report | 10218:2025 改版报道 |
| T06-S087 | https://www.therobotreport.com/now-available-full-403-page-ansi-a3-r15-06-2025-robot-safety-standard/ | secondary | 2026-09-02 | The Robot Report | R15.06-2025 篇幅与结构报道 |
| T06-S088 | https://eurogip.fr/en/machinery-regulation-2023-1230-what-the-digital-omnibus-on-ai-changes/ | secondary | 2026-09-02 | Eurogip | Omnibus 对机械法规的改动解读 |
| T06-S089 | https://robodk.com/doc/en/Robot-Validation-ISO9283.html | surrogate_primary | 2026-09-02 | RoboDK | vendor docs — ISO 9283 测试立方体实操口径 |
| T06-S090 | https://www.pilz.com/en-US/support/law-standards-norms/functional-safety | surrogate_primary | 2026-09-02 | Pilz | vendor docs — PL/SIL 对照与过渡期 |
| T06-S091 | http://www.news.cn/tech/20251227/68507c61722548a8befcb96df309418c/c.html | secondary | 2026-09-02 | 新华网 | 工信部人形机器人与具身智能标委会成立报道 |
| T06-S092 | https://www.news.cn/20260228/c27e2dfdb0f4496494c7e4991f2e8c2f/c.html | secondary | 2026-09-02 | 新华网 | 《标准体系（2026版）》发布报道 |
| T06-S093 | https://www.osha.gov/laws-regs/regulations/standardnumber/1910/1910.212 | verified_primary | 2026-09-02 | OSHA | regulator — 机械通用防护条款 |
| T06-S094 | https://www.osha.gov/laws-regs/oshact/section5-duties | verified_primary | 2026-09-02 | OSHA | regulator — OSH Act 一般责任条款 |
| T06-S095 | https://www.automate.org/robotics/robotics-certifications/robotic-integrator-certification-program | surrogate_primary | 2026-09-02 | A3 | association / 协会 — 集成商认证项目 |
| T06-S096 | https://chinajob.mohrss.gov.cn/upload/resources/jnbzpdf/4ccc6a76ab912072690801.pdf | verified_primary | 2026-09-02 | 人力资源社会保障部 | 监管 — 工业机器人系统运维员职业技能标准 |
| T06-S097 | https://www.miiteec.org.cn/plus/view.php?aid=1205 | surrogate_primary | 2026-09-02 | 工信部教育与考试中心 | certification body / 认证机构 — 职业技能标准颁布公告 |
| T06-S098 | https://www.tuvsud.com/en-us/services/functional-safety/iso-13849-iec-62061 | surrogate_primary | 2026-09-02 | TUV SUD | certification body / 认证机构 — PL/SIL 认证服务口径 |
| T06-S099 | https://ec.europa.eu/growth/tools-databases/nando/ | verified_primary | 2026-09-02 | 欧盟委员会 | 监管 — NANDO 公告机构数据库 |
| T06-S100 | https://www.iso.org/iso-9001-quality-management.html | surrogate_primary | 2026-09-02 | ISO | standards body — ISO 9001 质量管理体系 |

---

## 阅读说明

**这一行的语言有三套并存，混用就露怯：**

1. **机械/工业机器人一套**（ISO/GB 词汇、精度、节拍、PL/SIL）——说话人是集成商、产线工程师、安全工程师。名词有国标定义，说错会被当场纠正。
2. **学术/具身智能一套**（VLA、action chunking、cross-embodiment、sim2real）——说话人是研究员。名词多来自 2022 年后的论文，定义还在漂。
3. **落地工程一套**（干预率、循环时间、良率、换型、MTBF）——说话人是把 demo 变产品的人。这一套最能分辨「做过产品」和「只做过 demo」。

**中文圈口语的普遍情况**：技术名词大量直接说英文或中英混。`payload`「负载」两说都常见；`TCP`、`IK`、`MPC`、`VLA`、`sim2real`、`ROS`、`EtherCAT` 基本只说英文；`重复定位精度`、`节拍`、`换型`、`本体` 基本只说中文。下面每条会标「中文圈实际怎么说」。

**「本体」这个词要特别注意**：中文机器人圈里 `本体` = robot arm/robot body 这台机器（对应厂商语境的 "robot" 或 "manipulator"），而具身智能语境里的 `本体 / embodiment` = 某一个机器人形态（跨本体 cross-embodiment 的那个本体）。同一个中文词，工业圈指硬件实体，学术圈指形态类别。第一次跟对方说话要确认是哪个意思。

---

## A. 术语 — 本体与机械

> 这一组的定义大部分能在 ISO 8373:2021（机器人词汇，第 3 版，2021-11 发布）里查到官方版本 evidence: [T06-S001]

### A1. DOF — 自由度（degree of freedom）
- 中文圈说法：直接说「自由度」或 "DOF"（读字母 D-O-F，不读 "doff"）。
- Insider def：独立可控的运动轴数。工业臂 6 轴 = 6 DOF 刚好能任意位姿；7 DOF 是**冗余**，多出来那一维用来避奇异、避障、换构型。
- `_tell` 外行把「关节数」等同于「自由度」。夹爪的开合、带滑台的第 7 轴、双臂共用腰关节，算不算 DOF 取决于是否独立可控且参与末端位姿。人形机器人厂商宣传的「52 个自由度」通常把手指关节全算进去，跟工业臂的 6 DOF 不是一个量纲。

### A2. Reach — 臂展 / 工作半径
- 中文圈说法：「臂展」「工作半径」「够不够得着」。
- Insider def：从基座原点到腕心可达的最大距离；**规格书上的 reach 是腕心的，不含末端工具**。装上夹爪后有效 reach 变了、工作空间形状也变了。
- `_tell` 外行拿 reach 直接当「能操作的范围」。内行会问「灵巧工作空间（dexterous workspace）多大」——即在保持任意姿态的前提下能到达的区域，通常远小于可达工作空间。evidence: [T06-S079]

### A3. Payload — 负载
- 中文圈说法：「负载」「能扛多重」。
- Insider def：额定负载是在**指定重心偏置和转动惯量**下的值。同一台 20 kg 负载的臂，工具重心外伸 300 mm 时实际可用负载可能掉到 8 kg。
- `_tell` 外行说「这台机器人 20 公斤负载，我这个 15 公斤的件肯定行」。内行第一反应是问重心距离法兰多远、惯量多大、要不要高速。这是最常见的一句露馅话。

### A4. TCP — 工具中心点（tool center point）
- 中文圈说法：直接说 "TCP"（读字母）。注意与网络协议 TCP 同名，机器人语境里不会混。
- Insider def：定义在末端工具上的一个参考坐标系原点，示教、轨迹、精度都以它为准。**TCP 标定不准，所有精度指标都无意义**。
- `_tell` 外行以为 TCP 是机器人自带的固定点。内行知道每换一次工具就要重新标 TCP（四点法/六点法），且 TCP 误差会随姿态放大。

### A5. EOAT / End effector — 末端执行器 / 手爪 / 工装
- 中文圈说法：「末端」「手爪」「夹具」「EOAT」（读字母，北美用得多；欧洲更常说 gripper/end effector）。
- Insider def：装在法兰上的干活部件。产线上 **EOAT 的设计难度和交期常常是项目瓶颈**，比选哪台机器人重要。
- `_tell` 外行讨论「用哪个模型抓」，内行先问「用什么手爪、真空还是二指还是三指、有没有柔性指、换型要不要换爪」。

### A6. 谐波减速器 — harmonic drive / strain wave gear
- 中文圈说法：「谐波」（几乎不说全称）。
- Insider def：柔轮弹性变形传动，单级大减速比、体积小、**零背隙但有迟滞（hysteresis）和扭转刚度非线性**。协作臂和人形关节的主力方案。evidence: [T06-S074]
- `_tell` 外行说「谐波没有间隙所以精度高」。内行会说谐波的问题不是背隙而是**柔轮的扭转柔度和迟滞**，负载一变位置就偏，所以关节侧还要加编码器（双编码器）。

### A7. RV 减速器 / 摆线针轮 — cycloidal / RV reducer
- 中文圈说法：「RV」「摆线针轮」。
- Insider def：刚度高、抗冲击、适合大负载工业臂的前 3 轴；比谐波重、比谐波贵、背隙不为零但刚度高。evidence: [T06-S075]
- `_tell` 把 RV 和谐波当成「同类不同牌子」。内行的分工是：大臂用 RV（要刚度），小臂/腕用谐波（要轻和大减速比）。

### A8. Backlash — 背隙 / 回差
- 中文圈说法：「背隙」「回差」「间隙」。
- Insider def：传动链换向时的空程。它直接吃掉**双向重复定位精度**，且随磨损增大——这是老设备精度衰减的头号原因。
- `_tell` 外行把背隙和「精度」混谈。内行分得清：背隙影响的是换向重复性，而绝对精度主要被连杆参数误差和挠曲吃掉。

### A9. Backdrivability — 可反驱性
- 中文圈说法：「可反驱」「能不能推得动」「反驱」。
- Insider def：从输出端能否推动电机。高减速比 + 蜗杆式结构不可反驱；QDD 和低减速比可反驱。**可反驱是做力控与安全接触的物理前提**，不是软件能补出来的。
- `_tell` 外行说「加个力传感器就能做力控」。内行知道：不可反驱的关节即使测到力也来不及退让，带宽被机械限死。

### A10. SEA — 串联弹性驱动器（series elastic actuator）
- 中文圈说法：「SEA」「串联弹性」。
- Insider def：电机与负载之间串一个已知刚度的弹性元件，用弹簧变形量测力矩，天然做到力源特性和抗冲击。代价是控制带宽下降、位置刚度低。
- `_tell` 外行说「弹性关节 = 安全」。内行会追问弹簧刚度选多少、带宽掉到多少赫兹、能不能满足步态所需的力矩上升率。

### A11. QDD — 准直驱（quasi-direct drive）
- 中文圈说法：「准直驱」「QDD」「低减速比方案」。
- Insider def：大扭矩外转子电机 + 低减速比（常见 6:1~10:1）行星减速，靠电流环估力矩，牺牲峰值扭矩换可反驱和高带宽。四足与部分人形腿部的主流。
- `_tell` 外行把 QDD 当「直驱」。真直驱是 1:1 无减速。

### A12. 力矩密度 — torque density（N·m/kg）
- 中文圈说法：「力矩密度」「功率密度」。
- Insider def：关节模组的核心竞争指标。**要看是峰值还是连续**——峰值靠短时过流，连续受热限制。厂商标峰值、工程师算连续。
- `_tell` 只报峰值扭矩不报持续扭矩与热降额（derating）曲线，是硬件方最常见的话术。

### A13. IP 等级 — ingress protection（IP54 / IP67）
- 中文圈说法：「IP 几几」「防护等级」。
- Insider def：两位数字 = 防尘等级 + 防水等级。喷涂、食品、铸造场景对 IP 的要求经常直接决定选型；**IP67 的臂比同款 IP54 贵一档且散热更差**。
- `_tell` 把 IP67 说成「防水防尘都最好」。IP67 是短时浸水，IP69K 才是高压热水冲洗；且 IP 等级不覆盖化学腐蚀和粉尘爆炸（后者看 ATEX/防爆）。

### A14. 工作空间 — workspace / 灵巧工作空间 dexterous workspace
- 中文圈说法：「工作空间」「可达范围」。
- Insider def：可达工作空间（能到达）≠ 灵巧工作空间（到达且能任意姿态）≠ 无碰撞可用空间（装上工装和围栏后剩下的）。项目里真正能用的是第三个。evidence: [T06-S079, T06-S081]
- `_tell` 用厂商样本上的球形工作空间图直接做布局。内行会在仿真里跑一遍带工装的可达性 + 奇异回避 + 电缆干涉。

### A15. 本体 — robot body / manipulator（工业语境）vs embodiment（学术语境）
- 中文圈说法：工业圈「本体」= 不含控制柜和末端的那台机器；学术圈「本体」= embodiment，指形态。
- `_tell` 跨圈开会时不澄清这个词，两边会各说各的半小时。见「阅读说明」。

---

## B. 术语 — 控制与运动

### B1. 硬实时 — hard real-time / 抖动 jitter
- 中文圈说法：「硬实时」「实时性」「抖动」。
- Insider def：**硬实时不是「快」，是「最坏情况延迟有确定上界」**。1 kHz 伺服环允许的不是平均 1 ms，而是**每一拍都必须在 1 ms 内完成**，超一拍就可能丢步或触发保护。抖动（jitter）= 周期偏差的分布，比平均延迟重要得多。evidence: [T06-S072]
- `_tell` 「我们用的是实时系统，延迟只有几毫秒」——只报平均值不报最坏值和抖动，是最典型的外行/半吊子说法。内行报的是 `p99.9 / max jitter`。

### B2. 伺服周期 — servo cycle / control loop rate
- 中文圈说法：「伺服周期」「控制频率」「几赫兹的环」。
- Insider def：分层的：电流环 10~20 kHz（驱动器内）、速度/位置环 1~4 kHz、轨迹插补 250 Hz~1 kHz、规划与感知 10~30 Hz、大模型策略 3~50 Hz。**上层慢不要紧，下层不能抖**。
- `_tell` 说「我们的模型跑 30 Hz，所以机器人是 30 Hz 控制的」。内行知道 30 Hz 的策略输出必须被下层插值/平滑到伺服周期，中间那层才是安全和手感的关键。

### B3. 阻抗控制 — impedance control
- 中文圈说法：「阻抗控制」「阻抗」。
- Insider def：输入位置偏差、输出力（力矩），把机器人变成一个可调的「弹簧-阻尼-惯量」系统。需要力矩可控的关节（可反驱或带力矩传感器）。
- `_tell` 与导纳控制混用，见 B4 和 H 节。

### B4. 导纳控制 — admittance control
- 中文圈说法：「导纳控制」「导纳」。
- Insider def：输入测得的力、输出位置（速度）指令，套在**位置控制**的机器人外面。传统工业臂做拖动示教用的就是导纳。
- `_tell` 把阻抗和导纳当同义词。内行一句话分：**阻抗 = 位置进力出（适合刚度低、可反驱的机器人）；导纳 = 力进位置出（适合刚度高、位置控的机器人）**。硬接触时导纳容易不稳定，自由空间里阻抗容易漂——这是选型的实际分界。

### B5. 力/位混合控制 — hybrid force/position control
- 中文圈说法：「力位混合」「力控」。
- Insider def：在任务空间里把某些方向设为力控（如法向压紧），其余方向位置控（如切向进给）。装配、打磨、插拔的标准做法。
- `_tell` 外行说「力控」泛指一切碰得到东西的控制。内行会问「力控是哪个方向的、力的分辨率多少、力控带宽多少 Hz、用关节力矩还是六维力传感器」。

### B6. 重力补偿 — gravity compensation
- 中文圈说法：「重力补偿」。
- Insider def：在力矩指令中前馈掉连杆和负载自重。**没有准确的负载辨识（质量、重心、惯量）就没有可用的重力补偿**，这也是换工具后必须重新做负载辨识的原因。
- `_tell` 把「拖动示教手感不好」归因于算法，内行第一步查负载参数有没有重新标定。

### B7. 奇异位形 — singularity
- 中文圈说法：「奇异」「奇异点」「过奇异」。
- Insider def：雅可比降秩的位形，末端某个方向瞬时失去可控性，逆运动学解算出无穷大关节速度。腕奇异、肩奇异、肘（边界）奇异三类。
- `_tell` 外行说「机器人在这里会卡住/报警是坏了」。内行说「这条轨迹过奇异了，得改姿态或用冗余自由度绕开」。

### B8. 冗余与零空间 — redundancy / null space
- 中文圈说法：「冗余」「零空间」「自运动」。
- Insider def：DOF > 任务维度时存在零空间运动——末端不动、手肘能动。用来避障、避奇异、避关节限位、优化能耗。7 轴臂和人形手臂的核心价值在这里。
- `_tell` 「7 轴比 6 轴精度高」。冗余带来的是可达性与避障能力，不是精度。

### B9. ZMP — 零力矩点（zero moment point）
- 中文圈说法：直接说 "ZMP"。
- Insider def：地面反力合力矩水平分量为零的点。ZMP 落在支撑多边形内 = 不会绕脚边翻倒。**它是「不翻倒」的判据，不是「稳定」的充要条件**，也不适用于有飞行相的动态动作。
- `_tell` 把 ZMP 当成「平衡算法」。ZMP 是一个量/判据，基于它的走路方法叫 ZMP-based / preview control 步态。近几年动态运动主要不用纯 ZMP 了。

### B10. 捕获点 / DCM — capture point / divergent component of motion
- 中文圈说法：「捕获点」「DCM」「LIPM 的发散分量」。
- Insider def：把线性倒立摆的不稳定模态分离出来，落脚点踩在捕获点上就能一步止住。推倒恢复（push recovery）与落脚点规划的基础。
- `_tell` 外行看到机器人被推一下没倒就说「平衡做得好」。内行看的是它**改没改落脚点**——不迈步的只是踝策略，能迈步调整的才是 capture-point 级别。

### B11. MPC — 模型预测控制（model predictive control）
- 中文圈说法：直接说 "MPC"。
- Insider def：在有限时域内滚动求解带约束的最优控制，只执行第一步。足式和移动操作的主力。**关键指标是求解频率与预测时域**，不是「用了 MPC」本身。
- `_tell` 说「我们用 MPC 所以很鲁棒」。内行问：多少 Hz 重规划、时域多长、模型是质心动力学还是全身、约束里有没有摩擦锥、求不出解时的 fallback 是什么。

### B12. WBC — 全身控制（whole-body control）
- 中文圈说法：「WBC」「全身控制」「优先级任务」。
- Insider def：把多个任务（质心、末端、姿态、接触力）按优先级或加权解成一个 QP，一次性算出所有关节力矩。通常跑在 MPC 下面、以 500 Hz~1 kHz 执行。
- `_tell` 把 WBC 和 MPC 当二选一。工程实践里常见的是 **MPC（低频、长时域、简化模型）+ WBC（高频、瞬时、全身模型）** 两层叠。

### B13. 步态 — gait / 支撑相 stance、摆动相 swing、占空比 duty factor
- 中文圈说法：「步态」「支撑相/摆动相」「trot/慢跑」。
- Insider def：接触序列的时间安排。四足的 trot / pace / bound、双足的单支撑/双支撑相。**「步态生成」和「落脚点规划」是两件事**。
- `_tell` 用「走得像人」评价双足。内行看的是接触切换时有没有冲击、有没有拖脚、能不能在不平地面上改接触时序（contact schedule）。

### B14. 路径 vs 轨迹 — path vs trajectory
- 中文圈说法：「路径规划」「轨迹规划」，中文里常被混用，但工程上必须分。
- Insider def：**路径是几何（一串位形，无时间）；轨迹是路径 + 时间参数化（含速度、加速度、加加速度）**。RRT/PRM 出的是路径，时间最优参数化（TOPP）后才是轨迹。evidence: [T06-S081]
- `_tell` 说「规划出一条轨迹，然后让它慢点走」——内行知道降速要重新做时间参数化，不是简单缩放（关节限速/限加速度约束不是线性的）。

### B15. IK / FK — 逆运动学 / 正运动学
- 中文圈说法：「IK」「逆解」「正解」。
- Insider def：FK 唯一解；IK 多解（6 轴常见 8 组）+ 可能无解。**「解算失败」在产线上通常不是数学问题，是位形跳变/关节翻转**（configuration flip）。
- `_tell` 外行以为 IK 是「算一下就好」。内行关心的是解的连续性、构型分支（肩左/右、肘上/下、腕翻转）在整条轨迹上是否保持一致。

### B16. 顺应 / 柔顺 — compliance
- 中文圈说法：「柔顺」「顺应性」「软一点」。
- Insider def：分**被动柔顺**（机械结构本身有弹性，如 SEA、RCC 柔性手腕）和**主动柔顺**（控制器造出来的）。被动柔顺在碰撞瞬间就生效，主动柔顺受采样周期和带宽限制。
- `_tell` 「我们是柔性机器人，撞到人不会伤人」。内行知道这句话只有配上「在什么速度、什么接触面积、按 ISO 10218 系列的力/压强限值实测过」才成立。见 J 节。

---

## C. 术语 — 感知、状态估计与标定

### C1. 手眼标定 — hand-eye calibration（eye-in-hand / eye-to-hand）
- 中文圈说法：「手眼标定」「标定手眼关系」；两种构型说「眼在手上」「眼在手外」。
- Insider def：求相机坐标系与机器人法兰（或基座）之间的刚体变换，经典形式 `AX = XB`。**是所有视觉引导抓取的地基**；标不准，模型再好也抓偏。
- `_tell` 外行说「视觉识别准确率 99%，所以抓取成功率也应该很高」。内行知道：识别是像素级、抓取是毫米级，中间隔着手眼标定、相机内参、深度误差、TCP 误差、机械挠曲的误差链。

### C2. 内参 / 外参 — intrinsics / extrinsics
- 中文圈说法：「内参」「外参」「重标一下」。
- Insider def：内参 = 焦距、主点、畸变；外参 = 相机相对世界/机器人的位姿。**内参会随温度和振动漂**，产线上有定期复标制度。
- `_tell` 只标一次就当永久有效。内行会问「多久复标一次、用什么判据触发复标（重投影误差阈值）」。

### C3. 6D 位姿 — 6D pose（3 平移 + 3 旋转）
- 中文圈说法：「6D 位姿」「位姿」「pose」。注意中文「位姿」= position + orientation，比「位置」多三维。
- `_tell` 外行说「位置估计」「定位」时其实指 6D 位姿。内行严格区分 position（3D）/ pose（6D）/ transform（变换）。

### C4. 点云配准 — point cloud registration / ICP
- 中文圈说法：「配准」「ICP」「点云对齐」。
- Insider def：把观测点云对齐到模型或另一帧点云。ICP 需要好初值，容易陷局部极小；工业上通常先用全局粗配准（特征/PPF）再 ICP 精配。
- `_tell` 认为「有了点云就有了精确位姿」。内行关心的是点云的**深度噪声模型**（结构光近距准、ToF 远距准、双目依赖纹理）和反光/透明件的失效模式。

### C5. SLAM — 同步定位与建图
- 中文圈说法：直接说 "SLAM"（读 "斯拉姆"）。
- Insider def：一边估自身位姿一边建环境地图。AMR 用激光 SLAM 为主，视觉 SLAM 做辅助或低成本方案。
- `_tell` 外行把「有 SLAM」当成「导航能力强」。内行问的是**重定位（relocalization）成功率、动态环境下的地图退化、长走廊/大空场的退化方向、回环检测频次**。

### C6. VIO — 视觉惯性里程计（visual-inertial odometry）
- 中文圈说法：「VIO」。
- Insider def：相机 + IMU 紧耦合估计位姿，短时精度高、无回环时长期漂移。人形/四足的躯干状态估计常用 VIO + 腿式里程计（leg odometry）融合。
- `_tell` 把 VIO 和 SLAM 划等号。VIO 没有全局地图和回环，只有里程计。

### C7. 里程计漂移 / 回环检测 — odometry drift / loop closure
- 中文圈说法：「漂移」「回环」「累计误差」。
- Insider def：漂移量按「每米/每百米的相对误差」报，不是绝对值。回环检测把累计误差一次性压回去，代价是地图会「跳」。
- `_tell` 报「定位精度 2 cm」而不说是在什么距离、有没有回环、有没有反光柱/二维码辅助。

### C8. F/T 传感器与触觉 — force/torque sensor、tactile sensing
- 中文圈说法：「六维力」「力传感器」「触觉」。
- Insider def：腕部六维力/力矩传感器测的是**工具端合力**，测不出接触点在哪；分布式触觉（阵列式、视触觉如 GelSight 类）能给接触位置与滑移。**温漂和过载保护是六维力最现实的坑**。
- `_tell` 说「加了触觉就能做精细操作」。内行问采样率、分辨率、串扰、标定漂移、以及策略是否真用了这一路信号（很多论文里触觉通道被网络忽略）。

### C9. 深度相机三种原理 — 结构光 / ToF / 双目
- 中文圈说法：「结构光」「ToF」「双目」。
- Insider def：结构光近距高精但怕环境光与反光；ToF 远距快但多径误差与飞点；双目依赖纹理、可加投射器。**选型是被物料表面决定的**，不是被参数表决定的。
- `_tell` 只比较「深度精度 ±1 mm」这一个数，不问在什么距离、什么反射率、什么环境光下测的。

### C10. 抓取位姿检测 — grasp pose detection / antipodal grasp
- 中文圈说法：「抓取位姿」「抓点」「grasp」。
- Insider def：从点云/图像里输出一组可行的夹爪 6D 位姿 + 打分。二指夹爪常用 antipodal（对向）假设。**输出是候选集合，落地时还要过可达性、碰撞、力封闭、后续放置姿态的筛选**。
- `_tell` 把「抓取检测网络的 top-1 分数」当成抓取成功率。

### C11. 重投影误差 — reprojection error
- 中文圈说法：「重投影误差」「像素误差」。
- Insider def：标定质量的最常用数值判据（亚像素级算好）。**但重投影误差小不代表标定对**——标定板摆位覆盖不足时会过拟合。
- `_tell` 只报一个 0.2 px 就宣布标定完成。内行看误差分布、标定板姿态多样性、以及是否用独立数据做了验证。

### C12. 状态估计 — state estimation（vs「定位」）
- 中文圈说法：「状态估计」「估计器」。
- Insider def：足式机器人里指估躯干位姿 + 速度 + 接触状态 + IMU 零偏，通常是 EKF/因子图。**接触检测错一次，速度估计就会瞬间发散**。
- `_tell` 把状态估计说成「定位」。定位是其中一个输出维度。

---

## D. 术语 — 学习与具身大模型（IL / RL / VLA）

### D1. 行为克隆 — behavior cloning (BC)
- 中文圈说法：「BC」「行为克隆」「模仿学习」（后者是更大的类）。
- Insider def：把「观测 → 动作」当监督学习拟合。简单、样本效率高，缺点是只在演示分布内有效。
- `_tell` 说「我们做的是模仿学习」而讲不出跟 BC 的区别。模仿学习 ⊃ BC、DAgger、逆强化学习、对抗式模仿。

### D2. 协变量偏移 / 误差累积 — covariate shift / compounding error
- 中文圈说法：「协变量偏移」「误差累积」「越走越偏」。
- Insider def：策略自己开出去后访问到训练集里没有的状态，误差按时间步二次累积——这是 BC 的**根本病**，不是数据量问题。DAgger 就是为这个提出的。evidence: [T06-S062]
- `_tell` 「多采点数据就好了」。内行知道要采的是**恢复行为（recovery）数据**，即从偏离状态回到正轨的演示，不是更多的完美演示。

### D3. DAgger — dataset aggregation
- 中文圈说法：直接说 "DAgger"（读 "dagger"）。
- Insider def：让策略自己跑、专家在线标注正确动作、把这些状态加进数据集迭代重训。理论上把二次累积误差降到线性。evidence: [T06-S062]
- `_tell` 把 DAgger 当成「人工纠错的数据增强」。它的关键是**在策略访问的状态分布上**标注，而不是在人的分布上补数据。

### D4. Action chunking — 动作分块
- 中文圈说法：直接说 "action chunking"，或「动作块」「一次预测一段」。
- Insider def：一次预测未来 k 步动作序列并执行（或做时序集成 temporal ensembling），显著缓解误差累积与非马尔可夫性、减少抖动。ACT 把它带火。evidence: [T06-S056]
- `_tell` 外行说「模型输出频率低所以动作卡」。内行知道分块长度 k 是精度/反应性权衡的旋钮：k 太大不能对扰动做出反应，k 太小抖。

### D5. Diffusion policy — 扩散策略
- 中文圈说法：「扩散策略」「diffusion policy」「DP」。
- Insider def：用去噪扩散过程表示动作分布，能表达多峰行为（同一场景有多种正确做法），比高斯回归稳。代价是推理要多步去噪，需要蒸馏/流匹配加速。evidence: [T06-S055]
- `_tell` 「扩散模型是生成图片的，怎么控制机器人」。内行的点在于它建模的是**动作序列的条件分布**，多峰性正是遥操作数据的固有性质。

### D6. VLA — 视觉-语言-动作模型（vision-language-action model）
- 中文圈说法：直接说 "VLA"（读字母）。
- Insider def：把视觉语言模型的骨干拿来直接输出机器人动作 token / 连续动作，靠互联网语义先验做泛化。术语出自 RT-2（2023-07）。evidence: [T06-S057, T06-S059, T06-S061]
- `_tell` 把任何「用了大模型的机器人」都叫 VLA。内行区分：**VLM 做高层任务分解 + 传统控制执行**（分层）与 **VLA 端到端出动作** 是两条不同路线，性能与失败模式完全不同。
- `_tell` 说「VLA 是机器人的 GPT 时刻」——这是发布会语言，见 P 节。

### D7. 跨本体 — cross-embodiment
- 中文圈说法：「跨本体」「跨平台」。
- Insider def：同一策略/数据跨不同机器人形态使用。Open X-Embodiment 把它变成了公共议题。evidence: [T06-S060]
- `_tell` 「这个模型能跨本体」而不说是**跨相似形态**（都是 6-7 轴 + 二指爪）还是真的跨到不同 DOF/不同夹爪/不同视角。绝大多数「跨本体」结果属于前者。

### D8. 域随机化 — domain randomization
- 中文圈说法：「域随机化」「DR」「随机化」。
- Insider def：在仿真里随机化视觉外观或物理参数（质量、摩擦、延迟、电机常数），逼策略学到对参数不敏感的行为。视觉 DR 出自 Tobin 2017，动力学 DR 出自 Peng 2017。evidence: [T06-S063, T06-S064]
- `_tell` 「随机化范围越大越鲁棒」。内行知道范围过大策略会退化成保守/僵硬行为，实践上要配 curriculum 或自适应范围。

### D9. Teacher-student / 特权学习 — privileged learning
- 中文圈说法：「teacher-student」「特权信息」「蒸馏」。
- Insider def：先在仿真里用**特权观测**（真实地形高度、真实摩擦、真实状态）训一个 teacher，再蒸馏成只能看本体感受/相机的 student。足式 sim-to-real 的标准配方。evidence: [T06-S065]
- `_tell` 把它说成「模型蒸馏」。这里蒸馏的不是模型大小，是**观测空间**。

### D10. 离线 RL — offline RL / batch RL
- 中文圈说法：「离线 RL」。
- Insider def：只用固定数据集训，不与环境交互，核心难点是分布外动作的价值高估。真机数据贵时的现实选择。
- `_tell` 把「用历史数据训练」都叫离线 RL。若没有奖励标注和保守约束，那只是 BC。

### D11. 奖励塑形 — reward shaping
- 中文圈说法：「奖励设计」「reward shaping」「调奖励」。
- Insider def：加中间奖励项引导探索。**足式 RL 的实际工作量大头在这里**（跟踪项、能耗项、脚滑项、关节限位项、动作平滑项的权重表）。
- `_tell` 说「RL 自己学会走路」。内行知道 reward 里通常有十几项手工权重，改一个数就换一种步态。

### D12. sim2real gap / reality gap — 仿真到现实的差距
- 中文圈说法：「sim2real」「仿真差距」「仿真跟真机不一样」。
- Insider def：来源是接触模型、执行器动力学（含延迟与传动柔性）、传感器噪声、以及仿真里没建的东西（线缆、间隙、温漂）。**接触和执行器是两个最大头**。
- `_tell` 「我们仿真里成功率 95%」。这句话在这行等于什么都没说——内行只问真机数、试了多少次、谁在旁边。

### D13. 遥操作 / 数据采集 — teleoperation, data collection
- 中文圈说法：「遥操作」「遥操」「采数据」「主从」。
- Insider def：用主端设备（同构主臂、VR 手柄、外骨骼、手套）驱动从端采演示数据。**数据的质量由采集者一致性、时延、力反馈有无决定**；无力反馈的遥操作采不到细腻的接触策略。
- `_tell` 只报「采了 X 万条轨迹」，不报任务种类数、场景数、物体数、采集人数、成功轨迹占比、每条平均时长。数据量在这行不是单一维度。

### D14. 泛化（四个层次）— generalization
- 中文圈说法：「泛化」。这是这一行最被滥用的词。
- Insider def：至少要分四层说清是哪一层：**新物体**（同类不同实例）、**新场景**（换背景/光照/桌面/干扰物）、**新任务**（新指令组合）、**新本体**（换机器人）。难度依次递增，绝大多数论文的「泛化」是第一、二层。evidence: [T06-S057, T06-S059, T06-S060]
- `_tell` 只说「泛化好」不说哪一层——最典型的外行/营销破绽。

### D15. 零样本 / 少样本 — zero-shot / few-shot
- 中文圈说法：「零样本」「zero-shot」「不用微调」。
- Insider def：严格意义是该任务/物体在训练数据中完全没出现过。实务上大量所谓 zero-shot 是「没在这个具体实例上训过，但同类见过很多」。
- `_tell` 见 P 节，这是厂商话术重灾区。

### D16. 语言条件 / 指令跟随 — language-conditioned policy
- 中文圈说法：「语言条件」「用自然语言指挥」。
- Insider def：策略以文本指令为条件。**指令的分布通常极窄**（模板化的动词+名词），真正的开放指令跟随还很弱。
- `_tell` 拿视频里「说一句话它就做了」当通用能力证据。内行问的是指令模板集合有多大、换个说法还行不行。

---

## E. 术语 — 仿真与 sim-to-real

### E1. 接触求解 — contact solver / 穿模 penetration
- 中文圈说法：「接触」「求解器」「穿模」「打滑」。
- Insider def：刚体仿真的接触是数值近似（软接触/LCP/凸松弛），不同引擎结论不同。**抓取、插装、行走这些强接触任务，仿真结论跨引擎不可移植**。evidence: [T06-S076]
- `_tell` 拿一个引擎的成功率当客观事实。内行会说「这个结果在 MuJoCo 里成立，换到别的接触模型未必」。

### E2. 系统辨识 — system identification（sysid）
- 中文圈说法：「辨识」「sysid」「对齐真机参数」。
- Insider def：用真机数据拟合仿真参数（惯量、摩擦、电机常数、延迟）。**是缩小 sim2real gap 里性价比最高的一步**，常常比换算法有效。
- `_tell` 只做域随机化不做辨识，或反过来。实践上是两者配合：辨识把中心对上，随机化把方差覆盖住。

### E3. 并行仿真 — massively parallel simulation / GPU envs
- 中文圈说法：「并行环境」「几千个环境一起跑」「GPU 仿真」。
- Insider def：在 GPU 上并行成千上万个实例，把足式 RL 的训练从天级压到小时/分钟级。evidence: [T06-S077]
- `_tell` 拿「并行 4096 个环境」当性能指标。这是吞吐，不是策略质量。

### E4. 模型描述格式 — URDF / SRDF / MJCF / USD
- 中文圈说法：「URDF」「模型文件」「MJCF」「USD」。
- Insider def：URDF 是 ROS 生态的机器人描述（树状，不支持闭链）；MJCF 是 MuJoCo 的；USD 是 NVIDIA 生态的场景描述。**惯量参数写错是仿真跑不对的头号低级错误**。
- `_tell` 以为 URDF 里的东西就是真机。URDF 通常缺传动柔性、间隙、线缆、真实电机模型。

### E5. 数字孪生 — digital twin（与「仿真」的区别）
- 中文圈说法：「数字孪生」——在中国的产业语境里被大量泛用。
- Insider def：严格意义指**与真实设备保持数据同步、随真机状态更新**的模型；只是照着 CAD 建了个 3D 场景跑仿真，那叫仿真/离线编程，不是数字孪生。
- `_tell` 把离线编程演示叫数字孪生。见 P 节。

### E6. 随机化课程 — randomization curriculum / 自适应 DR
- 中文圈说法：「课程」「curriculum」「逐步加难」。
- Insider def：随训练进度扩大随机化范围或地形难度，避免一开始就把策略压成保守解。
- `_tell` 认为 curriculum 只是「先易后难」的直觉。内行关心的是切换判据（成功率阈值/自动课程）与是否引入了不该有的偏置。

---

## F. 术语 — 通信、实时与系统软件栈

### F1. ROS 2 — 节点 / 话题 / 服务 / 动作
- 中文圈说法：「ROS」「ROS 2」「跑个 node」「发个 topic」。
- Insider def：进程间通信 + 工具链的中间件，不是操作系统也不是实时系统。话题（topic）异步发布订阅、服务（service）请求响应、动作（action）带反馈的长任务。evidence: [T06-S067, T06-S068]
- `_tell` 说「ROS 2 是实时的」。ROS 2 **提供了实时友好的执行器与内存分配策略**，但实时性来自内核（PREEMPT_RT）、DDS 配置和你自己的代码，不是 ROS 自带的属性。伺服环基本不放在 ROS 里跑。

### F2. DDS — 数据分发服务（Data Distribution Service）
- 中文圈说法：直接说 "DDS"。
- Insider def：OMG 的发布订阅中间件规范，ROS 2 的默认底座（Fast DDS / Cyclone DDS / Connext 等实现）。evidence: [T06-S069, T06-S068]
- `_tell` 把 DDS 当成「ROS 2 的一个库」。它是**可替换的实现层**，选哪个实现、怎么配发现（discovery）直接决定多机通信是否可用。

### F3. QoS — 服务质量策略
- 中文圈说法：「QoS」「可靠性策略」「深度设多少」。
- Insider def：reliability（reliable/best-effort）、durability、history/depth、deadline、liveliness 等。**发布端和订阅端 QoS 不兼容就静默连不上**——ROS 2 里最常见的「明明发了收不到」。evidence: [T06-S067]
- `_tell` 遇到收不到消息先怀疑网络，内行先 `ros2 topic info -v` 看 QoS 兼容性。

### F4. EtherCAT — 工业实时以太网
- 中文圈说法：直接说 "EtherCAT"（读 "以太卡特"）。
- Insider def：主从式实时总线，报文「飞过」从站直接读写，微秒级周期与分布时钟（Distributed Clock）同步。多关节机器人和高性能伺服的事实标准之一。evidence: [T06-S070]
- `_tell` 把 EtherCAT 当「跑在以太网上的协议，所以能用交换机随便接」。它有拓扑与从站顺序的强要求，普通交换机会破坏实时性。

### F5. CANopen / CiA 402
- 中文圈说法：「CAN」「CANopen」「402 协议」「PDO/SDO」。
- Insider def：CAN 上的应用层协议，CiA 402 是伺服驱动的行规（位置/速度/力矩模式、状态机）。带宽低但便宜、抗干扰，移动机器人和小型关节常用。evidence: [T06-S071]
- `_tell` 说「CAN 总线延迟很低」。CAN 是仲裁式的，**优先级低的帧在总线忙时延迟不可预测**，做高频力矩环要看清负载率。

### F6. PREEMPT_RT — Linux 实时补丁
- 中文圈说法：「实时内核」「打 RT 补丁」「PREEMPT_RT」。
- Insider def：把 Linux 大部分临界区变为可抢占，目标是把最坏调度延迟压到几十微秒量级。**它降低的是延迟上界（抖动），不是提高吞吐**。evidence: [T06-S072]
- `_tell` 「装了实时内核就实时了」。还要做 CPU 隔离（isolcpus）、关电源管理与超线程、锁页内存、避免动态分配与日志阻塞——少一步就前功尽弃。

### F7. 上位机 / 下位机（实时层与非实时层）
- 中文圈说法：「上位机」「下位机」「运控」——这是中文工业圈非常高频、英文里没有完全对应词的一对词。
- Insider def：下位机 = 跑硬实时伺服/安全逻辑的控制器（专用控制柜、实时 Linux、PLC、驱动器）；上位机 = 跑感知、规划、大模型的通用计算机。**接口协议与最坏延迟是这条边界上的核心设计决策**。
- `_tell` 把大模型直接接到伺服环上讨论。内行的默认架构是分层 + 下位机独立的限速限力保护。

### F8. STO / 安全 IO — safe torque off
- 中文圈说法：「STO」「安全转矩关断」「安全回路」。
- Insider def：驱动器级的硬件安全功能，切断电机力矩输出而不必断主电。属于 IEC 61800-5-2 的安全子功能族（如 STO / SS1 / SLS / SLP），在机器人上与 PL/SIL 评估绑定。
- `_tell` 把「急停」和「STO」当一回事，或把「软件里加个停止指令」当安全功能。安全功能必须走独立的、经评估的安全通道。见 J 节与「合规红线」。

### F9. 急停 — emergency stop / 停止类别 0-1-2
- 中文圈说法：「急停」「拍下急停」「Cat.0/Cat.1」。
- Insider def：IEC 60204-1 定义停止类别：**0 类 = 立即切断动力（非受控停止）；1 类 = 受控减速后切断动力；2 类 = 受控停止但动力保持**。急停必须是 0 类或 1 类。evidence: [T06-S020, T06-S021]
- `_tell` 说「急停就是马上停」。内行会区分：机械臂高速运动时 0 类急停靠惯性停，制动距离可能比 1 类更长、还更伤机械。

### F10. 时间同步 — PTP / 硬件触发 / 时间戳对齐
- 中文圈说法：「时间同步」「对时」「硬触发」。
- Insider def：多相机 + IMU + 关节编码器的数据必须同源时间戳，否则融合结果系统性偏差。IEEE 1588 (PTP) 或总线分布时钟做同步，相机用硬件触发。
- `_tell` 用软件时间戳做 VIO 或视觉伺服。内行第一句问「同步是软的还是硬的、误差多少微秒」。

---

## G. 术语 — 评测、产线与运营指标

> 这一组是最能区分「做过产品」与「只做过 demo」的语言。

### G1. 重复定位精度 vs 绝对定位精度 — pose repeatability vs pose accuracy
- 中文圈说法：「重复定位精度」（最常用）、「绝对精度」「定位精度」。
- Insider def：**ISO 9283:1998 把两者严格分开**：pose accuracy（位姿准确度）= 指令位姿与多次实到位姿均值之差；pose repeatability（位姿重复性）= 多次实到位姿的离散度。规格书上标的 ±0.02 mm 几乎总是**重复性**，而绝对精度通常差一到两个数量级（毫米级）。evidence: [T06-S006, T06-S085]
- **测法要点**：在机器人工作空间内取最大内接立方体（ISO 测试立方体）上的 5 个位姿、每个位姿测 30 次；重复性 RP 定义为到质心平均距离加 3 倍标准差。evidence: [T06-S006, T06-S089]
- `_tell` **这是本行第一号外行破绽**：外行说「这台机器人精度 0.02 毫米」。内行立刻会问「是重复定位精度还是绝对精度？按 ISO 9283 在哪个负载、哪个速度、哪个立方体测的？」。中文里说「精度」而不限定，在正式场合会被当成不专业。

### G2. 循环时间 — cycle time
- 中文圈说法：「循环时间」「一个循环多久」「CT」。
- Insider def：完成一个完整作业循环的时间（含取放、等待、复位）。**产线上一切优化的分母**。
- `_tell` 只报「抓取用时 1.2 秒」不报整循环。

### G3. 节拍 — takt time
- 中文圈说法：「节拍」「TT」。
- Insider def：**由客户需求决定的时间配额**（可用工时 ÷ 需求量），是目标；循环时间是实际。**节拍 ≠ 循环时间**，混用会导致产能算错。
- `_tell` 中文里「节拍」经常被拿来指循环时间。跟精益/工业工程背景的人对话时这会立刻暴露。

### G4. 换型时间 — changeover / SMED
- 中文圈说法：「换型」「换线」「切换产品要多久」。
- Insider def：从上一种产品切到下一种产品所需的停机时间（含换爪、改程序、重标定、首件验证）。**柔性产线的真实瓶颈常在这里，不在机器人本身**。
- `_tell` 谈「柔性生产」却答不出换型时间和首件合格所需时间。

### G5. MTBF / MTTR — 平均无故障时间 / 平均修复时间
- 中文圈说法：「MTBF」「MTTR」。
- Insider def：可靠性与可维护性的一对指标。**机器人本体的 MTBF 通常远好于系统 MTBF**——系统故障多来自末端工装、视觉、上下料、线缆。
- `_tell` 引用厂商本体 MTBF 当系统可用性依据。

### G6. OEE — 设备综合效率（overall equipment effectiveness）
- 中文圈说法：「OEE」。
- Insider def：可用率 × 性能 × 良品率。客户验收常以 OEE 或直通率写进合同。
- `_tell` 把 OEE 当成「开机率」。

### G7. 良率 / 直通率 — yield / first pass yield (FPY)
- 中文圈说法：「良率」「直通率」「一次合格率」。
- `_tell` 报「成功率 95%」时不说失败的那 5% 是**可恢复**（重试即可）还是**破坏性**（撞件、划伤、掉件）。这两者对产线的意义天差地别。

### G8. 成功率 — success rate（**分母是关键**）
- Insider def：只有写清「**任务定义 + 试验次数 + 初始状态分布 + 判定标准 + 是否允许重试 + 是否有人在旁**」的成功率才有意义。
- `_tell` **本行第二号破绽**：说「成功率 90%」不给分母。内行的标准问法是：「多少次里的 90%？物体位置是随机摆的还是固定的？失败算不算重试？演示视频是第几次拍的？」

### G9. 干预率 — interventions per hour / MPI（mean [distance|tasks] per intervention）
- 中文圈说法：「干预率」「多久要人接管一次」「每小时接管几次」。
- Insider def：长时运行时人类介入的频次。**比成功率更能反映能不能上线**，因为它包含了长尾。
- `_tell` 只讲单次任务成功率，不讲连续跑 8 小时的干预率。

### G10. 自主率 / 接管 — autonomy rate / takeover
- 中文圈说法：「自主率」「接管率」「遥操作兜底」。
- Insider def：在部署里明确「哪些环节是自主的、哪些是遥操作兜底」。当前多数人形/移动操作的商业部署是**有人远程兜底**的。
- `_tell` 用「全自主」描述带远程兜底的部署。见 P 节。

### G11. 示教 / 示教器 — teaching / teach pendant
- 中文圈说法：「示教」「示教器」「拖动示教」「点位」。
- Insider def：传统工业机器人的编程方式（在线示教点位或离线编程）。**产线上「谁能改程序」是运维成本的关键**。
- `_tell` 认为「以后都用 AI 就不用示教了」。现实是绝大多数在役产线仍是示教/离线编程，且改动需要复现验证。

### G12. 机器人密度 — robot density（台/万名员工）
- 中文圈说法：「机器人密度」。
- Insider def：IFR 的统计口径，用于国别比较。**「机器人+」方案里「制造业机器人密度较 2020 年翻番」用的就是这个口径**。evidence: [T06-S043, T06-S083]
- `_tell` 拿装机量（installations）和存量（operational stock）混着说。

### G13. 回收期 / ROI — payback period
- 中文圈说法：「回收期」「几年能回本」「ROI」。
- Insider def：客户实际决策的量尺。计算里要含集成费、工装、停线损失、运维与备件，不只是机器人价格。
- `_tell` 只比机器人本体单价。行业里本体常只占项目总价的 20-40%。

### G14. 力/压强限值（协作场景）— force and pressure limits
- 中文圈说法：「碰撞力限值」「压力压强限值」「按 15066 那张表」。
- Insider def：人机协作的功率与力限制（PFL）模式下，对人体各部位规定的准静态与瞬态力/压强上限，需用专用测力装置**实测**。原本在 ISO/TS 15066:2016，现已并入 ISO 10218 系列 2025 版。evidence: [T06-S004, T06-S003, T06-S026]
- `_tell` 说「协作机器人天生安全」。**安全属于应用，不属于本体**——同一台协作臂装上刀具就不再是协作应用。见 J 节。

---

## H. 一词多义：同一个词在不同子领域含义不同

| 词 | 语境 A | 语境 B | 怎么点破 |
|---|---|---|---|
| **精度 / accuracy** | 工业机器人：绝对定位准确度（毫米级） | 工业机器人：重复定位精度（±0.02 mm 级） | 说「精度」必须限定是哪一个 + 按 ISO 9283 / GB/T 12642 的哪个条件测。evidence: [T06-S006, T06-S048] |
| **实时 / real-time** | 控制：最坏延迟有确定上界（硬实时） | 日常/AI：跑得快、能在线跑 | 问「你说的实时是有 deadline 保证，还是只是低延迟？抖动多少？」evidence: [T06-S072] |
| **泛化 / generalization** | VLA：新物体 / 新场景 / 新任务 / 新本体 四层 | 营销：什么都能干 | 逼问是哪一层、评测集怎么划的。evidence: [T06-S060] |
| **成功率 / success rate** | 工程：带分母与判定标准 | demo：剪辑后的一次成功 | 问分母、初始分布、是否允许重试。 |
| **本体** | 工业：这台机器（硬件） | 具身智能：embodiment（形态类别） | 开会先对齐。 |
| **协作 / collaborative** | 标准：一种**应用**方式（人机共享空间且经风险评估） | 营销：一类产品（协作臂） | 「协作是应用属性不是产品属性」。evidence: [T06-S026, T06-S003] |
| **自主 / autonomous** | 部署：无人介入完成闭环 | 演示：有远程兜底/有人盯着 | 问干预率与兜底方式。 |
| **安全 / safety** | 功能安全（PL/SIL、失效率） | 口语「不会撞到人」 | 问安全功能是哪些、达到 PL 几、谁做的验证。evidence: [T06-S008, T06-S018] |
| **标定 / calibration** | 视觉：内外参、手眼 | 机械：运动学参数辨识（DH 修正） | 二者都叫「标定」，但解决的误差源不同。 |
| **模型 / model** | 控制：动力学模型 | 学习：神经网络 | 中文「模型」歧义极大，写文档时要写全。 |
| **仿真 / simulation** | 物理引擎里跑策略 | 离线编程/节拍仿真（工艺验证） | 两个圈子说「仿真」指的东西完全不同。 |
| **抓取 / grasp** | 抓起来不掉（force closure） | 抓起来 + 能完成后续装配位姿 | 产线要的是后者（task-oriented grasp）。 |
| **DOF** | 工业臂：参与末端位姿的独立轴 | 人形宣传：含手指的全部关节数 | 问「哪几个自由度参与末端位姿」。evidence: [T06-S001] |
| **负载 / payload** | 额定（指定重心与惯量下） | 口语「能扛多重」 | 问重心偏置与惯量。 |
| **端到端 / end-to-end** | 从像素到关节指令一个网络 | 从下单到出货的全流程（业务口径） | 制造业客户听到「端到端」想的可能是后者。 |

---

## I. 标准 — 术语与性能测试

> 格式：**标准号 版本** ｜ 类型 ｜ 发布 ｜ 生效/适用 ｜ 法域 ｜ 适用对象 ｜ 这一行怎么用它

### I1. ISO 8373:2021 — Robotics — Vocabulary（机器人 词汇）
- 版本/发布：第 3 版，**2021-11 发布**；取代 ISO 8373:2012。法域：国际（自愿采用，被各国等同转化）。适用对象：所有 ISO 机器人文件的术语基准。evidence: [T06-S001]
- 用法：`robot`、`industrial robot`、`service robot`、`medical robot`、`autonomy`、`control system`、`degree of freedom`、`workspace` 等的官方定义都在这里。写标书、写安规文件、跟客户对术语时以它为准。
- 现实：**中文圈日常不查它**，但一旦进入合规文件、投标澄清、事故责任讨论，对方会直接引 8373 的定义。「服务机器人」「工业机器人」的分类争议（例如人形机器人算哪一类）最后都会回到这份词汇表。
- Decay：low（词汇标准迭代约 8-10 年）。

### I2. ISO 9283:1998 — Manipulating industrial robots — Performance criteria and related test methods
- 版本/发布：**1998 发布**，至今现行（已 20+ 年未大改）。法域：国际。适用对象：工业机械手（manipulating industrial robot）。evidence: [T06-S006]
- 覆盖指标（转述）：位姿准确度与重复性、多方向位姿准确度变动、距离准确度与重复性、位置稳定时间、位置超调、位姿特性漂移、互换性、轨迹准确度与重复性、再定向轨迹准确度、拐角偏差、轨迹速度特性、最小定位时间、静态柔顺度、摆动偏差。evidence: [T06-S006]
- 测法要点（转述）：在工作空间中最大内接立方体（俗称 **ISO 测试立方体**）的规定平面上取 5 个位姿，每个位姿重复 30 次；重复性以到质心的平均距离 + 3σ 表示。evidence: [T06-S006, T06-S089]
- `_tell` 厂商样本上「重复定位精度 ±0.02 mm」如果不注明按 ISO 9283 在额定负载与额定速度下测得，就只是市场数字。
- Decay：low，但**注意它没有覆盖协作臂拖动示教、力控精度、移动机器人定位精度**——这些没有等价的老标准可用。

### I3. GB/T 12642-2013 — 工业机器人 性能规范及其试验方法
- 版本/发布：**2013-11-12 发布，2014-03-15 实施**；代替 GB/T 12642-2001。类型：推荐性国家标准（GB/T）。法域：中国。**等同采用 ISO 9283:1998**。归口：全国机器人标准化技术委员会（TC591）。evidence: [T06-S048, T06-S053]
- 用法：国内客户验收、第三方检测机构出报告时的中文依据。跟外资客户对话用 ISO 9283，跟国内客户/检测院对话用 GB/T 12642，**两者内容一致**。
- Decay：medium — 与 ISO 9283 绑定，ISO 侧一旦修订会带动 GB 修订。

### I4. GB/T 20868-2024 — 工业机器人 性能试验应用规范
- 版本：**2024 版**（替代其早期版本）。类型：推荐性国标。法域：中国。适用对象：工业机器人性能试验的实施方法与选取。evidence: [T06-S054]
- 用法：GB/T 12642 定义「测什么」，这一份偏「实际怎么选取试验项与条件」。国内检测报告常两份一起引。
- Decay：low-medium（刚改版）。

### I5. ISO 18646 系列 — 服务机器人性能准则与试验方法
- 已发布分部（举例）：**ISO 18646-1:2016**（轮式机器人的移动性能）、**ISO 18646-2:2024**（导航；取代 2019 版）、**ISO 18646-4:2021**（腰背支撑机器人）。系列仍在扩展，另有在研分部（如面向人周围移动、电动汽车充电机器人）。法域：国际。适用对象：服务机器人。evidence: [T06-S013, T06-S014]
- 用法：AMR / 服务机器人报「导航精度」时，正规做法是引 18646-2 的测法而不是自定义。
- Decay：**medium-high** — 系列在活跃扩张，新分部会持续出现。

---

## J. 标准 — 安全与功能安全

> 机械安全的标准是分层的：**A 类（基础，ISO 12100）→ B 类（通用安全，ISO 13849 / IEC 62061 / IEC 60204-1）→ C 类（具体机器，ISO 10218 / ISO 3691-4 / ISO 13482）**。C 类优先于 B、A。这套分层是这一行安全对话的骨架，说不出来就外行。

### J1. ISO 12100:2010 — 机械安全 设计通则 风险评估与风险减小（A 类）
- 版本/发布：**2010 发布**，现行。法域：国际（EN ISO 12100 在欧盟为协调标准）。适用对象：所有机械。evidence: [T06-S007]
- 用法：**风险评估的方法论母标准**——识别限制、识别危险、风险评价、三步法风险减小（本质安全设计 → 安全防护与补充措施 → 使用信息）。任何机器人项目的安全文件第一页都从它开始。
- `_tell` 说「我们做了安全评估」但拿不出按 ISO 12100 结构写的风险评估文件（危险清单 + 风险等级 + 措施 + 剩余风险）。
- Decay：low（16 年未改，但修订讨论一直存在）。

### J2. ISO 10218-1:2025 — Robotics — Safety requirements — Part 1: Industrial robots
- 版本/发布：**第 2 版，2025 年发布**（发布月份存在两说：ANSI Blog 记为 2025-02；A3 与 The Robot Report 侧记为 10218-1 与 -2 于 2025 年 1 月联合发布 —— 相差约一个月，本文件不武断取舍，正式文件请以 ISO 目录页为准）。取代 ISO 10218-1:2011。法域：国际。适用对象：**机器人本体制造商**（robot as partly completed machinery，未完整机械）。evidence: [T06-S002, T06-S032, T06-S086]
- 关键变化（相对 2011，转述）：把协作应用相关要求从 ISO/TS 15066 并入 10218 系列；引入机器人分类（按预期用途/复杂度）；更新功能安全表述与安全相关控制系统要求；扩充了对软件、网络安全与验证的要求。evidence: [T06-S026, T06-S032]
- Decay：low（刚改版，未来 5 年稳定），但**采纳节奏是 high**：欧盟协调标准清单、各国等同转化、客户合同引用会在 12-36 个月内滚动更新。

### J3. ISO 10218-2:2025 — Part 2: Industrial robot applications and robot cells
- 版本/发布：**第 2 版，2025 年发布**；取代 ISO 10218-2:2011。法域：国际。适用对象：**集成商与用户**（机器人应用、机器人单元的集成、调试、运行、维护、报废）。evidence: [T06-S003, T06-S005]
- 【原文】ISO 目录页对本版说明包含：*"Where appropriate, ISO/TS 15066:2016 on the safety of collaborative robot applications was added to the ISO 10218 series. Because human-robot collaboration relates to the application and not to the robot alone, most of the requirements of ISO/TS 15066 have been incorporated into this document."* evidence: [T06-S003]
- 这句话的工程含义：**「协作」是应用属性，不是产品属性**。买一台标称协作的机器人不等于你的单元是协作应用；力/压强限值要在**具体应用**上验证。
- Decay：low（内容），medium（引用与协调状态）。

### J4. ISO/TS 15066:2016 — Robots and robotic devices — Collaborative robots
- 版本/发布：**技术规范（TS），2016 发布**。法域：国际。适用对象：协作机器人应用。evidence: [T06-S004]
- 状态（重要）：其大部分要求已被并入 **ISO 10218-1:2025 / -2:2025**；行业实践中它作为独立文件的地位正在被取代。**在正式文件里现在应引 10218:2025，把 15066 作为历史依据。** evidence: [T06-S026, T06-S003]
- 它定义/普及的四种协作方式（转述，业内高频口语）：**安全额定监控停止（safety-rated monitored stop）、手动引导（hand guiding）、速度与距离监控（speed and separation monitoring, SSM）、功率与力限制（power and force limiting, PFL）**。这四个词至今是协作项目的通用语言。
- `_tell` 现在还把「15066 认证」挂在嘴上（本身就没有「15066 认证」这回事，TS 也不是可认证对象）。

### J5. ISO 13849-1:2023 — 机械安全 控制系统安全相关部件 第 1 部分：设计通则（PL）
- 版本/发布：**第 4 版，2023 发布**；取代 ISO 13849-1:2015。EN ISO 13849-1:2023 于 **2024-05** 在欧盟官方公报公布，过渡期至 **2027-05-15**（在此之前旧版仍可用于符合性推定）。法域：国际 / 欧盟协调标准。适用对象：机器安全相关控制系统（SRP/CS）。evidence: [T06-S008, T06-S009, T06-S090]
- 关键概念：**PL a–e**（性能等级）、类别 Cat. B/1/2/3/4、MTTFD、DC、CCF。`PLr`（required PL）来自风险评估，`PL`（achieved）来自设计计算。
- `_tell` 说「我们的机器人是 PLd 的」。PL 是**安全功能**的属性，不是整机的属性——正确说法是「急停功能达 PLd Cat.3」「安全限速功能达 PLd」。这是安全工程师一听就分得出内外行的地方。

### J6. IEC 62061:2021（+AMD1:2024 +AMD2:2026）— 机械安全 安全相关控制系统的功能安全（SIL）
- 版本/发布：**第 2 版 2021 发布**；修正案 AMD1:2024、AMD2:2026 已发布（IEC 提供合并版 CSV）。法域：国际。适用对象：机械的安全控制系统（SCS）。evidence: [T06-S018, T06-S019]
- 关系：它是 **IEC 61508 在机械行业的应用标准**；用 **SIL 1/2/3** 表达。与 ISO 13849 的对应关系业内常用：**PL c ≈ SIL 1、PL d ≈ SIL 2、PL e ≈ SIL 3**（这是工程惯用对照，不是逐项等价）。evidence: [T06-S090, T06-S098]
- `_tell` 把 SIL 4 用在机械/机器人上。SIL 4 属过程工业量级，机械安全领域实际到 SIL 3 为止。

### J7. IEC 61508:2010（Parts 1–7）— 电气/电子/可编程电子安全相关系统功能安全
- 版本/发布：**2010 版（第 2 版）**，现行；IEC 提供 1–7 部分合订注释版。法域：国际。适用对象：功能安全的**母标准**，其他行业标准（IEC 62061、IEC 61511、ISO 26262 等）都由它派生。evidence: [T06-S022, T06-S023, T06-S024]
- 用法：机器人公司自研安全控制器 / 安全 MCU 时会直接被要求按 61508 做认证（TÜV/Exida 等）。
- Decay：**high 提醒** — 61508 第 3 版的修订工作已进行多年，未来 12-24 个月内需复查状态。

### J8. IEC 60204-1:2016（+AMD1:2021）— 机械电气安全 第 1 部分：通用技术条件
- 版本/发布：**2016 发布**，AMD1 于 **2021** 发布，IEC 有合并版 CSV。法域：国际（EN 60204-1 在欧盟为协调标准）。适用对象：机械的电气设备与系统。evidence: [T06-S020, T06-S021]
- 用法：**停止类别 0/1/2 的定义出自这里**；急停、电源切断（隔离）、导线颜色、PE 连接、接线标识都按它做。工厂验收挑毛病最多的一份。
- `_tell` 把「急停」和「安全停止」混说；把 STO 当成急停的替代（STO 是驱动器安全子功能，急停是整机功能要求）。

### J9. ISO 3691-4:2023 — 工业车辆 安全要求与验证 第 4 部分：无人驾驶工业车辆及其系统
- 版本/发布：**2023 发布**，取代 ISO 3691-4:2020。法域：国际（EN ISO 3691-4 在欧盟为协调标准）。适用对象：AGV / **AMR** / 自动导引小车 / 牵引车等无人驾驶工业车辆及其系统与运行区域。evidence: [T06-S010, T06-S011, T06-S034]
- 关键点：明确了**制造商、集成商、用户的责任划分**；对运行区域、人员安全距离、防护装置、速度与制动距离有要求。
- `_tell` 用「AMR 不是 AGV，所以 3691-4 不适用」。标准的适用对象按功能而非营销分类，**AMR 明确在其例举范围内**。evidence: [T06-S034]
- 状态提醒：已有 **prEN ISO 3691-4 / ISO/DIS 3691-4** 在修订流程中——这是未来 12-24 个月的变化点。evidence: [T06-S010]

### J10. ISO 13482:2014 — 个人护理机器人安全要求（+ 修订中的 ISO/DIS 13482）
- 版本/发布：**2014 发布**，现行。法域：国际。适用对象：移动仆从机器人、体力辅助机器人、载人机器人；**明确排除玩具机器人与医疗机器人**。evidence: [T06-S012]
- 状态：**正在修订，已到 DIS 阶段**，修订后的范围拟扩展为「服务机器人安全要求」。这是人形机器人进家庭场景最相关的一条国际标准线，**未来 12-24 个月会变**。evidence: [T06-S012]
- `_tell` 拿 ISO 10218（工业）去套家用/服务机器人。两者是不同 C 类标准，适用对象不同。

### J11. ANSI/A3 R15.06-2025（Parts 1/2/3）— 美国工业机器人安全国家标准
- 版本/发布：Part 1 与 Part 2 于 **2025-08-21 批准**，Part 3 于 **2025-10-07 批准**，三部分完整版于 **2025-10-29 发布**。取代 ANSI/RIA R15.06-2012（近 15 年来首次大改）。法域：美国（并与加拿大专家协同开发 Part 3）。evidence: [T06-S025, T06-S033, T06-S087]
- 结构：**Part 1 / Part 2 = ISO 10218-1:2025 / -2:2025 的美国国家采标；Part 3 = 美国自行开发的新增部分（面向用户侧）**。evidence: [T06-S025, T06-S033]
- `_tell` 在美国项目上只说「我们符合 ISO 10218」而不提 R15.06 版本；或仍引用 R15.06-2012。

### J12. ANSI/RIA R15.08 系列 — 工业移动机器人（IMR）安全
- **R15.08-1-2020**：面向 IMR 本体制造商，**2020 发布**。**R15.08-2-2023**：面向 IMR 系统与应用（集成商），**2023 发布**。**Part 3**：面向用户与车队运营，处于制定/发布推进中。法域：美国。evidence: [T06-S027, T06-S028, T06-S029]
- 与 ISO 3691-4 的关系：**同一类设备，两套体系**——北美项目看 R15.08，欧盟项目看 EN ISO 3691-4。中国出口企业两边都要做。
- `_tell` 认为「移动机器人没有标准」。这是 2019 年前的旧印象。

### J13. ANSI/CAN/UL 3300:2024 — 服务、通信、信息、教育与娱乐机器人（SCIEE Robots）
- 版本/发布：**ANSI/CAN/UL 3300:2024**，ANSI Webstore 记录的发布日期为 **2025-04-16**；此前经历过 Outline of Investigation 阶段（UL 3300 Ed.3 于 2021-01 前后）。法域：美国 + 加拿大（双国家标准）。适用对象：消费级/商用服务机器人、教育与娱乐机器人。evidence: [T06-S030, T06-S031]
- 用法：**服务机器人进北美零售/商用渠道的实际门槛**（配合 NRTL 认证）。跟工业侧的 R15.06 完全是两条线。
- `_tell` 拿工业安规去谈家用/商用服务机器人的北美准入。

### J14. IEC 61800-5-2 族的驱动安全子功能（STO / SS1 / SLS / SLP 等）
- 类型：驱动器层面的安全功能定义（可调速电气传动系统安全）。适用对象：伺服驱动器与其安全子功能。evidence: [T06-S090]
- 用法：机器人的「安全限速」「安全限位」「安全转矩关断」最终要落到驱动器的这些子功能上，并纳入 ISO 13849/IEC 62061 的 PL/SIL 计算。
- `_tell` 在方案里写「软件限速」当安全措施。安全限速必须是安全通道实现且可验证。

---

## K. 法规与标准 — 欧盟

### K1. Regulation (EU) 2023/1230 — 机械法规（Machinery Regulation）
- 类型：欧盟**法规**（regulation，直接适用，无需成员国转化）。通过日 **2023-06-14**；**2023-07-19 生效**（OJ 公布后 20 天）；**自 2027-01-20 起适用**，届时取代机械指令 2006/42/EC。法域：欧盟。适用对象：机械、可更换设备、安全部件、链条绳索带、可拆卸传动装置、未完整机械（partly completed machinery）。evidence: [T06-S035, T06-S038, T06-S039]
- **状态必须说清**：现在（2026-09）**仍在过渡期**——投放欧盟市场的机器仍按机械指令 2006/42/EC 做 CE，2027-01-20 起按新法规。不要把它当成已经生效的现状。
- 相对旧指令的主要变化（转述）：法规形式统一适用；新增/强化对**软件更新、AI 相关安全功能、网络安全（防篡改）**的要求；数字化说明书（数字形式的使用说明允许，但纸质仍可要求）；调整了高风险机械清单与合格评定路径。evidence: [T06-S039, T06-S038]
- 对机器人行业的直接影响：机器人本体作为**未完整机械**出具「并入声明」（declaration of incorporation）+ 装配说明；集成后的机器人单元由集成商作为「机械」出 **EU 合格声明 + CE 标志**。这条责任链在新法规下没变，但文件与网络安全要求变多。

### K2. Regulation (EU) 2024/1689 — 人工智能法案（AI Act）
- 类型：欧盟法规。**2024-08-01 生效**。分阶段适用：禁止性做法与 AI 素养义务自 **2025-02-02**；通用人工智能模型（GPAI）提供者义务自 **2025-08-02**；高风险条款原定 Annex III 类自 2026-08-02、Annex I 嵌入式类自 2027-08-02。法域：欧盟。evidence: [T06-S037]
- 与机器人的交叉点：**当 AI 系统作为受欧盟产品法（含机械法规）约束产品的「安全部件」，或本身是这类产品时，被归为高风险**。也就是说，用神经网络实现避障/限速/人体检测这类安全功能，会直接触发高风险义务。

### K3. Regulation (EU) 2026/1744 — Digital Omnibus on AI（**改变了上面两条**）
- 类型：欧盟法规，日期 **2026-07-08**；**OJ 公布 2026-07-24**；**2026-07-27 生效**。它修订了 (EU) 2024/1689（AI Act）、(EU) 2018/1139（EASA）与 **(EU) 2023/1230（机械法规）**。evidence: [T06-S036, T06-S088]
- 关键改动 1（延期）：**Annex III 独立高风险 AI 系统的适用推迟到 2027-12-02；作为 Annex I 产品安全部件的嵌入式高风险 AI 推迟到 2028-08-02**（原为 2027-08-02）。evidence: [T06-S036, T06-S088]
- 关键改动 2（换归口，对机器人最重要）：机械法规从 AI Act 附件 I 的 A 节移到 B 节，**面向机械的高风险 AI 技术要求将通过委托法案并入机械法规本身**，制造商不必为同一个安全部件做两次合格评定。委托法案的期限指向 **2028-08-02**。evidence: [T06-S088]
- 【原文·转述来源】Eurogip 引述该法规意图为：*"a single manufacturer will not have to conduct a separate conformity assessment under the AI Regulation for its safety component…and then another conformity assessment under the Machinery Regulation."* evidence: [T06-S088]
- **合规叙事必须更新**：2025 年写的「AI Act 2026 年 8 月就要合规」的材料现在是错的。这是 Track 06 里时效性最强的一条。

### K4. Directive 2006/42/EC — 机械指令（现行、将被取代）
- 类型：欧盟指令（需成员国转化）。现行有效直到 **2027-01-20**。法域：欧盟。evidence: [T06-S035, T06-S039]
- 用法：**今天出口欧盟的机器人单元仍按它做 CE**。EN ISO 10218-1/-2、EN ISO 13849-1、EN 60204-1、EN ISO 3691-4 等协调标准提供符合性推定。

### K5. CE 标志与合格评定路径（EU）
- 机制：自我声明为主 + 特定高风险机械需公告机构（Notified Body）介入。公告机构在 **NANDO 数据库**可查。evidence: [T06-S099]
- 关键文件链：风险评估（ISO 12100）→ 技术文件 → 协调标准符合性 → EU 合格声明 → CE 标志 → 使用说明书。**未完整机械出「并入声明」，不加 CE**（除非同时受其他指令约束）。evidence: [T06-S035, T06-S039]
- `_tell` 说「我们的机器人有 CE 认证」。CE **不是认证**，是制造商的符合性声明；说「CE 认证」在欧洲客户面前会掉分（除非确实走了公告机构的证书路径，那也应说「NB 证书」）。

---

## L. 法规与标准 — 美国

### L1. OSHA：没有机器人专用强制标准
- 事实：美国 OSHA **没有针对工业机器人的专门联邦标准**。执法依据是通用条款 + 通用机械防护条款，并把 ANSI/RIA R15.06 等共识标准作为「行业公认良好实践」引用。evidence: [T06-S040, T06-S093, T06-S094]
- 一般责任条款（OSH Act Section 5(a)(1)）：雇主须提供无已知致命/严重伤害危险的工作场所。机器人伤害事故通常按此条款开罚。evidence: [T06-S094]
- 29 CFR 1910.212（机械通用防护要求）：机械运动部件须有防护。evidence: [T06-S093]
- `_tell` 说「美国没有机器人法规所以随便做」。OSHA 用一般责任条款 + 共识标准照样能开罚单，且事故后会直接引用 R15.06。

### L2. OSHA Technical Manual (OTM) — Section IV, Chapter 4：Industrial Robot Systems and Industrial Robot System Safety
- 类型：OSHA 内部检查用技术手册章节（对 CSHO 检查员的指引，非强制标准）。**近年更新过**（OSHA 在 TED-01-00-015 系列指令中记录了该章的更新）。法域：美国。适用对象：检查员与雇主。evidence: [T06-S040, T06-S041]
- 用法：它实际上是**「OSHA 检查员会怎么看你的机器人单元」的说明书**——风险评估、防护方式、常见伤害情景。做美国项目的安全方案前应通读。

### L3. NRTL 认证（UL / ETL 等）
- 机制：美国职业安全场景要求电气设备经 OSHA 认可的 NRTL（Nationally Recognized Testing Laboratory）认证。**这跟 CE 的自我声明模式根本不同**——美国是第三方发证。evidence: [T06-S031]
- 与机器人相关的具体标准：工业侧看 UL 1740 / NFPA 79 体系与 R15.06；服务/消费侧看 ANSI/CAN/UL 3300:2024。evidence: [T06-S030, T06-S031]
- `_tell` 把 CE 与 UL 当成「两个地方的同一件事」。CE 自我声明 vs NRTL 第三方发证，成本、周期、责任主体完全不同。

### L4. 美国：AI 相关的联邦统一立法暂缺
- 现状：截至 2026-09，美国**没有与欧盟 AI Act 对等的联邦统一 AI 法规**；机器人 AI 的合规主要落在产品安全（NRTL / 共识标准）与侵权责任上，各州法规另有差异。
- 使用建议：跟美国客户谈 AI 安全时，**引 ISO 10218:2025 / R15.06-2025 与风险评估文件比引 AI 治理框架更有说服力**。

---

## M. 标准与政策 — 中国

### M1. GB 11291.1-2011 — 工业环境用机器人 安全要求 第 1 部分：机器人
- 类型：**强制性国家标准（GB）**。**2011-05-12 发布，2011-10-01 实施**，状态：现行。代替 GB 11291-1997。**等同采用 ISO 10218-1:2006 及其 Cor.1:2007**。法域：中国。适用对象：工业机器人本体。归口：工信部 / TC591。evidence: [T06-S046]
- **重要时效判断**：它对标的是 **ISO 10218-1:2006**，而国际侧已走到 **2025 版**。也就是说中国强制性国标与国际最新版之间存在**两代差**。做出口的企业实际上以 ISO/EN 版本为准，做国内合规以 GB 11291 为准。这是国内项目里最容易出错的一处。evidence: [T06-S046, T06-S002]

### M2. GB 11291.2-2013 — 机器人与机器人装备 工业机器人的安全要求 第 2 部分：机器人系统与集成
- 类型：强制性国家标准。**2013 发布**，状态：现行。对标 ISO 10218-2:2011。法域：中国。适用对象：机器人系统与集成（集成商侧）。evidence: [T06-S047]
- 用法：国内产线验收、安监检查、事故责任认定的中文依据。

### M3. GB/T 12642-2013 / GB/T 20868-2024 — 性能与试验
- 见 I3 / I4。evidence: [T06-S048, T06-S053, T06-S054]

### M4. 人形机器人国家标准 — TC591/SC5 与首批立项
- 机构：**全国机器人标准化技术委员会人形机器人分技术委员会（TC591/SC5）**，业务范围覆盖人形机器人的基础共性、安全与伦理、零部件、整机、应用与集成；由中国机械工业联合会组建与业务指导，秘书处设在北京机械工业自动化研究所。evidence: [T06-S044, T06-S045]
- 进度（**状态要写准**）：**2024-09** 工信部公示人形机器人标委会筹建方案 → **2025-04** 首批人形机器人系列国家标准正式立项 → **2026-06** 首批人形机器人国家标准进入审定阶段。审定涉及的技术要求系列覆盖总则、环境感知、决策规划、运动控制、操作任务、仿真测试平台等分部。**截至 2026-09，这批标准处于「已立项 / 审定中」，不是「已发布实施」。** evidence: [T06-S050, T06-S049, T06-S051, T06-S052]
- `_tell` 说「人形机器人国标已经出了」。目前正确说法是「首批国标已立项、部分进入审定」。

### M5. 工信部人形机器人与具身智能标准化技术委员会 + 《人形机器人与具身智能标准体系（2026 版）》
- 机构：**2025-12-26 在北京成立**（工信部行业标委会，秘书处设在中国电子学会）。承担人形机器人与具身智能领域**行业标准**的制修订。evidence: [T06-S091]
- 文件：**《人形机器人与具身智能标准体系（2026 版）》于 2026-02-28 在北京发布**，由 120 余家单位编制，分为**基础共性、类脑与智算、肢体与部组件、整机与系统、应用、安全伦理** 6 个部分。这是国内首个覆盖该产业链全生命周期的标准顶层设计。**注意：这是「标准体系」（规划性文件），不是可直接引用的技术标准。** evidence: [T06-S092]
- 两个委员会的分工：**TC591/SC5 归口国家标准（GB/GB/T），工信部标委会归口行业标准**。谈标准时要分清是哪一层。evidence: [T06-S044, T06-S091]

### M6. 《人形机器人创新发展指导意见》（工信部科〔2023〕193 号）
- 类型：部委政策文件（指导意见，非强制标准）。**印发日期 2023-10-20**，工信部官网发布日 2023-11-02。法域：中国。适用对象：地方工信主管部门、行业协会、企事业单位。evidence: [T06-S042]
- 内容（转述）：以大模型等 AI 技术突破为引领，在人形机器人「**大脑**」「**小脑**」「**肢体**」关键技术与技术创新体系上取得突破；提出到 2025 年创新体系初步建立、关键技术突破、在特种/制造/民生服务场景示范应用，并给出面向 2027 年的进一步目标。evidence: [T06-S042]
- **「大脑 / 小脑 / 肢体」这组词的来源就是这份文件**，它已成为中国政策与产业语境的通用分层说法（大脑≈任务理解与规划、小脑≈运动控制、肢体≈本体与部组件）。跟中国政府/产业方沟通时用这套词非常有效；在国际学术语境里没人这么说。

### M7. 《"机器人+"应用行动实施方案》（工信部联通装〔2022〕187 号）
- 类型：十七部门联合政策文件。**2023-01-18 印发**（中国政府网 2023-01-19 公开）。法域：中国。evidence: [T06-S043]
- 目标（转述）：到 2025 年**制造业机器人密度较 2020 年实现翻番**，服务/特种机器人行业应用深度与广度显著提升；聚焦制造业、农业、建筑、能源、商贸物流、医疗健康、养老服务、教育、安全应急与极限环境、商业社区服务**十大应用领域**。evidence: [T06-S043]
- 用法：国内立项、申报、招投标写背景时的标准引用；「机器人密度」的口径与 IFR 一致。evidence: [T06-S083]

### M8. 国家职业技能标准 — 工业机器人系统操作员 / 系统运维员（2020 年版）
- 类型：人力资源社会保障部 + 工业和信息化部联合颁布的国家职业技能标准。**2020 年发布施行**（操作员标准的通知为人社厅发〔2020〕108 号）。职业编码：工业机器人系统运维员 6-31-01-10。分四级：四级/中级工、三级/高级工、二级/技师、一级/高级技师。法域：中国。evidence: [T06-S096, T06-S097]
- 用法：国内是**唯一成体系的人员资质**（对应职业技能等级认定），产线运维岗招聘与职称评定会用。研发岗没有对应资质。

### M9. 未能核实、故不收录的项
- 本轮检索**未能在 std.samr.gov.cn / 国家数字标准馆确认「GB/T 39004」对应服务机器人标准**（检索命中的是 GB/T 38834 系列、GB/T 40013 等其他编号）。为避免造假，本文件不收录该编号，服务机器人国标应以 TC591 归口目录现场检索为准。
- 中国**没有针对工业机器人的 CCC 强制性产品认证目录条目**这一点，本轮亦未取得可直接引用的一手确认；涉及国内准入时应按项目实际以市场监管总局目录核对，不要在方案里断言。

---

## N. 认证、资质与合格评定

> 这一行的「认证」分四类：**产品合规**、**功能安全**、**企业/团队**、**个人**。中文圈普遍把它们混为一谈。

### N1. 产品合规（地区准入）
| 地区 | 机制 | 关键标准 | 责任主体 | evidence |
|---|---|---|---|---|
| 欧盟 | CE 标志（自我声明为主，高风险机械需公告机构 NB） | EN ISO 10218-1/-2、EN ISO 13849-1、EN 60204-1、EN ISO 3691-4 | 制造商/集成商 | [T06-S035, T06-S039, T06-S099] |
| 美国 | NRTL 第三方认证 + OSHA 执法 | R15.06-2025、R15.08 系列、UL 3300、NFPA 79 | 制造商 + 雇主 | [T06-S025, T06-S030, T06-S040] |
| 中国 | 强制性国标符合 + 项目验收 | GB 11291.1/.2、GB/T 12642 | 制造商/集成商/用户 | [T06-S046, T06-S047, T06-S048] |
- `_tell` 说「CE 认证」「我们有 CE 证书」。除非确实是 NB 出具的证书，否则应说「CE 符合性声明」。

### N2. 功能安全认证（PL / SIL）
- 对象：**安全功能**与实现它的部件/子系统（安全控制器、安全 I/O、驱动器安全子功能、安全软件）。由第三方（TÜV、Exida 等）依 ISO 13849-1 / IEC 62061 / IEC 61508 出证。evidence: [T06-S098, T06-S090, T06-S022]
- 正确说法示例：「本机器人的安全额定监控停止功能达 PLd Cat.3，由 XX 认证」，而不是「本机器人是 SIL2 的」。

### N3. 企业 / 团队级认证
- **A3 Certified Robot Integrator（美国）**：2012 年设立，含现场审核、关键人员实操评估、安全培训等，**有效期 2 年需复审**。北美大型集成合同的常见门槛。evidence: [T06-S095]
- **ISO 9001（质量管理体系）**：几乎所有向汽车/3C 供货的机器人企业都需要；汽车链条上还要 IATF 16949。evidence: [T06-S100]
- 中国无对等的「机器人集成商国家级认证」，实践中以行业协会资质 + 客户合格供应商审核代替。

### N4. 个人资质
- 中国：**工业机器人系统操作员 / 系统运维员**国家职业技能标准（2020 年版），四个等级。evidence: [T06-S096]
- 国际：无统一的「机器人工程师」执业资格；功能安全领域有 TÜV 系列的功能安全工程师（FS Eng./FSE）证书，是安全岗的实际通行证。evidence: [T06-S098]
- **N/A 说明**：机器人研发岗（控制、感知、学习）在全球范围内**没有执业资格制度**，靠论文、开源、项目履历。这一格是本行业的真实空白，不是本轮调研的遗漏。

---

## O. 外行破绽（`_tell`）

> 「一出口就暴露不是这行的人」。每条格式：**外行怎么说 → 这行人怎么说 → 为什么**。
> 标注 `_tell` 便于 Phase 2.5 表达 DNA 汇总。频率标记：★★★ = 几乎每次外部会议都出现。

1. `_tell` ★★★ **「这台机器人精度 0.02 毫米」** → 「重复定位精度 ±0.02 mm，绝对精度是毫米级；按 ISO 9283 在什么负载和速度下测的？」 → 因为 ISO 9283 / GB/T 12642 把 accuracy 与 repeatability 定义为两个量，规格书标的几乎总是后者，二者可差一到两个数量级。evidence: [T06-S006, T06-S048]

2. `_tell` ★★★ **「成功率 90%」（不给分母）** → 「N=50 次，物体位置在 30×30 cm 内均匀随机，判定为完整放入托盘，不允许重试，无人干预」 → 不给试验次数、初始状态分布、判定标准和重试规则的成功率无法比较，等于没说。

3. `_tell` ★★★ **「我们的系统是实时的，延迟只有几毫秒」** → 「伺服环 1 kHz，最坏情况抖动 < 50 μs（p99.99）」 → 硬实时讲的是延迟上界与抖动，不是平均值；报平均延迟说明没做过实时系统。evidence: [T06-S072]

4. `_tell` ★★★ **「这个模型泛化能力很强」** → 「在新物体上能，新场景光照变化下掉 20%，新任务没试过，新本体不行」 → 泛化必须按新物体/新场景/新任务/新本体四层分开说。evidence: [T06-S060]

5. `_tell` ★★★ **「协作机器人天生安全，不用围栏」** → 「协作是应用属性，要按 ISO 10218-2:2025（原 TS 15066）在**这个具体应用**上做风险评估并实测力/压强限值；装上刀具或高速搬运就不再是协作应用」 → 标准明确把协作归到 application 而非 robot。evidence: [T06-S003, T06-S026]

6. `_tell` ★★ **「我们的机器人有 CE 认证」** → 「我们出具了 EU 合格声明并加贴 CE 标志」/「这部分由公告机构 NB 出证」 → CE 是自我声明制度，不是认证；对欧洲客户说「CE 认证」立刻掉分。evidence: [T06-S035, T06-S099]

7. `_tell` ★★ **「这台机器人是 PLd 的 / SIL2 的」** → 「急停功能达 PLd Cat.3、安全限速功能达 PLd」 → PL/SIL 是**安全功能**的属性，不是整机属性。evidence: [T06-S008, T06-S018]

8. `_tell` ★★ **「20 kg 负载，我这个 15 kg 的件肯定没问题」** → 「重心离法兰多远？转动惯量多少？要跑多快？」 → 额定负载是在指定重心与惯量下的值，外伸后可用负载会大幅下降。

9. `_tell` ★★ **「加个力传感器就能做力控」** → 「关节可反驱吗？力控带宽多少 Hz？是关节力矩还是腕部六维力？」 → 不可反驱的高减速比关节即使测到力也来不及退让。

10. `_tell` ★★ **「仿真里成功率 95%」** → 「真机 N 次里成功多少？sim2real 掉了多少？」 → 仿真数在这一行不作为能力证据，接触与执行器动力学是最大的 gap 来源。evidence: [T06-S064]

11. `_tell` ★★ **「我们用 ROS 2，所以是实时的」** → 「实时性来自 PREEMPT_RT 内核 + CPU 隔离 + DDS 配置，伺服环不在 ROS 里跑」 → ROS 2 是中间件，不提供实时保证。evidence: [T06-S067, T06-S072]

12. `_tell` ★★ **「7 轴比 6 轴精度高」** → 「7 轴的价值是冗余：避奇异、避障、避关节限位，不是精度」 → 冗余与精度是两个维度。

13. `_tell` ★★ **「节拍 3 秒」（其实说的是循环时间）** → 「循环时间 3 秒，客户节拍 4.2 秒，所以有 30% 余量」 → 节拍是需求侧配额，循环时间是实际耗时；混用会算错产能。

14. `_tell` ★★ **「AMR 不是 AGV，所以 ISO 3691-4 不管我们」** → 「ISO 3691-4:2023 的适用对象按功能列举，AMR 明确在内」 → 营销分类不改变标准适用范围。evidence: [T06-S034, T06-S010]

15. `_tell` ★★ **「我们采了 10 万条轨迹」** → 「多少个任务、多少个场景、多少个物体、几个采集员、成功轨迹占比多少、平均时长多少」 → 遥操作数据的价值由多样性和一致性决定，不是条数。

16. `_tell` ★ **「机器人在这个位置会卡住/报警，是设备坏了」** → 「这条轨迹过奇异了，改姿态或用零空间绕开」 → 奇异是运动学固有现象，不是故障。

17. `_tell` ★ **「阻抗控制和导纳控制差不多」** → 「阻抗是位置进力出、适合可反驱本体；导纳是力进位置出、套在位置控机器人外面，硬接触时容易不稳」 → 这是控制岗面试的分水岭问题。

18. `_tell` ★ **「ZMP 就是平衡算法」** → 「ZMP 是不翻倒的判据；能不能被推倒后迈步恢复要看落脚点重规划（capture point / MPC）」 → 判据与方法混为一谈。

19. `_tell` ★ **「装了实时内核就实时了」** → 「还要 isolcpus、关 CPU 频率调节与深度 C-state、锁页内存、去掉热路径上的动态分配和日志」 → 实时是系统工程，不是装补丁。evidence: [T06-S072]

20. `_tell` ★ **「谐波减速器零背隙所以精度高」** → 「谐波的问题不是背隙，是柔轮扭转柔度和迟滞，负载一变位置就偏，所以要加关节侧编码器」 → 混淆背隙与刚度/迟滞。evidence: [T06-S074]

21. `_tell` ★ **「我们做了数字孪生」（其实是离线编程仿真）** → 「这是离线编程/节拍仿真；数字孪生要与真机数据同步」 → 中文产业语境里这个词被泛用到失去含义。

22. `_tell` ★ **「15066 认证」** → 「ISO/TS 15066 是技术规范，本身不可认证，且其内容已并入 ISO 10218:2025」 → 说这句话说明合规知识停留在 2016-2024 年。evidence: [T06-S004, T06-S026]

23. `_tell` ★ **「AI Act 2026 年 8 月就要合规了」** → 「Digital Omnibus (EU) 2026/1744 已把 Annex III 推到 2027-12-02、Annex I 嵌入式推到 2028-08-02，并把机械类 AI 要求归到机械法规下」 → 这是 2026 年最新的时效差。evidence: [T06-S036, T06-S088]

24. `_tell` ★ **「机械法规 2023/1230 已经生效了，现在就按它做」** → 「它 2023-07-19 生效但 **2027-01-20 才适用**；今天出口欧盟仍按 2006/42/EC 做 CE」 → 生效日与适用日在欧盟法里是两个概念，混淆会导致合规方案排期错一年半。evidence: [T06-S035, T06-S038]

25. `_tell` ★ **「人形机器人国标已经发布了」** → 「首批人形机器人系列国标 2025-04 立项、2026-06 进入审定，尚未发布实施；另有工信部标委会 2026-02-28 发布的是《标准体系（2026 版）》这一顶层规划文件」 → 立项/审定/发布是三个状态。evidence: [T06-S049, T06-S052, T06-S092]

26. `_tell` ★ **「我们的机器人 MTBF 5 万小时，所以产线可用率很高」** → 「本体 MTBF 好，系统故障主要来自末端工装、视觉、上下料和线缆」 → 用部件指标推系统指标。

---

## P. 厂商话术与营销词

> 每条：**营销里的意思 → 工程实质 → 追问什么**。这些词本身不都是坏词，问题在于发布会含义与论文/工程含义差得远。

| 营销词 | 发布会里的意思 | 工程实质 | 内行的追问 |
|---|---|---|---|
| **具身智能 / Embodied AI** | 「机器人有了智能」，一个融资叙事标签 | 一个研究方向的统称（策略需要与物理世界闭环）；不指任何具体能力 | 具体到哪一层：VLA 端到端？分层 VLM + 传统控制？还是脚本 + 视觉？ |
| **通用机器人 / General-purpose robot** | 一台什么都能干的机器 | 目前指「同一套硬件 + 同一个策略骨干可覆盖多任务，且每个任务仍需数据/微调」 | 覆盖多少任务？换任务要多少数据、多少小时？谁来采？ |
| **全自主 / Fully autonomous** | 完全无人 | 通常是「有远程兜底，干预率 X 次/小时」 | 干预率多少？谁在兜底？兜底的人机比是多少？ |
| **零样本泛化 / Zero-shot** | 没见过也能做 | 通常是「这个具体实例没见过，但同类见过很多」 | 训练集里同类样本有多少？评测集怎么切的？ |
| **AI 大脑 / 机器人大脑** | 一个会思考的大模型 | 政策语境里「大脑」= 任务理解与规划层（出自工信部指导意见的大脑/小脑/肢体分层）；厂商语境里常指一个 VLM | 是哪一层？输出频率多少？跟运动控制怎么接？evidence: [T06-S042] |
| **拟人化 / 类人** | 像人一样动作 | 通常只说明关节布局与外形接近人，不代表能力接近人 | 关节力矩密度、续航、负载、连续工作时长各是多少？ |
| **端到端** | 一个模型直通到底 | 从像素到关节指令一个网络；但绝大多数落地系统在底下仍有传统的限速、限力、避障与安全层 | 底层还有什么保护层？出问题时谁接管？ |
| **世界模型** | 机器人「理解」世界 | 学一个可预测未来观测/状态的模型，用于规划或数据生成 | 预测的是像素还是状态？时域多长？误差怎么评？ |
| **数字孪生** | 一个高保真虚拟工厂 | 与真机数据同步的模型；照 CAD 建的静态仿真不算 | 同步什么数据？多久同步一次？用来做什么决策？ |
| **协作机器人 = 安全** | 不用围栏、随便靠近 | 安全属于应用，需按 ISO 10218-2:2025 做风险评估并实测力/压强 | 做过风险评估吗？力/压强实测报告有吗？工具算进去了吗？evidence: [T06-S003] |
| **免编程 / 零代码** | 拖一拖就能用 | 图形化示教覆盖标准工序；异常处理、节拍优化、换型仍要工程师 | 换型要多久？异常恢复怎么做？谁维护？ |
| **柔性产线** | 什么产品都能做 | 在预定义的产品族内可切换 | 换型时间多少？首件合格要多久？新产品导入周期多长？ |
| **人形机器人已进厂/量产** | 已在工厂干活 | 多为试点工位、限定任务、有人陪同，产量口径常含订单与意向 | 几个工位？连续跑了多少小时？干预率？是交付量还是订单量？ |
| **智能柔顺 / 力控专利** | 独门技术 | 阻抗/导纳控制 + 力矩传感是公开方法 | 力控带宽多少 Hz？力分辨率多少 N？可反驱吗？ |
| **超越人类速度/精度** | 比人强 | 通常是单一维度的窄比较 | 在什么任务、什么容差、连续多长时间上比的？ |
| **具身大模型参数量 XXB** | 越大越强 | 参数量与真机成功率不单调相关，推理频率反而受限 | 推理频率多少 Hz？部署在什么算力上？功耗多少？ |

**这一行明确拒绝的说法**（拒绝本身就是行业价值观的体现）：
- 「视频里做到了」当作能力证据 —— 内行只认可重复试验的分母与干预率。
- 用仿真数字代替真机数字。
- 把安全说成产品属性而不是应用属性与流程属性。
- 用「AI 会自己学会」回避 reward 设计、数据采集、标定与验证的实际工作量。

---

## Q. 总览表

### Tier 1 — 核心必懂（35 个）

| 术语 | Type | Insider def（一句） | Outsider tell | Last_updated |
|---|---|---|---|---|
| 重复定位精度 / pose repeatability | term + standard | 多次到达同一指令位姿的离散度，ISO 9283 定义 | 说「精度」不分 accuracy / repeatability | 1998（ISO 9283） |
| 绝对精度 / pose accuracy | term + standard | 指令位姿与实到均值之差，通常毫米级 | 以为规格书的 ±0.02 mm 是绝对精度 | 1998 |
| TCP | acronym | 工具中心点，一切轨迹与精度的基准 | 以为是机器人自带固定点 | — |
| 负载 / payload | term | 指定重心与惯量下的额定负载 | 只比数字不问重心 | — |
| DOF / 自由度 | acronym | 参与末端位姿的独立可控轴数 | 把手指关节全算进去比 | ISO 8373:2021 |
| 奇异 / singularity | term | 雅可比降秩、末端某方向失控 | 当成设备故障 | — |
| IK / 逆运动学 | acronym | 多解，工程难点在构型连续性 | 以为「算一下就行」 | — |
| 阻抗控制 | term | 位置进力出，需可反驱 | 与导纳混用 | — |
| 导纳控制 | term | 力进位置出，套在位置控外面 | 与阻抗混用 | — |
| 硬实时 / jitter | term | 最坏延迟有确定上界 | 报平均延迟 | — |
| 伺服周期 | term | 分层：电流环 kHz、位置环 kHz、策略 10-50 Hz | 说「模型 30 Hz 所以机器人 30 Hz 控制」 | — |
| 手眼标定 | term | 求相机与法兰/基座的刚体变换 | 以为识别准 = 抓取准 | — |
| 6D 位姿 | term | 3 平移 + 3 旋转 | 说成「位置」 | — |
| SLAM | acronym | 同步定位与建图 | 当成「导航能力强」 | — |
| 行为克隆 / BC | term + acronym | 观测→动作的监督学习 | 与「模仿学习」混为一谈 | — |
| 协变量偏移 | term | 策略自走出分布，误差二次累积 | 「多采点数据就好」 | 2010（DAgger 论文） |
| Action chunking | term | 一次预测执行 k 步动作 | 以为只是「输出频率问题」 | 2023（ACT） |
| Diffusion policy | term | 用扩散建模多峰动作分布 | 「扩散是画图的」 | 2023 |
| VLA | acronym | 视觉-语言-动作端到端模型 | 把任何用大模型的机器人都叫 VLA | 2023（RT-2） |
| 跨本体 / cross-embodiment | term | 同一策略跨不同机器人形态 | 不区分跨相似形态与真跨形态 | 2023（OXE） |
| 域随机化 | term | 随机化仿真视觉/物理参数求鲁棒 | 「范围越大越好」 | 2017 |
| sim2real gap | term | 接触与执行器动力学是最大头 | 拿仿真数当能力证据 | — |
| 泛化（四层） | term | 新物体/新场景/新任务/新本体 | 只说「泛化好」 | — |
| 遥操作 / teleoperation | term | 主从采演示数据，力反馈决定质量 | 只报轨迹条数 | — |
| ROS 2 | standard-ish | 中间件，不是实时系统 | 「用 ROS 2 所以实时」 | — |
| QoS（DDS） | term | 收发端策略不兼容就静默连不上 | 先怀疑网络 | — |
| EtherCAT | standard | 微秒级实时总线 + 分布时钟 | 以为可随便接交换机 | — |
| PREEMPT_RT | term | 降低最坏调度延迟 | 「装了就实时」 | — |
| 循环时间 / cycle time | term | 完整作业循环耗时 | 只报单动作耗时 | — |
| 节拍 / takt time | term | 需求侧时间配额 | 与循环时间混用 | — |
| 成功率（分母） | term | 无分母不成立 | 报裸数字 | — |
| 干预率 | term | 每小时人类介入次数 | 只讲单次成功率 | — |
| ISO 10218-1/-2:2025 | standard | 工业机器人本体与应用安全 | 仍引 2011 版或谈「15066 认证」 | 2025 |
| PL / SIL | standard | 安全功能的性能等级 / 完整性等级 | 说「整机是 PLd」 | 2023 / 2021 |
| 风险评估（ISO 12100） | standard | 三步法风险减小的方法论母标准 | 「我们做了安全评估」但无文件 | 2010 |

### Tier 2 — 周边熟知（42 个）

| 术语 | Type | Insider def（一句） | Last_updated |
|---|---|---|---|
| Reach / 臂展 | term | 腕心可达最大距离，不含工具 | — |
| 灵巧工作空间 | term | 可任意姿态到达的子空间 | — |
| EOAT / 末端执行器 | acronym + term | 手爪与工装，常是项目瓶颈 | — |
| 谐波减速器 | term | 零背隙但有迟滞与扭转柔度 | — |
| RV / 摆线针轮 | term | 高刚度抗冲击，用于大臂 | — |
| 背隙 / backlash | term | 换向空程，吃掉双向重复性 | — |
| 可反驱 / backdrivability | term | 力控与安全接触的物理前提 | — |
| SEA | acronym | 串弹性元件测力矩，带宽换安全 | — |
| QDD / 准直驱 | acronym | 低减速比 + 大扭矩电机 | — |
| 力矩密度 | term | 要区分峰值与连续 | — |
| IP 等级 | standard | 防尘 + 防水两位数字 | — |
| 本体（两义） | term | 工业=硬件；学术=embodiment | — |
| 冗余 / 零空间 | term | 末端不动手肘能动 | — |
| ZMP | acronym | 不翻倒的判据 | — |
| 捕获点 / DCM | term | 一步止住的落脚点 | — |
| MPC | acronym | 滚动时域最优控制 | — |
| WBC | acronym | 优先级任务 QP，高频全身力矩 | — |
| 步态 / 支撑相摆动相 | term | 接触序列的时间安排 | — |
| 路径 vs 轨迹 | term | 几何 vs 带时间参数化 | — |
| 重力补偿 | term | 依赖准确的负载辨识 | — |
| 柔顺（被动/主动） | term | 机械弹性 vs 控制造出来的 | — |
| 内参 / 外参 | term | 会随温度振动漂，要复标 | — |
| ICP / 点云配准 | acronym | 需好初值，易陷局部极小 | — |
| VIO | acronym | 相机+IMU 紧耦合，无回环 | — |
| 回环检测 | term | 一次性压回累计误差 | — |
| 六维力 / F/T | term | 测工具端合力，不给接触点 | — |
| 触觉 / tactile | term | 给接触位置与滑移 | — |
| 结构光/ToF/双目 | term | 选型由物料表面决定 | — |
| 抓取位姿检测 | term | 输出候选集合，还需可达与碰撞筛选 | — |
| 重投影误差 | term | 标定质量判据，但会过拟合 | — |
| 状态估计 | term | 躯干位姿+速度+接触+零偏 | — |
| DAgger | acronym | 在策略访问的状态上标注 | 2010 |
| Teacher-student / 特权学习 | term | 蒸馏的是观测空间不是模型大小 | 2020 |
| 离线 RL | term | 难点在分布外动作价值高估 | — |
| 奖励塑形 | term | 足式 RL 的实际工作量大头 | — |
| 系统辨识 / sysid | term | 缩小 sim2real 性价比最高的一步 | — |
| 并行仿真 | term | GPU 上万环境，吞吐≠质量 | — |
| URDF / MJCF / USD | standard-ish | 模型描述格式，惯量最易写错 | — |
| CANopen / CiA 402 | standard | CAN 上的伺服驱动行规 | — |
| 停止类别 0/1/2 | standard | IEC 60204-1 定义 | 2016(+A1:2021) |
| STO / SS1 / SLS | acronym | 驱动器安全子功能 | — |
| MTBF / MTTR / OEE / FPY | acronym | 可靠性与产线效率口径 | — |

### Standards / Regulations 时间轴（近 5 年内有显著变化的才进表）

| 名称 | Issued | Applies / In force | 状态 | Decay | evidence |
|---|---|---|---|---|---|
| ISO 8373:2021 | 2021-11 | 现行 | 已发布 | low | [T06-S001] |
| ISO 10218-1:2025 | 2025（月份两说：2025-01 / 2025-02） | 现行 | 已发布，取代 2011 版 | low（内容）/ high（采纳节奏） | [T06-S002] |
| ISO 10218-2:2025 | 2025 | 现行 | 已发布，并入 TS 15066 主要内容 | low / high | [T06-S003, T06-S026] |
| ISO/TS 15066:2016 | 2016 | — | 内容已并入 10218:2025，正被取代 | high | [T06-S004, T06-S026] |
| ISO 13849-1:2023 | 2023 | EN 版 2024-05 列入 OJ；过渡期至 **2027-05-15** | 已发布，过渡中 | medium | [T06-S008, T06-S090] |
| IEC 62061:2021 +AMD1:2024 +AMD2:2026 | 2021 / 2024 / 2026 | 现行 | 已发布（含两个修正案） | medium | [T06-S018, T06-S019] |
| ISO 3691-4:2023 | 2023 | 现行 | 已发布；**ISO/DIS 3691-4 修订中** | high | [T06-S010] |
| ISO/DIS 13482 | DIS 阶段 | — | **修订中，未发布** | high | [T06-S012] |
| ISO 18646-2:2024 | 2024 | 现行 | 已发布，取代 2019 版 | medium-high | [T06-S014] |
| ANSI/A3 R15.06-2025 | P1/P2 批准 2025-08-21；P3 批准 2025-10-07；发布 2025-10-29 | 现行 | 已发布 | low / high（采纳） | [T06-S025] |
| ANSI/RIA R15.08-2-2023 | 2023 | 现行 | 已发布；Part 3 推进中 | medium | [T06-S028] |
| ANSI/CAN/UL 3300:2024 | 2024 版，ANSI 记录发布日 2025-04-16 | 现行 | 已发布 | medium | [T06-S030] |
| GB/T 20868-2024 | 2024 | 现行 | 已发布 | low | [T06-S054] |
| Regulation (EU) 2023/1230 机械法规 | 2023-06-14 通过，2023-07-19 生效 | **2027-01-20 起适用** | **已发布，尚未适用** | high | [T06-S035, T06-S038] |
| Regulation (EU) 2024/1689 AI Act | 2024-08-01 生效 | 分阶段（见 K2、K3） | 已发布，分阶段适用 | high | [T06-S037] |
| Regulation (EU) 2026/1744 Digital Omnibus on AI | 2026-07-08；OJ 2026-07-24 | **2026-07-27 生效** | 已发布并生效 | high | [T06-S036, T06-S088] |
| 人形机器人首批国家标准 | 2025-04 立项；2026-06 审定 | — | **立项/审定中，未发布** | high | [T06-S049, T06-S052] |
| 工信部人形机器人与具身智能标委会 | 2025-12-26 成立 | — | 已成立 | high | [T06-S091] |
| 《人形机器人与具身智能标准体系（2026 版）》 | 2026-02-28 发布 | — | 已发布（规划文件，非技术标准） | high | [T06-S092] |
| 《人形机器人创新发展指导意见》 | 2023-10-20 印发 | 现行 | 已发布 | medium | [T06-S042] |
| 《"机器人+"应用行动实施方案》 | 2023-01-18 印发 | 现行（目标年 2025） | 已发布，**目标年已过，后续文件待观察** | high | [T06-S043] |

（长期稳定、近 5 年无实质变化的不进本表：ISO 9283:1998、ISO 12100:2010、IEC 61508:2010、IEC 60204-1:2016、GB 11291.1-2011、GB 11291.2-2013、GB/T 12642-2013、ISO 13482:2014、2006/42/EC。）

### 行业「外行破绽」高亮

| 误用 | 内行实际意思 | 出现频率 |
|---|---|---|
| 「精度 0.02 mm」 | 重复定位精度，非绝对精度 | ★★★ |
| 「成功率 90%」无分母 | 需 N + 初始分布 + 判定 + 重试规则 | ★★★ |
| 「实时，延迟几毫秒」 | 硬实时看最坏值与抖动 | ★★★ |
| 「泛化能力强」 | 需分四层说 | ★★★ |
| 「协作机器人天生安全」 | 安全属于应用不属于产品 | ★★★ |
| 「CE 认证」 | CE 是自我声明 | ★★ |
| 「整机是 PLd」 | PL 属于安全功能 | ★★ |
| 「加个力传感器就能力控」 | 需可反驱与带宽 | ★★ |
| 「仿真成功率 95%」 | 真机数才算数 | ★★ |
| 「用 ROS 2 所以实时」 | ROS 2 不提供实时保证 | ★★ |
| 「节拍 3 秒」（指循环时间） | 节拍是需求配额 | ★★ |
| 「AMR 不适用 3691-4」 | 按功能列举，AMR 在内 | ★★ |
| 「15066 认证」 | TS 不可认证且已被并入 10218 | ★ |
| 「AI Act 2026-08 就要合规」 | 已被 2026/1744 推迟 | ★ |
| 「机械法规已经生效所以现在按它做」 | 2027-01-20 才适用 | ★ |
| 「人形机器人国标已发布」 | 立项/审定中 | ★ |

---

## Phase 2 提炼提示

### 「行业表达 DNA」直接素材（喂 Phase 2.5）

**高频黑话 top 12**（说出口就像内行）：
1. 「重复定位精度还是绝对精度？」
2. 「分母是多少？」（问成功率时）
3. 「干预率多少？」
4. 「过奇异了」
5. 「TCP 重标一下」
6. 「负载的重心离法兰多远？」
7. 「下位机 / 上位机」（中文工业圈特有，英文无对应）
8. 「大脑 / 小脑 / 肢体」（中国政策与产业语境专用分层，出自工信部指导意见）evidence: [T06-S042]
9. 「sim2real 掉了多少？」
10. 「QoS 不兼容」
11. 「换型要多久？」
12. 「这是应用属性还是产品属性？」（谈安全时）

**行业拒绝的厂商话术 top 6**（拒绝本身反映价值观）：
1. 「零样本泛化」（不说训练集里同类样本多少）
2. 「全自主」（不说干预率与远程兜底）
3. 「通用机器人」（不说换任务要多少数据）
4. 「协作机器人天生安全」（把安全说成产品属性）
5. 「数字孪生」（其实是离线编程仿真）
6. 「CE 认证」（把自我声明说成认证）

**外行破绽 top 15**（insider-only spotting tells，来自 O 节汇总，按暴露强度排序）：
1. 「精度 0.02 毫米」不分 accuracy / repeatability
2. 「成功率 90%」不给分母
3. 「实时，延迟几毫秒」只报平均值
4. 「泛化能力强」不分四层
5. 「协作机器人不用围栏」
6. 「CE 认证」
7. 「这台机器人是 PLd 的」
8. 「20 kg 负载，我这 15 kg 的件肯定行」
9. 「加个力传感器就能做力控」
10. 「仿真里成功率 95%」
11. 「用 ROS 2 所以是实时的」
12. 「节拍 3 秒」（说的其实是循环时间）
13. 「AMR 不是 AGV，标准不管我们」
14. 「采了 10 万条轨迹」不说多样性
15. 「AI Act 2026 年 8 月就要合规」/「机械法规已经生效」（时效错位）

### 「智识谱系」线索（喂 Phase 2.7）

- **安全标准的合并方向**：ISO/TS 15066:2016（把协作单独做成一份 TS）→ 2025 年被并回 ISO 10218-1/-2。**范式变化：行业不再把「协作机器人」当作一个独立品类来监管，而是回到「协作是一种应用方式」的框架。** 这直接对应工程界从「买台协作臂就安全」到「安全是应用级风险评估结果」的认知修正。evidence: [T06-S003, T06-S026]
- **AI 合规的归口之争**：AI Act 试图横向统管所有高风险 AI → Digital Omnibus (EU) 2026/1744 把机械类 AI 的技术要求推回机械法规（纵向的产品法）。**这是「横向 AI 法」与「纵向产品安全法」两种监管哲学的一次实际胜负**，结果是纵向产品法赢了机械这一块。evidence: [T06-S036, T06-S088]
- **中美欧三套体系并行**：同一台移动机器人在欧盟看 EN ISO 3691-4、在美国看 R15.08、在中国看 GB 11291 系列 —— 标准碎片化是这一行出海成本的硬件层。evidence: [T06-S010, T06-S028, T06-S046]
- **中国国标滞后于国际版本两代**：GB 11291.1-2011 等同采用的是 ISO 10218-1:**2006**，而国际已到 2025 版。**这个代差本身是中国机器人产业「内销合规」与「出口合规」双轨的结构性原因。** evidence: [T06-S046, T06-S002]
- **术语的两个源头**：机械侧术语来自 ISO/GB 词汇表（稳定、可查、有法律含义）；学习侧术语来自 2022 年后的论文（VLA / action chunking / cross-embodiment，三年内成型、定义仍在漂）。**这一行的语言正处在两套体系尚未融合的阶段**，是它区别于成熟工程行业的最显著特征。evidence: [T06-S001, T06-S057, T06-S056, T06-S060]

### 「时效性」信号（喂 Phase 2.8 诚实边界）

**过去 12 个月内有实质变化的（截至 2026-09-02）：**
1. **Regulation (EU) 2026/1744**（2026-07-27 生效）——推迟 AI Act 高风险适用日，并把机械类 AI 要求归到机械法规。evidence: [T06-S036, T06-S088]
2. **《人形机器人与具身智能标准体系（2026 版）》**（2026-02-28 发布）。evidence: [T06-S092]
3. **工信部人形机器人与具身智能标委会成立**（2025-12-26）。evidence: [T06-S091]
4. **ANSI/A3 R15.06-2025 三部分完整发布**（2025-10-29）。evidence: [T06-S025]
5. **首批人形机器人国家标准进入审定**（2026-06）。evidence: [T06-S052]
6. **IEC 62061 AMD2:2026** 发布。evidence: [T06-S019]

**预计未来 12-24 个月会变的（法规与标准时效风险清单）：**

| 项 | 变化 | 触发时间 | 影响 |
|---|---|---|---|
| Regulation (EU) 2023/1230 机械法规 | 从「已发布未适用」变为「适用」 | **2027-01-20** | 出口欧盟的全部 CE 文件路径切换；风险最高的一条 |
| EN ISO 13849-1:2023 过渡期结束 | 旧版 2015 失去符合性推定 | **2027-05-15** | 所有安全功能计算需按新版复核 |
| AI Act Annex III 独立高风险 | 开始适用 | **2027-12-02** | 独立 AI 系统（非嵌入产品）合规 |
| AI Act Annex I 嵌入式高风险 + 机械法规委托法案 | 开始适用 / 委托法案期限 | **2028-08-02** | 机器人 AI 安全部件的技术要求最终落到机械法规里 |
| ISO/DIS 3691-4 | 新版发布 | 12-24 个月内 | AMR/AGV 安全方案需复核 |
| ISO/DIS 13482 | 修订为「服务机器人安全要求」并发布 | 12-24 个月内 | 家用/服务/人形机器人最相关的一条国际安全线 |
| 中国首批人形机器人国家标准 | 从审定到发布实施 | 12-24 个月内 | 国内人形机器人验收与招投标依据出现 |
| GB 11291 系列 | 是否跟进 ISO 10218:2025 修订 | 未定，需持续监控 | 决定国内合规是否继续落后两代 |
| IEC 61508 第 3 版 | 修订中 | 未定 | 功能安全母标准变动会向下传导 |
| ISO 18646 系列新分部 | 持续扩张 | 12-24 个月内 | 服务机器人性能宣称的可比性 |

**decay 结论**：本 track 的**标准与法规部分 decay = high**（欧盟侧 2027-2028 有三个硬日期，中国侧人形标准正在发布通道里）；**术语部分 decay = low-medium**（机械侧稳定，学习侧的 VLA / action chunking 等 2022 年后术语仍在漂，2 年内定义可能收敛或分化）。**建议 master skill 的刷新触发点设在 2027-01-20 与 2027-05-15。**

### 「工作流变化触发」种子（喂 wave 3 Track 03）

近 12-24 个月内的修订将直接改变以下工作流假设：
1. **CE 技术文件工作流**：2027-01-20 起从机械指令切到机械法规 → 新增软件更新、网络安全（防篡改）、数字化说明书相关的文件项；出口项目的合规排期需提前 12 个月启动。evidence: [T06-S035, T06-S039]
2. **安全功能计算工作流**：EN ISO 13849-1:2023 过渡期 2027-05-15 结束 → 已交付项目的 PL 计算需按新版复核（方法学有变）。evidence: [T06-S008, T06-S090]
3. **协作单元验证工作流**：从「引 TS 15066 做力/压强测试」改为「引 ISO 10218-2:2025 相应内容」，测试仍要做，**引用依据变了**（合同与报告模板需更新）。evidence: [T06-S003, T06-S026]
4. **北美项目工作流**：R15.06-2012 → R15.06-2025（含全新 Part 3 用户侧要求）→ 用户方（终端工厂）第一次有了明确的美国国家标准义务。evidence: [T06-S025, T06-S033]
5. **AI 安全部件合规工作流**：不再做「AI Act + 机械法规」双份合格评定，改为在机械法规框架内一次完成 → 但要等 2028-08-02 前的委托法案，**当前处于「规则已定方向、细则未出」的过渡窗口**，方案里不应承诺具体条款。evidence: [T06-S088]
6. **国内人形机器人项目工作流**：首批国标发布后，招投标与验收将从「厂商自定义指标」转为「按国标测」——**现在就该按立项名单里的分部（总则/环境感知/决策规划/运动控制/操作任务/仿真测试平台）预留测试项**。evidence: [T06-S049, T06-S052]

### 合规红线（Phase 2 必须写进 skill 的「绝对不能给的建议」）

以下操作**在任何情况下都不能作为建议给出**，即使用户以「只是测试」「先跑起来」「demo 用」为由要求：

1. **绕过或跳过风险评估**——ISO 12100 的风险评估是所有后续措施的法律与工程前提，没有它，任何安全方案都不成立。evidence: [T06-S007]
2. **屏蔽、短接或旁路安全监控与安全回路**——包括短接安全门开关、旁路光幕、屏蔽安全限速/安全限位、把安全 I/O 接成常通。这是事故与刑责的直接来源。evidence: [T06-S040, T06-S093]
3. **超出经验证的速度或力限值运行协作应用**——PFL 模式下的力/压强限值必须实测验证；「先调高看看能不能过节拍」是明确禁止的。evidence: [T06-S003, T06-S026]
4. **拆除或不装安全围栏、光幕、安全地毯**而不做等效替代与重新评估。evidence: [T06-S040]
5. **用软件限速/软件急停替代安全通道**——安全功能必须由达到所需 PL/SIL 的安全相关部件实现并验证。evidence: [T06-S008, T06-S018]
6. **在示教/调试模式下取消使能装置（三位开关）或降速限制**。evidence: [T06-S002]
7. **把神经网络直接接到安全功能上**（如用视觉模型做唯一的人体检测来允许人进入危险区），而不叠加经认证的安全传感与限速。当前没有任何已发布标准支持这种架构作为独立安全措施。evidence: [T06-S002, T06-S037]
8. **在没有 CE/NRTL 合规路径的情况下向欧盟/美国市场投放设备**，或把「CE 自我声明」说成「CE 认证」以规避公告机构介入。evidence: [T06-S035, T06-S099]
9. **在国内项目上以「按 ISO 最新版做了」替代 GB 11291 强制性国标的符合性**——强制性国标是法定要求，国际标准不能自动替代。evidence: [T06-S046, T06-S047]
10. **伪造或选择性报告性能数据**——包括用仿真数字充当真机数字、报无分母成功率、报剪辑后的 demo 作为可重复能力。这是技术诚信红线，也是产品责任风险。

### 冷僻 / 信号薄弱评估

- 术语总数：**约 88 个**（A-G 七组）→ 远高于 25 的冷僻阈值。
- Tier 1：**35 个**（≥ 15 ✅）；Tier 1 + Tier 2 = **77 个**（≥ 40 ✅）。
- 标准与法规条目：**28 项**（≥ 20 ✅），全部带版本、发布日、适用日、法域、适用对象。
- Tier 1 全部填了 outsider-tell ✅；Tier 2 约 60% 填了 ✅。
- source 数：**100 条** — verified_primary 33 条、surrogate_primary 57 条、secondary 10 条，**无黑名单条目、无死链标记**（已用 `tools/research/source_verifier.py scan` 校验）。
- **本 track 不属于冷僻行业**。信号充足，但有两处需要在诚实边界里点明：
  1. **iso.org / webstore.iec.ch 的标准正文需付费**，本文件对标准内容的描述来自标准页摘要、发布机构 FAQ 与协会解读，**未逐条阅读标准正文**；因此**未引用任何条款号**，只写标准号与节名。
  2. **中国人形机器人系列国标处于立项/审定阶段**，其具体分部名称与指标以最终发布文本为准；本文件记录的是截至 2026-09-02 的公开状态。
- 5 类 type 分布：Term ✅（大头）、Acronym ✅（大量）、Standard ✅（≥ 20）、Regulation ✅（EU/US/CN 三地）、Certification ✅（但**研发岗执业资格 = N/A**，全球均无该制度，见 N4）。
