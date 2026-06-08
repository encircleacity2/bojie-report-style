# bojie-report-style 「白皮笔法」

> A personal writing-style skill for **industry strategy reports & leadership reporting** — captures Bojie's analyst voice so AI-drafted reports stop reading like AI. **Works for both English and Chinese.**

*English version first, 中文版在下方 ↓*

---

# 🇬🇧 English

A [Claude Code](https://claude.com/claude-code) / Claude Agent **skill** that encodes one person's (Bojie Sun, BytePlus SA) house style for writing and rewriting **industry solutions, sector reviews, campaign summaries, market-sizing analyses, and leadership reports** — typically Lark (Feishu) Docx, in **either English or Chinese**.

It was distilled from two of Bojie's own hand-written documents (a staged campaign summary and an industry solution doc), after an AI-generated first draft came back too "AI-flavored" (slogans, rainbow callouts, emoji, fake auto-generated charts). The skill turns that critique into a reusable rule set.

## What it does

When triggered, it steers the writing toward Bojie's voice and away from common LLM tells:

- **Analyst voice, not marketing voice** — show the reasoning chain and the math; keep the hedges, drop the slogans.
- **An anti-"AI-flavor" checklist** — zero-tolerance tells to strip: emotional emoji, rainbow callouts, templated symmetry, fake auto-generated SVG charts, "Source: …" footnotes, "three asks for leadership" packaging, etc.
- **Bilingual coverage (§8)** — separate AI-tell checklists for **Chinese** and **English**. The English list specifically kills LLM filler (*delve, leverage, robust, seamless, unlock, in today's fast-paced world*), the triadic-adjective rhythm tic, em-dash overuse, and "In conclusion" bloat.
- **Structural skeletons** — market-sizing tables, an *investment-quadrant* prioritization frame (All-in / Long-term / Explore / Watch) instead of bare P0/P1, KPI target-decomposition with explicit implementation paths.
- **A solution-writing template** — every solution opens with `Market trend → Solution summary → Value prop (Model / Ecosystem / Service)`, names each model's job (Seed / Seedream / Seedance), layers delivery modes (Workflow / Copilot / Agent), and **shows real demos** instead of describing them.
- **Lark Docx formatting conventions** — underline for key numbers, bold for judgments, `ℹ️` callouts only, inline `<cite>` to source docs instead of footnotes, tables as the workhorse, no hand-drawn SVG.

The full rule set lives in [`SKILL.md`](./SKILL.md) (8 sections + a pre-publish checklist).

## Install

```bash
git clone https://github.com/encircleacity2/bojie-report-style.git \
  ~/.claude/skills/bojie-report-style
```

Then restart Claude Code. It auto-triggers on phrases like:

> write a report · industry solution · sector review · market sizing · report for leadership · *de-AI-flavor this* · *write the English report in my style* · 写汇报 · 行业方案 · 帮我把这份写得不那么 AI 味 · 按我的风格写

## How it works

A "guidance" skill — a single `SKILL.md` with YAML frontmatter (`name`, `description` with trigger words) plus the style rules. No code to run; the agent reads it and applies the conventions while drafting in Lark Docx (via the `lark-doc` skill). It picks the target language first, then layers the matching §8 checklist on top. For long docs it follows a *skeleton → per-section* flow and **delivers chapter by chapter for review** rather than dumping a whole report at once.

## Repo layout

```
bojie-report-style/
├── SKILL.md     # the style guide (frontmatter + 8 sections + checklist)
├── README.md    # this file (EN + 中文)
└── LICENSE      # MIT
```

## Customizing it for yourself

This skill is opinionated toward one person and one domain (BytePlus / ads & e-commerce industry reports). To adapt it:

1. Swap the two **reference docs** in `SKILL.md` for your own best hand-written examples.
2. Edit the **AI-flavor checklists** (both the CN list and the EN list in §8) to match the tells *you* care about.
3. Adjust the **model-division** and **three-pillar value prop** lists to your products.
4. Keep the meta-pattern: *diagnose your own voice from real samples → encode the dos/don'ts → enforce a pre-publish checklist.*

## License

MIT — see [`LICENSE`](./LICENSE).

---
---

# 🇨🇳 中文

一个 [Claude Code](https://claude.com/claude-code) / Claude Agent **skill**，封装了某个人（孙博杰 / Bojie Sun，BytePlus SA）写**行业方案、赛道汇报、专项总结、市场空间分析、给管理层的 report** 的个人文风——典型载体是飞书 Docx，**中文、英文都适用**——让 AI 代写的报告读起来像一个犀利的人类分析师，而不是聊天机器人。

它从 Bojie 的两份亲笔文档（一份专项汇报阶段性总结、一份行业解决方案文档）里提炼而来——起因是 AI 生成的初稿"AI 味"太重（口号、彩色 callout、emoji、自制图表），于是把这份批评固化成了一套可复用的规则。

## 它做什么

触发后，它把写作拉向 Bojie 的口吻，避开常见的 AI 痕迹：

- **分析师口吻，不是市场宣讲口吻** —— 把推理链和测算摊开；保留 hedge（"激进点看""可想象空间按 10% 估"），删掉口号。
- **AI 味自查清单** —— 一批零容忍项：情绪 emoji、彩色 callout、模板化对称、自制 SVG 假图、"来源：《…》"脚注、"向管理层的三个 ask"式包装等。
- **中英双语覆盖（§8）** —— **中文**和**英文**各有一份 AI 味清单。英文那份专门干掉 LLM 套话（*delve, leverage, robust, seamless, unlock, in today's fast-paced world*）、"三个并列形容词"的招牌节奏、em-dash 滥用、"In conclusion"式注水收尾。
- **结构骨架** —— 市场空间拆分表、用**投入象限**（All in / 长期投资 / 探索 / 观察）取代单纯的 P0/P1、KPI 目标拆解并展开"实现路径"。
- **解决方案模板** —— 每个方案以 `市场趋势 → 方案总结 → 卖点（模型 / 生态 / 服务）` 三段开头，点名每个模型干什么（Seed / Seedream / Seedance），分层交付形态（Workflow / Copilot / Agent），并**给真实 demo** 而不是干讲。
- **飞书 Docx 格式约定** —— 下划线标关键数字、加粗标判断句、callout 只用 `ℹ️`、结论处 inline `<cite>` 源文档而非脚注、表格为主力载体、不画自制 SVG。

完整规则见 [`SKILL.md`](./SKILL.md)（8 个章节 + 落笔前检查清单）。

## 安装

```bash
git clone https://github.com/encircleacity2/bojie-report-style.git \
  ~/.claude/skills/bojie-report-style
```

然后重启 Claude Code。它会在以下措辞下自动触发：

> 写汇报 · 行业方案 · 赛道总结 · 专项汇报 · 市场空间 · 给管理层的 report · 帮我把这份写得不那么 AI 味 · 按我的风格写 · *de-AI-flavor this* · *write the English report in my style*

## 工作原理

这是一个"指南型" skill —— 单个 `SKILL.md`，含 YAML frontmatter（`name`、带触发词的 `description`）加风格规则。没有代码要跑；agent 读取它，在用 `lark-doc` skill 起草飞书 Docx 时套用这些约定。它**先判断目标语言**，再叠加对应的 §8 清单。长文档走"骨架 → 分章"流程，**一章一章交付 review**，而不是一口气生成整篇。

## 仓库结构

```
bojie-report-style/
├── SKILL.md     # 风格指南（frontmatter + 8 章 + 检查清单）
├── README.md    # 本文件（英文 + 中文）
└── LICENSE      # MIT
```

## 改成你自己的版本

这个 skill 高度针对一个人和一个领域（BytePlus / 广告与电商行业汇报）。要改成你自己的：

1. 把 `SKILL.md` 里的两份**范本文档**换成你自己最好的亲笔样稿。
2. 改 §8 里的**两份 AI 味清单**（中文那份 + 英文那份），换成*你*在意的痕迹。
3. 调整**模型分工**和**三支柱卖点**清单，对齐你自己的产品。
4. 保留这个元方法：*从真实样稿里诊断自己的文风 → 固化 do/don't → 用落笔前清单强制执行。*

## 许可

MIT —— 见 [`LICENSE`](./LICENSE)。
