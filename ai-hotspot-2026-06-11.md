# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-06-11

## 🌊 今日大势
1. **Anthropic 把"模型"和"产品"同时推到新台阶**：6/9 发布 Claude Fable 5（Mythos 级别、面向通用安全开放的最强 GA 模型），同时 Managed Agents 拿到「定时调度 + Vault 环境变量 + 私有 MCP 沙箱」三件套——Anthropic 正在把 Claude 从"会写代码的模型"重塑成"能托管运行的 agent 平台"。
2. **IDE 战争升级为"agent 编排层"之争**：Cognition 把 Windsurf 重命名为 Devin Desktop 并押注开放的 ACP 协议（Codex / Claude Agent / OpenCode 可同台跑），编辑器不再是单 agent 容器，而是多 agent 的看板调度台。
3. **Skills 生态彻底爆发**：今日 GitHub Trending 前列被 agent-skills / pm-skills / superpowers / google-skills 霸榜——"给 agent 装技能包"已成为继 vibe coding 之后最热的开发者范式，但 6/15 起 Claude 订阅拆分计费的阴影也开始让重度用户焦虑。

## ⭐ Claude 官方信号（最近 7 天 claude.com/blog）
| 标题 | 日期 | 分类 | 为什么重要 |
|---|---|---|---|
| The evolution of agentic surfaces: building with Claude Managed Agents | 06-10 | Agents | 官方系统阐述"agent 界面"演进方向，Managed Agents 是未来产品形态的下注 |
| New in Claude Managed Agents: 定时运行 + Vault 存环境变量 | 06-09 | Product | Agent 从"对话触发"走向"无人值守定时跑"，配合 Vault 解决密钥安全——agent 工程化关键一步 |
| Building intelligent apps for Apple platforms with Claude in Foundation Models framework | 06-08 | Product | ⭐ 对 iOS 开发者极重要：Claude 通过新 Swift 包接入 Apple Foundation Models 框架 |
| How one Anthropic seller rebuilt his team's workflows with Claude Code | 06-05 | Claude Code | GTM 团队用 Claude Code 重建工作流的实战案例 |
| The Claude Cowork product guide | 06-05 | Enterprise | Cowork 企业协作完整指南 |
| Lessons from building Claude Code: How we use skills | 06-03 | Claude Code | 官方讲 skills 设计哲学，呼应今日 skills 生态爆发 |
| Running an AI-native engineering org | 06-03 | Claude Code | AI 原生工程组织的组织转型方法论 |
| A harness for every task: dynamic workflows in Claude Code | 06-02 | Claude Code | dynamic workflows / ultracode 的官方设计文档 |

## 📌 今日推荐阅读（基于 iOS / SwiftUI / vibe coding 视角）
1. **Building intelligent apps for Apple platforms with Claude in Foundation Models framework** — 直接面向你的主战场：Claude 现在能通过 Swift 包嵌入 Apple Foundation Models 框架，SnapStamp/SnapChef 这类 iOS AI App 未来可考虑端云混合识别架构。
2. **A harness for every task: dynamic workflows in Claude Code** + ultracode 设置 — vibe coding 进阶：把一次性 prompt 升级成可编排的多 agent 工作流，但官方明确警告 token 消耗激增，先用小任务摸清用量再放开。
3. **addyosmani/agent-skills（+821 ⭐）/ obra/superpowers** — "给 coding agent 装生产级技能包"已成主流范式，正好对应你大量自研 ae-* skill 的玩法，可借鉴其技能组织与发布结构。

## 📈 当日 GitHub 爆发项目（主题相关，新增 star ≥ 1000）
| 项目名 | 简介 | 当日新增 | 总 star | 信号 |
|---|---|---|---|---|
| mvanhorn/last30days-skill | 跨 Reddit/X/YouTube/HN/Polymarket 的研究综合 agent skill | +2,535 | 39,075 | 📈📌 |
| obra/superpowers | agentic skills 框架 + 软件开发方法论 | +1,104 | 223,596 | ⭐📈 |
| addyosmani/agent-skills | 面向 AI coding agent 的生产级工程技能集 | +821 | 51,799 | ⭐📌 |
| phuryn/pm-skills | PM Skills 市场：100+ agentic skills / 命令 / 插件 | +804 | 14,864 | 📌 |

### 其他爆发项目（非主题）
- refactoringhq/tolaria (+612 ⭐)：管理 markdown 知识库的桌面应用
- FareedKhan-dev/train-llm-from-scratch (+247 ⭐)：从零训练 LLM 全流程教程
- 521xueweihan/HelloGitHub (+143 ⭐)：入门级开源项目周刊（中文榜）
- AstrBotDevs/AstrBot (+94 ⭐)：多 IM 平台 + 多 LLM 的 agent 框架（中文榜）

## GitHub 热门项目 — Agent 驱动 UI/UX 设计
| 项目名 | 简介 | 亮点 |
|---|---|---|
| nexu-io/open-design | 本地优先、开源的 Claude Design 替代品，原生桌面应用 | 259+ Skills / 142+ 设计系统，支持 Claude Code/Codex/Cursor 等 17+ CLI |
| ag-ui-protocol/ag-ui | Agent-User 交互协议，把 agent 带入前端应用 | 事件驱动、标准化 agent↔UI 实时连接 |
| veluthoor/ui-ux-design-review-agent | 用 Gemini 审查 AI 生成 UI 的设计质量 | 给配色、组件重设计、无障碍修复建议，solo dev 友好 |
| HermeticOrmus/LibreUIUX-Claude-Code | Claude Code 的完整 UI/UX 系统 | 67 个专用 agent + 设计词汇 + 实测 prompt |

## GitHub 热门项目 — 自动化测试 / AI Test Gen
| 项目名 | 简介 | 亮点 |
|---|---|---|
| getautonoma (Autonoma AI) | AI E2E 测试，从 prompt 生成并维护端到端套件 | 输出可在 CI 确定性运行的 Playwright/Appium 代码，应用变更自动更新 |
| OpenAI Evals / LangSmith / Braintrust | LLM/agent 评测框架标准化 | 2026 三大趋势：框架标准化、多 agent 测试、自主测试生成 |
| QA Wolf / Virtuoso | 生成式 AI 测试工具 | 从需求/用户故事自动产出测试用例 + 失败归因 |

> ⚠️ 行业共识：自主测试仍卡在"谁来验证 agent 生成的测试用例本身是否正确"这一 bootstrapping 难题，多数工具只做好了生成→执行→归因→自愈四步中的一两步。

## GitHub 热门项目 — 视频剪辑自动化
| 项目名 | 简介 | 亮点 |
|---|---|---|
| FireRedTeam/FireRed-OpenStoryline | 意图驱动的 AI 视频剪辑 agent | 自然语言导演 + LLM 规划 + 工具编排；新增 ASR 粗剪自动去口水词 |
| HKUDS/ViMax | 一体化 agentic 视频生成（导演/编剧/制片全包） | 从叙事输入到成片端到端自动化 |
| HKUDS/VideoAgent | 视频理解/剪辑/二创一体框架 | 图驱动工作流 + 自适应反馈循环 |
| aregrid/frame | 开源 "vibe video editor" | Cursor 式交互，自动剪辑 + 画质增强 |
| video-db/Director | AI 视频 agents 框架 | 总结/剪辑/搜索多 agent 协作 + 实时进度反馈 |

## ⚠️ 用户痛点 / 负面信号
- **6/15 订阅拆分计费**：Claude 订阅将拆成「交互用量（Claude Code/chat/Cowork）」与「程序化用量（agent 独立月度 credit 池）」两个池，重度 vibe coding / agent 用户担心成本上升。([it-connect](https://www.it-connect.tech/vibe-coding-claude-unlimited-api-ends-on-june-15-2026/))
- **Claude Code GitHub Action 安全漏洞**：单个恶意 issue 即可劫持仓库，提醒 agent 自动化流水线的供应链风险。([The Hacker News](https://thehackernews.com/2026/06/claude-code-github-action-flaw-let-one.html))
- **dynamic workflows token 暴涨**：官方自己警告 dynamic workflows 比常规 session 消耗多得多，建议先用 scoped 小任务试水。
- **agentic coding 心理疲劳**：HN 讨论提到高速 agent 编码会因决策与动作量过大导致精神耗竭。([HN](https://news.ycombinator.com/item?id=47467922))

## 论坛热门帖子（正向）
- **Claude Fable 5** 发布讨论（HN）：社区对 Mythos 级能力开放 GA 的关注。([HN](https://news.ycombinator.com/item?id=48463808))
- **"Tell HN: I'm 60 years old. Claude Code has re-ignited a passion"**：Claude Code 重燃老程序员编程热情的高赞帖。([HN](https://news.ycombinator.com/item?id=47282777))
- **The New Stack 横评**：Claude Code vs Cursor vs Codex vs Antigravity 半年使用复盘。([The New Stack](https://thenewstack.io/claude-code-vs-cursor-vs-codex-vs-antigravity-2026/))

## 科技公司最新动态
- **Anthropic（06-09）**：发布 Claude Fable 5（Mythos 级 GA），Mythos 5 经 Project Glasswing 限量开放；Glasswing 扩展至约 150 个新组织。
- **Anthropic（06-09）**：Managed Agents 支持定时运行 + Vault 环境变量 + 私有 MCP 沙箱（公测）。
- **Anthropic（06-03）**：推出 Claude Partner Network 的 Services Track 与 Partner Hub。
- **Anthropic（公告）**：Claude Opus 4.1 弃用，API 退役定于 2026-08-05。
- **Cognition / Windsurf（06-02）**：Windsurf 通过 OTA 更新更名为 Devin Desktop，引入 Agent Command Center + 开放 ACP 协议（多 agent 同台）。
- **OpenAI Codex（06 月）**：在 Amazon Bedrock GA，新增 Sites / in-thread Annotations / 6 个业务插件；GPT-5.3-Codex 原生进入 Cursor 和 VS Code。

## 今日新数据点
- Claude Fable 5 = 历史上 GA 开放的能力最强模型（Mythos 级，2.1.170 版本随 Claude Code 一同发布）。
- dynamic workflows 现已在 Claude Code CLI/Desktop/VS Code 扩展进入 research preview（Max/Team/Enterprise + API/Bedrock/Vertex/Foundry）。
- last30days-skill 单日 +2,535 star，为今日 AI 主题最高增长项目。
- obra/superpowers 总 star 突破 223.5k，仍单日 +1,104。

## 来源
**Claude 官方 / Anthropic**
- [claude.com/blog](https://claude.com/blog)
- [Anthropic Newsroom](https://www.anthropic.com/news)
- [Releasebot — Claude Code Updates](https://releasebot.io/updates/anthropic/claude-code)
- [Claude Code Changelog](https://code.claude.com/docs/en/changelog)
- [Gate News — Claude Fable/Mythos](https://www.gate.com/news/detail/anthropic-releases-claude-mythos-ai-model-as-claude-fable-on-june-9-2026-21740412)

**GitHub Trending**
- [GitHub Trending (daily)](https://github.com/trending?since=daily)
- [GitHub Trending (中文)](https://github.com/trending?since=daily&spoken_language_code=zh)

**行业动态 / 横评**
- [The New Stack — Claude Code vs Cursor vs Codex vs Antigravity](https://thenewstack.io/claude-code-vs-cursor-vs-codex-vs-antigravity-2026/)
- [CodingWithAI — Windsurf becomes Devin Desktop](https://codingwithai.com/news/windsurf-devin-desktop-launch-june-2026)
- [OpenAI Codex Changelog](https://developers.openai.com/codex/changelog)

**痛点 / 安全**
- [it-connect — Claude API pricing 6/15](https://www.it-connect.tech/vibe-coding-claude-unlimited-api-ends-on-june-15-2026/)
- [The Hacker News — Claude Code GitHub Action flaw](https://thehackernews.com/2026/06/claude-code-github-action-flaw-let-one.html)

**细分赛道项目**
- [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) · [ViMax](https://github.com/HKUDS/ViMax) · [VideoAgent](https://github.com/HKUDS/VideoAgent) · [video-db/Director](https://github.com/video-db/Director)
- [nexu-io/open-design](https://github.com/nexu-io/open-design) · [ag-ui-protocol/ag-ui](https://github.com/ag-ui-protocol/ag-ui) · [ui-ux-design-review-agent](https://github.com/veluthoor/ui-ux-design-review-agent)
