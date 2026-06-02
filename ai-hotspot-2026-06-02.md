# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-06-02

## 🌊 今日大势
1. **Anthropic 向 SEC 递交 IPO 文件（6/1）**，估值预计破万亿——这是"Claude 经济学"从烧钱期转向商业化兑现的最强信号，6/15 的订阅计费拆分正是同一叙事的另一面。
2. **"白嫖 vibe coding"时代正式终结**：6/15 起订阅内的程序化用量（Agent SDK / `claude -p`）被切到独立 credit 池，$20 Pro 跑 $500 API 工作流的套利窗口关闭，HN 一片哀嚎与重新算账。
3. **生态在"省钱"与"加速"两端同时爆发**：一端是 markitdown / Scrapling 这类喂给 agent 的数据管道工具集体冲榜，另一端是 MoneyPrinterTurbo 等一键生成工具——agent 把上下游都吃干抹净。

## ⭐ Claude 官方信号（最近 7 天 claude.com/blog）
| 标题 | 日期 | 分类 | 为什么重要 |
|---|---|---|---|
| ⭐ Introducing dynamic workflows in Claude Code | 05-28 | Product | `/workflows` 编排几十到上百个后台 agent，多 agent 编排从插件变成一等公民 |
| ⭐ Claude Opus 4.8 发布（默认 high effort） | 05-28 | Product | 新默认模型，`/effort xhigh` 应对最难任务；agentic coding 能力再升级 |
| How CodeRabbit used Claude to build agent orchestration | 05-27 | Claude Code | 真实多 agent 代码评审落地案例，可直接借鉴架构 |
| Using LLMs to secure source code | 05-27 | Enterprise | LLM 做漏洞识别，安全左移的官方背书 |
| Zero Trust for AI agents | 05-27 | Enterprise | agent 权限最小化框架，自治 agent 上生产必读 |
| Code w/ Claude London 2026 | 05-26 | Product | 官方开发者大会，"重新思考如何构建软件" |
| 📌 Best practices for computer & browser use | 05-13 | Agents | 与 SnapStamp/手机操控类 agent 直接相关的官方调优指南 |

> ⚠️ **重大政策**：6/15 起订阅拆分为"交互用量"+"程序化用量"两个 credit 池（$20–$200/月），Agent SDK 与 multica 后台 daemon 需提前评估额度。

## 📌 今日推荐阅读（基于 iOS / SwiftUI / vibe coding 视角）
1. **dynamic workflows in Claude Code** — 你正用 multica 跑 App 工厂，官方 `/workflows` 多 agent 编排能直接替代部分自搓调度逻辑，值得对照。
2. **Best practices for computer & browser use（Agents）** — 与 `ae-mobile-agent` / `ae-desktop-agent` 同一套路，官方调优经验可直接喂回你的手机/桌面操控 skill。
3. **EveryInc/compound-engineering-plugin** — Claude Code 官方"复合工程"插件冲上 1.9w star，和你的 skill 化工作流理念高度同构，值得拆解它的 plugin 组织方式。

## 📈 当日 GitHub 爆发项目（主题相关，新增 star ≥ 1000）
| 项目名 | 简介 | 当日新增 | 总 star | 信号 |
|---|---|---|---|---|
| harry0703/MoneyPrinterTurbo | 一键 AI LLM 生成短视频 | +3,375 | 76,834 | 📈 视频自动化 |
| microsoft/markitdown | 文件/Office 文档转 Markdown（喂 agent 上下文神器） | +3,034 | 138,422 | ⭐📈 官方 |
| D4Vinci/Scrapling | 自适应 Web 抓取框架，单请求到全站爬取（agent 数据管道） | +1,486 | 58,040 | 📈 |

### 其他爆发项目（非主题）
- codecrafters-io/build-your-own-x (+1,212 ⭐): 从零重建经典技术的学习清单
- OpenBMB/VoxCPM (+888 ⭐): 无 tokenizer 多语言 TTS / 声音克隆
- FareedKhan-dev/train-llm-from-scratch (+861 ⭐): 从数据到生成的 LLM 训练教程
- hiroi-sora/Umi-OCR (+110 ⭐): 免费离线 OCR 软件

## GitHub 热门项目 — Agent 驱动 UI/UX 设计
| 项目名 | 简介 | 亮点 |
|---|---|---|
| nexu-io/open-design | 本地优先开源版 "Claude Design"，原生桌面 app | 259+ skills / 142+ 设计系统，支持 17+ CLI（含 Claude Code / Codex / Cursor） |
| ag-ui-protocol/ag-ui | Agent-User Interaction 协议，把 agent 接进前端 | 事件驱动标准协议，实时用户上下文同步 |
| VoltAgent/awesome-design-md | 品牌设计系统的 DESIGN.md 集合 | 丢进项目即可让 coding agent 生成匹配 UI |
| veluthoor/ui-ux-design-review-agent | 用 Gemini 评审 AI 生成的 UI | 输出配色/组件重设计/无障碍修复，solo dev 友好 |

## GitHub 热门项目 — 自动化测试 / AI Test Gen
| 项目名 | 简介 | 亮点 |
|---|---|---|
| confident-ai/deepeval | LLM 评估框架 | 让 coding agent 生成数据集、写评估套件、对失败指标迭代 |
| Kumari-Pragati/Intelligent-Test-Automation | 多 agent LLM 测试用例生成与验证 | AutoGen + unittest，创建/验证/执行分工 |
| mindfiredigital/AUTOTEST | 动态分析网页生成 Selenium 脚本 | LLM 驱动的端到端 Web 测试用例生成 |
| furudo-erika/ai-testing-agent | 开源软件测试 AI agent | 通用测试自动化框架 |

> 🆕 **RAMPART**（微软，5/20）：pytest 原生的 agentic AI 安全测试框架，含跨提示注入探针、危害分类覆盖，直接接 CI/CD。

## GitHub 热门项目 — 视频剪辑自动化
| 项目名 | 简介 | 亮点 |
|---|---|---|
| FireRedTeam/FireRed-OpenStoryline | 意图驱动的 AI 剪辑 agent | 3 月新增 ASR 粗剪 skill，自动去口水词/重复句；human-in-the-loop |
| HKUDS/VideoAgent | 视频理解/编辑/重制一体化 agentic 框架 | 把用户意图拆成显式+隐式子意图，图驱动工作流 |
| HKUDS/ViMax | 编剧/分镜/角色/生成端到端 | 从叙事输入到成片全自动 |
| aregrid/frame | 开源 "vibe video editor" | Cursor 式交互，自动剪辑增强 |

## ⚠️ 用户痛点 / 负面信号
- **Claude Pro 持续"砍功能"**：XDA 专栏《Anthropic keeps taking features away from Claude Pro》，作者称"快没理由替它辩护了"。
- **6/15 计费拆分引爆 HN**：被普遍解读为"vibe coding 红利结束"，Boris Cherny 称第三方工具绕过缓存"难以可持续"；indie hacker / 自动化工作流用户重新算账。
- **multica 已立 issue 应对**：`multica-ai/multica#2815` 讨论 6/15 程序化 credit 对 daemon claude 后端的影响——你自己的工厂链路需提前评估额度。

## 论坛热门帖子（正向）
- HN《How I'm Productive with Claude Code》(#47494890) — 实战生产力技巧
- HN《A few random notes from Claude coding quite a bit》(#46771564) — 长期重度使用手记
- HN《What Claude Code's Source Revealed About AI Engineering Culture》(#47772282) — 源码泄露后的工程文化讨论

## 科技公司最新动态
- **Anthropic（6/1）**：向 SEC 递交保密 IPO 文件，估值或破万亿。
- **Anthropic（5/28）**：Opus 4.8 发布 + Claude Code dynamic workflows。
- **Anthropic**：推出 **Claude for Small Business**，一键接入 QuickBooks / PayPal / HubSpot / Canva / Docusign / Google Workspace / M365。
- **Cognition / Windsurf**：整合波次推进，SWE-1.5（号称比 Sonnet 4.5 快 13×）+ Codemaps 可视化代码导航 + 内嵌 Devin；Pro 涨到 $20/月。
- **GitHub Copilot（6/1）**：flex billing 上线，固定价之上叠加按量 AI Credits 池。

## 今日新数据点
- Anthropic IPO 估值预期 **> $1 万亿**（6/1 递交）。
- 6/15 程序化 credit 池区间 **$20–$200/月**，按订阅档位分配。
- Claude Code 当前版本约 **v2.1.154**。
- markitdown 单日 **+3,034** star（总 13.8w）；MoneyPrinterTurbo 单日 **+3,375**。

## 来源
**Claude 官方 / Anthropic**
- [claude.com/blog](https://claude.com/blog)
- [Anthropic files for IPO (WaPo)](https://www.washingtonpost.com/technology/2026/06/01/anthropic-maker-claude-files-with-sec-go-public-an-ipo/)
- [Claude for Small Business](https://www.anthropic.com/news/claude-for-small-business)
- [June 15 billing change](https://codersera.com/blog/anthropic-june-2026-billing-change-claude-code/)
- [Claude Code release notes](https://github.com/anthropics/claude-code/releases)

**GitHub Trending**
- [trending?since=daily](https://github.com/trending?since=daily)
- [trending zh](https://github.com/trending?since=daily&spoken_language_code=zh)

**生态 / 竞品**
- [Cognition Windsurf acquisition (NxCode)](https://www.nxcode.io/resources/news/cognition-windsurf-acquisition-swe-1-5-codemaps-2026)
- [AI Coding Agents 2026 比较 (Lushbinary)](https://lushbinary.com/blog/ai-coding-agents-comparison-cursor-windsurf-claude-copilot-kiro-2026/)
- [open-design](https://github.com/nexu-io/open-design) · [ag-ui](https://github.com/ag-ui-protocol/ag-ui)
- [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) · [VideoAgent](https://github.com/HKUDS/VideoAgent)
- [deepeval](https://github.com/confident-ai/deepeval) · [Intelligent-Test-Automation](https://github.com/Kumari-Pragati/Intelligent-Test-Automation)

**论坛 / 痛点**
- [HN: Productivity Panic of 2026](https://news.ycombinator.com/item?id=47467922)
- [XDA: Claude Pro 砍功能](https://www.xda-developers.com/anthropic-keeps-taking-features-away-from-claude-pro-running-out-of-reasons-to-defend/)
- [multica#2815](https://github.com/multica-ai/multica/issues/2815)
