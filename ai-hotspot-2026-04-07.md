# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-04-07

---

## 当日爆发项目（新增 star ≥ 1000）

⚠️ 此板块数据来源于 GitHub Trending（WebSearch 抓取，WebFetch 需手动授权）。以下为今日高速增长项目：

| 项目名 | 简介 | 当日新增 star | 总 star 数 | 语言 |
|--------|------|:------------:|:----------:|------|
| [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code) | 史上最快突破 100K star 的 AI Agent Repo，基于 Rust 构建 | 高速增长中 | ~166,800+ | Rust |
| TypeScript 头部仓库（名称待 WebFetch 确认） | TypeScript 热门 AI 工具类项目 | **1,823** | ~23,933 | TypeScript |
| [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | 汇集主流网站设计系统 DESIGN.md 的合集 | 高速增长中 | ~15,700 | — |
| [santifer/career-ops](https://github.com/santifer/career-ops) | 基于 Claude Code 的 AI 求职系统，含 14 种 Skill 模式、Go Dashboard、PDF 生成与批处理 | 高速增长中 | ~3,800 | Go/TypeScript |

> 注：WebFetch 被权限拦截，无法直接读取 github.com/trending 实时页面。如需精确「今日新增 star」数据，请在 Claude Code 设置中授权 WebFetch 后重新运行。

---

## GitHub 热门项目 — AI / Claude / Agent

| 项目名 | 简介 | 亮点 |
|--------|------|------|
| [anthropics/claude-code](https://github.com/anthropics/claude-code) | Anthropic 官方 AI 编程代理，在终端中理解代码库并执行任务 | 已超 82K star；GitHub 原生集成（Public Preview 2026-02-04）；源码因 npm 打包失误于 2026-03-31 意外泄露，成为 HN 热榜 #1 |
| [ultraworkers/claw-code](https://github.com/ultraworkers/claw-code) | Rust 实现的 AI Agent，OpenCode 前身，史上最快破 100K | 从 9K 飙至 21 万+ star，2026 年最大开源爆款 |
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | 社区 1000+ Agent Skills 合集，兼容 Claude Code / Codex / Gemini CLI / Cursor 等 | 官方开发团队贡献，多平台通用 |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Claude Code Skills、Hooks、Slash-Commands、Orchestrators 精选列表 | 社区最全 Claude Code 生态导航 |
| [quemsah/awesome-claude-plugins](https://github.com/quemsah/awesome-claude-plugins) | 用 n8n 工作流自动收集 Claude Code Plugin 在 GitHub 的采用率指标 | 数据驱动的插件生态监控 |
| Vibe Kanban | 跨平台 AI 编程 Agent 可视化看板，支持并行运行 Claude Code / Codex / Amp / Cursor Agent CLI 等 | Claude Code 占有率从 83% 降至 70%，但仍居首位 |
| Claude Squad | 在独立工作区管理多个 Claude Code / Codex / Aider 实例的终端应用 | 多 Agent 并发管理利器 |

---

## GitHub 热门项目 — 视频剪辑自动化

| 项目名 | 简介 | star 数 / 近期增长 |
|--------|------|--------------------|
| [FireRedTeam/FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | AI 视频编辑 Agent，通过自然语言交互、LLM 规划和精准工具编排将手动剪辑转化为意图驱动的导演模式 | 2026-02-10 开源，2026-03-22 新增 ASR 粗剪技能，活跃增长 |
| [HKUDS/ViMax](https://github.com/HKUDS/ViMax) | "Agentic Video Generation"：导演、编剧、制片、视频生成四合一多 Agent 工作流 | 港大出品，端到端视频生成 |
| [RayVentura/ShortGPT](https://github.com/RayVentura/ShortGPT) | YouTube Shorts / TikTok 自动化内容创作框架，用 EML（编辑标记语言）和 JSON 拆解剪辑流程 | LLM 可理解的结构化剪辑管线 |
| [debarch777/AI-Video-Editor](https://github.com/debarch777/AI-Video-Editor) | CLI 工具，将对话视频自动转化为带字幕的社交媒体短视频，全程 LLM 驱动 | Python，零人工干预流水线 |
| [toxtli/AutomEditor](https://github.com/toxtli/AutomEditor) | 基于多模态时空 NG 识别与定位的视频博主 Blooper 自动删除工具，融合人脸、骨骼、情绪、音频特征 | Keras 实现，多特征融合 |

---

## 论坛热门帖子

### Hacker News

- **[The Claude Code Source Leak](https://news.ycombinator.com/item?id=47586778)** — 1,888 points，926 评论，HN 热榜 #1。2026-03-31 安全研究员 Chaofan Shou 发现 Anthropic 在 Claude Code npm 包中意外附带了 `.map` 源码映射文件，完整源码（含注释、内部代号、架构细节）可被任何人读取。
- **[The Claude Code Leak（讨论主帖）](https://news.ycombinator.com/item?id=47609294)** — 后续深度讨论，Alex Kim 博客解析了"假工具"、"沮丧正则"、"隐蔽模式"等内部实现细节。
- **[Claude Code Unpacked: A Visual Guide](https://news.ycombinator.com/item?id=47597085)** — 泄露代码的可视化解析，深度技术帖。
- **[How I'm Productive with Claude Code](https://news.ycombinator.com/item?id=47494890)** — 实战效率技巧分享，高赞社区帖。
- **[Claude Code is all you need](https://news.ycombinator.com/item?id=44864185)** — 观点讨论：Claude Code 作为全能编程伴侣。

### Reddit

- **r/vibecoding**（89K 成员）：热议 Vibe Kanban 数据——Claude Code 从独占 83% 市场降至 70%，仍无对手超过 20%。工具讨论涵盖 Cursor、Lovable、Bolt.new、Emergent。
- **r/ClaudeAI / r/LocalLLaMA**：Claude Code 源码泄露引发安全与架构大讨论，"frustration regexes"（挫败感正则表达式）成为网络梗图素材。

---

## 科技公司最新动态

### Anthropic
- **Claude Code 源码泄露（2026-03-31）**：npm 打包失误导致带注释的完整源码外泄，Anthropic 已确认。源码暴露了内部代号、"隐蔽模式"（undercover mode）及工具系统架构。
- **GitHub 原生集成（2026-02-04）**：Claude 和 Codex 在 GitHub 中以 Public Preview 形式上线。
- **Claude Code 生态**：累计超 82K GitHub Stars；官方 Skills 系统持续扩展，Claude Code 成为 vibe coding 工具事实标准。
- **OAuth 安全加固（2026-01-09）**：针对 OpenCode（原 OpenClaw）等工具伪造 Claude Code HTTP 头、盗用 Pro/Max 订阅 Token 的行为部署服务端防护。

### Cursor（Anysphere）
- **Composer 2 发布（2026-03-19）**：首款由编程工具公司自研的前沿级代码模型，Terminal-Bench 2.0 得分 61.7%，超越 Claude Opus 4.6 的 58.0%；定价仅 $0.50/百万输入 token，约为 Anthropic 旗舰模型的 1/10。
- **商业里程碑**：ARR 突破 $20 亿（2026 年 2 月），正洽谈以 $500 亿估值融资。

### Windsurf（Codeium）
- **三分命运（2025 年 7 月）**：Google DeepMind 以 $24 亿授权交易签约并招募 CEO Varun Mohan 及联合创始人 Douglas Chen；Cognition（Devin 母公司）收购 Windsurf 品牌、产品、IP 及约 210 名员工；OpenAI 最终落空。

### OpenAI
- **Codex 进入 GitHub**（与 Claude 同期，2026-02-04 Public Preview）。
- 因 Windsurf 收购失败，转向自有代码工具生态布局。

### Google
- Google DeepMind 通过 $24 亿 Windsurf 授权交易获得核心编程 AI 人才，强化 Gemini 代码能力布局。

---

## 行业数据

| 指标 | 数据 | 来源 |
|------|------|------|
| Claude Code GitHub Stars | 82,000+ | Augment Code 报告 |
| OpenCode/claw-code GitHub Stars | 210,000+（历史最快破 100K） | WebSearch |
| Vibe Kanban 工具市占：Claude Code | 70%（前值 83%） | Reddit r/vibecoding |
| Cursor ARR | $20 亿（2026-02） | Bloomberg / TechCrunch |
| Cursor 估值（洽谈中） | $500 亿 | Bloomberg |
| r/vibecoding 社区规模 | 89,000 成员 | Reddit |
| HN Claude Code 泄露帖热度 | 1,888 points，926 评论 | Hacker News |

---

## 来源

- [Claude Code GitHub Stars 超 82K — Augment Code](https://www.augmentcode.com/learn/claude-code-github)
- [Claude and Codex 进入 GitHub Public Preview — GitHub Changelog](https://github.blog/changelog/2026-02-04-claude-and-codex-are-now-available-in-public-preview-on-github/)
- [Claude Code 源码泄露分析 — Alex Kim's Blog](https://alex000kim.com/posts/2026-03-31-claude-code-source-leak/)
- [Claude Code 泄露 — The Hacker News](https://thehackernews.com/2026/04/claude-code-tleaked-via-npm-packaging.html)
- [HN: The Claude Code Leak](https://news.ycombinator.com/item?id=47609294)
- [HN: Claude Code Unpacked](https://news.ycombinator.com/item?id=47597085)
- [HN: The Claude Code Source Leak（技术解析）](https://news.ycombinator.com/item?id=47586778)
- [HN: How I'm Productive with Claude Code](https://news.ycombinator.com/item?id=47494890)
- [Claude Code 源码泄露架构分析 — APIdog](https://apidog.com/blog/claude-code-source-leak-analysis/)
- [Cursor Composer 2 发布 — Bloomberg](https://www.bloomberg.com/news/articles/2026-03-19/ai-coding-startup-cursor-plans-new-model-to-rival-anthropic-openai)
- [Cursor Composer 2 性能与定价 — Top AI Product](https://topaiproduct.com/2026/03/19/cursor-composer-2-takes-on-anthropic-and-openai-with-a-0-50-m-token-coding-model-and-the-benchmarks-back-it-up/)
- [OpenAI 选择 Windsurf 而非 Cursor — TechCrunch](https://techcrunch.com/2025/04/22/why-openai-wanted-to-buy-cursor-but-opted-for-the-fast-growing-windsurf/)
- [2026 AI 编程工具战争 — Redreamality](https://redreamality.com/blog/ai-coding-tools-war-vibe-coding-mainstream/)
- [AI Coding Agents 2026 全面对比 — Lushbinary](https://www.lushbinary.com/blog/ai-coding-agents-comparison-cursor-windsurf-claude-copilot-kiro-2026/)
- [Claude Code Reddit 使用调查 — AIToolDiscovery](https://www.aitooldiscovery.com/guides/claude-code-reddit)
- [GitHub Trending](https://github.com/trending)
- [Trendshift](https://trendshift.io)
- [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline)
- [ViMax](https://github.com/HKUDS/ViMax)
- [ShortGPT](https://github.com/RayVentura/ShortGPT)
- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)
- [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code)
- [Beyond Vibe Coding — 2026 AI 编程趋势](https://beyond.addy.ie/2026-trends/)
