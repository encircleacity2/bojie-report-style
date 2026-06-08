---
name: bojie-report-style
version: 1.1.0
description: "Bojie-style industry / strategy / leadership report writing guide, bilingual Chinese and English. Use when drafting or rewriting market sizing, sector reports, strategy memos, customer progress, solution docs, management reports, or when asked to match Bojie's style / reduce AI flavor / de-AI-flavor writing. Enforces analyst tone, explicit assumptions, cited numbers, direct judgment, sparse neutral formatting, and sentence-level de-AI rewrites. 触发词：写汇报、行业方案、赛道总结、专项汇报、市场空间、管理层 report、按我的风格写、去 AI 味。"
---

# 白皮笔法 — Bojie 的行业汇报写作风格

为 Bojie（孙博杰 / Bojie Sun，BytePlus SA）撰写或改写面向公司 leader / 管理层的**行业方案、赛道汇报、专项总结、市场空间分析、解决方案文档**时，遵循本指南。目标只有一个：**写出来像 Bojie 自己写的——分析师口吻、信息密度高、判断敢下、没有 AI 味。**

> **中英双语 / Bilingual.** 本指南同时适用于**中文**和**英文**报告（Bojie 的解决方案文档常是英文，专项汇报常是中文）。§一 ~ §七 的方法论、结构、卖点框架两种语言通用；语言专属的 AI 味自查见 **§八 语言专属规则**。改写时先判断目标语言，再叠加对应 §八 的清单。
> This guide applies to BOTH Chinese and English reports. The methodology, structure and value-prop frames in §1–§7 are language-agnostic; language-specific "AI-flavor" tells live in **§8**.

---

## 一、最高准则（一句话）

> 分析师口吻、判断敢下、测算摊开、数字挂源文档 cite；强调用**下划线 + 加粗**；callout 只用 `ℹ️` 承载结构化小结；方案走"**趋势 → 方案 → 卖点（模型/生态/服务）**"三段 + 真实 demo；删掉所有情绪 emoji 和自制 SVG 假图。

---

## 二、AI 味自查清单（写完逐条过，命中就改）

这些是最容易暴露"机器代笔"的特征，**零容忍**：

- ❌ **情绪化口号**："拐点红利""战略窗口""最确定路径""确立领先身位""吃下这波红利""杠杆"——全删，只留"数字 + 判断"。
- ❌ **情绪 emoji**：🚀🎯🥊⭐🏁🔥 等装饰性 emoji。**只允许** `ℹ️`（小结）和 `1️⃣2️⃣3️⃣`（并列项编号）。
- ❌ **彩色 callout 堆砌**：每节都套 `background-color` 彩框。callout 要稀疏、中性、结构化。
- ❌ **模板化对称**：每节都"callout→表→图→来源"一个模子。结构要跟着内容走，允许不对称。
- ❌ **自制 SVG 柱状图/示意图**：一眼 AI 生成。改用真实截图 / demo 视频 / 源文档 cite，或留空待 Bojie 补图。
- ❌ **"来源：内部《xxx》"脚注**：改成在结论处直接 inline `<cite doc-id="...">`。
- ❌ **"一句话结论 / 一句话收尾 / 向管理层的三个 ask"** 这类宣讲式包装：去掉，落到清单或下一步。
- ❌ **替读者把话说满**：少用"显著""极大""完美覆盖"。该 hedge 就 hedge（"6 月激进点看一下""可想象空间按 10% 估"）。
- ❌ **笼统说"全家桶/一站式"**：必须点名每个模型干什么（见 §五）。
- ❌ **抽象价值词堆叠**："赋能""助力""打造""构建""释放价值""形成闭环""全链路覆盖"——默认删，除非后面紧跟具体对象、数字、流程边界。
- ❌ **万能背景段**："随着行业快速发展 / 在数字化浪潮下 / 面对复杂市场环境"——直接切到事实、客户动作、预算变化或产品卡点。
- ❌ **过度完整的自洽感**：每段都像标准答案、没有口径/边界/待确认项，也会像 AI。保留真实研究过程中的假设、缺口和下一步验证。

---

## 三、Bojie 的语气（DO）

1. **分析师口吻，把推理链摊开**。不仅给结论，给"怎么算的 / 假设是什么 / 为什么这么判断"。
   - 例："假设 9 家平均渗透率 5%，DRR + 18k""从全球广告支出 1 万亿、素材制作占 10% 来看，当前 TAM 占比仅 0.25%"。
2. **保留不确定性与 hedge**。"激进点看""保守预期""可想象空间按 X 估""进展中""持续观察"。
3. **判断敢下**。该拍的判断直接拍："时尚/美妆/家装是 3 个最关键品类""付费媒体从战役中剔除""GEO 取代 SEO"。
4. **中英自然混用**，不强行翻译：DRR、TAM、MoM、variant、DCO、FDE、R2V、pack shot、GMV、CTR、LTV、SKU、ISV、GEO/SEO 直接用。
5. **引号包装有信息量的记忆点**（不是口号）：「管线里的一个渲染节点」vs「agency 的端到端生产工具」、"从内容交付走向效果交付"、"创意在我，执行在 AI"、"算法利润"。
6. **数字精确且带口径**：720p/5s 归一、$0.73/条、日均 X 条/天、MoM +54%、渗透率 X%。每个大数字后面跟"怎么测的"。
7. **研究过程感可以保留**。允许写"先按 X% 粗估""这个数还要和源表对齐""暂不把 paid media 算进去""Q3 需要用真实转化回收一次"。这类边界比完美口号更像真人汇报。

### 3.1 句子级去 AI 味动作

命中 AI 味时，不要只删词，要把句子改成可验证的业务判断：

- **抽象名词 → 具体对象**：不要只写"能力建设 / 业务赋能 / 生态协同"，改成"哪个客户、哪个流程、哪个模型、哪个指标"。
- **形容词 → 数字口径**：不要写"显著提升 / 大幅降低"，改成"CTR +X%、成本降到 $X/条、日均 X 条、渗透率 X%"。
- **宏大判断 → 假设链**：不要写"市场空间巨大"，改成"TAM = 客户数 × 使用频次 × 单价，先按保守渗透率 X% 算"。
- **闭环叙事 → 边界条件**：写清"当前能做什么 / 暂不做什么 / 依赖什么前提"，不要用"端到端闭环"糊过去。
- **顺滑连接词 → 直接推进**：少用"首先/其次/此外/最终/综上"。每段只保留一个主判断，下一句接数字、原因或动作。

### 3.2 Before / After 参考

**中文**

AI 味：
> 该方案可以赋能客户构建从内容生产到投放优化的全链路闭环，持续释放业务价值。

Bojie 味：
> 这件事先不要写成"全链路"。当前能打的是 <u>高频素材生产</u>：先把主图、短视频、variant 三类素材的单条成本和产能算清楚；投放优化是否纳入，取决于客户有没有稳定的反馈数据。

AI 味：
> 随着市场需求持续增长，该赛道已经进入关键窗口期。

Bojie 味：
> 需求不是泛增长，主要来自两类预算迁移：一是原外包制作费，二是原广告平台内置工具预算。先按 10 家头部客户、5% 渗透率估，26 年可看 $XM；这个数还要用客户外采量回收一次。

**English**

AI-flavored:
> The solution empowers brands to unlock a seamless end-to-end workflow from ideation to execution.

Bojie-style:
> Do not call this end-to-end yet. The first wedge is high-frequency asset production: image variants, short clips, and localized copy. Media optimization is out of scope until the customer can send stable feedback data.

AI-flavored:
> This presents a unique opportunity to transform the industry landscape.

Bojie-style:
> The opportunity is narrower and more measurable: replace the repeatable production spend first. If 20 target accounts move 5% of external creative spend onto the workflow, the near-term revenue pool is roughly $XM.

---

## 四、结构骨架

### 4.1 章节层级
- 标题**朴素、不标题党**："26 年市场空间""当前主要的卡点和问题"——不要"为什么是现在""谁动了我的奶酪"这种。
- **汇报/总结类**（节奏快、给结论）：扁平 `h3` 平铺即可，参照 v0.5 范本。
- **成品方案类**（讲透一个场景）：可下钻到 `h3/h4`（场景 → 场景需求 → demo → 方案设计），参照电商范本第 2 章。

### 4.2 行业方案/汇报的常用章节序（按需裁剪，不必全有）
1. **市场空间** — 客群拆分表（客群/典型客户/年度外采量/日均/支出/优先级分析）+ 总盘汇总 + 测算口径
2. **竞争格局与我们的位置** — 友商分模型营收/占比表 + 我方"在哪"的判断
3. **客群目标拆解和实现路径** — 核心 KPI（如 DRR/MRR）+ 分阶段目标 + 每个目标的"实现路径"展开
4. **标杆客户进展** — 进展数字 + 里程碑 + 卡点
5. **当前主要卡点和问题** — 表格：类别(P0/P1) / 问题描述 / 参考文档 / Owner(@人) / 需求
6. **方案 / 弹药库** — 客群画像 × 方案材料矩阵，每条挂源文档 cite

### 4.3 投入象限（给优先级的更好方式）
不要只标 P0/P1。对场景或客群套**带门槛的投入姿态四象限**：
- **All in**：长期 TAM 大（如 30 年 >5 亿美金）且近期收入目标可达（如 26 年 >10M）
- **长期投资**：长期 TAM 大、但近期收入目标中等（市场/产品 ready 度原因）
- **探索**：当前定义/TAM 不清晰但想象空间大，保持小投入探索
- **观察**：长期与近期都不高，持续观察市场变量
门槛数字要写明，让管理层一眼看懂"为什么放这个象限"。

### 4.4 段落节奏

优先用这三种节奏，避免宣传稿式铺垫：

1. **判断 → 数字 → 口径 → 下一步**
2. **现象 → 为什么重要 → 我们的位置**
3. **客户/场景 → 当前卡点 → 可切入点**

避免："行业背景 → 趋势判断 → 价值升华 → 总结展望"。这套节奏太像通用白皮书。

---

## 五、解决方案怎么写（三段抬头 + 三支柱卖点）

每个方案/场景开头用一个 `ℹ️` callout，固定三段：

```
ℹ️
- 市场趋势：<这个赛道正在发生什么变化>
- 方案总结：<我们做什么，一句有判断的话，如"从内容交付走向效果交付">
- BytePlus 卖点总结：
  1. 模型：<具体到模型与角色，见下>
  2. 生态：<TikTok Shop / 抖音 TT 电商 / FDE 等独有生态>
  3. 方案与服务：<行业最佳实践 + FDE 技术交付 + agentic 升级>
```

**点名模型分工**（不要说"全家桶"）：
- **Seed-1.6 / Seed 2.0 (LLM·VLM)**：深度理解、脚本、Reflection 视觉巡检纠错、agent 编排
- **Seedream-4.5 / 5.0 (图像)**：4K 原生超高清、多参考图特征一致性、品牌视觉规范
- **Seedance (视频)**：专业级高连贯广告视频、单次多镜头成片、同步音
- 按实际方案选用并写清"谁负责哪一段"。

**作业模式分层**（描述交付形态时套用）：
- **Workflow（模板）**：海量 SKU 一键大规模覆盖，替代人工降基础成本
- **Copilot（边聊边创作）**：品牌精品/社交内容，交互式微调（"创意在我，执行在 AI"）
- **Agent（自主闭环）**：全托管效果广告，按反馈 24/7 自动重绘优化（"算法利润"）

**给看的东西**：方案章节要嵌**真实 demo**——一方 demo 链接 + 三方 ISV 案例 + 样例视频/截图，或引用 First Pitch / 案例文档 cite。不要用文字干讲，更不要拿自制 SVG 充数。

---

## 六、飞书 Docx 格式约定（lark-doc XML）

配合 `lark-doc` skill 写入，遵循以下约定（详见 lark-doc 的 `lark-doc-xml.md`）：

| 用途 | 怎么写 | 不要 |
|---|---|---|
| 强调关键数字/结论 | `<u>下划线</u>` | 彩色 `<span text-color>` |
| 强调判断句 | `<b>加粗</b>` | emoji 前缀 |
| 结构化小结 | `<callout emoji="ℹ️">` 三段式 | 🚀🎯 彩框 |
| 并列项编号 | `1️⃣2️⃣3️⃣` 或 `<callout emoji="ℹ️">` | — |
| 数据载体 | `<table>`（多列：客群/数据/优先级分析） | 散落的 `<p>` 堆叠 |
| 引用来源 | 结论处 inline `<cite doc-id="..." file-type="..." title="...">` | "来源：《xxx》"脚注 |
| @负责人 | `<cite type="user" user-id="ou_...">` | 纯文本人名 |
| 图文并排 | `<grid><column>` 文字 + `<img>`/`<figure>` | 自制 `<whiteboard type="svg">` 假图 |
| 真实图表/画板 | 引用已有 `<whiteboard token>` 或截图 `<img>` | 现编 SVG 柱状/示意图 |

- **作者署名永远是 Bojie / Bojie Sun**。源材料里的其他人名（如 @刘一）按 Owner 原样保留；**王文杰不是 Bojie，不要把他当作者或与 Bojie 混淆**。
- 写长文档用 lark-doc 的"骨架 → 分章 block_replace/append"工作流，**不要一次性塞超长 `--content`**。

---

## 七、工作方式（很重要）

- **一章一章写，每章交给 Bojie review 再继续**——不要一口气生成整篇。
- 写之前**先读 1-2 份范本文档**对齐当下语气，再动笔。
- 新汇报**新建干净文档**，不覆盖既有的 v0.5 等原稿（除非明确要求）。
- 改写已有 AI 味文档时，先按 §二 自查清单逐条诊断、列出"病根对照表"给 Bojie 看，再改。
- 公开 research **嵌进论点做佐证**（"外部锚点：Publicis CoreAI €300M…"一句带过），不单独堆成一节。

---

## 八、语言专属规则（中文 / English）

方法论通用，但**两种语言的 AI 味长得不一样**。先定目标语言，再叠加对应清单。

### 8.1 中文报告
- 已在 §二 / §三 覆盖：去口号、去情绪 emoji、下划线标数字、判断敢下、hedge 保留。
- 中英术语自然混排（DRR/TAM/variant/GMV…），**不要**把所有英文硬翻成中文（"漏斗"可以，但"渗透率""归因"别翻成生造词）。
- 句子短、断句利落，少用"首先/其次/此外/综上所述"这种连接词套壳。
- **中文高危词默认删除**：赋能、助力、打造、构建、沉淀、抓手、底座、体系化、全链路、全场景、深度融合、持续深化、价值释放、降本增效、提质增效、业务增长新引擎、打开想象空间、形成飞轮。
- 这些词不是绝对禁用，但只有在后面能接具体对象、口径数字或明确 owner 时才保留。例如不要写"打造增长飞轮"，改成"用复购率、素材产能、获客成本三项指标看是否形成正循环"。

### 8.2 English reports — extra AI-tell checklist
英文里最暴露 AI 的，是用词和句式套路。**英文报告额外删除：**
- ❌ **LLM filler verbs/adjectives**: *delve, leverage, robust, seamless, cutting-edge, game-changer, unlock, harness, supercharge, elevate, empower, streamline, navigate the landscape, in today's fast-paced world, it's worth noting, it's important to note*.
- ❌ **Hedging-as-padding**: *arguably, fundamentally, essentially, ultimately* 当连接词刷存在感。
- ❌ **Triadic rhythm tic**: 凡事三个并列形容词（"fast, scalable, and reliable"）——AI 的招牌节奏，砍成一个准确的词。
- ❌ **Em-dash overuse** 和每段都 bold 一个 lead-in。
- ❌ **Conclusion bloat**: *In conclusion / Overall / To summarize* 开头的收尾段。
- ❌ **AI sentence frames**: *As brands increasingly look to...*, *This presents a unique opportunity to...*, *By leveraging X...*, *Not only does X..., but it also...*, *From ideation to execution...*, *a comprehensive suite of capabilities...*.
- ✅ **DO**: 短句、主动语态、具体动词、数字带口径；判断直接下（"Paid media is out of scope — platforms self-produce 88–96%"）；保留 analyst hedge（"call it ~10% long-term", "aggressively, 40%→60%"）；术语全篇一致。
- ✅ **强调方式**：英文里同样优先 `<u>` 标关键数字、`<b>` 标判断句；引号包装 memorable framing（"a render node in the pipeline" vs "an end-to-end production tool"）。

### 8.3 中英对照版文档
若一份文档要中英双语（如对客 pitch + 内部汇报），**先写定一种语言定稿，再翻另一种**——不要逐句直译，按目标语言的 §8.1/§8.2 重写句式，保证两版各自读起来都像母语分析师写的、数字与 cite 完全一致。

---

## 九、落笔前 10 秒检查

1. 有没有情绪 emoji / 口号？→ 删
2. 关键数字有没有带测算口径？→ 补
3. 结论有没有挂源文档 cite？→ 挂
4. 有没有自制 SVG 假图？→ 换真实素材或留空
5. 方案有没有点名模型分工、给 demo？→ 补
6. 语气像不像"分析师在摊牌推理"而非"市场在宣讲"？→ 调
7. 每个大判断有没有数字、客户、模型、cite 或显式假设之一？→ 没有就补证据或降级为待验证
8. 有没有"闭环 / 全链路 / 赋能 / seamless / unlock"这类抽象词？→ 换成对象、边界和动作
9. 段落是不是太整齐、太满、太像标准答案？→ 加入口径、例外、待确认项
10. 如果删掉所有形容词，核心判断还成立吗？→ 不成立就重写
