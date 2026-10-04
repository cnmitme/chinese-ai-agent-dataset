# SCHEMA — agents.json

顶层：`{ "meta": {...}, "agents": [...] }`，`meta` 含 name/source/license/attribution/generated_at/count/schema_version；网站证据投影契约为 `okcodex.agent-evidence.v1`。

每个 agent：
| 字段 | 说明 |
| --- | --- |
| `slug` / `name` / `name_en` | 唯一标识与中英文名 |
| `tagline` / `categories` / `model` / `pricing` / `language` | 定位、分类、底层模型、定价、语言 |
| `codex_score` | 好码评分（0-100）：overall + utility/craft/reliability/value |
| `url` / `canonical` | 官网链接 / OKCodex 权威页面（引用请链此） |
| `review` | 来源型评论对象（无则 null） |
| `review.overall` + `score_task/quality/speed/chinese/value` | 来源型评论评分（1-5）综合与五维 |
| `review.publication_mode` / `review_evidence_status` | automatic 为自动资料分析；manual 是发布来源，不自动证明人工亲测；catalog_only 无合格评论 |
| `review.evidence_level` / `review.tested_at` / `review.review_run_id` | 声明证据类型 / 声明时间 / 关联运行标识；资料来源核对与这些字段本身不等同于人工实测，实际运行须核对 benchmarks.json |
| `review.score_reasons` | 逐维打分理由 |
| `review.one_liner` / `verdict` | 一句话定义 / 关键结论 |
| `review.fit_for` / `not_fit_for` | 适合 / 不适合人群 |
| `review.source_url` / `tested_version` / `reviewer` / `reviewed_at` | 出处 / 声明版本 / 署名 / 评论日期 |

`comparisons.json`：每条含 slug_a/slug_b/url_slug/one_liner/verdict/verdict_a_for/verdict_b_for/reviewer/canonical；官方资料型含 sources 与核验时间。
`radar-demands.json`：每条含 query/trend/sources/pain/matched_agents/week_label/opportunity_score/score_breakdown。
`benchmarks.json`：顶层含 `meta`（CC BY 4.0 / 任务数 / 仅 verified 计数）、`tasks`（固定任务清单）、`results`（仅 verification_status=verified 的运行：outcome/score/latency/token/cost/verified_at）。
