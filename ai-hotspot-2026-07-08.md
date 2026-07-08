# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-07-08

## 🌊 今日大势
Anthropic 把「模型可选 + effort 分级」下放进 Claude Code、并把 Cowork 推向移动端与政府市场，agentic 工作流从「工具」正式变成「团队编制」。生态侧的爆发全押在「Claude Code 之上再造一层产品」——找工作、Office 自动化、视频分析都是 fork Claude Code 起手。与此同时 HN 的另一面在冒烟：约 50 种绕过 Claude Code 权限系统的攻击面被披露，vibe coding 的「过测试却带洞」正在变成主流焦虑。

## ⭐ Claude 官方信号（最近 7 天 claude.com/blog）
| 标题 | 日期 | 分类 | 为什么重要 |
|---|---|---|---|
| Bringing Claude Code and Cowork to government | 07-07 | Product | Claude Code 进政府采购，企业级信任背书再上一档 ⭐ |
| Choosing a Claude model and effort level in Claude Code | 07-07 | Claude Code | 模型 + effort 可选下放到 CC，直接影响每次调用成本/质量取舍 ⭐📌 |
| Claude Cowork is coming to mobile and web | 07-07 | Product | Cowork 脱离桌面，agent 协作走向随身 |
| How people are using Claude Cowork | 07-07 | Enterprise | 真实用例集，human-agent 团队编排的样板 |
| A field guide to Claude Fable 5: Finding your unknowns | 07-06 | Claude Code | Fable 5 出口管制解除后回归，官方给出使用手册 |
| Giving admins more visibility/control over Claude spend | 07-02 | Product | 成本可观测/可控，企业 rollout 的关键闸门 |
| Getting started with loops | 06-30 | Claude Code | loops 功能入门，迭代式 agent 任务的新原语 |

## 📌 今日推荐阅读（基于 iOS / SwiftUI / vibe coding 视角）
1. **Choosing a Claude model and effort level in Claude Code** — 你在 SnapStamp/AE 后台跑大量 agent 任务，模型+effort 分级意味着可以把便宜档留给机械活、贵档留给硬 verify，直接省钱。
2. **addyosmani/agent-skills（+1,317⭐，72k）** — 生产级「AI coding agent 工程技能」合集，正好对齐你把可复用原则沉淀进知识库的做法，可挑用于 SwiftUI 工作流。
3. **nexu-io/open-design** — 开源版 Claude Design，让 coding agent 直接产 mockup/landing/PPTX/MP4，vibe-coding 出 UI 稿的本地替代方案，和你「先 mockup 再原生」的门控习惯契合。

## 📈 当日 GitHub 爆发项目（主题相关，新增 star ≥ 1000）
| 项目名 | 简介 | 当日新增 | 总 star | 信号 |
|---|---|---|---|---|
| MadsLorentzen/ai-job-search | 基于 Claude Code 的找工作框架：评估岗位、定制简历、写 cover letter、面试准备 | +2,514 | 11,000 | 📈📌 |
| addyosmani/agent-skills | 面向 AI coding agent 的生产级工程技能库 | +1,317 | 72,172 | ⭐ |

### 其他爆发项目（非主题）
- iOfficeAI/OfficeCLI (+893 ⭐): 为 AI agent 打造的 Office 套件，读写自动化 Word/Excel/PPT（单二进制）
- bradautomates/claude-video (+965 ⭐): 让 Claude 下载/抽帧/转录来分析视频

## GitHub 热门项目 — Agent 驱动 UI/UX 设计
| 项目名 | 简介 | 亮点 |
|---|---|---|
| nexu-io/open-design | 开源 Claude Design 替代，本地优先桌面 app | 让编码 agent 变设计引擎，产 HTML/PDF/PPTX/MP4 真文件，BYOK 20+ CLI |
| plugin87/ux-ui-agent-skills | 把 Claude 变资深设计架构师 | DTCG design tokens + 42 组件 + WCAG 2.2 + 138 套设计系统 |
| veluthoor/ui-ux-design-review-agent | AI 生成 UI 的评审工具 | 给配色/组件重设计/可访问性修复，solo dev 快速出货友好 |
| ag-ui-protocol/ag-ui | Agent-User 交互协议 | 事件驱动，把 agent 接入前端应用的标准 |

## GitHub 热门项目 — 自动化测试 / AI Test Gen
| 项目名 | 简介 | 亮点 |
|---|---|---|
| confident-ai/deepeval | LLM 评估框架 | agent 可生成数据集、写 eval 套件、跑测试并对失败指标迭代 |
| qodo-ai/qodo-cover | AI 自动化测试生成 + 覆盖率增强 | 聚焦单测自动补全 |
| Kumari-Pragati/Intelligent-Test-Automation | 多 agent LLM 测试框架 | AutoGen + unittest 从需求动态生成并校验用例 |
| tugkanboz/awesome-ai-testing | AI 测试工具清单 | 覆盖测试生成→自愈自动化→MCP 测试→LLM 评估 |

## GitHub 热门项目 — 视频剪辑自动化
| 项目名 | 简介 | 亮点 |
|---|---|---|
| calesthio/OpenMontage | 开源 agentic 视频生产系统 | 12 pipeline / 52 工具 / 500+ agent skill，兼容 CC/Cursor/Copilot/Windsurf/Codex |
| HKUDS/VideoAgent | 视频理解/编辑/重制一体化框架 | 图驱动工作流 + 自适应反馈环 |
| FireRedTeam/FireRed-OpenStoryline | 意图驱动的 AI 剪辑 agent | 自然语言指挥 + 可复用 Style Skills + human-in-the-loop |
| poseljacob/agentic-video-editor | 原始素材 + brief → 成品广告 | Gemini + FFmpeg agent 集成 |

## ⚠️ 用户痛点 / 负面信号
- **Claude Code 权限系统 ~50 种绕过**：HN/安全研究披露约 50 种绕过权限系统执行命令的方法（[SecurityWeek](https://www.securityweek.com/new-attack-abuses-claude-code-and-harmless-looking-repositories-to-hijack-developer-machines/)）。
- **恶意仓库劫持开发机**：研究者演示用「看似无害的仓库」劫持开发者机器；此前还有 Claude Code GitHub Action 漏洞——一个恶意 issue 即可劫持仓库（[The Hacker News](https://thehackernews.com/2026/06/claude-code-github-action-flaw-let-one.html)）。
- **vibe coding「沉默杀手」**：过了测试、躲过传统安全工具的可利用缺陷，被称为 vibe coding 的结构性风险。

## 论坛热门帖子（正向）
- [Tell HN: 我 60 岁，Claude Code 重新点燃了热情](https://news.ycombinator.com/item?id=47282777)
- [I used Claude Code to get a second opinion on my MRI](https://news.ycombinator.com/item?id=48708941)
- [A few random notes from Claude coding quite a bit](https://news.ycombinator.com/item?id=46771564) — 社区共识：把项目规则放进 repo、用 skills 编码可复用工作流、prompt 保持短而具体。

## 科技公司最新动态
- **Anthropic**（07-01）：Claude Sonnet 5 发布，成为 Free/Pro 默认模型，最 agentic 的 Sonnet，8/31 前引入价低于 Sonnet 4.6。
- **Anthropic**（06-29~07）：Claude apps gateway 上 Bedrock/Google Cloud；Claude 在 Microsoft Azure AI Foundry GA（首次跑在 NVIDIA GB300 Blackwell Ultra）。
- **Anthropic**：Fable 5 / Mythos 5 出口管制解除，7/1 全球恢复；发布 Claude Science 科研工作台。
- **OpenAI**（07-04）：GPT-5.6 Sol/Terra/Luna 驱动 Codex。
- **Cognition/Windsurf**：Windsurf 变 Devin Desktop，Pro 降至 $15/月（比 Cursor 便宜 $5）。
- **Google**：Antigravity 2.0 + Gemini 3.5 Flash。

## 今日新数据点
- Claude Code 2.1.202（07-06）：新增 `/config` 里「Dynamic workflow size」设置 + workflow.run_id/name 的 OpenTelemetry 属性；新增登录到期预警、手动权限模式灰色 ⏸ 徽章。
- ai-job-search 单日 +2,514⭐（当日爆发第一）。
- 2026 AI coding 已成七强格局：Claude Code / Antigravity / Codex / Cursor / Kiro / Copilot / Windsurf。

## 来源
- 官方：[claude.com/blog](https://claude.com/blog) · [Anthropic Newsroom](https://www.anthropic.com/news) · [Claude Code changelog](https://code.claude.com/docs/en/changelog)
- Trending：[GitHub Trending daily](https://github.com/trending?since=daily) · [zh](https://github.com/trending?since=daily&spoken_language_code=zh)
- 行业：[The New Stack](https://thenewstack.io/ai-coding-tool-stack/) · [Cognition/Windsurf](https://www.nxcode.io/resources/news/cognition-windsurf-acquisition-swe-1-5-codemaps-2026)
- 安全：[SecurityWeek](https://www.securityweek.com/new-attack-abuses-claude-code-and-harmless-looking-repositories-to-hijack-developer-machines/) · [The Hacker News](https://thehackernews.com/2026/06/claude-code-github-action-flaw-let-one.html)
- 项目：[ai-job-search](https://github.com/MadsLorentzen/ai-job-search) · [agent-skills](https://github.com/addyosmani/agent-skills) · [open-design](https://github.com/nexu-io/open-design) · [OpenMontage](https://github.com/calesthio/OpenMontage) · [deepeval](https://github.com/confident-ai/deepeval)
