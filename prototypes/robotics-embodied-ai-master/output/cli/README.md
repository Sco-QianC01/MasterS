# 机器人与具身智能 CLI

把 机器人与具身智能 master skill 的认知 OS 物化成 bash 工具。
不替代 SKILL.md（思维顾问），是它的「执行端」：交互问询 → 应用 playbook / protocol → 输出结构化报告。

## 用法

所有脚本支持 `--help` / `--explain` / `--dry-run` / `--json` 四个标准 flag。

```bash
# 拿到新问题时, 按 N 个研究维度做功课
./protocol/agentic.sh

# 决策树评估 (基于 playbook)
./decision/topic-1.sh
# SOP 走查 (workflow)
./workflow/workflow-1.sh

# 看背后的心智模型 / playbook (不交互)
./protocol/agentic.sh --explain
```

## 脚本清单

| 脚本 | 作用 |
|------|------|
| `protocol/agentic.sh` | Agentic Protocol (7 维度) — 拿到新问题时按这一行的研究维度做功课 |
| `decision/topic-1.sh` | 数据 决策树 (1 条规则) |
| `decision/topic-2.sh` | 案例 决策树 (5 条规则) |
| `decision/topic-3.sh` | 仿真 决策树 (1 条规则) |
| `decision/topic-4.sh` | 分母 决策树 (1 条规则) |
| `decision/topic-5.sh` | —— 决策树 (1 条规则) |
| `workflow/workflow-1.sh` | 任务定义与可行性判断（先证明「不该上机器人」） SOP 走查 |
| `workflow/workflow-2.sh` | 形态与本体选型（含成本与工期账） SOP 走查 |
| `workflow/workflow-3.sh` | 误差预算与硬件选型（从末端精度反推） SOP 走查 |
| `workflow/workflow-4.sh` | 环境搭建与标定（手眼、工件坐标系、力传感器、重复性验收） SOP 走查 |
| `workflow/workflow-5.sh` | 仿真环境与资产准备（建模到什么程度就够） SOP 走查 |
| `workflow/workflow-7.sh` | 数据采集与训练循环（遥操作的人力成本与停止条件） SOP 走查 |
| `workflow/sim-to-real.sh` | sim-to-real 迁移与真机调试 SOP 走查 |
| `workflow/workflow-9.sh` | 评测协议设计与「怎么读别人的评测」 SOP 走查 |
| `workflow/workflow-10.sh` | 安全评估与合规 SOP 走查 |
| `workflow/workflow-11.sh` | 现场部署与集成（节拍、换型、异常恢复、PLC/MES 边界） SOP 走查 |
| `workflow/workflow-12.sh` | 监控、失败复盘与迭代 SOP 走查 |
| `workflow/workflow-13.sh` | 演示与交付验收（POC vs 量产） SOP 走查 |

## 设计与生成

CLI 子树由 `tools/cli_writer.py` 自动从 `references/synthesis.md` (Section 2 Playbook + Section 9 Agentic Protocol) 和 `references/research/03-workflows.md` 生成。

完整 spec 在 master-skill 仓库 `references/cli-spec.md`。

## 重新生成

如果 synthesis.md 或 03-workflows.md 更新了, 重跑:

```bash
python3 <master-skill>/tools/cli_writer.py emit \
  --skill-dir <this-skill-dir> \
  --synthesis references/synthesis.md \
  --workflows references/research/03-workflows.md \
  --industry-cn "机器人与具身智能"
```
