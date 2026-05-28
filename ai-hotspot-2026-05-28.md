# AI 热点 · 2026-05-28
> 你跟一个懂行朋友 20 分钟通话的笔记。

## 🔥 本周一个 hot-take

**主流叙事说 "AI coding tool 七强大战正酣"——Claude Code / Cursor / Windsurf / Codex / Antigravity / Kiro / Copilot 在 IDE 维度死磕价格、上下文、速度、自研模型。我不同意这个画面。**

实情是 Claude Code 已经悄悄离开 IDE 跑道。看一下 Anthropic 过去 9 周往里塞的功能（What's new 原文，每周一篇）：Auto mode（Week 13）→ computer use 进 CLI（Week 14）→ Ultraplan（Week 15）→ Monitor tool 流式背景事件（Week 15）→ Routines 定时跑 cloud agent（Week 16）→ `/ultrareview` 云端 bug 猎手（Week 17）→ `/team-onboarding` 把配置打包成可重放指南 → background sessions + `/goal` 跨 turn 持续工作 → Agent View 一屏看所有 session 状态。

这些不是 "IDE 增强功能"——这是**给你整台机器装一层 agent 控制平面**。Cursor 在比 Composer 推理速度，Windsurf 在比 SWE-1.5 跑得多快，Antigravity 在比 Gemini 3.5 Flash 多便宜——但 Claude Code 已经在比"我能不能后台跑 4 小时、给你整 6 个 PR 出来、自己上 CI"。**这不是同一场比赛**。

我押 6 个月后回看，"七强对比"这类文章会显得很傻——就像 2008 年还在比黑莓和诺基亚的物理键盘。真正的格局会是：Claude Code 当 agent OS，剩下几家继续做 IDE，价格往下卷。这个押注可能错——错的方式是 Anthropic 自己把功能砸太多导致质量崩盘（5/27 v2.1.152 已经在打 startup hang 75 秒的回归 bug，是个早期信号）。但我愿意押。

---

## ✅ 3 件真信号

### 1. Mythos 1 公开预览即将通过 Claude Code 释放

[cybersecuritynews](https://cybersecuritynews.com/claude-mythos-moves-toward-public/) 报道：`claude-mythos-1-preview` 准备通过 Claude Code 和 Claude Security 发布，**在 Claude.com 短暂可见过**——属于 controlled rollout 信号。这跟过去几周 Anthropic 三连发"Using LLMs to Secure Source Code / Zero Trust for AI Agents / CodeRabbit Agent Orchestration"（5/27 同日三篇 [Anthropic blog](https://www.anthropic.com/news)）形成闭环：**Mythos 主打的不是通用对话，是『让 agent 在企业网安场景里跑』**。

跟 30 天前比看变化：4/28 报告里 Mythos 第一次出现是因为它"发现了主流系统大量零日漏洞"——当时是 lab 模式。现在已经走到 "preview release via Claude Code"——这是 Anthropic 把模型分层投放的策略，Opus 4.7 做通用，Mythos 走垂直场景。

**你该改变什么？** 如果你的 SnapStamp 后端（snapstamp-app-service / snapstamp-purchase-service）有任何敏感面（用户数据、支付链路），未来 1-2 个月可以等 Mythos 走出 preview 再决定要不要跑一次安全审计。**不需要现在做**。

### 2. "反 AI 味" 成为独立赛道

5/28 一天，`Leonxlnx/taste-skill`（+2,715⭐，总 24k）和 `hardikpandya/stop-slop`（+664⭐，总 5.7k）双爆发，单日合计 +3,379⭐。它们做的是同一件事：**让 LLM 输出不要那么"AI 味"**——避免那种"As an AI language model" / 过度礼貌 / 模板化 bullet point / 永远在结尾总结的腔调。

这个赛道 30 天前不存在。4/28 报告里完全没有"AI 味去除"主题，那时候社区还在追 Karpathy CLAUDE.md（减少 LLM 编码错误，140k⭐）。一个月时间，**话题从"AI 写代码烂"转到"AI 写文字烂"**——前者是工程问题，后者是语用问题。

为什么是真信号：两个独立项目同日双爆发，不是营销推力，是用户痛点已经积压到某个临界点。Karpathy CLAUDE.md 当时是这个模式（一个文件减少 4 类编码问题，民间共识压不住），现在轮到文字侧。**[The Pragmatic Engineer 2 月调查](https://www.pragmaticengineer.com/)** 显示 46% 工程师把 Claude Code 列为"最爱"，但**这不代表他们爱 Claude 输出的中文/英文文体**。

**你该改变什么？** 你写 SwiftUI、写 hotspot 报告（就这一份）、写 wiki——所有地方都受 AI 味污染。可以下载 taste-skill 装一下试试看，输出会不会更像"人写的"。**这是今天唯一一个值得你 30 分钟实验的项目**。

### 3. Claude Code 进入"OS 阶段"——具体证据

5 月 11–15 的 Week 20 更新（[官方原文](https://code.claude.com/docs/en/whats-new)）一次性塞了：`claude agents` 单屏看所有 session、`/goal` 跨 turn 持续工作、fast mode 默认 Opus 4.7、Rewind 菜单 "Summarize up to here" 压缩 context。Week 19 加了 plugin from `.zip`/URL、auto mode 硬拒规则、hooks 看到 `effort.level`。Week 17 推 `/ultrareview` 云端 bug 猎手。

跟 5/21 报告对比：那天列的是 "Code with Claude 大会发布 agent infrastructure 而非新模型"——当时还是大会预告口吻。一周过去，**这些功能已经落到 v2.1.140+ 实际版本里能用了**。从 announcement 到 shipping 的速度让人不舒服——好的不舒服。

**你该改变什么？** 你的 worktree + subagent + ae-issue-orchestrate 工作流，**可以试试用 `/goal` 替代手动 task 编排**——给 Claude 一个完成条件，让它自己跑直到达标。这跟你的 superpowers:executing-plans 模式互补。**今晚就可以试一次**：挑一个 SnapStamp 里小的 IJP* fix，用 `/goal "fix X and verify build passes"` 看看 Claude 跑几轮收敛。

---

## 🗑️ 3 件噪音

### 噪音 1：SWE-1.5 "比 Sonnet 4.5 快 13×"

Cognition / Windsurf 一直在重复这个数字。它没说**什么任务、什么 batch size、什么硬件、什么 prompt 长度**。13× 速度在 1k token 推理和在 200k context agentic 任务上意义完全不同。任何 benchmark 没有 controlled comparison 都是 marketing。比这更重要的是 Windsurf Teams 涨到 $40/seat——这告诉你 Cognition 在用收购后的定价权"先卖给信徒，等下一代再说"。

### 噪音 2：OpenClaw 373k⭐ / Hermes Agent 12 周 160k⭐

这些是**消费者 AI 助手**——WhatsApp/Telegram/Slack 上的个人 agent。跟你做独立 iOS 开发完全无关。star 数大是因为消费者市场基数大，不代表它们对开发者有任何意义。新闻媒体喜欢报这个数字（"史上最快增长开源项目"），但点开 README 你会发现跟你的工作没有任何 API surface 重合。**忽略**。

### 噪音 3：HN 第 N 次的 "Productivity Panic of 2026"

[HN #47467922](https://news.ycombinator.com/item?id=47467922) 这个帖子已经在 5 月的报告里出现过至少 3 次。每次讨论都是同样的循环：管理层追 AI 生产力 KPI → 工程师承担 review 成本 → 共识"AI 写得快但留下 review 债"。**这个共识 3 月份就稳定了**。继续刷它的人是在用集体焦虑取暖，不是在产生新认知。这周如果你看到 HN 出现这个话题再次冲热，**直接划走**。

---

## 🎯 一个反共识

**主流叙事：GitHub star 增长 = 项目质量信号**。新闻每周报道"OpenClaw 突破 React"、"Hermes 12 周 160k"、"Karpathy CLAUDE.md 一个文件 150k"——把 star 数当做事实裁判。

**我不同意**。star 数现在严重失真，原因是 **AI coding 圈的"集邮文化"**——工程师看到任何带 "claude-code" / "skill" / "agent" 关键词的项目就 star，作为一种"我在跟进前沿"的姿态。50 天 hotspot 历史就是证据：我（这个 skill 自己）反复推荐过 codegraph (40k⭐)、Understand-Anything (40k⭐)、taste-skill (24k⭐)——**没有一个被你实际装上**（grep 测试结果，参考前一轮辩论数据）。

真正的项目质量信号不是 star，是**"被引用进生产工作流的次数"**。obra/superpowers 209k⭐ 看着很猛，但它**真的被嵌进你 80+ skill 体系**——这是 1 次有效采纳。Karpathy CLAUDE.md 140k⭐，你装了 karpathy-guidelines skill——这也是 1 次。剩下 150k+ star 的项目里，0 个被你采纳。

**结论**：star 数衡量的是**注意力流通**，不是**生产力流通**。下次看到"X 项目突破 Y star"标题，先问"这个项目的 production 用户有谁"——如果答不出，那个 star 数就是表演。

---

## 📱 跟 SnapStamp / iOS 工作流的关联

**今天的事里，3 件跟你直接相关，1 件无关。**

直接相关：(1) `taste-skill` 值得今晚装一下试。你的报告/wiki/SwiftUI 注释都有 AI 味污染，这是低风险高回报的实验。(2) Claude Code `/goal` 命令——下次跑 IJP* fix 试着用，看能不能让 ae-issue-orchestrate Phase 3 从"手动派 subagent"变成"指定完成条件让 Claude 自己跑"。(3) Anthropic 5/19 那篇 ["Self-Hosted Sandboxes and MCP Tunnels"](https://www.anthropic.com/news) 不直接影响 SnapStamp，但**如果你之后想做 SnapStamp 后端的 MCP 接入**（让 Claude 通过 MCP 查邮票数据库），这个 sandbox 机制是关键基础设施。

无关：今天 OpenAI 那堆动态（GPT-5.5 Instant 默认、ChatGPT 个人理财、Realtime Voice、Deployment Company）——你不用 ChatGPT 做开发，跟 SnapStamp 邮票识别 / iOS 工作流 0 关联。**不要硬扯**。

---

## 📎 原文引用

⭐ [Anthropic — Claude Mythos prepares public release via Claude Code](https://cybersecuritynews.com/claude-mythos-moves-toward-public/) — 如果只点一个，点这个。它告诉你 Anthropic 模型分层投放战略的具体形态。

- [Claude Code Weekly digest (W13–W20)](https://code.claude.com/docs/en/whats-new) — 过去 9 周功能落地的原文清单，是"agent OS"判断的证据基础。
- [GitHub Trending Daily](https://github.com/trending?since=daily) — 自己刷一遍验证 taste-skill / stop-slop 的爆发是不是真的。
- [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) — 装这个，今晚 30 分钟实验。
- [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) — taste-skill 同主题对照组。
- [Anthropic 5/27 三连发 — Source Code Security / Zero Trust / CodeRabbit](https://www.anthropic.com/news) — Mythos 战略的背景叙事。
