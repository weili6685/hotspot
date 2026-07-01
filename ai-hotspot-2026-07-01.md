# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-07-01

## 🌊 今日大势
Anthropic 本周把重心从"拼参数"切到"铺渠道"——Microsoft Foundry GA、Bedrock/Google Cloud 双云 gateway、Claude Science 科研工作台一次性把企业和科研入口铺满，再叠上 Sonnet 5 成为 Claude Code 默认模型（原生 1M context、$2/$10 促销价），这是一场"无处不在"的部署面争夺战。生态侧 agent 编排框架继续霸榜（agency-agents 单日 +1791、superpowers、google/agents-cli），而 video-use、facebook/astryx 说明"agent-ready"正从写代码蔓延到视频剪辑和设计系统。与此同时安全阴影加深：研究者演示用"看似无害的仓库"劫持 Claude Code 开发机，vibe coding 的"沉默漏洞"成为 HN 主线焦虑。

## ⭐ Claude 官方信号（最近 7 天 claude.com/blog）
| 标题 | 日期 | 分类 | 为什么重要 |
|---|---|---|---|
| Getting started with loops | 06-30 | Claude Code | Claude Code 原生循环/迭代自动化落地，vibe coding 长任务托管的关键能力 |
| Introducing the Claude apps gateway for Amazon Bedrock and Google Cloud | 06-29 | Product | Claude 应用可跨 AWS/GCP 部署，双云战略进一步补齐 |
| Claude in Microsoft Foundry is now generally available | 06-29 | Product | 三大云全部就位，企业采买门槛再降 |
| Building effective human-agent teams | 06-24 | Enterprise AI | 官方给出"人机协作团队"编排方法论，呼应 agent teams 主线 |
| Agent identity in Claude Tag: a new access model for autonomous, team-wide AI | 06-24 | Claude Code | 自治 agent 的身份/权限模型，团队级自动化的基础设施 |
| The full Claude Desktop experience on AWS, Google Cloud, and Microsoft Foundry | 06-22 | Enterprise AI | Claude Desktop 全功能进三云 |
| Steering Claude Code: CLAUDE.md files, skills, hooks, rules, subagents and more | 06-18 | Claude Code | 一篇讲清 Claude Code 全部可控面，vibe coder 必读 |
| Claude Code now supports artifacts | 06-18 | Product | Claude Code 加入 artifacts，代码可视化增强 |

> 补充（近期检索到的官方动态）：**Claude Science** 科研工作台开放 beta（Pro/Max/Team/Enterprise 可用，最高 $30k credits，申请截止 **07-15**）；**Claude for Small Business** 上线；**Claude Code 周用量上调 50%（延续至 07-13）**——被外界解读为对标 Codex 的防守动作。

## 📌 今日推荐阅读（基于 iOS / SwiftUI / vibe coding 视角）
1. **Steering Claude Code（官方）** — 你天天在用 CLAUDE.md / skills / hooks / subagents，这篇是唯一一份把它们讲全的官方地图，直接决定你的 vibe coding 效率上限。
2. **altic-dev/FluidVoice（Swift, +588⭐）** — 纯 Swift 写的 macOS 端上语音听写 + AI 增强，on-device speech 的工程实现，对做 iOS/Apple 平台的你最有参照价值。
3. **Getting started with loops（官方）+ Claude Code 循环能力** — 长任务托管 / 无人值守跑完一批活，正好对上你 SnapStamp 的构建-验证-修复回路。

## 📈 当日 GitHub 爆发项目（主题相关）
| 项目名 | 简介 | 当日新增 | 总 star | 信号 |
|---|---|---|---|---|
| msitarzewski/agency-agents | 完整"AI 代理公司"，从前端到社区运营的专业化 agent 集合 | +1,791 | 120,885 | 📈📌 |
| xbtlin/ai-berkshire | AI 方法论驱动的价值投资研究框架 | +969 | 7,486 | 📈 |
| obra/superpowers | Agentic 技能框架 + 软件开发方法论 | +890 | 242,492 | ⭐ |
| browser-use/video-use | 由 coding agent 驱动的视频剪辑工具 | +721 | 12,594 | 📌 |
| HKUDS/Vibe-Trading | 个人交易 agent 应用 | +721 | 15,791 | 📈 |
| altic-dev/FluidVoice | macOS 端上语音听写 + AI 增强（Swift） | +588 | 4,928 | ⭐📌 |
| usestrix/strix | 开源 AI 渗透测试工具，自动找并修复漏洞 | +515 | 28,124 | ⚠️ |
| ogulcancelik/herdr | 终端内的 agent 多路复用器（Rust） | +486 | 9,012 | — |
| google/agents-cli | Google Cloud 上创建/部署 AI agent 的 CLI 与 skills | +445 | 4,192 | ⭐ |
| diegosouzapw/OmniRoute | 免费 AI 网关，支持 231+ 提供商 + token 压缩 | +387 | 8,519 | — |

### 其他爆发项目（非主题）
- hasaneyldrm/exercises-dataset (+1,343 ⭐)：含 433 个动作的健身数据集
- simplex-chat/simplex-chat (+1,235 ⭐)：无用户标识符的隐私优先即时通讯网络
- ripienaar/free-for-dev (+742 ⭐)：开发者免费额度 SaaS/PaaS/IaaS 清单

## GitHub 热门项目 — Agent 驱动 UI/UX 设计
| 项目名 | 简介 | 亮点 |
|---|---|---|
| facebook/astryx | 开源、完全可定制且"agent ready"的设计系统 | 今日趋势榜 +364⭐；大厂出品，agent 时代设计系统范式 |
| educlopez/ui-craft | 面向 AI coding agent 的设计工程系统，可作 skill 安装 | spec 驱动管线：brief→tokens→shape→craft→converge→ship |
| Seance1723/UXCraft | AI coding agent 的 UI/UX skill，一键激活设计师+研究员+前端 Lead 工作流 | 20+ UI 风格、WCAG、16 框架、dev handoff |
| veluthoor/ui-ux-design-review-agent | 用 Gemini 审 AI 生成的 UI，给配色/组件重设计/无障碍建议 | 单人开发者快速出货的"审美兜底"工具 |
| ag-ui-protocol/ag-ui | Agent-User 交互协议，把 agent 接进前端应用 | 事件驱动、标准化 agent↔UI 连接 |
| HermeticOrmus/LibreUIUX-Claude-Code | Claude Code 的完整 UI/UX 系统，67 个专用 agent | 设计词汇 + 实测 prompts |

## GitHub 热门项目 — 自动化测试 / AI Test Gen
| 项目名 | 简介 | 亮点 |
|---|---|---|
| confident-ai/deepeval | LLM 评估框架 | 可让 coding agent 生成数据集、写 eval 套件、跑 test run 迭代失败指标 |
| strands-agents/evals | AI agent 与 LLM 应用的综合评估框架 | 从上下文描述自动生成完整测试套件 |
| Kumari-Pragati/Intelligent-Test-Automation | 多 agent LLM 框架，动态生成+验证测试用例 | 基于 AutoGen + Python unittest，按需求自动生成 |
| herchila/unittest-ai-agent | AI 自动生成单元测试 | 轻量、聚焦单测生成 |
| tugkanboz/awesome-ai-testing | AI 测试工具/框架/资源清单 | 覆盖测试生成、自愈自动化、MCP 测试、LLM eval |

## GitHub 热门项目 — 视频剪辑自动化
| 项目名 | 简介 | 亮点 |
|---|---|---|
| browser-use/video-use | coding agent 驱动的视频剪辑 | 今日趋势榜 +721⭐，来自 browser-use 团队 |
| FireRedTeam/FireRed-OpenStoryline | 意图驱动的 AI 视频剪辑 agent | AI 转场生成 + ASR 粗剪自动去口水词/重复句 |
| calesthio/OpenMontage | 号称首个开源 agentic 视频生产系统 | 12 管线 / 52 工具 / 500+ agent skills，把 coding 助手变制片厂 |
| HKUDS/ViMax | 多 agent 视频框架，自动多镜头生成 | 保证人物/场景一致性 |
| HKUDS/VideoAgent | 视频理解/剪辑/重制一体化 agentic 框架 | 图驱动工作流 + 自适应反馈环 |
| aregrid/frame | 开源"vibe video editor"，Cursor 式交互 | 面向创作者的专业剪辑替代品 |

## ⚠️ 用户痛点 / 负面信号
- **供应链攻击演示**：研究者展示用"看似无害的仓库"滥用 Claude Code、劫持开发者机器（SecurityWeek）。给所有跑本地 agent 的人敲警钟——untrusted repo + 自动执行 = 高危。
- **vibe coding 的"沉默漏洞"**：自然语言生成的代码能过测试、却躲过传统安全工具，成为可利用缺陷的温床。
- **"2026 生产力恐慌"**：HN 长贴讨论 Claude Code 带来的岗位/技能焦虑（news.ycombinator.com/item?id=47467922）。
- **fast mode 迁移坑**：Claude Opus 4.7 的 fast mode 将于 **07-24 移除**，此后 `speed:"fast"` 请求报错，需迁移到 Opus 4.8 fast mode。

## 论坛热门帖子（正向）
- **Claude Code 登顶 HN #1**：`.claude/` 目录结构深度拆解贴收获 556 分。
- **Agent teams 成 2026 关键词**：大型软件工作自然拆成规划/实现/测试修复/安全审查/文档/迁移/浏览器 QA/发布说明等专业分工，Claude Code 被认为是首批"原生支持"该拆分的工具（Developers Digest playbook）。
- **Ask HN: 2026 最佳托管 agent** 讨论热度高（item?id=46917293），Claude Managed Agents 单独成贴。

## 科技公司最新动态
**Anthropic**
- 06-29 Claude 进 Microsoft Foundry GA；同日发布 Bedrock + Google Cloud apps gateway。
- 近期 Claude Science 科研工作台开放 beta，申请截止 07-15、07-31 发通知。
- Claude Sonnet 5 成为 Claude Code 默认模型，原生 1M context，$2/$10 per Mtok 促销至 08-31（需升级到 2.1.197）。
- Claude Code 周用量上调 50%，延续至 07-13。

**Cognition（Devin / 原 Windsurf）**
- 06-02 Windsurf OTA 更名为 **Devin Desktop**；本地 Cascade agent **今日 07-01 EOL**，由 Devin Local 取代。
- 已发自研编码模型 **SWE-1.5**，宣称比 Claude Sonnet 4.5 快 13×（厂商口径，待独立验证）。
- 此前 OpenAI 约 $3B 收购 Windsurf 因微软 IP 争议告吹；Cognition 以 $250M 完成收购。

**OpenAI / Codex**
- Codex 推出 Skills、并有官方插件可在 Claude Code 内运行；Plus/Pro/Business/Enterprise 已从按条计费切换为 API token 计费。

## 今日新数据点
- **07-01（今日）**：Cognition 本地 Cascade agent 正式 EOL，切换 Devin Local。
- Claude Science credits 申请窗口开放，**07-15** 截止。
- Claude Code fast mode（Opus 4.7）将于 **07-24** 移除。
- Claude Code 周用量 +50% 延续至 **07-13**。
- 单日 GitHub 最强 AI/agent 增长：agency-agents **+1,791⭐**。

## 来源
**Claude 官方**
- [claude.com/blog](https://claude.com/blog)
- [Anthropic Newsroom](https://www.anthropic.com/news) · [Claude for Small Business](https://www.anthropic.com/news/claude-for-small-business)
- [Claude Code release notes (Releasebot)](https://releasebot.io/updates/anthropic/claude-code) · [What's new — Claude Code Docs](https://code.claude.com/docs/en/whats-new)
- [Claude Science Workbench (Technobezz)](https://www.technobezz.com/news/anthropic-launches-claude-science-workbench-for-researchers-and-drug-discovery)
- [Claude Code weekly limits +50% (Pasquale Pillitteri)](https://pasqualepillitteri.it/en/news/2494/claude-code-weekly-limits-50-percent-anti-codex-anthropic-2026)

**GitHub Trending**
- [github.com/trending (daily)](https://github.com/trending?since=daily) · [trending zh](https://github.com/trending?since=daily&spoken_language_code=zh)

**竞品 / 行业**
- [Cognition × Windsurf 收购 (NxCode)](https://www.nxcode.io/resources/news/cognition-windsurf-acquisition-swe-1-5-codemaps-2026) · [Devin 2026 (Apidog)](https://apidog.com/blog/whats-new-in-devin-2026/)
- [AI coding stack merging (The New Stack)](https://thenewstack.io/ai-coding-tool-stack/)

**安全 / HN / Reddit**
- [Claude Code repo 劫持攻击 (SecurityWeek)](https://www.securityweek.com/new-attack-abuses-claude-code-and-harmless-looking-repositories-to-hijack-developer-machines/)
- [Great Productivity Panic (HN)](https://news.ycombinator.com/item?id=47467922) · [Claude Managed Agents (HN)](https://news.ycombinator.com/item?id=47693047) · [Best hosted agent 2026 (HN)](https://news.ycombinator.com/item?id=46917293)
- [Agent teams playbook (Developers Digest)](https://www.developersdigest.tech/blog/claude-code-agent-teams-subagents-2026)

**分类项目源**
- 视频：[video-use](https://github.com/browser-use/video-use) · [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) · [OpenMontage](https://github.com/calesthio/OpenMontage) · [ViMax](https://github.com/HKUDS/ViMax)
- UI/UX：[astryx](https://github.com/facebook/astryx) · [ui-craft](https://github.com/educlopez/ui-craft) · [UXCraft](https://github.com/Seance1723/UXCraft) · [ag-ui](https://github.com/ag-ui-protocol/ag-ui/)
- 测试：[deepeval](https://github.com/confident-ai/deepeval) · [strands-agents/evals](https://github.com/strands-agents/evals) · [awesome-ai-testing](https://github.com/tugkanboz/awesome-ai-testing)
