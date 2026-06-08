# bojie-report-style 「白皮笔法」

> A personal writing-style skill for **industry strategy reports & leadership reporting** — captures Bojie's analyst voice so AI-drafted reports stop reading like AI.

A [Claude Code](https://claude.com/claude-code) / Claude Agent **skill** that encodes one person's (Bojie Sun, BytePlus SA) house style for writing and rewriting **行业方案 / 赛道汇报 / 专项总结 / 市场空间分析 / 解决方案文档** — typically Lark (Feishu) Docx — so the output sounds like a sharp human analyst, not a chatbot.

It was distilled from two of Bojie's own hand-written documents (a staged campaign summary and an industry solution doc), after an AI-generated first draft came back too "AI-flavored" (玩具感口号、彩色 callout、emoji、自制图表). The skill turns that critique into a reusable rule set.

---

## What it does

When triggered, it steers the writing toward Bojie's voice and away from common LLM tells:

- **Analyst voice, not marketing voice** — show the reasoning chain and the math; keep the hedges (“激进点看”, “保守预期”), drop the slogans (“拐点红利”, “战略窗口”).
- **An anti-"AI-flavor" checklist** — 9 zero-tolerance tells to strip: emotional emoji, rainbow callouts, templated symmetry, fake auto-generated SVG charts, "来源：《…》" footnotes, "向管理层的三个 ask" packaging, etc.
- **Structural skeletons** — market-sizing tables, an *investment-quadrant* prioritization frame (All-in / Long-term / Explore / Watch) instead of bare P0/P1, KPI target-decomposition with explicit "实现路径".
- **A solution-writing template** — every solution opens with `市场趋势 → 方案总结 → 卖点(模型/生态/服务)`, names each model's job (Seed / Seedream / Seedance), layers delivery modes (Workflow / Copilot / Agent), and **shows real demos** instead of describing them.
- **Lark Docx formatting conventions** — underline for key numbers, bold for judgments, `ℹ️` callouts only, inline `<cite>` to source docs instead of footnotes, tables as the workhorse, no hand-drawn SVG.

The full rule set lives in [`SKILL.md`](./SKILL.md).

---

## Install

Clone into your Claude skills directory:

```bash
git clone https://github.com/encircleacity2/bojie-report-style.git \
  ~/.claude/skills/bojie-report-style
```

Then restart Claude Code so the skill is picked up. It will auto-trigger on phrases like:

> 写汇报 · 行业方案 · 赛道总结 · 专项汇报 · 市场空间 · 给管理层的 report · 帮我把这份写得不那么 AI 味 · 按我的风格写

---

## How it works

This is a "guidance" skill — a single `SKILL.md` with YAML frontmatter (`name`, `description` with trigger words) plus the style rules. There's no code to run; the agent reads it and applies the conventions while drafting in Lark Docx (via the `lark-doc` skill). For long docs it follows a *skeleton → per-section* writing flow and **delivers chapter by chapter for review** rather than dumping a whole report at once.

---

## Repo layout

```
bojie-report-style/
├── SKILL.md     # the style guide (frontmatter + 8 sections)
└── README.md    # this file
```

---

## Customizing it for yourself

This skill is opinionated toward one person and one domain (BytePlus / ads & e-commerce industry reports). To adapt it:

1. Swap the two **reference docs** in `SKILL.md` §intro for your own best hand-written examples.
2. Edit the **AI-flavor checklist** (§二) to match the tells *you* care about.
3. Adjust the **model-division** and **三支柱卖点** lists to your products.
4. Keep the meta-pattern: *diagnose your own voice from real samples → encode the dos/don'ts → enforce a pre-publish checklist.*

---

## License

MIT — see [`LICENSE`](./LICENSE).
