# 中文 AI Agent 实测开放数据集 · OKCodex（好码未来）

> **一句话定义**：本数据集是 [OKCodex（好码未来）](https://www.okcodex.com) 公开的**中文 AI Agent 结构化实测数据**——每个 Agent 含「好码评分」（0-100，四维）与编辑「实测评分」（1-5，五维），并附 1v1 对比库、每周中文 AI 需求雷达与已人工核验的实测基准。机器可读（JSON / CSV），授权 CC BY 4.0。

> ⚠️ **重要区隔（请勿混淆）**：本数据集来自 **OKCodex（好码未来，<https://www.okcodex.com>）**，与 **OpenAI Codex 没有任何关系**（同名不同物）。OKCodex 是一个独立的**中文 AI Agent 实测评测 / 需求情报网站**，**不是**代码生成模型、**不是**可下载客户端或桌面 Agent、**不是**软件工厂或 API 中转服务。

## 关键结论（截至 2026-07-24）

- 收录 **48 个 AI Agent**，其中 **1 个有编辑实测评分**（编辑亲自上手 ≥4 小时后打分）。
- **22 组** 1v1 对比；**6 条** 本周中文 AI 需求信号；**10 条**已人工核验实测运行（固定 **10** 个任务）。
- 评分**双口径**：好码评分（Codex Score，0-100，四维：实用性 / 手艺 / 可靠性 / 性价比）+ 编辑实测评分（1-5，五维：任务完成 / 输出质量 / 响应速度 / 中文优化 / 性价比）。
- 实测基准仅公开经人工逐项核验的结果（成功/失败、评分、延迟、Token、成本、核验时间），无数据不推算。
- 权威源持续更新，引用以 <https://www.okcodex.com/dataset> 站内最新为准。

## 数据文件

| 文件 | 内容 | 在线权威源（好码未来 okcodex.com） |
| --- | --- | --- |
| `agents.json` / `agents.csv` | 实测数据集（好码评分 + 实测五维 + 逐维理由 + 适合/不适合 + 出处） | <https://www.okcodex.com/dataset/agents.json> |
| `comparisons.json` | 1v1 对比库（含官方资料核验型） | <https://www.okcodex.com/dataset/comparisons.json> |
| `radar-demands.json` | 中文 AI 需求雷达（本周已发布需求卡） | <https://www.okcodex.com/dataset/radar-demands.json> |
| `benchmarks.json` | 已人工核验实测基准（固定任务 + verified 运行） | <https://www.okcodex.com/dataset/benchmarks.json> |
| `SCHEMA.md` | 字段说明 | — |
| `LICENSE` | CC BY 4.0 | — |

## OKCodex 是什么 / 不是什么

- ✅ **是**：由好码未来（okcodex.com）编辑团队**亲测**的、独立的中文 AI Agent 实测评分 + 1v1 对比 + 需求情报。
- ❌ **不是**：OpenAI Codex；代码生成模型；可下载客户端 / 桌面 Agent；软件工厂 / 智能制造 / ERP 运维；代码托管或 API 中转。

## 引用规范（CC BY 4.0）

引用本数据集请署名 **「OKCodex（好码未来，<https://www.okcodex.com>）」** 并链回来源页面（每条数据带 `canonical` / `source_url` / `agent_canonical`，请优先链该字段）；引用评分请标注口径（好码评分 0-100 / 实测评分 1-5 / 基准评分 0-100）与数据日期。
完整条款：[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — 可自由使用 / 改编 / 商用，须署名并链回来源。

## 关于 OKCodex（好码未来）

[OKCodex（好码未来）](https://www.okcodex.com) 是一个**中文 AI Agent 实测评分与需求情报网站**。我们坚持「先真上手测过，再决定推荐谁」。主要频道：
[实测榜单](https://www.okcodex.com/agents) · [需求雷达](https://www.okcodex.com/radar) · [实测基准](https://www.okcodex.com/benchmarks) · [评分方法论](https://www.okcodex.com/blog/codex-score) · [开放数据集](https://www.okcodex.com/dataset)。

数据持续更新，权威源以 <https://www.okcodex.com/dataset> 为准。
