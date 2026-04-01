# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-04-01

## GitHub 热门项目 — AI / Claude / Agent

| 项目名 | 简介 | 亮点 |
|--------|------|------|
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Anthropic 官方 Claude Code 终端智能编程工具 | 2026-03-31 源码发布至 npm，引发全网热议 |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Claude Code 精选技能、Hooks、插件、Agent 编排器合集 | 含"Codebase to Course"等实用技能，社区活跃 |
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | 1000+ Agent 技能合集，兼容 Codex/Cursor/Gemini CLI | 覆盖多平台，官方与社区双轨并行 |
| [caramaschiHG/awesome-ai-agents-2026](https://github.com/caramaschiHG/awesome-ai-agents-2026) | 2026 年最全 AI Agent 框架与工具列表，300+ 资源 | 每月更新，ByteDance 框架曾登 GitHub Trending #1（25k+ stars）|
| [th3vib3coder/vibe-science](https://github.com/th3vib3coder/vibe-science) | 对抗式 Agent 循环，Claude Code 插件，科研完整性优先 | Falsification-first 研究运行时，vibe coding 方向新星 |
| [FlorianBruniaux/claude-code-ultimate-guide](https://github.com/FlorianBruniaux/claude-code-ultimate-guide) | Claude Code 从入门到高阶使用完整指南 | 含模板、Quiz、Cheatsheet，适合系统学习 |
| [shanraisshan/claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) | Claude Code 最佳实践案例集 | 含 /weather-orchestrator、Agent 团队协作示例 |

## GitHub 热门项目 — 视频剪辑自动化

| 项目名 | 简介 | star 数 / 近期增长 |
|--------|------|-------------------|
| [FireRedTeam/FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | AI 视频剪辑 Agent，自然语言驱动意图式导演模式，LLM 规划 + 工具编排 | 2026-02 正式开源，近期新增 ASR 自动去除口误/重复句功能，增长迅速 |
| [RayVentura/ShortGPT](https://github.com/RayVentura/ShortGPT) | YouTube Shorts / TikTok 自动化实验框架，EditingEngine 基于 Editing Markup Language | 老牌高星项目，持续迭代 |
| [HKUDS/ViMax](https://github.com/HKUDS/ViMax) | 全流程 AI 视频生成 Agent（导演+编剧+制片+生成一体化），输入叙事即输出成片 | 港大出品，2026 年受关注度高 |
| [debarch777/AI-Video-Editor](https://github.com/debarch777/AI-Video-Editor) | LLM 驱动的 CLI 视频自动化工具，转录→分析→渲染字幕+特效一键完成 | 面向 talking-head 短视频，社媒场景适配 |
| [jungdj/AI-Effects](https://github.com/jungdj/AI-Effects) | 自动化 Web 视频编辑工具 | 轻量级，适合快速原型 |

## 论坛热门帖子

### Hacker News

- [Claude Code is all you need](https://news.ycombinator.com/item?id=44864185) — Claude Code 深度使用讨论，556 点，登上 HN #1
- [How I'm Productive with Claude Code](https://news.ycombinator.com/item?id=47494890) — 开发者生产力实战经验分享
- [Tell HN: I'm 60 years old. Claude Code has re-ignited a passion](https://news.ycombinator.com/item?id=47282777) — 60 岁开发者帖子爆红，1058 点 + 300 评论，引发代际共鸣

### DEV Community / Reddit

- [Claude Code's Entire Source Code Just Leaked — 512,000 Lines Exposed](https://dev.to/evan-dong/claude-codes-entire-source-code-just-leaked-512000-lines-exposed-3139) — 2026-03-31 源码泄露事件，揭露未发布功能 `kairos`、`Buddy System`、`Undercover mode`
- [The 60-Year-Old Developer Who Broke Hacker News](https://dev.to/matthewhou/the-60-year-old-developer-who-broke-hacker-news-this-is-what-vibe-coding-actually-looks-like-11l7) — Vibe Coding 真实面貌深度分析
- [Claude Code Just Hit #1 on Hacker News](https://dev.to/max_quimby/claude-code-just-hit-1-on-hacker-news-heres-everything-you-need-to-know-j74) — 事件完整梳理

## 科技公司最新动态

### Anthropic
- **Claude Code 源码意外泄露（2026-03-31）**：将 Claude Code 发布至 npm 时附带了 source map，导致 512,000 行 TypeScript 源码、内部 prompts、Feature Flags 及未发布功能（`kairos` 模式、`Buddy System` 宠物功能、`Undercover` 模式）被还原并公开讨论。

### Cursor（Anysphere）
- **Composer 2 模型发布（2026-03-19）**：首次自研 frontier 级编码模型，Terminal-Bench 2.0 得分 **61.7%**，超越 Claude Opus 4.6（58.0%），价格仅 **$0.50/M tokens**（Opus 的十分之一）。
- 估值谈判中达 **$500 亿**，日活用户突破 **100 万**，企业客户 **5 万家**（含 Stripe、Figma）。

### OpenAI
- 以 **$30 亿** 收购 Windsurf（原 Codeium），战略意图：对抗 Anthropic + Google，巩固企业级 AI 编程赛道地位。
- 此前曾洽谈收购 Cursor，最终转向 Windsurf。

### Google / Windsurf
- Windsurf 被 OpenAI 收购后，AI-native IDE 格局重新洗牌，Google 与 Anthropic 面临更大竞争压力。

### 市场格局
- AI 编码工具战场全面白热化：Claude Code（终端 Agent）vs Cursor Composer 2 vs Codex vs Copilot vs Windsurf，竞争轴从模型能力转向**工作流整合**。

## 行业数据

| 指标 | 数据 |
|------|------|
| Cursor 日活用户 | 100 万+ |
| Cursor 企业客户 | 50,000 家 |
| Cursor 估值（融资谈判） | ~$500 亿 |
| OpenAI 收购 Windsurf 价格 | $30 亿 |
| Composer 2 定价 | $0.50/M input tokens |
| Composer 2 vs Claude Opus 4.6（Terminal-Bench 2.0） | 61.7% vs 58.0% |
| Claude Code 源码泄露规模 | ~512,000 行 TypeScript |
| HN 60岁开发者帖子热度 | 1,058 点，300+ 评论 |

## 来源

- [GitHub - hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code)
- [GitHub - VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)
- [GitHub - caramaschiHG/awesome-ai-agents-2026](https://github.com/caramaschiHG/awesome-ai-agents-2026)
- [GitHub - th3vib3coder/vibe-science](https://github.com/th3vib3coder/vibe-science)
- [GitHub - anthropics/claude-code](https://github.com/anthropics/claude-code)
- [GitHub - FireRedTeam/FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline)
- [GitHub - RayVentura/ShortGPT](https://github.com/RayVentura/ShortGPT)
- [GitHub - HKUDS/ViMax](https://github.com/HKUDS/ViMax)
- [Claude Code is all you need | Hacker News](https://news.ycombinator.com/item?id=44864185)
- [How I'm Productive with Claude Code | Hacker News](https://news.ycombinator.com/item?id=47494890)
- [Tell HN: I'm 60 years old. Claude Code has re-ignited a passion](https://news.ycombinator.com/item?id=47282777)
- [Claude Code Source Leak — DEV Community](https://dev.to/evan-dong/claude-codes-entire-source-code-just-leaked-512000-lines-exposed-3139)
- [Claude Code Reddit Guide 2026](https://www.aitooldiscovery.com/guides/claude-code-reddit)
- [Cursor Composer 2 takes on Anthropic and OpenAI — Bloomberg](https://www.bloomberg.com/news/articles/2026-03-19/ai-coding-startup-cursor-plans-new-model-to-rival-anthropic-openai)
- [Cursor Composer 2 beats Claude at 1/10th price](https://aiforautomation.io/news/2026-03-20-cursor-composer-2-ai-model-beats-claude-tenth-price)
- [OpenAI's $3B Windsurf move — VentureBeat](https://venturebeat.com/ai/openais-3b-windsurf-move-the-real-reason-behind-its-enterprise-ai-agent-code-push)
- [Why OpenAI opted for Windsurf — TechCrunch](https://techcrunch.com/2025/04/22/why-openai-wanted-to-buy-cursor-but-opted-for-the-fast-growing-windsurf/)
- [AI Coding Tools War of 2026 — redreamality](https://redreamality.com/blog/ai-coding-tools-war-vibe-coding-mainstream/)
- [AI Coding Agents Comparison 2026 — Lushbinary](https://www.lushbinary.com/blog/ai-coding-agents-comparison-cursor-windsurf-claude-copilot-kiro-2026/)
