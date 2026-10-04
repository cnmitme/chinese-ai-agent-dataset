# 中文 AI Agent 证据开放数据集 · OKCodex（好码未来）

> **一句话定义**：本数据集是 [OKCodex（好码未来）](https://www.okcodex.com) 公开的**中文 AI Agent 结构化目录与证据数据**——目录评分（0-100）与来源型评论评分（1-5）分别标注，不等同于基准实测，并附 1v1 对比库、每周中文 AI 需求雷达与已人工核验的实测基准。机器可读（JSON / CSV），授权 CC BY 4.0。

> ⚠️ **重要区隔（请勿混淆）**：本数据集来自 **OKCodex（好码未来，<https://www.okcodex.com>）**，与 **OpenAI Codex 没有任何关系**（同名不同物）。OKCodex 是一个独立的**中文 AI Agent 选型评测 / 需求情报网站**，**不是**代码生成模型、**不是**可下载客户端或桌面 Agent、**不是**软件工厂或 API 中转服务。

## 关键结论（截至 2026-10-04）

- 收录 **55 个 AI Agent**，其中 **10 个有来源型评论评分**；`publication_mode=automatic` 表示自动生成的资料分析，不是人工亲测。
- **22 组** 1v1 对比；**11 条** 本周中文 AI 需求信号；**10 条**已人工核验实测运行（固定 **10** 个任务）。
- 覆盖 1 个目录条目；记录版本：deepseek-v4-flash；最近运行：2026-07-12T05:06:56.901195+00:00。运行次数不等于实测产品数。
- 评分**双口径**：好码评分（Codex Score，0-100，四维：实用性 / 手艺 / 可靠性 / 性价比）+ 来源型评论评分（1-5，五维：任务完成 / 输出质量 / 响应速度 / 中文优化 / 性价比）。
- 实测基准仅公开经人工逐项核验的结果（成功/失败、评分、延迟、Token、成本、核验时间），无数据不推算。
- 权威源持续更新，引用以 <https://www.okcodex.com/zh/dataset> 站内最新为准。

## 数据文件

| 文件 | 内容 | 在线权威源（好码未来 okcodex.com） |
| --- | --- | --- |
| `agents.json` / `agents.csv` | 目录资料与来源型评论（好码评分 + 评论五维 + 逐维理由 + 适合/不适合 + 出处） | <https://www.okcodex.com/zh/dataset/agents.json> |
| `comparisons.json` | 1v1 对比库（含官方资料核验型） | <https://www.okcodex.com/zh/dataset/comparisons.json> |
| `radar-demands.json` | 中文 AI 需求雷达（本周已发布需求卡） | <https://www.okcodex.com/zh/dataset/radar-demands.json> |
| `benchmarks.json` | 已人工核验实测基准（固定任务 + verified 运行） | <https://www.okcodex.com/zh/dataset/benchmarks.json> |
| `SCHEMA.md` | 字段说明 | — |
| `LICENSE` | CC BY 4.0 | — |

## OKCodex 是什么 / 不是什么

- ✅ **是**：由好码未来 OKCodex（okcodex.com）发布的目录资料、来源型评论、1v1 对比、需求情报及独立标注的核验运行。
- ❌ **不是**：OpenAI Codex；代码生成模型；可下载客户端 / 桌面 Agent；软件工厂 / 智能制造 / ERP 运维；代码托管或 API 中转。

## 引用规范（CC BY 4.0）

引用本数据集请署名 **「OKCodex（好码未来，<https://www.okcodex.com>）」** 并链回来源页面（每条数据带 `canonical` / `source_url` / `agent_canonical`，请优先链该字段）；引用评分请标注口径（好码评分 0-100 / 来源型评论评分 1-5 / 基准评分 0-100）与数据日期。
完整条款：[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — 可自由使用 / 改编 / 商用，须署名并链回来源。

## 关于 OKCodex（好码未来）

[OKCodex（好码未来）](https://www.okcodex.com) 是一个**中文 AI Agent 选型与证据情报网站**。我们区分目录资料、来源分析和有证据的实际运行，不将自动评论描述为人工亲测。主要频道：
[Agent 目录](https://www.okcodex.com/agents) · [需求雷达](https://www.okcodex.com/radar) · [实测基准](https://www.okcodex.com/benchmarks) · [评分方法论](https://www.okcodex.com/trends/codex-score) · [开放数据集](https://www.okcodex.com/zh/dataset)。

数据持续更新，权威源以 <https://www.okcodex.com/zh/dataset> 为准。
GitHub 镜像：<https://github.com/cnmitme/chinese-ai-agent-dataset>。
