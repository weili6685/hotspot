# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-04-04

---

## 当日爆发项目（新增 star ≥ 1000）

> ⚠️ 数据来源：GitHub Trending 页面直接抓取因权限受限，以下数据来自 Trendshift / WebSearch 综合整理（2026 年 4 月累计增长 / 今日估算）。

| 项目名 | 简介 | 当日新增 star（估算） | 总 star 数 | 语言 |
|--------|------|----------------------|------------|------|
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端内 AI 编程代理，理解代码库，自然语言执行任务 | ~2,984 | 94,600+ | TypeScript |
| [everything-claude-code](https://github.com/topics/claude-code) | Agent harness 性能优化系统，4 月累计 +4,973 stars | ~1,500+ | — | TypeScript |
| [OpenScreen](https://github.com/topics/claude-code) | 免费创建精美产品演示，无水印/无订阅，Screen Studio 替代 | ~1,200+ | 11,400 | TypeScript |
| [HKUDS/ViMax](https://github.com/HKUDS/ViMax) | 全流程 AI 视频生成代理（导演/编剧/制片一体化） | ~1,000+ | — | Python |
| [OmX (Oh My codeX)](https://github.com/topics/claude-code) | 为 AI 编程工具添加 hooks、agent teams、HUD 等扩展 | ~1,000+ | 7,700 | TypeScript |

---

## GitHub 热门项目 — AI / Claude / Agent

| 项目名 | 简介 | 亮点 |
|--------|------|------|
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | 终端 AI 编程代理，v1.0 GA，82K+ stars | 4 月增长 13,429 stars，登上 Hacker News #1；源码意外泄露引发全球关注 |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Claude Code skills/hooks/agent orchestrators 精选列表 | 社区驱动，涵盖 slash-commands、插件、应用 |
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | 1,340+ agentic skills，兼容 Claude Code/Cursor/Codex/Gemini CLI | 官方团队 + 社区双轨，2026-04-02 更新，已索引 10,167 个仓库 |
| [quemsah/awesome-claude-plugins](https://github.com/quemsah/awesome-claude-plugins) | 用 n8n 工作流自动采集 Claude Code 插件 GitHub 指标 | 自动化数据追踪，2026-04-02 最新更新 |
| [shareAI-lab/learn-claude-code](https://github.com/shareAI-lab/learn-claude-code) | 从 0 到 1 仿写 Claude Code 的 nano agent harness | "Bash is all you need" 教学项目，适合理解 agent 架构 |
| [superpowers skills framework](https://github.com/VoltAgent/awesome-agent-skills) | Agentic skills 框架 & 软件开发方法论 | 4 月累计 +2,657 stars |

---

## GitHub 热门项目 — 视频剪辑自动化

| 项目名 | 简介 | star 数 / 近期增长 |
|--------|------|-------------------|
| [FireRedTeam/FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | 意图驱动的 AI 视频编辑代理，自然语言交互 + LLM 规划 + 工具编排 | 2026-02-10 开源，快速增长中 |
| [HKUDS/ViMax](https://github.com/HKUDS/ViMax) | 全流程视频生成：剧本→分镜→角色→最终视频，端到端自动化 | 近期爆发，进入 AI 视频生成热门话题 |
| [RayVentura/ShortGPT](https://github.com/RayVentura/ShortGPT) | YouTube Shorts / TikTok 频道自动化框架，含配音/剪辑/素材 | 老牌项目，持续活跃 |
| [debarch777/AI-Video-Editor](https://github.com/debarch777/AI-Video-Editor) | LLM 驱动 CLI，自动转录、分析、渲染短视频，带字幕/音效设计 | 轻量 CLI 工具，适合快速上手 |

---

## 论坛热门帖子

### Hacker News

- [Claude Code Source Leaked via npm Packaging Error](https://thehackernews.com/2026/04/claude-code-tleaked-via-npm-packaging.html) — **1,888 points / 926 comments**，3 月 31 日登顶 HN #1
  - 研究员 Chaofan Shou 发现 Anthropic 在 npm 包中附带了 `.map` 源码文件，完整源码（含注释、内部代号、架构细节）被任何下载者可读
- [The Claude Code Source Leak: fake tools, frustration regexes, undercover mode](https://news.ycombinator.com/item?id=47586778) — Alex Kim 深度分析，揭露内部架构
- [Claude Code Unpacked: A visual guide](https://news.ycombinator.com/item?id=47597085) — 可视化拆解 Claude Code 内部机制
- [Claude Code is all you need](https://news.ycombinator.com/item?id=44864185) — 持续热议的核心帖

### Reddit / Dev 社区

- [Claude Code Just Hit #1 on Hacker News](https://dev.to/max_quimby/claude-code-just-hit-1-on-hacker-news-heres-everything-you-need-to-know-j74) — DEV Community 整理的全面指南
- Vibe Coding "静默杀手"漏洞讨论：自然语言生成代码引入无法被传统工具发现的安全漏洞，正在 Reddit 安全圈引发热议

---

## 科技公司最新动态

### Anthropic
- **Claude Code npm 源码泄露事件**（2026-03-31）：Claude Code npm 包附带 `.map` 文件，导致完整源码外泄，Anthropic 已确认。3 月 31 日 00:21–03:29 UTC 期间更新的版本还包含一个**木马化的 HTTP 客户端**（跨平台远程访问木马），已影响供应链安全。
- **Claude & Codex GitHub 集成**（2026-02-04 GA）：Claude 和 Codex 编程代理进入 GitHub Copilot Pro+ 和 Copilot Enterprise 公开预览。
- **OAuth 封锁行动**（2026-01-09）：Anthropic 部署服务端保护，屏蔽所有伪造 Claude Code HTTP 头的第三方 OAuth 访问（针对 OpenCode 等工具的仿冒行为）。

### Cursor（Anysphere）
- **Composer 2 发布**（2026-03-19）：Anysphere 自研代码专用模型，Terminal-Bench 2.0 得分 61.7%，超越 Claude Opus 4.6（58.0%），价格仅 $0.50/M tokens（Opus 的 1/10）。
- Cursor 年化营收突破 **$20 亿**，成为 AI 编程工具赛道最快增长公司之一。

### Windsurf / Google / OpenAI
- **Windsurf 三分天下**：OpenAI 原计划以 ~$30 亿收购 Windsurf，因与微软 IP 权利冲突告吹：
  - Google DeepMind：$24 亿许可协议 + 招募 CEO Varun Mohan 等核心团队
  - Cognition（Devin 母公司）：收购 Windsurf 的 IP、产品、品牌及 ~210 名员工
  - OpenAI：最终空手而归
- **Google Antigravity**：多代理编排，从第一天起即全面 agentic，与 Claude Code / Codex 形成三足鼎立格局。

### 行业格局
2026 年七大 AI 编程工具：Claude Code、Google Antigravity、OpenAI Codex、Cursor、Kiro、GitHub Copilot、Windsurf，全线向 "agent" 范式演进。

---

## 行业数据

| 指标 | 数据 |
|------|------|
| Claude Code GitHub Stars | 94,600+（4 月增长 13,429） |
| Claude Code npm 泄露窗口 | 2026-03-31 00:21–03:29 UTC |
| Cursor 年化营收 | $20 亿+ |
| Cursor Composer 2 价格 | $0.50/M input tokens |
| Cursor Composer 2 Terminal-Bench 2.0 | 61.7%（Claude Opus 4.6：58.0%） |
| Windsurf Google 许可协议 | $24 亿 |
| awesome-claude-plugins 索引仓库数 | 10,167 个（2026-04-02） |
| VoltAgent awesome-agent-skills | 1,340+ skills |

---

## 来源

- [GitHub Trending](https://github.com/trending)
- [Trendshift](https://trendshift.io/)
- [Claude Code Source Leak — The Hacker News](https://thehackernews.com/2026/04/claude-code-tleaked-via-npm-packaging.html)
- [Claude Code Source Leak Analysis — Alex Kim](https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/)
- [Claude Code Leak — Hacker News](https://news.ycombinator.com/item?id=47609294)
- [Claude Code Unpacked — Hacker News](https://news.ycombinator.com/item?id=47597085)
- [Claude Code is all you need — Hacker News](https://news.ycombinator.com/item?id=44864185)
- [Claude and Codex on GitHub — GitHub Changelog](https://github.blog/changelog/2026-02-04-claude-and-codex-are-now-available-in-public-preview-on-github/)
- [Cursor Composer 2 模型发布 — Bloomberg](https://www.bloomberg.com/news/articles/2026-03-19/ai-coding-startup-cursor-plans-new-model-to-rival-anthropic-openai)
- [Cursor Composer 2 vs Claude — Top AI Product](https://topaiproduct.com/2026/03/19/cursor-composer-2-takes-on-anthropic-and-openai-with-a-0-50-m-token-coding-model-and-the-benchmarks-back-it-up/)
- [OpenAI vs Windsurf 收购 — TechCrunch](https://techcrunch.com/2025/04/22/why-openai-wanted-to-buy-cursor-but-opted-for-the-fast-growing-windsurf/)
- [AI Coding Tools War 2026](https://redreamality.com/blog/ai-coding-tools-war-vibe-coding-mainstream/)
- [FireRed-OpenStoryline — GitHub](https://github.com/FireRedTeam/FireRed-OpenStoryline)
- [ViMax — GitHub](https://github.com/HKUDS/ViMax)
- [ShortGPT — GitHub](https://github.com/RayVentura/ShortGPT)
- [awesome-claude-code — GitHub](https://github.com/hesreallyhim/awesome-claude-code)
- [awesome-agent-skills — GitHub](https://github.com/VoltAgent/awesome-agent-skills)
- [Claude Code完整指南 — ComputeLeap](https://www.computeleap.com/blog/claude-code-complete-guide-2026/)
- [AI Coding Agents 2026 Comparison — Lushbinary](https://lushbinary.com/blog/ai-coding-agents-comparison-cursor-windsurf-claude-copilot-kiro-2026/)
