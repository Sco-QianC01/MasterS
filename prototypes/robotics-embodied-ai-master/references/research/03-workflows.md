# Track 03 — Workflows（工作流 / SOP）· 机器人与具身智能（locale=zh-CN）

> Phase 1 Wave 2 · Track 03。全部 `last_checked = 2026-09-02`。
> Wave 1 seed：`04-canon.md`（经典著作与课程描述的流程）、`05-sources.md`（数据集采集口径）、`06-glossary.md`（评测与运营术语、合规红线、外行破绽）。跨轨 evidence 直接引用 `T04-*` / `T05-*` / `T06-*` id，**不在本 manifest 重复登记**。
>
> **本 track 的三条口径纪律**（先读这个再读工作流卡）：
> 1. **区分「论文里的流程」与「交付里的流程」**。论文流程公开、可追溯、可引用；交付流程大量闭源，只能从厂商部署手册、集成商验收规范、招聘 JD、标准条文里反推。每条工作流会标注它属于哪一类，以及哪一段是反推的。
> 2. **数字带口径**。凡出现「多久」「多少条」「多少钱」，要么有一手来源 id，要么写明「本轨未获取公开一手数据」。**不编行业经验值**。
> 3. **遥操作介入与自主性能分开记**。「有人接管」的成功不算自主成功——这是本行评测最大的糊涂账，见工作流 9。evidence: [T06-S044]

## Source Manifest

> 全部 `last_checked = 2026-09-02`。标注约定与 Track 06 保持一致：**政府/监管原文与同行评议论文** → `verified_primary`；**厂商与项目自有文档、集成商自有站点、协会、标准机构页、招聘 JD、课程** → `surrogate_primary` 并在 note 写明来源类型；**行业媒体与二手转述** → `secondary`。跨轨 id（`T04-*` / `T05-*` / `T06-*`）不在此表重复登记。

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T03-S001 | https://www.nist.gov/blogs/manufacturing-innovation-blog/how-make-your-first-robot-integration-success | verified_primary | 2026-09-02 | NIST MEP | regulator / 政府机构 — 首次机器人集成项目四条建议 |
| T03-S002 | https://arxiv.org/abs/2503.10966 | verified_primary | 2026-09-02 | Snyder, Hanks et al. | 模仿学习策略对比的近最优停止规则 |
| T03-S003 | https://arxiv.org/abs/2506.18123 | verified_primary | 2026-09-02 | Atreya et al. | RoboArena 分布式真机双盲评测 |
| T03-S004 | https://proceedings.mlr.press/v305/atreya25a.html | verified_primary | 2026-09-02 | PMLR / CoRL 2025 | RoboArena 正式出版版本 |
| T03-S005 | https://github.com/robo-arena/roboarena | verified_primary | 2026-09-02 | RoboArena 团队 | 评测基础设施代码与评测协议 |
| T03-S006 | https://arxiv.org/abs/2510.17950 | verified_primary | 2026-09-02 | RoboChallenge 团队 | 大规模真机评测平台与任务集 |
| T03-S007 | https://arxiv.org/abs/2510.04354 | verified_primary | 2026-09-02 | Zhao, Ren et al. | 用不完美仿真器做可靠策略评测（含置信区间） |
| T03-S008 | https://arxiv.org/abs/2603.13616 | verified_primary | 2026-09-02 | (2026-03 预印本) | 超越二元成功率的样本高效策略比较 |
| T03-S009 | https://medium.com/toyotaresearch/statistical-thinking-for-robot-policy-evaluation-from-rigorous-a-b-testing-to-effective-0ae886fbd68d | surrogate_primary | 2026-09-02 | Toyota Research Institute | own publication — 机器人策略评测的统计学方法 |
| T03-S010 | https://toyotaresearchinstitute.github.io/lbm1/ | surrogate_primary | 2026-09-02 | Toyota Research Institute | own publication — LBM 1.0 评测方法与真机 rollout 数 |
| T03-S011 | https://www.tri.global/news/tri-pretrained-large-behavior-models-accelerate-robot-learning | surrogate_primary | 2026-09-02 | Toyota Research Institute | own site — LBM 预训练效果的官方口径 |
| T03-S012 | https://www.roboticsproceedings.org/rss20/p120.pdf | verified_primary | 2026-09-02 | Khazatsky et al. | DROID 论文全文（RSS 2024），采集协议细节 |
| T03-S013 | https://www.roboticsproceedings.org/rss20/p045.pdf | verified_primary | 2026-09-02 | Chi et al. | UMI 论文全文（RSS 2024），手持夹爪采集协议 |
| T03-S014 | https://umi-gripper.github.io/ | surrogate_primary | 2026-09-02 | UMI 团队 | originator 官方页 — 硬件 BOM 与复现说明 |
| T03-S015 | https://arxiv.org/abs/2409.19499 | verified_primary | 2026-09-02 | FastUMI 团队 | 去镜面 / 硬件无关的 UMI 变体 |
| T03-S016 | https://moveit.picknik.ai/main/doc/examples/hand_eye_calibration/hand_eye_calibration_tutorial.html | surrogate_primary | 2026-09-02 | PickNik / MoveIt | vendor docs — 手眼标定操作流程与最少样本数 |
| T03-S017 | https://github.com/moveit/moveit2_tutorials/blob/main/doc/examples/hand_eye_calibration/hand_eye_calibration_tutorial.rst | verified_primary | 2026-09-02 | MoveIt 项目 | 手眼标定教程源文件（可查改动历史） |
| T03-S018 | https://blog.zivid.com/precision-and-trueness | surrogate_primary | 2026-09-02 | Zivid | vendor docs — precision 与 trueness 的区分 |
| T03-S019 | https://support.zivid.com/camera/academy/applications/piece-picking/prepare-for-production.html | surrogate_primary | 2026-09-02 | Zivid | vendor docs — 拣选应用投产前准备流程 |
| T03-S020 | https://blog.zivid.com/achieving-optimal-hand-eye-calibration-for-enhanced-robotics-performance | surrogate_primary | 2026-09-02 | Zivid | vendor docs — 手眼标定位姿分布与误差来源 |
| T03-S021 | https://www.cognex.com/en/applications/guidance-and-alignment/vision-guided-robotics-for-industrial-automation | surrogate_primary | 2026-09-02 | Cognex | vendor docs — 视觉引导机器人应用口径 |
| T03-S022 | https://pmc.ncbi.nlm.nih.gov/articles/PMC9581431/ | verified_primary | 2026-09-02 | Enebuse et al. | 手眼标定方法精度评估（同行评议） |
| T03-S023 | https://www.universal-robots.com/manuals/EN/HTML/SW5_21/Content/prod-cable40m/risk_assessment.htm | surrogate_primary | 2026-09-02 | Universal Robots | vendor docs — 用户手册里的风险评估义务条款 |
| T03-S024 | https://www.universal-robots.com/media/1805223/28_05_2019-ur_safety_made_easy.pdf | surrogate_primary | 2026-09-02 | Universal Robots | vendor docs — 协作应用安全配置与验证白皮书 |
| T03-S025 | https://www.universal-robots.com/blog/collaborative-robots-iso-technical-specification/ | surrogate_primary | 2026-09-02 | Universal Robots | vendor docs — 15066 在应用层怎么用 |
| T03-S026 | https://www.pilz.com/en-US/services/machinery-safety/validation | surrogate_primary | 2026-09-02 | Pilz | vendor docs — 安全验证服务的交付物清单 |
| T03-S027 | https://www.pilz.com/en-US/trainings/articles/236038 | surrogate_primary | 2026-09-02 | Pilz | vendor docs — 机器人安全与集成培训大纲 |
| T03-S028 | https://www.pilz.com/en-US/products/robotics | surrogate_primary | 2026-09-02 | Pilz | vendor docs — PRMS 力/压强实测系统 |
| T03-S029 | https://arxiv.org/abs/2203.02706 | verified_primary | 2026-09-02 | Fischer et al. | ISO/TS 15066 不同解读如何改变风险评估结果 |
| T03-S030 | https://pmc.ncbi.nlm.nih.gov/articles/PMC11033501/ | verified_primary | 2026-09-02 | (同行评议) | 人机协作接触力痛阈实测研究 |
| T03-S031 | https://pmc.ncbi.nlm.nih.gov/articles/PMC10446043/ | verified_primary | 2026-09-02 | VALU3S 项目 | 车身白车身机器人检测单元的 V&V 用例 |
| T03-S032 | https://arxiv.org/abs/2011.10294 | verified_primary | 2026-09-02 | (同行评议预印本) | 基于仿真的机器人系统早期安全验证 |
| T03-S033 | https://github.com/Physical-Intelligence/openpi | verified_primary | 2026-09-02 | Physical Intelligence | openpi 微调三步流程与显存门槛 |
| T03-S034 | https://www.pi.website/blog/openpi | surrogate_primary | 2026-09-02 | Physical Intelligence | own publication — 开源权重与微调数据量口径 |
| T03-S035 | https://www.pi.website/blog/pi0 | surrogate_primary | 2026-09-02 | Physical Intelligence | own publication — π0 预训练/后训练两段式配方 |
| T03-S036 | https://arxiv.org/abs/2504.16054 | verified_primary | 2026-09-02 | Physical Intelligence | π0.5 开放世界泛化与数据配比 |
| T03-S037 | https://huggingface.co/blog/pi0 | verified_primary | 2026-09-02 | Hugging Face | π0 移植进 LeRobot 的工程说明 |
| T03-S038 | https://github.com/huggingface/lerobot/blob/main/docs/source/smolvla.mdx | verified_primary | 2026-09-02 | Hugging Face LeRobot | 录多少 episodes、训练多久的官方建议 |
| T03-S039 | https://huggingface.co/lerobot/smolvla_base | verified_primary | 2026-09-02 | Hugging Face LeRobot | SmolVLA 基座模型卡与微调口径 |
| T03-S040 | https://isaac-sim.github.io/IsaacLab/main/source/policy_deployment/index.html | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Isaac Lab sim2real 部署工作流入口 |
| T03-S041 | https://isaac-sim.github.io/IsaacLab/main/source/policy_deployment/02_gear_assembly/gear_assembly_policy.html | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — UR10e 齿轮装配策略训练到 ROS 部署全流程 |
| T03-S042 | https://isaac-sim.github.io/IsaacLab/main/source/refs/reference_architecture/index.html | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — 端到端机器人学习参考架构 |
| T03-S043 | https://developer.nvidia.com/blog/closing-the-sim-to-real-gap-training-spot-quadruped-locomotion-with-nvidia-isaac-lab/ | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — Spot 四足 sim2real 的域随机化与 actuator net |
| T03-S044 | https://developer.nvidia.com/blog/bridging-the-sim-to-real-gap-for-industrial-robotic-assembly-applications-using-nvidia-isaac-lab/ | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — 工业装配场景的 sim2real 流程 |
| T03-S045 | https://arxiv.org/abs/2511.04831 | verified_primary | 2026-09-02 | NVIDIA 等 | Isaac Lab 框架论文（训练规模与接口） |
| T03-S046 | https://isaac-sim.github.io/IsaacLab/main/source/api/lab/isaaclab.sim.converters.html | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — URDF/MJCF→USD 转换器与碰撞体近似参数 |
| T03-S047 | https://docs.isaacsim.omniverse.nvidia.com/5.0.0/importer_exporter/ext_isaacsim_asset_importer_urdf.html | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs — URDF 导入器：惯量、碰撞网格、关节驱动设置 |
| T03-S048 | https://foxglove.dev/product/visualization | surrogate_primary | 2026-09-02 | Foxglove | vendor docs — 多源日志同一时间线回放 |
| T03-S049 | https://foxglove.dev/robotics/rviz-vs-foxglove-vs-rerun | surrogate_primary | 2026-09-02 | Foxglove | vendor docs — 可视化/回放工具的定位差异（含自评偏向） |
| T03-S050 | https://arxiv.org/abs/2506.09937 | verified_primary | 2026-09-02 | Gu et al. | SAFE：VLA 策略的多任务失败检测 |
| T03-S051 | https://hbba.sacinfo.org.cn/stdDetail/4d3a45b4f20d7c3828f85f1a585dfba1 | surrogate_primary | 2026-09-02 | 全国标准信息公共服务平台 | standards body — JB/T 10825-2025《工业机器人产品验收实施规范》 |
| T03-S052 | https://std.samr.gov.cn/gb/search/gbDetailed?id=71F772D7896BD3A7E05397BE0A0AB82A | verified_primary | 2026-09-02 | 国家标准委 | 监管 — GB/T 20867-2007《工业机器人 安全实施规范》 |
| T03-S053 | https://openstd.samr.gov.cn/bzgk/gb/newGbInfo?hcno=195AC593CF1E50EDD9CB4AA4BAD78104 | verified_primary | 2026-09-02 | 国家标准委 | 监管 — GB/T 20868-2024 在线全文入口 |
| T03-S054 | https://www.jaka.com/jszl.html | surrogate_primary | 2026-09-02 | 节卡 JAKA | vendor docs — 中国协作臂厂商的技术资料/手册下载页 |
| T03-S055 | https://www.jaka.com/profile/upload/2025/11/25/20251125172831A006.pdf | surrogate_primary | 2026-09-02 | 节卡 JAKA | vendor docs — 硬件用户手册（安装、接线、安全配置） |
| T03-S056 | https://www.codroid.ai/download/shouce/v1107.pdf | surrogate_primary | 2026-09-02 | 埃斯顿酷卓 | vendor docs — S 系列协作机器人用户手册 V1.0（2025） |
| T03-S057 | https://www.codroid.ai/file | surrogate_primary | 2026-09-02 | 埃斯顿酷卓 | vendor docs — 资料下载总入口 |
| T03-S058 | https://www.unitree.com/cn/position/ | surrogate_primary | 2026-09-02 | 宇树科技 Unitree | JD — 数据运营/具身软件/评估/测试岗职责反推分工 |
| T03-S059 | https://www.unitree.com/position/ | surrogate_primary | 2026-09-02 | 宇树科技 Unitree | JD — 英文版岗位列表（交叉核对） |
| T03-S060 | https://blog.unchainedrobotics.de/en/how-does-the-commissioning-of-a-turnkey-robotic-solution-work | surrogate_primary | 2026-09-02 | Unchained Robotics | vendor docs — 交钥匙机器人方案从 FAT 到 SAT 的阶段划分 |
| T03-S061 | https://blog.unchainedrobotics.de/en/how-to-choose-the-right-system-integrator-for-your-robot-cell | surrogate_primary | 2026-09-02 | Unchained Robotics | vendor docs — 集成商筛选与 run-off 验收标准 |
| T03-S062 | https://motioncontrolsrobotics.com/resources/tech-talk-articles/what-is-a-robot-system-fat/ | surrogate_primary | 2026-09-02 | Motion Controls Robotics | vendor docs — FANUC 认证集成商对 FAT 的定义与清单 |
| T03-S063 | https://blog.svtrobotics.com/re-envision-robotics-integration-three-steps-to-success | surrogate_primary | 2026-09-02 | SVT Robotics | vendor docs — 集成项目三阶段（含与 WMS/MES 边界） |
| T03-S064 | https://doug-machine.com/feeds/blog/robotic-welding-integration | surrogate_primary | 2026-09-02 | Doug Machine（集成商） | vendor docs — 集成失败主因归结为零件变异/工装不良/需求不清 |
| T03-S089 | https://www.automationwithinreach.com/blog/integrating-cnc-robotics-into-operations | surrogate_primary | 2026-09-02 | Automation Within Reach | vendor docs — 找集成商前要备齐的图纸与公差材料清单 |
| T03-S090 | https://mtlcraftautomationgroup.com/blog/common-mistakes-when-implementing-robotics | surrogate_primary | 2026-09-02 | Metalcraft Automation Group | vendor docs — 机器人导入常见错误清单（集成商视角） |
| T03-S065 | https://www.automate.org/robotics/tech-papers/innovating-small-assembly-robot-integration-concepts-within-the-plc | surrogate_primary | 2026-09-02 | A3 | 协会 — 机器人逻辑放进 PLC 的集成范式技术文 |
| T03-S066 | https://ifr.org/post/faster-robot-communication-through-the-opc-robotics-companion-specification | surrogate_primary | 2026-09-02 | IFR | 协会 — OPC UA Robotics Companion Spec 的产线通信定位 |
| T03-S067 | https://control.com/technical-articles/robot-to-plc-handshaking/ | secondary | 2026-09-02 | Control.com | 机器人与 PLC 握手信号的具体信号集 |
| T03-S068 | https://www.agilityrobotics.com/content/digit-deployed-at-gxo-in-historic-humanoid-raas-agreement | surrogate_primary | 2026-09-02 | Agility Robotics | own site — 首个人形 RaaS 商业部署的官方描述 |
| T03-S069 | https://gxo.com/news_article/gxo-signs-industry-first-multi-year-agreement-with-agility-robotics/ | surrogate_primary | 2026-09-02 | GXO Logistics | own site — 用户方（终端客户）对同一部署的口径 |
| T03-S070 | https://www.agilityrobotics.com/content/digits-next-steps | surrogate_primary | 2026-09-02 | Agility Robotics | own site — 部署迭代与产品路线的官方说明 |
| T03-S071 | https://www.sec.gov/Archives/edgar/data/0002074973/000121390026071287/ea029548401ex99-2.htm | verified_primary | 2026-09-02 | SEC EDGAR | 监管 — 上市文件里的人形部署与 RaaS 单位经济披露 |
| T03-S072 | https://m.thepaper.cn/newsDetail_forward_33035259 | secondary | 2026-09-02 | 澎湃新闻（澎湃号专栏） | 中国具身数据采集产业的成本与规模转述（非一手） |
| T03-S073 | https://www.21jingji.com/article/20251230/herald/b0276617203a86aca6b23944b5b45b46.html | secondary | 2026-09-02 | 21 世纪经济报道 | 优必选管理层访谈：人形进厂聚焦哪些工位 |
| T03-S074 | https://www.ithome.com/0/908/238.htm | secondary | 2026-09-02 | IT 之家 | 第 1000 台工业人形下线报道（产能口径，非部署口径） |
| T03-S075 | https://m.chinaagv.com/news/detail/202412/31970.html | secondary | 2026-09-02 | AGV 网 | 人形机器人进车厂「实训」的中文行业口径来源 |
| T03-S076 | https://www.trossenrobotics.com/post/robot-learning-evaluation-benchmarking-real-hardware | surrogate_primary | 2026-09-02 | Trossen Robotics | vendor docs — 真机评测的可重复性要求（硬件供应商视角） |
| T03-S077 | https://www.stereolabs.com/blog/droid-case-study-robotics-research | surrogate_primary | 2026-09-02 | Stereolabs | vendor docs — DROID 相机配置与同步的供应商侧描述 |
| T03-S078 | https://arxiv.org/abs/2605.20774 | verified_primary | 2026-09-02 | (2026-05 预印本) | VLA-REPLICA：低成本可复现的真机评测基准 |
| T03-S079 | https://arxiv.org/abs/2511.04665 | verified_primary | 2026-09-02 | (2025-11 预印本) | 高斯泼溅 real-to-sim 评测软体接触 |
| T03-S080 | https://openreview.net/forum?id=cpmwi3Xwcr | verified_primary | 2026-09-02 | OpenReview / CoRL | RoboArena 公开评审意见（含评测协议争议） |
| T03-S081 | https://sites.google.com/view/corl-roboarena | surrogate_primary | 2026-09-02 | CoRL RoboArena Workshop | 协会/会议 — 评测方法学专题研讨 |
| T03-S082 | https://arxiv.org/abs/2410.24164 | verified_primary | 2026-09-02 | Black et al. | π0 论文（预训练/后训练两段与真机评测口径） |
| T03-S083 | https://www.automate.org/robotics/robotics-certifications/robotic-integrator-certification-program | surrogate_primary | 2026-09-02 | A3 | 协会 — 集成商认证审核项（反推交付流程要求） |
| T03-S084 | https://simulately.wiki/docs/toolkits/ConvexDecomp/ | secondary | 2026-09-02 | Simulately（社区 wiki） | 凸分解工具链（VHACD/CoACD）实操口径 |
| T03-S085 | https://rigyd.com/resources/how-to-convert-3d-models-to-simulation-ready-assets | surrogate_primary | 2026-09-02 | Rigyd | vendor docs — CAD→仿真资产的清理与物理属性补全流程 |
| T03-S086 | https://forums.developer.nvidia.com/t/importing-pre-computed-convex-decomp-collision-meshes-from-urdf/202562 | surrogate_primary | 2026-09-02 | NVIDIA 开发者论坛 | vendor docs — 预计算碰撞网格导入的实际坑 |
| T03-S087 | https://www.roboticsproceedings.org/ | verified_primary | 2026-09-02 | RSS Foundation | 会议全文开放库（本轨多篇论文的稳定入口） |
| T03-S088 | https://arxiv.org/abs/2403.12945 | verified_primary | 2026-09-02 | Khazatsky et al. | DROID arXiv 版（与 T05-S033 官方页互证） |

**Manifest 统计**：90 条（机械计数）。`verified_primary` **33** 条（36.7%）、`surrogate_primary` **51** 条（56.7%）、`secondary` **6** 条（6.7%）、`reference` 0 条。**无黑名单条目**（搜索中出现的知乎 / CSDN / 腾讯新闻 / emergentmind 等 AI 摘要站均已剔除，未进表）。所有 `surrogate_primary` 的 note 均含规定关键词（vendor docs / own site / own publication / originator / 协会 / standards body / 监管 / JD），未使用 `official`。
**一手占比口径**：本轨把「论文原文 + 政府监管原文 + 项目自有代码仓」记为一手（33 条），把「厂商与集成商自有文档 + 协会 + 招聘 JD + 会议/课程页」记为准一手（51 条）；两者合计 **84/90 = 93.3%**，二手转述仅 6 条（其中 4 条用于中国侧产业数字），正文中已逐条标注「媒体转述，非一手」。

**链接可达性复核（2026-09-02，`curl -L` 实测）**：全部 URL 均无 4xx 死链。以下几条在自动化访问时返回反爬状态码（**不是死链**，浏览器可正常打开，内容已在调研时读取）：`T03-S026 / T03-S027 / T03-S028`（pilz.com，403）、`T03-S065 / T03-S083`（automate.org，403）、`T03-S021`（cognex.com，429）。另有两条首次请求超时、重试后 200：`T03-S004`（proceedings.mlr.press）、`T03-S016`（moveit.picknik.ai）。Phase 4 复核时按 `403/429 = 反爬` 而非 `dead` 处理。另有两条需带合规 User-Agent 才能访问：`T03-S069`（gxo.com）、`T03-S071`（sec.gov，SEC 要求 UA 内含联系方式），以及 `T03-S009`（medium.com，403 反爬）。**唯一一条真死链已剔除**：调研中曾用到的 `diy-robotics.com/implementing-your-first-robot-in-manufacturing` 返回 500，已从 manifest 移除并用同类集成商材料（T03-S064 / T03-S089 / T03-S090）替代。

## 总览（按 decay risk 分组）

**13 条工作流，覆盖「要不要做 → 上线之后」全链路。** 阅读顺序即交付顺序；工作流 9（评测）与 10（安全）是横切的，在多个阶段反复调用。

### High decay（12 个月内会显著改写）— 6 条

| # | Workflow | Trigger | Output | Last_updated | 资深差异（skip/optimize/add） |
|---|----------|---------|--------|-------------|------------------------------|
| 5 | 仿真环境与资产准备 | 要走学习路线 / 要验节拍 / 硬件未到 | 可复现仿真工程 + 「不可信清单」 | 2025-11 | 2/2/1 |
| 6 | 方案开发（传统/学习/混合分层） | 标定完成，进入功能开发 | 可重复系统 + 「自主/规则/人工」架构图 | 2026-09-02 | 2/2/2 |
| 7 | 数据采集与训练循环 | 观测动作空间冻结 | 带元数据数据集 + 策略 + 补采清单 | 2026-06-03 | 2/2/2 |
| 8 | sim-to-real 与真机调试 | 仿真收敛 | 真机可跑策略 + gap 归因记录 | 2025-11 | 2/2/2 |
| 9 | 评测协议设计与读别人的评测 | 要回答「A 比 B 好吗 / 能否上线」 | 带不确定度的评测报告 | 2026-03 | 1/3/3 |
| 10 | 安全评估与合规 | 有人可进入可达空间 / 要出口 | 安全文件包 + 实测数据 + 地区合规文件 | 2026-07-27 | 1/2/3 |

### Medium decay（12–24 个月出现显著优化路径）— 5 条

| # | Workflow | Trigger | Output | Last_updated | 资深差异 |
|---|----------|---------|--------|-------------|---------|
| 1 | 任务定义与可行性判断 | 有人提出「上机器人」 | 任务定义书（含「不做」的论证） | 2026-06-03 | 1/2/2 |
| 2 | 形态与本体选型 | 任务书过评审 | 选型报告 + 成本表 + 被否形态 | 2026-06 | 2/1/2 |
| 11 | 现场部署与集成 | 厂内验证通过 / 现场具备条件 | 通过 SAT 的设备 + 文档包 + 培训 | 2026-07-01 | 2/2/3 |
| 12 | 监控、失败复盘与迭代 | 已上线 / 指标恶化 | 失败分类分布 + 五类改动清单 | 2026-09-02 | 1/2/3 |
| 13 | 演示与交付验收（POC vs 量产） | 要写验收条款 / 评估 demo | 两套验收标准表 | 2026-07-01 | 1/2/3 |

### Low decay（已稳态）— 2 条

| # | Workflow | Trigger | Output | Last_updated | 资深差异 |
|---|----------|---------|--------|-------------|---------|
| 3 | 误差预算与硬件选型 | 要回答「能不能保证 ±X」 | 误差预算表 + 选型 + 验收测法 | 2026-09-02 | 1/2/2 |
| 4 | 环境搭建与标定 | 硬件装配到位 | 标定包 + 重复性报告 + 重标触发清单 | 2026-09-02 | 1/2/2 |

**统计**：13 条全部有 `last_updated` 与 `decay risk`；13/13（100%）填了近期变化字段（其中 3 条明确写「稳态 / 无重大变化」）；13/13（100%）有 ≥ 2 处资深差异点。差异点合计 **75 处**，类型分布 **skip 19 / optimize 26 / add 30** —— add 最多，说明这一行的资深特征是「多做几件初学者不做的事」（尤其是留证据、留基线、留退路），而不是单纯少走几步。

## 工作流卡片

### 1. 任务定义与可行性判断（先证明「不该上机器人」）

- **One-liner**：从「客户/老板说想上机器人」到「一份写明该不该做、做哪一段、按什么指标验收的任务书」。**这一步的主要产出经常是「不做」或「先不做机器人」。**
- **属于哪一类流程**：交付流程（论文里没有这一步）。公开材料稀薄，主要证据来自政府制造业推广机构与集成商的自有材料。
- **Trigger**：出现下列任一信号——工位招不到人 / 工位有工伤或职业病风险 / 产能受限于某一工位 / 客户要求自动化率 / 上级要求「上人形试点」。evidence: [T03-S001, T03-S090]
- **Output**：一页任务定义书，含：作业对象与来料状态、循环时间目标与客户节拍、精度与力的容差、异常种类清单、全部运行模式（正常/换型/卡料恢复/维护/可预见误用）、投资与回收期口径、验收指标与测法。evidence: [T03-S001, T03-S089, T06-S043]

**入门 SOP（最少 6 步）**

1. **去现场，掐表，拍视频**（角色：方案工程师 + 现场班组长）。输入：工位实况；输出：一段完整循环的视频 + 手工分解的动作时间表。
   - 跳过会怎样：拿客户口述的「一件 8 秒」去做方案，到现场发现人手在等料、双手同时做两件事、每 20 件要清一次屑，节拍全部作废。
2. **先问三个「能不能不上机器人」**（角色：方案工程师 + 客户工艺）。①能不能改工装/夹具/送料方式，让人做得更快更稳？②能不能改产品设计或来料状态（定向包装、托盘化、增加定位特征）？③能不能改流程顺序或合并工位？输出：三条替代方案的成本与工期，与机器人方案并列。
   - 跳过会怎样：把「来料杂乱、位置随机」这个最贵的问题带进机器人方案，让视觉与规划去补工装的账。多家集成商的公开表述一致指向：机器人集成失败大多不是机器人坏了，是**来料变异、工装不良、需求不清**——设备很少先坏，先坏的是规划。evidence: [T03-S064, T03-S090, T03-S001]
3. **量化来料变异**（角色：工艺 + 质量）。输出：位置/姿态/尺寸/表面状态的分布（不是「大概」，是抽样测出来的范围与离群比例）。
   - 跳过会怎样：所有后续的误差预算、视觉方案、抓取策略全部建立在假设上，真机阶段推倒重来。
4. **写全部运行模式，不只写正常模式**（角色：方案工程师 + 安全工程师）。ISO 12100 的「确定机械限制」这一步要求把设置、卡料恢复、维护、可预见误用都算进去。evidence: [T06-S007, T03-S023]
   - 跳过会怎样：风险评估在后期返工；更常见的是节拍算错——真实产线的时间大量花在异常恢复上。
5. **算一笔含全成本的账**（角色：销售/项目经理 + 客户财务）。分母要含：本体 + 末端工装 + 视觉 + 安全件 + 电控 + 集成人工 + 停线改造 + 培训 + 备件与运维。本行的常识是**本体常只占项目总价的 20–40%**。evidence: [T06-S013]
   - 跳过会怎样：用本体报价谈下项目，交付时发现工装和调试吃掉利润。
6. **定验收指标与测法，写进任务书**（角色：项目经理 + 客户）。每条指标必须写：定义、测法、样本量、判定标准、谁签字。evidence: [T03-S060, T03-S061]
   - 跳过会怎样：交付时进入「你说好了没有 / 我说没好」的扯皮，尾款拖住。

**资深路径（差异点）**

- `skip` 资深人跳过「先做一版仿真给客户看」：在任务定义阶段不碰仿真。理由是此时来料变异还没量化，仿真只会把一个漂亮的假设可视化，反而锁死客户预期。仿真在工作流 5 才进场。
- `optimize` 把第 2 步（能不能不上机器人）提前到**第一次客户会议就问**，并且用「如果我们把来料改成定向托盘，这个项目能便宜多少、快多少」的形式问——把「劝退」变成「降本建议」，客户更容易接受。evidence: [T03-S001]
- `optimize` 第 3 步不测「平均」，只测**最坏 5%**：资深人知道机器人系统的成败由分布尾部决定，均值好看没有意义。这与本行评测的通则一致（成功率必须带分母与初始分布）。evidence: [T06-S044]
- `add` 额外做「谁来改程序」的调研：产线上「换型时谁能动这台机器」决定了运维成本，也决定了该选示教式还是脚本式方案。初学者从不问这一条。evidence: [T06-S044]
- `add` 额外做「失败的破坏性分级」：把预期失败分成可恢复（重试即可）与破坏性（撞件/划伤/掉件/伤人），并在任务书里分开写允许率。evidence: [T06-S044]

**判断这一步是否通过（具体标准）**

- 任务书里的每一条指标都能回答「怎么测、测几次、谁判定」——做不到就不算通过。
- 「不上机器人」的替代方案被明确写下并被客户否掉（而不是没人提过）。
- 全部运行模式（≥ 5 类）都有对应的处理约定。
- 回收期计算里有集成人工与停线损失两项。evidence: [T06-S013]

**常见失败模式**

- **拿演示视频当可行性依据**：客户看了某厂商发布会就要求「这个我们也做」。破解：要求对方给分母（多少次、什么初始分布、有没有人接管）。evidence: [T06-S044]
- **把「柔性」写进需求却不定义换型时间**：结果方案按最难的产品设计，成本翻倍。破解：让客户排出产品族与切换频率，定义换型时间上限。evidence: [T06-S044]
- **需求里只有正常模式**：异常恢复到调试期才发现要占 30% 的工程量（本轨未获取该比例的公开一手数据，此处只写「常被严重低估」）。
- **用本体单价谈判**：签完才发现工装与视觉预算不够。evidence: [T06-S044]

**时间与人力量级**

- 入门 SOP：现场 1–2 天 + 内部 3–5 天，1 名方案工程师 + 0.5 名工艺。
- 资深路径：现场半天 + 2 天出任务书。
- **口径说明**：以上为本轨依据集成商公开的项目阶段描述（FAT/SAT 分期、准备材料清单）做的量级推断，**没有公开一手统计**，不要当行业均值引用。evidence: [T03-S060, T03-S062]

**近期变化（近 12 个月）**：2026-06-03 工信部与国资委联合印发《2026 年度人形机器人与具身智能实景实训专项行动的通知》（工信厅联科函〔2026〕256 号），要求用户单位选取「目标需求明确、工作状况清晰、标准化程度高且具备经济可行性的真实场景单元」，按「最小干预、利旧复用」原则做环境适配，并要求用户单位**制定应用验证测试规程与达标条件**、出具含「作业成功率、效率提升率、安全可靠性及经济可行性」的评估报告。**这条文件把「任务定义 + 验收口径」变成了国内人形试点项目的规定动作**，且明确「最小干预」——即优先改环境而不是改机器人。触发事件类型：政策/法规变化。evidence: [T05-S048]

- **Last_updated**: 2026-06-03（最新一手文件日期）
- **Decay risk**: medium（方法本身稳态十余年；变的是国内政策把它变成了强制环节）
- **关键工具**：秒表 / 视频 + 产品 2D 图与公差 + 3D 模型 + 现有夹具与设备图纸手册（集成商在报价前的标准索取清单）。evidence: [T03-S089, T03-S064]



### 2. 形态与本体选型（含成本与工期账）

- **One-liner**：从「任务书」到「选定形态（专机 / 工业臂 / 协作臂 / 移动操作 / 足式 / 人形）+ 具体型号 + 一张带工期的成本表」。
- **属于哪一类流程**：交付流程。论文完全不涉及；证据来自厂商手册、集成商材料、协会与上市披露。
- **Trigger**：任务书通过评审，进入方案设计。evidence: [T03-S060]
- **Output**：选型报告，含形态判据表、候选型号对比（负载/臂展/重复定位精度/防护等级/接口）、末端与工装方案、成本表（本体/工装/视觉/安全/电控/集成）、工期甘特、以及**被否掉的形态和否掉的理由**。evidence: [T03-S061, T06-S044]

**入门 SOP（5 步）**

1. **按「作业空间 × 变异度 × 节拍」先定形态类别**（角色：方案工程师）。
   - 固定工位 + 固定来料 + 高节拍 → 优先**专机 / 硬自动化**（可能根本不需要机器人）。
   - 固定工位 + 有变异 + 需要柔性 → 工业臂或协作臂。
   - 跨工位取放、场地大 → 移动机器人（AMR）+ 臂 = 移动操作。
   - 环境为人设计、有台阶楼梯或不可改造 → 才考虑足式/人形。
   - 跳过会怎样：直接从「人形很酷」倒推需求，得到一个贵 5–10 倍、节拍差、维护无人会的方案。
2. **按「人机是否共享空间」而不是按「是不是协作臂」定安全路线**（角色：安全工程师）。协作是**应用属性**，同一台协作臂装上刀具或高速搬运就不再是协作应用。evidence: [T06-S003, T06-S026, T03-S023]
   - 跳过会怎样：以为买协作臂就免掉围栏与风险评估，交付时被安全审查打回，工期延一到三个月。
3. **列候选型号，按规格书的**真实**口径比较**（角色：方案工程师）。重复定位精度必须问清是按 ISO 9283 / GB/T 12642 在什么负载、什么速度、哪个测试立方体测的；额定负载必须问重心偏置与转动惯量。evidence: [T06-S006, T06-S048, T06-S044]
   - 跳过会怎样：按 ±0.02 mm 的规格选型，真机在实际外伸与负载下达不到工艺要求。
4. **同步定末端工装（EOAT）与来料呈现方式**（角色：机械工程师）。末端与工装通常是项目中最贵、最容易返工的部分，且**系统故障主要来自末端工装、视觉、上下料与线缆，不是本体**。evidence: [T06-S044]
   - 跳过会怎样：本体选好了，工装做不出来，或工装重量把可用负载吃光。
5. **出成本表与工期，并写清被否形态**（角色：项目经理）。
   - 跳过会怎样：客户三个月后重新问「为什么不用人形」，没有留痕就要重做一遍论证。

**资深路径（差异点）**

- `skip` 资深人跳过「先比十家品牌」：直接锁定团队已有备件、已有调试经验、当地有服务的 1–2 个品牌。理由是本行的隐性成本在**运维与备件**，不在采购价差。
- `skip` 资深人在明确的高节拍固定工位上**跳过机器人**，直接上专机或桁架——并在选型报告里把这条写成正式建议。
- `optimize` 先定末端工装再定本体：工装决定了负载、惯量与所需工作空间，反过来选本体一次到位。初学者顺序相反。
- `add` 额外做「换型账」：把产品族切换时要换的爪、要改的程序、要重标定的项目列成表，估换型时间。柔性产线的真实瓶颈常在换型，不在机器人。evidence: [T06-S044]
- `add` 额外做「谁维护」的落地安排：现场是否有人能改程序、备件从哪里来、故障响应多久。国内有对应的职业技能标准（工业机器人系统运维员），可以用来定岗位能力要求。evidence: [T06-S096]

**判断这一步是否通过（具体标准）**

- 选型报告里每个形态都被显式评估并给出否掉理由（含「不上机器人」）。
- 精度、负载两项指标都写了**测试条件**，不是只抄规格书数字。evidence: [T06-S006]
- 安全路线（围栏 / 光幕 / 安全限速 / PFL 力限）在这一步就已确定，不是留给后面。evidence: [T06-S003]
- 成本表里本体占比被明确算出（若本体占比 > 60%，说明工装与集成预算大概率估少了）。

**常见失败模式**

- **「人形/通用机器人先买一台试试」**：人形当前的商业部署普遍是**限定工位、限定任务、有人陪同**，且中文语境里的「进厂」经常指「实训」而不是常态化生产。选型阶段要把「实训」和「上线」分开写。evidence: [T03-S073, T03-S075, T06-S044]
- **把订单量/产能当部署量**：厂商公布「第 1000 台下线」是产能口径，不是「1000 台在产线上干活」。evidence: [T03-S074, T06-S044]
- **7 轴当成更高精度买**：7 轴的价值是冗余（避奇异、避障、避关节限位），不是精度。evidence: [T06-S044]
- **用协作臂做高节拍**：安全限速一开，节拍直接不达标；再调高速度就要重做风险评估与力/压强实测。evidence: [T03-S024, T06-S003]

**时间与人力量级**

- 入门 SOP：1–3 周（含厂商询价与工装初设），1 名方案 + 0.5 名机械 + 0.3 名安全。
- 资深路径：3–5 天（品牌已锁定、工装有可复用平台）。
- **口径说明**：量级推断自集成商公开的项目阶段划分，**无公开一手统计**。evidence: [T03-S060, T03-S061]

**近期变化（近 12 个月）**：2025-10-29 起 ANSI/A3 R15.06-2025 三部分完整发布，其中**新增的 Part 3 第一次对用户方（终端工厂）提出美国国家标准层面的义务**——北美项目的选型阶段现在要把「用户方要承担什么」写进合同边界。evidence: [T06-S025, T06-S033]。国内侧：首批人形机器人系列国标 2025-04 立项、2026-06 进入审定（含总则/环境感知/决策规划/运动控制/操作任务/仿真测试平台等分部），**尚未发布实施**；人形项目的选型现在应预留按这些分部测试的接口。触发事件类型：标准更新。evidence: [T06-S049, T06-S052]

- **Last_updated**: 2026-06（国标审定）/ 2025-10-29（R15.06-2025）
- **Decay risk**: medium
- **关键工具**：厂商选型手册与用户手册（节卡、埃斯顿酷卓等国内厂商的手册可公开下载，含安装、接线与安全配置章节，是核对接口与安装条件的一手材料）。evidence: [T03-S054, T03-S055, T03-S056, T03-S057]



### 3. 误差预算与硬件选型（从末端精度反推）

- **One-liner**：从「工艺要求的末端容差」反推出一张误差分配表，据此决定相机选型、标定方案、结构刚度、工装定位方式与是否需要力控/柔性补偿。
- **属于哪一类流程**：交付流程 + 机器视觉厂商的公开工程流程。这是把「精度」这个词从营销拉回工程的关键一步。
- **Trigger**：形态与本体已选定，需要回答「这套方案到底能不能保证 ±X mm / ±Y N」。evidence: [T03-S018, T03-S019]
- **Output**：误差预算表（每一项误差源的量级、分布假设、合成方式、余量）、相机与镜头选型、标定方案、工装定位方案、验收测法。evidence: [T03-S018, T03-S020]

**入门 SOP（6 步）**

1. **写下工艺容差与判定方式**（角色：工艺）。例如插入间隙、涂胶宽度、拧紧同轴度。输出：一个数字 + 一个测法。
   - 跳过会怎样：整条误差链没有目标，最后只能靠现场试凑。
2. **列全误差源，逐项给量级**（角色：视觉/机械工程师）。至少要有：相机的 precision（重复性/噪声）与 trueness（与真值的偏差）、内参与畸变残差、手眼标定残差、机器人**绝对**定位误差（不是重复定位精度）、结构与工装的定位误差、热漂移、抓取后工件在爪内的位姿变化。evidence: [T03-S018, T03-S020, T06-S085]
   - 跳过会怎样：把机器人规格书上的 ±0.02 mm 当系统精度用——那是重复性，绝对精度通常差一到两个数量级。evidence: [T06-S006, T06-S085]
3. **合成误差并留余量**（角色：视觉工程师）。明确写清哪些项按方和根（独立随机）合成、哪些按最坏情况直接相加（系统性偏置）。
   - 跳过会怎样：所有项按最坏相加 → 方案过设计、成本爆炸；所有项按方和根 → 现场超差。
4. **决定用「绝对精度路线」还是「相对精度路线」**（角色：方案工程师）。相对路线（视觉在抓取/装配点附近再看一次、做视觉伺服或力控找正）可以绕过机器人绝对精度这一大项；绝对路线必须做运动学标定并接受成本。
   - 跳过会怎样：在一台绝对精度毫米级的机器人上追求亚毫米装配，靠不断加标定次数去补，永远不稳定。
5. **决定容差归谁吃**（角色：机械 + 工艺）。柔性夹爪、浮动法兰、导向倒角、力控搜孔都可以把一部分几何误差转成「机构吸收」。刚性爪 + 金属件几乎没有余量。evidence: [T03-S018]
   - 跳过会怎样：把机构能吃掉的误差交给算法去解，成本高十倍且不稳。
6. **写出验收测法**（角色：质量）。规定在哪些位姿、测多少次、按什么统计量判定。工业侧可直接借用 ISO 9283 / GB/T 12642 的测试立方体与「5 个位姿 × 30 次」的做法。evidence: [T06-S006, T06-S089, T03-S053]
   - 跳过会怎样：验收时双方对「精度」定义不一致。

**资深路径（差异点）**

- `skip` 资深人跳过「做机器人运动学（绝对精度）标定」——只要能改成相对路线就不做，因为运动学标定要专用设备、有效期短、温度一变就漂。只有在必须离线编程或必须绝对定位（如大型构件加工）时才做。
- `optimize` 把相机的**预热**写进流程：需要紧公差（供应商给的口径是每米工作距离小于 5 mm 级别的容差）的应用要先让相机热稳定再标定与作业。evidence: [T03-S019]
- `optimize` 手眼标定的位姿**分布**比次数更重要——姿态角要拉开、平移要覆盖工作区域，而不是原地小幅动几下多采几组。evidence: [T03-S020, T03-S022]
- `add` 额外做「热机测试」：连续跑 2–4 小时后重测精度，看漂移是否在预算内。初学者只在冷机时验收。
- `add` 额外做「抓取后位姿不确定性」的实测：件被夹起来之后会不会在爪里转/滑，这一项经常比视觉误差还大。

**判断这一步是否通过（具体标准）**

- 误差预算表里每一项都有**数值**与**来源**（供应商规格 / 实测 / 保守假设），没有「忽略不计」而不给理由的项。
- 合成后的总误差 ≤ 工艺容差的一半（留一倍余量）——这是本轨从视觉供应商「刚性爪+金属件几乎没有余量」的表述做出的工程判断，**不是标准规定**。evidence: [T03-S018]
- 验收测法写清了位姿数、重复次数、统计量。evidence: [T06-S006]

**常见失败模式**

- **把 repeatability 当 accuracy 用**（本行第一号外行破绽）。破解：任何精度数字都追问「重复性还是绝对精度？按 ISO 9283 在什么条件下测的？」evidence: [T06-S044, T06-S006]
- **相机 precision 好就以为 trueness 好**：点云噪声小不代表尺度与形状忠实；bin picking 里 trueness 误差直接变成抓偏。evidence: [T03-S018]
- **手眼标定只采 5 组就收工**：工具最少样本数（MoveIt 默认 5 组即可求解）是**能算**的下限，不是**能用**的下限。evidence: [T03-S016, T03-S020]
- **忽略工件在爪内的二次误差**：装配阶段才发现每次插入都偏，误以为是视觉问题。

**时间与人力量级**

- 入门 SOP：3–5 天（含供应商咨询），1 名视觉 + 0.5 名机械。
- 资深路径：1 天出表，剩下的时间花在实测两三项关键误差源。
- **口径说明**：无公开一手统计；量级为本轨基于供应商工作流文档的推断。evidence: [T03-S019]

**近期变化（近 12 个月）**：**无重大变化（本工作流稳态）**。ISO 9283:1998 至今未大改，GB/T 12642-2013 仍现行，2024 年新增的 GB/T 20868-2024《工业机器人 性能试验应用规范》属于试验应用层的补充而非方法学改动。最近一次显著变化是 2024 年 GB/T 20868 换版。触发事件类型：标准更新。evidence: [T06-S006, T06-S048, T06-S054, T03-S053]

- **Last_updated**: 2026-09-02（复核日；方法学本身 1998 至今稳定）
- **Decay risk**: low
- **关键工具**：3D 相机供应商的精度文档与投产前准备流程（Zivid / Cognex 等）、ISO 9283 测试立方体实操口径（RoboDK 文档）。evidence: [T03-S018, T03-S019, T03-S021, T06-S089]



### 4. 环境搭建与标定（手眼、工件坐标系、力传感器、重复性验收）

- **One-liner**：从「硬件装好了」到「所有坐标系互相对齐、传感器读数可信、重复性有实测报告」——之后的所有算法工作才有意义。
- **属于哪一类流程**：两边都有。手眼标定在开源工具链里有完整公开流程（MoveIt）；工件坐标系、力矩标定与重复性验收在厂商手册与标准里。
- **Trigger**：本体、相机、末端工装、安全件都已装配到位，准备开始编程或采数据。evidence: [T03-S016]
- **Output**：一份标定包（相机内参 + 手眼外参 + 工件/工装坐标系 + 工具 TCP + 负载与重心参数 + 力/力矩零偏与重力补偿参数）+ 一份重复性与精度实测报告 + 一份「什么时候必须重标」的触发清单。evidence: [T03-S016, T03-S020, T06-S089]

**入门 SOP（7 步）**

1. **相机内参标定**（角色：视觉工程师）。输出：内参与畸变系数 + **重投影误差**统计。
   - 跳过会怎样：外参标定把内参误差吸收进去，换个工作距离就全错。evidence: [T06-S085]
2. **手眼标定**（角色：视觉工程师）。eye-in-hand（相机装在末端）或 eye-to-hand（相机固定看机器人）。流程：贴/放标定靶 → 机器人走到若干位姿 → 每个位姿同时记录「末端在基座下的位姿」与「靶在相机下的位姿」→ 求解 AX=XB。MoveIt 的手眼标定插件在采到 **5 组**样本后即可求解，默认用 Daniilidis 解算器。evidence: [T03-S016, T03-S017]
   - 跳过会怎样：视觉给出的位姿在机器人坐标系里是错的，整套抓取无从谈起。
   - **注意**：5 组是数学下限。工程上要靠位姿的姿态与平移分布拉开来降低噪声，供应商文档明确把「旋转与平移的运动范围」列为影响标定精度的因素。evidence: [T03-S020, T03-S022]
3. **TCP（工具中心点）与负载/重心标定**（角色：机械/调试工程师）。多数厂商控制器有内置的多点法 TCP 标定与负载辨识向导，国内厂商手册里同样有这一节。evidence: [T03-S055, T03-S056]
   - 跳过会怎样：轨迹在末端偏移；力控与碰撞检测因负载参数错误而误触发或不触发。
4. **工件/工装坐标系建立**（角色：调试工程师）。三点法或用定位销/基准面。输出：工件系相对基座系的变换。
   - 跳过会怎样：换一批工装或工装被撞过之后，程序全部要重教。
5. **力/力矩传感器标定与重力补偿**（角色：控制工程师，仅力控应用）。零偏、温漂、工具重力与重心补偿；标定后要在多个姿态下验证「空载读数接近零」。
   - 跳过会怎样：一改姿态力读数就漂，力控阈值只能放很松，等于没有力控。
6. **重复性/精度实测验收**（角色：质量）。按 ISO 9283 / GB/T 12642 的方法：在工作空间最大内接立方体上取 5 个位姿、每个位姿 30 次，重复性按到质心平均距离加 3 倍标准差计。evidence: [T06-S006, T06-S089]
   - 跳过会怎样：出问题时无法判断是硬件退化还是算法问题——没有基线。
7. **写「重标触发清单」并交给现场**（角色：调试工程师）。典型触发：撞机、换末端、换相机或镜头、拧过相机支架、大修、环境温度显著变化、精度巡检超差。
   - 跳过会怎样：现场撞过一次机之后继续用旧标定，良率悄悄掉。

**资深路径（差异点）**

- `skip` 资深人在**只做相对定位**（视觉在抓取点附近二次定位 / 视觉伺服）的方案里跳过机器人运动学标定与高精度手眼标定，只求把误差压到「够二次定位收敛」的量级。
- `optimize` 标定顺序固定为「内参 → 手眼 → TCP → 工件系 → 力传感器」，且每一步都单独出残差数字；一旦某步残差异常就停住，不往下走。初学者习惯一口气做完再看结果。
- `optimize` 标定位姿用脚本自动生成并覆盖实际作业区域（而不是手动示教几个点），并把标定脚本纳入版本管理，做到可复现。
- `add` 额外做**热机后复标**：设备预热后再采一组，比较冷/热两套外参的差；供应商明确建议紧公差应用要做相机预热。evidence: [T03-S019]
- `add` 额外做**标定的验证任务**（不是只看残差）：用标定结果去抓一个已知位置的标准件 N 次，测末端落点分布。残差小但落点偏，说明有系统性误差没被建模。

**判断这一步是否通过（具体标准）**

- 内参重投影误差、手眼残差都有具体数字并记录在案（数字量级随相机与靶而变，本轨不给通用阈值——**无公开一手统一阈值**）。
- 重复性实测按 ISO 9283 / GB/T 12642 方法完成，有报告。evidence: [T06-S006, T06-S048]
- 空载力读数在多姿态下接近零（力控应用）。
- 标定包可一键复现：脚本 + 数据 + 结果都在版本库里。
- 「重标触发清单」已交付并被现场签收。

**常见失败模式**

- **只采 5 组样本、位姿分布集中**：残差看着小，换个工作区域就偏。破解：位姿覆盖实际作业区、姿态角拉开、样本数远超求解下限。evidence: [T03-S016, T03-S020]
- **标定靶不平/靶尺寸录错**：整套外参有系统性偏置。破解：先用已知距离验证靶的尺度。
- **相机支架不刚**：标定当天好，一周后偏。破解：把支架刚度与是否被人碰过列入巡检项。
- **标定与作业的温度状态不同**：冷机标定、热机作业。evidence: [T03-S019]
- **没有基线报告**：后期良率下降时无法判断是不是标定退化。evidence: [T06-S006]

**时间与人力量级**

- 入门 SOP：1–3 天（首次，含返工），1 名视觉 + 1 名调试。
- 资深路径：半天（脚本化之后），标定 + 验证 + 出报告。
- **口径说明**：无公开一手统计；量级为本轨从工具文档流程步骤数与实操环节做的推断。evidence: [T03-S016]

**近期变化（近 12 个月）**：**无重大变化（本工作流稳态）**。手眼标定的方法学自 1980–90 年代确定，工具链（MoveIt 手眼标定插件、厂商内置向导）近年只有易用性改进。最近一次值得记的变化是标定工具从「自研脚本」普遍转向「厂商向导 + 开源插件」，时间上早于 12 个月窗口。触发事件类型：无。evidence: [T03-S016, T03-S017]

- **Last_updated**: 2026-09-02（复核日）
- **Decay risk**: low
- **关键工具**：MoveIt 手眼标定（必备）、厂商控制器内置 TCP/负载辨识向导（必备）、Zivid/Cognex 等供应商的标定指引（场景特化）。evidence: [T03-S016, T03-S020, T03-S021, T03-S055]



### 5. 仿真环境与资产准备（建模到什么程度就够）

- **One-liner**：从「CAD 与真机」到「一个能跑、能并行、且在**你关心的那几个量**上与真机对得上的仿真环境」——同时明确列出哪些东西仿真里永远不要信。
- **属于哪一类流程**：论文流程为主（并行仿真与域随机化有大量公开工作），但「建到什么程度就够」这条判断几乎只在工具文档与工程实践里。
- **Trigger**：要用学习路线（RL/IL）、要做离线编程与节拍验证、或要在硬件到货前先开工。evidence: [T03-S040, T03-S042]
- **Output**：可复现的仿真工程（机器人模型 + 场景资产 + 传感器配置 + 随机化配置 + 评测脚本）+ 一份「仿真可信 / 不可信」清单。evidence: [T03-S042, T03-S046]

**入门 SOP（6 步）**

1. **明确仿真要回答什么问题**（角色：算法负责人）。三类目的完全不同：①训练策略（要快、要能并行、接触保真度重要）②验证节拍与可达性（要几何准确，物理可以粗）③做数字孪生（要与真机数据同步，照 CAD 建的静态仿真不算数字孪生）。evidence: [T06-S044]
   - 跳过会怎样：拿一个为节拍验证建的模型去训练接触密集的装配策略，怎么调都迁不过去。
2. **准备机器人模型**（角色：仿真工程师）。URDF/MJCF → USD 的转换在 Isaac Lab 有官方转换器；导入时要处理惯量张量、质量、关节驱动增益、碰撞几何。evidence: [T03-S046, T03-S047]
   - 跳过会怎样：零质量/非法惯量之类的问题会让仿真「能跑但物理不对」，且很难事后定位。evidence: [T03-S085]
3. **做碰撞体简化**（角色：仿真工程师）。视觉网格可以高面数，碰撞网格必须简化：凸包、包围盒、基本体，或用凸分解（VHACD / CoACD）得到多个凸块。直接拿视觉网格做碰撞既慢又容易不稳。evidence: [T03-S085, T03-S084, T03-S086]
   - 跳过会怎样：仿真步长被迫调小、并行数上不去、接触求解发散或穿模。evidence: [T06-S044]
4. **配传感器与观测**（角色：仿真工程师）。相机内参、噪声、帧率、延迟要与真机一致；观测里不要塞真机拿不到的特权信息（除非明确走 teacher-student 特权学习路线）。evidence: [T06-S044, T04-S057]
   - 跳过会怎样：策略在仿真里用了真机没有的信息，迁移必然失败。
5. **做最小系统辨识**（角色：控制工程师）。至少辨识：关节摩擦/阻尼、执行器延迟与力矩上限、传动柔性。腿足领域的通行做法是训练一个 actuator network 来拟合真实执行器的非线性响应（把真机记录的关节数据拿去拟合 MLP）。evidence: [T03-S043, T04-S055]
   - 跳过会怎样：域随机化的范围只能瞎放大，训练更难且仍然迁不过去。
6. **写「仿真不可信清单」**（角色：算法负责人）。典型条目：摩擦系数与接触刚度、软体与线缆、抓取时的滑移、相机在真实光照与反光下的表现、电机热衰减、连接器/线束干涉。
   - 跳过会怎样：团队会拿仿真成功率当能力证据——本行明确拒绝这种做法。evidence: [T06-S044]

**资深路径（差异点）**

- `skip` 资深人跳过「把整条产线建进仿真」：只建与接触/可达性直接相关的那一小块，其余用基本体代替。理由是保真度的边际收益在非接触区域几乎为零，而资产工时是线性成本。
- `skip` 在**纯位置控制、来料确定**的传统方案里，资深人完全跳过物理仿真，只用离线编程软件做可达性与节拍验证。
- `optimize` 先做系统辨识再定域随机化范围（而不是先随机化再调），把随机化中心放在辨识值上、范围放在辨识不确定度上。evidence: [T03-S043]
- `optimize` 把「资产准备」做成流水线：CAD 清理 → 单位/坐标系统一 → 碰撞体生成 → 物理属性补全 → 校验（质量、惯量、坐标系可视化），每一步可脚本重跑。evidence: [T03-S085]
- `add` 额外做「仿真–真机一致性测点」：选 3–5 个可在两边都测的量（如给定力矩下的关节响应、给定轨迹下的末端落点、抓取滑移距离），每次改仿真参数都比一遍。这是把「sim2real gap」从形容词变成数字的唯一办法。

**判断这一步是否通过（具体标准）**

- 仿真工程能一条命令复现（模型 + 资产 + 配置 + 随机种子都在版本库）。
- 碰撞体经过简化并可视化检查过，接触没有明显穿模。evidence: [T06-S044]
- 一致性测点上仿真与真机的偏差被量化并记录（数值目标随任务而变，本轨不给通用阈值）。
- 「不可信清单」写下来了，且团队里每个人都知道。

**常见失败模式**

- **建模精度往「像不像」上使劲，而不是往「接触对不对」上使劲**：渲染很漂亮，接触参数没辨识过。
- **用视觉网格当碰撞体**：并行数上不去，训练慢十倍。evidence: [T03-S085, T03-S084]
- **仿真里能拿到真值位姿**：策略学会依赖真值，真机没有。
- **报仿真成功率当能力证据**（本行第十号破绽）：内行只会问真机 N 次里成功多少、sim2real 掉了多少。evidence: [T06-S044]
- **把离线编程仿真叫「数字孪生」**：中文产业语境里这个词已被泛用到失去含义。evidence: [T06-S044]

**时间与人力量级**

- 入门 SOP：新本体 + 新场景，1–3 周（资产清理与物理参数占大头），1 名仿真 + 0.5 名控制。
- 资深路径：复用已有本体资产时 2–5 天。
- **口径说明**：无公开一手统计；量级为本轨从资产准备文档描述的步骤数与常见返工点做的推断。evidence: [T03-S085, T03-S047]

**近期变化（近 12 个月）**：GPU 并行仿真已从「研究技巧」变成默认基础设施——Isaac Lab 提供了从训练到 ROS 部署的官方参考架构与端到端示例（如 UR10e 齿轮装配从 Isaac Lab 训练到 Isaac ROS 部署），把过去要自己拼的 sim2real 链路变成了有文档的工作流；框架论文于 2025-11 公开。触发事件类型：新工具。evidence: [T03-S040, T03-S041, T03-S042, T03-S045]

- **Last_updated**: 2025-11（Isaac Lab 框架论文）
- **Decay risk**: high（仿真栈与资产格式 12 个月内仍在快速演化）
- **关键工具**：Isaac Lab / Isaac Sim（必备，GPU 并行与 USD 资产）、MuJoCo（必备，接触与轻量实验）、URDF/MJCF→USD 转换器（必备）、VHACD / CoACD 凸分解（必备）。evidence: [T03-S040, T03-S046, T03-S084, T06-S076, T06-S077]



### 6. 方案开发：传统路线 / 学习路线 / 混合分层架构

- **One-liner**：从「标定好的硬件 + 明确的任务」到「一个能重复完成任务的系统」。有两条正统路线和一条现实里最常见的混合路线，**它们的 SOP 不一样，验收方式也不一样**。
- **属于哪一类流程**：传统路线在教科书与工具文档里完整公开；学习路线在论文与开源仓库里公开；**混合分层架构公开材料最薄**——它主要活在厂商产品与交付项目里，本轨只能从产品文档与公开表述反推，如实标注。
- **Trigger**：标定完成、仿真或真机可用，进入功能开发。evidence: [T03-S041]
- **Output**：可重复运行的任务程序或策略 + 一份说明「哪一段是自主的、哪一段是脚本/规则、哪一段有人兜底」的架构图。evidence: [T06-S044]

#### 6A. 传统路线 SOP（感知 → 位姿 → 规划 → 控制）

1. **感知与位姿估计**（角色：视觉工程师）：分割/检测 → 6D 位姿或抓取位姿检测 → 位姿置信度输出。跳过置信度输出会怎样：系统无法区分「没看到」和「看错了」，异常处理无从写起。evidence: [T06-S044]
2. **抓取/接触点规划**（角色：视觉/工艺）：从位姿到可执行的抓取位姿（含避碰与后续装配可行性）。**产线要的是 task-oriented grasp——抓起来且能完成后续装配位姿，不是抓起来不掉。** evidence: [T06-S044]
3. **运动规划**（角色：软件工程师）：采样式（RRT/PRM 系）或优化式（轨迹优化）规划，加上速度/加速度限制与避奇异。跳过奇异处理会怎样：现场随机报警，被当成「设备故障」。evidence: [T06-S044]
4. **控制与顺应**（角色：控制工程师）：纯位置控制够不够？需要阻抗/导纳还是力/位混合？可反驱性决定了力控能不能做。跳过会怎样：装配阶段一直卡死或压坏件。evidence: [T06-S044]
5. **异常分支**（角色：软件工程师）：没看到、看错、抓空、掉件、卡料、超力、超时，各自的恢复动作。跳过会怎样：产线一有异常就停线等人。

#### 6B. 学习路线 SOP（数据 → 策略 → 评测）

1. **定任务与观测/动作空间**（角色：算法负责人）：相机布置、动作是关节位置还是末端位姿增量、控制频率、动作分块长度。跳过会怎样：采完几万条数据才发现观测里缺了关键视角，数据作废。
2. **采数据**（角色：数据采集团队）→ 见工作流 7。
3. **选策略族并训练**（角色：算法工程师）：行为克隆系（ACT / Diffusion Policy）、VLA 微调（π0 / OpenVLA / SmolVLA 等）。开源 VLA 的通行做法是「预训练大模型 + 用自己平台的小数据后训练」。evidence: [T03-S035, T03-S033, T03-S038]
4. **仿真或离线评测做粗筛**（角色：算法工程师）：只用于淘汰明显不行的 checkpoint，不作为结论。evidence: [T06-S044]
5. **真机评测**（角色：评测负责人）→ 见工作流 9。**这一步的严谨程度决定了整条路线是不是在自欺欺人。**

#### 6C. 混合分层架构（现实中最常见）

- 典型分层：**上层用大模型/规则做任务理解与分解 → 中层用学习策略或传统规划做技能执行 → 底层是传统的位置/力控伺服环 + 独立的安全层（限速、限力、避障、急停）**。
- 这个分层与国内政策文件里的「大脑 / 小脑 / 肢体」表述对得上：政策语境里的「大脑」= 任务理解与规划层。evidence: [T06-S042, T06-S044]
- **底层安全层永远不由神经网络单独承担**：把视觉模型当唯一的人体检测来放行人员进入危险区，当前没有任何已发布标准支持。evidence: [T06-S044]
- **端到端不等于没有保护层**：绝大多数落地系统在网络下面仍有限速、限力、避障与安全通道。evidence: [T06-S044]
- **公开材料稀薄声明**：分层怎么切、接口怎么定、上层多久出一次指令，这些几乎没有可引用的一手工程文档；本节的描述来自政策文件的分层表述 + 厂商话术的工程还原，**不是从某一家的交付文档里读到的**。

**资深路径（差异点）**

- `skip` 资深人在**来料确定、任务固定**的工位上直接跳过学习路线，用传统路线两周做完——并且会明确告诉客户「这里上 VLA 没有收益」。
- `skip` 资深人跳过「先做一个大而全的通用策略」：先把任务切到能在一两周内闭环的最小粒度。
- `optimize` 先写异常分支再写正常流程：正常流程谁都能写，产线的稳定性全在异常分支里。
- `optimize` 学习路线优先做**后训练**而不是从零训练：开源 VLA 权重可用之后，用自己平台的小数据微调是默认路径。evidence: [T03-S034, T03-S033]
- `add` 额外做「架构诚实图」：一张图标清哪一段自主、哪一段规则、哪一段有人兜底、干预点在哪。对外汇报和对内排障都靠它。evidence: [T06-S044]
- `add` 额外做「回退路径」：策略失败时退回到传统规划或退回到人工工位，而不是停线。

**判断这一步是否通过（具体标准）**

- 系统能在无人干预下连续完成 N 次（N 由工作流 9 的评测协议定），且每次失败都被自动分类记录。
- 每一类异常都有明确的恢复动作，且恢复动作本身被测过。
- 架构图里「自主 / 规则 / 人工兜底」三色分明，没有含糊地带。evidence: [T06-S044]
- 安全层独立于算法层，且不依赖任何神经网络的输出作为唯一判据。evidence: [T06-S044]

**常见失败模式**

- **用学习路线去解一个工装问题**：来料乱 → 采数据 → 泛化不了 → 采更多数据。正确做法是回到工作流 1 第 2 步改工装。
- **抓取只按 force closure 设计**，抓起来了但姿态不对，后续装配做不了。evidence: [T06-S044]
- **把「端到端」当成不需要安全层**。evidence: [T06-S044]
- **只做正常流程的 demo**：能连续跑 10 次，跑 8 小时就崩——因为没有异常分支。evidence: [T06-S044]
- **中途换观测/动作空间**：已采的数据全部作废，这是学习路线最贵的一次返工。

**时间与人力量级**

- 传统路线（单工位、来料确定）：入门 2–6 周；资深 1–2 周。
- 学习路线（单任务、已有平台与开源权重）：数据采集另计，微调训练本身在单张 A100 上约 4 小时 / 2 万步（SmolVLA 官方口径）；π0 全量微调需要 >70 GB 显存（A100 80G / H100），LoRA 微调 >22.5 GB（如 RTX 4090），推理 >8 GB。evidence: [T03-S038, T03-S033]
- **口径说明**：显存与训练时长是**厂商/项目文档的一手数字**；「2–6 周」是本轨对交付节奏的量级推断，**无公开一手统计**。

**近期变化（近 12 个月）**：开源 VLA 权重与配套微调工具链已经成熟到「默认从后训练起步」——Physical Intelligence 开源 π0 / π0.5 权重与 openpi 仓库（含数据转 LeRobot 格式 → 计算归一化统计 → 训练 → 起策略服务器的三步流程），Hugging Face 侧把 π0 移植进 LeRobot 并提供 SmolVLA 这类消费级 GPU 可训的基座。**结果是学习路线的入场门槛从「自己搭训练栈」变成「跑三条命令」**，工作重心整体前移到数据与评测。触发事件类型：新模型 + 新工具。evidence: [T03-S033, T03-S034, T03-S037, T03-S038, T03-S039]

- **Last_updated**: 2026-09-02（openpi / LeRobot 文档复核日）
- **Decay risk**: high
- **关键工具**：openpi（新兴→必备）、LeRobot（必备）、MoveIt / OMPL（传统路线必备）、Isaac Lab（学习路线必备）。evidence: [T03-S033, T03-S038, T04-S025, T04-S026]



### 7. 数据采集与训练循环（遥操作的人力成本与停止条件）

- **One-liner**：从「决定走学习路线」到「一批可训练、可复现、知道自己缺什么的数据 + 一条能持续迭代的训练循环」，并且知道**什么时候该停止采数据**。
- **属于哪一类流程**：论文与开源项目公开得相当充分（DROID / UMI / LeRobot / openpi），但**采集的人力组织与单位成本几乎全部闭源**，中国侧只有媒体转述数字，本轨如实标注。
- **Trigger**：任务已定、观测/动作空间已冻结、平台可稳定运行。evidence: [T03-S012]
- **Output**：带元数据的数据集（任务标签、场景、物体、采集员、成功/失败标记、时间戳对齐）+ 数据质量报告 + 训练好的策略 + 一份「下一批该采什么」的清单。evidence: [T03-S012, T03-S038]

**入门 SOP（7 步）**

1. **先冻结采集协议再采第一条**（角色：数据负责人）。DROID 的做法是用一份共享采集协议来统一 13 个机构、50 名采集员、18 套完全相同的硬件（Franka Panda + Robotiq 2F-85 + 两台桌面 ZED 2 + 一台腕部 ZED Mini），协议专门用来防止「相机看不见机器人」「采集员入镜」这类常见错误。evidence: [T03-S012, T03-S077]
   - 跳过会怎样：采完发现相机位姿每台不一样、有人入镜、时间戳没对齐——数据不能合并训练。
2. **先采 20–50 条做贯通测试**（角色：数据负责人 + 算法）。走完「采集 → 转格式 → 训练 → 部署 → 真机跑一次」的完整链路。
   - 跳过会怎样：采了几千条才发现动作空间定义错了，全部作废——这是学习路线最贵的返工。
3. **按「变化维度 × 每维重复次数」排采集计划**（角色：数据负责人）。LeRobot 官方给 SmolVLA 的起步建议是**约 50 条 episode**，示例是 **5 个不同物体位置 × 每个位置 10 条**；同一文档明确记录了 **25 条不够、效果很差**。evidence: [T03-S038]
   - 跳过会怎样：条数堆上去但全是同一初始状态，策略只会背轨迹。
4. **边采边做质量筛查**（角色：数据运营）。宇树的「机器人数据运营工程师」岗位职责把这条写得很直白：负责数据采集、清洗、审核、标注、归档、上传全流程，**制定采集规范、质量评估标准与数采员培训教程**，并处理采集过程中的硬件异常与通信故障。另设「具身数据评估工程师」负责自动化数据筛选、难例挖掘与负样本生成。evidence: [T03-S058]
   - 跳过会怎样：废数据混进训练集；而在手持夹爪（UMI 类）路线上，公开报道提到过「一周的采集可能大半是废数据」的情况（**媒体转述，非一手**）。evidence: [T03-S072]
5. **训练与配比**（角色：算法工程师）。当前默认路径是「大规模预训练 + 小规模后训练」：π0 的配方是先在跨本体大数据上预训练，再用小批高质量数据后训练到具体任务；openpi 的官方口径是**用自己平台 1–20 小时的数据微调即可覆盖多种任务**。evidence: [T03-S035, T03-S033, T03-S034]
   - 跳过会怎样：从零训练需要的数据量高一个数量级以上。
6. **真机评测并回填**（角色：评测负责人）→ 工作流 9。把失败案例转成下一批采集的目标场景。
   - 跳过会怎样：采集变成开环，数据越采越多但成功率不动。
7. **决定停止条件**（角色：算法负责人）。见下面「什么时候该停止采数据」。

**什么时候该停止采数据（本轨的判断规则，来源见下）**

- **数据加倍但真机成功率的置信区间重叠** → 停。继续采只是在买噪声；判定要用严谨的对比方法（见工作流 9 的序贯检验）。evidence: [T03-S002, T03-S009]
- **失败集中在同一类原因**（如某个视角看不到、某种反光材质、某个卡料姿态）→ 停止「泛采」，改成**定向补采**那一类，或干脆改工装/改相机位置。
- **失败原因是硬件或标定**（抓不稳、力控带宽不够、相机看不见）→ 停止采数据，回到工作流 3/4。**这是最常被忽略的一条：数据补不了硬件的账。**
- **策略在训练集分布内已经很好、只在新物体/新场景掉** → 该采的是**多样性**（新场景/新物体），不是同一场景的更多条数。DROID 的做法就是每个场景采到一定量就换场景。evidence: [T03-S012]
- **单位成本已高于替代方案**：如果一小时有效数据的成本乘以还需要的小时数，超过了改造工装/换方案的成本，就该换路线。国内公开报道给出的口径是「单小时有效数据成本仍在 500 元以上」（智元遥操作方案，**媒体转述，非一手，不要当行业均值**）。evidence: [T03-S072]

**采集方式的三条路线与代价**

| 路线 | 代表 | 好处 | 代价 |
|---|---|---|---|
| 真机遥操作 | DROID（VR 手柄）、ALOHA/Mobile ALOHA（双臂主从） | 动作与本体严格对齐，可直接训 | 要占用真机、要人、要场地；本体一改数据贬值 |
| 手持采集器（无本体） | UMI（手持夹爪 + GoPro） | 不占机器人、能在真实野外场景采、硬件便宜 | 推理时才出现的传感/推理/执行延迟必须在策略接口里显式补偿；采集器与真机的运动学差异要处理 |
| 人体动作/第一人称视频 | 数据手套、Ego 类视频 | 采集速度最快、场景最真实 | 缺关节级动作与力信息，映射到本体损失大 |

evidence: [T03-S012, T03-S013, T03-S014, T03-S015, T04-S079, T04-S080]

**资深路径（差异点）**

- `skip` 资深人跳过「先建大数据集再训练」：先跑通最小闭环，再按评测结果定向补采。
- `skip` 资深人跳过「自己从零训练」：默认从开源权重后训练起步。evidence: [T03-S034]
- `optimize` 把采集规范、采集员培训、质量抽检做成固定岗位与固定流程（而不是让算法工程师兼职），这正是头部公司把它单列成岗位的原因。evidence: [T03-S058]
- `optimize` 元数据比数据本身更重要：采集员 ID、场景 ID、物体 ID、光照、成功/失败、干预标记都要在采集时就写进去，事后补不回来。
- `add` 额外做「负样本与难例挖掘」：把失败轨迹保留并标注，用于失败检测与难例定向补采。evidence: [T03-S058, T03-S050]
- `add` 额外做「数据贬值评估」：本体、末端、相机位置一改，历史数据的可用性要重新评估——这是学习路线里最容易被低估的沉没成本。

**判断这一步是否通过（具体标准）**

- 每条轨迹都能追溯到：谁采的、什么场景、什么物体、成功还是失败、是否有干预。
- 数据集能一条命令转成训练格式并复现出一个已知性能的 checkpoint。evidence: [T03-S033]
- 有一份「下一批采什么」的清单，且清单来自真机评测失败分类，不是来自感觉。
- 训练与评测用的数据严格不重叠（场景/物体/采集员层面切分，不是随机切分）。

**常见失败模式**

- **只报条数不报多样性**（本行第 15 号破绽）：「我们采了 10 万条」而答不出多少任务、多少场景、多少物体、几个采集员、成功轨迹占比、平均时长。evidence: [T06-S044]
- **把小时数当有效数据**：采集小时 ≠ 有效小时 ≠ 训练可用小时，三个口径要分开报。
- **中途改硬件/改相机位置**：历史数据贬值，且经常没人算这笔账。
- **用数据补硬件的账**：抓不稳就多采，实际该换爪或加力控。
- **随机切分做验证集**：同一场景的相邻帧同时进训练与验证，指标虚高。

**时间与人力量级**

- **有公开一手数字的**：DROID 用 **12 个月**、**50 名采集员**、**13 个机构**、**18 套相同硬件**采到 **7.6 万条轨迹 / 350 小时交互 / 564 个场景 / 86 类任务**；由此可推算平均每条轨迹的**交互**时长约 16–17 秒（本轨用 350 小时 ÷ 76,000 条推得，**是交互时长不是人力工时**，不含场景搭建、复位、失败重采与清洗）。evidence: [T03-S012, T03-S088, T05-S033]
- TRI 训练 LBM 用了约 **1,700 小时**机器人数据。evidence: [T03-S010]
- SmolVLA：**约 50 条 episode 起步**；2 万步训练在单张 A100 上约 **4 小时**。evidence: [T03-S038]
- openpi：自有平台 **1–20 小时**数据可微调出多种任务。evidence: [T03-S033]
- **中国侧（媒体转述，非一手，仅作量级参考）**：单小时有效数据成本 500 元以上；数据基地年产能「十几万小时」量级；某电商公司宣称组织十万级员工加五十万级社会人员的采集队伍、目标两年积累千万小时。这些数字**没有第三方验证，口径（有效/原始、含不含清洗）也未公开**。evidence: [T03-S072]

**近期变化（近 12 个月）**：①**采集从实验室行为变成产业行为**——2026-06-03 工信部与国资委联合发文推动「实景实训」，要求用户单位提供作业流程数据与环境语义信息，并构建覆盖「全身运动轨迹、力位控制曲线、操作执行序列」的高质量数据集，各省重点场景不少于 20 个、各央企不少于 10 个。这把「去哪里采数据」从公司自己想办法，变成了有政策通道的资源。evidence: [T05-S048] ②**低成本采集硬件与开源数据格式统一**（LeRobot 数据格式成为事实标准，手持采集器路线成熟），使小团队第一次能在没有大机器人农场的情况下起步。触发事件类型：法规/政策 + 新工具。evidence: [T03-S038, T03-S013]

- **Last_updated**: 2026-06-03（政策）/ 2026-09-02（工具文档复核）
- **Decay risk**: high
- **关键工具**：LeRobot（必备，数据格式与录制）、openpi（必备，后训练）、VR 遥操作套件 / 主从臂 / 手持夹爪（场景特化）。evidence: [T03-S038, T03-S033, T03-S013]



### 8. sim-to-real 迁移与真机调试

- **One-liner**：从「仿真里能跑」到「真机上能跑」，并且知道**什么时候该停止折腾仿真、直接上真机**。
- **属于哪一类流程**：论文与厂商文档公开充分（域随机化、teacher-student、actuator net、并行训练），这是本行少数「论文流程 ≈ 交付流程」的环节。
- **Trigger**：仿真里策略已收敛且通过仿真评测粗筛。evidence: [T03-S040]
- **Output**：能在真机上运行的策略 + 一份「哪些量是靠随机化扛过去的、哪些是靠辨识对齐的」的记录 + 真机评测结果。evidence: [T03-S043]

**入门 SOP（6 步）**

1. **先对齐再随机化**（角色：控制工程师）。做最小系统辨识（关节摩擦阻尼、执行器延迟与力矩上限、传动柔性），把随机化的中心放在辨识值上。腿足领域的标准做法是训练 actuator network：用真机部署时记录的关节数据训练一个 MLP，使其输出的力矩与真实关节位置/速度下的力矩误差最小。evidence: [T03-S043, T04-S055]
   - 跳过会怎样：只能靠把随机化范围放到极大来硬扛，训练更难、策略更保守、迁移仍不稳。
2. **配域随机化**（角色：算法工程师）。原则是**覆盖真机实际会遇到的范围**，不是越大越好——官方文档明确指出随机化范围越大策略越难学，但能容纳更大的输入与系统参数变化。evidence: [T03-S040, T03-S043]
   - 跳过会怎样：策略过拟合到单一仿真参数，真机换一批电机就崩。
3. **观测与时序对齐**（角色：软件工程师）。相机帧率、控制频率、通信延迟、动作执行延迟必须在仿真里建模。UMI 明确处理了这一类问题：手持采集时观测与动作**没有**延迟，而推理时存在传感、推理、执行三类延迟，因此策略接口里要做推理时延迟匹配，并用相对轨迹动作表示。evidence: [T03-S013]
   - 跳过会怎样：仿真里完美的策略在真机上像喝醉了——这是最典型也最容易误诊为「模型不行」的问题。
4. **先跑受限真机测试**（角色：控制 + 安全）：降速、限力、限工作空间、人手放在急停上。
   - 跳过会怎样：第一次真机就撞机、损坏工装或伤人。
5. **量化 gap 并归因**（角色：算法负责人）：在一致性测点上比仿真与真机（见工作流 5 第 6 步的「一致性测点」），把差异归到「动力学 / 感知 / 时序 / 接触」四类之一。
   - 跳过会怎样：只能盲调随机化参数。
6. **决定是继续调仿真还是转真机**（角色：算法负责人）→ 见下面的判据。

**什么时候该放弃仿真、直接上真机（本轨的判断规则）**

- **gap 的主因是接触与柔性**（软体、线缆、粘性、滑移、变形件）→ 转真机。这类正是仿真最不可信的一类，继续调参回报很低。evidence: [T06-S044]
- **gap 的主因是感知**（真实光照、反光、脏污）→ 转真机采数据，或改光源/改相机，不要靠渲染去补。
- **gap 的主因是动力学或时序** → 留在仿真里，做系统辨识与延迟建模，回报很高。
- **仿真里的改动已经连续三轮不再改善真机表现** → 转真机。
- **任务本身是低速、准静态、位置主导** → 传统路线可能根本不需要仿真训练。

**资深路径（差异点）**

- `skip` 资深人跳过「渲染保真度军备竞赛」：除非任务对视觉外观敏感，否则把预算花在动力学与时序对齐上。
- `skip` 在接触密集的装配任务上，资深人直接跳过 sim2real，走真机数据 + 行为克隆或传统力控。
- `optimize` 用 teacher-student（特权学习）：仿真里让 teacher 用特权信息（真值地形、真值状态）学到高水平策略，再蒸馏成只用真机可得观测的 student。这是腿足领域跨越 gap 的主力方法。evidence: [T04-S057, T06-S044]
- `optimize` 随机化范围做成课程（从窄到宽自适应扩张），而不是一开始就全开。evidence: [T06-S044]
- `add` 额外做「首次真机上电清单」：限速值、限力值、软限位、急停可达性、日志开着、有人盯着——写成纸质清单逐项打勾。
- `add` 额外做「真机数据回灌」：把真机上记录的关节响应拿回去改 actuator net / 摩擦模型，形成闭环。evidence: [T03-S043]

**判断这一步是否通过（具体标准）**

- 真机上能在**限速/限力**条件下连续完成任务，且失败模式与仿真中的失败模式一致（不一致说明 gap 归因错了）。
- 一致性测点上的偏差被记录，且每一项都有归因。
- 「靠随机化扛过去」与「靠辨识对齐」两类被分开记录——前者是脆弱性来源，换硬件批次要重测。
- 真机评测按工作流 9 的协议做，**不用仿真数字替代真机数字**。evidence: [T06-S044]

**常见失败模式**

- **报仿真成功率当结论**（本行第十号破绽）。破解：真机 N 次里成功多少、sim2real 掉了多少，两个数字都要给。evidence: [T06-S044]
- **随机化范围一把开到最大**：策略学到极度保守的行为，节拍完全不达标。evidence: [T03-S040]
- **忽略延迟**：把时序问题误诊为策略能力问题，然后去加数据。evidence: [T03-S013]
- **观测里混进特权信息**：仿真无敌、真机瞎跑。evidence: [T04-S057]
- **第一次真机不降速**：撞机损失几天到几周。

**时间与人力量级**

- 入门 SOP：新任务 1–4 周（大部分时间在辨识与延迟对齐上），1 名算法 + 1 名控制。
- 资深路径：已有本体与辨识结果时 2–5 天。
- **口径说明**：无公开一手统计；量级为本轨从官方 sim2real 教程的步骤复杂度做的推断。evidence: [T03-S041, T03-S043]

**近期变化（近 12 个月）**：sim2real 从「每家自己拼」变成「有官方参考路径」——Isaac Lab 把「仿真训练（含域随机化）→ 真机部署（Isaac ROS）」写成了带完整示例的官方工作流（UR10e 齿轮装配、Spot 四足运动），并公开了参考架构；框架论文 2025-11 公开。同时**评测侧出现了 real-to-sim 路线**（用高斯泼溅等方法把真实场景重建进仿真做策略评测），使「用仿真做评测」这件事第一次有了可量化可信度的方法，但**仍不能替代真机数字**。触发事件类型：新工具 + 新方法。evidence: [T03-S040, T03-S041, T03-S043, T03-S045, T03-S007, T03-S079]

- **Last_updated**: 2025-11（Isaac Lab 论文）/ 2026-09-02（文档复核）
- **Decay risk**: high
- **关键工具**：Isaac Lab（必备）、MuJoCo（必备）、actuator network 训练脚本（场景特化）、Isaac ROS（部署）。evidence: [T03-S040, T03-S043, T06-S076]



### 9. 评测协议设计与「怎么读别人的评测」

- **One-liner**：从「感觉它变好了」到「一份别人能复现、能反驳、带不确定度的结论」。**这是本行最能区分专业与业余的一步，也是最大的一笔糊涂账所在。**
- **属于哪一类流程**：论文流程近 18 个月才成型（评测方法学本身正在成为一个研究方向）；交付侧的验收评测另有一套（见工作流 13）。
- **Trigger**：要回答「A 比 B 好吗」「能不能上线」「客户验收能不能过」中的任意一个。evidence: [T03-S002, T03-S009]
- **Output**：一份评测报告，含任务集定义、初始状态随机化范围、试验次数、判定标准、干预记法、统计量与不确定度、原始逐次记录。evidence: [T03-S002, T03-S009, T06-S044]

**入门 SOP（8 步）**

1. **定任务集与判定标准**（角色：评测负责人）。每个任务写清「成功=什么」（例如：完整放入托盘且未倾倒），二值判定要能由不知情的第三人复判。
   - 跳过会怎样：成功的定义在评测中途漂移，数据不可比。
2. **定初始状态随机化范围并写下来**（角色：评测负责人）。例如「物体位置在 30×30 cm 内均匀随机，姿态随机 ±180°，光照两档」。
   - 跳过会怎样：得到的是「摆好位置能做」的成功率，换个摆法就崩——这是 demo 与工程的分界线。evidence: [T06-S044]
3. **定试验次数并预先声明**（角色：评测负责人）。真机评测的现实约束是样本量小：公开研究指出策略比较的可行样本量常在**10 或 50 的量级**，操作研究中**典型只做 20–30 次真机试验**。evidence: [T03-S002]
   - 跳过会怎样：跑到看着好就停（optional stopping），结论没有统计意义。
4. **定干预记法——这一条最重要**（角色：评测负责人）。必须把下面几类分开记：
   - **完全自主成功**（无人接触、无人遥操作、无人重摆物体）
   - **有人介入后成功**（记录介入类型：物理帮一把 / 遥操作接管 / 重置场景 / 重启程序）
   - **失败**（再分为可恢复失败与破坏性失败：撞件、划伤、掉件）
   - **「有人接管」的成功不计入自主成功率**，只计入「带兜底的任务完成率」，两个数字分开报。evidence: [T06-S044]
   - 跳过会怎样：得到一个既不是自主能力也不是系统可用性的混合数字，对谁都没用。
5. **做盲测与配对比较**（角色：评测负责人）。TRI 在 LBM 研究中的做法是引入统计评测框架，在仿真与真机上都做**盲 A/B 测试**；同一份工作里做了约 **1,800 次真机 rollout** 与 **47,000+ 次仿真 rollout**。evidence: [T03-S010, T03-S011]
   - 跳过会怎样：评测者知道哪个是自家新模型，判定会不自觉偏向。
6. **算不确定度，不只报点估计**（角色：评测负责人）。小样本二项比例要给置信区间；比较两个策略要用能控制错误率的方法。近期方法学工作提供了**序贯/随时有效的检验**（安全随时有效推断 SAVI），允许在证据积累够时提前停止，同时保持预先设定的置信水平。evidence: [T03-S002, T03-S008]
   - 跳过会怎样：「85% vs 80%」在 N=20 时毫无意义，却被当成改进。
7. **记录环境与硬件配置**（角色：评测负责人）。硬件型号、相机位置、光照、物体清单、软件版本、标定日期都要记，且**评测环境要可重建**。硬件供应商侧的建议同样是：控制该控制的变量、记录硬件与传感器配置、逐次记录试验。evidence: [T03-S076]
   - 跳过会怎样：三个月后没人能复现这次评测。
8. **公开逐次记录**（角色：评测负责人）。不是只给汇总成功率，要给每次的结果与失败原因分类。
   - 跳过会怎样：无法做失败分析，也无法被别人检验。

**怎么读别人的评测（追问清单）**

1. **分母是多少**？多少次里的百分之多少。evidence: [T06-S044]
2. **初始状态怎么随机**？固定摆位还是随机？范围多大？
3. **允不允许重试**？失败后重来算不算成功？
4. **有没有人在旁**？有没有遥操作兜底、有没有人帮忙复位？自主率是多少？evidence: [T06-S044]
5. **是仿真数还是真机数**？sim2real 掉了多少？evidence: [T06-S044]
6. **泛化是哪一层**？新物体 / 新场景 / 新任务 / 新本体，四层分开说。evidence: [T06-S044]
7. **失败的性质**？可恢复还是破坏性。evidence: [T06-S044]
8. **连续跑多久**？单次成功率之外，8 小时的干预率是多少。evidence: [T06-S044]
9. **视频是第几次拍的**？
10. **评测者是谁**？自家人自评还是第三方/盲测。

**资深路径（差异点）**

- `skip` 资深人跳过「每改一次就跑一次完整评测」：日常用小规模冒烟测试（固定几个初始状态，10 次），只在里程碑节点跑完整协议。
- `optimize` 用配对设计（同一批初始状态、同一批物体摆位，两个策略各跑一遍）来降低方差——同样的试验次数能得到更紧的区间。evidence: [T03-S002]
- `optimize` 用序贯检验决定何时停止，而不是固定跑满 N 次。evidence: [T03-S002, T03-S008]
- `optimize` 用仿真做**粗筛**而不是做结论；近期工作在研究如何用不完美仿真器给出带可靠性保证的评测，但这仍是补充手段。evidence: [T03-S007, T03-S079]
- `add` 额外做**分布式/跨机构评测**：RoboArena 的思路是不做固定基准，而是众包一张评测网络，评测者自选任务与环境，但必须做**成对策略的双盲评测**——用多样性换可比性。evidence: [T03-S003, T03-S004, T03-S005, T03-S080]
- `add` 额外做**失败分类学**：把失败按「感知错 / 规划错 / 控制错 / 抓取错 / 硬件问题 / 场景外」分类，每次评测都出分类分布图——这比总成功率更能指导下一步。
- `add` 额外做**长时评测**：连续 4–8 小时运行，报干预率而不只是单次成功率。evidence: [T06-S044]

**判断一次评测是否合格（具体标准）**

- 报告里同时有：任务定义、随机化范围、N、判定标准、重试规则、干预记法、统计量与不确定度。缺任一项即不合格。evidence: [T06-S044, T03-S002]
- 自主成功率与「带人工兜底的完成率」分开报。evidence: [T06-S044]
- 仿真数字与真机数字分开报，且结论只基于真机。evidence: [T06-S044]
- 逐次原始记录可查。
- 与基线的比较用配对设计或明示为非配对，并给出不确定度。evidence: [T03-S002]

**常见失败模式**

- **无分母成功率**（本行第二号破绽）。evidence: [T06-S044]
- **看着好就停**：optional stopping 使 p 值失效。破解：预先声明 N，或用随时有效的序贯方法。evidence: [T03-S002, T03-S008]
- **把接管后的成功计入自主成功**：本行最大的糊涂账。破解：三分类记法（自主成功 / 介入后成功 / 失败）。evidence: [T06-S044]
- **拿仿真成功率当能力证据**。evidence: [T06-S044]
- **只报二元成功率**：忽略了完成时间、恢复行为、失败严重度等信息；近期方法学工作正是针对「超越二元成功率」的度量做的。evidence: [T03-S008]
- **评测集与训练集在场景/物体上重叠**：泛化被高估。
- **自家人非盲评**。破解：盲 A/B。evidence: [T03-S010]

**时间与人力量级**

- 单任务完整真机评测（N=50、含复位与记录）：**半天到 2 天**，1–2 人。以操作研究常见的 20–30 次真机试验计，人工复位是主要成本项。evidence: [T03-S002]
- 多策略对比（如 4 个 checkpoint × 5 个任务 × 30 次）：**1–2 周**，且必须排班保证环境一致。
- 参考量级：TRI 在一份 LBM 研究里做了约 **1,800 次真机 rollout**——这是工业实验室级别的投入。evidence: [T03-S010]
- **口径说明**：「半天到 2 天」「1–2 周」是本轨的量级推断（**无公开一手统计**）；20–30 次、1,800 次、10/50 量级是一手数字。evidence: [T03-S002, T03-S010]

**近期变化（近 12 个月）**：**机器人评测方法学在近 18 个月里本身变成了一个研究方向**——① 2025-03 起，策略比较的序贯/近最优停止方法被提出并被引用为默认做法之一；② 2025-06 RoboArena 提出分布式双盲成对评测并在 CoRL 2025 正式发表，配套开源基础设施；③ 2025-10 起出现大规模真机评测平台（RoboChallenge）与「用不完美仿真器做可靠评测」的方法；④ 2026 年出现「超越二元成功率」的样本高效比较方法与低成本可复现的真机基准（VLA-REPLICA）。**净效果：只报一个成功率数字的论文与发布会，正在迅速失去说服力。** 触发事件类型：新方法 + 社区规范变化。evidence: [T03-S002, T03-S003, T03-S004, T03-S006, T03-S007, T03-S008, T03-S078]

- **Last_updated**: 2026-03（最新方法学预印本）
- **Decay risk**: high（评测规范正在快速收敛，12 个月内很可能出现社区默认模板）
- **关键工具**：RoboArena 评测基础设施（新兴）、序贯检验脚本（新兴）、逐次记录表 + 视频归档（必备）。evidence: [T03-S005, T03-S002]



### 10. 安全评估与合规

- **One-liner**：从「一个能干活的机器人单元」到「一份能过审、能签字、能在事故后站得住的安全文件包」。
- **属于哪一类流程**：标准与监管规定的流程，公开且强制。这是本 track 里**唯一一条不能自己发挥**的工作流。
- **Trigger**：任何人可能进入机器人可达空间；或产品要投放欧盟/北美/中国市场。evidence: [T03-S023, T06-S044]
- **Output**：风险评估报告 + 安全功能清单与 PL/SIL 计算 + 验证与确认（V&V）记录 + 实测数据（PFL 场景的力/压强、SSM 场景的停止距离）+ 使用说明书与残余风险告知 + 地区合规文件（EU 合格声明 / NRTL / GB 符合性）。evidence: [T06-S007, T06-S008, T03-S026, T03-S024]

**入门 SOP（8 步，对应 ISO 12100 的框架）**

1. **确定机械限制**（角色：安全工程师 + 方案）。机型、负载、末端与工具、工件、循环时间、**全部运行模式**（正常 / 设置示教 / 卡料恢复 / 维护 / 可预见误用）与人员类别。evidence: [T06-S007, T03-S023]
   - 跳过会怎样：后面所有分析的边界是错的，报告作废。
2. **识别危险**（角色：安全工程师）。挤压、剪切、冲击、工具（刀具/焊枪/激光）、工件（尖锐/高温/掉落）、电气、热、噪声、以及**人机同时在场**的场景。
   - 跳过会怎样：漏项的危险在事故里就是责任。
3. **风险评估（估计 + 评价）**（角色：安全工程师）。按严重度 / 暴露频次 / 发生概率 / 可避免性打分。**同一份 15066 的不同解读会导致不同的风险评估结论，学术界已有专门研究指出这一点**——所以解读口径要写进报告。evidence: [T03-S029, T06-S007]
4. **按三步法减小风险**（角色：安全工程师 + 设计）：①本质安全设计（改机构、降速度、降力、去尖角、改布局）→ ②安全防护与补充措施（围栏、光幕、安全扫描仪、安全限速/限位、双手控制、使能装置）→ ③使用信息（说明书、标识、培训）。**顺序不能颠倒。**
   - 跳过第①层直接上传感器会怎样：方案更贵、更脆弱，且审查时会被质疑。
5. **定义安全功能并做 PL/SIL 计算**（角色：功能安全工程师）。**PL/SIL 是安全功能的属性，不是整机属性**——写法是「急停功能达 PLd Cat.3」「安全限速功能达 PLd」。evidence: [T06-S044, T06-S008, T06-S018]
   - 跳过会怎样：客户/审查方要求提供计算书时拿不出来。
6. **实测验证**（角色：安全工程师 + 第三方设备）。
   - **PFL（功率与力限制）场景**：用专用测力装置实测人体各部位的准静态与瞬态力/压强，与限值比较。厂商侧提供专门的测量系统与按 15066 的标准化验证服务。evidence: [T06-S044, T03-S028, T03-S026]
   - **SSM（速度与间距监控）场景**：实测**停止时间与停止距离**，并据此校核安全距离——传感器响应时间 + 机器人停止时间共同决定最小安全距离。evidence: [T03-S027, T03-S026]
   - 跳过会怎样：安全方案只是纸面计算，实际不成立。**「先调高速度看看能不能过节拍」是明确禁止的。** evidence: [T06-S044]
7. **验证与确认（V&V）并留档**（角色：安全工程师 + 质量）。逐条检查每个安全功能是否按设计实现、是否可被旁路、失效模式如何。ISO 13849 / IEC 62061 / IEC 61508 都要求对安全系统做验证。evidence: [T03-S026, T06-S008, T06-S018]
8. **出地区合规文件**（角色：合规负责人）。
   - **欧盟**：今天（2026-09）出口欧盟仍按 2006/42/EC 做 CE；机械法规 (EU) 2023/1230 **2027-01-20 才适用**。CE 是**自我声明**制度不是「认证」，必要时由公告机构介入。evidence: [T06-S035, T06-S038, T06-S044, T06-S099]
   - **美国**：OSHA 没有机器人专用强制标准，走一般责任条款 + ANSI/A3 R15.06-2025（2025-10-29 三部分完整发布，**新增 Part 3 对用户方提出要求**）+ NRTL。evidence: [T06-S040, T06-S025, T06-S033]
   - **中国**：GB 11291.1-2011 / GB 11291.2-2013 是强制性国标，**不能用「按 ISO 最新版做了」替代**。另有 GB/T 20867-2007《工业机器人 安全实施规范》可作实施层参考。evidence: [T06-S046, T06-S047, T06-S044, T03-S052]

**什么时候必须停下来找第三方**

- 需要在欧盟走公告机构（NB）路径，或客户/保险/审查方要求第三方证书时。evidence: [T06-S099, T06-S098]
- **PFL 力/压强实测**没有合规测量设备时——这项不能用估算代替。evidence: [T03-S028]
- 安全功能的 PL/SIL 计算涉及自研安全部件（自己做的安全控制器/自研安全逻辑）时。
- 出现过伤人或险些伤人事件后。
- 团队里没有人能对风险评估签字负责时。国内可参考 A3 的集成商认证与国家职业技能标准来定「谁有资格签」。evidence: [T06-S095, T06-S096, T03-S083]

**资深路径（差异点）**

- `skip` 资深人跳过「先做完功能再补安全」：安全路线在选型阶段（工作流 2 第 2 步）就定了，到这一步是执行而不是设计。
- `optimize` 把风险评估与方案设计**并行**做，每次方案改动都回头更新评估表，而不是最后集中做一次。
- `optimize` 优先用本质安全设计把风险降下去（改布局、降速、去尖角），因为传感器方案的长期维护成本更高。
- `add` 额外做**残余风险与培训**交付：说明书写清残余风险、给操作与维护人员做记录在案的培训。
- `add` 额外做**变更管理**：约定「改了什么就要重做哪一部分评估」（换末端、改速度、改布局、改程序逻辑都可能触发重评）。
- `add` 额外做**基于仿真的早期安全验证**（在硬件到位前先在仿真里跑危险场景），学术界已有专门方法讨论。evidence: [T03-S032, T03-S031]

**判断这一步是否通过（具体标准）**

- 风险评估覆盖了**全部运行模式**，不只是正常生产。evidence: [T06-S007]
- 每个安全功能都有：功能描述 + 所需 PL/SIL + 计算书 + 验证记录。evidence: [T06-S008, T06-S018]
- PFL/SSM 的**实测数据**在档（不是计算值）。evidence: [T03-S026, T03-S028]
- 地区合规路径明确，且用词正确（「EU 合格声明 + CE 标志」，不是「CE 认证」）。evidence: [T06-S044]
- 没有任何一条安全措施依赖神经网络作为唯一判据。evidence: [T06-S044]

**绝对红线（任何理由都不能破，直接引用 Track 06 的合规红线）**

绕过或跳过风险评估 / 短接旁路安全回路与安全监控 / 超出经验证的速度与力限值运行协作应用 / 拆除防护而不做等效替代 / 用软件限速替代安全通道 / 示教模式下取消使能装置或降速限制 / 把神经网络直接接到安全功能上 / 无合规路径投放市场 / 用「按 ISO 做了」替代强制性国标 / 伪造或选择性报告性能数据。evidence: [T06-S007, T06-S040, T06-S093, T06-S002, T06-S003, T06-S008, T06-S018, T06-S035, T06-S046, T06-S037]

**常见失败模式**

- **「协作机器人天生安全，不用围栏」**（本行第五号破绽）：协作是应用属性；装上刀具就不再是协作应用。evidence: [T06-S044, T03-S023]
- **「15066 认证」**：TS 不可认证，且内容已并入 ISO 10218:2025。evidence: [T06-S044, T06-S026]
- **「我们有 CE 认证」**：CE 是自我声明。evidence: [T06-S044]
- **「这台机器人是 PLd 的」**：PL 属于安全功能不属于整机。evidence: [T06-S044]
- **把安全留到最后一周**：撞上出货节点，于是有人提议「先把光幕短接过了这一批」——这就是红线。evidence: [T06-S044]
- **只算不测**：停止距离与接触力必须实测。evidence: [T03-S026]

**时间与人力量级**

- 入门 SOP：单个机器人单元 **2–6 周**（含实测与整改），0.5–1 名安全工程师 + 第三方设备租用/服务。
- 资深路径：**1–2 周**（有模板、有测量设备、方案阶段已定安全路线）。
- **口径说明**：无公开一手统计；量级为本轨从安全服务商公开的服务阶段划分做的推断。evidence: [T03-S026, T03-S027]

**近期变化（近 12 个月）**：①**ISO 10218-1/-2:2025 发布，TS 15066 内容并入**——协作单元的验证仍要做，但**引用依据变了**，合同与报告模板需更新。evidence: [T06-S002, T06-S003, T06-S026] ②**ANSI/A3 R15.06-2025 三部分 2025-10-29 完整发布**，新增 Part 3 首次对用户方（终端工厂）提出美国国家标准义务。evidence: [T06-S025, T06-S033] ③**IEC 62061 AMD2:2026 发布**。evidence: [T06-S019] ④**(EU) 2026/1744 Digital Omnibus on AI（2026-07-27 生效）把机械类 AI 的技术要求归回机械法规**，并把 AI Act Annex III 推到 2027-12-02、Annex I 嵌入式推到 2028-08-02——当前处于「方向已定、细则未出」的过渡窗口，**方案里不应承诺具体条款**。evidence: [T06-S036, T06-S088] 触发事件类型：标准更新 + 法规变化。
**未来 12–24 个月的硬日期（应写进项目排期）**：2027-01-20 机械法规适用；2027-05-15 EN ISO 13849-1:2015 失去符合性推定。evidence: [T06-S035, T06-S008]

- **Last_updated**: 2026-07-27（Digital Omnibus 生效）
- **Decay risk**: high（法规侧，三个硬日期在 2027–2028）
- **关键工具**：风险评估模板（必备）、PL/SIL 计算工具（必备）、力/压强测量系统与停止时间测量装置（必备，通常外租或外包）。evidence: [T03-S026, T03-S028]



### 11. 现场部署与集成（节拍、换型、异常恢复、PLC/MES 边界）

- **One-liner**：从「实验室里能跑的单元」到「在客户产线上按节拍连续生产、能换型、能自己从异常里爬出来」的设备。
- **属于哪一类流程**：纯交付流程。公开材料以集成商与协会的自有材料为主，**真实的现场调试日志几乎全部闭源**——这是本 track 里公开材料最薄的一段之一。
- **Trigger**：单元在集成商厂内验证通过，准备发运；或客户现场具备进场条件。evidence: [T03-S060, T03-S062]
- **Output**：通过 SAT 的产线设备 + 与上位系统的接口文档 + 换型作业指导书 + 异常恢复手册 + 培训记录 + 备件清单 + 尾款签字。evidence: [T03-S060, T03-S061]

**入门 SOP（8 步）**

1. **厂内预验收 FAT**（角色：集成商项目经理 + 客户工程）。在集成商现场、用客户的真实零件、按书面规格逐条验证。FAT 是发运前的第一次正式验证，在电柜制作、软件配置、机械装配与内部质检完成之后进行。evidence: [T03-S062, T03-S060]
   - 跳过会怎样：设备到现场才发现不满足规格，返修成本与停线损失翻数倍。
2. **发运、就位、接电接气接网**（角色：安装队 + 客户设施）。
   - 跳过（指跳过预先确认现场条件）会怎样：到场才发现地面不平、电压不对、没有压缩空气、网口在另一头。
3. **现场标定与首件验证**（角色：调试工程师）→ 复用工作流 4；此时坐标系要与客户产线基准对齐。
   - 跳过会怎样：厂内标定在运输后已失效，第一批件全废。
4. **接上位系统：定清楚边界**（角色：控制工程师 + 客户 IT/自动化）。
   - **安全信号走安全通道**：机器人上电前需要「急停正常」「安全门关闭」这类信号，来自安全 PLC / 安全继电器或安全现场总线（如 CIP Safety / PROFIsafe），**不走普通通信**。evidence: [T03-S067]
   - **过程握手走 PLC**：PLC 发指令、机器人执行、状态信号回给 PLC 闭环。常见做法是把单元逻辑放在 PLC 里，机器人只做动作执行。evidence: [T03-S067, T03-S065]
   - **业务信息走 MES/WMS**：工单、批次、追溯、结果上报；OPC UA（含机器人 Companion Specification）是这一层的通用接口。evidence: [T03-S066, T03-S063]
   - 跳过会怎样：三层职责混在一起，出问题时没人能说清是谁的锅——业界的判断是**多数机器人集成失败不是软件 bug，而是逻辑、架构与职责边界的问题**。evidence: [T03-S067]
5. **节拍调试**（角色：调试工程师）。测**循环时间**并与客户**节拍**比较，留余量。**节拍是需求侧配额，循环时间是实际耗时，两者不能混用。** evidence: [T06-S044]
   - 跳过会怎样：单件能做但跟不上线，产能算错。
6. **异常恢复设计与演练**（角色：调试 + 客户操作工）。对每一类异常（没看到、抓空、掉件、卡料、超力、超时、上游断料、下游堵塞）演练恢复流程，并写进手册。
   - 跳过会怎样：每次异常都要叫工程师，设备实际可用率远低于验收时。
7. **换型验证**（角色：调试 + 客户工艺）。实测从上一产品切到下一产品的**换型时间**（含换爪、改程序、重标定、首件验证），并确认操作工能独立完成。evidence: [T06-S044]
   - 跳过会怎样：「柔性产线」在实际排产里变成不敢换型。
8. **SAT 现场验收 + 培训 + 移交**（角色：项目经理 + 客户）。SAT 在真实运行环境下、用客户零件、客户操作工、产线接口与维护流程一起验证；通过 SAT、完成培训、交付移交包、遗留问题正式约定，项目才算完成。evidence: [T03-S060, T03-S061]
   - 跳过会怎样：设备「装完了」但没人会用，三个月后闲置。

**资深路径（差异点）**

- `skip` 资深人跳过「到现场再优化节拍」：节拍在 FAT 前就要达标，现场只做微调。现场时间是全项目最贵的时间。
- `skip` 资深人跳过「先接 MES 再调工艺」：先把单元本身跑稳，上位接口最后接。
- `optimize` 把接口文档（信号表、时序图、错误码表）在**发运前**与客户自动化工程师逐条对过并签字。
- `optimize` 现场调试期间开满日志并做录制，为后续复盘留素材（见工作流 12）。evidence: [T03-S048]
- `add` 额外做「操作工视角走查」：让最不熟悉的那位操作工独立跑一遍开机、换型、清障、关机，全程不许工程师说话。
- `add` 额外做「首月陪产」：安排现场值守或远程支持窗口，把早期故障吃掉。
- `add` 额外做「备件与响应」约定：哪些件必须常备、坏了多久能到。系统 MTBF 的短板通常是末端工装、视觉、上下料与线缆，不是本体。evidence: [T06-S044]

**判断这一步是否通过（具体标准）**

- SAT 逐条对应书面需求，每条有测试步骤与责任人签字。evidence: [T03-S061]
- 连续生产验证：按约定时长连续跑（如一个班次/一天/一周），记录 OEE 或直通率与**干预次数**。evidence: [T06-S044]
- 换型时间实测并达标，且由客户操作工完成。evidence: [T06-S044]
- 每类异常都演练过并有书面恢复步骤。
- 接口文档与安全文件包齐全，培训有签到记录。

**常见失败模式**

- **来料在现场比样品差**：厂内用挑过的好件做 FAT，现场用真实来料就崩。破解：FAT 必须用客户提供的**真实批次**件，含边界件。evidence: [T03-S062]
- **安全信号接进普通 IO**：审查不过，且事故时无免责空间。evidence: [T03-S067]
- **验收只做单次成功不做连续运行**：验收当天好，第二周不行。破解：验收含连续运行与干预率。evidence: [T06-S044]
- **换型没人会**：设备变成「只做一种产品的专机」。evidence: [T06-S044]
- **把「免编程/零代码」当成不需要工程师**：图形化示教覆盖标准工序，异常处理、节拍优化与换型仍要工程师。evidence: [T06-S044]
- **本体 MTBF 当系统可用率依据**。evidence: [T06-S044]

**时间与人力量级**

- 入门 SOP：单工位单元现场 **1–4 周**（含标定、节拍、异常与培训），1–2 名调试工程师。
- 资深路径：**3 天–2 周**（接口预先对过、异常库可复用）。
- **口径说明**：无公开一手统计；量级为本轨从集成商公开的 FAT/SAT 阶段划分与移交清单做的推断。evidence: [T03-S060, T03-S061, T03-S062]

**近期变化（近 12 个月）**：①**北美项目的用户方义务**随 ANSI/A3 R15.06-2025 Part 3 落地，现场移交时要明确用户方的持续责任（培训、变更管理、巡检），合同模板需更新。evidence: [T06-S025, T06-S033] ②**国内人形试点的部署路径被政策化**：2026-06-03 工信部/国资委的实景实训专项要求用户单位按「最小干预、利旧复用」做环境适配、制定验证测试规程与达标条件、并在验证通过后推动「常态化部署」——**这实际上把「试点 → 上线」之间加了一道有书面标准的闸门**。evidence: [T05-S048] ③国内产品验收侧，JB/T 10825-2025《工业机器人产品验收实施规范》替代旧版，旧的 JB/T 8896-1999《工业机器人 验收规则》自 2026-07-01 废止。evidence: [T03-S051] 触发事件类型：标准更新 + 政策变化。

- **Last_updated**: 2026-07-01（旧验收规则废止日）/ 2026-06-03（政策）
- **Decay risk**: medium
- **关键工具**：PLC 编程环境与信号表（必备）、OPC UA 客户端（必备）、示教器/离线编程（必备）、日志录制与回放（必备）。evidence: [T03-S065, T03-S066, T03-S048]



### 12. 监控、失败复盘与迭代

- **One-liner**：从「上线之后」到「每一次失败都能被复现、被归类、被转成一个明确的下一步动作」——并且知道**什么时候该重新采数据、什么时候只是调参、什么时候该改硬件**。
- **属于哪一类流程**：工具链公开（日志格式、回放、可视化），**失败分类学与迭代决策规则几乎全部闭源**，本轨从工具文档、失败检测论文与岗位职责反推，如实标注。
- **Trigger**：设备已上线且有连续运行数据；或出现良率下降、干预率上升、客户投诉。evidence: [T03-S048]
- **Output**：失败分类分布 + 每类的根因与对策 + 下一版的改动清单（分为「调参 / 补数据 / 改工装 / 改硬件 / 改流程」五类）+ 更新后的监控指标基线。evidence: [T03-S049, T03-S050]

**入门 SOP（7 步）**

1. **先定要监控的指标基线**（角色：项目/运维）。至少：循环时间、干预次数与干预率、失败分类计数、直通率/良率、可用率或 OEE、以及**自主完成 vs 有人兜底**的比例。evidence: [T06-S044]
   - 跳过会怎样：出问题时无法判断「是变差了还是一直如此」。
2. **上线日志与回放**（角色：软件工程师）。机器人侧滚动录制短片段（分钟级）并自动上传，云端按时间线合并多源数据回放。工具侧的常见做法是设备上记录 MCAP/rosbag 片段、由 agent 自动上传，之后用同一套布局在同一时间线上回放多文件、多传感器、多机器人。evidence: [T03-S048, T03-S049]
   - 跳过会怎样：现场故障靠口述，永远复现不了。
3. **建失败分类学**（角色：算法/项目负责人）。建议的一级分类：感知错 / 定位标定漂移 / 规划或轨迹问题 / 控制与力控问题 / 抓取与工装问题 / 上下游与来料问题 / 硬件故障 / 场景超出设计范围 / 人为操作问题。
   - 跳过会怎样：所有失败都被归到「模型不行」，然后无脑加数据。
4. **每次失败强制归类并留证据**（角色：现场 + 工程）。归类要有对应的日志片段/视频/图片。
   - 跳过会怎样：分类分布不可信，迭代方向也就不可信。
5. **按分布决定下一步**（角色：技术负责人）→ 见下面的信号规则。
6. **改动后做 A/B 回归**（角色：评测负责人）。用工作流 9 的协议做配对比较，不要用「感觉好多了」。evidence: [T03-S002, T03-S009]
   - 跳过会怎样：改动之间互相掩盖，性能在几轮之后无人说得清。
7. **把新失败案例回灌到评测集与数据集**（角色：数据负责人）。
   - 跳过会怎样：同一个坑掉两次。

**什么信号说明该重新采数据（而不是调参）**

- **失败集中在「训练分布之外」**：新物体、新摆位、新光照、新场景——这是数据问题。定向补采那一类。evidence: [T03-S012]
- **同一任务在旧场景仍好、新场景掉** → 采多样性数据。
- **失败模式是「动作合理但幅度/时机不对」** → 通常是数据里该情况少，补数据有效。
- **反过来，下列信号说明不要采数据**：
  - 失败伴随**标定残差变化或撞机史** → 重标定（工作流 4），不是数据问题。
  - 失败集中在**抓不稳/滑落/力太大** → 改末端工装或加力控（工作流 3），数据补不了。
  - 失败随**时间/温度单调漂移** → 硬件或热问题。
  - 失败集中在**上下游来料变异** → 回到工作流 1 第 2 步改工装/改来料呈现。
  - 失败是**罕见但破坏性**（撞件、伤人风险） → 立刻加安全层与规则兜底，不要指望模型学会。evidence: [T06-S044]
- **本轨口径声明**：以上规则是从「失败归因四分法（数据/标定/硬件/流程）」与本行公开的失败讨论中整理出的**判断规则**，**没有公开的一手阈值表**；不要把它当成有统计支撑的门限。

**资深路径（差异点）**

- `skip` 资深人跳过「先加数据试试」：先看失败分类分布，分布不指向数据就不动数据。
- `optimize` 把「干预」做成一等公民：每次人工介入都自动记录时间、类型、上下文片段，而不是靠人事后填表。evidence: [T06-S044]
- `optimize` 用**在线失败检测**在失败发生时就打标并触发保存高分辨率片段；近期研究已经把「VLA 策略的多任务失败检测」做成了一个可训练的模块。evidence: [T03-S050]
- `add` 额外做**回归集**：把历史失败案例固化成一个每次改动都要跑的固定集合（相当于机器人版的单元测试）。
- `add` 额外做**变更日志与版本对齐**：模型版本、标定版本、程序版本、硬件批次要能一起追溯到某一次运行。
- `add` 额外做**长尾统计**：干预率比单次成功率更能反映能不能上线，因为它包含长尾。evidence: [T06-S044]

**判断这一步是否通过（具体标准）**

- 任意一次现场失败都能在 1 小时内被复现（找到对应日志片段并在回放里看到）。
- 失败分类分布每周更新，且分类由证据支持。
- 每一项改动都对应一个分类里的具体条目，并有回归结果。evidence: [T03-S002]
- 干预率与自主完成率分开统计并进入周报。evidence: [T06-S044]

**常见失败模式**

- **只存汇总指标不存原始数据**：知道变差了，不知道为什么。破解：滚动录制 + 自动上传。evidence: [T03-S048]
- **所有失败都归因为「模型能力不足」**：于是无限加数据。破解：强制分类。
- **干预不记账**：现场工人顺手扶一把、重摆一下，从不记录，导致「成功率」虚高。破解：把干预做成必须记录的动作。evidence: [T06-S044]
- **改动不做回归**：几轮之后无人知道当前版本比三个月前好还是差。evidence: [T03-S002]
- **日志只在开发机上有**：现场设备为省磁盘关掉了录制。破解：分片滚动 + 保留策略。evidence: [T03-S048]

**时间与人力量级**

- 建立监控与回放链路：**1–3 周**（首次），1 名软件工程师。
- 每周复盘：**半天**，技术负责人 + 现场。
- **口径说明**：无公开一手统计；量级为本轨从工具文档描述的部署方式做的推断。evidence: [T03-S048]

**近期变化（近 12 个月）**：①**失败检测从「事后人工分类」向「在线自动检测」演进**——2025-06 起有专门针对 VLA 策略的多任务失败检测方法公开。evidence: [T03-S050] ②**日志与回放工具栈成熟并分化**：MCAP 成为跨工具的记录格式，云端片段上传 + 多源同一时间线回放成为常见部署形态。evidence: [T03-S048, T03-S049] ③国内政策侧要求用户单位出具含「作业成功率、效率提升率、安全可靠性及经济可行性」的评估报告，把运营指标的采集变成了合规动作。evidence: [T05-S048] 触发事件类型：新方法 + 新工具 + 政策。

- **Last_updated**: 2026-09-02（工具文档复核）/ 2025-06（失败检测方法）
- **Decay risk**: medium
- **关键工具**：Foxglove / Rerun（必备，回放与可视化）、rosbag/MCAP（必备）、失败检测模块（新兴）。evidence: [T03-S048, T03-S049, T03-S050, T05-S077, T05-S078]



### 13. 演示与交付验收（POC vs 量产）

- **One-liner**：从「一个能拍视频的 demo」到「一份不会被 demo 骗的验收标准」，以及从 POC 到量产验收之间那道最容易被跳过的闸门。
- **属于哪一类流程**：交付流程；标准侧有产品验收规范，项目侧的验收条款闭源。
- **Trigger**：要做 POC 立项、要写验收条款、或要评估别人的 demo。evidence: [T03-S060, T03-S051]
- **Output**：一份验收标准表（每条含定义、测法、样本量、判定、责任人）+ POC 与量产两套不同的标准 + 明确的「不通过怎么办」条款。evidence: [T03-S061]

**POC 验收 vs 量产验收：差在哪**

| 维度 | POC / 试点验收 | 量产 / 上线验收 |
|---|---|---|
| 目的 | 证明**技术路径可行** | 证明**能持续赚钱且不出事** |
| 来料 | 可以是挑过的代表件 | 必须含真实批次与边界件 |
| 试验量 | 数十次，单次任务 | 连续班次/天/周，长时运行 |
| 主指标 | 成功率（带分母） | 循环时间 vs 节拍、直通率/OEE、**干预率**、换型时间、MTBF/MTTR | 
| 人的角色 | 允许有人在旁，但**必须记录** | 明确哪些环节允许人工、允许到什么程度 |
| 安全 | 受控环境、可降速 | 完整安全文件包 + 实测 |
| 失败处理 | 记录并分析即可 | 必须有恢复流程与责任人 |
| 交付物 | 报告 + 视频 + 数据 | 设备 + 文档包 + 培训 + 备件 + 服务条款 |

evidence: [T03-S060, T03-S061, T06-S044]

**入门 SOP（6 步）**

1. **把每条验收指标写成「定义 + 测法 + 样本量 + 判定 + 责任人」**（角色：项目经理 + 客户）。集成商侧的实践是：每个验收点都对应一条书面需求、一个测试步骤和一个具名责任人；过程 run-off 的验收准则要写成具体的东西（例如焊缝质量、循环时间、重复性）。evidence: [T03-S061]
   - 跳过会怎样：验收变成主观判断，尾款拖住。
2. **成功率必须带分母**（角色：项目经理）。写清任务定义、试验次数、初始状态分布、判定标准、是否允许重试、是否有人在旁。evidence: [T06-S044]
   - 跳过会怎样：双方对同一个「95%」理解不同。
3. **把人工介入写成独立条款**（角色：项目经理）。规定：哪些介入允许、每班允许多少次、介入后是否仍计成功、遥操作兜底是否算交付范围。**「有人接管」的成功不计入自主成功率。** evidence: [T06-S044]
   - 跳过会怎样：交付了一台需要人一直盯着的机器，双方都以为达标了。
4. **加连续运行条款**（角色：客户质量 + 项目经理）。规定连续跑多长时间、允许多少次停机、恢复时间上限。
   - 跳过会怎样：验收当天通过，第二周不行。
5. **加换型与异常条款**（角色：客户工艺）。换型时间上限 + 由客户操作工独立完成 + 每类异常的恢复时间。evidence: [T06-S044]
   - 跳过会怎样：柔性只存在于 PPT 里。
6. **写清不通过的处理**（角色：商务）。整改期限、复测规则、部分验收与扣款方式。
   - 跳过会怎样：出现争议时只能靠关系解决。

**怎么不被 demo 骗（评估别人的演示）**

- **问分母**：多少次里的多少。evidence: [T06-S044]
- **问初始分布**：物体是随机摆的还是固定的。
- **问干预**：有没有人接管、遥操作兜底、场景复位。evidence: [T06-S044]
- **问真机 vs 仿真**：仿真数字不作为能力证据。evidence: [T06-S044]
- **问连续性**：连续跑 8 小时的干预率是多少。evidence: [T06-S044]
- **问「进厂」的含义**：是常态化生产还是「实训/试点」？几个工位？跑了多少小时？国内公开表述里「进厂实训」与「上线生产」经常混用。evidence: [T03-S073, T03-S075]
- **问产能口径**：「第 N 台下线」是制造产能，不是部署量；订单量也不是交付量。evidence: [T03-S074, T06-S044]
- **问部署的商业结构**：按小时计费的 RaaS 模式下，供应商披露的是合同额与单机生命周期收入，这与「机器人能自主干多少活」是两件事——上市披露文件里可以看到这类单位经济口径。evidence: [T03-S071, T03-S068, T03-S069]
- **要求现场复现**：让对方在你的件、你的场地、你选的初始状态下跑 N 次。

**资深路径（差异点）**

- `skip` 资深人跳过「先做一个惊艳 demo 拿项目」这条路径的**后半段**：demo 可以做，但绝不用 demo 的条件写进验收条款。
- `optimize` 验收标准在**项目启动时**就写完并双方签字（工作流 1 第 6 步），不是交付前才谈。evidence: [T03-S061]
- `optimize` 把验收拆成 FAT（厂内，用客户件）与 SAT（现场，真实环境与人员）两道，早暴露问题。evidence: [T03-S060, T03-S062]
- `add` 额外做**边界件验收**：专门准备一批公差边缘、变形、脏污的件用于验收。
- `add` 额外做**换人验收**：由客户最不熟的操作工执行，工程师不许出手。
- `add` 额外做**留档口径**：所有验收数据、视频、逐次记录归档，作为后续争议与改进的依据。

**判断验收标准本身是否合格（元标准）**

- 每一条指标都能被第三人独立测出同样结果。
- 成功率条款含分母六要素（任务定义 / 次数 / 初始分布 / 判定 / 重试 / 有无人在旁）。evidence: [T06-S044]
- 自主与人工兜底分开写。evidence: [T06-S044]
- 含连续运行、换型、异常恢复三类「非单次任务」条款。
- 有不通过的处理条款。
- 国内工业机器人产品侧可引用 JB/T 10825-2025《工业机器人产品验收实施规范》作为产品验收依据（注意它是产品验收，不等于系统集成项目验收）。evidence: [T03-S051]

**常见失败模式**

- **用 demo 条件写验收**：固定摆位、挑过的件、工程师在旁。evidence: [T06-S044]
- **只验单次成功不验连续运行**。evidence: [T06-S044]
- **不写干预条款**：交付后才发现每小时要人管两次。evidence: [T06-S044]
- **把「实训/试点」当成「上线」写进宣传与合同**。evidence: [T03-S073, T03-S075]
- **验收指标写成形容词**（「运行平稳」「效果良好」）。
- **只报仿真或只报最好的一次**（技术诚信红线）。evidence: [T06-S044]

**时间与人力量级**

- 写验收标准：**1–3 天**（有模板时半天），项目经理 + 客户工艺 + 质量。
- 执行 FAT：**1–3 天**；SAT + 连续运行验证：**3 天–2 周**。
- **口径说明**：无公开一手统计；量级为本轨从集成商公开的 FAT/SAT 阶段说明做的推断。evidence: [T03-S060, T03-S062]

**近期变化（近 12 个月）**：①国内产品验收依据换版：JB/T 10825-2025《工业机器人产品验收实施规范》，旧的 JB/T 8896-1999 自 **2026-07-01** 废止。evidence: [T03-S051] ②**国内人形试点第一次有了政策规定的验收动作**：2026-06-03 的实景实训专项要求用户单位制定应用验证测试规程与达标条件，并出具含作业成功率、效率提升率、安全可靠性、经济可行性四项的评估报告——**这四项正好覆盖了「demo 骗不过去」的四个维度**。evidence: [T05-S048] ③首批人形机器人系列国标 2026-06 进入审定，发布后招投标与验收将从「厂商自定义指标」转向「按国标测」。evidence: [T06-S052, T06-S049] 触发事件类型：标准更新 + 政策变化。

- **Last_updated**: 2026-07-01（旧验收规则废止）/ 2026-06-03（政策）
- **Decay risk**: medium
- **关键工具**：验收标准表模板（必备）、逐次记录表 + 视频归档（必备）、ISO 9283 / GB/T 12642 测法（必备）。evidence: [T06-S006, T06-S048, T06-S089]



## Phase 2 接口

### A. 入门 SOP —— 一个最小完整任务的最少步骤

**场景**：单工位、来料基本确定、要在一台机械臂上做一个取放或简单装配任务，从零到能交付。

1. **去现场掐表 + 先问「能不能不用机器人」**（工作流 1）→ 出一页任务书，含容差、节拍、全部运行模式、验收指标。
2. **定形态与本体，同时定安全路线**（工作流 2）→ 选型报告 + 成本表。
3. **做误差预算，决定绝对精度路线还是相对定位路线**（工作流 3）→ 误差预算表。
4. **装配 + 标定 + 出重复性基线报告**（工作流 4）→ 标定包 + 基线。
5. **写功能，先写异常分支再写正常流程**（工作流 6A；若走学习路线则先冻结观测/动作空间再采 20–50 条贯通测试，工作流 7）。
6. **按协议做真机评测：带分母、带随机化范围、自主与人工兜底分开记**（工作流 9）。
7. **做风险评估与安全验证，实测力/压强或停止距离**（工作流 10）。
8. **FAT → 现场 SAT → 连续运行 + 换型 + 异常演练 + 培训移交**（工作流 11、13）。
9. **上线后开日志、建失败分类、每周复盘**（工作流 12）。

**入门 SOP 的最少步数：9 步**（跨 8 条工作流）。**没有任何一步可以在第一次交付中省略**——省略的后果在各工作流卡片的「跳过会怎样」里逐条写了。

### B. 资深路径 —— 跳过了什么、为什么敢跳

| 资深人跳过的事 | 为什么敢跳 | 什么条件下不敢跳 |
|---|---|---|
| 机器人运动学（绝对精度）标定 | 改走相对定位路线（视觉/力控在作业点二次找正），绝对精度不进误差链 | 必须离线编程、必须绝对定位（大件加工、多机协同） |
| 比十家品牌 | 隐性成本在运维与备件，不在采购价差 | 客户指定品牌或有强制国产化要求 |
| 把整条产线建进仿真 | 保真度的边际收益集中在接触区域 | 要做整线节拍仿真或布局论证 |
| 从零训练策略 | 开源 VLA 权重 + 自有平台 1–20 小时数据后训练即可（evidence: [T03-S033]） | 本体与动作空间与所有开源数据都不兼容 |
| 每改一次跑完整评测 | 用小规模冒烟测试筛掉明显退步，里程碑才跑完整协议 | 要对外发布或作为验收依据 |
| 先做惊艳 demo 再谈条款 | demo 条件不能写进验收，写了就等于给自己挖坑 | —（这一条没有例外） |
| 在高节拍固定工位上用机器人 | 专机/桁架更便宜更稳 | 需要柔性切换产品族 |
| 仿真里继续调接触参数 | 接触与柔性是仿真最不可信的一类，回报低 | gap 归因明确指向动力学或时序 |

**资深人反而多做的事（add 类占 30 处，是三类里最多的）**：留基线（标定基线、评测基线、指标基线）、留证据（逐次记录、日志片段、视频归档）、留退路（回退到传统规划、回退到人工工位）、留触发条件（重标触发清单、变更管理规则）。

**入门与资深的最大差距**：入门 SOP 是**线性**的（一步做完做下一步）；资深路径是**带早停与回跳**的——每一步都带一个「这一步的结果是否说明该回到上一步」的判据。最典型的三处回跳：
- 评测失败 → 回到「是数据问题还是标定/硬件问题」（工作流 12 的信号规则）。
- sim2real 三轮不改善 → 回到真机（工作流 8）。
- 数据加倍但置信区间重叠 → 停止采数据（工作流 7）。

### C. 反复出现在 ≥ 3 个工作流里的步骤（候选 playbook 通则）

1. **「先量化再决策」**：出现于工作流 1（量化来料变异）/ 3（量化误差源）/ 8（量化 sim2real gap）/ 12（量化失败分布）→ 候选规则：如果一个判断还停留在形容词上，则先把它变成一个带口径的数字再往下走。
2. **「分母与口径先于结论」**：出现于工作流 9（成功率分母）/ 12（干预率口径）/ 13（验收条款）→ 候选规则：如果对方给了一个百分比，则先问分母与判定标准。
3. **「留基线」**：出现于工作流 4（重复性基线）/ 9（评测基线）/ 12（指标基线）→ 候选规则：如果一项能力将来需要判断「是不是退化了」，则今天就要留一份可复现的基线。
4. **「安全属于应用，且必须实测」**：出现于工作流 2（选型阶段定安全路线）/ 10（实测力与停止距离）/ 11（安全信号走安全通道）→ 候选规则：如果有人把安全说成产品属性，则回到应用级风险评估。
5. **「自主与人工兜底分开记」**：出现于工作流 9 / 11 / 12 / 13 → 候选规则：如果一个成功里有人碰过，则它不计入自主成功率。
6. **「异常分支先于正常流程」**：出现于工作流 1（写全部运行模式）/ 6（先写异常分支）/ 11（异常演练）/ 12（失败分类）→ 候选规则：如果只演示过正常流程，则这个系统还没有进入工程阶段。

### D. 近 12 个月工作流的真实变化（带日期与触发事件）

| 日期 | 事件 | 改变了哪条工作流的哪一步 | 触发类型 | evidence |
|---|---|---|---|---|
| 2025-03 | 策略比较的近最优停止 / 序贯检验方法公开 | 工作流 9：从「固定跑 N 次」到「预先声明或用随时有效的序贯检验」 | 新方法 | [T03-S002] |
| 2025-06 | RoboArena 分布式双盲成对评测提出（CoRL 2025 发表） | 工作流 9：新增「分布式/跨机构评测」这一资深动作 | 新方法 | [T03-S003, T03-S004] |
| 2025-06 | 针对 VLA 的多任务失败检测方法公开 | 工作流 12：失败分类从事后人工转向在线自动打标 | 新方法 | [T03-S050] |
| 2025-10 | 大规模真机评测平台（RoboChallenge）与「不完美仿真器可靠评测」方法公开 | 工作流 8/9：仿真评测第一次有了可量化可信度的用法 | 新工具 + 新方法 | [T03-S006, T03-S007] |
| 2025-10-29 | ANSI/A3 R15.06-2025 三部分完整发布（新增用户方 Part 3） | 工作流 2/10/11：北美项目要把用户方义务写进合同与移交 | 标准更新 | [T06-S025, T06-S033] |
| 2025-11 | Isaac Lab 框架论文公开 + 官方 sim2real 部署工作流与参考架构 | 工作流 5/8：从「自己拼 sim2real 链路」到「跟着官方示例走」 | 新工具 | [T03-S045, T03-S040, T03-S042] |
| 2025 全年 | 开源 VLA 权重与后训练工具链成熟（openpi / LeRobot / SmolVLA） | 工作流 6/7：学习路线默认从后训练起步；工作重心前移到数据与评测 | 新模型 + 新工具 | [T03-S033, T03-S034, T03-S038] |
| 2025-12-26 | 工信部人形机器人与具身智能标委会成立 | 工作流 2/13：国内人形项目的验收依据开始有归口 | 标准更新 | [T06-S091] |
| 2026-02-28 | 《人形机器人与具身智能标准体系（2026 版）》发布 | 工作流 2/13：顶层规划出台，测试项开始可预留 | 标准更新 | [T06-S092] |
| 2026-03 | 「超越二元成功率」的样本高效比较方法公开 | 工作流 9：评测度量从单一成功率扩展到多维 | 新方法 | [T03-S008] |
| 2026-06 | 首批人形机器人系列国标进入审定 | 工作流 2/13：招投标与验收将从厂商自定义指标转向按国标测 | 标准更新 | [T06-S052, T06-S049] |
| 2026-06-03 | 工信部/国资委《2026 年度人形机器人与具身智能实景实训专项行动》（工信厅联科函〔2026〕256 号） | 工作流 1/7/11/13：场景选取、环境「最小干预」改造、数据集维度、验证测试规程与四项评估报告全部被政策规定 | 政策/法规 | [T05-S048] |
| 2026-07-01 | JB/T 8896-1999《工业机器人 验收规则》废止，JB/T 10825-2025 替代 | 工作流 13：国内产品验收引用依据换版 | 标准更新 | [T03-S051] |
| 2026-07-27 | (EU) 2026/1744 Digital Omnibus on AI 生效 | 工作流 10：机械类 AI 要求归回机械法规；AI Act 高风险适用日推迟 | 法规变化 | [T06-S036, T06-S088] |

**变化触发事件类型分布**：新方法 5 / 新工具 3 / 标准更新 5 / 政策法规 2 —— **这一行的工作流变化有近一半来自标准与政策，而不是来自新模型**。这与「LLM agent 行业的工作流变化几乎全部来自新模型」形成鲜明对比，是 Phase 2 识别本行外部驱动力时的关键信号：**本行同时被「AI 迭代速度」和「工业标准迭代速度」两个时钟驱动，后者慢但硬。**

### E. 候选 playbook 规则（16 条，格式：如果 {场景} → 则 {决策方向}）

1. **如果**有人拿一段演示视频要求「这个我们也做」→ **则**先要分母（多少次、什么初始分布、有没有人接管、真机还是仿真），拿不到就按「未验证」处理，不进任务书。*案例*：本行第二号外行破绽就是无分母成功率。evidence: [T06-S044, T03-S002]
2. **如果**任务的主要难点是来料位置/姿态不确定 → **则**先算「改工装/改来料呈现」的成本，再算机器人方案的成本，两者并列给客户。*案例*：集成失败的主因公开表述为零件变异、工装不良与需求不清，而非机器人硬件。evidence: [T03-S064, T03-S090, T03-S001]
3. **如果**工位固定、来料确定、节拍很高 → **则**优先专机/桁架，而不是机器人；把这条写进选型报告的「被否形态」。*案例*：选型报告要求显式记录被否形态与理由。evidence: [T03-S061]
4. **如果**规格书写着 ±0.02 mm → **则**默认它是重复定位精度，绝对精度按毫米级估，并追问 ISO 9283 的测试条件。evidence: [T06-S006, T06-S085, T06-S044]
5. **如果**要求亚毫米级装配而机器人绝对精度只有毫米级 → **则**改走相对定位路线（作业点二次视觉/力控找正），不要靠加标定次数硬补。evidence: [T03-S018, T03-S020]
6. **如果**手眼标定残差看着很小但换个工作区域就偏 → **则**问题在位姿分布而不是样本数，重采覆盖实际作业区、姿态角拉开的位姿。*案例*：工具最少 5 组即可求解，但供应商明确把旋转/平移运动范围列为精度影响因素。evidence: [T03-S016, T03-S020, T03-S022]
7. **如果**要建仿真 → **则**先明确它服务于「训练策略 / 验节拍 / 数字孪生」中的哪一个，三者的建模精度要求完全不同。*案例*：照 CAD 建的静态仿真不是数字孪生。evidence: [T06-S044]
8. **如果**sim2real 的 gap 主因是接触、柔性或真实光照 → **则**转真机，不要继续调仿真参数；如果主因是动力学或时序 → **则**留在仿真做系统辨识与延迟建模。evidence: [T03-S043, T03-S013, T06-S044]
9. **如果**策略在仿真里完美、真机上「像喝醉了」→ **则**先查延迟与时序对齐，再怀疑模型能力。*案例*：UMI 明确区分「采集时无延迟」与「推理时有传感/推理/执行三类延迟」，并在策略接口里做延迟匹配。evidence: [T03-S013]
10. **如果**数据量翻倍但真机成功率的置信区间仍重叠 → **则**停止采数据，改做定向补采或回查硬件/标定。evidence: [T03-S002, T03-S008]
11. **如果**失败集中在抓不稳、滑落、力过大 → **则**改末端工装或加力控，数据补不了这类账。evidence: [T06-S044]
12. **如果**失败是罕见但破坏性的（撞件/伤人风险）→ **则**加规则与安全层兜底，不要指望模型学会。evidence: [T06-S044, T06-S002]
13. **如果**要在人机共享空间作业 → **则**按应用做风险评估并**实测**力/压强或停止距离；「先调高速度看看能不能过节拍」是红线。evidence: [T06-S007, T06-S003, T03-S026, T03-S028]
14. **如果**项目要出口欧盟且交付在 2027-01-20 之后 → **则**合规排期按机械法规 (EU) 2023/1230 提前 12 个月启动；在此之前交付的仍按 2006/42/EC 做 CE。evidence: [T06-S035, T06-S038]
15. **如果**一个「成功」里有人碰过（扶一把、遥操作、重摆、重启）→ **则**它不计入自主成功率，只计入带兜底完成率，两个数字分开报。evidence: [T06-S044]
16. **如果**验收条款里没有「连续运行 + 换型 + 异常恢复」三类非单次任务条款 → **则**这份验收标准会被 demo 骗，退回重写。evidence: [T03-S060, T03-S061, T06-S044]

### F. 质量基准 —— 什么算一次合格的交付

1. **有书面任务定义书**，含全部运行模式、容差、节拍、验收指标与测法，且「不上机器人」的替代方案被显式论证过。evidence: [T03-S001, T06-S007]
2. **有误差预算表与标定基线报告**，重复性按 ISO 9283 / GB/T 12642 方法实测。evidence: [T06-S006, T06-S048]
3. **有带分母的评测结果**，自主成功率与带人工兜底完成率分开报，含不确定度。evidence: [T03-S002, T06-S044]
4. **有完整安全文件包**：风险评估（覆盖全部运行模式）+ 安全功能与 PL/SIL 计算 + V&V 记录 + 力/压强或停止距离实测数据 + 地区合规文件。evidence: [T06-S007, T06-S008, T03-S026]
5. **通过 FAT 与 SAT**，SAT 用真实来料、真实环境与客户操作工完成，每条对应书面需求与具名责任人。evidence: [T03-S060, T03-S061, T03-S062]
6. **连续运行验证过**，并记录了循环时间 vs 节拍、干预率、换型时间。evidence: [T06-S044]
7. **每类异常都有书面恢复步骤且演练过**，客户操作工能独立完成。
8. **日志与回放链路可用**，任一现场失败可复现。evidence: [T03-S048]
9. **文档包齐全**：接口信号表与时序、换型作业指导书、异常恢复手册、备件清单、培训记录、重标触发清单。
10. **没有任何一条安全措施依赖神经网络作为唯一判据。** evidence: [T06-S044]

### G. 反模式（外行 / 新手最常犯的 12 条）

1. **拿演示视频当能力证据**，不问分母、不问干预、不问真机还是仿真。evidence: [T06-S044]
2. **从「人形很酷」倒推需求**，跳过「能不能不用机器人 / 用什么形态最省」的论证。evidence: [T03-S001, T03-S090]
3. **把 repeatability 当 accuracy 用**，用 ±0.02 mm 的规格去承诺系统精度。evidence: [T06-S006, T06-S085]
4. **认为买了协作臂就免掉风险评估与围栏**——协作是应用属性，装上工具就不再是协作应用。evidence: [T06-S003, T06-S026]
5. **用数据去补硬件/工装/标定的账**：抓不稳就多采数据，来料乱就多采数据。
6. **先采几万条数据再跑通链路**，结果观测/动作空间定义错，数据全废。
7. **中途改硬件、相机位置或动作空间**，不评估历史数据的贬值。
8. **只做正常流程**，异常分支留到现场再写；然后发现产线时间大量花在异常恢复上。
9. **报仿真成功率、报最好的一次、报无分母百分比**——技术诚信红线。evidence: [T06-S044]
10. **把「有人接管」的成功计入自主成功率**（本行最大的糊涂账）。evidence: [T06-S044]
11. **混用节拍与循环时间**、混用订单量与交付量、混用产能与部署量、混用「实训」与「上线」。evidence: [T06-S044, T03-S074, T03-S073]
12. **安全留到最后一周**，然后提议「先把光幕短接过了这一批」——这是刑责级红线。evidence: [T06-S040, T06-S093]

### H. 冷僻 / 信号薄弱评估（诚实边界）

- **工作流数量**：13 条（远高于 floor 4）。每条有完整卡片 + `last_updated` + `decay risk` + 近期变化字段。
- **一手来源占比**：论文原文 + 政府监管原文 + 项目自有代码仓 = 33/90（36.7%）；加上厂商与集成商自有文档、协会、招聘 JD 等准一手 = 84/90（**93.3%**）。二手转述 6 条，主要用于中国侧产业数字，正文已逐条标注。
- **资深差异点**：13/13（100%）workflow 有 ≥ 2 处，合计 75 处。
- **本 track 不属于冷僻行业**，但有 **4 处必须写进诚实边界**：
  1. **交付流程大量闭源**。工作流 1、11、12、13 的真实企业内部 SOP（现场调试日志、验收条款模板、失败分类学）几乎没有可引用的公开一手文档。本文件这几条主要从 **集成商自有材料 + 协会技术文 + 标准条文 + 招聘 JD** 反推，已在每条卡片顶部标注「属于哪一类流程」。
  2. **时间与人力量级绝大多数没有公开一手统计**。本文件只在 5 处给出了一手数字（DROID 的 12 个月/50 人/76k 条/350 小时/564 场景/86 任务；TRI 的 1,700 小时数据与 1,800 次真机 rollout；SmolVLA 的 ~50 episodes 与 A100 4 小时/2 万步；openpi 的 1–20 小时微调数据与显存门槛；操作研究常见的 20–30 次真机试验）。其余的「1–3 周」「2–6 周」一律标注为**本轨的量级推断**，Phase 2 引用时必须保留这个限定词，**不要转写成行业均值**。
  3. **中国侧的采集成本与规模数字全部是媒体转述**（单小时有效数据成本 500 元以上、数据基地年产能十几万小时、六十万人采集队伍等），无第三方验证、口径未公开。本文件已标注「媒体转述，非一手」，Phase 2 若要引用必须连同这个标签一起写。
  4. **混合分层架构（工作流 6C）是本文件公开材料最薄的一段**。分层怎么切、接口怎么定、上层出指令频率，这些几乎全部闭源；本文件的描述来自政策文件的「大脑/小脑/肢体」表述与厂商话术的工程还原，**不是从任一家的交付文档里读到的**。
- **矛盾保留（供 Phase 1.5 裁决）**：
  - **评测该不该标准化**：一派主张固定基准（RoboChallenge、VLA-REPLICA 的低成本可复现基准），一派主张放弃固定基准、用分布式众包双盲评测换多样性（RoboArena）。两者都在 2025–2026 年公开，尚未收敛。evidence: [T03-S006, T03-S078, T03-S003]
  - **仿真能不能用于评测**：本行的公开共识是「仿真数字不作为能力证据」，但 2025-10 起出现「用不完美仿真器给出带可靠性保证的评测」的方法学工作。这是一个正在发生的规范转折，本文件按「仿真只做粗筛」写，并标注了新方向。evidence: [T06-S044, T03-S007, T03-S079]
- **decay 结论**：本 track 的 **6/13 条为 high decay**，且其中 5 条（5/6/7/8/9）集中在学习路线一侧。**建议 Phase 2 在诚实边界写明：本 skill 的工作流节中，学习路线相关的 5 条建议每 6 个月复查一次；安全合规一条的刷新触发点设在 2027-01-20（欧盟机械法规适用）与 2027-05-15（EN ISO 13849-1:2015 失效）；传统工程侧的 2 条（误差预算、标定）可 24 个月不动。**

## 自检清单

- [x] **Workflow 数量 ≥ 4**：13 条（覆盖「要不要做 → 上线之后」全链路，含任务定义、选型、误差预算、标定、仿真、方案开发、数据、sim2real、评测、安全、部署、复盘、验收）。
- [x] **每个 workflow 有完整卡片 + `last_updated`**：13/13。每张卡含 one-liner / 属于哪一类流程 / trigger / output / 入门 SOP（含每步跳过的后果）/ 资深路径（skip·optimize·add）/ 判定标准 / 常见失败模式 / 时间与人力量级 / 近期变化 / decay risk / 关键工具。
- [x] **入门 SOP 与资深路径分开**：13/13 分开写；13/13（100%）有 ≥ 2 处资深差异点，合计 75 处（skip 19 / optimize 26 / add 30）。
- [x] **近期变化字段 ≥ 60%**：13/13（100%）填写，其中 3 条明确写「稳态 / 无重大变化」并给出最近一次显著变化的年份与事件（合法填法）。
- [x] **一手来源占比 ≥ 50%**：论文 + 政府监管原文 + 项目自有仓 = 36.7%；加厂商/集成商自有文档、协会、JD 等准一手 = 93.3%。二手仅 6 条且全部标注。
- [x] **Decay risk 每条都标**：high 6 / medium 5 / low 2。
- [x] **总览表按 decay 分组**：见「总览」节三张表。
- [x] **Phase 2 接口齐全**：入门 SOP（A）/ 资深路径与跳过理由（B）/ 跨 workflow 共同步骤（C）/ 近 12 个月带日期的变化与触发类型分布（D）/ 候选 playbook 16 条（E，每条带案例与 evidence）/ 质量基准 10 条（F）/ 反模式 12 条（G）/ 冷僻与薄弱信号（H）。
- [x] **Source Manifest 合规**：90 条，表头字段齐全，`last_checked` 全部为 2026-09-02；bucket 仅用 `verified_primary` / `surrogate_primary` / `secondary`；**无黑名单条目**（搜索过程中出现的知乎、CSDN、腾讯新闻、Quora、emergentmind 等 AI 摘要站、以及 SEO 型 FAT/SAT 站点均已剔除）；全部 `surrogate_primary` 的 note 含规定关键词（vendor docs / own site / own publication / originator / 协会 / association / standards body / 监管 / regulator / JD / 课程），**未使用 `official`**。
- [x] **evidence 挂载**：每条工作流的 Trigger / Output / 资深差异 / 判定标准 / 近期变化均挂 evidence id，跨轨引用 `T04-*` / `T05-*` / `T06-*` 未重复登记。
- [x] **数字带口径**：一手数字（DROID、TRI LBM、SmolVLA、openpi、真机试验次数量级）标了来源；无一手来源的时长与人力一律标注「本轨的量级推断 / 无公开一手统计」；中国侧产业数字标注「媒体转述，非一手」。**全文没有编造行业经验值。**
- [x] **区分论文流程与交付流程**：13/13 卡片顶部标注「属于哪一类流程」，并在 H 节点名了 4 处公开材料稀薄的地方。
- [x] **中国侧**：政策（工信厅联科函〔2026〕256 号、机器人+方案）、强制性国标（GB 11291 系列）、产品验收行标（JB/T 10825-2025 及旧版废止日）、人形国标进程（立项/审定）、国内厂商可下载手册（节卡、埃斯顿酷卓）、国内招聘 JD（宇树）均已覆盖；**薄的地方（集成商项目级验收模板、真实调试日志）已如实标注为未获取到公开一手材料**。
- [x] **遥操作介入与自主性能分开记**：工作流 9 第 4 步给出三分类记法（自主成功 / 介入后成功 / 失败），工作流 11、12、13 反复强化，并写进 playbook 第 15 条与反模式第 10 条。
- [x] **无空标题、无「回填中/待补」占位**。
