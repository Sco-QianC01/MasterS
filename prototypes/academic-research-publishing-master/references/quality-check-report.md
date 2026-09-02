# Quality Check Report — academic-research-publishing-master

- **Skill version**: v1.4 (generator master-skill v1.4)
- **Check date**: 2026-09-02
- **Subagent runs**: 4.1 (3 questions) / 4.2 (1 question + gap audit) / 4.3 (1 voice sample + label audit) / claim audit / package audit
- **Note**: this run is a continuation. An earlier fire the same day (18:04–20:00) produced research + synthesis + SKILL.md and passed the mechanical rubric, then was cut before Phase 4. Artifacts were integrity-checked (no empty tail sections, no half-done markers, 0 blacklisted URLs) before continuing.

## 4.1 Sanity check — ✅ PASS (3/3)

Ground truth taken from Track 02/04 (not from the tested file).

| # | Question | Ground truth | Verdict |
|---|----------|--------------|---------|
| 1 | p=0.07，审稿人要求事后功效分析 | 观测功效与 p 值一一对应、无信息量；正解是效应量+置信区间、敏感性分析、必要时等效性检验（`02-tools.md:1042`, `04-canon.md:1061`） | ✅ |
| 2 | 预注册协方差分析改为非参数检验 | 偏离允许，但必须在论文中明确列出偏离项与理由，预注册分析仍需报告（`02-tools.md:615`） | ✅ |
| 3 | 新开放获取刊两周审完、自称影响因子 | 靠正向核查清单而非黑名单：DOAJ 收录、编委真实且知情、评审记录可查、费用投稿前明示（`03-workflows.md:378`, `T03-S055` 德尔菲共识定义） | ✅ |

## 4.2 Edge case — ✅ PASS

题：全自动 LLM 做系统综述 title/abstract 筛选能否进论文。答案显式调用 4 个心智模型（§1.6 / §1.5 / §1.2 + playbook 9），未给定论，点名三处需现场核实的来源（目标刊 AI 条款、PRISMA 及其自动化扩展现行版本、Cochrane/JBI 立场）并标注本文件截止日。Hedging 充分。

## 4.3 Voice check — ⚠️ PARTIAL

- 字面判据达标：14 个 Tier-1 术语自然使用、0 处厂商话术、0 处 ChatGPT 腔（无「总的来说」「值得注意的是」「综上所述」），`06-glossary.md` §L 十二条外行破绽全部避开。
- 判 PARTIAL 的理由：register 偏通用。两段样本都从结论/指令开头，而 `01-figures.md` 记录的中文侧特征恰恰相反（从具体场景开头，如「昨天参加了一场博士生预答辩…」）；另有「一是/二是/三是」「三件」两处整齐三段式，属轻度机器腔。**不改判 PASS 以换绿灯。**
- 引文标签审计（本轮重点）：§5.A 十四条语料与 `01-figures.md` 上游标签逐条对齐，**没有发现「要义转述」被升格成「原话」**；11 条反引号英文原话全部在研究文件中逐字可查。

## 4.4 Mechanical rubric — ✅ PASS

16 pass / 0 partial / 0 fail / 1 needs_subagent（item 7 由上方 4.3 判 PARTIAL）。640 条 manifest，一手 96.6%，黑名单 0。

## 修正记录（Phase 4 发现、已回改 synthesis.md 并重新生成）

11 处内容错误 + 1 处可用性缺口，全部为机械 rubric 查不到的语义问题：

1. 投掠夺性期刊被写成中国明文列举的科研失信行为 — 该法规列举的是买卖论文与代写代投，掠夺性期刊是另一套德尔菲共识判据（范围膨胀）
2. 中国科技部 AI 评议指引被并入「一律禁止」— 原文是「须事先征得评议活动组织者同意」，与三家出版商措辞不同（引证指向的文档说的不是这件事）
3. 新兴层「七条里有六条 high」— 实际七条全部 high，且与本文件自己的小节标题打架
4. Time-decay Registry 的 Tool stack / Workflows 写 high，而正文两处小节写 medium（内部矛盾，已在生成器修）
5. 「欧洲有大规模转型协议」漏掉 cOAlition S 对转型安排的资助已于 2024 年底终止 —— 而所引来源正是那份终止公告
6. 入门/资深差异的发现挂在 ICMJE 2026-01 更新公告上（该结论上游本无 source_id）
7. 撤稿率/接受率/审稿周期口径挂在影响因子说明与分区表停更公告上（上游即已错挂，本轮改正）
8. 审稿措辞解码挂在 Elsevier 决定类型页上，引用胁迫改挂 `T06-S026, T06-S036`
9. 47% 复制判据丢了「95% 预测区间」这一口径 —— 出现在本文件唯一要求「数字必须带口径」的镜片里
10. 「共同一作/共同通讯」观察挂错马军的博文（S082→补 S083），且引号内文字被改动（「与」应为「/」）
11. Agentic Protocol 把「数字口径提醒」指向 `01-figures.md`，该字段实际只在 `04-canon.md`
12. （4.1 发现的缺口）事后功效在全文出现三次禁令、零次解释 —— 补上「与 p 值一一对应、不提供新信息」的技术理由

## 未采纳、如实记录

4.2 的结构性缺口批评成立但本轮未补（单轮只做一个行业）：zh-CN 侧的学位法/论文抽检与盲审/教科技〔2020〕2号/国际期刊预警名单主要活在研究文件里；`03-workflows.md` 的理工–社科九行差异表未进正文，而正文 Agentic 维度 1 正指向它；基金申请「本子」的八段结构与形式审查自查表被压缩掉；Track 05 的官方源清单未成模块。列为该 slug 下次 update 的第一优先。
