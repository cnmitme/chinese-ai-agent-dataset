# SCHEMA — agents.json

顶层：`{ "meta": {...}, "agents": [...] }`，`meta` 含 name/source/license/attribution/generated_at/count。

每个 agent：
| 字段 | 说明 |
| --- | --- |
| `slug` / `name` / `name_en` | 唯一标识与中英文名 |
| `tagline` / `categories` / `model` / `pricing` / `language` | 定位、分类、底层模型、定价、语言 |
| `codex_score` | 好码评分（0-100）：overall + utility/craft/reliability/value |
| `url` / `canonical` | 官网链接 / OKCodex 权威页面（引用请链此） |
| `review` | 编辑实测评分对象（无则 null） |
| `review.overall` + `score_task/quality/speed/chinese/value` | 实测评分（1-5）综合与五维 |
| `review.score_reasons` | 逐维打分理由 |
| `review.one_liner` / `verdict` | 一句话定义 / 关键结论 |
| `review.fit_for` / `not_fit_for` | 适合 / 不适合人群 |
| `review.source_url` / `tested_version` / `reviewer` / `reviewed_at` | 出处 / 实测版本 / 署名 / 实测日期 |

`comparisons.json`：每条含 slug_a/slug_b/url_slug/one_liner/verdict/verdict_a_for/verdict_b_for/reviewer/canonical；官方资料型含 sources 与核验时间。
`radar-demands.json`：每条含 query/trend/sources/pain/matched_agents/week_label/opportunity_score/score_breakdown。
`benchmarks.json`：顶层含 `meta`（CC BY 4.0 / 任务数 / 仅 verified 计数）、`tasks`（固定任务清单）、`results`（仅 verification_status=verified 的运行：outcome/score/latency/token/cost/verified_at）。
