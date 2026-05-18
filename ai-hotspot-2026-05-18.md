# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-05-18

## 🌊 今日大势
Claude 阵营在 5 月密集出招：**Code w/ Claude SF 2026** 大会刚收官，**Agent view in Claude Code** 上线，**Claude Platform on AWS** 完成原生上云，企业线 PwC / 法律行业垂直化全面铺开。同时 Anthropic 宣布 6/15 起对外部 agent 工具用量启用独立计费池，**生态从"塞进 Claude Code"转向"独立 agent SDK 计费"**——OpenAI 借机在 token 定价上挖人。GitHub 当日只有 `tinyhumansai/openhuman`（+1690 ⭐，Rust 本地化 AI）单项目突破千星，主旋律明显从"框架/SDK 爆款"切到了"垂直 agent 团队（六 agent / scientific-agent / cli-anything）"。

## ⭐ Claude 官方信号（最近 7 天 claude.com/blog）

| 标题 | 日期 | 分类 | 为什么重要 |
|---|---|---|---|
| Deploying Claude across the legal industry | 2026-05-15 | Enterprise AI | 法律垂直成为继金融后第二个"模板包"产品线，对应同期 12 个新 plugin |
| The founder's playbook: Building an AI-native startup | 2026-05-14 | Claude Code | 把 Claude Code 定位成"从 0 到 1 的起步底座"，直击 vibe coder 受众 |
| How Claude Code works in large codebases | 2026-05-14 | Enterprise AI | 终于补齐"大 codebase 怎么用"的官方答疑，对你 SnapStamp 之后扩展有参考 |
| Best practices for computer and browser use with Claude | 2026-05-13 | Agents | computer use / browser use 重新被官方系统化，Mac/iPhone agent 落地有依据 |
| Code w/ Claude SF 2026 recap | 2026-05-12 | Product announcements | 一次性梳理本季所有新东西（Plugin Marketplace、Agent View、AWS、1M context） |
| Claude for the legal industry | 2026-05-12 | Product announcements | 第一个明确按"行业"打包发布的 product，验证"垂直 + 工作流"路线 |
| How Anthropic's cybersecurity team built a threat detection platform with Claude Code | 2026-05-12 | Claude Code | 自家 dogfood，演示"Claude Code = production app builder" |
| Agent view in Claude Code | 2026-05-11 | Product announcements | 终于把多 agent 状态可视化做进 IDE — vibe coder 单兵指挥多 agent 的拐点 |
| Introducing the Claude Platform on AWS | 2026-05-11 | Product announcements | AWS 原生集成 = 企业采购阻力进一步降低 |

## 📌 今日推荐阅读（基于 iOS / SwiftUI / vibe coding 视角）

1. **[Best practices for computer and browser use with Claude](https://claude.com/blog)** — 你 ae-mobile-agent / ae-desktop-agent 两个 skill 的官方理论支撑，更新一次"为什么这么做"的依据。
2. **[How Claude Code works in large codebases](https://claude.com/blog)** — SnapStamp 已经接近"超出短 prompt 一次性 hold 住"的体量，是该把 Anthropic 给的 large-codebase pattern 对照一下自己工作流的时候。
3. **[Agent view in Claude Code](https://claude.com/blog)** — Work Chain 在 iOS 项目里你已经在用"链式 agent"思维了，Agent View 上线意味着可以在 IDE 里直接看到链路状态，下次开 BC* skill chain 调试时值得试。

## 📈 当日 GitHub 爆发项目（主题相关，新增 star ≥ 1000）

| 项目名 | 简介 | 当日新增 | 总 star | 信号 |
|---|---|---|---|---|
| [tinyhumansai/openhuman](https://github.com/tinyhumansai/openhuman) | "Your Personal AI super intelligence. Private, Simple and extremely powerful."（Rust 本地化 AI 助手） | +1,690 | 13.2k | 📈📌 本地化 / 私有 AI 路线再起，关注 Apple Intelligence 对位 |

> 今日只有 1 个主题相关项目越过千星阈值，但下面的次档（500-1000）信号其实更值得看：

| 项目名 | 简介 | 当日新增 | 信号 |
|---|---|---|---|
| [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 代码图谱 / 大代码库导航工具 | +857 | ⭐ 与官方 large-codebase blog 同周爆发，呼应趋势 |
| [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | 科研领域 agent skill 集 | +762 | ⭐ "skill ≠ prompt" 的生态外溢，验证 Anthropic skill 协议外化 |
| [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI) | 开源 GenAI 工具合集 | +703 | 📌 |
| [calcom/cal.diy](https://github.com/calcom/cal.diy) | Cal.com 出的 DIY 自托管套件 | +433 | ⭐ Cal 团队第一次玩 vibe-coding 友好版本 |
| [microsoft/ai-agents-for-beginners](https://github.com/microsoft/ai-agents-for-beginners) | MS 出的 agent 入门 Notebook 集 | +485 | 微软 agent 教育线在持续推 |
| [HKUDS/CLI-Anything](https://github.com/HKUDS/CLI-Anything) | HKUDS 系新作：把任意 CLI 包成 agent tool | +238 | HKUDS 系出品（同系列还有 VideoAgent、ViMax） |

### 其他爆发项目（非主题）
- [oven-sh/bun](https://github.com/oven-sh/bun) (+910 ⭐): JS runtime / bundler，基础设施类
- [521xueweihan/HelloGitHub](https://github.com/521xueweihan/HelloGitHub) (+191 ⭐): 中文区入门项目精选

## GitHub 热门项目 — Agent 驱动 UI/UX 设计

| 项目名 | 简介 | 亮点 |
|---|---|---|
| [ag-ui-protocol/ag-ui](https://github.com/ag-ui-protocol/ag-ui) | AG-UI: Agent-User Interaction Protocol | 想给 agent <-> 前端做"MCP for UI"的标准事件协议，注意是协议级 |
| [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) | DESIGN.md 文件集合，丢给 coding agent 生成匹配 UI | "Design as context file" 模式，呼应你 ae-ui-mockup 思路 |
| [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | 一个 AI skill：跨平台专业 UI/UX 设计智能 | 直接以 Anthropic skill 形态发布，可参考结构 |
| [barbarosselimbuyukelci/mobile-ai-ui-ux-revamp-skill](https://github.com/barbarosselimbuyukelci/mobile-ai-ui-ux-revamp-skill) | 移动 UI/UX 改版 skill：codebase intent 推断 + 设计系统映射 + CI 校验 | 工作流和你 ae-verify-app + ae-ui-mockup 链路很像，值得对照 |
| [veluthoor/ui-ux-design-review-agent](https://github.com/veluthoor/ui-ux-design-review-agent) | 用 Gemini 2.0 review AI 生成 UI 的小工具 | "vibe 生成的 UI 看起来 meh"是普遍痛点，正是 pm-review skill 解决的事 |
| [RedHat-UX/next-gen-ui-agent](https://github.com/RedHat-UX/next-gen-ui-agent) | 根据 prompt + 后端数据动态生成富 UI 组件 | RedHat 进场，企业 UI 自动化的官方信号 |

## GitHub 热门项目 — 自动化测试 / AI Test Gen

| 项目名 | 简介 | 亮点 |
|---|---|---|
| [confident-ai/deepeval](https://github.com/confident-ai/deepeval) | LLM Evaluation Framework | 让 coding agent 自己生成 dataset + 写 eval + 跑测 + 迭代失败 metric，闭环 |
| [Kumari-Pragati/Intelligent-Test-Automation](https://github.com/Kumari-Pragati/Intelligent-Test-Automation) | 多 agent LLM 框架：动态测试用例生成 + 验证 | 一个 agent 写 case、一个 agent validate、一个 execute 的分工范式 |
| [furudo-erika/ai-testing-agent](https://github.com/furudo-erika/ai-testing-agent) | 开源 AI Testing Agent，针对 API 自动生成测试计划和代码 | 支持自然语言反馈迭代改测试，适合 API-first 项目 |
| [mindfiredigital/AUTOTEST](https://github.com/mindfiredigital/AUTOTEST) | LLM 动态分析网页 → 生成 Selenium 脚本 | Web 端自动化测试 / E2E 试点参考 |
| [githubnext/testpilot](https://github.com/githubnext/testpilot) | GitHub Next 出的 npm 包单测自动生成 | 官方实验，"signature + 文档示例"路线值得借鉴 |
| [herchila/unittest-ai-agent](https://github.com/herchila/unittest-ai-agent) | GPT-4o 写单测 | 最简版参考实现 |

## GitHub 热门项目 — 视频剪辑自动化

| 项目名 | 简介 | 亮点 |
|---|---|---|
| [HKUDS/VideoAgent](https://github.com/HKUDS/VideoAgent) | 全栈视频理解 / 编辑 / 重制 agent | 图驱动 workflow + 自适应反馈环 |
| [HKUDS/ViMax](https://github.com/HKUDS/ViMax) | 一体化视频生产：导演 / 编剧 / 制片 / 生成 | 把视频生产 pipeline 多 agent 化 |
| [FireRedTeam/FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | "意图驱动导演"式 AI 剪辑 agent | 4 月新增 AI 转场自动生成；Style Skills 可复用 |
| [aregrid/frame](https://github.com/aregrid/frame) | 开源 vibe 视频编辑器 | Cursor-like 交互定位"剪辑界的 vibe coding" |
| [video-db/Director](https://github.com/video-db/Director) | 多 agent 视频框架：摘要 / 编辑 / 搜索 | 适合做内容平台底座 |

## ⚠️ 用户痛点 / 负面信号

- **Anthropic 6/15 计费分离 / 用量收紧**：从 5/14 起，Claude 订阅对外部 agent 工具用量启用独立 credit meter。Axios 同日报道：Anthropic 主动收紧 Claude 限额，OpenAI 反过来用 token 定价拉客 — _agent 经济学开始挤压重度用户_。([Axios](https://www.axios.com/2026/05/14/anthropic-claude-price-openai-tokens), [Apiyi 解读](https://help.apiyi.com/en/anthropic-claude-subscription-agent-sdk-billing-split-june-2026-en.html))
- **HN: "Claude Code 与 2026 的生产力恐慌"** — 真实痛点是"vibe coding 看起来 work，细看 TUI 渲染只渲了前 20 字符"。下一个 feature 出不来是因为你在调上一个 feature 没人发现的渲染 bug。([HN #47467922](https://news.ycombinator.com/item?id=47467922))
- **Claude Code 源码 npm 泄漏事件后续讨论**：业界讨论"fake tools / frustration regex / undercover mode"暴露的工程文化与边界。([The Hacker News](https://thehackernews.com/2026/04/claude-code-tleaked-via-npm-packaging.html))

## 论坛热门帖子（正向）

- **[From Vibe Coding to a Six-Agent Claude Code Team](https://www.decodingai.com/p/squid-my-agentic-coding-setup-may-2026)** — 详细 dogfood 一份"六 agent 团队"配置（May 2026）。值得对照你自己 .claude/agents/ 配比。
- **[HN: What Hacker News Gets Right About AI Coding Agents in 2026](https://www.developersdigest.tech/blog/what-hacker-news-gets-right-about-ai-coding-agents-2026)** — 共识从"AI 工具是不是真的"过渡到"怎么让它经济可用 / 操作可信 / 结构可复用"。
- **[Secure Vibe Coding in 2026](https://snehbavarva.medium.com/secure-vibe-coding-in-2026-the-files-prompts-and-rules-of-use-and-research-e821021ee908)** — 整理 vibe coding 的文件 / prompt / 使用规则，安全侧最新汇编。

## 科技公司最新动态

### Anthropic
- **2026-05-14**：宣布 6/15 起 Claude 订阅大改 — Agent SDK 走独立 credit meter，paid plan 重新支持外部 agent 工具。
- **2026-05-14**：12 个法律垂直 plugin 发布。
- **2026-05-13**：**Claude for Small Business** 发布，深度集成 Quickbooks / PayPal / HubSpot / Canva / Docusign / Google Workspace / Microsoft 365。
- **2026-05-12**：Code w/ Claude SF 2026 大会收官（Plugin Marketplace / Agent View / Opus 4.7 1M context / AWS Platform）。
- **2026-05-11**：Claude Platform on AWS 上线、Agent View in Claude Code 上线。
- **2026-05-05**：10 个金融行业 ready-to-run agent template；Claude 接入 Microsoft Excel / PowerPoint / Word / Outlook 全套 add-in。
- **PwC 合作扩大**：在美区铺开 Claude Code + Cowork，新设 "Office of the CFO" 业务线基于 Claude。

### OpenAI
- 借 Anthropic 收紧之机，主动以 token 定价拉重度 agent 用户（Axios 2026-05-14）。
- **Codex CLI**：开源终端 coding agent 持续成为"用 OpenAI 写代码"的默认入口，已有大量 fork。

### Cursor / Windsurf / Cognition
- **Windsurf**：Google 拿走 CEO + co-founder + 40 工程师 + 2.4B 授权；Cognition 用 ~$250M 拿下剩余 IP / 品牌 / 210 员工。
- **Windsurf 2.0**（2026 年 4 月）：Agent Command Center + 与 Devin 集成；SWE-1.5（原 Devin 模型）成 Windsurf 默认。
- 业内共识：**Windsurf = 开发者在环 / Devin = 完全自主，底层共享 agent 层**。
- Cursor / Windsurf / Zed 三分高端 native 市场，其余卷价格或垂直。

### Microsoft / GitHub
- microsoft/ai-agents-for-beginners 持续在 trending（教育线）。
- githubnext/testpilot 持续作为"官方实验"放在生态前沿，单测生成方向。

## 今日新数据点

- **tinyhumansai/openhuman**：13.2k star，单日 +1,690（Rust 本地 AI 助手）。
- **GitHub 当日"主题相关 ≥ 1000 star"项目数：1**（明显低于本周平均，但 500-1000 档密度上升）。
- **Claude blog 近 7 天产出**：9 篇高密度，平均 < 1 天 1 篇，**产品 + 行业 + Code 三线齐推**。
- **Anthropic 计费改革倒计时：28 天**（6/15 生效）。

## 来源

### Claude 官方
- [claude.com/blog](https://claude.com/blog)

### Anthropic 新闻
- [Anthropic — Claude for Small Business](https://www.anthropic.com/news/claude-for-small-business)
- [Anthropic — Finance Agents](https://www.anthropic.com/news/finance-agents)
- [Anthropic — PwC Expanded Partnership](https://www.anthropic.com/news/pwc-expanded-partnership)
- [Releasebot: Anthropic 2026-05 Updates](https://releasebot.io/updates/anthropic)
- [Releasebot: Claude Code 2026-05](https://releasebot.io/updates/anthropic/claude-code)
- [Claude Code Changelog (claudefa.st)](https://claudefa.st/blog/guide/changelog)
- [Bloomberg Law: Anthropic Legal Push](https://news.bloomberglaw.com/legal-ops-and-tech/anthropic-pushes-deeper-into-legal-work-with-claude-updates)
- [SiliconANGLE: Claude for Small Business](https://siliconangle.com/2026/05/13/anthropic-launches-claude-small-business-new-automation-workflows/)
- [Axios: Anthropic vs OpenAI on tokens](https://www.axios.com/2026/05/14/anthropic-claude-price-openai-tokens)
- [Apiyi: 6/15 Billing Overhaul 解读](https://help.apiyi.com/en/anthropic-claude-subscription-agent-sdk-billing-split-june-2026-en.html)
- [pasqualepillitteri.it: Claude Code May 2026 Release Notes](https://pasqualepillitteri.it/en/news/2223/claude-code-may-2026-release-notes-radio-plugin-marketplace)

### HN / 行业讨论
- [HN: What Claude Code's Source Revealed](https://news.ycombinator.com/item?id=47772282)
- [HN: A few random notes from Claude coding](https://news.ycombinator.com/item?id=46771564)
- [HN: Claude Code and the Great Productivity Panic of 2026](https://news.ycombinator.com/item?id=47467922)
- [DecodingAI: Six-Agent Claude Code Team](https://www.decodingai.com/p/squid-my-agentic-coding-setup-may-2026)
- [Developer's Digest: HN AI Coding Agents 2026](https://www.developersdigest.tech/blog/what-hacker-news-gets-right-about-ai-coding-agents-2026)
- [Medium: Secure Vibe Coding in 2026](https://snehbavarva.medium.com/secure-vibe-coding-in-2026-the-files-prompts-and-rules-of-use-and-research-e821021ee908)
- [The Hacker News: Claude Code Leak](https://thehackernews.com/2026/04/claude-code-tleaked-via-npm-packaging.html)
- [DarkReading: LatAm Vibe Hackers](https://www.darkreading.com/cloud-security/ai-agents-generate-custom-hacking-tools)

### 编辑器 / IDE 对比
- [StartupHub: Cursor Alternatives 2026](https://www.startuphub.ai/ai-news/insights/2026/cursor-alternatives-ai-coding-tools-2026)
- [Blink: Best AI Coding Agents 2026](https://blink.new/blog/best-ai-coding-agents-2026)
- [NxCode: AI Coding Pricing 2026](https://www.nxcode.io/resources/news/ai-coding-tools-pricing-comparison-2026)

### GitHub 项目（已在正文中各表列出链接）
- 当日 trending：tinyhumansai/openhuman, oven-sh/bun, colbymchenry/codegraph, K-Dense-AI/scientific-agent-skills, Anil-matcha/Open-Generative-AI, calcom/cal.diy, microsoft/ai-agents-for-beginners, HKUDS/CLI-Anything
- UI/UX agent：ag-ui-protocol/ag-ui, VoltAgent/awesome-design-md, nextlevelbuilder/ui-ux-pro-max-skill, barbarosselimbuyukelci/mobile-ai-ui-ux-revamp-skill, veluthoor/ui-ux-design-review-agent, RedHat-UX/next-gen-ui-agent
- Test gen：confident-ai/deepeval, Kumari-Pragati/Intelligent-Test-Automation, furudo-erika/ai-testing-agent, mindfiredigital/AUTOTEST, githubnext/testpilot, herchila/unittest-ai-agent
- Video agent：HKUDS/VideoAgent, HKUDS/ViMax, FireRedTeam/FireRed-OpenStoryline, aregrid/frame, video-db/Director
