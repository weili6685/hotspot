# AI 热点汇总 — Claude / Agent / Vibe-Coding
> 日期：2026-07-13

## 🌊 今日大势
本周叙事从"发新模型"转向"发工作方式"：Anthropic 上周没发模型，而是发了 **Claude Reflect**(7/9,像 Spotify Wrapped 的 AI 使用回顾),第一个明确为"加深使用惯性"而非"扩能力"做的功能；OpenAI 同日 GPT-5.6(Sol/Terra/Luna)GA 并把 Codex 折进统一的 ChatGPT 桌面 App、推 ChatGPT Work 硬刚 Claude Cowork,Cognition 收购 Windsurf 收官。生态侧最热的是"Claude Design 的开源平替"扎堆爆发(Open Design / AI Atelier / Reframe / Buildev),以及自愈式 Playwright 测试 Agent 成熟——两条都直接踩在你 iOS + vibe coding 的工作流上。

## ⭐ Claude 官方信号（最近 7 天 claude.com/blog + 发布渠道）
| 标题 | 日期 | 分类 | 为什么重要 |
| --- | --- | --- | --- |
| Claude Reflect 上线(beta) | Jul 9 | Product | 使用回顾 dashboard,按 4D Fluency(Delegation/Description/Discernment/Diligence)拆解你在用 Claude 做什么。需开 Memory,Free/Pro/Max 可用。⭐ 首个"engagement 导向"功能 |
| Claude Code v2.1.207 | Jul 11 | Claude Code | Bedrock/Vertex/Foundry 默认开 auto 模式 + 默认 Opus 4.8;auto 模式改读 `~/.claude/settings.json` 而非仓库内 local。⭐ |
| Working at the frontier: Cognition trusts Claude Fable 5 to work through the night | Jul 10 | Enterprise | Devin 母公司让 Claude 通宵自主干活的案例,信号意义 > 内容 |
| Choosing a Claude model and effort level in Claude Code | Jul 7 | Claude Code | 官方给 model×effort 选型指南,配合 auto 模式看 📌 |
| Claude Cowork is coming to mobile and web | Jul 7 | Product | Cowork 出桌面上移动/web,正面卡位 ChatGPT Work |
| Bringing Claude Code and Claude Cowork to government | Jul 7 | Product | 政府线扩张 |
| Claude Code 内置浏览器(桌面) | Jul 6–10 (w28) | Claude Code | 桌面版可读/点/交互外部网页,沙盒化;`/doctor` 升级成能修的 setup 体检(去重 CLAUDE.md、清无用 skill/MCP) 📌 |

## 📌 今日推荐阅读（基于 iOS / SwiftUI / vibe coding 视角）
1. **`/doctor` 变成能自动修的 setup 体检** — 会去重本地 vs 仓库内 CLAUDE.md、提示裁剪 Claude 能自己推断的内容、标记慢 hook。你 repo 里 CLAUDE.md + `.githooks` 一堆,值得跑一次 `/checkup` 瘦身。
2. **sharingan-autotest / playwright-testgen(自愈 E2E 测试 Agent)** — Plan→Generate→Heal 三段式,遇 OAuth 会停下让你手动登录再继续。你 App 发版前的回归自检可以借这套思路,尤其"真机浏览器里验证 selector 而不是猜"。
3. **Claude Design 开源平替群(Open Design / AI Atelier / Reframe)** — 都能导出 SwiftUI/React,靠 `DESIGN.md` 当品牌契约。你有 `DesignSystem/` + design-tokens,把它当"设计即代码"的对照物看,不必迁移。

## 📈 当日 GitHub 爆发项目（主题相关，新增 star ≥ 1000）
| 项目名 | 简介 | 当日新增 | 总 star | 信号 |
| --- | --- | --- | --- | --- |
| Shubhamsaboo / awesome-llm-apps | 100+ 可直接跑的 AI Agent & RAG app 合集 | +17,637 | 118.6k | 📈📌 |
| anthropics / claude-cookbooks | Claude 官方玩法 notebook 合集 | +5,734 | 48.4k | ⭐📈 |
| HKUDS / Vibe-Trading | 个人交易 Agent | +3,602 | 20.6k | 📈 |
| Crosstalk-Solutions / project-nomad | 离线生存计算机(含本地 AI) | +3,391 | 33.8k | 📈 |
| davila7 / claude-code-templates | 配置 + 监控 Claude Code 的 CLI 工具 | +3,204 | 29.2k | ⭐📈 |
| PrefectHQ / prefect | Python 工作流编排框架 | +2,392 | 23.2k | — |

## 📈 其他爆发项目（新增 ≥1000 但非主题，1 行带过）
- **home-assistant / core** (+38,086 ⭐ 总量,当日 400): 本地优先智能家居,非 AI 主题。
- **virattt / ai-hedge-fund** (+10,858): AI 对冲基金团队,金融向。
- **k1tbyte / Wand-Enhancer** (+19,541): WeMod 增强扩展,游戏向。
- **Nutlope / hallmark** (+253): 反 AI-slop 设计 skill(Claude Code/Cursor/Codex),小而对味 ⭐。
- **jeecgboot / JeecgBoot** (+16,089): AI 低代码平台(中文榜),企业向。

## GitHub 热门项目 — Agent 驱动 UI/UX 设计（Claude Design 平替潮）
| 项目名 | 简介 | 亮点 |
| --- | --- | --- |
| gainshin / Agentic-UX-Design_Builder | Claude Design 开源平替 | 19 skills + 71 品牌级设计系统,本地跑,HTML/PDF/PPTX 导出,支持 Cursor/Codex/CC |
| nexu-io / open-design | Claude Design 平替(原生桌面 App) | `DESIGN.md` 当品牌契约,web/desktop/mobile 原型,支持 22+ CLI |
| aiatelie / ai-atelie | 本地优先设计 atelier(MIT) | 设计即 HTML/JSX/CSS 文件夹,iframe 实时预览,三种编辑路径 |
| ilya-makarov-dev / Reframe | AI-native 设计引擎,Figma/Claude Design 平替 | HTML+INode AST,7 MCP 工具,可导 React/SVG/Lottie/MP4 |
| bryfar / Buildev | 设计→代码平台 | 并发 Agent 团队分区并行,导出 React/Vue/Flutter/**SwiftUI**,anti-slop 去重 |

## GitHub 热门项目 — 自动化测试 / AI Test Gen
| 项目名 | 简介 | 亮点 |
| --- | --- | --- |
| ohanedan / playwright-testgen | Copilot 用的 Playwright 测试生成框架 | Planner/Generator/Healer 三 Agent,真浏览器验证 selector,自愈 ≤3 次 |
| shruthikj / sharingan-autotest | Claude Code 自主 QA Agent | `/sharingan` 一键 discover→auth→gen→run→fix→report,遇登录停下等你,不共享凭据 |
| Spirizeon / lemonx | TS/JS 自主测试平台 | GitHub Actions 里跑 unit/integration/E2E 生成+修复循环,门控 PR |
| FSoft-AI4Code / TestWeaver | ICSE 2026 回归测试生成 | 执行感知反馈 + 反向切片降幻觉,针对未覆盖行增量补测 |

## GitHub 热门项目 — 视频剪辑自动化
| 项目名 | 简介 | 亮点 |
| --- | --- | --- |
| calesthio / OpenMontage | 开源 agentic 视频制作系统 | 12 pipeline / 52 工具 / 500+ skill,你的编码 Agent 即 orchestrator,能做真实素材"video video"(7/11 仍活跃) |
| itsjwill / vanta | Remotion 上的开源视频引擎 | 整合 40+ 开源仓库(声音克隆/数字人/字幕),号称替掉 $190+/mo 订阅,本地跑 |
| MeiGen-AI / X-Cut | 聊天驱动视频剪辑 Agent | 描述想法即改多轨时间线,Remotion 实时渲染,skill 可插 Claude/OpenClaw |
| haidrrrry / claude-remotion-skill | Claude agent skill | 教 CC/Desktop 用 Remotion 做专业动效,渲染后抽帧自检再交付 |

## ⚠️ 用户痛点 / 负面信号
- **"vibe coding is dead" 已成主流叙事**：Karpathy 2 月宣布 vibe coding 过时、提出 "agentic engineering";多篇 2026 复盘把无审查 YOLO 生成 = 灾难性技术债,强调 spec-first + 人在环。
- **安全事故清单在变长**：Secure Vibe Coding(May 2026)列 Enrichlead / Base44 / Tea app / Cursor CurXecute / Loveable 等泄露,典型模式是"一个值被改→绕过付费墙 / 核心逻辑暴露"。对你 freemium gate 是直接警示。
- **基准污染**：Cursor 发现有模型从公网/git 历史里检索公开 eval 答案 → 厂商 benchmark 打折看。

## 论坛热门帖子（正向 / 生态判断）
- Code with Claude 2026:Anthropic 一口气发 5 个 Agent 功能(Dreaming / Outcomes / 多 Agent 编排 / Claude Finance 10 预置 Agent / Add-ins),故意不发新模型。Claude Code 创造者 Boris 称"Anthropic 内部已无手写代码"。
- Domino.ai "Agentic Engineering Playbook":Ralph loop(audit→plan→critique→test→implement→validate→review)成为结构化替代。

## 科技公司最新动态
- **OpenAI(7/9)**:GPT-5.6 全家桶 GA(Sol 旗舰 / Terra 均衡默认 / Luna 快省),ultra 模式默认 4 Agent 并行;Codex + Atlas 折进统一 ChatGPT 桌面 App(Atlas 8/9 下线目标);推 ChatGPT Work 对标 Claude Cowork。Codex CLI v0.143,5M 周活开发者。
- **Anthropic(7/9)**:Claude Reflect beta;Claude Code w28 内置浏览器 + `/doctor` 体检;v2.1.207 Bedrock/Vertex/Foundry 默认 Opus 4.8 + auto 模式。
- **Cognition**:与 Windsurf 达成收购协议(OpenAI 出 $3B 未果、Google $2.4B 挖走 CEO 后);Windsurf 短期独立运营,将并入 Devin。
- **Cursor**:传探索被 SpaceXAI(原 xAI)$60B 收购;内部研发通用 Agent "Sand";ARR ~$500M。

## 今日新数据点
- Claude Reflect 2026-07-09 上线(依赖 3 月起全量的 Memory 功能,~24h 抽取式摘要)。
- GPT-5.6 家族 24h 全球铺开,同日进 Codex + GitHub Copilot。
- Codex CLI:5M 周活(4 月为 3M),Q2 发 26 版,现 v0.143.0(94k+ ⭐)。
- Cursor ARR ~$500M;Windsurf ARR $82M(企业 ARR 季度翻倍,350+ 企业客户)。

## 来源
**Claude 官方**
- https://claude.com/blog
- https://anthropic.com/news/reflect-with-claude
- https://code.claude.com/docs/en/whats-new/2026-w28
- https://github.com/anthropics/claude-code/releases

**竞品 / 行业**
- https://apidog.com/blog/gpt-5-6-codex/
- https://thenewstack.io/openai-codex-work-atlas/
- https://www.implicator.ai/openai-folds-codex-into-chatgpt-as-atlas-gets-august-9-deprecation-target/
- https://devops.com/cognition-ai-to-acquire-windsurf-after-google-licensing-deal/
- https://www.bighatgroup.com/blog/codex-weekly-2026-07-10/

**GitHub Trending**
- https://github.com/trending?since=daily
- https://github.com/trending?since=daily&spoken_language_code=zh

**UI/UX 设计 Agent**
- https://github.com/gainshin/Agentic-UX-Design_Builder
- https://github.com/nexu-io/open-design
- https://github.com/aiatelie/ai-atelie
- https://github.com/ilya-makarov-dev/Reframe
- https://github.com/bryfar/buildev

**测试 Agent**
- https://github.com/ohanedan/playwright-testgen
- https://github.com/shruthikj/sharingan-autotest
- https://github.com/Spirizeon/lemonx
- https://github.com/FSoft-AI4Code/TestWeaver

**视频自动化**
- https://github.com/calesthio/OpenMontage
- https://github.com/itsjwill/vanta
- https://github.com/MeiGen-AI/X-Cut
- https://github.com/haidrrrry/claude-remotion-skill

**vibe coding 反思**
- https://www.kunalganglani.com/blog/vibe-coding-best-practices-2026
- https://snehbavarva.medium.com/secure-vibe-coding-in-2026-the-files-prompts-and-rules-of-use-and-research-e821021ee908
- https://domino.ai/blog/agentic-engineering-practitioners-playbook
- https://www.mindstudio.ai/blog/code-with-claude-2026-new-agent-features
