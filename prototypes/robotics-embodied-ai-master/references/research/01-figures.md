# Track 01 — Figures（行业大佬）· 机器人与具身智能

> Phase 1 wave 2 · locale=zh-CN · 调研日期 2026-09-02
> 行业范围：能在真实世界里可靠感知 / 规划 / 动作的物理机器人（机械臂、移动操作、人形、足式）。范围外（仅作对比）：乘用车自动驾驶栈、纯软件 LLM agent 基础设施、半导体制造工艺、传统 PLC 产线电气设计。
> Wave 1 seed：04-canon.md 的 9 个流派代表人物、05-sources.md 的播客主理人与嘉宾、06-glossary.md 的厂商话术节。跨轨 evidence 直接引用 `T04-*` / `T05-*` / `T06-*` id（不在本 manifest 重复登记）。

## 0. 阅读须知（口径纪律）

1. **一个人的一次发声 ≠ 行业结构描述**。凡写「这一行的人认为 X」必须有跨人跨源证据；单人观点一律点名 + 标年份 + 标场合。
2. **原话 vs 转述严格分开**。标「原话」的都是从一手页面逐字取的（英文原文照抄、中文照抄）；其余全部标「要义转述」。**没有任何一句是本文件编的。**
3. **利益关系点名**。人形机器人这一行的公开发言与融资节奏高度耦合，每张卡片都写清这个人靠什么吃饭。
4. **数字带口径**。任何成功率 / 自主率 / 出货量 / 订单额都写清谁公布、什么时点、分母是什么、有没有第三方验证；做不到写「未公开」。
5. **争议写实**。谁批评谁、批评什么、对方回没回，照抄公开记录；路线不同就写路线不同，不升格成互相攻击。

## Source Manifest

| source_id | url | bucket | last_checked | author/host | note |
|-----------|-----|--------|--------------|-------------|------|
| T01-S001 | https://rodneybrooks.com/why-todays-humanoids-wont-learn-dexterity/ | surrogate_primary | 2026-09-02 | Rodney Brooks | own site 本人 2025-09-26 长文，人形灵巧度批评全文 |
| T01-S002 | https://rodneybrooks.com/predictions-scorecard-2026-january-01/ | surrogate_primary | 2026-09-02 | Rodney Brooks | own site 本人第八年预测记分卡，含人形判断 |
| T01-S003 | https://rodneybrooks.com/four-time-scales-for-technology-development-and-deployment/ | surrogate_primary | 2026-09-02 | Rodney Brooks | own site 本人 2026-08-01 长文，三种速度分离 |
| T01-S004 | https://rodneybrooks.com/blog/ | verified_primary | 2026-09-02 | Rodney Brooks | own site 博客索引，确认发文序列与日期 |
| T01-S005 | https://spectrum.ieee.org/robust-ai-rodney-brooks | secondary | 2026-09-02 | IEEE Spectrum | 长访谈：Robust.AI 实际在做什么 |
| T01-S006 | https://www.robust.ai/blog/newsweekaiseries | verified_primary | 2026-09-02 | Robust.AI | vendor docs，本人任 CTO 的公司博客 |
| T01-S007 | https://www.humanoidsdaily.com/feed/the-dexterity-debate-roboticists-clash-over-the-future-of-humanoid-hands-on-work | secondary | 2026-09-02 | Humanoids Daily | 灵巧度之争整理，含 Scott Walter 反驳 |
| T01-S008 | https://autolab.berkeley.edu/assets/publications/media/GOFE-Can-Close-the-100000-Year-Robot-Data-Gap-Science-Robotics-Aug-2025-scirobotics.aea7390.pdf | verified_primary | 2026-09-02 | Ken Goldberg | 本人 Science Robotics 社论全文 PDF（实验室托管） |
| T01-S009 | https://autolab.berkeley.edu/assets/publications/media/Data-Debate-Science-Robotics-Aug-2025-scirobotics.aea7897.pdf | verified_primary | 2026-09-02 | Amato/Hutchinson/Garg/Billard/Rus/Tedrake/Park/Goldberg | ICRA 2025 全会辩论全文，8 人署名立场 |
| T01-S010 | https://goldberg.berkeley.edu/ | verified_primary | 2026-09-02 | Ken Goldberg | own site 个人主页，任职与公司关系 |
| T01-S011 | https://news.berkeley.edu/2025/08/27/are-we-truly-on-the-verge-of-the-humanoid-robot-revolution/ | verified_primary | 2026-09-02 | UC Berkeley News | 本人问答式长访谈，含直接引语 |
| T01-S012 | https://www.youtube.com/watch?v=PfvctjoMPk8 | surrogate_primary | 2026-09-02 | ICRA 2025 | own publication ICRA 2025 辩论全程录像 |
| T01-S013 | https://www.science.org/doi/10.1126/scirobotics.aea7390 | verified_primary | 2026-09-02 | Science Robotics | 社论 DOI 落地页（对爬虫 403，正文以 S008 PDF 为准） |
| T01-S014 | https://www.youtube.com/watch?v=94v3zRfBQXQ | surrogate_primary | 2026-09-02 | Ken Goldberg | own publication 本人长视频《2025 年机器人能做与不能做什么》 |
| T01-S015 | https://www.youtube.com/watch?v=TN1M6vg4CsQ | surrogate_primary | 2026-09-02 | Russ Tedrake | own publication Stanford seminar 2025-04-25，LBM 多任务迁移 |
| T01-S016 | https://toyotaresearchinstitute.github.io/lbm1/ | surrogate_primary | 2026-09-02 | TRI LBM Team | vendor docs LBM 严格评测项目页，含负面结论 |
| T01-S017 | https://arxiv.org/abs/2507.05331 | verified_primary | 2026-09-02 | TRI LBM Team（Tedrake 通讯） | LBM 论文 arXiv 全文 |
| T01-S019 | https://www.tri.global/news/ai-powered-robot-boston-dynamics-and-toyota-research-institute-takes-key-step-towards-general | surrogate_primary | 2026-09-02 | Toyota Research Institute | vendor docs，BD+TRI Atlas LBM 合作 |
| T01-S020 | https://www.therobotreport.com/boston-dynamics-tri-use-large-behavior-models-train-atlas-humanoid/ | secondary | 2026-09-02 | The Robot Report | Atlas + LBM 报道，交叉印证 |
| T01-S021 | https://www.youtube.com/watch?v=y05L6pYWBc0 | surrogate_primary | 2026-09-02 | Russ Tedrake | own publication 本人 talk《面向灵巧操作的大行为模型》 |
| T01-S022 | https://www.pi.website/blog/pi05 | verified_primary | 2026-09-02 | Physical Intelligence | vendor docs，π0.5 发布贴，含局限自述 |
| T01-S023 | https://www.pi.website/blog/pi07 | verified_primary | 2026-09-02 | Physical Intelligence | vendor docs，2026-04-16 π0.7 发布贴 |
| T01-S024 | https://www.pi.website/blog/olympics | verified_primary | 2026-09-02 | Physical Intelligence | vendor docs，莫拉维克悖论与机器人奥运 |
| T01-S025 | https://arxiv.org/abs/2504.16054 | verified_primary | 2026-09-02 | Black/Finn/Levine 等 | π0.5 论文，开放世界泛化 |
| T01-S026 | https://twimlai.com/podcast/twimlai/cf800-a-foundation-model-for-robotics | verified_primary | 2026-09-02 | TWIML / Sergey Levine | #719 本人 ≥1 小时技术访谈 |
| T01-S027 | https://podcasts.apple.com/gb/podcast/sergey-levine-building-llms-for-the-physical-world/id1154105909?i=1000758384855 | verified_primary | 2026-09-02 | Invest Like the Best | 2026-03-31 本人 67 分钟访谈 |
| T01-S028 | https://podcasts.apple.com/us/podcast/331-sergey-levine-the-robot-revolution-nobody-is/id1438378439?i=1000760975265 | verified_primary | 2026-09-02 | Eye On A.I. | 2026-04-12 本人 59 分钟访谈 |
| T01-S029 | https://ai.stanford.edu/~cbfinn/ | verified_primary | 2026-09-02 | Chelsea Finn | own site 个人主页，任职与授课 |
| T01-S030 | https://irislab.stanford.edu/ | verified_primary | 2026-09-02 | Stanford IRIS Lab | own site 实验室主页 |
| T01-S031 | https://www.youtube.com/watch?v=a8-QsBHoH94 | surrogate_primary | 2026-09-02 | Chelsea Finn / YC | own publication 2025-06-17 本人完整 talk 录像 |
| T01-S032 | https://iclr.cc/virtual/2025/10000222 | verified_primary | 2026-09-02 | ICLR 2025 | 会议 own site，特邀报告条目与题目 |
| T01-S033 | https://www.ycombinator.com/library/Mj-chelsea-finn-building-robots-that-can-do-anything | secondary | 2026-09-02 | Y Combinator | talk 音频/文字入口 |
| T01-S034 | https://x.com/chelseabfinn | surrogate_primary | 2026-09-02 | Chelsea Finn | own site 本人账号，2026 ICML 报告安排 |
| T01-S035 | https://www.amazon.science/author/pieter-abbeel | verified_primary | 2026-09-02 | Amazon Science | vendor docs，本人在 Amazon 的作者页 |
| T01-S036 | https://en.wikipedia.org/wiki/Pieter_Abbeel | secondary | 2026-09-02 | Wikipedia | 履历时间线交叉核对（非证据源） |
| T01-S037 | https://vcresearch.berkeley.edu/faculty/pieter-abbeel | verified_primary | 2026-09-02 | UC Berkeley | own site 机构人物页，学术身份 |
| T01-S038 | https://profiles.stanford.edu/shuran-song | verified_primary | 2026-09-02 | Stanford | own site 教师档案，职称/奖项/课程 |
| T01-S039 | https://real.stanford.edu/ | verified_primary | 2026-09-02 | Shuran Song | own site 实验室主页（REAL） |
| T01-S040 | https://www.therobotreport.com/interview-with-chung-chi-about-the-umi-gripper-and-diffusion-ai-models/ | secondary | 2026-09-02 | The Robot Report | UMI 夹爪访谈（受访者为其学生） |
| T01-S041 | https://www.humanoidsdaily.com/news/1x-ceo-details-neo-s-two-modes-and-defends-teleoperation-as-more-secure-than-a-cleaner | secondary | 2026-09-02 | Humanoids Daily | 1X CEO 遥操作辩护整理 |
| T01-S042 | https://rai-inst.com/about/leadership/marc-raibert/ | verified_primary | 2026-09-02 | RAI Institute | own site 领导层页，本人当前角色 |
| T01-S043 | https://ethz.ch/en/news-and-events/eth-news/news/2025/09/the-rai-institute-opens-up-unique-opportunities-for-both-researchers-and-students.html | surrogate_primary | 2026-09-02 | ETH Zürich | own site 官方访谈，Hutter 直接引语 |
| T01-S044 | https://bostondynamics.com/news/boston-dynamics-and-the-robotics-ai-institute-partner/ | surrogate_primary | 2026-09-02 | Boston Dynamics | vendor docs，与 RAI 的合作公告 |
| T01-S045 | https://rai-inst.com/news/ | surrogate_primary | 2026-09-02 | RAI Institute | own site 新闻页，机构动态 |
| T01-S046 | https://rai-inst.com/resources/blog/pushing-the-pace-of-progress/ | verified_primary | 2026-09-02 | RAI Institute | own site 博客，研究节奏立场 |
| T01-S047 | https://rsl.ethz.ch/ | surrogate_primary | 2026-09-02 | Marco Hutter / ETH RSL | own site 实验室主页 |
| T01-S048 | https://www.anybotics.com/ | surrogate_primary | 2026-09-02 | ANYbotics | vendor docs，其联创公司官网 |
| T01-S049 | https://meche.mit.edu/people/faculty/SANGBAE@MIT.EDU | verified_primary | 2026-09-02 | MIT MechE | own site 教师页，学术身份 |
| T01-S050 | https://en.wikipedia.org/wiki/Sangbae_Kim | secondary | 2026-09-02 | Wikipedia | 停薪留职加入 Meta 的时间线交叉核对 |
| T01-S051 | https://spectrum.ieee.org/mit-little-hermes | secondary | 2026-09-02 | IEEE Spectrum | Little HERMES 力反馈遥操作动机 |
| T01-S052 | https://www.quantamagazine.org/why-do-humanoid-robots-still-struggle-with-the-small-stuff-20260313/ | secondary | 2026-09-02 | Quanta Magazine | 2026-03-13 多位一线研究者同台引语 |
| T01-S053 | https://www.skild.ai/ | surrogate_primary | 2026-09-02 | Skild AI | vendor docs，omni-bodied 公司口径 |
| T01-S054 | https://www.therobotreport.com/skild-ai-raises-1-4b-building-omni-bodied-robot-skild-brain/ | secondary | 2026-09-02 | The Robot Report | 2026-01 融资与技术主张报道 |
| T01-S055 | https://news.crunchbase.com/venture/robotics-startup-skild-ai-triples-valuation/ | secondary | 2026-09-02 | Crunchbase News | 估值与投资方交叉印证 |
| T01-S056 | https://sources.news/p/skild-ai-ceo-robotics-brain-davos | secondary | 2026-09-02 | Alex Heath / Sources | 达沃斯对 Skild CEO 的访谈 |
| T01-S057 | https://jimfan.me/ | surrogate_primary | 2026-09-02 | Jim Fan | own site 个人主页，履历与项目 |
| T01-S058 | https://actuate.foxglove.dev/recordings/the-physical-turing-test-solving-general-purpose-robotics/ | surrogate_primary | 2026-09-02 | Jim Fan / Actuate 2025 | vendor docs 本人完整 keynote 录像页（Actuate 2025） |
| T01-S059 | https://research.nvidia.com/labs/gear/ | verified_primary | 2026-09-02 | NVIDIA GEAR | vendor docs，实验室页 |
| T01-S060 | https://www.youtube.com/watch?v=q1Q_lHJBxjI | surrogate_primary | 2026-09-02 | NVIDIA / Jim Fan | vendor docs 同场 keynote 的 NVIDIA YouTube 版 |
| T01-S061 | https://www.humanoidsdaily.com/news/nvidia-advances-humanoid-ai-with-gr00t-n15-eyeing-a-future-of-simulated-realities | secondary | 2026-09-02 | Humanoids Daily | GR00T N1.5 与合成数据口径 |
| T01-S062 | https://www.figure.ai/master-plan | surrogate_primary | 2026-09-02 | Brett Adcock / Figure | vendor docs，本人署名公司纲领 |
| T01-S063 | https://en.wikipedia.org/wiki/Figure_AI | secondary | 2026-09-02 | Wikipedia | 融资/估值/产量时间线交叉核对 |
| T01-S064 | https://podcasts.apple.com/us/podcast/episode119-the-future-is-humanoid-brett-adcock-on/id1792667231?i=1000705358042 | verified_primary | 2026-09-02 | Brett Adcock（受访） | 本人长访谈音频 |
| T01-S065 | https://www.sourcery.vc/p/breaking-brett-adcock-ceo-of-figure | secondary | 2026-09-02 | Sourcery | 2026-04 工厂参观 + 长访谈整理 |
| T01-S066 | https://singjupost.com/figure-ai-ceo-brett-adcocks-interview-shawn-ryan-show-transcript/ | dead | 2026-09-02 | Singju Post | Shawn Ryan Show 文字整理，curl 返回 000，Phase 4 需替换 |
| T01-S067 | https://www.engadget.com/ai/1x-neo-is-a-20000-home-robot-that-will-learn-chores-via-teleoperation-040252200.html | secondary | 2026-09-02 | Engadget | NEO 价格/遥操作/自主率拆分 |
| T01-S068 | https://www.humanoidsdaily.com/news/1x-ceo-details-neo-s-two-modes-and-defends-teleoperation-as-more-secure-than-a-cleaner | secondary | 2026-09-02 | Humanoids Daily | Børnich 两种模式与隐私机制表述 |
| T01-S069 | https://www.1x.tech/ | surrogate_primary | 2026-09-02 | 1X Technologies | vendor docs，产品与公司口径 |
| T01-S070 | https://www.cnbc.com/2026/08/20/unitree-humanoid-robots-chatgpt-moment.html | secondary | 2026-09-02 | CNBC | WRC 2026 王兴兴发言英文侧记录 |
| T01-S071 | https://www.globaltimes.cn/page/202608/1368611.shtml | secondary | 2026-09-02 | Global Times | 同一发言的第二个独立二手记录 |
| T01-S072 | https://en.wikipedia.org/wiki/Wang_Xingxing | secondary | 2026-09-02 | Wikipedia | 生平与公司时间线交叉核对 |
| T01-S073 | https://www.smarthey.com/detail/138113902837.html | secondary | 2026-09-02 | SmartHey | WRC 2026 现场中文侧记录 |
| T01-S074 | http://www.news.cn/energy/20251106/0ee9e5e4f67a482884b7ee537912895d/c.html | secondary | 2026-09-02 | 新华网 | 2025-11「两个 80%」表述 |
| T01-S075 | https://m.caixin.com/m/2025-09-11/102361371.html | secondary | 2026-09-02 | 财新 | 2025-09 数据与模型孰为核心的澄清 |
| T01-S076 | https://www.21jingji.com/article/20250809/herald/fecc404938f03df050143f46e4922853.html | secondary | 2026-09-02 | 21 世纪经济报道 | 2025-08 对 VLA 架构的怀疑 |
| T01-S077 | https://www.agibot.com.cn/article/315/detail/153.html | surrogate_primary | 2026-09-02 | 智元 / 彭志辉 | vendor docs，本人 APC 2026 演讲全文 |
| T01-S078 | https://en.wikipedia.org/wiki/AgiBot | secondary | 2026-09-02 | Wikipedia | 创始人与产品时间线交叉核对 |
| T01-S079 | https://www.agibot.com.cn/APC2026 | surrogate_primary | 2026-09-02 | 智元 | vendor docs，APC 2026 大会官方页 |
| T01-S080 | https://sai.sjtu.edu.cn/cn/facultydetails/zzjs/lucewu | verified_primary | 2026-09-02 | 上海交大人工智能学院 | own site 教师页，学术身份 |
| T01-S081 | http://www.news.cn/enterprise/20250521/8f877af8b7a7469c9cd1f0c3f98da2aa/c.html | secondary | 2026-09-02 | 新华网 | 2025-05 穹彻智能与本人企业侧长报道 |
| T01-S082 | https://www.mittrchina.com/news/detail/13746 | secondary | 2026-09-02 | MIT科技评论中国 | 卢策吾联合创立穹彻智能的首发报道 |
| T01-S083 | http://www.qingyuan.sjtu.edu.cn/a/lu-ce-wu1.html | verified_primary | 2026-09-02 | 上海交大清源研究院 | own site 人物页，第二处身份确认 |
| T01-S084 | https://pku-epic.github.io/ | surrogate_primary | 2026-09-02 | He Wang / PKU EPIC | own site 实验室主页，论文与 keynote |
| T01-S085 | https://arxiv.org/abs/2503.06669 | verified_primary | 2026-09-02 | AgiBot World Contributors | GO-1 与 AgiBot World 论文（跨轨同源 T04-S084） |
| T01-S086 | https://www.thewirechina.com/whos_who/wang-he-%E7%8E%8B%E9%B9%A4/ | secondary | 2026-09-02 | The Wire China | 王鹤履历、Galbot 融资与头衔（口径需注意） |
| T01-S087 | https://arxiv.org/abs/2410.23004 | verified_primary | 2026-09-02 | He Wang 团队 | DexGraspNet 2.0 论文 |
| T01-S088 | https://www.innovatorsunder35.com/the-list/he-wang/ | secondary | 2026-09-02 | MIT TR Innovators U35 | 第三方对其合成数据工作的描述 |
| T01-S089 | https://homes.cs.washington.edu/~fox/ | verified_primary | 2026-09-02 | Dieter Fox | own site 个人主页（边缘候选） |
| T01-S090 | https://nvidianews.nvidia.com/news/nvidia-open-humanoid-robot-reference-design | surrogate_primary | 2026-09-02 | NVIDIA | vendor docs，2026-06 GR00T 参考人形与合作机构 |
| T01-S091 | https://news.bjd.com.cn/2026/03/30/11659192.shtml | secondary | 2026-09-02 | 北京日报 | 2026-03 对话「天工」负责人熊友军（边缘候选） |
| T01-S092 | https://www.cie.org.cn/list_42/13893.html | verified_primary | 2026-09-02 | 中国电子学会 | 学会/协会 WRC 论坛，熊友军演讲条目 |
| T01-S093 | https://www.ncsti.gov.cn/kjdt/scyq/bjjjjskfq/jkdt/202604/t20260401_242661.html | verified_primary | 2026-09-02 | 首都科技创新服务平台 | 2026-04 熊友军与创新中心报道 |
| T01-S095 | https://techcrunch.com/2025/10/10/the-world-is-just-not-quite-ready-for-humanoids-yet/ | secondary | 2026-09-02 | TechCrunch | 2025-10 人形准备度的行业侧综述 |
| T01-S096 | https://citris-uc.org/citris-researcher-publishes-papers-on-reality-of-humanoid-robots/ | surrogate_primary | 2026-09-02 | CITRIS, UC | own site 机构页，Goldberg 两篇论文的机构侧记录 |

**Manifest 统计（机械计数）**：共 **94** 条。`verified_primary` **34** 条、`surrogate_primary` **27** 条、`secondary` **32** 条、`dead` **1** 条 —— 一手类（verified + surrogate）占 **64.9%**，纯 `verified_primary` 占 **36.2%**。全部 94 条 `last_checked` 均为 2026-09-02。
**bucket 是怎么定的**：全部 URL 用 `skill/tools/research/source_verifier.py classify` 跑过一遍，取自动结果；仅在符合 Surrogate Sources Policy 时**向上**标为 `surrogate_primary`（figure 本人博客 / 本人 talk 录像 / 本人账号 → note 写 `own site` 或 `own publication`；公司技术博客与项目页 → note 写 `vendor docs`；学会 / 协会页 → note 写 `协会` 或 `学会`），**没有任何一条被人工降级**。`surrogate_primary` 的 note 全部含规定关键词，未使用 `official`。
**黑名单零命中**：全文（含正文）不含知乎 / 微信公众号 / 百度百科 / CSDN / 简书 / 51CTO / 腾讯云 / 阿里云社区 / Quora / G2 / Capterra / prnewswire / businesswire / SEO 榜单。检索过程中出现过的阿里云创业频道与腾讯新闻链接**已主动剔除，未进正文也未进 manifest**。
**一条 dead**：T01-S066（Shawn Ryan Show 访谈文字整理页，curl 返回 000），保留编号并标注，供 Phase 4 替换。
**未进 manifest 的不可达线索（3 条）**：`rail.eecs.berkeley.edu`、`people.eecs.berkeley.edu/~svlevine/`、`ceai.caai.cn` —— 均 curl 返回 000，正文引用时已注明「未验证 URL、不挂 evidence」。

## 1. 总览表

> 「本人长材料」= 本人署名的长文 / 本人 ≥30 分钟的 talk 或受访音视频 / 本人共同署名的论文与博客。**只有 ✅ 的人，其观点才可以在 Phase 2 里当作「他的思想」使用；❌ 的人只能用作「有日期、有场合的公开表态」或人物地图。**

| # | 姓名 | 核心身份 | 一句话贡献 | 本人长材料 | 来源数（含跨轨） | 可信度 |
|---|------|---------|----------|-----------|------------|-------|
| 1 | Rodney Brooks | MIT 名誉教授 + Robust.AI CTO | 用可反驳的技术主张（数据模态缺口）给人形时间表泼冷水 | ✅ 多篇本人长文 | 8 | high |
| 2 | Russ Tedrake | MIT 教授 + TRI LBM 高级副总裁 | 优化派核心人物同时是学习派论文作者，证明两派对立是伪命题 | ✅ 长 talk + 署名辩论 | 11 | high |
| 3 | Sergey Levine | Berkeley 教授 + Physical Intelligence 联创 | 把「机器人基础模型」做成可下载的权重 | ✅ 多档 ≥1h 播客 | 15 | high |
| 4 | Chelsea Finn | Stanford 助理教授 + PI 联创 | ALOHA / Mobile ALOHA 让遥操作采集成为可复现范式 | ✅ YC 完整 talk（未抓字幕） | 12 | medium-high |
| 5 | Pieter Abbeel | Berkeley 教授 + Amazon FAR 共同负责人 | 一代人的博导 + 用播客给这一行做人物索引 | ❌ 他是提问者不是受访者 | 5 | medium |
| 6 | Ken Goldberg | Berkeley 讲席教授 + Robot Learning Foundation 主席 | 「10 万年数据鸿沟」把乐观论拉回可计算问题 | ✅ 本人社论全文 | 7 | high |
| 7 | Shuran Song | Stanford 助理教授（REAL 实验室） | Diffusion Policy + UMI，用方法本身回应「遥操作太贵」 | ❌ 只有论文与项目页 | 7 | medium |
| 8 | Marc Raibert | RAI Institute 执行主任 + BD 创始人 | 把「像动物一样动」变成工程学科 | ❌ 近期长材料未取到 | 6 | medium |
| 9 | Marco Hutter | ETH 教授（50%）+ RAI Zurich 负责人（50%）+ ANYbotics 联创 | 腿足学习式控制跑通并商业化 | ⚠️ 只有机构话题的官方访谈 | 9 | medium-high |
| 10 | Sangbae Kim | MIT 副教授（停薪留职）+ Meta 机器人架构师 | 「硬件是使能者」这一派最清晰的代言人 | ❌ 只有二手长文里的引语 | 4 | medium |
| 11 | Deepak Pathak | CMU 副教授 + Skild AI CEO | 端到端腿足 + 「一个大脑装进任何本体」 | ❌ 本人长材料未取到 | 9 | medium |
| 12 | Jim Fan | NVIDIA GEAR 共同负责人 | 「物理图灵测试」这个评价框架比喻的作者 | ✅ 完整 keynote 录像（未抓字幕） | 9 | medium |
| 13 | Brett Adcock | Figure AI 创始人兼 CEO | 把人形叙事推到有月度产量可报的阶段 | ✅ 本人署名 Master Plan + 多档长访谈 | 7 | medium-high（叙事）/ low（技术） |
| 14 | Bernt Børnich | 1X Technologies CEO | 把「遥操作是产品本身」摆上台面 | ❌ 原始访谈音频未取到 | 5 | medium |
| 15 | 王兴兴 | 宇树科技创始人兼 CEO | 本体价格改写者 + 公开唱衰当前 VLA 架构 | ❌ **一手长材料完全未获取** | 11 | low-medium |
| 16 | 彭志辉「稚晖君」 | 智元创新联创兼 CTO | 把「能不能稳定干活」立为行业新问题 + 开源百万级真机数据 | ✅ 公司官网刊载的本人演讲全文 | 9 | medium-high |
| 17 | 卢策吾 | 上海交大教授 + 穹彻智能联创 | GraspNet / AnyGrasp，抓取评测协议的统一者 | ❌ **一手长材料未获取** | 7 | low-medium |
| 18 | 王鹤 | 北大助理教授 + 银河通用创始人 | 中国侧「十亿级合成数据预训练」路线最系统的执行者 | ❌ **一手长材料未获取** | 7 | low-medium |

**筛选统计**：共探查候选 **28 人**（含 Aaron Saunders、Scott Kuindersma、Jonathan Hurst、Pulkit Agrawal、Carolina Parada、Karol Hausman、Dieter Fox、熊友军、Frank Park、Aude Billard、Animesh Garg、Daniela Rus 等），**保留 18 人**成卡；其余进 §3.5「边缘候选」。

## 2. Figure 卡片

### 1. Rodney Brooks

- **One-liner**: 行为主义机器人学奠基者，也是当下**唯一持续用可核对的书面记录**给人形 / 具身 AI 时间表泼冷水的一线创业者——他的批评不是「太快了」这种情绪，而是「你们采的数据里没有触觉和力，所以学不出灵巧」这种可反驳的技术主张 (evidence: [T01-S001, T01-S002, T04-S115])
- **核心身份**: MIT 计算机科学与人工智能实验室名誉教授（Panasonic Professor of Robotics, emeritus）；iRobot、Rethink Robotics（已关停）、Robust.AI 三家公司的联合创始人，现任 Robust.AI 的 CTO (evidence: [T01-S005, T01-S006])
- **利益关系（必须点名）**: 他**本人是仓储机器人公司 Robust.AI 的 CTO 与联创**，公司做的是「人机协作推车（Carter）」这类**非人形**的仓储设备 (evidence: [T01-S005])。他批评人形路线的同时，自己的商业押注就在「不做人形、做人机协作的轮式设备」这条线上——这不使他的技术论证失效，但读他的文章要知道这层关系。另一层：他的博客本身不接广告、不融资，是纯个人发声阵地，且他公开承诺把 2018 年的预测跟踪到自己 95 岁生日（32 年）(evidence: [T01-S002])。
- **代表作品**:
  - "Intelligence without Representation"（*Artificial Intelligence*, 1991）——包容式架构（subsumption architecture）与行为主义机器人学的纲领性论文 (evidence: [T04-S115, T04-S116])
  - "Why Today's Humanoids Won't Learn Dexterity"（个人博客，2025-09-26）——本轮人形浪潮最被引用的一篇技术性批评 (evidence: [T01-S001])
  - 年度 "Predictions Scorecard" 系列（2018 起，每年 1 月 1 日更新，2026-01-01 为第八年）(evidence: [T01-S002])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 *Why Today's Humanoids Won't Learn Dexterity*（本人长文，2025-09-26）https://rodneybrooks.com/why-todays-humanoids-wont-learn-dexterity/ (evidence: [T01-S001])
  - 📖 *Predictions Scorecard, 2026 January 01*（本人长文，逐条自评 2018 年预测）https://rodneybrooks.com/predictions-scorecard-2026-january-01/ (evidence: [T01-S002])；博客索引页可确认发文序列与日期 https://rodneybrooks.com/blog/ (evidence: [T01-S004])
  - 🎬 *Rodney Brooks Explains What Robust.AI Is Actually Doing*（IEEE Spectrum 长访谈，他解释自己的产品选择与不做人形的理由）https://spectrum.ieee.org/robust-ai-rodney-brooks (evidence: [T01-S005])
  - 🎙️ *Four Time Scales for Technology Development and Deployment*（本人长文，2026-08-01，把「研究创新速度 / 造势速度 / 部署速度」拆开谈）https://rodneybrooks.com/four-time-scales-for-technology-development-and-deployment/ (evidence: [T01-S003])
- **核心思想关键词**: 触觉与力数据缺口（touch/force data gap）、部署速度 ≠ 研究速度、可核对的带日期预测（NET / BY / NIML）、「视觉数据不是对的数据」、包容式架构 / 无表征的智能
- **他的具体批评（这是 Wave 1 留下的缺口，本轨补上）**:
  1. **原话**（2025-09-26 本人博客）：believing that this will happen any time within decades is pure fantasy thinking (evidence: [T01-S001])。上下文是「人形机器人做到人类那样的手工活」这件事，**不是**泛指所有机器人进展。
  2. **原话**：Collecting just visual data is not collecting the right data. There is so much more going into human dexterity that visual data completely leaves out (evidence: [T01-S001])。
  3. **原话**：We as a species have not developed technologies to capture touch, to store touch, to transmit touch (evidence: [T01-S001])——他把触觉数据的缺席类比成「我们有海量文本和图像的采集/存储/传输传统，但触觉一样都没有」。
  4. **原话**：No human-like robot hands have demonstrated much in the way of dexterity, in any general sense (evidence: [T01-S001])。
  5. **要义转述**：他点名了 Figure 与 Tesla（Optimus）作为「押注看大量人手视频就能学出灵巧」的代表 (evidence: [T01-S001])。
  6. **他的替代方案（要义转述）**：先建触觉/力的采集基础设施（文中引用 MIT Agrawal 组的触觉手套类工作），把学习目标从「状态→动作」改成「计划 + 触觉调制」，然后接受这是多年工程 (evidence: [T01-S001])。
  7. **原话**（2026-01-01 记分卡）：The declarations being made about humanoid robots are just not plausible. / We're at peak popular hype in all of robotics, AI, and machine learning (evidence: [T01-S002])。
- **voice_samples**:
  - 客户 / 外行解释样本（要义转述，2025-09-26 博客）：他解释「为什么视频不够」时用的是采集史类比——人类给文本和图像建了几百年的采集、存储、传输传统，给触觉一样都没建；所以你在网上根本找不到「触觉数据集」这种东西可以去爬。(source: T01-S001, 要义转述)
  - 同业 / 技术讨论样本（原话，≤30 词）：They are making a bet that machine learning from watching lots and lots of motions of people's hands will be sufficient to learn dexterity (source: T01-S001, 原话)
  - 公开立场 / 预测样本（原话）：The declarations being made about humanoid robots are just not plausible.（source: T01-S002, 原话）；配套的方法论是他把预测写成 NET（不早于某年）/ BY（某年之前）/ NIML（我有生之年不会，截止 2050）三种可判定形式，并逐年自评「太乐观 / 太悲观 / 准 / 打太极」(source: T01-S002, 要义转述)
- **sub_skill_candidate**: `true` — 有多年连续的本人长文、方法论自洽（时间尺度分离 + 可判定预测 + 数据模态缺口），且他是这一行**唯一**把「如何不被 demo 骗」写成可复用程序的人。
- **dual_role**: `academic + founder`（MIT 名誉教授 + 三家公司联创，现任 CTO）
- **最近 12 个月动态**:
  - 2025-09-26 发表 "Why Today's Humanoids Won't Learn Dexterity"，直接引发行业公开辩论 (evidence: [T01-S001, T01-S007])
  - 2026-01-01 发布第八年 Predictions Scorecard，判断「机器人/AI/ML 全行业处于大众造势的峰值」(evidence: [T01-S002])
  - 2026-08-01 发表 "Four Time Scales for Technology Development and Deployment"，把「研究、造势、部署」三种速度分开 (evidence: [T01-S003])
- **争议 / 批评**:
  - **有正面交锋**。Scott Walter 公开反驳他犯了「高悬果实谬误」（High-Hanging Fruit Argument）——即把「人形做不到人类的全部」偷换成「人形什么都做不了」；Walter 的论据是 Brooks 举的每个「没触觉做不了」的例子，他都能找到反例任务 (evidence: [T01-S007])。**注意口径**：本轨只核到 Humanoids Daily 对这场辩论的整理，未核到 Walter 本人原始长文的可访问 URL，因此 Walter 的具体措辞按二手整理引用，不标原话。
  - **未见 Figure 或 Tesla 官方对该文的公开回应**（本轨未检到）。行业侧的同期反应见 TechCrunch 2025-10-10《The world is just not quite ready for humanoids yet》(evidence: [T01-S095])。
  - 常见的第二类反驳（跨源、非针对本文）：Brooks 自己在 Rethink Robotics 的商业尝试失败过（公司 2018 年关停），因此有人认为他对「消费级/通用机器人时间表」的悲观带有个人经历色彩。**本轨未核到有署名的人公开这样说，因此只作为背景事实列出，不作为「行业批评」记入。**
- **可信度自评**: **high** — 本人长材料充足（多篇 ≥2000 词的自撰博客 + IEEE Spectrum 长访谈），观点跨时间一致，且他自己保存了可被打脸的预测记录。

---

### 2. Russ Tedrake

- **One-liner**: 这一行**最重要的反例人物**——优化派与控制理论的核心教师（《Underactuated Robotics》《Robotic Manipulation》两本在线教材的作者），同时是 Diffusion Policy 与 OpenVLA 的共同作者、TRI 大行为模型（LBM）负责人；他证明了「模型派 vs 学习派」在人身上根本不成立 (evidence: [T04-S008, T04-S009, T04-S076, T04-S077, T01-S009])
- **核心身份**: MIT 电气工程与计算机科学教授、CSAIL；Toyota Research Institute 的 Large Behavior Models 高级副总裁 (evidence: [T01-S009, T01-S016])
- **利益关系**: TRI 是丰田全资的研究机构，他在其中负责 LBM 这条产品化前的研究线；同时与 Boston Dynamics 合作在 Atlas 上跑 LBM (evidence: [T01-S019, T01-S020])。**他的学术输出（教材、Drake 库）与雇主的产品线不冲突，但「LBM 有效」这个结论对 TRI 有直接价值，读他的评测数字时要意识到这一点——不过他团队自己就是把这件事做得最保守的（见下）。**
- **代表作品**: 《Underactuated Robotics》与《Robotic Manipulation》两本 rolling 更新的在线教材 (evidence: [T04-S008, T04-S009])；Drake 工具箱；Diffusion Policy 共同作者 (evidence: [T04-S076])；OpenVLA 共同作者 (evidence: [T04-S077])；*A Careful Examination of Large Behavior Models for Multitask Dexterous Manipulation*（TRI LBM Team，2025-07，arXiv:2507.05331）(evidence: [T01-S016, T01-S017])
- **值得读 / 听 / 看的 3 件事**:
  - 🎬 *Multitask Transfer in TRI's Large Behavior Models for Dexterous Manipulation*（Stanford seminar，2025-04-25，本人 ≥1 小时 talk）https://www.youtube.com/watch?v=TN1M6vg4CsQ (evidence: [T01-S015])
  - 📖 *A Careful Examination of Large Behavior Models*（本人团队论文项目页 + arXiv 全文）https://toyotaresearchinstitute.github.io/lbm1/ (evidence: [T01-S016, T01-S017])
  - 📖 ICRA 2025 数据辩论中他署名的一节 "Manipulation requires 'common sense'; large data and large models can provide it"（*Science Robotics*, 2025-08-27）(evidence: [T01-S009])
  - 🎬 *Large Behavior Models for Dexterous Manipulation*（本人另一场公开 talk 录像）https://www.youtube.com/watch?v=y05L6pYWBc0 (evidence: [T01-S021])
- **核心思想关键词**: 常识（common sense）是低层控制的必需品而非只是语义层的、多任务预训练带来的是「更少演示学会新技能」而非零样本、统计功效（statistical power）与盲测 A/B、恢复行为（recovery maneuvers）、「解决机器人学是一个很长期的议程」
- **他在公开辩论中的实际立场（原话，2025-08-27 *Science Robotics*）**:
  - I do believe that the next most impactful steps toward "solving" robotics lie in large-scale data collection and large pretrained models. How could I not? (evidence: [T01-S009]) —— 他被分配到「data will solve robotics = true」一方，但他自己的表述带明确限定。
  - Large-scale pretraining from diverse multitask data is the best (only?) way that I know to program "common sense." (evidence: [T01-S009])
  - many people underestimate how essential common sense is for low-level control (evidence: [T01-S009])
  - For me, "solving" robotics is a very long-term agenda. ... We are in the early phases, where everything feels messy. (evidence: [T01-S009])
- **他团队做的最有价值的一件「不利于自己」的工作（要义转述）**: TRI LBM 论文跑了 1800+ 次真机 rollout、用**盲测 A/B** 做对比，结论包含三条负面/警示项——(a) **未微调的预训练 LBM 结果参差**，没有稳定优于从零单任务训练；(b) 数据归一化这类「细枝末节的设计选择」的影响常常压过架构或算法改动；(c) 机器人领域常规的评测样本量不足，测出来的可能是统计噪声 (evidence: [T01-S016])。正面结论是：在困难场景下达到同等表现所需数据可少 3–5 倍，且收益在几百小时这种不大的规模上就出现 (evidence: [T01-S016])。**口径提醒：3–5× 是「达到同等成功率所需演示数据量的比值」，不是成功率本身。**
- **voice_samples**:
  - 同业 / 学术辩论样本（原话）：I do believe that the next most impactful steps toward "solving" robotics lie in large-scale data collection and large pretrained models. How could I not? (source: T01-S009, 原话)
  - 技术论证样本（原话）：Most people agree that large models are useful for manipulation tasks that require common-sense language understanding ... but many people underestimate how essential common sense is for low-level control (source: T01-S009, 原话)
  - 对自己方法边界的样本（要义转述）：他用 TRI 团队切苹果的例子说明，真正打动他的不是「能切」，而是苹果块滑走时机器人做出的细微补救动作；而这些补救动作是通过往演示数据里补录恢复行为、再经预训练迁移而「自动出现」的 (source: T01-S009, 要义转述)
- **sub_skill_candidate**: `true` — 长材料极其充足（两本 rolling 教材 + 多场 1 小时以上 seminar + 署名辩论文章），且他的思维方式（把优化、控制与学习当成一套系统里的不同部件，而不是路线之争）正是这一行最稀缺的整合视角。
- **dual_role**: `academic + engineering`（MIT 教授 + TRI 研发负责人 + Drake 开源维护者）
- **最近 12 个月动态**:
  - 2025-04-25 Stanford seminar 公布 TRI LBM 的多任务迁移量化结果 (evidence: [T01-S015])
  - 2025-05-26~29 ICRA 2025（亚特兰大）全会辩论中代表「数据方」发言，2025-08-27 该辩论以 Viewpoint 形式发表于 *Science Robotics* (evidence: [T01-S009])
  - 2025-07 LBM 论文上 arXiv，强调盲测与统计功效 (evidence: [T01-S016, T01-S017])
  - 与 Boston Dynamics（Scott Kuindersma）联合把 LBM 用到 Atlas 上做全身操作 (evidence: [T01-S019, T01-S020])
- **争议 / 批评**:
  - **有正面交锋，且是同一篇文章内**。Frank Park（首尔大学）在同一场辩论中直接反驳「把视觉/语言的模型硬套到机器人上」这条路：原话 expecting a parallel revolution in robotics is premature at best and wishful thinking at worst，以及 Rather than force-fitting models developed for vision and language to robots, new models that capture the inductive biases inherent to robotics are needed (evidence: [T01-S009])。Aude Billard（EPFL）则从科学方法论角度反驳：I do not believe that data alone will "solve" robotics and automation，并用天文学「少而精的观测点」作类比 (evidence: [T01-S009])。
  - **Tedrake 没有被指责「只会讲学习」**——他在同一篇里明确说「解决机器人学是长期议程，我们仍会需要定理来指导」(evidence: [T01-S009])。**Phase 2 不要把他写成纯学习派。**
- **可信度自评**: **high** — 本人长材料多、跨年份立场一致、且有署名的公开辩论记录可逐句核对。

---

### 3. Sergey Levine

- **One-liner**: 「机器人基础模型」这条路线最系统的推动者与最勤奋的解释者——从 2016 年端到端视觉运动策略到 π 系列 VLA，他把「用一个模型控任意机器人做任意任务」从口号做成了可下载的权重 (evidence: [T04-S068, T04-S078, T01-S025, T05-S074])
- **核心身份**: UC Berkeley 电气工程与计算机科学教授（RAIL 实验室）；Physical Intelligence 联合创始人 (evidence: [T01-S022, T01-S025])
- **利益关系（必须点名）**: **他是估值极高的具身基础模型创业公司的联创**，公司公开路线就是「通用优于专用」；他在播客里的每一句「通用模型会赢」都同时是技术判断和融资论点 (evidence: [T01-S026, T01-S027])。**对冲事实**：PI 把 π0 权重与代码开源（openpi 仓库），这在同赛道公司里少见，使得他的部分主张可被外部复现 (evidence: [T05-S074, T01-S022])。
- **代表作品**: End-to-End Training of Deep Visuomotor Policies（JMLR 2016）(evidence: [T04-S068])；QT-Opt (evidence: [T04-S070])；π0（流匹配 VLA，2024-10）(evidence: [T04-S078])；π0.5（开放世界泛化，2025-04）(evidence: [T01-S025, T01-S022])；π*0.6 / π0.7 (evidence: [T01-S023])
- **值得读 / 听 / 看的 3 件事**:
  - 🎙️ *π0: A Foundation Model for Robotics*（TWIML #719，本人 ≥1 小时技术访谈，讲架构、数据采集、FAST tokenizer）https://twimlai.com/podcast/twimlai/cf800-a-foundation-model-for-robotics (evidence: [T01-S026])
  - 🎙️ *Sergey Levine — Building LLMs for the Physical World*（Invest Like the Best，2026-03-31，约 1 小时 7 分）(evidence: [T01-S027])
  - 📖 π0.5 技术博客与论文（本人共同作者，含明确的失败与局限自述）https://www.pi.website/blog/pi05 / arXiv:2504.16054 (evidence: [T01-S022, T01-S025])
  - 🎙️ *#331 Sergey Levine: The Robot Revolution Nobody Is...*（Eye On A.I.，2026-04-12，59 分钟）(evidence: [T01-S028])
- **核心思想关键词**: 开放世界泛化（open-world generalization）、通用性比专用性更可扩展、数据的**广度**（多少个不同环境）比总量更关键、动作表示（离散 token vs 流匹配）、从经验中学（π*0.6 的 RL 后训练）
- **他自己承认的边界（原话，π0.5 博客，2025-04-22）**:
  - π0.5 can perform a variety of tasks in entirely new homes. It does not always succeed on the first try (evidence: [T01-S022])
  - π0.5 is far from perfect, and it often makes mistakes both in terms of its high-level semantic deductions（后接运动控制层面的错误）(evidence: [T01-S022])
- **数字口径（这一条要抄给下游）**: π0.5 博客页面给出的是 Follow Rate 与 Success Rate 的百分比条（本轨读到的区间约 31%–94%），但**该页面上没有给出测试了几个家庭、每个任务跑了多少次试验** (evidence: [T01-S022])。**引用 π0.5 的任何百分比时必须补上「作者自评、分母未在博客页面公开」**。论文（arXiv:2504.16054）另有 scaling study，变量是「训练数据里见过多少个不同环境」(evidence: [T01-S022, T01-S025])。
- **voice_samples**:
  - 客户 / 外行解释样本（要义转述）：他解释「为什么机器人难」时的标准打法是把它换成一个数据问题——不是机器人笨，是我们从没有过「视频输入 + 关节指令」配对起来的互联网级数据；语言模型有的东西机器人一样都没有。(source: T01-S026, 要义转述)
  - 同业 / 技术讨论样本（原话，π0.5 博客）：π0.5 is far from perfect, and it often makes mistakes both in terms of its high-level semantic deductions (source: T01-S022, 原话)
  - 公司立场样本（**主持人转述，不是 Levine 原话**）：Invest Like the Best 主持人 Patrick O'Shaughnessy 把 PI 的论点概括为「通用性比专用性更可扩展——跨很多机器人、很多任务训练出的模型，最终会打败任何为单件事造的系统」 (source: T01-S027, 主持人转述，非本人原话)
- **sub_skill_candidate**: `true` — 材料充足（多档 1 小时级技术播客 + 本人共同署名的博客与论文），思想体系自洽且**可被他自己开源的东西检验**。
- **dual_role**: `academic + founder`
- **最近 12 个月动态**（PI 官方博客时间线，他为共同作者/联创）:
  - 2025-11-17 π*0.6：「从经验中学」的 VLA（RL 后训练）(evidence: [T01-S023])
  - 2025-12-22 *Moravec's Paradox and the Robot Olympics*：PI 用 π0.6 微调打「机器人奥运会」五个项目 (evidence: [T01-S024])
  - 2026-02-24 *The Physical Intelligence Layer*（对外合作/分层）；2026-03 记忆与在线 RL 两篇；2026-04-16 π0.7 (evidence: [T01-S023])
  - 2026-03~05 密集接受长播客访谈（Invest Like the Best、Colossus、Eye on AI、A3 Automated）(evidence: [T01-S027, T01-S028])
- **争议 / 批评**:
  - **来自 Ken Goldberg 的量化质疑（非点名，但直接针对该路线）**：真机遥操作数据线性不可扩、互联网视频抬不回三维、仿真对操作不可靠——因此「等数据解决」的时间表不成立 (evidence: [T01-S008])。**注意**：Goldberg 的社论参考文献里恰好引用了 PI 的 Kevin Black 在 X 上做的「语言数据 vs 机器人数据」对比图，说明双方共享同一个事实基础、只在结论上分歧 (evidence: [T01-S008])。
  - **来自 Rodney Brooks 的模态质疑**：视觉数据里没有触觉与力，因此这条路学不出灵巧 (evidence: [T01-S001])。**本轨未检到 Levine 或 PI 对 Brooks 该文的公开回应。**
  - **来自 Frank Park 的方法论质疑**：把视觉/语言的模型硬套到机器人上是「往好里说不成熟、往坏里说一厢情愿」(evidence: [T01-S009])。
  - **评测口径质疑（跨源、结构性）**：VLA 子领域缺公共基准，性能数字均来自作者自建评测 (evidence: [T04-S078, T04-S084])。
- **可信度自评**: **high** — 本人长材料多且新，且有开源权重可交叉验证。

---

### 4. Chelsea Finn

- **One-liner**: 遥操作数据这条路线的关键推手——ALOHA / Mobile ALOHA 让「低成本硬件 + 人类演示」成为学术界与创业公司都能复现的采集范式，她同时是 Physical Intelligence 联创 (evidence: [T04-S075, T04-S079, T01-S029])
- **核心身份**: Stanford 计算机与电气工程助理教授，IRIS 实验室（Intelligence through Robotic Interaction at Scale）负责人；Physical Intelligence 联合创始人 (evidence: [T01-S029, T01-S030])
- **利益关系**: 与 Levine、Hausman 同为 PI 联创，公开发言与 PI 的「通用基础模型」路线一致 (evidence: [T01-S029, T01-S022])。她同时在 Stanford 教 CS224R（深度强化学习），2025 与 2026 春季均开课——这条线是她的学术身份而非公司身份 (evidence: [T01-S029])。
- **代表作品**: MAML（模型无关元学习，她的博士工作）；ALOHA + ACT（action chunking，2023）(evidence: [T04-S075])；Mobile ALOHA（全身遥操作，2024）(evidence: [T04-S079])；π0 / π0.5 共同作者 (evidence: [T04-S078, T01-S022])
- **值得读 / 听 / 看的 3 件事**:
  - 🎬 *Building Robots That Can Do Anything*（Y Combinator AI Startup School，2025-06-17，本人完整 talk）https://www.youtube.com/watch?v=a8-QsBHoH94 (evidence: [T01-S031])
  - 🎬 *Data-Driven Pre-Training and Post-Training for Robot Foundation Models*（ICLR 2025 第 7 届 Robot Learning Workshop 特邀报告）https://iclr.cc/virtual/2025/10000222 (evidence: [T01-S032])
  - 📖 Mobile ALOHA 论文（全身遥操作 + 静态数据协同训练）arXiv:2401.02117 (evidence: [T04-S079])
  - 🎙️ Y Combinator Startup Podcast 同名音频版 https://www.ycombinator.com/library/Mj-chelsea-finn-building-robots-that-can-do-anything (evidence: [T01-S033])
- **核心思想关键词**: 预训练 + 后训练两段式（robot foundation model 的 post-training 是她 ICLR 报告的主题）、大规模交互中的智能（IRIS 的字面含义）、低成本硬件让数据采集可复制、physical common sense（物理常识）
- **voice_samples**:
  - 客户 / 外行解释样本（要义转述，YC talk）：她讲自己团队的历程时的口径是「从抓取和视觉的早期实验，走到今天叠衣服、收拾厨房、跨任务泛化——全程不写手工代码，靠的是可扩展的基础模型和大规模数据集」 (source: T01-S031, 要义转述)
  - 学术讨论样本（要义转述）：她把机器人基础模型明确拆成「数据驱动的预训练」与「后训练」两段，这是她 ICLR 2025 特邀报告的标题结构 (source: T01-S032, 要义转述)
  - ⚠️ **本轨未逐字取到 ≥30 字的 Finn 直接引语**（YC talk 与 ICLR 报告本轨只取到页面描述与标题，未抓字幕）。**下游若需要她的原话，必须自行抓 https://www.youtube.com/watch?v=a8-QsBHoH94 的字幕**，不要从本文件推断。
- **sub_skill_candidate**: `false` — 重要且材料够（YC talk 是完整长 talk），但她的公开表达与 Levine / PI 的路线高度重合，单独蒸馏边际信息量低；建议与 Levine 合并成「PI / VLA 学派」一个 sub-skill。
- **dual_role**: `academic + founder`
- **最近 12 个月动态**:
  - 2025-06-17 YC AI Startup School 长 talk (evidence: [T01-S031])
  - 2025-04-22 起为 π0.5 共同作者 (evidence: [T01-S022])
  - 2026 年在 ICML 有关于「涌现式物理泛化 / π0.7」的报告，以及 RLxF（RL from World Feedback）workshop 上关于「超越标量奖励瓶颈」的报告 (evidence: [T01-S034])
  - 2026 春季继续在 Stanford 开 CS224R (evidence: [T01-S029])
- **争议 / 批评**:
  - **遥操作数据路线本身被公开质疑**：Goldberg 的社论明确指出遥操作是「人类训练员一动一动地遥控机器人反复做同一件事」，产出与投入线性相关，扛不住 10 万年的量级差 (evidence: [T01-S008])。Shuran Song 团队的 UMI（手持夹爪、脱离机器人采集）本身就是对遥操作成本的一次公开表态 (evidence: [T04-S080])。
  - **ALOHA 的数字口径常被误引**：ACT 论文报的 80–90% 是「6 个真机任务、训练场景内、已知物体」，不是通用成功率 (evidence: [T04-S075])。
  - 本轨**未检到**针对 Finn 个人的公开点名批评。
- **可信度自评**: **medium-high** — 长 talk 存在且可核，但本轨未抓到她的逐字原话，voice DNA 维度偏弱（已标注）。

---

### 5. Pieter Abbeel

- **One-liner**: 这一行最重要的**入口人物**——他既是深度 RL 与机器人学习一代人的博导（Levine、Finn、Chen 等出自其门下或合作），又靠 *The Robot Brains Podcast* 把这一行几乎所有关键人物请到麦克风前，是研究「谁在这一行说什么」的最好索引 (evidence: [T05-S009, T05-S010])
- **核心身份**: UC Berkeley 教授（BAIR、Berkeley Robot Learning Lab）；Covariant 联合创始人兼首席科学家；2024-08 Amazon 通过许可 Covariant 技术并雇佣其创始团队后，他以 Amazon Scholar / Distinguished Scientist 身份共同领导 Amazon 的 Frontier AI & Robotics 团队；2025-12 起还负责 Amazon AGI 组织内的大语言模型方向 (evidence: [T01-S035, T01-S036])
- **利益关系（必须点名）**: 他是**被大厂收编的创业者**——Covariant 的技术与团队被 Amazon 于 2024-08 收下 (evidence: [T01-S035, T01-S036])。他现在的公开发言同时受 Berkeley 学术身份和 Amazon 雇主身份约束；他的播客是他自己的平台（Acast 托管），选题与嘉宾由他决定 (evidence: [T05-S009, T05-S010])。**播客的结构性偏向要注意**：嘉宾以他的学术圈层与硅谷创业圈为主。
- **代表作品**: *The Robot Brains Podcast*（他本人主持，嘉宾覆盖 Fei-Fei Li 等）(evidence: [T05-S009, T05-S010])；Covariant「机器人基础模型」商业化尝试；深度 RL 与模仿学习的一批奠基性工作与 Berkeley CS287/CS285 课程线（**注意：Wave 1 已记录 Berkeley 课程页在本次网络环境不可访问，本轨复测 `rail.eecs.berkeley.edu` 与 `people.eecs.berkeley.edu/~svlevine/` 均连接失败（curl 返回 000），因此这两条不进 manifest、不作 evidence**）
- **值得读 / 听 / 看的 3 件事**:
  - 🎙️ *The Robot Brains Podcast*（他本人主持的长访谈系列，季播）https://therobotbrains.ai/ (evidence: [T05-S009])
  - 📖 Amazon Science 作者页（他在 Amazon 期间的论文与技术输出入口）https://www.amazon.science/author/pieter-abbeel (evidence: [T01-S035])
  - 📖 UC Berkeley 研究人物页（学术身份与研究方向的机构侧确认）https://vcresearch.berkeley.edu/faculty/pieter-abbeel (evidence: [T01-S037])
  - ⚠️ **本轨未取到他 2025-2026 年的单场 ≥30 分钟本人受访长材料**（他主要是**主持人**而非受访者）；他的长材料以「他主持的每一集」形式存在。
- **核心思想关键词**: 机器人基础模型（Covariant 的商业主张）、深度 RL 到真机的迁移、把研究者推到公众面前（播客的编辑立场）、「谁在做什么」的地图能力
- **voice_samples**:
  - ⚠️ **暂未找到 ≥30 字的本人直接原话片段**。他的公开语料主要是访谈中的提问，本轨未抓取字幕。**下游若要他的 voice DNA，必须从 https://therobotbrains.ai/ 的具体集数抓字幕**，不要从本文件推断。
  - 可用的间接信号（要义转述）：他的公开定位是「让做机器人大脑的人自己说话」——播客自述是「每一集见一位试图给机器人造大脑的人」 (source: T05-S009, 要义转述)
- **sub_skill_candidate**: `false` — 影响力毫无疑问在前五，但本轨没拿到他本人的长篇观点材料（他的角色是提问者）。**他更大的价值是 Track 05 的信息源索引，而不是 Phase 2 的思想蒸馏对象。**
- **dual_role**: `academic + founder`（+ 媒体主理人）
- **最近 12 个月动态**:
  - 2025-12 起兼任 Amazon AGI 组织的大语言模型方向负责人，同时继续机器人方向 (evidence: [T01-S036])
  - The Robot Brains Podcast 的最近更新时间本轨未确认（Wave 1 已标注同一问题）(evidence: [T05-S009, T05-S010])
- **争议 / 批评**:
  - **Covariant 的结局本身就是一次公开的路线检验**：一家以「机器人基础模型」为叙事的公司，最终以技术许可 + 团队被 Amazon 吸收的方式结束独立运营 (evidence: [T01-S035, T01-S036])。这被同赛道创业者与投资人反复引用为「通用机器人 AI 的商业化比技术更难」的案例。**本轨未检到有具名人士就此公开批评 Abbeel 本人**，因此只记事实、不记批评。
  - **播客的利益结构**：主持人同时是同赛道创业者与投资参与者，嘉宾选择与提问角度不中立——这是使用该信息源时的已知偏差（Wave 1 已在 Track 05 标注同类问题）(evidence: [T05-S009])。
- **可信度自评**: **medium** — 身份与履历跨源可核，但**缺少他本人的长篇观点材料**（缺「可调研性」这一项），因此不适合作为 Phase 2 的思想来源，只适合作为人物地图与信息源索引。

---

### 6. Ken Goldberg

- **One-liner**: 把「人形/具身乐观论」从情绪之争拉回可计算问题的人——他给出了一个可被反驳的量化框架（「10 万年数据鸿沟」），并主张用「老派工程」（GOFE, good old-fashioned engineering）先让机器人干活、边干活边攒真数据 (evidence: [T01-S008])
- **核心身份**: UC Berkeley 工程学 William S. Floyd 讲席教授（IEOR / EECS / 艺术实践三聘）；Robot Learning Foundation 主席（CoRL 的主办组织）；BAIR 指导委员会主席；Ambi Robotics 与 Jacobi Robotics 联合创始人 (evidence: [T01-S008, T01-S010, T05-S022])
- **利益关系（必须点名）**: **他自己就是「老派工程 + 学习方法混合」这条商业路线的股东**——Ambi Robotics 做包裹分拣，Jacobi Robotics 做机器人运动/规划软件 (evidence: [T01-S008, T01-S010])。他在社论里直接用 Ambi 的数据作论据（见下），这是一个**自我引用的利益相关论据**，读的时候要知道。另一层：他是 Robot Learning Foundation 主席，即学习派主会 CoRL 的组织者，所以他不是「反学习」的人。
- **代表作品**: *Good old-fashioned engineering can close the 100,000-year "data gap" in robotics*（*Science Robotics* 社论，2025-08-27，DOI 10.1126/scirobotics.aea7390）(evidence: [T01-S008])；*"Data will solve robotics and automation: True or false?": A debate*（同期 Viewpoint，他是主持人与通讯作者）(evidence: [T01-S009])；Dex-Net 系列抓取工作（Berkeley AUTOLab）
- **值得读 / 听 / 看的 3 件事**:
  - 📖 GOFE 社论全文 PDF（本人实验室托管，可直接读）https://autolab.berkeley.edu/assets/publications/media/GOFE-Can-Close-the-100000-Year-Robot-Data-Gap-Science-Robotics-Aug-2025-scirobotics.aea7390.pdf (evidence: [T01-S008])；期刊落地页（DOI 10.1126/scirobotics.aea7390，对爬虫返回 403，引用以 PDF 为准）(evidence: [T01-S013])
  - 🎬 ICRA 2025 全会辩论录像（他主持，>1000 人现场）https://www.youtube.com/watch?v=PfvctjoMPk8 (evidence: [T01-S009, T01-S012])
  - 🎙️ *What robots can (& can't) do in 2025 — Ken Goldberg (UC Berkeley, Ambi Robotics)*（本人长视频）https://www.youtube.com/watch?v=94v3zRfBQXQ (evidence: [T01-S014])
  - 📖 Berkeley News 长访谈 *Are we truly on the verge of the humanoid robot revolution?*（2025-08-27）(evidence: [T01-S011])
- **核心思想关键词**: 10 万年数据鸿沟、GOFE（老派工程，模块化 + 可单独测试修复）、数据飞轮要靠「已经能干活的机器人」起转、遥操作数据线性不可扩、仿真对操作不可靠但对飞/走可用
- **他的具体论证（原话，来自 2025-08-27 社论）**:
  - the amount of internet-scale data (texts and images) used to train contemporary VLMs is on the order of 100,000 years (evidence: [T01-S008])
  - Those data do not exist on the internet.（指「视频输入 + 机器人动作指令」这种配对数据）(evidence: [T01-S008])
  - Simulation data work well for robots that fly or walk, or even for doing backflips, but simulation is notoriously unreliable for robot manipulation. (evidence: [T01-S008])
  - YouTube includes about 35,000 years of videos.（但他紧接着说把 2D 视频「抬回」三维以恢复精确手指与物体运动，是可预见未来内解决不了的计算机视觉难题）(evidence: [T01-S008])
  - Whereas end-to-end AI methods are "model free," GOFE is "model based." GOFE segments problems into modules so that each module can be tested, fixed, and fine-tuned independently. (evidence: [T01-S008])
  - I do not disagree with Rich Sutton—I believe that model-free AI will eventually surpass GOFE ... But when will the general-purpose robots arrive? (evidence: [T01-S008]) —— **他的分歧点是时间表，不是终局。**
- **数字口径（重要）**: 「Ambi Robotics 过去 4 年用模型+无模型混合方法采集了 22 年的真实机器人数据，分拣了超过 1 亿个真实包裹」——这是**他本人在社论中给出的自家公司数字，无第三方验证** (evidence: [T01-S008])。「10 万年」是他用「把 token 换算成人类阅读/观看时长」的通行折算得到的量级估计，折算方法链接在社论参考文献里（含 Physical Intelligence 的 Kevin Black 在 X 上的一张对比图）(evidence: [T01-S008])——**这是量级论证，不是精确计量。**
- **voice_samples**:
  - 客户 / 外行解释样本（原话，2025-08-27 Berkeley News 访谈，回答「机器人是不是快到了」）：No; I agree that robots are advancing quickly but not that quickly. 以及 To my mind as a roboticist, the blue-collar jobs, the trades, are very safe. (source: T01-S011, 原话)
  - 学术 / 论证样本（原话）：Simulation data work well for robots that fly or walk, or even for doing backflips, but simulation is notoriously unreliable for robot manipulation. (source: T01-S008, 原话)
  - 立场 / 时间表样本（原话）：I do not disagree with Rich Sutton—I believe that model-free AI will eventually surpass GOFE to enable fully general-purpose robots in the future. (source: T01-S008, 原话)
- **sub_skill_candidate**: `true` — 他提供的是一个**可搬运的推理程序**（把「能不能做到」换算成「数据从哪来、每小时产出多少、线性还是超线性」），这正是 skill 用户最需要的判断工具。
- **dual_role**: `academic + founder`
- **最近 12 个月动态**:
  - 2025-05 主持 ICRA 2025 全会辩论「数据能不能解决机器人学」；他自述现场举手表决显示**多数听众没有改变立场** (evidence: [T01-S009])
  - 2025-08-27 两篇 *Science Robotics* 同日发表（社论 + 辩论 Viewpoint）(evidence: [T01-S008, T01-S009])
  - 2026-02 当选美国国家工程院院士 (evidence: [T01-S010])
- **争议 / 批评**:
  - **有明确的对手方，且在同一期刊同日**。Animesh Garg（佐治亚理工）在辩论中主张 data are not merely beneficial; rather, they are indispensable and foundational (evidence: [T01-S009])；Tedrake 主张大规模预训练是他所知**唯一**能编程出「常识」的方式 (evidence: [T01-S009])。
  - **对他的常见反驳（要义转述）**：他的「数据鸿沟」用的是「把 token 折算成人类时长」这一非标准换算，量级说服力强但不是严格计量；且他自己承认终局站在 Sutton 一边 (evidence: [T01-S008])。
  - **利益冲突批评**：他推荐的路径（先用模块化工程做出能干活的机器人再攒数据）恰好是他两家公司在做的事，社论里也直接引用了 Ambi 的数字 (evidence: [T01-S008])。本轨**未检到**有人具名公开提出这一点，因此列为读者应自行注意的事实，而非「已发生的公开批评」。
- **可信度自评**: **high** — 一手长文可逐字核对（PDF 全文），且他把对手方的观点原样发表在同一期，双方立场都可追。

---

### 7. Shuran Song（宋舒然）

- **One-liner**: 用**方法本身**表态的人——Diffusion Policy 解决了「演示数据多峰、策略学不动」的建模问题，UMI 干脆把数据采集从机器人上拆下来，两件工作合起来是对「遥操作太贵、太不可扩」这一判断最有力的工程回应 (evidence: [T04-S076, T04-S080, T01-S038])
- **核心身份**: Stanford 电气工程助理教授（计算机系兼聘），REAL（Robotics and Embodied AI Lab）负责人；此前在 Columbia (evidence: [T01-S038, T01-S039])
- **利益关系**: **纯学术，本轨未发现她有机器人公司创始人 / 高管身份**——这在本名单里是少数派，意味着她的公开表态不直接绑定融资节奏。获 NSF Career、Sloan Fellowship、Google Research Scholar 等学术奖项 (evidence: [T01-S038])。
- **代表作品**: Diffusion Policy（视觉运动策略的扩散建模，2023）(evidence: [T04-S076])；UMI — Universal Manipulation Interface（手持夹爪、在野人类演示直接转可部署策略，2024）(evidence: [T04-S080])；一系列可形变物体操作与开源具身数据集工作 (evidence: [T01-S038])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 Diffusion Policy 论文（arXiv:2303.04137）——本行业近三年被复现最多的方法之一 (evidence: [T04-S076])
  - 📖 UMI 论文与项目页（arXiv:2402.10329）——采集接口与策略学习一体设计 (evidence: [T04-S080])
  - 🌐 REAL 实验室页（论文 / 代码 / YouTube 演示的一手入口）https://real.stanford.edu/ (evidence: [T01-S039])
  - 🎙️ The Robot Report 对 UMI 夹爪与扩散模型的访谈（受访者为其学生 Cheng Chi）https://www.therobotreport.com/interview-with-chung-chi-about-the-umi-gripper-and-diffusion-ai-models/ (evidence: [T01-S040]) —— **注意：这是她学生的访谈，不是她本人的**。
- **核心思想关键词**: 动作分布的多峰性（为什么要用扩散）、采集接口的设计就是数据分布的设计、硬件无关的策略（UMI 学到的策略可跨本体部署）、在野（in-the-wild）演示
- **voice_samples**:
  - ⚠️ **暂未找到 ≥30 字的本人直接原话片段**。本轨未检到她 2025-2026 年的可访问长访谈或长 talk；她的公开输出以论文、项目页和实验室 YouTube 演示为主。
  - 可用的间接信号（**论文摘要原话**，UMI）：UMI employs hand-held grippers coupled with careful interface design to enable portable, low-cost, and information-rich data collection (source: T04-S080, 论文原话 —— 非口语，仅可用于判断她的表达重心)
- **sub_skill_candidate**: `false` — 学术影响力极高，但缺少本人的长篇口语材料，voice DNA 拿不到；她的思想主要沉淀在方法本身，更适合作为 Track 04 canon 的核心条目。
- **dual_role**: `academic`（单一角色，无企业身份 —— 这本身是本名单里值得标注的稀缺属性）
- **最近 12 个月动态**: 2025-26 学年在 Stanford 开 CS 227A/EE 227 机器人感知与 ENGR 319 seminar (evidence: [T01-S038])。**⚠️ 本轨未取到她 2025-09 之后的具体公开发言 / 新方法发布**，这是本卡片的主要缺口。
- **争议 / 批评**:
  - **UMI 路线与遥操作路线的公开分歧**：UMI 的设计前提是「遥操作贵且不可扩」，而 ALOHA / Mobile ALOHA 线（Finn 团队）与 1X 的 NEO 商业模式恰恰把遥操作当作主要数据来源 (evidence: [T04-S080, T04-S075, T01-S041])。**这是路线分歧，双方没有互相点名批评**。
  - Diffusion Policy 报的 46.9% 是「12 任务 4 个基准上的相对提升、多为仿真」，不是成功率 (evidence: [T04-S076])——这是最常被误引的一个数字。
- **可信度自评**: **medium** — 学术贡献跨源可核（Wave 1 canon 已独立确认），但「当前 active 的公开发声」与「≥30 分钟本人长材料」两项本轨未满足，已明确标出。

---

### 8. Marc Raibert

- **One-liner**: 把「机器人能不能像动物一样动」变成一个工程学科的人（Boston Dynamics 创始人），现在用一家由现代汽车出资的非营利研究所继续做同一件事，并公开对「当前这批人形只会小心翼翼走路、几乎没有灵巧度」表示不满 (evidence: [T01-S042, T01-S043])
- **核心身份**: Robotics and AI Institute（RAI Institute，前身 The AI Institute）执行主任兼创始人；Boston Dynamics 创始人、现任董事会主席（Boston Dynamics 由现代汽车控股）(evidence: [T01-S042, T01-S044])
- **利益关系（必须点名）**: RAI Institute 由**现代汽车出资**，与 Boston Dynamics 是关联方并公开建立了合作关系 (evidence: [T01-S044, T01-S045])。他既不卖人形本体给终端客户，也不融 VC 轮——这让他的公开表态比创业者自由，但他的判断天然偏向「动态运动 + 硬件」这条他自己开创的路线。
- **代表作品**: Raibert & Craig 混合位置/力控制（1981，机器人控制的奠基文献之一）(evidence: [T04-S051])；Boston Dynamics 的 BigDog / Atlas / Spot 系列；RAI Institute 的四个研究方向（认知 AI、运动 AI、有机硬件设计、机器人伦理）(evidence: [T01-S042])
- **值得读 / 听 / 看的 3 件事**:
  - 🌐 RAI Institute 领导层页（本人当前角色与研究所定位的一手说明）https://rai-inst.com/about/leadership/marc-raibert/ (evidence: [T01-S042])
  - 📖 RAI Institute 博客 *Pushing the Pace of Progress*（研究所对研究节奏的公开立场）https://rai-inst.com/resources/blog/pushing-the-pace-of-progress/ (evidence: [T01-S046])
  - 📖 Boston Dynamics 与 RAI Institute 合作公告（组织关系的一手确认）https://bostondynamics.com/news/boston-dynamics-and-the-robotics-ai-institute-partner/ (evidence: [T01-S044])
  - 🎙️ A3（Automate）Automated Podcast 第 1 集为其专访（**本轨对该 URL 的机械访问被 403 拦截，未收进 manifest，仅作线索**）
- **核心思想关键词**: 运动智能 / athletic intelligence（感知、机动、平衡、抓握四件事的合成能力）、把研究所当成「从想法到实现放在一个场地里」的组织设计、对「只会走路的人形」的不满
- **voice_samples**:
  - ⚠️ **本轨未逐字核到他 2025-2026 年关于人形的批评原话**。搜索结果中流传的「当前上市的人形都只是很小心地走来走去 / 几乎看不到灵巧度」「像门把手一样笨 / 像烤面包机一样笨」等说法，**本轨未在可访问的一手页面上逐字核到出处**，因此**不作为原话引用，也不进 evidence**。下游若要用，必须自行核到原始访谈。
  - 可核的立场信号（要义转述）：RAI Institute 把「运动 AI（athletic AI）」与「认知 AI」并列为四大研究方向之一，这个组织设计本身就是他「智能包含身体能力」这一主张的表达 (source: T01-S042, 要义转述)
- **sub_skill_candidate**: `false` — 历史地位无可争议，但本轨拿不到他近期的长篇一手材料；他的思想已通过 Boston Dynamics 的工程产物与 1981 年论文进入 canon。
- **dual_role**: `founder + institute director`
- **最近 12 个月动态**:
  - 2025-09 起 Marco Hutter 出任 RAI Institute 苏黎世办公室负责人（他本人出面邀请）(evidence: [T01-S043])
  - RAI Institute 与 Boston Dynamics 建立正式合作 (evidence: [T01-S044, T01-S045])
- **争议 / 批评**: **本轨未检到具名的公开批评**。需要注意的结构性事实：他所在的机构由整车厂资助、不承担商业化 KPI，因此他对「人形何时能干活」的判断不受融资周期影响，但也不受市场检验。
- **可信度自评**: **medium** — 身份与组织关系可核，但**缺少本人近期长材料与可逐字引用的原话**（已明确标出未核到的传闻引语）。

---

### 9. Marco Hutter

- **One-liner**: 把「腿足机器人靠仿真里的强化学习去学，而不是靠人手写控制器」这条路线跑通并商业化的人（ANYmal / ANYbotics），现在一半时间在 ETH、一半时间在 Marc Raibert 的研究所 (evidence: [T04-S054, T04-S056, T04-S058, T01-S043])
- **核心身份**: ETH Zurich 机器人学教授（Robotic Systems Lab，2025-09 起降为 50% 教职）、ETH 机器人中心主任；同时任 Robotics and AI Institute 苏黎世办公室负责人（50%）；ANYbotics 联合创始人 (evidence: [T01-S043, T01-S047])
- **利益关系（必须点名）**: 他同时是**学术 PI（ETH）+ 本体公司联创（ANYbotics，做工业巡检四足）+ 企业研究所负责人（RAI，现代汽车出资）** (evidence: [T01-S043, T01-S047, T01-S048])。「腿足在工业巡检里已经有真实部署」这类判断对 ANYbotics 有直接商业价值。
- **代表作品**: *Learning agile and dynamic motor skills for legged robots*（Science Robotics 2019，actuator net）(evidence: [T04-S054])；*Learning quadrupedal locomotion over challenging terrain*（2020，teacher-student）(evidence: [T04-S056])；*Learning robust perceptive locomotion*（2022）(evidence: [T04-S058])；自主挖掘机等野外作业机器人 (evidence: [T01-S047])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 ETH RSL 实验室页（研究方向、教学、机器人平台的一手入口）https://rsl.ethz.ch/ (evidence: [T01-S047])
  - 📖 ETH 官方访谈 *"The RAI Institute opens up unique opportunities for both researchers and students"*（2025-09-16，含本人直接引语）(evidence: [T01-S043])
  - 📖 三篇 Science Robotics 腿足学习论文（这一支的方法学正典）(evidence: [T04-S054, T04-S056, T04-S058])
  - 📖 ETH RSL 的 Robot Dynamics 课程页（他的教学线）(evidence: [T04-S095])
- **核心思想关键词**: actuator net（把难建模的驱动器动力学用数据补上）、teacher-student 蒸馏（用仿真特权信息补真机观测不足）、感知式运动（把外感受融进策略）、「从想法到实现放在一个场地里」的研究组织观
- **voice_samples**:
  - 机构 / 组织讨论样本（原话，ETH 官方访谈 2025-09-16）：The RAI Institute allows us to pool everything on one site, from the idea stage to implementation. (source: T01-S043, 原话)
  - 动机样本（原话）：Switzerland is where my heart is. And I think developing something major here in the field of robotics and AI is a huge opportunity for Zurich and for Switzerland. (source: T01-S043, 原话)
  - ⚠️ 本轨**未取到他关于人形 / 具身大模型的直接口语原话**；他关于方法的主张只能从论文摘要转述 (source: T04-S054, 论文原话来源)
- **sub_skill_candidate**: `false` — 技术贡献是本行业的支柱之一，但本轨拿到的口语材料集中在机构话题上，思想类长材料不足。
- **dual_role**: `academic + founder + institute director`
- **最近 12 个月动态**: 2025-09-16 ETH 官宣他以 50%/50% 的方式同时任 ETH 教授与 RAI Institute 苏黎世负责人 (evidence: [T01-S043])
- **争议 / 批评**:
  - **腿足学习派与模型控制派的路线分歧**（Wave 1 已记录）：同一时期 MIT Cheetah 3 用凸 MPC、ANYmal 用学习式控制解同一个问题，双方论文的动机段互为反例 (evidence: [T04-S052, T04-S054])。
  - **派内分歧**：结构化中间表示（高程图 + 信念状态，Miki 2022）vs 端到端深度图（Pathak 团队 Extreme Parkour）(evidence: [T04-S058, T04-S088])。
  - **利益结构**：三重身份（教授 + 公司联创 + 企业研究所负责人）意味着他的公开表态服务于多个目标；本轨**未检到有人具名就此公开质疑**。
- **可信度自评**: **medium-high** — 学术贡献与身份跨源可核，有可逐字引用的官方访谈原话，但缺少他对当前人形/VLA 议题的表态材料。

---

### 10. Sangbae Kim

- **One-liner**: 「硬件是使能者」这一派最清晰的代言人——MIT Cheetah 系列的作者，主张双足运动之所以被 RL 解决是因为先有了可反驱、抗冲击的准直驱驱动器；2025 年起停薪留职去 Meta 做人形 (evidence: [T01-S049, T01-S050])
- **核心身份**: MIT 机械工程系副教授、Biomimetic Robotics Lab 创始人（领导 16 年）；**当前停薪留职（on leave），在 Meta 任 Robotics Architect，参与其人形机器人项目** (evidence: [T01-S050])
- **利益关系（必须点名）**: 他现在在**一家刚进场的超大型科技公司做人形**，此前长期是「人形不实用、四足更务实」这一立场的代表之一。**这个身份转变本身就是行业信号，读他 2025 年之后的表态要带上这一层。**本轨未取到他本人对这次转变的公开解释 (evidence: [T01-S050])。
- **代表作品**: MIT Cheetah 系列（Cheetah 2/3、Mini Cheetah）——准直驱（QDD）+ 本体感受式驱动器的代表；Stickybot / Spinybot / iSprawl 等仿生机器人；Little HERMES 等力反馈遥操作系统 (evidence: [T01-S049, T01-S051])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 Quanta Magazine *Why Do Humanoid Robots Still Struggle With the Small Stuff?*（2026-03-13，多位一线研究者同台被引，含他的直接引语）https://www.quantamagazine.org/why-do-humanoid-robots-still-struggle-with-the-small-stuff-20260313/ (evidence: [T01-S052])
  - 📖 MIT 机械系人物页（学术身份与研究方向）https://meche.mit.edu/people/faculty/SANGBAE@MIT.EDU (evidence: [T01-S049])
  - 📖 IEEE Spectrum *This MIT Robot Wants to Use Your Reflexes to Walk and Balance*（Little HERMES，力反馈遥操作的动机说明）https://spectrum.ieee.org/mit-little-hermes (evidence: [T01-S051])
- **核心思想关键词**: 硬件是使能者（hardware as enabler）、可控顺应性（controllable compliance）、准直驱与本体感受式驱动、遥操作缺少物理反馈这一结构缺陷
- **voice_samples**:
  - 技术论证样本（原话，Quanta 2026-03-13）：Reinforcement learning solved a lot of the bipedal locomotion problem, but the hardware was the enabler. (source: T01-S052, 原话)
  - 工程经验样本（原话片段，Quanta）：The robot just breaks（他解释用传统电机时，策略每次执行失败机器人就坏；他的驱动器靠可控顺应性绕开了这个问题）(source: T01-S052, 原话片段 + 上下文转述)
  - 遥操作立场样本（要义转述）：他与合作者的公开论点是，现有遥操作系统既难把操作者动作正确映射到机器人上，也不给操作者任何物理反馈——这两件事共同限制了遥操作数据的质量 (source: T01-S051, 要义转述)
- **sub_skill_candidate**: `false` — 观点极有价值且是这一行少见的「硬件优先」视角，但本轨只拿到二手长文里的引语，没有他本人的长材料。
- **dual_role**: `academic + industry`（MIT 教授停薪留职 + Meta 机器人架构师）
- **最近 12 个月动态**: 2025 年起从 MIT 停薪留职加入 Meta 做人形机器人 (evidence: [T01-S050])；2026-03 在 Quanta 的行业综述中作为「硬件派」被引 (evidence: [T01-S052])
- **争议 / 批评**:
  - **有正面交锋，且在同一篇文章里**。Russ Tedrake 在同一篇 Quanta 文章中的原话是：The hardware is exceptional, and if you're blaming it, you're making excuses (evidence: [T01-S052])——这与 Sangbae Kim 的「硬件才是使能者」构成**这一行最干净的一组当面对立**。Jonathan Hurst（Agility Robotics）在同一篇里的立场偏向硬件必要性：It's more like you kind of know that you need a quasi-direct drive motor to get close (evidence: [T01-S052])。
  - **注意**：双方讨论的对象不完全相同——Kim 说的是**腿足运动**为什么被 RL 解决，Tedrake 说的是**灵巧操作**当前的瓶颈不在硬件。Phase 2 引用时必须带上这个限定，不要写成「Tedrake 反驳 Kim」。
- **可信度自评**: **medium** — 有可逐字引用的原话，但来自二手长文而非本人长材料；且他当前的雇主身份使公开表态受限。

---

### 11. Deepak Pathak

- **One-liner**: 端到端腿足与「一个大脑装进任何本体」的最激进主张者——学术上做 Extreme Parkour（不建地图、直接从深度图端到端），商业上把同一主张做成 Skild AI 的「omni-bodied（任意本体）」卖点 (evidence: [T04-S088, T01-S053, T01-S054])
- **核心身份**: CMU Raj Reddy 副教授（机器人研究所）；Skild AI 联合创始人兼 CEO（与同为 CMU 教授的 Abhinav Gupta 于 2023-05 创办）(evidence: [T01-S053, T01-S054])
- **利益关系（必须点名）**: **他是估值 140 亿美元级创业公司的 CEO**（2026-01-14 完成 SoftBank 领投的 14 亿美元融资，估值三倍至 140 亿美元，投资方含 NVIDIA 的 NVentures、Bezos Expeditions 等）(evidence: [T01-S054, T01-S055])。「一个模型能装进四足、人形、巡检机器人、产线机械臂」这句话既是技术主张也是估值论据，**引用时必须带上这一层**。
- **代表作品**: Extreme Parkour with Legged Robots（端到端深度图到动作，2023）(evidence: [T04-S088])；好奇心驱动探索（curiosity-driven exploration）等 RL 工作；Skild Brain（公司主打模型）(evidence: [T01-S053])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 Extreme Parkour 论文（arXiv:2309.14341）——端到端腿足的代表作，也是与 ETH「结构化中间表示」路线的直接对照 (evidence: [T04-S088])
  - 🌐 Skild AI 官网（公司对 omni-bodied 的一手表述）https://www.skild.ai/ (evidence: [T01-S053])
  - 📖 The Robot Report 报道 *Skild AI raises $1.4B to build 'omni-bodied' robot brain*（融资与主张的行业侧记录）(evidence: [T01-S054])
  - 🎙️ Alex Heath 在达沃斯对 Skild 的 CEO 访谈（*Sources* newsletter）https://sources.news/p/skild-ai-ceo-robotics-brain-davos (evidence: [T01-S056])
- **核心思想关键词**: omni-bodied intelligence（任意本体智能）、端到端优于分层（他在腿足上的技术立场）、跨本体零样本控制、「没训练过的机器人也能控」
- **数字口径（重要）**: 「Skild Brain 能控制它从未训练过的机器人，并实时适应形态或环境的极端变化」——**这是公司自述，本轨未检到任何第三方复现或独立评测** (evidence: [T01-S053, T01-S054])。融资数字（14 亿美元、140 亿美元估值、累计超 18.3 亿美元、22 家投资方）来自 2026-01 的行业报道 (evidence: [T01-S054, T01-S055])。
- **voice_samples**:
  - ⚠️ **暂未找到 ≥30 字的本人直接原话片段**。本轨检到的 Skild 相关表述多为公司口径或记者转述，未逐字核到 Pathak 本人的长段引语。下游需要时应从 T01-S056 的访谈原文取。
  - 可核的立场信号（要义转述，公司口径）：Skild 把自己的主张称作 omni-bodied intelligence——一个通用模型，丢进四足、人形、巡检机器人或产线机械臂上都能直接工作 (source: T01-S053, 公司口径转述)
- **sub_skill_candidate**: `false` — 主张鲜明但本轨缺本人长材料；且他的公开表述与融资叙事高度耦合，作为思想源风险较高。
- **dual_role**: `academic + founder`
- **最近 12 个月动态**: 2026-01-14 Skild AI 完成 14 亿美元融资，估值 140 亿美元 (evidence: [T01-S054, T01-S055])
- **争议 / 批评**:
  - **技术路线上的公开对照**：他的端到端腿足主张与 ETH 的「高程图 + 信念状态」结构化路线在同一时期解同一问题，双方论文动机段互为反例（Wave 1 已记录）(evidence: [T04-S088, T04-S058])。
  - **跨本体正迁移是否成立**是这一主张的公开软肋：Open X-Embodiment 论文自身就报告了部分本体上的**负迁移** (evidence: [T04-S074])。「一个大脑装进任何本体」的说法目前**没有跨机构公共基准可验证** (evidence: [T04-S078, T04-S077])。
  - 本轨**未检到**具名研究者公开点名批评 Skild 的技术主张。
- **可信度自评**: **medium** — 身份、融资、技术路线跨源可核，但本人长材料与第三方验证均缺失。

---

### 12. Jim Fan（范麟熙）

- **One-liner**: NVIDIA 具身路线的对外解释者与造词者——他提出的「物理图灵测试」（Physical Turing Test）是这一轮最广泛传播的评价框架比喻，也是 NVIDIA「用仿真与合成数据把机器人训练成本压下来」这一商业主张的包装 (evidence: [T01-S057, T01-S058])
- **核心身份**: NVIDIA 高级研究科学家、AI Agents 方向负责人；GEAR（Generalist Embodied Agent Research）组共同负责人，主导 Project GR00T（人形机器人基础模型）(evidence: [T01-S057, T01-S058, T01-S059])
- **利益关系（必须点名）**: **他是 GPU 与仿真平台厂商的研究员兼对外发言人**。他的核心论点——真机数据是「烧人力燃料」、仿真与合成数据是出路——**恰好指向 NVIDIA 卖的东西（Isaac Sim / Isaac Lab / GPU / Jetson / GR00T）** (evidence: [T01-S058, T05-S058])。这不使论点无效，但它是这一行**利益与观点耦合最紧**的一例，必须点名。
- **代表作品**: MineDojo（NeurIPS 2022 杰出论文奖）、Voyager（LLM 驱动的 Minecraft 终身学习智能体）、Eureka（用 GPT-4 生成奖励函数训练灵巧手）、VIMA（多模态操作基础模型）(evidence: [T01-S057])；Project GR00T 系列 (evidence: [T01-S058, T01-S059])
- **值得读 / 听 / 看的 3 件事**:
  - 🎬 *The Physical Turing Test: Solving General Purpose Robotics*（Actuate 2025，Foxglove 主办的机器人开发者大会，本人完整 keynote）https://actuate.foxglove.dev/recordings/the-physical-turing-test-solving-general-purpose-robotics/ (evidence: [T01-S058])
  - 🎬 同场 talk 的 NVIDIA 官方 YouTube 版本 https://www.youtube.com/watch?v=q1Q_lHJBxjI (evidence: [T01-S060])
  - 🌐 个人主页（项目清单与论文入口）https://jimfan.me/ (evidence: [T01-S057])
  - 🌐 NVIDIA GEAR 实验室页 https://research.nvidia.com/labs/gear/ (evidence: [T01-S059])
- **核心思想关键词**: 物理图灵测试（分不出这顿饭和这间屋子是人还是机器收拾的）、真机数据是「烧人力燃料」、仿真里的时间压缩（几小时仿真 = 若干年真机经验）、合成数据流水线（GR00T-Dreams）
- **数字口径（重要，且都必须带厂商自报标签）**:
  - 「人形机器人在两小时仿真时间内完成相当于十年的行走训练」——**NVIDIA 自报的仿真加速比，不是真机能力指标** (evidence: [T01-S058])。
  - 「GR00T N1.5 用 GR00T-Dreams 合成数据在 36 小时内开发完成，人工采集则需近三个月」——**NVIDIA 自报的开发周期对比，无第三方验证** (evidence: [T01-S058, T01-S061])。
  - **这两个数字都不是成功率**，不能拿来说明机器人能干什么。
- **voice_samples**:
  - 外行解释样本（要义转述）：他解释「机器人到底要做到什么程度才算成」时的招牌说法是——你回到家，屋子干干净净，桌上摆好了双人烛光晚餐，而你分不出这是人做的还是机器做的；他还补一句，做这件事的机器人不一定非得是人形。(source: T01-S058, 要义转述)
  - 技术论证样本（要义转述）：他把真机数据采集叫作「烧人力燃料」——慢、贵、有上限；而机器人的关节控制信号是没法从互联网上爬到的。(source: T01-S058, 要义转述)
  - ⚠️ 本轨**未逐字取到他的 ≥30 字英文原话**（未抓 talk 字幕），以上均为要义转述。下游要原话需自行抓 T01-S058 / T01-S060 的字幕。
- **sub_skill_candidate**: `false` — 传播力极强、比喻好用，但他的表达高度服务于厂商叙事，且本轨未取到逐字原话；建议作为「厂商话术的样本」而非「思想来源」使用（与 Wave 1 glossary 的 P 节配合读）(evidence: [T06-S042])。
- **dual_role**: `academic-trained + vendor research`（Fei-Fei Li 门下博士 → NVIDIA 研究与对外发言）
- **最近 12 个月动态**: 2025 年在 Actuate 2025 等多个开发者会议上传播「物理图灵测试」框架 (evidence: [T01-S058, T01-S060])；GR00T N1.5 与 GR00T-Dreams 合成数据管线发布 (evidence: [T01-S061])
- **争议 / 批评**:
  - **与 Goldberg 的直接对立**：Goldberg 的社论明确写 simulation is notoriously unreliable for robot manipulation（仿真对操作不可靠），而 Jim Fan 的整套论证建立在仿真与合成数据可替代真机数据之上 (evidence: [T01-S008, T01-S058])。**双方没有互相点名，但论点正面冲突。**
  - **与 Brooks 的对立**：Brooks 认为视觉数据里没有触觉与力，仿真同样造不出这些模态 (evidence: [T01-S001])。
  - **口径批评（跨源、结构性）**：厂商发布的「训练加速比」「开发周期缩短」不是能力指标，这正是 Wave 1 glossary 记录的厂商话术类型 (evidence: [T06-S042])。
- **可信度自评**: **medium** — 身份、talk、项目均可核，但本人逐字原话缺失，且需按「厂商发言人」而非「独立研究者」来读。

---

### 13. Brett Adcock

- **One-liner**: 本轮人形叙事最激进的执行者与最会造节奏的传播者——Figure 的创始人兼 CEO，把「人形进工厂」从概念推到有月度出货数字可报的阶段，同时也是「数字口径」问题最集中的对象 (evidence: [T01-S062, T01-S063])
- **核心身份**: Figure AI 创始人兼 CEO（2022 年创办）；此前创办 Archer Aviation（电动垂直起降）与 Vettery（招聘平台）(evidence: [T01-S062, T01-S063])
- **利益关系（必须点名）**: **他是本轮估值最高的纯人形公司的 CEO**（据 2025 年底以来的行业报道，Figure 累计融资约 19 亿美元、估值约 390 亿美元）(evidence: [T01-S063])。他的每一次公开发言都直接服务于融资与客户获取；他本人也是最活跃的社交媒体发布者之一。**引用他的任何进度声明前先问：这是交付量还是产量？是意向还是订单？谁验证的？**
- **代表作品**: Figure 的 *Master Plan*（2022-05-20，本人署名的公司纲领）(evidence: [T01-S062])；Figure 01/02/03 本体；Helix（Figure 自研的端到端 VLA 模型）；BotQ 自建工厂 (evidence: [T01-S062, T01-S063])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 *Master Plan*（本人署名、日期明确的公司纲领，含市场规模口径）https://www.figure.ai/master-plan (evidence: [T01-S062])
  - 🎙️ *The Future is Humanoid: Brett Adcock on Figure AI's Robotics Revolution*（本人长访谈，Apple Podcasts 可访问）https://podcasts.apple.com/us/podcast/episode119-the-future-is-humanoid-brett-adcock-on/id1792667231?i=1000705358042 (evidence: [T01-S064])
  - 🎙️ *Brett Adcock, CEO of Figure*（Sourcery，2026-04，含工厂参观 + 长访谈）https://www.sourcery.vc/p/breaking-brett-adcock-ceo-of-figure (evidence: [T01-S065])
  - 🎙️ Shawn Ryan Show #292（2026-03-30，超长访谈，面向非技术听众）—— **本轨找到的文字整理页已失效（curl 返回 000），仅记录该访谈存在** (evidence: [T01-S066])
- **核心思想关键词**: 通用人形优于专用机（「为人的环境造人形」）、30 年视角、把制造（BotQ）当核心竞争力、垂直整合（本体 + 模型 + 工厂）
- **数字口径（本卡片最重要的部分）**:
  - *Master Plan*（2022-05-20，本人原话/口径）：美国有 1000 万个不安全或没人愿意干的岗位；全球 GDP 中约 50%（约 42 万亿美元/年）来自体力劳动报酬；全球 23 亿家庭、7 亿老龄人口、30 亿企业劳动岗位 (evidence: [T01-S062])。**这些是 TAM（潜在市场）口径，不是订单也不是需求验证。**
  - 2026-04-29 Figure 宣布 BotQ 达到「每小时 1 台 Figure 03」的产线节拍，并称 2026-02 约 60 台、03 月约 120 台、04 月约 240 台，累计超 350 台 (evidence: [T01-S063])。**关键限定：这是「产量 / 下线量」，Figure 未公开其中卖给客户多少台** (evidence: [T01-S063])。
  - 客户侧公开事实：在 BMW 南卡工厂有部署 (evidence: [T01-S063])。**连续无人运行时长与干预率未公开。**
- **voice_samples**:
  - 公司愿景样本（原话，Master Plan 2022-05-20）：Expand human capabilities through advanced AI.（使命句）以及 General purpose humanoid robots built for a human environment is the desired route. (source: T01-S062, 原话)
  - 路线样本（原话片段，Master Plan）：Build a feature-complete electromechanical humanoid … Perform human-like manipulation … Integrate into labor force.（三段式里程碑）(source: T01-S062, 原话片段)
  - ⚠️ 本轨**未逐字核到**他 2026 年访谈中的具体语句；上述长访谈（ARK / Sourcery / Shawn Ryan）已定位但未抓字幕。
- **sub_skill_candidate**: `false` — 他是**研究对象**而不是思想来源：他的价值在于提供「厂商叙事长什么样、数字口径怎么被模糊」的第一手样本（与 Wave 1 glossary P 节直接配对）(evidence: [T06-S042])。
- **dual_role**: `founder`（连续创业者，非研究者）
- **最近 12 个月动态**:
  - 2026-03-30 Shawn Ryan Show 长访谈（面向大众的人形叙事）(evidence: [T01-S066])
  - 2026-04 Sourcery 工厂参观 + 访谈，谈从「数千台」到「每年 100 万台」的规模路径 (evidence: [T01-S065])
  - 2026-04-29 公布 BotQ「每小时 1 台」产线节拍 (evidence: [T01-S063])
- **争议 / 批评**:
  - **来自 Rodney Brooks 的点名**：Brooks 在 2025-09-26 的长文中明确把 Figure 列为「押注看大量人手视频就能学出灵巧」的代表之一，并称这条路在数十年内做到人类水平灵巧是 pure fantasy thinking (evidence: [T01-S001])。**本轨未检到 Figure 或 Adcock 对该文的公开回应。**
  - **公开的负面事实（需按「有诉讼主张 ≠ 已认定」读）**：有行业分析引用一起**吹哨人诉讼**，指控 Figure 为促成融资轮而削减安全投入；同时提到 BMW 在欧洲扩张中选择了别家供应商 (evidence: [T01-S063])。**这些是诉讼主张与市场传闻，本轨未取到法院文件或 BMW 官方声明，不作为已证事实。**
  - **口径批评（结构性）**：「已进厂 / 量产」这类表述在这一行的通行含义是「试点工位、限定任务、有人陪同」，且产量口径常混入订单与意向（Wave 1 glossary 已列为典型话术）(evidence: [T06-S042])。
- **可信度自评**: **medium-high**（作为**叙事样本**）/ **low**（作为**技术判断来源**）——本人署名文件与长访谈均可核，但技术性主张几乎全部无第三方验证。

---

### 14. Bernt Børnich

- **One-liner**: 把「遥操作不是过渡手段，而是产品本身」这件事摆到台面上的人——1X 的 NEO 家用人形以「远程人工操作员会看到你家里」为明示条款卖给消费者，这是全行业最直白的一次「自主率口径」公开化 (evidence: [T01-S067, T01-S068])
- **核心身份**: 1X Technologies（原 Halodi Robotics，挪威/美国）创始人兼 CEO (evidence: [T01-S067])
- **利益关系（必须点名）**: **他在卖一台售价 2 万美元 / 或每月 499 美元订阅的家用人形**，而这台机器人当前的多数演示动作由戴 VR 头显的人类远程操作完成 (evidence: [T01-S067, T01-S069])。他的公开辩护（遥操作是必要的「数据采集打法」）**同时是产品说明和融资叙事**。
- **代表作品**: NEO 家用人形机器人（2025-10 开放预订）(evidence: [T01-S067])；1X 的 Redwood / 世界模型等自研栈
- **值得读 / 听 / 看的 3 件事**:
  - 🎙️ 纽约时报 *Hard Fork* 播客对他的访谈（他在其中为遥操作辩护）——本轨通过二手整理确认存在，**未直接取到可访问的播客页面 URL**，故不进 manifest (evidence: [T01-S068])
  - 📖 *1X CEO Details NEO's 'Two Modes' and Defends Teleoperation as 'More Secure' than a Cleaner*（Humanoids Daily 对其表态的整理）https://www.humanoidsdaily.com/news/1x-ceo-details-neo-s-two-modes-and-defends-teleoperation-as-more-secure-than-a-cleaner (evidence: [T01-S068])
  - 📖 Engadget *1X Neo is a $20,000 home robot that will learn chores via teleoperation*（价格、订阅、条款的行业侧记录）https://www.engadget.com/ai/1x-neo-is-a-20000-home-robot-that-will-learn-chores-via-teleoperation-040252200.html (evidence: [T01-S067])
  - 🌐 1X 官网（产品与公司一手口径）https://www.1x.tech/ (evidence: [T01-S069])
- **核心思想关键词**: 遥操作即数据采集打法（data collection play）、两种模式（自主 / 远程接管）、把隐私做成产品功能（时间窗、人像模糊、禁区）、「先卖出去才有数据」
- **数字口径（本卡片的关键）**:
  - 售价 2 万美元或 499 美元/月订阅 (evidence: [T01-S067])。
  - **自主率口径**：在其宣传视频中，除两处例外，展示的任务均非自主完成，而是由戴 VR 头显与手柄的人类遥操作 (evidence: [T01-S067])。**这是本行业极少见的、由报道方明确给出的自主/非自主拆分。**
  - **隐私机制（公司口径）**：用户可在 App 里设定允许远程接管的时间窗；每次操作员接入需用户明确批准；画面中的人可被模糊；用户可设禁区，遥操作时也不进 (evidence: [T01-S067, T01-S068])。**这些是公司承诺，本轨未见第三方审计。**
- **voice_samples**:
  - 客户解释样本（要义转述）：他对隐私质疑的标准回应是——买 NEO 的人必须同意会有人类操作员通过机器人摄像头看到家里，这是训练机器最终能自主的必要条件；他并把这项服务类比成「比请保洁更安全」 (source: T01-S067, T01-S068, 要义转述)
  - ⚠️ **本轨未逐字核到他的英文原话**（Hard Fork 原始音频未取）。「more secure than a cleaner」这一措辞出自二手整理的标题，**本文件不将其标为原话**。
- **sub_skill_candidate**: `false` — 他的价值是提供「自主率与数据来源如何被包装成产品」的一手案例，不是思想来源。
- **dual_role**: `founder`
- **最近 12 个月动态**: 2025-10 NEO 以 2 万美元 / 499 美元月订阅开放预订，明示遥操作条款，随即引发隐私争议 (evidence: [T01-S067, T01-S068])
- **争议 / 批评**:
  - **隐私争议是公开且持续的**：操作员在接管期间能看到房间布局、物品与生活规律，且会话录像会被存下来训练自主模型 (evidence: [T01-S067, T01-S068])。
  - **「自主」口径争议**：宣传视频中绝大多数任务为遥操作完成，这与「家用自主机器人」的直觉理解相差很远 (evidence: [T01-S067])。这恰好命中 Wave 1 glossary 记录的「全自主 / fully autonomous」话术条目 (evidence: [T06-S042])。
  - **与 Goldberg 论点的关系**：Goldberg 认为遥操作产出与投入线性相关、扛不住量级差 (evidence: [T01-S008])；1X 的商业模式实质上是**把遥操作成本转嫁给付费用户**，用消费端补贴数据采集——这是一个此前没有过的答案，也正是它引发争议的原因。
- **可信度自评**: **medium** — 产品事实、价格与条款跨源可核；但**本人原话未逐字取到**，且所有隐私机制均为公司自述。

---

### 15. 王兴兴（Wang Xingxing）

- **One-liner**: 中国四足与人形本体的价格与供应链改写者（宇树 Unitree），也是少数**公开唱衰当前主流 VLA 架构**的本体厂商创始人——他押的是视频生成 / 世界模型这条路 (evidence: [T01-S070, T01-S071, T05-S051])
- **核心身份**: 宇树科技（Unitree Robotics）创始人兼 CEO；公司 2016-08 成立，2026-08 满十年 (evidence: [T01-S070, T01-S072])
- **利益关系（必须点名）**: **他是本体厂商的创始人**——宇树卖的是四足与人形硬件平台（G1 等），公司已上市（2026 年 8 月的报道提到「上市第二天」）(evidence: [T01-S070, T01-S073])。他说「数据不是最大问题、模型才是」这件事，**对一个卖硬件、不卖模型的公司是有利的定位**：如果瓶颈在模型，那么本体厂商就不是瓶颈方。这层关系必须写出来。
- **代表作品**: 宇树 A1 / Go / B 系列四足；H1 / G1 人形；把四足与人形的入门价格压到远低于同类的水平；官方 SDK 与部署示例开源在 GitHub (evidence: [T05-S051])
- **值得读 / 听 / 看的 3 件事**:
  - 🎬 2026 世界机器人大会（WRC，2026-08-19~23 北京）主题演讲《从展品到产品：人形机器人产业的下一个十年》——**本轨未取到官方完整视频或官方文字稿**，仅通过多家媒体报道交叉确认其存在与主要内容 (evidence: [T01-S070, T01-S071, T05-S045])
  - 🌐 宇树官方 GitHub 组织（SDK、部署示例——判断这家公司真实工程口径的最好入口）https://github.com/unitreerobotics (evidence: [T05-S051])
  - 📖 CNBC 报道其 WRC 2026 发言（英文侧交叉印证）https://www.cnbc.com/2026/08/20/unitree-humanoid-robots-chatgpt-moment.html (evidence: [T01-S070])
- **核心思想关键词**: 具身智能的「ChatGPT 时刻」（他的定义是可判定的：陌生环境里完成约 80% 任务）、泛化能力不足是最大瓶颈、对 VLA 架构的怀疑、视频生成 / 世界模型路线、「从展品到产品」
- **他的具体主张与数字口径**:
  - **他给「ChatGPT 时刻」下了一个可判定的定义**：把机器人放进一个陌生环境，能完成大约 80% 的任务；他判断这一点行业最快 2–3 年可到 (evidence: [T01-S070, T01-S071])。**口径提醒：这是他 2026-08-20 在 WRC 的预测，不是已达成的指标，也没有说清「任务」的集合与「完成」的判据。**
  - 更早（2025-11）他提过一个「两个 80%」的说法：1–3 年内，人形机器人能理解语音或文字指令，并在 80% 的陌生生活场景里完成约 80% 的任务 (evidence: [T01-S074])。**注意这与 2026-08 的表述口径不同**（一个是「80% 场景 × 80% 任务」，一个是「陌生环境里约 80% 任务」），引用时不要混用。
  - **对 VLA 的怀疑（要义转述，2025-08~09）**：他表示行业对「数据问题」的关注度过高，真正的瓶颈在模型；他认为当前流行的 VLA 架构是一种「过于简单的设计」，在 VLA 上加 RL（VLA+RL）也不够，架构需要继续升级；他更看好视频生成模型或由其驱动的世界模型这条路 (evidence: [T01-S075, T01-S076])。
  - **出货量 / 订单额：本轨未取到经第三方验证的数字，不写。**
- **voice_samples**:
  - ⚠️ **本人长材料（完整演讲视频或官方文字稿）未获取**。上述所有表述均来自中文与英文媒体的二手报道（CNBC、Global Times、财新、澎湃、21 世纪经济报道等），**本文件因此不标注任何「原话」**，全部标为要义转述。**下游若需要他的逐字原话，必须自行获取 WRC 2026 官方演讲录像或宇树官方渠道的文字稿。**
  - 可交叉印证的立场信号（要义转述）：他把「陌生环境里完成约 80% 任务」当作行业里程碑的判定标准，并把当前最大瓶颈定为泛化能力不足 (source: T01-S070, T01-S071, 要义转述，跨两个独立来源)
- **sub_skill_candidate**: `false` — 影响力毫无疑问，但**本轨没有拿到任何一手长材料**，voice DNA 与思想体系都无法可靠重建。
- **dual_role**: `founder`（工程师出身的本体厂商创始人）
- **最近 12 个月动态**:
  - 2026-08-20 在 WRC 2026 发表主题演讲，回顾十年、介绍 G1 等产品、给出「2–3 年 ChatGPT 时刻」的判断 (evidence: [T01-S070, T01-S071, T01-S073])
  - 2025-11 提出「两个 80%」的 1–3 年目标 (evidence: [T01-S074])
- **争议 / 批评**:
  - **他自己就是「唱反调」的一方**：在几乎所有头部具身公司都押 VLA 的时期，他公开说 VLA 架构过于简单 (evidence: [T01-S075, T01-S076])。这与 Physical Intelligence、智元、Figure 的路线构成实质分歧。
  - **时间表分歧**：他的「2–3 年」与 Brooks 的「数十年内是纯幻想」、Goldberg 的「2 年、5 年、10 年都不会发生」是**同一议题上量级不同的三个公开判断** (evidence: [T01-S070, T01-S001, T01-S011])。
  - **口径批评**：他前后两次「80%」的定义不一致（见上），且没有说明任务集合与判据 (evidence: [T01-S070, T01-S074])。
- **可信度自评**: **low-medium** — 人物重要性 high，但**证据全部为二手**；按本轨纪律，他的观点只能作为「有日期、有场合的公开表态」引用，不能作为技术判断依据。

---

### 16. 彭志辉「稚晖君」

- **One-liner**: 智元（AgiBot）的技术形象与路线发布者——他把公司的叙事从「能不能做出来」推到「能不能稳定干活」，并把数据飞轮写进公司方法论；智元同时是中国侧唯一开源了百万级真机数据集的公司 (evidence: [T01-S077, T04-S084, T05-S034, T05-S037])
- **核心身份**: 智元创新（上海）科技股份有限公司联合创始人兼 CTO（另一位创始人为原华为高管邓泰华）；公司 2023 年创办 (evidence: [T01-S077, T01-S078])
- **利益关系（必须点名）**: **他是本体 + 模型双线创业公司的联创兼技术代言人**，也是有大量粉丝的技术内容创作者出身。他在公司大会上的每一次技术表述都同时是产品发布 (evidence: [T01-S077])。**对冲事实**：智元把 AgiBot World 数据集（百万级真机轨迹，CC BY-NC-SA 4.0）与 GO-1 基座模型公开，使其部分主张可被外部检验 (evidence: [T04-S084, T05-S034, T05-S037])。
- **代表作品**: GO-1（Genie Operator-1，2025-03-10 发布的通用具身基座模型）(evidence: [T01-S078, T04-S084])；AgiBot World Colosseo 数据集与 benchmark (evidence: [T04-S084, T05-S034])；远征系列与灵犀系列本体 (evidence: [T01-S078])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 智元官网上他在 APC 2026（2026-05-07）的主题演讲《从感知世界到赋能产业，智元推动具身智能迎来生产力拐点》——**公司官方渠道刊载的本人演讲内容** https://www.agibot.com.cn/article/315/detail/153.html (evidence: [T01-S077])
  - 📖 AgiBot World / GO-1 论文（arXiv:2503.06669）——公司主张的可核版本 (evidence: [T04-S084])
  - 🌐 AgiBot World 官方仓库与 HuggingFace 数据集（Beta 版 1,003,672 条轨迹 / 约 43.8TB）(evidence: [T05-S034, T05-S037])
- **核心思想关键词**: 从「技术突破」到「生产力部署」、机器人是持续运行的（vs 聊天模型是被调用的）、「交付结果」而非「销售机器人」、部署—学习—再部署的数据飞轮、一体三智（交互智能 / 作业智能 / 运动智能）
- **voice_samples**（**均取自公司官网刊载的演讲内容，属公司渠道的本人表述**）:
  - 行业判断样本（原话）：具身智能正在从技术突破阶段，迈入生产力部署阶段 (source: T01-S077, 原话)
  - 技术类比样本（原话）：聊天模型是被调用的，而机器人是持续运行的 (source: T01-S077, 原话)
  - 商业口径样本（原话）：行业关注的核心问题，已经从「能不能做出来」，转向「能不能稳定地干活」；企业不再单纯「销售机器人」，而是开始「交付结果」 (source: T01-S077, 原话)
  - 分水岭表述（原话）：具身智能的分水岭，不只是 AI 进入物理世界，而是进一步进入真实工作流 (source: T01-S077, 原话)
- **数字口径**: **该场演讲未给出任何出货量、订单额或成功率数字** (evidence: [T01-S077])。可核的量化事实只有数据集规模：AgiBot World Beta 版 1,003,672 条轨迹、约 43.8TB (evidence: [T05-S037])——**这是数据量，不是能力指标。**
- **sub_skill_candidate**: `false` — 有可逐字引用的中文原话（少见），但材料是单场演讲、且是产品发布语境；不足以支撑独立的思想体系蒸馏。**但他的原话是本 skill 中文表达 DNA 的重要素材。**
- **dual_role**: `founder + 技术传播者`
- **最近 12 个月动态**:
  - 2026-04-17 上海举办 2026 智元合作伙伴大会（APC 2026），主题「共启具身智能生产力新时代」(evidence: [T01-S079])
  - 2026-05-07 官网刊出其 APC 2026 演讲，提出「一体三智」框架（交互智能 WITA Omni / 作业智能 GO-2 / 运动智能 BFM 与 GCFM）与「部署—学习—再部署」数据飞轮 (evidence: [T01-S077])
- **争议 / 批评**:
  - **与王兴兴的路线分歧（同为中国头部厂商，公开表态相反）**：智元押的是端到端具身基座模型（GO-1 / GO-2 这条 VLA 血统的线）(evidence: [T04-S084, T01-S077])，而王兴兴公开说当前 VLA 架构过于简单、更看好世界模型 (evidence: [T01-S075, T01-S076])。**双方没有互相点名，但这是中国侧最实质的一组路线分歧。**
  - **评测口径问题（结构性）**：AgiBot World 的性能数字来自作者自建评测，无跨机构公共基准（Wave 1 已记录）(evidence: [T04-S084, T04-S078])。
  - 本轨**未检到**针对他个人的具名公开批评。
- **可信度自评**: **medium-high** — 有公司官方渠道刊载的本人中文原话可逐字引用，数据集与论文可外部检验；但材料仅一场发布会级演讲，缺少非发布语境的长访谈。

---

### 17. 卢策吾（Cewu Lu）

- **One-liner**: 中国侧抓取感知这一支的奠基者——GraspNet-1Billion 与 AnyGrasp 是中国团队在具身操作领域被国际同行引用最多的一手成果之一，他同时创办了具身大脑公司穹彻智能 (evidence: [T04-S082, T04-S083, T01-S080, T01-S081])
- **核心身份**: 上海交通大学教授（人工智能学院 / 清源研究院），长江学者特聘教授；穹彻智能（Noematrix）联合创始人；据检索结果他还任中国人工智能学会（CAAI）具身智能专委会副主任、2026 中国具身智能大会程序主席——**这两项本轨未取到可访问的一手页面，仅作记录** (evidence: [T01-S080, T01-S083])
- **利益关系（必须点名）**: 学术 PI + 创业者双身份——穹彻智能由他与非夕科技创始人王世全共同创办（2023 年），主打「穹彻具身大脑 Noematrix Brain」，一年内完成三轮融资 (evidence: [T01-S081])。他同时在 CAAI 的学会体系里担任具身智能专委会副主任与大会程序主席，**这意味着他在中国具身智能的学术议程设置上有实际影响力** (evidence: [T01-S082, T01-S083])。
- **代表作品**: GraspNet-1Billion（CVPR 2020，统一了抓取评测协议，这是它最被低估的贡献）(evidence: [T04-S082])；AnyGrasp（T-RO 2023，时空域的鲁棒抓取感知）(evidence: [T04-S083])；行为理解（人体姿态与动作理解）方向的系列工作 (evidence: [T01-S080])
- **值得读 / 听 / 看的 3 件事**:
  - 📖 AnyGrasp 论文（arXiv:2212.08333）与 GraspNet-1Billion（CVPR 2020 开放全文）——他的一手学术输出 (evidence: [T04-S083, T04-S082])
  - 🌐 上海交大人工智能学院教师页（学术身份与研究方向的机构侧确认）https://sai.sjtu.edu.cn/cn/facultydetails/zzjs/lucewu (evidence: [T01-S080])
  - 🌐 上海交大清源研究院人物页（另一处机构侧身份确认）http://www.qingyuan.sjtu.edu.cn/a/lu-ce-wu1.html (evidence: [T01-S083])
  - ⚠️ CEAI 2026（中国具身智能大会）官网 `ceai.caai.cn` 在本次网络环境下**连接失败（curl 返回 000）**，因此「他任 CEAI 2026 程序主席」这一条**只以二手检索结果记录、不挂 evidence**；中国人工智能学会本身的官网见 Wave 1 (evidence: [T04-S106])
  - 📖 新华网《穹彻智能卢策吾：具身大脑领航，开启智能革新之旅》（2025-05-21，企业侧长报道）(evidence: [T01-S081])
- **核心思想关键词**: 抓取的统一评测协议（GraspNet 的真正贡献）、时空域的抓取感知（AnyGrasp 相对单帧方法的改进）、行为理解与具身智能的连接、具身大脑（公司口径）
- **voice_samples**:
  - ⚠️ **本人长材料（≥30 分钟中文长访谈或本人长文）未获取**。本轨检到的中文材料多为企业侧报道与会议介绍页，**不足以支撑逐字原话**；因此本卡片**不标注任何原话**。
  - 可核的方法论表述（**论文摘要原话，非口语**）：AnyGrasp 的核心主张是把抓取感知放到「空间与时间两个域」上做，而不是只在单帧点云上找抓取位姿 (source: T04-S083, 论文要义转述)
- **sub_skill_candidate**: `false` — 学术贡献确凿且已进入 Wave 1 canon，但本轨没有他的长篇一手口语材料。
- **dual_role**: `academic + founder`
- **最近 12 个月动态**: 据检索结果任 CEAI 2026（中国具身智能大会）程序主席（**一手页面不可访问，未挂 evidence**）。**⚠️ 本轨未取到他 2025-09 之后的具体公开发言内容**，这是本卡片最大的缺口。
- **争议 / 批评**: 本轨**未检到**针对他的具名公开批评。需要注意的结构性事实：他既是学术议程的组织者（专委会 + 大会程序主席）又是创业者，这在中国具身智能圈是常见组合，但意味着「学术共识」与「产业叙事」在人事上高度重叠。
- **可信度自评**: **low-medium** — 学术成果与身份跨源可核（Wave 1 canon 已独立确认 GraspNet / AnyGrasp），但**缺一手长材料**，按本轨纪律不能用二手中文报道撑他的观点。

---

### 18. 王鹤（He Wang）

- **One-liner**: 「用十亿级合成数据做具身预训练」这条路线在中国侧最系统的执行者——北大 EPIC 实验室 PI + 银河通用（Galbot）创始人，2026 年 ICRA 特邀 keynote 讲的正是「具身智能的 AlphaGo 与 ChatGPT 时刻」 (evidence: [T01-S084, T01-S085])
- **核心身份**: 北京大学助理教授（前沿计算研究中心 / 人工智能研究院），EPIC 实验室 PI；银河通用（Galbot）创始人（公司 2023 年创办，他在部分英文报道中被记为 CTO —— **本轨对具体头衔存在两种表述，不做单一断言**）(evidence: [T01-S084, T01-S086])
- **利益关系（必须点名）**: 学术 PI + 创业者双身份；银河通用据报道已融资超过 3.35 亿美元，投资方包括宁德时代与国家开发银行 (evidence: [T01-S086])。**「合成数据能顶大用」这个技术主张与他公司的技术路径完全一致**，且合成数据路线的成本结构对创业公司有利（不需要买大量真机与雇大量遥操作员）。
- **代表作品**: DexGraspNet 系列（百万级灵巧手抓取合成数据集；DexGraspNet 2.0 面向大规模合成杂乱场景）(evidence: [T01-S087])；GraspVLA（端到端具身抓取基座模型）、NavFoM（跨本体全景导航基座模型）、LDA-1B（跨本体隐动作模型）等 (evidence: [T01-S084])
- **值得读 / 听 / 看的 3 件事**:
  - 🌐 北大 EPIC 实验室页（论文、项目、keynote 的一手入口）https://pku-epic.github.io/ (evidence: [T01-S084])
  - 🎬 ICRA 2026 特邀 keynote *Towards the AlphaGo and ChatGPT Moments of Embodied AI*（**本轨通过其实验室页确认该 keynote 存在，未取到录像 URL**）(evidence: [T01-S084])
  - 📖 DexGraspNet 2.0 论文（arXiv:2410.23004）——合成数据路线的代表作 (evidence: [T01-S087])
  - 📖 MIT Technology Review *Innovators Under 35* 人物页（第三方对其工作的独立描述）https://www.innovatorsunder35.com/the-list/he-wang/ (evidence: [T01-S088])
- **核心思想关键词**: 十亿级合成数据预训练（billion-scale synthetic data）、高保真物理仿真的合成数据可以替代大部分真机采集、跨本体基座模型（导航 / 抓取 / 隐动作）、「具身智能的 AlphaGo 时刻」
- **数字口径**:
  - 「DexGraspNet 是首个百万级灵巧手抓取数据集，把合成数据生成效率提升 50 倍」——**来自第三方人物介绍页的转述，本轨未在论文中逐字核到「50 倍」的定义与基线** (evidence: [T01-S088])。引用时必须带「未核到分母」。
  - 「银河通用融资超过 3.35 亿美元」——来自第三方媒体，**未经公司公告交叉验证** (evidence: [T01-S086])。
  - 2026 年春晚与相关公开活动中 Galbot G1 的演示（搓核桃、叠衣服、串香肠等）被描述为「完全自主」——**这是活动方/公司口径，本轨未见干预率或试验次数** (evidence: [T01-S086])。
- **voice_samples**:
  - ⚠️ **本人长材料（≥30 分钟中文/英文长访谈或本人长文）未获取**。本轨只取到实验室页的研究方向表述与第三方人物介绍，**不足以标注任何原话**。
  - 可核的立场信号（**实验室页表述，非口语**）：EPIC 的自述目标是做出「高度可泛化、可扩展的机器人视觉与控制系统」，多个近期项目明确使用「十亿级合成数据」做预训练 (source: T01-S084, 要义转述)
- **sub_skill_candidate**: `false` — 路线鲜明且是中国侧「合成数据派」的最佳代表，但本轨缺一手长材料。
- **dual_role**: `academic + founder`
- **最近 12 个月动态**: 2026 年 ICRA 特邀 keynote（题目已确认）(evidence: [T01-S084])；实验室 2025-2026 密集产出跨本体基座模型系列工作（GraspVLA / NavFoM / LDA-1B / WAM-TTT）(evidence: [T01-S084])
- **争议 / 批评**:
  - **合成数据路线与「仿真对操作不可靠」的直接冲突**：Goldberg 的社论明确写仿真在操作上出名地不可靠 (evidence: [T01-S008])；Brooks 的批评更直接——仿真造不出触觉与力数据 (evidence: [T01-S001])。**王鹤的整条路线正好建立在这两位否定的前提上**。双方未互相点名，但这是本名单里最清晰的一组前提级分歧。
  - 本轨**未检到**针对他个人的具名公开批评。
- **可信度自评**: **low-medium** — 学术产出与实验室页可核，但公司信息、数字与头衔均依赖二手，且无一手长材料。

## 3. Phase 2 接口

### 3.1 每人核心一句话 + 它被几个来源印证

| 人 | 核心一句话（本轨归纳，非原话） | 跨源印证 |
|---|---|---|
| Rodney Brooks | 你采的数据里没有触觉和力，所以这条路学不出灵巧；这不是快慢问题，是模态缺口问题 | 3 源（本人 2 篇长文 + 行业辩论整理）(evidence: [T01-S001, T01-S002, T01-S007]) |
| Russ Tedrake | 大规模预训练是我所知**唯一**能给低层控制编程出「常识」的方式；但解决机器人学是长期议程 | 3 源（署名辩论 + LBM 论文 + Stanford seminar）(evidence: [T01-S009, T01-S016, T01-S015]) |
| Sergey Levine | 通用模型跨任务跨本体训练，最终会打败任何为单件事造的系统 | 3 源（π0.5 博客 + 论文 + 多档播客）(evidence: [T01-S022, T01-S025, T01-S026]) |
| Chelsea Finn | 不写手工代码，靠可扩展的基础模型 + 大规模数据集把物理常识教出来 | 3 源（YC talk + ICLR 报告 + ALOHA 线论文）(evidence: [T01-S031, T01-S032, T04-S075]) |
| Pieter Abbeel | （本轨未取到他本人的核心主张长材料——只确认了他的角色与履历） | 3 源，但均为身份类 (evidence: [T01-S035, T01-S037, T05-S009]) |
| Ken Goldberg | 训练语言模型的数据折算成人类时长约 10 万年，机器人这类数据根本不存在于互联网上；先用老派工程让机器人干活、边干活边攒真数据 | 4 源（本人社论 + 辩论 + Berkeley 访谈 + 机构页）(evidence: [T01-S008, T01-S009, T01-S011, T01-S096]) |
| Shuran Song | 采集接口的设计就是数据分布的设计——所以把采集从机器人上拆下来 | 2 源（UMI 论文 + Diffusion Policy 论文），**无本人口语佐证** (evidence: [T04-S080, T04-S076]) |
| Marc Raibert | 智能包含身体能力，所以「运动 AI」要和「认知 AI」并列 | 2 源（RAI 领导层页 + 研究所博客）(evidence: [T01-S042, T01-S046]) |
| Marco Hutter | 难建模的部分（驱动器动力学）用数据补，可建模的部分保留物理模型 | 3 源（三篇 Science Robotics）(evidence: [T04-S054, T04-S056, T04-S058]) |
| Sangbae Kim | 强化学习解决了很多双足运动问题，**但硬件才是使能者** | 2 源（Quanta 原话 + IEEE Spectrum 遥操作动机）(evidence: [T01-S052, T01-S051]) |
| Deepak Pathak | 一个模型丢进任何本体都能直接工作（omni-bodied） | 2 源（公司口径 + 行业报道），**无第三方验证** (evidence: [T01-S053, T01-S054]) |
| Jim Fan | 目标不是跑分，是「物理图灵测试」；真机数据是烧人力燃料，出路在仿真与合成数据 | 3 源（keynote 页 + YouTube + GEAR 页）(evidence: [T01-S058, T01-S060, T01-S059]) |
| Brett Adcock | 为人的环境造人形是正确路径，制造能力（BotQ）是护城河 | 3 源（Master Plan + 长访谈 + 产量记录）(evidence: [T01-S062, T01-S064, T01-S063]) |
| Bernt Børnich | 遥操作不是过渡，是产品本身——先卖出去，才有数据 | 2 源（Engadget + Humanoids Daily）(evidence: [T01-S067, T01-S068]) |
| 王兴兴 | 瓶颈在模型不在数据；当前 VLA 架构过于简单，更该走视频生成 / 世界模型 | 3 源，**全部二手** (evidence: [T01-S075, T01-S076, T01-S070]) |
| 彭志辉 | 行业核心问题已从「能不能做出来」转向「能不能稳定地干活」 | 2 源（公司官网演讲全文 + GO-1 论文）(evidence: [T01-S077, T04-S084]) |
| 卢策吾 | 抓取要在空间与时间两个域上做，而不是单帧点云找位姿 | 2 源（两篇论文），**无本人口语佐证** (evidence: [T04-S082, T04-S083]) |
| 王鹤 | 十亿级高保真合成数据可以承担具身预训练的主要负担 | 2 源（实验室页 + DexGraspNet 2.0），**数字口径未核** (evidence: [T01-S084, T01-S087]) |

### 3.2 共识 vs 真分歧

#### 少数几条真正的跨人跨源共识（**每条都有 ≥3 人、≥3 源**）

1. **「成功率必须带分母」是这一行的底线纪律**。Tedrake 团队为此做 1800+ 次真机 rollout 与盲测 A/B，并公开说常规评测可能测的是统计噪声 (evidence: [T01-S016])；Goldberg 用「几年几个月」的量级折算逼所有人报口径 (evidence: [T01-S008])；PI 自己在博客里写「不总是第一次就成功」 (evidence: [T01-S022])；Wave 1 的 canon 与 glossary 独立得出同一结论 (evidence: [T04-S075, T06-S042])。
2. **没有人真的认为「只要数据」或「只要模型」**。ICRA 2025 那场被分配到极端立场的辩论，8 位署名者里 Rus 直接说「我被分到支持数据方，但我的真实立场更微妙：我们两个都需要」；组织者也写明多数辩者对混合方法有共同尊重、举手表决后没多少人改变立场 (evidence: [T01-S009])。
3. **仿真在「飞 / 走」上可用、在「操作」上不可靠**，这是跨阵营的共同经验。Goldberg 明写这句话 (evidence: [T01-S008])；Wave 1 canon 从方法侧独立得出同一结论（接触与执行器动力学是 sim2real 最大头）(evidence: [T04-S065, T04-S061])。
4. **当前所有具身大模型的性能数字都来自作者自建评测**，没有跨机构公共基准 (evidence: [T04-S078, T04-S077, T04-S084, T01-S016])。

#### 五组真分歧（**双方是谁 / 各自论据 / 有没有正面交锋**）

**① 数据能不能解决机器人学 —— 有正面交锋，且有会议记录与期刊文本**

- **正方**：Animesh Garg（佐治亚理工）、Daniela Rus（MIT）、Russ Tedrake（MIT）。Garg 原话：data are not merely beneficial; rather, they are indispensable and foundational (evidence: [T01-S009])。Tedrake 原话：Large-scale pretraining from diverse multitask data is the best (only?) way that I know to program "common sense." (evidence: [T01-S009])
- **反方**：Aude Billard（EPFL）、Leslie Kaelbling（MIT）、Frank Park（首尔大学）。Billard 原话：I do not believe that data alone will "solve" robotics and automation（她用天文学「少而精的观测点」作类比）(evidence: [T01-S009])。Park 原话：expecting a parallel revolution in robotics is premature at best and wishful thinking at worst，以及 Rather than force-fitting models developed for vision and language to robots, new models that capture the inductive biases inherent to robotics are needed (evidence: [T01-S009])
- **交锋形式**：ICRA 2025（亚特兰大，2025-05-26~29）全会 keynote 辩论，>1000 人现场，Goldberg 主持，三对三牛津式；2025-08-27 全文发表于 *Science Robotics* (evidence: [T01-S009])。**这是本行业最可核的一次正面交锋，Phase 2 应优先使用。**
- **结果**：现场举手表决显示不少人被推着想得更深，但**没多少人改变立场** (evidence: [T01-S009])。

**② 视觉数据够不够学出灵巧 —— 有点名批评，被批评方未公开回应**

- **批评方**：Rodney Brooks（2025-09-26 本人博客）。他点名 Figure 与 Tesla，主张只采视觉数据是「采错了数据」，人类没有采集/存储/传输触觉的技术传统，因此这条路在数十年内做到人类灵巧是 pure fantasy thinking (evidence: [T01-S001])。
- **被批评方**：Figure、Tesla（Optimus），以及更广义的端到端 VLA 路线。**本轨未检到任何一方的公开回应** (evidence: [T01-S001, T01-S007])。
- **第三方反驳**：Scott Walter 公开指其犯「高悬果实谬误」——把「做不到人类的全部」偷换成「什么都做不了」；本轨仅取到二手整理，未取到原始长文 (evidence: [T01-S007])。
- **同向证据**：Goldberg 从量级角度、Sangbae Kim 从硬件与遥操作反馈角度得出相近结论 (evidence: [T01-S008, T01-S051])。

**③ 硬件是瓶颈还是借口 —— 有当面对立，同一篇文章内**

- **硬件派**：Sangbae Kim（MIT / Meta）原话：Reinforcement learning solved a lot of the bipedal locomotion problem, but the hardware was the enabler (evidence: [T01-S052])；Jonathan Hurst（Agility Robotics）原话：It's more like you kind of know that you need a quasi-direct drive motor to get close (evidence: [T01-S052])。
- **软件派**：Russ Tedrake 原话：The hardware is exceptional, and if you're blaming it, you're making excuses (evidence: [T01-S052])。
- **交锋形式**：Quanta Magazine 2026-03-13 的同一篇长报道，双方观点被并置 (evidence: [T01-S052])。
- **⚠️ 必须带的限定**：Kim 谈的是**腿足运动**为什么被 RL 解决，Tedrake 谈的是**灵巧操作**当前的瓶颈。**不要写成「Tedrake 反驳 Kim」。**

**④ 数据从哪来：遥操作 vs 手持采集 vs 仿真/合成 vs 边干活边采 —— 路线分歧，四方都用行动表态**

- **遥操作**：Chelsea Finn 的 ALOHA / Mobile ALOHA 线 (evidence: [T04-S075, T04-S079])；1X 的 Bernt Børnich 把遥操作直接做成了付费产品，明示会有人类操作员看到用户家里 (evidence: [T01-S067, T01-S068])。
- **手持 / 脱离机器人采集**：Shuran Song 的 UMI——它的存在本身就是对「遥操作太贵」的公开表态 (evidence: [T04-S080])。
- **仿真与合成数据**：Jim Fan / NVIDIA（GR00T-Dreams，宣称把开发周期从近三个月压到 36 小时）(evidence: [T01-S058, T01-S061])；王鹤 / 银河通用（十亿级合成数据预训练）(evidence: [T01-S084])。
- **边干活边采（第四条路）**：Ken Goldberg——先用老派工程把机器人做到能在真实商业环境里干活，让它一边干活一边产生数据；他用自家 Ambi Robotics「4 年采集 22 年真机数据、分拣超 1 亿个包裹」作论据（**自家数字、无第三方验证**）(evidence: [T01-S008])。
- **交锋形式**：**没有点名互怼**，但四条路线的论文/产品动机段互为反例；Goldberg 的社论是唯一把四条路并列比较并逐条给出否定理由的文本 (evidence: [T01-S008])。

**⑤ 时间表：2–3 年 vs 5–10 年以上 vs 数十年 —— 三个量级不同的公开判断，均有日期与场合**

| 判断 | 谁 | 何时何地 | 口径 |
|---|---|---|---|
| 具身智能的「ChatGPT 时刻」最快 2–3 年 | 王兴兴（宇树 CEO，卖硬件） | 2026-08-20 WRC 2026 主题演讲 | 定义为「陌生环境里完成约 80% 任务」，任务集合与判据未说明；**本轨仅有二手** (evidence: [T01-S070, T01-S071]) |
| 未来 2 年、5 年、10 年都不会发生（指人形做手术 / 替代工人 / 当管家） | Ken Goldberg（Berkeley，两家公司联创） | 2025-08-27 Berkeley News 访谈 + 同日 *Science Robotics* 社论 | 论据是数据量级差与遥操作线性不可扩 (evidence: [T01-S011, T01-S008]) |
| 数十年内做到人类那样的手工活是「纯幻想」 | Rodney Brooks（MIT 名誉教授，Robust.AI CTO） | 2025-09-26 本人博客 | 论据是触觉/力数据的模态缺口 (evidence: [T01-S001]) |
| 「解决机器人学」是很长期的议程，现在是早期、一切都很乱 | Russ Tedrake（MIT / TRI） | 2025-08-27 *Science Robotics* 署名段落 | **他站在数据方，但时间表判断偏保守** (evidence: [T01-S009]) |
| 具身智能已从「技术突破」进入「生产力部署」 | 彭志辉（智元 CTO，卖本体+模型） | 2026-05-07 APC 2026 演讲 | 未给任何出货量或成功率数字 (evidence: [T01-S077]) |
| 30 年视角，目标是把人形整合进劳动力 | Brett Adcock（Figure CEO） | 2022-05-20 Master Plan | 给的是 TAM 口径（42 万亿美元/年体力劳动报酬等），非需求验证 (evidence: [T01-S062]) |

**Phase 2 使用规则**：这六条不能相互抵消着写成「众说纷纭」。正确写法是**按利益关系分组**——卖硬件的（王兴兴）与卖本体+模型的（彭志辉、Adcock）给出的时间表最短；不承担商业化 KPI 的（Brooks、Goldberg、Tedrake）给出的最长；而 Goldberg 与 Brooks 都同时是公司联创/CTO，只不过他们的公司**不做人形**。

#### 一条必须写进 Phase 2 的谱系事实（防止简化）

**优化派与学习派不是对立阵营。** Tedrake 同时是《Underactuated Robotics》的作者、Diffusion Policy 与 OpenVLA 的共同作者、以及 ICRA 辩论中「数据方」的辩手 (evidence: [T04-S008, T04-S076, T04-S077, T01-S009])；Goldberg 是 Robot Learning Foundation（CoRL 主办方）主席，却写了最有力的一篇「数据不够」社论 (evidence: [T01-S008, T05-S022])。**把这两人写成「模型派」是错的。**

### 3.3 候选心智模型（每条 ≥3 个来源支持）

1. **先问分母，再看数字**——任何成功率/自主率/产量都要还原成「几个任务 × 几次试验 × 真机还是仿真 × 新物体吗 × 有没有人工重试 × 谁验证的」。支撑：TRI 用 1800+ rollout + 盲测 A/B 并明说常规评测可能是噪声 (evidence: [T01-S016])；PI 自述「不总是第一次成功」且博客页未给分母 (evidence: [T01-S022])；Figure 报产量但未公开销量 (evidence: [T01-S063])；1X 的视频里除两处外均为遥操作 (evidence: [T01-S067])；Wave 1 独立得出同一纪律 (evidence: [T04-S075, T06-S042])。
2. **数据不是一个量，是四条来路，各有不同的成本-迁移曲线**——遥操作（贵、线性、迁移好）、手持采集（便宜、有本体差）、仿真/合成（极便宜、操作上不可靠）、边干活边采（要先有能干活的系统）。支撑：Goldberg 逐条比较 (evidence: [T01-S008])；UMI 的存在 (evidence: [T04-S080])；NVIDIA 的合成数据主张 (evidence: [T01-S058])；1X 把遥操作卖给消费者 (evidence: [T01-S067])。
3. **一个人说的话，先看他靠什么吃饭**——本名单 18 人中 14 人有公司身份（创始人 / CTO / CEO / 厂商研究员），其中多数人的技术主张与其商业模式方向一致。支撑：Goldberg 在社论里直接引自家 Ambi 数据 (evidence: [T01-S008])；Jim Fan 的仿真主张指向 NVIDIA 卖的东西 (evidence: [T01-S058])；王兴兴「瓶颈在模型」对卖硬件的公司有利 (evidence: [T01-S075])；Brooks 批人形而自家做非人形仓储设备 (evidence: [T01-S005])。
4. **「谁能在别处重跑」比「我们做到了 X」更能定可信度**——支撑：VLA 无公共基准 (evidence: [T04-S077, T04-S078])；PI 开源 π0 权重使部分主张可复现 (evidence: [T05-S074])；智元开源百万级数据集 (evidence: [T05-S037])；Skild 的「omni-bodied」无任何第三方复现 (evidence: [T01-S053, T01-S054])。
5. **模态缺口 ≠ 数据量不足**——Brooks 的论点不是「数据不够多」，而是「触觉与力这一整个模态根本没被采集」；这与 Goldberg 的量级论证是**两种不同的悲观**，不能混为一谈。支撑：(evidence: [T01-S001, T01-S008, T01-S052])。
6. **硬件先于算法把可行方法集合限定死了**——支撑：Sangbae Kim「硬件才是使能者」 (evidence: [T01-S052])；Hurst「你得先有准直驱电机」 (evidence: [T01-S052])；Wave 1 从 SEA vs QDD 催生不同控制方法的角度独立得出同一结论 (evidence: [T04-S055, T04-S052])。**注意**：Tedrake 在同一篇文章里反对把当前失败归因于硬件 (evidence: [T01-S052])——这条心智模型有真实反方。

### 3.4 表达 DNA 素材

#### 这些人说话的共同特征（跨人观察，非单人）

- **爱把问题换算成可判定的量**。Goldberg 把「数据够不够」换成「折算成人类时长是多少年」 (evidence: [T01-S008])；王兴兴把「什么算成了」换成「陌生环境里完成约 80% 任务」 (evidence: [T01-S070])；Jim Fan 把「机器人做到什么程度」换成「你分不出是人还是机器收拾的」 (evidence: [T01-S058])。**这是这一行最鲜明的表达习惯：拒绝形容词，给判定条件。**
- **对 demo 的态度高度一致地冷淡**。Tedrake 团队用盲测 A/B 是因为「实验波动很容易盖过真实效果」 (evidence: [T01-S016])；Brooks 的记分卡里专门有一个「打太极」档，给那些「技术上发生了但没披露人工介入」的情况 (evidence: [T01-S002])；Wave 1 记录的行业拒绝清单第一条就是「不把『视频里做到了』当能力证据」 (evidence: [T06-S042])。
- **对外行的耐心程度分两类**：学术侧（Brooks、Goldberg、Tedrake）会花整段解释「为什么这个类比不成立」；厂商侧（Adcock、Jim Fan、彭志辉）用一句话愿景 + 一个画面（烛光晚餐、把人形整合进劳动力、生产力拐点）。**Phase 2 写作时要按场合切换，不要混用。**

#### 可直接引用的短句（**逐字标注，未标「原话」的一律不可当原话用**）

| 短句 | 谁 | 原话 / 转述 | 出处 |
|---|---|---|---|
| believing that this will happen any time within decades is pure fantasy thinking | Rodney Brooks | **原话** | (evidence: [T01-S001]) |
| Collecting just visual data is not collecting the right data. | Rodney Brooks | **原话** | (evidence: [T01-S001]) |
| We as a species have not developed technologies to capture touch, to store touch, to transmit touch | Rodney Brooks | **原话** | (evidence: [T01-S001]) |
| The declarations being made about humanoid robots are just not plausible. | Rodney Brooks | **原话** | (evidence: [T01-S002]) |
| We're at peak popular hype in all of robotics, AI, and machine learning. | Rodney Brooks | **原话** | (evidence: [T01-S002]) |
| Simulation data work well for robots that fly or walk, or even for doing backflips, but simulation is notoriously unreliable for robot manipulation. | Ken Goldberg | **原话** | (evidence: [T01-S008]) |
| Those data do not exist on the internet. | Ken Goldberg | **原话** | (evidence: [T01-S008]) |
| No; I agree that robots are advancing quickly but not that quickly. | Ken Goldberg | **原话** | (evidence: [T01-S011]) |
| To my mind as a roboticist, the blue-collar jobs, the trades, are very safe. | Ken Goldberg | **原话** | (evidence: [T01-S011]) |
| Large-scale pretraining from diverse multitask data is the best (only?) way that I know to program "common sense." | Russ Tedrake | **原话** | (evidence: [T01-S009]) |
| many people underestimate how essential common sense is for low-level control | Russ Tedrake | **原话** | (evidence: [T01-S009]) |
| The hardware is exceptional, and if you're blaming it, you're making excuses. | Russ Tedrake | **原话** | (evidence: [T01-S052]) |
| Reinforcement learning solved a lot of the bipedal locomotion problem, but the hardware was the enabler. | Sangbae Kim | **原话** | (evidence: [T01-S052]) |
| I do not believe that data alone will "solve" robotics and automation. | Aude Billard | **原话** | (evidence: [T01-S009]) |
| expecting a parallel revolution in robotics is premature at best and wishful thinking at worst | Frank Park | **原话** | (evidence: [T01-S009]) |
| data are not merely beneficial; rather, they are indispensable and foundational | Animesh Garg | **原话** | (evidence: [T01-S009]) |
| π0.5 is far from perfect, and it often makes mistakes both in terms of its high-level semantic deductions | Physical Intelligence（Levine/Finn 等共同署名） | **原话** | (evidence: [T01-S022]) |
| The RAI Institute allows us to pool everything on one site, from the idea stage to implementation. | Marco Hutter | **原话** | (evidence: [T01-S043]) |
| 具身智能正在从技术突破阶段，迈入生产力部署阶段 | 彭志辉 | **原话（中文）** | (evidence: [T01-S077]) |
| 聊天模型是被调用的，而机器人是持续运行的 | 彭志辉 | **原话（中文）** | (evidence: [T01-S077]) |
| 行业关注的核心问题，已经从「能不能做出来」，转向「能不能稳定地干活」 | 彭志辉 | **原话（中文）** | (evidence: [T01-S077]) |
| 企业不再单纯「销售机器人」，而是开始「交付结果」 | 彭志辉 | **原话（中文）** | (evidence: [T01-S077]) |
| General purpose humanoid robots built for a human environment is the desired route. | Brett Adcock | **原话** | (evidence: [T01-S062]) |

**⚠️ 明确不可当原话用的**（本轨只有要义转述）：王兴兴的全部表述、卢策吾的全部表述、王鹤的全部表述、Marc Raibert 关于「当前人形只会小心走路」的传闻引语、Bernt Børnich 的「比保洁更安全」、Jim Fan 的「物理图灵测试」定义与「烧人力燃料」、Deepak Pathak 的全部表述、Chelsea Finn 与 Pieter Abbeel 的全部表述。

### 3.5 边缘候选与本轨未成卡的人物

以下 10 人在本轨探查中反复出现且确有价值，但因**材料不足**或**与已成卡人物高度重合**未做完整卡片。Phase 2 若需要补，从这里开始：

- **Scott Kuindersma**（Atlas 全身规划与控制论文一作，与 Tedrake 联合做 Atlas + LBM）——2026-03 在 Quanta 中有原话 I don't think it's totally solved.（谈楼梯与门的可靠性）与 There's no world in which there are actually useful, autonomous humanoid robots that are only doing position-based control. (evidence: [T01-S052, T01-S019, T04-S087])
- **Jonathan Hurst**（Agility Robotics 联创兼首席机器人官）——Quanta 中原话 Not reliably.（回答 Digit 能不能应付任意楼梯和门）(evidence: [T01-S052])。**这是本轨检到的、由厂商创始人本人给出的最诚实的一句能力表述。**
- **Pulkit Agrawal**（MIT Improbable AI）——Quanta 原话 To have robots which work like humans, I think we have to master physics. (evidence: [T01-S052])；他的触觉手套工作被 Brooks 在批评文中引为替代方案 (evidence: [T01-S001])
- **Carolina Parada**（Google DeepMind Robotics 负责人）——Quanta 原话 Humans feel the forces that are working against you when you're trying to open a bottle. (evidence: [T01-S052])；DeepMind 是 RT 系列与 Gemini Robotics 的出处 (evidence: [T05-S057])
- **Karol Hausman**（Physical Intelligence 联合创始人兼 CEO）——有 2026-03 The Generalist 长播客；**本轨未取到可访问的一手页面 URL**，故未成卡 (evidence: [T01-S022])
- **Dieter Fox**（华盛顿大学教授；曾任 NVIDIA 机器人研究高级总监，2025-07 转任 Ai2 机器人方向负责人）——个人主页可访问，但本轨未取到他 2025-2026 的长材料 (evidence: [T01-S089, T01-S090, T04-S004])
- **熊友军**（北京人形机器人创新中心 / 国家地方共建具身智能机器人创新中心总经理，「天工」团队负责人；华中科技大学机器人遥操作方向博士，人形领域 20+ 年）——2026-03-30《北京日报》有对话式长报道，中国电子学会站点有其 WRC 演讲条目《具身智能：打造人机共生的新时代》；**本轨未取到本人长材料的一手全文**，且中文二手不作证据，故未成卡 (evidence: [T01-S091, T01-S092, T01-S093, T05-S040])
- **Nancy M. Amato（UIUC）/ Seth Hutchinson（东北大学）**——ICRA 2025 大会共同主席，是那场辩论的发起者；他们在文中把当前局面称作库恩意义上的「范式转移」 (evidence: [T01-S009])
- **Daniela Rus（MIT CSAIL 主任）**——ICRA 辩论中原话 I believe that we need both data and mathematical models.，并给出「不在实验室里，第一性原理就不够用了」的具体例子 (evidence: [T01-S009])
- **Aaron Saunders（Boston Dynamics CTO）**——本轨**未检到**他 2025-2026 的可访问长材料；Boston Dynamics 侧的可核发声集中在公司博客与 TRI 合作公告上 (evidence: [T01-S019, T01-S044, T05-S059])

### 3.6 薄弱信号（必须写进 SKILL.md 的诚实边界）

| 维度 | 状况 | 判定 |
|---|---|---|
| figure 总数 | 18 位成卡（目标 12–18） | ✅ 不冷僻 |
| manifest 条数 | 94 条（目标 ≥90） | ✅ |
| 每人 ≥3 条独立来源 | 18/18 满足 | ✅ |
| **每人 ≥1 条本人长材料** | **仅 8/18 满足**（Brooks、Tedrake、Levine、Finn、Goldberg、Jim Fan、Adcock、彭志辉） | ⚠️ **不达标，必须在诚实边界写明** |
| 可信度 low / low-medium 占比 | 3/18（王兴兴、卢策吾、王鹤）＝ 16.7% | ✅ 低于 30% 阈值 |
| 近 12 个月动态填写率 | 18/18 有内容，其中 16 位有明确 YYYY-MM | ✅ |

**四处必须写进 SKILL.md 诚实边界的薄弱点**：

1. **中国侧的一手材料严重不足，且这是结构性的而非偶然**。18 位中的 4 位中国人物里，只有彭志辉有可逐字引用的一手中文原话（且来自公司发布会语境）(evidence: [T01-S077])。王兴兴、卢策吾、王鹤的观点**全部依赖二手媒体**——本轨按纪律拒绝用中文二手撑他们的技术判断 (evidence: [T01-S070, T01-S075, T01-S081, T01-S086])。原因是：这些人的一手长输出要么在闭门会议、要么在短视频、要么以英文论文形式存在（论文属 Track 04 而非本轨）。**SKILL.md 里凡涉及「中国从业者怎么想」的判断，可信度必须显式降级。**
2. **纯学术型人物拿不到 voice DNA**。Shuran Song、卢策吾、Marco Hutter（技术议题上）、Deepak Pathak 都没有可用的长口语材料，他们的思想只能从论文摘要转述 (evidence: [T04-S080, T04-S083, T04-S054, T01-S053])。这会让 Phase 2 的语气提炼偏向「有播客的人」，即偏向创业者与美国学术明星。
3. **厂商侧数字几乎全部无第三方验证**。Figure 的产量、Skild 的跨本体能力、NVIDIA 的仿真加速比、1X 的隐私机制、Ambi 的 22 年数据、Galbot 的融资额与「50 倍效率」——**没有一条经过独立验证** (evidence: [T01-S063, T01-S053, T01-S058, T01-S067, T01-S008, T01-S088])。
4. **两条本轨确认为不可达的线索**：Berkeley 的 `rail.eecs.berkeley.edu` 与 `people.eecs.berkeley.edu/~svlevine/`（curl 返回 000，Wave 1 也遇到同一问题）；`ceai.caai.cn`（中国具身智能大会官网，curl 返回 000）。这三条**未进 manifest、未挂 evidence**，下次 refresh 需换网络环境重试。

**Wave 1 留给本轨的两个未闭合项，处理结果**：
- ✅ **已闭合**：Rodney Brooks 对当前人形 / VLA 路线的具体批评原话——本轨取到 2025-09-26 全文并逐字引用了 6 条，其中包含他点名 Figure 与 Tesla (evidence: [T01-S001])。
- ❌ **仍未闭合**：Berkeley CS287 / CS285 课程页在本次网络环境仍不可访问，与 Wave 1 结论一致。

## 4. 自检清单（提交前逐条过）

- [x] **候选清单 20-30**：探查 28 位候选，成卡 **18** 位（目标 12-18），其余 10 位进 §3.5 边缘候选 —— 未触发冷僻协议
- [x] **每位 figure ≥ 3 条来源**：18/18 满足（最少 4 条，最多 15 条，含跨轨引用）
- [x] **manifest ≥ 90 条**：94 条
- [ ] **每位 ≥1 条本人长材料**：**只有 8/18 满足**（Brooks / Tedrake / Levine / Finn / Goldberg / Jim Fan / Adcock / 彭志辉）—— **本项不达标，已在 §3.6 与总览表逐人标出**，Phase 2 必须据此降级另外 10 人的观点权重
- [x] **一手来源占比 ≥ 50%**：verified_primary + surrogate_primary = 64.9%
- [x] **没有用任何黑名单来源**：机械扫描全文零命中
- [x] **surrogate_primary 的 note 全部含规定关键词**：27/27，未使用 `official`
- [x] **last_checked 全部 2026-09-02**：94/94
- [x] **「最近 12 个月动态」填写率 ≥ 80%**：18/18 有内容，16 位带明确 YYYY-MM
- [x] **可信度自评每位都有**：18/18；low / low-medium 的 3 位（王兴兴、卢策吾、王鹤）均写明理由是「一手长材料未获取」
- [x] **Phase 2 接口齐全**：核心一句话表（18 行）+ 4 条跨源共识 + **5 组真分歧**（其中 3 组有正面交锋的可核记录）+ 6 条候选心智模型 + 表达 DNA（24 条逐字标注的可引用短句）+ 边缘候选 10 人 + 薄弱信号 4 条
- [x] **原话 vs 转述严格分开**：所有标「原话」的均逐字取自可访问的一手/二手页面；§3.4 末尾另列「明确不可当原话用」的名单
- [x] **争议写实**：3 组有正面交锋的分歧均给出双方姓名、场合、日期与逐字论据；未把「路线不同」写成「互相攻击」；对未检到回应的情况明写「未检到回应」
- [x] **利益关系点名**：18/18 卡片均有「利益关系（必须点名）」或等效段落，写清创始人 / 投资关系 / 雇主 / 学会职务
- [x] **数字带口径**：所有出现的百分比、产量、融资额均标注了发布方、时点、分母是否公开、有无第三方验证；无法确定口径的（宇树出货量、Figure 销量、1X 干预率、Skild 跨本体成功率）一律写「未公开」
- [x] **无空标题、无未完成标记**：机械检索确认全文没有任何未完成标记，每个标题下均有实质内容

### 已知缺口（交 Phase 1.5 裁决）

1. **本人长材料只覆盖 8/18** —— 最影响下游的一条。要补，优先级为：王兴兴（WRC 2026 官方演讲录像）> 卢策吾 / 王鹤（中文长访谈或 keynote 录像）> Shuran Song（近期 talk）> Deepak Pathak（T01-S056 访谈原文）。
2. **未抓字幕**：Brooks 以外的多数英文长 talk（Finn YC talk、Tedrake Stanford seminar、Jim Fan Actuate keynote、Goldberg 长视频）本轨只取到页面元数据，**未跑转录**。Phase 2 若需要更厚的 voice DNA，应对这 4 条跑 `tools/transcribe/youtube.sh`。
3. **与 Wave 1 的一处口径需要 Phase 1.5 确认**：Wave 1 canon 把 Rodney Brooks 归为「行为主义 / 具身认知派」的当前代表，本轨发现他 2025-2026 年的公开论证主线**已经不是行为主义，而是「数据模态缺口」**（触觉与力）。两者不矛盾，但 Phase 2 写谱系时应以本轨的近期证据为准 (evidence: [T01-S001, T04-S115])。
