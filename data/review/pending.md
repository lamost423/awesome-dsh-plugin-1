# 待审核仓库 / Pending review

> 新增到 `dsh-plugin` Topic 下、带有简介、尚未经维护者核实的仓库。本文件由 `scripts/update.mjs` 每日刷新，仅供审核使用，不是用户可见页面。
>
> Repositories newly added to the `dsh-plugin` topic that the maintainer has not verified yet. Refreshed daily by `scripts/update.mjs`; review-only, not a user-facing page.

- 生成时间 / Generated: **2026-09-04**
- 快照日期 / Snapshot date: **2026-09-04 (UTC)**
- 待审核 / Pending: **1985**
- 从快照消失的已核准仓库 / Approved repositories missing from the snapshot: **424**

审核决定记到数据文件后运行 `node scripts/merge.mjs` 生效：

- 通过 → 加入 [data/approved.json](../approved.json)（`"owner/name": "YYYY-MM-DD"`）
- 剔除 → 加入 [data/curated.json](../curated.json) 的 `excluded_repos`，理由只写「不是 DSH 插件 + 它是什么」，并同步从 `approved.json` 移除
- 只进目录、不进榜单 → 加入 `approved.json` + `curated.json` 的 `leaderboard_exclusions`
- 非插件形态 / market 类（插件市场、商店、技能商城、内置市场的桌面端等）→ 加入 `curated.json` 的 `market_exclusions`（市场不能包含市场）
- 目录站 / awesome-list / 榜单站（如 `awesome-dsh-plugin*` 系列）→ `excluded_repos` 整体剔除，不留目录

完整约定见 [data/review/README.md](./README.md)。

Record decisions in the data files, then run `node scripts/merge.mjs`:

- Approve → add to [data/approved.json](../approved.json) (`"owner/name": "YYYY-MM-DD"`)
- Exclude → add to `excluded_repos` in [data/curated.json](../curated.json) — the reason just states "not a DSH plugin + what it is" — and remove it from `approved.json`
- Catalog-only (not in the board) → add to `approved.json` + `leaderboard_exclusions` in `curated.json`
- Non-plugin form / market class (plugin market, store, skill mall, desktop with a built-in market) → `market_exclusions` in `curated.json` (the market cannot include another market)
- Directory sites / awesome-lists / leaderboards (e.g. the `awesome-dsh-plugin*` family) → `excluded_repos` outright

See [data/review/README.md](./README.md) for the full convention.

| # | Project | Stars | Created | First seen | Description |
| ---: | --- | ---: | --- | --- | --- |
| 1 | [plastic-labs/honcho](https://github.com/plastic-labs/honcho) | 7017 | 2023-09-10 | 2026-09-02 |  Memory library for building stateful agents |
| 2 | [anbeime/skill](https://github.com/anbeime/skill) | 6196 | 2026-02-02 | 2026-09-01 | 收录最全、更新最快的技能Skills商店：精选原创技能包（涵盖文档处理、内容创作、编程开发、机器学习、自动化工作流），全部打包好可直接安装使用！同时自动抓取GitHub上万个Skills项目，按分类、更新时间、Star数量整理。The most comprehensive and frequently updated AI Agent skill library, featuring curated skill packs across document processing, content creation, programming, machine learning, automated workflows, and many more domains. |
| 3 | [huangruiteng/loopx](https://github.com/huangruiteng/loopx) | 5600 | 2026-05-31 | 2026-08-31 | Long-horizon agent control plane for durable, governed work across Codex, Claude Code, and other harnesses. |
| 4 | [chuspeeism/dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) | 2932 | 2026-07-24 | 2026-08-29 | 现代化可灵活嵌入的任务面板，支持 Codex、DeepSeek Harness |
| 5 | [AdamPlatin123/dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1445 | 2026-08-04 | 2026-08-28 | DSH Plugin Radar — 开源 DSH 插件生态雷达：自动发现 15900+ 候选、k8s 运行级实测 10000+、15 分钟快照管线；插件目录是其自动生成的 artifact |
| 6 | [Unclecheng-li/AI_Animation](https://github.com/Unclecheng-li/AI_Animation) | 1225 | 2026-04-11 | 2026-08-29 | 本项目整理了用于生成[炫酷 HTML 动画网页]的 AI Prompts，涵盖动画效果、3D 可视化、PPT 风格演示、UI 美化等多个类别。 |
| 7 | [OpenPetsHQ/openpets](https://github.com/OpenPetsHQ/openpets) | 1163 | 2026-05-04 | 2026-09-03 | Local first, desktop companion platform with animated pets, plugin SDK and coding-agent integrations. |
| 8 | [platonai/Browser4](https://github.com/platonai/Browser4) | 1122 | 2018-03-12 | 2026-08-27 | Browser4 — an AI-native browser engine for autonomous agents, intelligent extraction, and large-scale web automation. |
| 9 | [Tiger3807861189/GLM-5.3-Flash-J-Space-Capability-Realization-Report](https://github.com/Tiger3807861189/GLM-5.3-Flash-J-Space-Capability-Realization-Report) | 1023 | 2026-08-16 | 2026-09-02 | GLM-5.3-Flash × J-Space capability realization — benchmark presentation of the J-Space Cognition Suite |
| 10 | [Minglink/dsh-infinite-gen-3](https://github.com/Minglink/dsh-infinite-gen-3) | 965 | 2026-08-15 | 2026-08-31 | DeepSeek 专用破甲插件「无限三代」dsh-infinite-gen-3 — armor-breaking plugin for DeepSeek，破甲版：稳定化破甲，求 Star 收藏 ⭐ |
| 11 | [wecode-ai/Wegent](https://github.com/wecode-ai/Wegent) | 781 | 2026-01-10 | 2026-08-30 | Plan, build, and deliver with an open-source, self-hostable AI workspace for coding, collaboration, and automation. |
| 12 | [myYangyunfan/dsh_desktop](https://github.com/myYangyunfan/dsh_desktop) | 631 | 2026-08-13 | 2026-08-30 | DeepSeek Harness (dsh) Windows desktop client - bundled Node.js + dsh CLI, one-click launch |
| 13 | [inclusionAI/Avernet](https://github.com/inclusionAI/Avernet) | 533 | 2026-07-06 | 2026-09-03 | Distributed agent coordination platform where agents live, connect, coordinate, execute, and evolve together. |
| 14 | [YuJunZhiXue/dsh-purge](https://github.com/YuJunZhiXue/dsh-purge) | 343 | 2026-08-19 | 2026-09-01 | DeepSeek Harness 破甲：让所有模型都能破甲，不同模型可换不同提示词；默认提示词面向国模「小码酱」。Jailbreak for every model — swap prompts per model. 求 Star 收藏 ⭐ |
| 15 | [pax-beehive/dsh-hub-cli](https://github.com/pax-beehive/dsh-hub-cli) | 215 | 2026-08-25 | 2026-09-02 | Open-source CLI, schemas, resolver, and DSH agent tools for DSH Plugin Hub |
| 16 | [leenkcool/Blue-Whale-Harness](https://github.com/leenkcool/Blue-Whale-Harness) | 192 | 2026-08-13 | 2026-09-01 | 🐋 DeepSeek Harness 插件总目录 · The catalog of DSH plugins：1958 个仓库 / 1819 个真插件（Skills · MCP · Tools · UI · Orchestration），中英文搜索、分类筛选、STAR 排序 → leenkcool.github.io |
| 17 | [liguobao/ds-harness-remote](https://github.com/liguobao/ds-harness-remote) | 162 | 2026-08-14 | 2026-08-30 | 一个基于 DeepSeek Harness 插件机制构建的多端远程访问方案，通过安全、低延迟、端到端加密的 P2P 优先网络，支持从 PC、Android 和 Web 随时访问并操作远程 Harness。 (A multi-device remote access solution built on the DeepSeek Harness plugin system, enabling PC, Android, and Web clients to securely access and operate a remote Harness over a low-latency, end-to-end encrypted, P2P-first network.) |
| 18 | [theBigGavin/marketingdashboard](https://github.com/theBigGavin/marketingdashboard) | 151 | 2026-07-17 | 2026-08-30 | 面向金融与产业研究的一屏式实时行情大屏：A股/港股/美股指数、大宗商品、美债收益率、板块热点、主力资金流、7×24 快讯、产业链自选股、AI 大模型 Token 追踪。A real-time market research cockpit on a single screen: CN/HK/US indices, commodities, treasury yields, sector hotspots, capital flows, 7×24 news, industry-chain watchlists and AI token usage trends.  |
| 19 | [LivXue/dsh-plugin-shop](https://github.com/LivXue/dsh-plugin-shop) | 143 | 2026-08-25 | 2026-09-03 | The most comprehensive DeepSeek Harness plugin market — refreshed daily, sourced across the Internet, reviewed before publishing. |
| 20 | [Justin-sky/ai-art-engine](https://github.com/Justin-sky/ai-art-engine) | 119 | 2026-07-24 | 2026-08-31 | AI 艺术创作引擎，专业的短视频创作工具 |
| 21 | [fangqian616/consensus-pipeline](https://github.com/fangqian616/consensus-pipeline) | 117 | 2026-07-16 | 2026-08-30 | Multi-agent department framework for long-form complex tasks, fighting AI hallucination, validated on academic research. 共识管线：多智能体部门长线任务解决框架，对抗AI幻觉，以学术研究为验证场景。 |
| 22 | [xing-shuyin/pi-web-ui](https://github.com/xing-shuyin/pi-web-ui) | 96 | 2026-08-04 | 2026-09-02 | dsh / pi-agent web ui |
| 23 | [zhu1090093659/dsh-trading](https://github.com/zhu1090093659/dsh-trading) | 92 | 2026-08-30 | 2026-09-03 | Agent-native trading terminal built on DeepSeek Harness. Crypto, US, CN and HK in one three-column GUI, 19+ hot-swappable connectors, dry-run by default with human approval on every live order. BYOK, no data redistribution. |
| 24 | [justlovemaki/PrismFlowAgent](https://github.com/justlovemaki/PrismFlowAgent) | 88 | 2025-10-11 | 2026-09-03 | 全栈资讯处理与 AI Agent 系统。它能够自动化地从全球多源渠道抓取高质量资讯，利用顶级大语言模型进行深度总结，并将其分发至多种终端 |
| 25 | [Jackywxsz/DSH-Creator](https://github.com/Jackywxsz/DSH-Creator) | 87 | 2026-08-25 | 2026-08-27 | Jacky Creator：面向内容创作者的 DeepSeek Harness 本地内容与运营工作台 |
| 26 | [lamost423/dsh-maze](https://github.com/lamost423/dsh-maze) | 65 | 2026-08-18 | 2026-08-27 | DeepSeek Harness 的执行迷宫——看 Agent 真实怎么干活：迷宫时间轴 · 数据轨道 · 确定性执行分析 · 多会话对比 \| The execution maze for DSH agents: maze timeline, per-step data tracks, deterministic execution analysis, multi-session comparison. Formerly dsh-trace-compare. |
| 27 | [SiriusNEO/StarAgent](https://github.com/SiriusNEO/StarAgent) | 56 | 2026-05-29 | 2026-09-02 | Lightweight agent multiplexer, all in one Web dashboard  |
| 28 | [HakureiMonika/dsh-sandbox-escalation-fix](https://github.com/HakureiMonika/dsh-sandbox-escalation-fix) | 45 | 2026-08-16 | 2026-08-28 | Session-aware sandbox escalation compatibility plugin for DeepSeek Harness/DSH第三方模型会话沙箱升级兼容插件 |
| 29 | [niuhuoshan/launch-wechat-miniprogram](https://github.com/niuhuoshan/launch-wechat-miniprogram) | 45 | 2026-08-11 | 2026-08-31 | 面向完全新手的微信小程序 Agent Skill，从需求确认、原生 UI 和高保真原型，到 AppID、备案、开发测试、腾讯云后台、体验版、提审、发布及版本更新。 |
| 30 | [huaweicloud/huaweicloud-devkit](https://github.com/huaweicloud/huaweicloud-devkit) | 44 | 2026-07-28 | 2026-09-02 |  Official Huawei Cloud plugin for AI agents — skills, MCP tools, safety guardrails, and cloud sandbox to help AI agents build, deploy, and operate on Huawei Cloud securely. |
| 31 | [KongFangXun/sofagent](https://github.com/KongFangXun/sofagent) | 42 | 2026-06-18 | 2026-09-01 | FDE Harness: audit-first governance for AI coding agents — 24 rules, HMAC chain, snapshot rollback (80 tools, 13 plugins) |
| 32 | [extracurricular-ai/dsh-filesnap](https://github.com/extracurricular-ai/dsh-filesnap) | 41 | 2026-08-27 | 2026-08-27 | dsh-filesnap — 把对话和它改过的文件一起回退到某一轮之前,不需要 git 仓库. A blazing-fast rewind and redo plugin for DeepSeek Harness, powered by a 🦀 Rust core, tracking the conversion and the files it changed, no git required, low disk consumption |
| 33 | [Axiaohungry/dsh-llm-workbuddy](https://github.com/Axiaohungry/dsh-llm-workbuddy) | 29 | 2026-08-14 | 2026-09-03 | 在deepseek harness中使用workbuddy api，因为公司只提供workbuddy积分 |
| 34 | [SuperJJ007/papermachine](https://github.com/SuperJJ007/papermachine) | 29 | 2026-08-24 | 2026-09-04 | The AI analyst that shows its work. Runs Python and R on your own machine, and traces every chart back to the code behind it. |
| 35 | [Jimmy0123-ux/dsh-token-pet](https://github.com/Jimmy0123-ux/dsh-token-pet) | 28 | 2026-09-01 | 2026-09-01 | DeepSeek Harness Desktop 悬浮用量小宠物：12 个正式逐帧动作反馈请求、工具、上下文压缩、归档与提示词增强；展示实时上下文占用、跨会话 Lifetime Ledger、服务商/模型统计和小时 Token 趋势；支持可编辑提示词增强、拖拽缩放、低性能模式与后台增量索引。 |
| 36 | [FrankHu-HK/mnemosyne](https://github.com/FrankHu-HK/mnemosyne) | 27 | 2026-08-10 | 2026-08-27 | Mnemosyne OS 7.0.0 — zero-dependency, local-first AI memory system (MCP / API / CLI / Python). MIT. |
| 37 | [See-Sol-Lab/DeepSeekGUI](https://github.com/See-Sol-Lab/DeepSeekGUI) | 27 | 2026-08-17 | 2026-08-27 | A Windows desktop client for DeepSeek Harness. V1 wraps the official Web UI; v2 (independent workbench) in development. |
| 38 | [Amakurai/dsh-liketavern](https://github.com/Amakurai/dsh-liketavern) | 25 | 2026-08-19 | 2026-09-04 | A DeepSeek Harness (dsh) plugin — turns dsh web into a SillyTavern-style roleplay frontend: character cards, prompt presets, lorebooks, personas, BM25 long-term memory, world-state deltas, and rollback-able floor operations, all on the dsh agent runtime. |
| 39 | [Kihara777/NixKits](https://github.com/Kihara777/NixKits) | 25 | 2026-03-28 | 2026-09-03 | 软件、补丁、NixOS 模块与 AI 编码助手的技能合集。 |
| 40 | [tnnevol/fn-os-apps](https://github.com/tnnevol/fn-os-apps) | 25 | 2026-05-15 | 2026-09-01 | 飞牛 fnOS 应用 Monorepo |
| 41 | [SepineTam/cnki-mcp](https://github.com/SepineTam/cnki-mcp) | 24 | 2026-07-03 | 2026-09-01 | An MCP server for reach CNKI.  |
| 42 | [FishBottle7/opencode2dsh](https://github.com/FishBottle7/opencode2dsh) | 23 | 2026-08-29 | 2026-08-29 | DSH plugin — free OpenCode Zen models for DeepSeek Harness (DSH). Free LLM API, no API key needed. 在 DSH 中使用 OpenCode Zen 免费模型，无需 API key |
| 43 | [opdsh/unity-plugin](https://github.com/opdsh/unity-plugin) | 21 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: control the Unity Editor through the unity CLI |
| 44 | [GZX2211/dsh-Visual-Workflow](https://github.com/GZX2211/dsh-Visual-Workflow) | 20 | 2026-08-15 | 2026-09-01 | 专为 DeepSeek Harness Web GUI 打造的可视化多 Agent 工作流编排插件。公开测试版已上线！接下来会随着 DSH 的正式版上线一并发布正式版！ |
| 45 | [sagirimo/BioDSH](https://github.com/sagirimo/BioDSH) | 20 | 2026-08-31 | 2026-09-01 | The bioinformatics agent desktop for clinicians and wet-lab scientists — built on DeepSeek Harness. One-click installers, a skill store, offline mode. |
| 46 | [Suiwan/whale-purse](https://github.com/Suiwan/whale-purse) | 19 | 2026-08-14 | 2026-08-30 | A cute whale desktop pet for DeepSeek Harness that keeps an eye on your DeepSeek balance and session usage/cost. Drag her anywhere, click to open a live panel with real-time spend, peak/off-peak pricing, budget alerts, and history trends. |
| 47 | [Ed-Marcavage/awesome-security-agent-harnesses](https://github.com/Ed-Marcavage/awesome-security-agent-harnesses) | 18 | 2026-08-03 | 2026-08-30 | AI agents for pentesting, code audit, fuzzing, vulnerability discovery, and reverse engineering — harnesses, sandboxes, security MCP servers, benchmarks, and evals. |
| 48 | [chumingjun/dsh-harness-one](https://github.com/chumingjun/dsh-harness-one) | 17 | 2026-08-20 | 2026-08-27 | Visual AI workflow orchestrator for DeepSeek Harness (dsh): multi-agent DAGs, live execution, recovery, and Feishu integration. |
| 49 | [liangdabiao/dsh-plugin-developer-skill](https://github.com/liangdabiao/dsh-plugin-developer-skill) | 16 | 2026-09-01 | 2026-09-01 | dsh-plugin-developer — DeepSeek Harness 插件开发 Skill  > 指导 AI Agent 从 0 到 1 开发、构建、安装、测试 DeepSeek Harness（dsh）插件。基于 **dsh 0.1.1-rc.2** 与 dsh-openmaic 项目的完整实战经验，并内置一个**已通过 web 界面实测**的天气插件作为整包参考案例。  ## 这是什么  dsh 采用"无特权内核、万物皆插件"的设计：模型适配器、工具注册表、Agent 循环、网页界面都是插件 |
| 50 | [maxwell-feng/dsh-tinyfish-search](https://github.com/maxwell-feng/dsh-tinyfish-search) | 15 | 2026-08-30 | 2026-08-30 | TinyFish-backed web search provider for DeepSeek Harness (ctx.web) — 将内置 web_search 接入 TinyFish Search API 的 DeepSeek Harness 插件 |
| 51 | [NekroAI/nekro-nxt](https://github.com/NekroAI/nekro-nxt) | 15 | 2026-08-15 | 2026-08-27 | NekroNXT：基于 DeepSeek Harness（DSH）的多平台群聊智能体系统｜A DSH-powered multi-platform group-chat agent system |
| 52 | [null119/dsh-mcp-manage](https://github.com/null119/dsh-mcp-manage) | 15 | 2026-08-17 | 2026-08-30 | DSH（DeepSeek Harness）Web GUI 插件：在设置页管理 MCP 服务器——列出已安装工具，添加/编辑/删除、启用/停用；组合配置提供的 MCP 同样可在运行时直接编辑、停用、移除并恢复，无需重启宿主。 |
| 53 | [jingyunstudio/jingyun-dsh](https://github.com/jingyunstudio/jingyun-dsh) | 14 | 2026-08-27 | 2026-08-29 | 基于 Jingyun Studio + DeepSeek Harness (DSH) 打造的一站式 AI 商业化桌面客户端 |
| 54 | [ddtcorex/govard](https://github.com/ddtcorex/govard) | 13 | 2026-02-08 | 2026-08-28 | Go-based local development orchestrator for Magento, Laravel, Symfony, Next.js, WordPress, and more. Docker stacks, SSL, Xdebug, and a desktop dashboard. |
| 55 | [awesome-deepseekharness/awesome-deepseek-harness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness) | 11 | 2026-08-15 | 2026-08-27 | Awesome DeepSeek Harness (dsh) — curated awesome list of plugins, tools, skills & resources. Everything is a plugin. |
| 56 | [justhalfbit/dsh-plugin-memory](https://github.com/justhalfbit/dsh-plugin-memory) | 11 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 跨会话记忆插件：对话模型边干边记的 Markdown 项目记忆，支持专题文件渐进式披露、可选后台静默蒸馏、按项目隔离与热更新设置面板。机制对齐 Claude Code auto memory。 \| Agent-maintained cross-session Markdown memory: progressive-disclosure topic files, opt-in silent distillation, per-project isolation. Claude Code-aligned. |
| 57 | [fb0sh/dsh-pentester](https://github.com/fb0sh/dsh-pentester) | 10 | 2026-08-19 | 2026-08-29 | 基于 DeepSeek Harness 的多 Agent PTES 渗透测试编排插件，支持自动化侦察、漏洞分析、验证与报告，使用 Docker/Kali 隔离工具箱 \| Multi-agent PTES penetration testing plugin for DeepSeek Harness with automated recon, vulnerability analysis, validation, reporting, and Docker/Kali toolbox |
| 58 | [LaoYueHanNi/dsh-token-usage](https://github.com/LaoYueHanNi/dsh-token-usage) | 10 | 2026-08-14 | 2026-08-27 | 贴近 DSH 原生设计风格的 token 用量统计插件：实时记录每次请求的用量与费用，在 Web UI 中提供趋势图表、按模型定价明细和供应商配额显示。 |
| 59 | [Minglink/dsh-stream-market](https://github.com/Minglink/dsh-stream-market) | 10 | 2026-09-04 | 2026-09-04 | DeepSeek Harness 内置可视化插件市场 — 极速秒开、官方 dsh:// 联动、深度本地管理与原子化彻底卸载 |
| 60 | [Qian-Ning/prompt-skill-armory](https://github.com/Qian-Ning/prompt-skill-armory) | 10 | 2026-08-27 | 2026-08-30 | Managing prompts，, skills, MCP tools & wallpaper for DeepSeek Harness |
| 61 | [tinqiao-oss/clawtouch-mcp](https://github.com/tinqiao-oss/clawtouch-mcp) | 10 | 2026-06-01 | 2026-08-29 | ClawTouch MCP server — exposes a real USB-HID keyboard/mouse (Raspberry Pi Pico 2) as Model Context Protocol tools for any LLM agent. MIT. |
| 62 | [chen731215-dev/dsh-tavern-v2](https://github.com/chen731215-dev/dsh-tavern-v2) | 9 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Tavern Plugin - character card roleplay, worldbook management, preset switching, dark theme, memory summary, relationship graph, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 63 | [goatliamia/dsh-runtime-react](https://github.com/goatliamia/dsh-runtime-react) | 9 | 2026-08-31 | 2026-09-02 | 不要让 Model 为确定性问题反复思考，也不要让 Harness 为不确定的问题假装知道答案 |
| 64 | [imsai-sh/dsh-1024store](https://github.com/imsai-sh/dsh-1024store) | 9 | 2026-08-24 | 2026-08-27 | DeepSeek Harness plugin store, marketplace and hub — 11,000+ dsh plugins with search, rankings, install commands and a free public API. DeepSeek Harness 插件市场 / 插件商店：自动收集与格式校验，免费搜索 API。deepseek1024.com |
| 65 | [keman-ai/dsh-skin-market](https://github.com/keman-ai/dsh-skin-market) | 9 | 2026-08-18 | 2026-08-27 | Skin marketplace for DeepSeek Harness — search and install community skins from dsh.a2hmarket.ai right in the settings page |
| 66 | [maxwell-feng/dsh-windows-ocr](https://github.com/maxwell-feng/dsh-windows-ocr) | 9 | 2026-08-15 | 2026-09-01 | dsh plugin: OCR attached images locally with the built-in Windows OCR engine — text-only models can see, privacy-first |
| 67 | [cloveric/tarocub](https://github.com/cloveric/tarocub) | 8 | 2026-04-08 | 2026-08-29 | Feishu/Lark-first local AI agent gateway and native DeepSeek Harness plugin for Codex, Claude Code, Kimi Code, DeepSeek Harness, and Antigravity; Telegram optional. |
| 68 | [greenthree/ProbHub-skill](https://github.com/greenthree/ProbHub-skill) | 8 | 2026-05-25 | 2026-08-30 | 算法竞赛出题自动化skill（个人出题习惯），支持完善题面、构造数据、组卷用typ编译pdf和生成domjudge题目包 |
| 69 | [jiazz197-cmyk/omd-dsh](https://github.com/jiazz197-cmyk/omd-dsh) | 8 | 2026-08-23 | 2026-08-29 | Multi-mode agent presets for DeepSeek Harness — per-mode model routing + tiered subagent delegation. |
| 70 | [Ramenne/DeepSeek-Harness-Gov](https://github.com/Ramenne/DeepSeek-Harness-Gov) | 8 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 政务版：基于 deepseek-ai/deepseek-harness 的政务办事 WebUI 与红头公文插件 |
| 71 | [Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl](https://github.com/Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl) | 8 | 2026-08-29 | 2026-08-31 | DeepSeek Harness（DSH）Web 界面右下角的常驻余额挂件。基于 MeteorNOX/DeepSeek-Balance-Whale-Widget 修改的铁盆鲸鱼娘版。 |
| 72 | [yu-wenchao/dsh-free-models-hub](https://github.com/yu-wenchao/dsh-free-models-hub) | 8 | 2026-08-26 | 2026-08-27 | 免费模型排行榜 · DeepSeek Harness 社区插件，在 DeepSeek Harness (DSH) Web UI 左侧边栏提供「免费模型榜」：分页浏览（每页 20 条、页码窗口、首页/末页）、 点击标题展开 API 调用地址 / 模型名称 / 【点击这里申请免费密钥key】按钮， 并支持一键配置到 设置 → 模型 → 自定义提供方 —— 用户只需自行粘贴免费 API Key |
| 73 | [AngelosZou/graphlint](https://github.com/AngelosZou/graphlint) | 7 | 2026-07-01 | 2026-08-27 | Dead-code detection for AI-generated codebases: graphlint builds a dependency graph, finds code unreachable from any entry point to enable codebase cleanup and functional‑effectiveness understanding. |
| 74 | [BertramWang12399/dsh-projects-mode](https://github.com/BertramWang12399/dsh-projects-mode) | 7 | 2026-08-27 | 2026-09-01 | Project mode plugin for DSH Web GUI: sidebar entry, full-screen project manager, live per-project context injection (instructions + refreshable memory), session badge |
| 75 | [cryjkd/dsh-clawbot](https://github.com/cryjkd/dsh-clawbot) | 7 | 2026-09-03 | 2026-09-03 | 在 DeepSeek Harness（DSH）里接入微信官方 ilink 机器人网关：扫码绑定后，AI 能主动给自己发微信通知；每次回复后自动推送任务完成摘要；目标完成/阻断时自动通知；需要批准/选择时主动微信提醒。自带设置界面（设置 → ClawBot：扫码二维码、微信在线/断线状态、手动发送、三个自动通知开关、监听开关、解除绑定、自定义图标）。  底层走腾讯官方 ilink 网关（https://ilinkai.weixin.qq.com），无第三方破解、无自建中转，消息只发给绑定的账号自己。 |
| 76 | [PeterTXPan/dsh-unreal-mcp](https://github.com/PeterTXPan/dsh-unreal-mcp) | 7 | 2026-08-25 | 2026-08-31 | DeepSeek Harness Bundle for Unreal Engine 5.8 via Unreal MCP |
| 77 | [RiemannRe3/DSH-RolePlay](https://github.com/RiemannRe3/DSH-RolePlay) | 7 | 2026-08-25 | 2026-08-27 | DeepSeek Harness 的 Tavern 角色卡兼容与原生 Agent RolePlay 插件。 |
| 78 | [wanderer-yk/dsh-xueqiu](https://github.com/wanderer-yk/dsh-xueqiu) | 7 | 2026-08-14 | 2026-09-03 | 雪球 mini 行情面板 — DeepSeek Harness 免登录 A股/港美股实时行情、K线、分时、热榜、7x24快讯。可拖拽悬浮面板，交易时段智能刷新。 |
| 79 | [wbin0001/dsh-comfyui-canvas](https://github.com/wbin0001/dsh-comfyui-canvas) | 7 | 2026-08-31 | 2026-09-02 | DSH+ComfyUI画布插件dsh-comfyui-canvas embeds your ComfyUI instance as a split-screen canvas inside DeepSeek Harness Web. The agent writes prompts and edits nodes right in chat, applies them live to the canvas you're watching, and turns ideas into images, video, and 3D — all without switching front-ends. |
| 80 | [HuaJi2077/empty-fort-strategy](https://github.com/HuaJi2077/empty-fort-strategy) | 6 | 2026-08-29 | 2026-08-29 | DSH插件，感受空城计的巧妙，消耗多余的Token。 |
| 81 | [JopenChen/dsh-go](https://github.com/JopenChen/dsh-go) | 6 | 2026-08-30 | 2026-08-31 | dsh-go 是一个纯 Go、进程内的 DeepSeek Harness Agent 实现 —— 让任意 Go 后端能以内嵌库的方式直接获得一个等价、具备规划能力的 Agent，无需界面、无需独立运行时。它不是又一个 ReAct 骨架，而是对 DSH 全量能力接缝的系统级复刻。 |
| 82 | [LaoYueHanNi/dsh-git-worktree](https://github.com/LaoYueHanNi/dsh-git-worktree) | 6 | 2026-08-16 | 2026-08-30 | 在 Web 界面进行分支切换与 git worktree 隔离的 DSH 插件 |
| 83 | [liangyou09/lyshell-archive](https://github.com/liangyou09/lyshell-archive) | 6 | 2026-08-12 | 2026-09-04 | AI-native terminal & SSH client — Harness launches DeepSeek / CodEx / Claude agents on PowerShell 7 in TUI or embedded Web UI, plus SFTP, serial/Telnet and a built-in MCP server. |
| 84 | [liceses/dsh-workspace-tree](https://github.com/liceses/dsh-workspace-tree) | 6 | 2026-08-18 | 2026-08-30 | 把 DSH Web 左侧栏的「工作区」重做为文件系统树双模式。核心原则： 工作区 = 目录强绑定——会话的 cwd 就是它所在的目录，环境真正隔离。 |
| 85 | [lw-storm/dsh-plugin-masterprompt](https://github.com/lw-storm/dsh-plugin-masterprompt) | 6 | 2026-08-27 | 2026-08-28 | This plugin is used for custom persona configuration. It facilitates users in code development and customized‑role setup, and supports flexible persona adjustments for each conversation. |
| 86 | [ParticleLight/dsh-all-usage](https://github.com/ParticleLight/dsh-all-usage) | 6 | 2026-08-17 | 2026-08-29 | DeepSeek Harness 用量看板 / Usage dashboard: tokens, cache, model/provider/workspace analytics, DeepSeek balance, heatmap, and CSV export. |
| 87 | [ppy-web/dsh-plugin-xiaomi-mimo-tts](https://github.com/ppy-web/dsh-plugin-xiaomi-mimo-tts) | 6 | 2026-08-20 | 2026-08-28 | 给DSH接入免费的 Xiaomi MiMo TTS API，支持使用预置/自定义/浏览器内置声音朗读正文 |
| 88 | [rogerdigital/dsh-searxng](https://github.com/rogerdigital/dsh-searxng) | 6 | 2026-08-16 | 2026-08-29 | DeepSeek Harness (dsh) plugin that adds a SearXNG-backed web_search provider to the ctx.web seam — free, self-hosted, key-less search instead of paid Exa/Perplexity APIs. |
| 89 | [WongYuYe/dsh-appshots](https://github.com/WongYuYe/dsh-appshots) | 6 | 2021-06-16 | 2026-09-04 | Codex-style Appshots for DSH Desktop: capture the frontmost macOS window and attach it to the current chat. |
| 90 | [xiaosurongjia/dsh-improved-inline-edit](https://github.com/xiaosurongjia/dsh-improved-inline-edit) | 6 | 2026-08-28 | 2026-08-29 |  当你的DSH正在工作时，你可以不用停止对话就可以再次提出要求 |
| 91 | [Drhushi/dsh-plugin-tav2](https://github.com/Drhushi/dsh-plugin-tav2) | 5 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 插件 —— 对话式游戏本地化：跟 AI 助手说说话，完成游戏翻译全流程。引擎适配器架构，首发支持 Ren'Py。 |
| 92 | [flymysql/dsh-memory](https://github.com/flymysql/dsh-memory) | 5 | 2026-08-14 | 2026-08-30 | DeepSeek Harness 跨会话记忆库：memory_remember/recall/forget 三个工具 + 系统提示注入，agent 持久化记忆 |
| 93 | [Gru110110110/dsh-launcher](https://github.com/Gru110110110/dsh-launcher) | 5 | 2026-08-16 | 2026-09-02 | 让 DeepSeek Harness 人人可用的桌面入口——不用 Node、不用命令行，双击即用，还无损跟随每次官方更新。支持MacOs和Windows。DeepSeek Harness, for everyone. No Node.js. No command line. Just double-click and go. Always in step with every official update. For macOS & Windows. |
| 94 | [guoxiucai/dsh-code](https://github.com/guoxiucai/dsh-code) | 5 | 2026-08-16 | 2026-08-28 | pi tui  style code agent base on deepseek harness |
| 95 | [jukanntenn/grill-me-sleek](https://github.com/jukanntenn/grill-me-sleek) | 5 | 2026-05-28 | 2026-09-01 | Stress-test your plan before vibe coding. The AI asks you questions to build a shared understanding — you answer in a sleek web UI. |
| 96 | [keman-ai/dsh-skin-pack](https://github.com/keman-ai/dsh-skin-pack) | 5 | 2026-08-26 | 2026-08-27 | A full set of skins for DeepSeek Harness — one repository, each theme installable on its own |
| 97 | [maxwell-feng/dsh-tesseract-ocr](https://github.com/maxwell-feng/dsh-tesseract-ocr) | 5 | 2026-08-15 | 2026-09-01 | dsh plugin: OCR attached images locally with Tesseract — text-only models can see, privacy-first |
| 98 | [recoluan/recowork](https://github.com/recoluan/recowork) | 5 | 2026-07-06 | 2026-08-27 | Give your AI a workflow. |
| 99 | [scotthuang/agent-knock-knock](https://github.com/scotthuang/agent-knock-knock) | 5 | 2026-05-15 | 2026-08-31 | Control local Codex and Claude Code from OpenClaw through shared tmux terminals, with seamless human-agent handoff. |
| 100 | [Shaky77/weiwen-law-dsh](https://github.com/Shaky77/weiwen-law-dsh) | 5 | 2026-08-19 | 2026-08-27 | 唯稳律 (Weiwen's Law) 白箱风控 DSH 插件 — DeepSeek Harness 因果约束中间件 |
| 101 | [tta-lab/organon](https://github.com/tta-lab/organon) | 5 | 2026-03-18 | 2026-08-30 | Structure-aware tools for AI agents. Tree-sitter code editing, web page navigation, search. No daemon, no JSON, just stdin. |
| 102 | [vibe-any/dsh-plugin-save-token](https://github.com/vibe-any/dsh-plugin-save-token) | 5 | 2026-08-27 | 2026-08-27 | A DeepSeek Harness (dsh) dynamic plugin that cuts token cost without cutting model intelligence |
| 103 | [VinciBeans/deepseek-plugin-liangwengu](https://github.com/VinciBeans/deepseek-plugin-liangwengu) | 5 | 2026-08-22 | 2026-08-31 | 梁文谷 DSH 插件：在 Web GUI 右上角显示当前算力错峰时段（已适配deepseek 2026.08.22 公布的最新峰谷收费政策，工作日 09:00–12:00 与 14:00–18:00 为梁文峰，其余时间含整个周末为梁文谷），并实时倒计时当前时段剩余时间；谷期跨天计算，直达下一工作日 09:00。 |
| 104 | [whutzefengxie-ops/dsh-shadow-mind](https://github.com/whutzefengxie-ops/dsh-shadow-mind) | 5 | 2026-08-24 | 2026-08-28 | Independent Shadow agent orchestration plugin for DeepSeek Harness |
| 105 | [xianrui69/dsh-quick-phrases](https://github.com/xianrui69/dsh-quick-phrases) | 5 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: quick-phrase chip bar above the composer + /-triggered phrase menu |
| 106 | [ai-eks/dsh-docking-layout](https://github.com/ai-eks/dsh-docking-layout) | 4 | 2026-08-21 | 2026-08-29 | Organize unlimited conversation tabs into editor-style, drag-to-split groups for DeepSeek Harness Web. |
| 107 | [AstroLiao/dsh-launcher](https://github.com/AstroLiao/dsh-launcher) | 4 | 2026-08-15 | 2026-09-01 | Windows launcher for DeepSeek Harness running in WSL2 (dsh) |
| 108 | [better-er/dsh-cache-billing](https://github.com/better-er/dsh-cache-billing) | 4 | 2026-08-28 | 2026-08-28 | DSH 缓存账单插件：上下文圆环弹层里实时算账，峰谷自动计价，第三方中转照常记账 |
| 109 | [better-er/dsh-edit-diff](https://github.com/better-er/dsh-edit-diff) | 4 | 2026-08-28 | 2026-08-28 | dsh·去重复 diff 展示插件 |
| 110 | [chengdb/dsh-plugin-capability-panel](https://github.com/chengdb/dsh-plugin-capability-panel) | 4 | 2026-08-21 | 2026-08-27 | 在 Web GUI 里可视化管理项目的全部能力——Skills、MCP 服务器、快捷消息， 全部支持项目级 / 全局级双作用域，全部可以不离开浏览器完成安装、启停与分发 |
| 111 | [dushaobindoudou/dsh-freeroute](https://github.com/dushaobindoudou/dsh-freeroute) | 4 | 2026-08-21 | 2026-08-27 | dsh free token route |
| 112 | [EasyTZ/dsh-desktop](https://github.com/EasyTZ/dsh-desktop) | 4 | 2026-08-20 | 2026-08-31 | Deepseek-Harness-Desktop |
| 113 | [elizax/dsh-http-proxy](https://github.com/elizax/dsh-http-proxy) | 4 | 2026-08-26 | 2026-08-27 | 支持设置LLM的代理地址 |
| 114 | [Icstick/dsh-adaptive-context](https://github.com/Icstick/dsh-adaptive-context) | 4 | 2026-08-27 | 2026-09-03 | DeepSeek Harness 的 AdaptiveContextPlane (ACP) 插件——带治理的长期记忆系统 |
| 115 | [iimaguest/phone-tunnel-pool](https://github.com/iimaguest/phone-tunnel-pool) | 4 | 2026-08-23 | 2026-08-28 | Refreshable Cloudflare quick-tunnel pool for the dsh web GUI — phone access with QR + embedded login |
| 116 | [ItBayMax/dsh-replay-theater](https://github.com/ItBayMax/dsh-replay-theater) | 4 | 2026-09-01 | 2026-09-01 | Replay a DeepSeek Harness session at its original token cadence — an in-app playback theater with play/pause/step/speed/seek. |
| 117 | [liyi3068238601-oss/dsh-comfyui-ctl](https://github.com/liyi3068238601-oss/dsh-comfyui-ctl) | 4 | 2026-08-31 | 2026-08-31 | Native DeepSeek Harness plugin for controlling ComfyUI queues, history, outputs, models, uploads, and generation. |
| 118 | [meyaomiao/dsh-server-deck](https://github.com/meyaomiao/dsh-server-deck) | 4 | 2026-08-26 | 2026-08-28 | 服务器卡片仪表盘 for DeepSeek Harness — card dashboard (status/CPU/mem/disk) + one-click xterm terminal, better-sidebar tab or standalone drawer |
| 119 | [ningbonb/dsh-client-ui-brand](https://github.com/ningbonb/dsh-client-ui-brand) | 4 | 2026-08-26 | 2026-08-27 | Custom product name and logo branding for DeepSeek Harness Web 自定义 DeepSeek Harness Web 端 logo 和产品名称 |
| 120 | [pgmi-builds/better-dsh](https://github.com/pgmi-builds/better-dsh) | 4 | 2026-08-16 | 2026-08-28 | Make your dsh ready for serious coding. (Tools x Schemas)^REPL. skill://, ctx://, agent://, dvc://, dsh://, IPython REPL, Context as Variables, cross compaction recallable, full context revive. hash-edit, dvc://browser, subagent as a function, workflow as a function. |
| 121 | [RexCue/dsh-wallpaper](https://github.com/RexCue/dsh-wallpaper) | 4 | 2026-08-14 | 2026-08-30 | Wallpaper skin for the DeepSeek Harness (dsh) web UI: image background with opacity, mask and blur controls. |
| 122 | [taoshi1999/dsh-workspace-hygiene](https://github.com/taoshi1999/dsh-workspace-hygiene) | 4 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin for agent workspace hygiene: artifact value assessment, metadata indexing, and auditable cleanup. |
| 123 | [TencentCloud/cloudq-for-dsh](https://github.com/TencentCloud/cloudq-for-dsh) | 4 | 2026-08-28 | 2026-09-03 | CloudQ integration for DeepSeek Harness, providing multi-cloud architecture governance, AIOps, risk inspection, usage, artifacts, and architecture views. |
| 124 | [tiphareth0/dsh-sshworkspaces](https://github.com/tiphareth0/dsh-sshworkspaces) | 4 | 2026-08-28 | 2026-08-31 | Workspace-level SSH remote development plugin for DeepSeek Harness: transparent seam-routed fs, git & terminal across multiple hosts and workspaces, with a built-in 4-column IDE and SSH ops toolkit. 提供工作区级 SSH 远程开发的Deepseek Harness插件：文件/Git/终端按工作区透明路由，支持多服务器多工作区并行开发，内置四列 IDE 与 SSH 运维工具。 |
| 125 | [wkscc310/dsh-client-ui-cpa-quota](https://github.com/wkscc310/dsh-client-ui-cpa-quota) | 4 | 2026-08-17 | 2026-08-30 | Easily view your CLiProxyAPI quota in DeepSeek Harness. |
| 126 | [WSL043/dsh-chat-manager](https://github.com/WSL043/dsh-chat-manager) | 4 | 2026-08-15 | 2026-08-27 | DeepSeek Harness chat history and session management: search archives, restore conversations, and delete safely. |
| 127 | [yailPeralta/ast-mcp-server](https://github.com/yailPeralta/ast-mcp-server) | 4 | 2026-08-03 | 2026-08-29 | Correctness-oriented MCP server and batch CLI for compact structural reads and reviewed TypeScript/JavaScript edits. |
| 128 | [yaoshuo530/dsh-prompt-enhancer](https://github.com/yaoshuo530/dsh-prompt-enhancer) | 4 | 2026-08-28 | 2026-08-28 | A prompt-enhancement plugin for DeepSeek Harness: an ✨ Enhance composer button that rewrites prompts with first-principles thinking using session context, and asks clarifying questions when key info is missing. |
| 129 | [yohanchen1/MathModelingAgent](https://github.com/yohanchen1/MathModelingAgent) | 4 | 2025-08-11 | 2026-09-02 | Closed-loop scientific modeling agent with evidence-backed verification and reproducible correction. |
| 130 | [Z-6354/dsh-version-autoupdate](https://github.com/Z-6354/dsh-version-autoupdate) | 4 | 2026-08-18 | 2026-08-28 | DSH version badge + one-click auto-update (dual-surface Cordis plugin) |
| 131 | [173787247/dsh-wsl-open](https://github.com/173787247/dsh-wsl-open) | 3 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: open WSL Linux paths from chat in Windows. |
| 132 | [9931666/dsh-plugin-roundtable](https://github.com/9931666/dsh-plugin-roundtable) | 3 | 2026-08-22 | 2026-08-29 | （roundtable V0.2.2）把一次 DeepSeek Harness 会话，从"你和 AI 一对一聊天"，升级成"你 + 主持人(DeepSeek) + 一圈专家 AI 开圆桌会 |
| 133 | [addozhang/dsh-discord](https://github.com/addozhang/dsh-discord) | 3 | 2026-08-30 | 2026-08-31 | Discord-first adapter for DeepSeek Harness — sessions, streaming, approvals and controls from a Discord guild. |
| 134 | [Aliuyanfeng/dsh-soul](https://github.com/Aliuyanfeng/dsh-soul) | 3 | 2026-08-31 | 2026-08-31 | The DeepSeek Harness Personalization Settings plugin is used to configure the nickname, response style, tone, and custom commands of the Agent. |
| 135 | [AnLifeX/dsh-credits](https://github.com/AnLifeX/dsh-credits) | 3 | 2026-08-17 | 2026-08-29 | DeepSeek Harness（dsh web）额度插件：跟随当前模型显示官方余额或 OpenCode Go 订阅用量，支持本会话估算、跨会话累计消耗与可视化设置。 |
| 136 | [Binaryinject/dsh-review-checkout](https://github.com/Binaryinject/dsh-review-checkout) | 3 | 2026-08-26 | 2026-08-28 | dsh-review-checkout |
| 137 | [CodermanYHZ/dsh-node-flow](https://github.com/CodermanYHZ/dsh-node-flow) | 3 | 2026-08-27 | 2026-08-27 | 节点式 DSH 工作流画布：编排子代理、代码、条件、循环与定时任务，支持模型路由与 AI 生成指南。 Node-mode DSH workflow canvas: orchestrate sub-agents, code, conditions, loops & scheduled tasks. |
| 138 | [Crosery/dsh-viewer](https://github.com/Crosery/dsh-viewer) | 3 | 2026-08-31 | 2026-08-31 | Everything renders: images, video, audio, PDF, Office documents and local web pages inline in the DeepSeek Harness web UI, via a display_file tool. |
| 139 | [dingminhua/dsh-connect-workbuddy](https://github.com/dingminhua/dsh-connect-workbuddy) | 3 | 2026-08-28 | 2026-08-30 | Connect locally signed-in WorkBuddy models to DeepSeek Harness with a read-only credits overview and model management. |
| 140 | [EL4CTEO/roblox-devforum-mcp](https://github.com/EL4CTEO/roblox-devforum-mcp) | 3 | 2026-03-30 | 2026-08-30 | Give your AI coding agent the Roblox DevForum and official creator docs — check if a bug is already known, read the accepted answer, and verify APIs before writing Luau. |
| 141 | [Fakek0f3sT/dsh-mcp-diff](https://github.com/Fakek0f3sT/dsh-mcp-diff) | 3 | 2026-08-27 | 2026-08-27 | Uniform diff cards for every file mutation in DeepSeek Harness Web — MCP filesystem (edit_file/write_file) and built-in edit/write, collapsed by default, with per-line highlighting |
| 142 | [FeatherHunter/dsh-im-companion](https://github.com/FeatherHunter/dsh-im-companion) | 3 | 2026-09-02 | 2026-09-04 | dsh-im 辅助插件（IM Companion）：以 Agent 为单位，把飞书/微信/QQ 机器人收进 DSH 工作区，左栏绿灯、一键过滤、舰队总览、拖拽搬家，卸载即净。 |
| 143 | [fengb3/dsh-session-icons](https://github.com/fengb3/dsh-session-icons) | 3 | 2026-08-22 | 2026-08-31 | DSH（DeepSeek Harness）Web 界面的会话标题图标插件：当模型为一次新会话生成标题时，宿主半用同一条路由发起一次辅助小请求，让模型按标题画一枚 24×24 单色 SVG 隐喻图标；浏览器半把它注入到左侧会话列表每行标题的左侧，跟随主题色。 |
| 144 | [fu827707013/dsh-concurrency-guard](https://github.com/fu827707013/dsh-concurrency-guard) | 3 | 2026-08-26 | 2026-08-27 | DSH（DeepSeek Harness）并发请求监控与门闩插件。 |
| 145 | [FylarOpen/fylar-deepseek-harness-office-editor](https://github.com/FylarOpen/fylar-deepseek-harness-office-editor) | 3 | 2026-09-02 | 2026-09-04 | Office document preview, editing, and DOCX generation for DeepSeek Harness, powered by Fylar Office SDK. |
| 146 | [GM-HZ/agent-dag-workflow](https://github.com/GM-HZ/agent-dag-workflow) | 3 | 2026-08-23 | 2026-08-29 | Host-neutral durable DAG workflows for Agents: CLI-native access, fixed MCP gateway, on-demand Skills, triggers, replay, and visual Canvas. |
| 147 | [gulagala001/dsh-trisoul](https://github.com/gulagala001/dsh-trisoul) | 3 | 2026-08-27 | 2026-08-27 | TriSoul —— 三魂共识 Agent：三个灵魂盲写+匿名互评，三官（对齐/博识/实证）补偿生成，画布式上下文，记忆中枢。DeepSeek Harness 插件套件，一键装/独立端口/一键卸载 |
| 148 | [gwsbhqt/dsh-insight](https://github.com/gwsbhqt/dsh-insight) | 3 | 2026-08-25 | 2026-08-27 | 洞察 — read-only insight panel for a DeepSeek Harness profile: where every plugin, service, tool and model came from, which config layer inserted or disabled it, and what is running right now. |
| 149 | [Haniubub/seo-toolkit](https://github.com/Haniubub/seo-toolkit) | 3 | 2026-08-29 | 2026-08-30 | The SEO audit toolkit built for DeepSeek Harness (DSH) — runs locally, no Claude Code, no API key required. Self-contained port of claude-seo v2.2.5: 53 Python scripts + 24 sub-skills + 18 agents, weighted score, gated fan-out, schema.org, E-E-A-T, GBP, GEO/AI Overviews. |
| 150 | [harryopo/dsh-cloud-workspaces](https://github.com/harryopo/dsh-cloud-workspaces) | 3 | 2026-08-14 | 2026-08-31 | Cloud workspaces for DeepSeek Harness — pick Cloud (SSH) in the workspace picker and the agent's bash/read/write/edit/glob/grep tools transparently run on your Linux server over SSH. Zero remote install. |
| 151 | [Hou-DL/dsh-token-pulse](https://github.com/Hou-DL/dsh-token-pulse) | 3 | 2026-08-24 | 2026-08-28 | Local Token heatmap plugin for DSH Web — GitHub-style calendar views, per-hour/week/month/quarter/year, fully local, zero billing. |
| 152 | [hr98w/dsh-memory](https://github.com/hr98w/dsh-memory) | 3 | 2026-09-01 | 2026-09-01 | 融合 Claude Code 的 Auto Memory 与 Codex 的 Session 记忆整理，为 DeepSeek Harness 提供简单、透明、上下文友好的长期记忆。Claude Code-inspired Auto Memory meets Codex-inspired Session consolidation, bringing simple, transparent, and context-efficient long-term memory to DeepSeek Harness. |
| 153 | [HTian-qwq/prts-terrarchive](https://github.com/HTian-qwq/prts-terrarchive) | 3 | 2026-08-31 | 2026-08-31 | 为明日方舟的长篇剧情打造的RAG类DSH插件，拥有多种快速检索能力。 |
| 154 | [huanghai-lab/dsh-custom-instructions](https://github.com/huanghai-lab/dsh-custom-instructions) | 3 | 2026-08-15 | 2026-08-28 | DSH Web 安全自定义指令管理器：编辑全局 AGENTS.md，支持模板、Markdown 预览、历史恢复、导入导出与并发保护。 |
| 155 | [imMamdouhaboammar/get-fable](https://github.com/imMamdouhaboammar/get-fable) | 3 | 2026-08-11 | 2026-09-01 | Make the model you already use work more like a frontier model with better planning, persistent context, skills, hooks, failure handling, and verification |
| 156 | [jinxlux/xiao-theme-dsh-ui-plugin](https://github.com/jinxlux/xiao-theme-dsh-ui-plugin) | 3 | 2026-08-23 | 2026-08-29 | UI plugin for deepseek harness web |
| 157 | [Jonah-Wu23/dsh-agy-safe](https://github.com/Jonah-Wu23/dsh-agy-safe) | 3 | 2026-09-03 | 2026-09-03 | DeepSeek Harness plugin: connect logged-in Antigravity CLI (agy) as chat and subagent model provider |
| 158 | [Kevin66Z0/dsh-telegram](https://github.com/Kevin66Z0/dsh-telegram) | 3 | 2026-08-28 | 2026-09-02 | Remote-control DeepSeek Harness from Telegram: stream replies, one-tap keyboards, whitelist-secured, zero inbound ports. |
| 159 | [kirbylynx/dsh-hub](https://github.com/kirbylynx/dsh-hub) | 3 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Hub |
| 160 | [lansi-ai/dsh-desktop](https://github.com/lansi-ai/dsh-desktop) | 3 | 2026-08-25 | 2026-08-27 | 把 DeepSeek Harness 做成一个真正的桌面应用：Electron 主进程内嵌 Cordis Host（与官方 Web 版同内核、零移植）， 渲染进程加载官方 Web UI 发行物（file:///自定义协议 + IPC 桥接，不开放 HTTP 端口）， 所有桌面原生能力（托盘、全局热键、系统通知、剪贴板、开机自启、协议唤起、多窗口）以 host 插件 形态注入运行时， 与官方「一切皆插件」的架构同构——不是给网页套壳，而是把桌面能力变成可装配、可卸载、可审查的插件树。  AI 驱动开发声明 |
| 161 | [liangdabiao/dsh-weather-plugin](https://github.com/liangdabiao/dsh-weather-plugin) | 3 | 2026-09-01 | 2026-09-01 | dsh = 一台"所有零件都能换"的智能体机器。写插件 = 造一个零件装上去。本项目展示怎样开发一个天气插件：天气插件的设计：Node 端调 Open-Meteo 拿温度风力，浏览器端用这些数据画一张会动的天气卡片。 |
| 162 | [mantonlove/dsh-prism-plugin](https://github.com/mantonlove/dsh-prism-plugin) | 3 | 2026-08-18 | 2026-08-27 | Prism · 棱镜 — a deeply customizable glassmorphism theme plugin for the DeepSeek Harness Web GUI |
| 163 | [meyaomiao/dsh-github-workbench](https://github.com/meyaomiao/dsh-github-workbench) | 3 | 2026-08-26 | 2026-08-27 | DSH 插件:在侧边栏使用 GitHub —— 仓库目录树 + Issues/PR/Actions 页签,支持建 Issue/PR、评论、合并、重跑 CI;better-sidebar 页签与独立面板双形态 |
| 164 | [miaomiao636/dsh-message-navigator](https://github.com/miaomiao636/dsh-message-navigator) | 3 | 2026-08-15 | 2026-09-01 | DeepSeek Harness message navigator: a table of contents for long conversations — user-message outline, click-to-jump, scroll-synced highlight, search and Markdown outline export. |
| 165 | [niuhuoshan/dsh-connect](https://github.com/niuhuoshan/dsh-connect) | 3 | 2026-08-29 | 2026-08-31 | DeepSeek Harness 数据源连接插件，支持数据库元数据发现、AI 语义建模、只读 SQL 查询和固定 HTTP API 调用 |
| 166 | [NOirBRight/dsh-llm-opencode-go](https://github.com/NOirBRight/dsh-llm-opencode-go) | 3 | 2026-08-26 | 2026-08-29 | OpenCode Go LLM provider plugin for DeepSeek Harness |
| 167 | [plolpl789/dsh-raw-html-v2](https://github.com/plolpl789/dsh-raw-html-v2) | 3 | 2026-09-03 | 2026-09-03 | VCP visual-synesthesia plugin v2 for DeepSeek Harness (official Slot API): raw-HTML vcp-root cards, streaming render, KaTeX/Mermaid/SVG, builtin fonts |
| 168 | [QinpanWan/dsh-hiboard-push](https://github.com/QinpanWan/dsh-hiboard-push) | 3 | 2026-08-23 | 2026-08-27 | Push task-completion messages to the Huawei HarmonyOS assistant-today (负一屏) card feed from DeepSeek Harness — wire-compatible with the OpenClaw today-task skill. |
| 169 | [qinyre/dsh-plugin-archive-manager](https://github.com/qinyre/dsh-plugin-archive-manager) | 3 | 2026-08-18 | 2026-09-03 | Archive manager (browse / unarchive / auto-rules) plus a Codex-style fisheye conversation rail for dsh.·归档管理与对话刻度尺插件 |
| 170 | [SaekiRaku/deepseek-rainbow-fart](https://github.com/SaekiRaku/deepseek-rainbow-fart) | 3 | 2026-08-26 | 2026-08-31 | 当你使用 DeepSeek Harness WebUI 发送消息后，插件会基于你的内容生成夸赞你的话，并通过 TTS 合成并播放声音。 \| After you send a message via DeepSeek Harness WebUI, the plugin generates compliments based on your input and plays them via TTS. |
| 171 | [Scorpio69t/teach-math-with-manim](https://github.com/Scorpio69t/teach-math-with-manim) | 3 | 2026-08-19 | 2026-08-31 | Teach Math with Manim — 图书《用 Manim 讲好数学》官方配套开源仓库 |
| 172 | [snzhi000-sys/harness-macos-desktop-plugin-suite](https://github.com/snzhi000-sys/harness-macos-desktop-plugin-suite) | 3 | 2026-08-31 | 2026-09-02 | 基于 DeepSeek‑Harness 的 macOS 桌面定制客户端，在基座之上完成原生打包运行；内置多款自研、经过迭代优化的办公插件，适配产品经理轻度开发、PRD 文档撰写等办公场景。⚠️本项目属于社区第三方项目，非 DeepSeek 官方出品。 |
| 173 | [StvLi/dsh-phoenix](https://github.com/StvLi/dsh-phoenix) | 3 | 2026-08-30 | 2026-08-31 | Never-interrupt, resumable lifecycle for DeepSeek Harness (dsh): graceful restart + client auto-reconnect + cross-restart goal continuation. |
| 174 | [SuCriss/dsh-leekbox](https://github.com/SuCriss/dsh-leekbox) | 3 | 2026-08-26 | 2026-08-27 | 韭菜盒子 LeekBox — A股看盘助手 · DeepSeek Harness (DSH) web 插件 |
| 175 | [taoser258/dsh-client-ui-skin-qingxiao](https://github.com/taoser258/dsh-client-ui-skin-qingxiao) | 3 | 2026-08-29 | 2026-08-29 | 清宵 · 弦凝清霄 —— DeepSeek Harness (DSH) Web 界面美化皮肤：以《鸣潮》角色清宵为灵感的冰蓝·青碧·月白·玄夜调色板，含可换背景画卷、剑气流光粒子、磨砂玻璃面板与新会话迎宾页。A Qingxiao (Wuthering Waves) themed client UI skin for the DSH web GUI. |
| 176 | [theoneLee/deepseek-harness-sdk-go](https://github.com/theoneLee/deepseek-harness-sdk-go) | 3 | 2026-08-15 | 2026-08-27 | Go SDK for driving DeepSeek Harness |
| 177 | [Tkingxiao/dsh-novel-solo](https://github.com/Tkingxiao/dsh-novel-solo) | 3 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的「单核写作」插件：面向量化小模型做了充分的工具瘦身与输出加固，适合在本机用本地模型跑长篇小说流水线。 |
| 178 | [UncleK/dsh-think-translate](https://github.com/UncleK/dsh-think-translate) | 3 | 2026-08-24 | 2026-08-27 | Thinking-chain UI translation for DeepSeek Harness: 8 target languages, local Ollama model primary with in-panel download, Google/Bing fallback |
| 179 | [wishesl/dsh-launcher](https://github.com/wishesl/dsh-launcher) | 3 | 2026-08-28 | 2026-08-29 | Manage DSH plugins & runtime without launching it: plugin market, per-instance masking, version install. Wails v2 (Go + React).  DeepSeek Harness 桌面启动器：不启动 DSH 即可安全管理插件与本体——多实例/多版本一键启动、实时日志、npm 版本查询、插件市场（安装/卸载/开关/收藏/分享码）、实例级插件临时屏蔽。基于 Wails v2 (Go + React)。 |
| 180 | [wp-a/dsh-academic-paper-search](https://github.com/wp-a/dsh-academic-paper-search) | 3 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 的中文学术论文检索 Bundle：复用 Academic Paper Search MCP，支持多源检索去重、引用核验、引文图谱、MeSH、试验检索与审计导出。 |
| 181 | [wycto/dsh-dock](https://github.com/wycto/dsh-dock) | 3 | 2026-08-21 | 2026-08-28 | dsh-dock · DeepSeek Harness 功能中枢：用一张管理面板统一注册、开关所有小功能（模型余额、Token 用量记录、任务动画等）。每个功能独立模块，支持开关与错误隔离，新功能即插即用。0.1.0 为基础框架，功能接入按 README 路线图迭代。 |
| 182 | [x102201/deepseek-harness-helper](https://github.com/x102201/deepseek-harness-helper) | 3 | 2026-08-25 | 2026-08-27 | 🖥️ 一台电脑并行无限 DeepSeek Harness 实例 · 🔀 每个 dsh 一个专职实例 · 🪟 同一工作区并行 · 📦 .dshpack 配置交付 |
| 183 | [Xyanxhu/kilo-zen2dsh](https://github.com/Xyanxhu/kilo-zen2dsh) | 3 | 2026-08-31 | 2026-09-01 | Kilo Gateway free models for DeepSeek Harness (DSH) |
| 184 | [yxv1203-collab/dsh-conversation-archive](https://github.com/yxv1203-collab/dsh-conversation-archive) | 3 | 2026-09-01 | 2026-09-01 | Native archive, retention, safe deletion, and verified backup management for DeepSeek Harness. |
| 185 | [zh851233/docs-mode](https://github.com/zh851233/docs-mode) | 3 | 2026-08-25 | 2026-08-27 | You can use this plugin to complete the writing of technical documents, including development briefs, user manuals, reports/summary materials, and interface/API documentation, while reducing traces of AIGC. |
| 186 | [10086ggqq/dsh_theme_Minecraft](https://github.com/10086ggqq/dsh_theme_Minecraft) | 2 | 2026-09-02 | 2026-09-02 | 把 DeepSeek Harness 变成 Minecraft Java Edition 风格——WebGL 旋转全景主菜单、存档式会话选择、四种游戏模式对应 Agent 预设、世界内 HUD 聊天台、像素风工具卡片与审批面板、AI 思考时触发跑酷小游戏、8-bit 合成音效与自定义背景音乐、五类互动桌宠与红石粒子特效。零侵入 DSH 核心源码，经典界面一键切回。 |
| 187 | [162568316/dsh-tokenrhythm-bill](https://github.com/162568316/dsh-tokenrhythm-bill) | 2 | 2026-08-31 | 2026-08-31 | dsh-tokenrhythm-bill |
| 188 | [452926826/dsh-at-skill](https://github.com/452926826/dsh-at-skill) | 2 | 2026-08-25 | 2026-08-27 | Invoke DeepSeek Harness skills with @name and composer suggestions |
| 189 | [Aik358/dsh-literature](https://github.com/Aik358/dsh-literature) | 2 | 2026-08-30 | 2026-09-01 | DSH Literature 文献侧窗插件：在 DeepSeek Harness 侧边栏识别 DOI/arXiv/标题、抓取元数据与全文、写入本地文献库或导出目录，内置 PDF 阅读器。 |
| 190 | [aiyacharley/dsh-pubmed](https://github.com/aiyacharley/dsh-pubmed) | 2 | 2026-08-27 | 2026-08-27 | DSH plugin for DeepSeek Harness: 25 model tools spanning PubMed, Europe PMC, PubTator3 & Semantic Scholar — entity-aware search, cross-source unified search, metadata, full text, citations, MeSH & ID tools, citation counts & recommendations — plus a personal literature knowledge graph with an AI-powered PubTator3 concept layer. |
| 191 | [allmodels-io/dsh-speech](https://github.com/allmodels-io/dsh-speech) | 2 | 2026-08-27 | 2026-09-03 | Real-time voice input and spoken answer summaries for DeepSeek Harness. |
| 192 | [Andiii208/gzhflow](https://github.com/Andiii208/gzhflow) | 2 | 2026-08-19 | 2026-09-01 | 跨 Agent 公众号内容发布工作流框架 — 素材先行/写作/去AI味/配图/排版/推草稿箱 六阶段流水线，适配 Claude Code/Cursor/Codex/Gemini/Qwen/DeepSeek 等主流 Agent |
| 193 | [AndKinoko/DSH-Search-Citation-Auditor](https://github.com/AndKinoko/DSH-Search-Citation-Auditor) | 2 | 2026-09-01 | 2026-09-01 | Audit citation sources in AI responses – extract URLs from the reply, score and rank them by threat level, and output a detailed report. Domains on your blocklist will be genuinely blocked – web tools such as web_search and web_fetch will directly refuse to access them. The blocklist is fully maintained by you. |
| 194 | [Anionex/dsh-smarter-edit](https://github.com/Anionex/dsh-smarter-edit) | 2 | 2026-09-04 | 2026-09-04 | A better approach to editing files in DSH. |
| 195 | [AnLifeX/dsh-attention](https://github.com/AnLifeX/dsh-attention) | 2 | 2026-08-20 | 2026-08-29 | dsh 提醒插件：别错过需要你的时刻 |
| 196 | [Ansonfishing/dsh-cap-profile](https://github.com/Ansonfishing/dsh-cap-profile) | 2 | 2026-08-28 | 2026-08-28 | Per-model capability profiling for DSH: turns local session history into tool-usage and error-rate dashboards with time-range filters |
| 197 | [AstroLiao/dsh-memory-core](https://github.com/AstroLiao/dsh-memory-core) | 2 | 2026-09-01 | 2026-09-01 | DeepSeek Harness cross-session long-term memory + user profile plugin: the AI remembers who you are, your projects and preferences across sessions. Pure Markdown, zero-config, fully local. (monorepo: dsh-memory-core + dsh-memory-ui) |
| 198 | [bettermen/xiashuo](https://github.com/bettermen/xiashuo) | 2 | 2026-08-23 | 2026-08-30 | 虾说教材写作 · dsh-course-writer — AI course-authoring workspace plugin for DeepSeek Harness (DSH). 三栏式工作台 · 九阶段门禁 · 课程/章节/资料库/知识图谱 · 导出 TXT/Word · 分享协作。Three-pane workspace, nine-phase gated workflow, lorebook, export & share. |
| 199 | [BHXiang/auto-pwa](https://github.com/BHXiang/auto-pwa) | 2 | 2026-08-19 | 2026-08-28 | AI驱动的分波分析自动化。 |
| 200 | [BlueChonk/dsh-cli-anything](https://github.com/BlueChonk/dsh-cli-anything) | 2 | 2026-08-27 | 2026-08-27 | 将 CLI-Anything 集成到 DSH (DeepSeek Harness) 的插件方案。安装后通过自然语言对话即可浏览、安装、启动和管理 100+ CLI 工具。 |
| 201 | [CJL-1995/dsh-memory-self-evolution](https://github.com/CJL-1995/dsh-memory-self-evolution) | 2 | 2026-08-30 | 2026-08-31 | dsh自动进化记忆系统 |
| 202 | [CJYLZS/dsh-commandcode-provider](https://github.com/CJYLZS/dsh-commandcode-provider) | 2 | 2026-08-28 | 2026-09-04 | a lightweight plugin supports commandcode coding plan in dsh |
| 203 | [CoolTea001/dsh-cool-theme](https://github.com/CoolTea001/dsh-cool-theme) | 2 | 2026-08-30 | 2026-08-30 | A plugin for changing themes for DSH, with a number of popular default themes built in. |
| 204 | [curtainsmall/dsh-electro-lab](https://github.com/curtainsmall/dsh-electro-lab) | 2 | 2026-08-22 | 2026-09-01 | Electrical & electronics calculation plugin for the DeepSeek Harness. 面向 DeepSeek Harness 的电气电子计算插件。 |
| 205 | [d3vmeh/dsh-fetch-timeouts](https://github.com/d3vmeh/dsh-fetch-timeouts) | 2 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: raise Node's HTTP timeouts process-wide so slow local models (Ollama, LM Studio) are not cut off at 5 minutes |
| 206 | [d86e/dsh-doctor](https://github.com/d86e/dsh-doctor) | 2 | 2026-08-27 | 2026-08-27 | dsh-doctor: self-healing watchdog for the DeepSeek Harness web profile. Recovers from plugin-induced boot failures within 60s, runs an unbounded CLI doctor, captures every tool error, and watches all live sessions for stuck turns. |
| 207 | [delock/dsh-pr-board](https://github.com/delock/dsh-pr-board) | 2 | 2026-08-26 | 2026-08-27 | Maintainer PR review queue board for DeepSeek Harness: five-state tracking (waiting on me / waiting on author / ready to merge / merged / inbox), sidebar counters, fullscreen kanban, polling, and back-to-you transition toasts. |
| 208 | [dingminhua/dsh-connect-trae](https://github.com/dingminhua/dsh-connect-trae) | 2 | 2026-08-28 | 2026-08-28 | Connect locally signed-in Trae models to DeepSeek Harness with a read-only credits overview. |
| 209 | [dugujun3-cloud/dshos-dock](https://github.com/dugujun3-cloud/dshos-dock) | 2 | 2026-09-04 | 2026-09-04 | Workspace-OS status bar for DeepSeek Harness (DSH): task counts, latest run event, checkup date. Zero deps, read-only, .dshos/ data contract. |
| 210 | [eons2long/dsh-codex-oauth](https://github.com/eons2long/dsh-codex-oauth) | 2 | 2026-08-15 | 2026-09-03 | DeepSeek Harness plugin for using ChatGPT Plus/Pro Codex models through OpenAI Codex OAuth. |
| 211 | [everclear077/dsh-progressive-tools](https://github.com/everclear077/dsh-progressive-tools) | 2 | 2026-08-24 | 2026-08-27 | Progressive tool discovery for DeepSeek Harness — tiny stable surface, searchable catalog, real pipeline execution, context cache intact. |
| 212 | [ExplorerZYzhou/DSH-freeweb](https://github.com/ExplorerZYzhou/DSH-freeweb) | 2 | 2026-08-27 | 2026-08-27 | DSH 免费联网搜索插件（Parallel 后端，零依赖） |
| 213 | [FanetheDivine/dsh-plugin-om](https://github.com/FanetheDivine/dsh-plugin-om) | 2 | 2026-08-15 | 2026-08-27 | DSH插件，以Observational Memory方式管理上下文 |
| 214 | [felix-lj-ct/dsh-mcp-workspace-scope](https://github.com/felix-lj-ct/dsh-mcp-workspace-scope) | 2 | 2026-08-31 | 2026-08-31 | Scopes MCP tool injection per workspace directory in the DeepSeek Harness: a session opened in a project sees only the MCP servers that project needs — removed from the model's tool list and refused at call time. Plus per-session switches in the composer to narrow or widen the session you are in, temporarily. |
| 215 | [FlameTN7/dsh-tui-browser-use](https://github.com/FlameTN7/dsh-tui-browser-use) | 2 | 2026-08-25 | 2026-08-31 | Browser automation bridge sub-plugin for dsh-tui.                    dsh-tui的浏览器自动化子插件 |
| 216 | [FraYoshi/dsh-ui-models-invert-selection](https://github.com/FraYoshi/dsh-ui-models-invert-selection) | 2 | 2026-08-29 | 2026-08-29 | Invert selection in Deepseek Harness for when we are selecting models  |
| 217 | [fufengyuan/dsh-stool-plugin](https://github.com/fufengyuan/dsh-stool-plugin) | 2 | 2026-08-25 | 2026-08-27 | DSH 运维工具箱插件。将 stool 运维 CLI 的全部能力注册为 DSH 模型可调用的工具，无需手动操作即可让 Agent 自动执行服务器管理、日志搜索、数据库查询、CI/CD 部署等操作。 |
| 218 | [g-yixuan/dsh-sidenote](https://github.com/g-yixuan/dsh-sidenote) | 2 | 2026-08-19 | 2026-08-28 | Codex-style side chat & selection annotations for DeepSeek Harness (DSH) web — fork the session into a persistent side panel; quote selections into context. Thin consumer of dsh-better-sidebar. |
| 219 | [gameswu/dsh-human-coding](https://github.com/gameswu/dsh-human-coding) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 增加古法编程模式，让模型监督你写代码！ |
| 220 | [hackernotfound/dsh-tacit](https://github.com/hackernotfound/dsh-tacit) | 2 | 2026-08-27 | 2026-08-27 | Learns what you leave unsaid in your prompts and steers the DeepSeek Harness agent for you |
| 221 | [HeShen-1/deepseek-whale-wallpaper](https://github.com/HeShen-1/deepseek-whale-wallpaper) | 2 | 2026-09-04 | 2026-09-04 | 🐋 Live dot-matrix whale wallpaper plugin for the DeepSeek Harness (dsh) web UI — 1,750 breathing WebGL2 particles, pointer vortices, light/dark themes · 深度求索 Harness 点阵鲸鱼动态壁纸插件 |
| 222 | [hhb1028/dsh-retry-boost](https://github.com/hhb1028/dsh-retry-boost) | 2 | 2026-08-27 | 2026-08-27 | 让 DeepSeek Harness 自动重试商汤 429/QUOTA 等瞬时网关故障直到任务完成——启动时给所有 llm-pi-ai provider 热注入加固版 retryPolicy。 |
| 223 | [hi-fangj/dsh-models-radar](https://github.com/hi-fangj/dsh-models-radar) | 2 | 2026-08-26 | 2026-08-27 | Model capability radar plugin for the DeepSeek Harness Web GUI |
| 224 | [HiQ-AI/dingtalk-dsh-assistant](https://github.com/HiQ-AI/dingtalk-dsh-assistant) | 2 | 2026-08-25 | 2026-08-29 | 基于 DeepSeek Harness 的钉钉群聊常驻个人助理插件 |
| 225 | [huaxiren6/DSH-EmailReader](https://github.com/huaxiren6/DSH-EmailReader) | 2 | 2026-08-20 | 2026-08-27 | IMAP email reader for DeepSeek Harness: list, read, and search mail via imapflow (email_list / email_read / email_search). |
| 226 | [huaxiren6/DSH-SmsWebhook](https://github.com/huaxiren6/DSH-SmsWebhook) | 2 | 2026-08-20 | 2026-08-27 | SMS forwarding webhook for DeepSeek Harness: receive pushes from phone SMS Forwarder apps, store them, expose sms_recent / sms_search tools. |
| 227 | [huenjie/dsh-paste-collapse](https://github.com/huenjie/dsh-paste-collapse) | 2 | 2026-08-27 | 2026-09-04 | dsh-plugin |
| 228 | [ianho7/dsh-port-inspector](https://github.com/ianho7/dsh-port-inspector) | 2 | 2026-08-20 | 2026-08-30 | DeepSeek Harness 的 Windows Web 插件，可将本地 TCP 监听回溯至进程、会话与工具调用，保障编程助手安全处理端口冲突/A Windows DSH Web plugin for DeepSeek Harness that traces local TCP listeners back to processes, Sessions, and Tool Calls for safe Coding Agent port-conflict handling. |
| 229 | [Icstick/dsh-work-continuity](https://github.com/Icstick/dsh-work-continuity) | 2 | 2026-08-27 | 2026-09-03 | DeepSeek Harness 的 Work Continuity 插件——跨会话工作状态显式持久化，与通用记忆解耦 |
| 230 | [imroc/dsh-project-prompt](https://github.com/imroc/dsh-project-prompt) | 2 | 2026-08-26 | 2026-08-27 | Private, per-project prompt rules for DeepSeek Harness — matched by git remote/repo/path, worktree-aware, never committed to the repo |
| 231 | [ipromise2021/dsh-omc-tui](https://github.com/ipromise2021/dsh-omc-tui) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness (DSH) 原生全功能终端交互界面 · Claude Code-styled Terminal TUI & CLI for DeepSeek Harness |
| 232 | [jarvisluk/dsh-projectless-session](https://github.com/jarvisluk/dsh-projectless-session) | 2 | 2026-08-18 | 2026-08-27 | Projectless sessions for DeepSeek Harness with isolated date-organized working directories |
| 233 | [jing-hy/computer-user](https://github.com/jing-hy/computer-user) | 2 | 2026-08-21 | 2026-08-27 | DSH plugin: Codex-style computer use for Windows - read the screen, drive mouse & keyboard via SendInput; pairs with picturereader to close the look-act-verify loop. |
| 234 | [jing-hy/dsh-unified-market](https://github.com/jing-hy/dsh-unified-market) | 2 | 2026-08-21 | 2026-08-27 | Unified plugin market for DSH Desktop (EAC): curated catalog + GitHub dsh-plugin + npm registry three sources; install/update management and .dshpack feature packs. 统一插件市场（三源聚合，EAC 特化）。 |
| 235 | [jinsiyu/dsh-code-server-app](https://github.com/jinsiyu/dsh-code-server-app) | 2 | 2026-08-25 | 2026-08-27 | 将code-server（VSCode网页版）打包安装到dsh内的插件，快速实现专业的文件编辑。Package and install code-server (the web version of VSCode) as a plugin within dsh to quickly achieve professional file editing. |
| 236 | [jiuge2467/DSH-Desktop](https://github.com/jiuge2467/DSH-Desktop) | 2 | 2026-08-18 | 2026-08-28 | 🐬 专为小白与极客打造的 DeepSeek Harness 桌面全栈工作台：内置小鲸鱼姬桌宠、多源 MCP 调试沙箱、持久化终端与看板 \| The Geek & Cozy Desktop Client for DeepSeek Harness with Whale-chan Mascot, MCP Hub & Terminal. |
| 237 | [JochenYang/dsh-app](https://github.com/JochenYang/dsh-app) | 2 | 2026-08-20 | 2026-08-28 |   A community-maintained branded desktop client for  DeepSeek Harness, Windows / macOS / Linux |
| 238 | [KannaKuron/dsh-better-workspace](https://github.com/KannaKuron/dsh-better-workspace) | 2 | 2026-08-30 | 2026-08-30 | DSH web plugin: a hierarchical workspace tree for the sidebar — titles containing / group into virtual folders; the add-workspace flow gains a parent-group popup |
| 239 | [Kilganon725/dsh-mic-dictation](https://github.com/Kilganon725/dsh-mic-dictation) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: mic dictation button next to the Full access control |
| 240 | [kiligzzz/dsh-skill-mcp-manager](https://github.com/kiligzzz/dsh-skill-mcp-manager) | 2 | 2026-08-21 | 2026-08-30 | Capability Manager for DeepSeek Harness: manage MCP servers and Skills from a Settings-page UI (dual-face dsh plugin) |
| 241 | [kober-basket/dsh-cachescope](https://github.com/kober-basket/dsh-cachescope) | 2 | 2026-08-26 | 2026-08-28 | Prompt-cache observability and logical-input diagnostics for DeepSeek Harness. |
| 242 | [LamplitIsles/dsh-companion](https://github.com/LamplitIsles/dsh-companion) | 2 | 2026-08-30 | 2026-08-30 | dsh as companion ai frontend in Svelte |
| 243 | [leolee9086/dsh-zhihu-tools](https://github.com/leolee9086/dsh-zhihu-tools) | 2 | 2026-08-22 | 2026-08-31 | 知乎数据开放平台 DSH 静态双面插件:17工具+精美卡片+串行化限流。QQ群1017854502 https://qm.qq.com/q/RAHJuyhQQ |
| 244 | [lhuans/dsh-genui](https://github.com/lhuans/dsh-genui) | 2 | 2026-08-15 | 2026-09-01 | GenUI for DeepSeek Harness: interactive charts, forms, calculators, dashboards, and mini apps rendered inline in assistant replies, with actions that flow back to the model. |
| 245 | [lnabc03/bright-drift](https://github.com/lnabc03/bright-drift) | 2 | 2026-08-31 | 2026-08-31 | Workspace drift awareness for agents — so the agent immediately knows what external changes happened in its workspace. |
| 246 | [LoKiGGo/dsh-tools](https://github.com/LoKiGGo/dsh-tools) | 2 | 2026-08-16 | 2026-08-27 | dsh web通用工具箱插件，纯AI制作（包括仓库），零人工含量，可能不会维护，请谨慎使用。 |
| 247 | [LouisHaoL/cloudcli-timer-agent](https://github.com/LouisHaoL/cloudcli-timer-agent) | 2 | 2026-09-01 | 2026-09-01 | CloudCLI plugin: cron & fixed-interval scheduler for AI agent prompts and command jobs (dsh-timer-agent port) \| CloudCLI 定时任务插件 |
| 248 | [lovaxi/Rubato_Plugins](https://github.com/lovaxi/Rubato_Plugins) | 2 | 2026-08-30 | 2026-09-01 | Make your AI's working state visible on a physical desk device - one Rubato plugin per coding agent. |
| 249 | [loyalchiiina/dsh-font-enhancer](https://github.com/loyalchiiina/dsh-font-enhancer) | 2 | 2026-08-27 | 2026-08-27 | DIY 你的 DSH 界面：按区域自定义字体/字号/颜色 \| DIY your DSH UI fonts & colors |
| 250 | [Lsc-91-69/dsh-brain-compaction](https://github.com/Lsc-91-69/dsh-brain-compaction) | 2 | 2026-08-28 | 2026-08-28 | 人脑式上下文压缩逻辑，大幅减少长任务上下文占用以及token消耗 |
| 251 | [luckzhangfengbo/dsh-web-theme](https://github.com/luckzhangfengbo/dsh-web-theme) | 2 | 2026-08-29 | 2026-08-29 | deepseek harness 背景主题插件 |
| 252 | [mackwan84/dsh-ui-mockup](https://github.com/mackwan84/dsh-ui-mockup) | 2 | 2026-08-26 | 2026-08-31 | DSH plugin for generating UI wireframes and high-fidelity mockups with DashScope Qwen/Wan and Volcengine Seedream. |
| 253 | [maxmilian/dsh-grafana-query](https://github.com/maxmilian/dsh-grafana-query) | 2 | 2026-08-26 | 2026-08-27 | Read-only Grafana metrics and alert tools for DeepSeek Harness (PromQL via datasource proxy). |
| 254 | [maxmilian/dsh-odoo](https://github.com/maxmilian/dsh-odoo) | 2 | 2026-08-26 | 2026-08-27 | Read-only Odoo tools for DeepSeek Harness, with an opt-in restricted draft-create tool. |
| 255 | [maxmilian/dsh-sentry](https://github.com/maxmilian/dsh-sentry) | 2 | 2026-08-26 | 2026-08-27 | Read-only Sentry issue and event tools for DeepSeek Harness. |
| 256 | [Medesol/dsh-kimi-formula](https://github.com/Medesol/dsh-kimi-formula) | 2 | 2026-08-31 | 2026-08-31 | Kimi (Moonshot AI) official Formula API tools for DeepSeek Harness — web_search via kimi-official provider + 10 kimi_* tools, no DeepSeek/Exa/Perplexity key needed |
| 257 | [mekos2772/dsh-plugin-mimi](https://github.com/mekos2772/dsh-plugin-mimi) | 2 | 2026-08-17 | 2026-09-03 | 鲸鱼娘 Mimi：DeepSeek Harness（DSH）桌面宠物插件，内置 Windows Computer Use 与桌宠聊天好感度。 |
| 258 | [MichaelShii/dsh-plugin-teamflow](https://github.com/MichaelShii/dsh-plugin-teamflow) | 2 | 2026-08-17 | 2026-08-27 | dsh plugin teamflow |
| 259 | [mikasaxin529/dsh-nightshift](https://github.com/mikasaxin529/dsh-nightshift) | 2 | 2026-09-02 | 2026-09-02 | Off-peak task queue plugin for DeepSeek Harness — queue at peak price, drain at night, read the savings report |
| 260 | [ming-14/PTY-Agent](https://github.com/ming-14/PTY-Agent) | 2 | 2026-06-22 | 2026-08-31 |  Give your AI agent a real terminal: persistent PTY sessions, prompt-triggered returns, screen snapshots, and   TUI/GUI/crash awareness. |
| 261 | [miuzel/dsh-subagent-ui](https://github.com/miuzel/dsh-subagent-ui) | 2 | 2026-08-26 | 2026-08-27 | Searchable workspace subagent manager for DeepSeek Harness Web |
| 262 | [Moonshile/moonshile-dsh-plugins](https://github.com/Moonshile/moonshile-dsh-plugins) | 2 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) plugins — dsh-workspace-sort: re-sorts sidebar workspaces by last activity once per day. One-command npm bundle install. |
| 263 | [mrRisega/dsh-remote](https://github.com/mrRisega/dsh-remote) | 2 | 2026-08-19 | 2026-08-27 | Remote control for DeepSeek Harness (dsh web) from any phone browser: tunnel-mode relay client with one-command install and self-hosting support |
| 264 | [nabin-qq273274877/dsh-desktop](https://github.com/nabin-qq273274877/dsh-desktop) | 2 | 2026-08-31 | 2026-08-31 | DeepSeek Harness Desktop - 桌面启动器 (Tauri 2 + 内置 Node + 自动更新) |
| 265 | [Nagi-ovo/dsh-music-tui](https://github.com/Nagi-ovo/dsh-music-tui) | 2 | 2026-08-31 | 2026-08-31 | YesPlayMusic controls and now-playing status for dsh-TUI |
| 266 | [nickkkkkk123123/dsh-whale-girl](https://github.com/nickkkkkk123123/dsh-whale-girl) | 2 | 2026-08-27 | 2026-08-27 | 鲸鱼娘·灵动挂件 — 会卖萌、会记账、会弹跳的 DSH 桌面挂件插件（余额/用量/上下文/峰谷/右键菜单/拖动甩抛） |
| 267 | [NOirBRight/dsh-llm-commandcode](https://github.com/NOirBRight/dsh-llm-commandcode) | 2 | 2026-08-27 | 2026-08-29 | Command Code Provider API LLM plugin for DeepSeek Harness |
| 268 | [ohmejj/dsh-chat-archive](https://github.com/ohmejj/dsh-chat-archive) | 2 | 2026-08-28 | 2026-09-02 | 自动归档 DeepSeek Harness 对话记录 |
| 269 | [omdsh-dev/dsh-file-trace](https://github.com/omdsh-dev/dsh-file-trace) | 2 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 270 | [onenameneo/dsh-plugin-loom-chat](https://github.com/onenameneo/dsh-plugin-loom-chat) | 2 | 2026-08-30 | 2026-08-31 | Loom Chat is a DSH Web client plugin that turns linear ordinary sessions into a pannable, zoomable Loom-style canvas for parallel exploration. |
| 271 | [pavangupta352/stalegreen](https://github.com/pavangupta352/stalegreen) | 2 | 2026-09-03 | 2026-09-03 | Keeps a coding agent's green claims honest: verification runs are recorded unmasked, and done is blocked when the evidence is stale, failed or masked. |
| 272 | [ph4310822/dsh-edex-jarvis-ui](https://github.com/ph4310822/dsh-edex-jarvis-ui) | 2 | 2026-08-25 | 2026-08-27 | DeepSeek Harness eDEX-UI shell plugin — JARVIS variant: electric cyan HUD with VITAL SIGNS / RT-MONITOR / RT-LOG left bar, POWER CORE / RADAR right bar, JARVIS header |
| 273 | [PianoPrince/dsh-workspace-mover](https://github.com/PianoPrince/dsh-workspace-mover) | 2 | 2026-08-26 | 2026-08-30 | 拖拽跨工作区真迁移 DSH 会话：批量移动、挂错归位、分组合并；步步备份回滚，零 token 消耗 / Move DSH sessions across workspaces by drag & drop — true migration, batch move, misfiled homing, group merge; backups + rollback, zero tokens. |
| 274 | [pirate-608/dsh-multi-tools](https://github.com/pirate-608/dsh-multi-tools) | 2 | 2026-08-14 | 2026-08-31 | Multimodal tool suite for DeepSeek Harness: ModLens vision, local ComfyUI, Unity, creative apps, CAD, and Ren'Py. |
| 275 | [plastic-labs/dsh-honcho](https://github.com/plastic-labs/dsh-honcho) | 2 | 2026-08-31 | 2026-09-02 | Honcho integration for the DeepSeek Harness |
| 276 | [PolinniZhong/dsh-session-workbench](https://github.com/PolinniZhong/dsh-session-workbench) | 2 | 2026-08-21 | 2026-08-30 | Session Workbench for DeepSeek Harness: session-library full-text search + recall + conversation-view management (show/hide + reorder). 会话工作台：会话库（历史会话全文搜索与召回）+ 会话视图（标签栏显示/隐藏 + 拖拽排序）。 |
| 277 | [porcelaintech/dsh-plugin-voice-input](https://github.com/porcelaintech/dsh-plugin-voice-input) | 2 | 2026-09-03 | 2026-09-03 | Voice input plugin for DeepSeek Harness: a minimal mic control in the composer with continuous bilingual recognition, context-aware term correction, punctuation, and a live waveform |
| 278 | [qingmomo233/dsh-thinking-language](https://github.com/qingmomo233/dsh-thinking-language) | 2 | 2026-08-16 | 2026-08-29 | 更改 deepseek harness 思考过程语言 |
| 279 | [QinpanWan/dsh-sky-skin](https://github.com/QinpanWan/dsh-sky-skin) | 2 | 2026-08-25 | 2026-08-27 | Sky: Children of the Light themed skin for DeepSeek Harness web UI - light children on a glowing star map, candlelight gold and starry night. 光遇·遇境主题皮肤。 |
| 280 | [Qiongkura/dsh-interface-settings](https://github.com/Qiongkura/dsh-interface-settings) | 2 | 2026-08-16 | 2026-08-29 | DSH interface customization plugin: wallpaper / transparency / glass blur / splash screen一个 DeepSeek Harness 前端插件：把「壁纸 / 区域透明 / 输入框与轨迹毛玻璃 / 模糊程度 / 启动画面」做成一站式界面设置，作为独立插件项目上传、分享，装进 DSH 即可使用 |
| 281 | [QuantumKuba/dsh-graphify-plugin](https://github.com/QuantumKuba/dsh-graphify-plugin) | 2 | 2026-08-31 | 2026-08-31 | Native Graphify knowledge graph plugin for DeepSeek Harness (DSH) — code intelligence, god nodes, and topological agent tools. |
| 282 | [rootkiller6788/dsh-launcher](https://github.com/rootkiller6788/dsh-launcher) | 2 | 2026-08-31 | 2026-08-31 | DSHL — A desktop launcher for managing AI runtimes, instances, plugins, MCP servers, skills, profiles, and distributions. |
| 283 | [SA1992X/dsh-ctrl-enter-submit](https://github.com/SA1992X/dsh-ctrl-enter-submit) | 2 | 2026-08-25 | 2026-08-27 | 轻松换行 |
| 284 | [sakthiveltofficial/dsh-shopify-plugins](https://github.com/sakthiveltofficial/dsh-shopify-plugins) | 2 | 2026-08-26 | 2026-08-27 | Shopify plugin for DeepSeek Harness: 213 model-facing shopify_* tools over the Shopify Admin REST + GraphQL APIs (products, orders, customers, inventory, fulfillments, discounts, content, webhooks, themes, billing, bulk operations) with Admin API access-token auth. |
| 285 | [seewhydee/dsh-emacs-bridge](https://github.com/seewhydee/dsh-emacs-bridge) | 2 | 2026-08-23 | 2026-08-27 | Deepseek Harness to Emacs bridge |
| 286 | [SeverusZh/dsh-skills-mcp-group-manager](https://github.com/SeverusZh/dsh-skills-mcp-group-manager) | 2 | 2026-08-28 | 2026-08-28 | DeepSeek Harness Skills & MCPs 分组管理器 — 分组管理 Skills、过滤模型技能目录、独立开关 MCP 服务器、左侧面板一键管理 / Group skills, filter the model skill catalog, toggle MCP servers, left panel UI |
| 287 | [Shyboy0499/dsh-git-tools](https://github.com/Shyboy0499/dsh-git-tools) | 2 | 2026-08-26 | 2026-08-27 | Local git tools for DeepSeek Harness (dsh): git_status, git_diff, git_log, git_commit |
| 288 | [squirrel20/dsh-cron](https://github.com/squirrel20/dsh-cron) | 2 | 2026-08-26 | 2026-08-27 | Unattended scheduled jobs for the DeepSeek Harness (dsh): agent/command tasks on cron schedules |
| 289 | [STARDUSTLC666/dsh-cite](https://github.com/STARDUSTLC666/dsh-cite) | 2 | 2026-08-15 | 2026-08-27 | DeepSeek Harness 参考文献插件：cite_lookup/check/format/bibtex/health 五工具，DOI 精确查询、Crossref 题录检索、GB/T 7714/APA/MLA/Chicago 格式化、有界并发 DOI 校验；纯 Node 全平台。· Citation tools for DeepSeek Harness agents. 已验证兼容 DeepSeek Harness v0.1.2-alpha.5。 |
| 290 | [starefinger/dsh-llm-qwen-local](https://github.com/starefinger/dsh-llm-qwen-local) | 2 | 2026-08-26 | 2026-08-27 | 面向 DeepSeek Harness(dsh)的 LLM 适配器插件:驱动由 OpenAI 兼容服务的本地部署 Qwen3.8-27B 模型。支持按模型多模态开关、完全可配置的推理档位、请求图像投影,以及中英双语 Web 设置页。 |
| 291 | [statem-li/dsh-triad](https://github.com/statem-li/dsh-triad) | 2 | 2026-08-28 | 2026-08-28 | 用量趋势 · 技能与 MCP Server 管理 · 自动沉淀的长期记忆——一套插件装齐 DSH 三个工作台。纯插件注入，不动官方源码，一句话安装。 |
| 292 | [Stylelinzzz/dsh-chat-history](https://github.com/Stylelinzzz/dsh-chat-history) | 2 | 2026-08-17 | 2026-08-30 | Chat history TOC for DeepSeek Harness: a History conversation view tab listing user messages with auto-paging and click-to-jump back into the chat. / DeepSeek Harness 会话目录插件：用户消息历史一键跳转。 |
| 293 | [summer-521/deepseek-harness-desktop](https://github.com/summer-521/deepseek-harness-desktop) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness 的非官方桌面封装：本地优先、沙箱隔离，内置 dsh 版本管理与插件管理，支持自动更新与任务完成桌面通知（macOS）。 |
| 294 | [SUONSUN9527/deepseek-harness-flow-arrange](https://github.com/SUONSUN9527/deepseek-harness-flow-arrange) | 2 | 2026-08-31 | 2026-08-31 | Claude-orchestrator x Codex-executor distribution of DeepSeek Harness |
| 295 | [supersyh-sss/dsh-voice-assistant](https://github.com/supersyh-sss/dsh-voice-assistant) | 2 | 2026-08-29 | 2026-08-30 | Offline voice assistant for dsh web — wake word, speech dictation, voice edit commands & Chinese TTS. On-device sherpa-onnx WASM ASR, no Google dependency, works in China. |
| 296 | [swordordead/dsh-Veneer](https://github.com/swordordead/dsh-Veneer) | 2 | 2026-08-18 | 2026-08-31 | DIY你的小蓝鲸吧 |
| 297 | [Tsqurt/dsh-plugin-studio](https://github.com/Tsqurt/dsh-plugin-studio) | 2 | 2026-08-27 | 2026-08-28 | 为了开发插件，开发了一个开发插件的插件。通过可视化的事件流、插件管理、工具管理、技能管理、预设管理，简化插件的开发流程，方便开发者理解插件的作用。 |
| 298 | [umineko987/dsh-search-enhance](https://github.com/umineko987/dsh-search-enhance) | 2 | 2026-08-14 | 2026-09-04 | 提供 Grok-compatible 网页搜索、保留来源分页、Context7 与 Exa 文档检索、有界网页提取、站点映射、离线研究计划和只读诊断。 |
| 299 | [unknowbug/dsh-thinking-loop-guard](https://github.com/unknowbug/dsh-thinking-loop-guard) | 2 | 2026-08-27 | 2026-08-27 | Detect & break thinking-chain loops in DSH agents at the turn boundary (no proxy). Ported from ollama-loop-guard. |
| 300 | [vuldin/yapa](https://github.com/vuldin/yapa) | 2 | 2026-03-24 | 2026-08-27 | Yet Another Personal Assistant |
| 301 | [wang-kaopu/dsh-cordis-devtools](https://github.com/wang-kaopu/dsh-cordis-devtools) | 2 | 2026-08-23 | 2026-08-27 | Give coding Agents runtime evidence for debugging and verifying DSH / Cordis plugins. 让 Coding Agent 获得用于调试和验证 DSH / Cordis 插件的运行时证据。 |
| 302 | [wangxueqi00/dsh-client-ui-knowledge-cards](https://github.com/wangxueqi00/dsh-client-ui-knowledge-cards) | 2 | 2026-08-31 | 2026-08-31 | A plugin of Deepseek Harness(DSH),transform your recent chat history into beautifully designed knowledge cards, ready to download and share. |
| 303 | [wanyexin1998/dsh-workbench](https://github.com/wanyexin1998/dsh-workbench) | 2 | 2026-08-26 | 2026-08-27 | Community-maintained source preview for two-Pane DeepSeek Harness Web workflows |
| 304 | [weiwang988/dsh-session-spend](https://github.com/weiwang988/dsh-session-spend) | 2 | 2026-09-04 | 2026-09-04 | DSH 客户端插件：实时会话花费（¥）· 官方峰谷计价 + 节省分解 DSH client plugin: live session cost readout (¥) with official DeepSeek peak/valley pricing and savings breakdown |
| 305 | [whh110112/human-writing-skills](https://github.com/whh110112/human-writing-skills) | 2 | 2026-06-15 | 2026-09-01 | Advanced multilingual AI humanizer and writing toolkit for natural prose, voice preservation, long-form continuity, and focused audits. |
| 306 | [wly8691-jpg/dsh-office-com](https://github.com/wly8691-jpg/dsh-office-com) | 2 | 2026-08-26 | 2026-08-27 | DSH plugin: COM-driven real Office automation (VBA/pivot/recalc/layout) |
| 307 | [WSL043/dsh-reasoning-slider](https://github.com/WSL043/dsh-reasoning-slider) | 2 | 2026-08-23 | 2026-08-27 | 已归档：DeepSeek Harness 模型感知推理强度滑杆；现有 Release 与演示保留，不再适配未来 DSH。 |
| 308 | [x1shang/dsh-koin-lily-news](https://github.com/x1shang/dsh-koin-lily-news) | 2 | 2026-08-21 | 2026-08-27 | 菲奖得主强推的百合新闻订阅DSH插件 |
| 309 | [Xiamu-ssr/dsh-wind-aifin](https://github.com/Xiamu-ssr/dsh-wind-aifin) | 2 | 2026-07-13 | 2026-09-03 | Credential-safe Wind AIFin MCP and Alice integration for DeepSeek Harness. |
| 310 | [xiaoguomeiyitian/dsh-qr-share](https://github.com/xiaoguomeiyitian/dsh-qr-share) | 2 | 2026-08-29 | 2026-08-30 | DSH web plugin: a sidebar-footer QR-code button that lets a phone scan and re-issue the current browser's authenticated launch URL. |
| 311 | [xiaoshi7915/dsh-kb-manager](https://github.com/xiaoshi7915/dsh-kb-manager) | 2 | 2026-08-27 | 2026-08-27 | DSH local knowledge base plugin: multi-format import, smart chunking, vector index, hybrid search (BM25 + sqlite-vec + RRF) for agent long-term memory |
| 312 | [xiaoso456/dsh-tool-plus](https://github.com/xiaoso456/dsh-tool-plus) | 2 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 基础工具增强：持久 bash、结构化 read、多模式 edit、原子 write、双引擎 grep/glob、图像直读，一个插件全覆盖 |
| 313 | [xxww0098/dsh-plugin-oauth-subs](https://github.com/xxww0098/dsh-plugin-oauth-subs) | 2 | 2026-08-26 | 2026-09-03 | ChatGPT Codex and xAI Grok subscription OAuth for DeepSeek Harness — PKCE / device-code, local Responses proxy, llm-pi-ai sync |
| 314 | [Ycet/dsh-awesome-hud](https://github.com/Ycet/dsh-awesome-hud) | 2 | 2026-08-29 | 2026-08-30 | dsh侧边HUD面板，包含多个信息展示模块（可自定义是否展示），集成压缩上下文、查看git graph等功能。DSH side HUD panel, containing multiple information display modules (customizable whether to display), integrating features such as compressed context, viewing git graph, etc. |
| 315 | [yhfgyyf/dsh-audit-mode](https://github.com/yhfgyyf/dsh-audit-mode) | 2 | 2026-08-23 | 2026-09-02 | Guardian preset for DeepSeek Harness with independent persistent Codex auditing |
| 316 | [youngrock-labs/dsh-provider-copilot](https://github.com/youngrock-labs/dsh-provider-copilot) | 2 | 2026-09-01 | 2026-09-03 | use a GitHub Copilot subscription as a DSH LLM provider |
| 317 | [yu-wenchao/dsh-opencode-free-models](https://github.com/yu-wenchao/dsh-opencode-free-models) | 2 | 2026-09-03 | 2026-09-03 | 无限免费额度的deepseek harnes 免费模型插件-免费api-DeepSeek Harness (DSH) 插件 — 在聊天界面里实时展示 OpenCode Zen 的最新免费模型，无需登录、无需密钥，直接在模型选择器选用即可对话。切换网络实现无限额度，无限量token自由！ |
| 318 | [yuioi666/dsh-plugin-model-capability](https://github.com/yuioi666/dsh-plugin-model-capability) | 2 | 2026-08-27 | 2026-08-31 | Model Capability Manager for DSH Web: thinking levels, context window, output caps, input modalities, gateway compat presets, EN/中文 UI. \| DSH 网页端模型能力管理插件。 |
| 319 | [Yur0918/dsh-user-addons](https://github.com/Yur0918/dsh-user-addons) | 2 | 2026-08-28 | 2026-08-28 | Community DSH web plugin for file uploads, archived-session management, image capability detection, and model/token usage insights. |
| 320 | [yushi-javatoai/ai-web-ppt-maker](https://github.com/yushi-javatoai/ai-web-ppt-maker) | 2 | 2026-08-31 | 2026-08-31 | AI 网页 PPT 生成器：粘贴长文案，AI 流式拆解为多页网页 PPT，支持全屏演示、键盘翻页、多套主题与独立 HTML 导出。 |
| 321 | [Yvesgao/dsh-shortcut-creator](https://github.com/Yvesgao/dsh-shortcut-creator) | 2 | 2026-08-15 | 2026-08-30 | DSH 启动器- 在 DSH 设置页一键创建 Windows 桌面快捷方式，自动打开浏览器、可固定任务栏。DSH plugin: one-click Windows desktop shortcut launcher from the Settings page (DeepSeek Harness or any local server) —Install: dsh plugin --profile web add github:Yvesgao/dsh-desktop-shortcut#main |
| 322 | [zengweicheng666/dsh-svn-tools](https://github.com/zengweicheng666/dsh-svn-tools) | 2 | 2026-08-29 | 2026-08-29 | SVN (Subversion) tools + sidebar UI for DeepSeek Harness: 33 agent tools with UTF-8 Chinese commit logs, plus an SVN panel in dsh-better-sidebar. |
| 323 | [zhenghaoyang24/obsidian-plugin-deepshian](https://github.com/zhenghaoyang24/obsidian-plugin-deepshian) | 2 | 2026-08-27 | 2026-08-27 | Sidebar AI chat powered by the local DeepSeek Harness (dsh): streaming replies, tool calls, and real vault file edits. |
| 324 | [zhoulvyuan/dsh-plugin](https://github.com/zhoulvyuan/dsh-plugin) | 2 | 2026-08-26 | 2026-08-28 | deepseek-harness插件 |
| 325 | [zingzheng/dsh-gb](https://github.com/zingzheng/dsh-gb) | 2 | 2026-09-04 | 2026-09-04 | 把手机变成 DSH 的语音遥控外设 |
| 326 | [zuohaisu/dsh-ai-soul](https://github.com/zuohaisu/dsh-ai-soul) | 2 | 2026-08-26 | 2026-09-01 | Persistent identity layer for DeepSeek Harness. The first reference implementation of AI Soul. |
| 327 | [zzy-12345678/dsh-file-convert](https://github.com/zzy-12345678/dsh-file-convert) | 2 | 2026-08-29 | 2026-08-30 | Local-first file conversion for DeepSeek Harness — images, PDF, data, audio/video & office docs. 7 tools, 26 conversions, no API keys, no uploads. |
| 328 | [0x5446/rowel](https://github.com/0x5446/rowel) | 1 | 2026-08-14 | 2026-09-01 | Native iOS client for DeepSeek Harness (dsh). Answer your agent from your phone — the relay only ever sees ciphertext. |
| 329 | [0xrushmoon/dsh-freeroute](https://github.com/0xrushmoon/dsh-freeroute) | 1 | 2026-08-25 | 2026-08-27 | Free-tier model aggregation plugin for the DeepSeek Harness (dsh): transparent failover, multi-key rotation, settings panel |
| 330 | [123twtd/dsh-plugin-manager](https://github.com/123twtd/dsh-plugin-manager) | 1 | 2026-08-29 | 2026-08-29 | Independent DSH plugin inventory and transactional Profile manager. |
| 331 | [166767/dsh-error-audit](https://github.com/166767/dsh-error-audit) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 实时 AI 自审插件：任何报错/警告第一时间连同时间、错误码、会话、用户原话、AI 动作与工作区写入专用日志目录，并主动通知 AI、内置 read_error_logs 工具随时读取。Real-time AI self-audit for DeepSeek Harness — captures every error/warning with timestamp, error code, session, user prompt, AI action and workspace into a dedicated log folder; instantly notifies the agent and ships a read_error_logs tool. |
| 332 | [173787247/dsh-tool-budget](https://github.com/173787247/dsh-tool-budget) | 1 | 2026-08-29 | 2026-08-29 | Hard-stop DeepSeek Harness tool use after a per-session call budget |
| 333 | [173787247/dsh-wsl-browser](https://github.com/173787247/dsh-wsl-browser) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: open http(s) URLs in the Windows default browser from WSL. |
| 334 | [173787247/dsh-wsl-clipboard](https://github.com/173787247/dsh-wsl-clipboard) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: read/write the Windows clipboard from WSL. |
| 335 | [173787247/dsh-wsl-cred](https://github.com/173787247/dsh-wsl-cred) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: safe Git credential hints for Windows GCM from WSL. |
| 336 | [173787247/dsh-wsl-distro](https://github.com/173787247/dsh-wsl-distro) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: current WSL distro facts and multi-distro warnings. |
| 337 | [173787247/dsh-wsl-github](https://github.com/173787247/dsh-wsl-github) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness: GitHub App status (open PRs + latest Actions) for WSL agents |
| 338 | [173787247/dsh-wsl-gpu](https://github.com/173787247/dsh-wsl-gpu) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: probe nvidia-smi / GPU visibility inside WSL. |
| 339 | [173787247/dsh-wsl-kit](https://github.com/173787247/dsh-wsl-kit) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness WSL kit (EN/ZH): docs + install.sh + cordis.patch for Windows browser + WSL agent plugins |
| 340 | [173787247/dsh-wsl-launch](https://github.com/173787247/dsh-wsl-launch) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: launch allowlisted Windows apps from WSL. |
| 341 | [173787247/dsh-wsl-notify](https://github.com/173787247/dsh-wsl-notify) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: Windows MessageBox notification from WSL. |
| 342 | [173787247/dsh-wsl-path](https://github.com/173787247/dsh-wsl-path) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: convert WSL Linux and Windows paths with /mnt/c caveats. |
| 343 | [173787247/dsh-wsl-port](https://github.com/173787247/dsh-wsl-port) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: diagnose WSL port listening and Windows localhost forwarding. |
| 344 | [17861102832/fleet-os](https://github.com/17861102832/fleet-os) | 1 | 2026-09-01 | 2026-09-01 | Fleet OS · 舰队模式 — 生产级多 Agent 协同引擎：WS 黑板 + 事件溯源 + 盲评对抗 + 跨舰队接力 + 上下文压缩 + 多厂商负载均衡 + 自进化。36 模块，零运行时依赖，MCP 40 工具，48 项 e2e 全绿。 |
| 345 | [240xu/verdict-engine](https://github.com/240xu/verdict-engine) | 1 | 2026-08-24 | 2026-08-27 | Verdict Engine — machine-checkable engineering governance: prose skill for any agent + dsh-themis DSH plugin (read-only tools, fail-closed, protocolJson negotiation). 纯文本规范 + 可校验运行时双载体。 |
| 346 | [2DogsLee/dsh_whalebuddy](https://github.com/2DogsLee/dsh_whalebuddy) | 1 | 2026-08-29 | 2026-08-29 | whalebuddy - DeepSeek Harness desktop pet (Windows): a DSH bundle plugin + Tauri shell. A porthole whale reflects your agent live state, with autostart & skin settings. |
| 347 | [33moren33/dsh-slice-bench](https://github.com/33moren33/dsh-slice-bench) | 1 | 2026-08-30 | 2026-08-30 | 把插件放进一台真起来的最小 DSH 机器，让 harness 自己说它站不站得住 · Runtime bench for DSH plugin version conflicts — the harness gives the verdict, not us |
| 348 | [452926826/dsh-feishu-bot](https://github.com/452926826/dsh-feishu-bot) | 1 | 2026-08-25 | 2026-08-27 | Connect a Feishu bot to DeepSeek Harness projects and conversations |
| 349 | [452926826/dsh-ssh-logs](https://github.com/452926826/dsh-ssh-logs) | 1 | 2026-08-25 | 2026-08-27 | Read allowlisted remote logs over SSH from DeepSeek Harness conversations |
| 350 | [66-empty/DeepSeek-Harness-Desktop](https://github.com/66-empty/DeepSeek-Harness-Desktop) | 1 | 2026-09-04 | 2026-09-04 | Electron desktop shell for the DeepSeek Harness Web GUI; first run auto-installs a portable runtime (Node + pinned deepseek-harness), with prebuilt packs, CN mirrors and zh/en UI. DeepSeek Harness 桌面版外壳:首启自动装配运行环境,支持预构建运行包与国内镜像,界面中英双语。 |
| 351 | [6pofx/dsh-tool-explorer](https://github.com/6pofx/dsh-tool-explorer) | 1 | 2026-08-30 | 2026-09-03 | DSH（DeepSeek Harness）技能与 MCP 管理控制台插件：按来源分级浏览全部已加载技能，独立开关模型/用户调用，创建/编辑/删除技能（可恢复回收站），从 GitHub 多选批量安装；增删改 MCP 服务器、状态监控与连接测试。Management console for DeepSeek Harness (dsh): grouped skill browsing, model/user invocation toggles, GitHub batch install, recoverable trash, and MCP server management. |
| 352 | [988hj7tczd-oss/harness-github](https://github.com/988hj7tczd-oss/harness-github) | 1 | 2026-08-23 | 2026-08-27 | DeepSeek Harness GitHub plugin: review PRs, triage issues, debug Actions CI, handle incoming GitHub events (webhooks + polling) via dsh-native tools. |
| 353 | [aalvsz/dsh-hermes-bridge](https://github.com/aalvsz/dsh-hermes-bridge) | 1 | 2026-08-27 | 2026-08-27 | Literal Hermes Agent → DeepSeek Harness bridge: shared memory, skills, live tools, MCP, and full-agent delegation. |
| 354 | [abbccdd/dsh-localtts](https://github.com/abbccdd/dsh-localtts) | 1 | 2026-08-28 | 2026-08-29 | Local IndexTTS 2.5 and GPT-SoVITS speech synthesis and playback for DeepSeek Harness. |
| 355 | [Aealen/dsh-coding-workspace](https://github.com/Aealen/dsh-coding-workspace) | 1 | 2026-08-27 | 2026-09-03 | coding 工作台。以 git worktree 并行开发为地基，向上提供跨会话协作原语、项目分组侧栏与停靠式工作区面板(资源管理器 / Git Changes·Logs),把 dsh 的单会话界面变成多工作区并行开发驾驶舱。 |
| 356 | [algerkong/dsh-image-preview](https://github.com/algerkong/dsh-image-preview) | 1 | 2026-08-27 | 2026-08-27 | Image preview for DSH (DeepSeek Harness) web sessions: read_image results render as a thumbnail, click for full size in the built-in lightbox. |
| 357 | [ALKAERR/dsh-pet](https://github.com/ALKAERR/dsh-pet) | 1 | 2026-09-03 | 2026-09-03 | 一只常驻 DSH 界面的鲸鱼娘女仆长「会话监督挂件」。替主人监督 AI 助手的工作——读工具调用结果做证据，戳破"口嗨式完成"，用自然女仆口吻温柔纠偏，并一键给出可直接复制的修正 Prompt。标准 DSH bundle，代码+立绘自包含、开箱即用。 |
| 358 | [americanjeff/filestab](https://github.com/americanjeff/filestab) | 1 | 2026-08-31 | 2026-09-01 | Adds a file/vcs browser with diff and markdown preview support to the DeepSeek Harness · 为 DeepSeek Harness 添加文件 / VCS 浏览器，支持 diff 与 Markdown 预览。 |
| 359 | [amphilagus/dsh-gamer](https://github.com/amphilagus/dsh-gamer) | 1 | 2026-08-20 | 2026-08-28 | DSH bundle + 游戏玩家 preset: play on a dsh-gaming-platform instance. |
| 360 | [Andor-Z/dsh-turn-outline](https://github.com/Andor-Z/dsh-turn-outline) | 1 | 2026-09-03 | 2026-09-03 | DSH 轮次轨迹侧边栏插件：按用户轮次折叠会话（输入+工具步骤+输出），一键跳回对话原位；零 AI、只读 \| Turn-outline tab for dsh-better-sidebar: fold sessions by user turns with one-click jump-back; zero-LLM, read-only |
| 361 | [Anionex/dsh-pinned-sessions](https://github.com/Anionex/dsh-pinned-sessions) | 1 | 2026-09-04 | 2026-09-04 | dsh会话置顶插件 ｜ dsh session pinning plugin, pin important DeepSeek Harness sessions in the workspace sidebar |
| 362 | [Ansonfishing/dsh-ca-ref](https://github.com/Ansonfishing/dsh-ca-ref) | 1 | 2026-08-28 | 2026-08-28 | Clean Architecture reference library for DSH: 8 pinned reference repos with FTS5 search, assertion rules, and a review ledger for architecture reviews |
| 363 | [arthur20150522/dsh-token-usage-cost](https://github.com/arthur20150522/dsh-token-usage-cost) | 1 | 2026-08-28 | 2026-08-28 | Shows per-turn and session token costs in DSH web conversations. |
| 364 | [Ary66101/dsh-desktop](https://github.com/Ary66101/dsh-desktop) | 1 | 2026-08-25 | 2026-08-27 | dsh的自制桌面端 |
| 365 | [Ary66101/dsh-instruction-bubble](https://github.com/Ary66101/dsh-instruction-bubble) | 1 | 2026-08-27 | 2026-08-27 | 你的上文语境小气泡 |
| 366 | [ashuai/dsh-s2s](https://github.com/ashuai/dsh-s2s) | 1 | 2026-08-31 | 2026-08-31 | Connect AI agent sessions on one machine — a DeepSeek Harness plugin for session-to-session collaboration, with lifecycle support to wake finished sessions and loop-safe messaging budgets. |
| 367 | [awnlight/talon-ui](https://github.com/awnlight/talon-ui) | 1 | 2026-08-28 | 2026-08-28 | A terminal UI for DeepSeek Harness (dsh) agents. |
| 368 | [BaronCyrus/dsh-kimi-subscription](https://github.com/BaronCyrus/dsh-kimi-subscription) | 1 | 2026-08-28 | 2026-08-28 | Use a Kimi Code subscription in DeepSeek Harness with OAuth, quota display, and composer usage |
| 369 | [better-er/dsh-peak-block](https://github.com/better-er/dsh-peak-block) | 1 | 2026-08-31 | 2026-08-31 | 梁文峰时间高峰自动拦截官方 DeepSeek 请求 |
| 370 | [better-er/dsh-write-create-only](https://github.com/better-er/dsh-write-create-only) | 1 | 2026-09-01 | 2026-09-02 | write 仅创建：禁止 write 覆盖已存在文件，目标已存在时自动拒绝并提示改用 edit，防止模型误覆写已有内容。纯 host 端 dsh 插件。 |
| 371 | [better-er/dsh-write-rule-guard](https://github.com/better-er/dsh-write-rule-guard) | 1 | 2026-09-02 | 2026-09-02 | dsh 插件：按可配置正则规则拦截 edit/write 的写入内容，默认拦全角括号，host 单半身经 cordis 配置注入。 |
| 372 | [big0lives/dsh-web-window-companion](https://github.com/big0lives/dsh-web-window-companion) | 1 | 2026-08-31 | 2026-08-31 | DSH Web 窗口伴侣插件：App 模式窗口打开 Web GUI，关窗即优雅停服。Close the window = stop the server. |
| 373 | [big0lives/dsh-win-quick-launcher](https://github.com/big0lives/dsh-win-quick-launcher) | 1 | 2026-08-31 | 2026-08-31 | DSH 的 Windows 便捷启动器：双击桌面图标启动 DeepSeek Harness Web，关掉浏览器窗口即停服务。支持源码安装与 npm 安装。 |
| 374 | [biliye/dsh-voice-call](https://github.com/biliye/dsh-voice-call) | 1 | 2026-08-16 | 2026-08-31 | 这是一个deepseek专属的语音通话插件 |
| 375 | [bill277048-hash/DSH-guardian](https://github.com/bill277048-hash/DSH-guardian) | 1 | 2026-09-03 | 2026-09-03 | for DSH |
| 376 | [bingaha/dsh-live-mcp](https://github.com/bingaha/dsh-live-mcp) | 1 | 2026-08-19 | 2026-08-31 | 给DSH提供会话级的MCP控制能力 |
| 377 | [biubiu23333333/dsh-memory](https://github.com/biubiu23333333/dsh-memory) | 1 | 2026-09-04 | 2026-09-04 | dsh-memory |
| 378 | [bjzkhy/dsh-token-ledger-pro](https://github.com/bjzkhy/dsh-token-ledger-pro) | 1 | 2026-08-30 | 2026-08-30 | DSH cost panel: meters every request from session events, prices it against a built-in catalog of 136 models across 16 providers, and shows model, balance, session/today/month spend and a monthly budget bar next to the composer. |
| 379 | [bluechips-zhao/dsh-browser-slotpool](https://github.com/bluechips-zhao/dsh-browser-slotpool) | 1 | 2026-09-03 | 2026-09-03 | DSH bundle: slot-pool wrapper for concurrent browser sessions｜并发浏览器会话槽位池插件 |
| 380 | [BlueChonk/dsh-balance-phoebe](https://github.com/BlueChonk/dsh-balance-phoebe) | 1 | 2026-08-28 | 2026-08-29 | 菲比啾比查 longcat token 余量挂件 |
| 381 | [bobjia/dsh-context-milvus](https://github.com/bobjia/dsh-context-milvus) | 1 | 2026-08-29 | 2026-08-29 | claude-context-milvus like plugin for Deepseek Harness (DSH)  |
| 382 | [Bobnemimimmi/dsh-always-status-bar](https://github.com/Bobnemimimmi/dsh-always-status-bar) | 1 | 2026-08-26 | 2026-08-27 | 始终显示消息下的 status bar，无需鼠标悬停 |
| 383 | [buchylx/create-dsh-content-plugin](https://github.com/buchylx/create-dsh-content-plugin) | 1 | 2026-08-26 | 2026-08-27 | Zero-dependency CLI that scaffolds a content-automation DSH plugin (Dev.to/GitHub/Bluesky/Mastodon). Like create-vite, for DSH. |
| 384 | [bug-huntter/dsh-vision-plugin](https://github.com/bug-huntter/dsh-vision-plugin) | 1 | 2026-09-03 | 2026-09-04 | 让你的deepseek拥有识图能力，配置简单，易上手 |
| 385 | [caopu16/dsh-local-memory](https://github.com/caopu16/dsh-local-memory) | 1 | 2026-08-27 | 2026-08-27 | DSH（DeepSeek Harness）本地跨会话记忆插件：捕获每轮对话摘要、注入最近几天记忆，并提供 memory_search 工具按需检索全部历史记忆。 |
| 386 | [carlclouder/dsh-image-serve](https://github.com/carlclouder/dsh-image-serve) | 1 | 2026-09-02 | 2026-09-03 | DeepSeek Harness 的本地文件展示插件：安装一次，会话 markdown 即可通过 /ws/<本地绝对路径> 直接渲染磁盘上任何位置的图片与文件。 |
| 387 | [Carrick-K7/dsh-plugin-source](https://github.com/Carrick-K7/dsh-plugin-source) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: group the Settings plugin list by origin (official/community), show version, upstream repo link and local-dev marker. Read-only, zero network. |
| 388 | [cat552/dsh-agent-quality-diagnosis](https://github.com/cat552/dsh-agent-quality-diagnosis) | 1 | 2026-09-01 | 2026-09-01 | Actionable quality diagnostics for DSH agent sessions, with tool-call evidence and next-step recommendations. |
| 389 | [cayan0x/Lume](https://github.com/cayan0x/Lume) | 1 | 2026-08-29 | 2026-08-31 | Lume - DSH Desktop persona-switching plugin (loli/senpai/none) with P0-P3 thinking logic |
| 390 | [ccll/dsh-activity-pane](https://github.com/ccll/dsh-activity-pane) | 1 | 2026-08-24 | 2026-08-29 | Activity session overview pane for DeepSeek Harness (DSH) web — running sessions, sub-agents, waiting-for-action reminders & recent history at a glance / DSH 活动会话总览窗格 |
| 391 | [Charlie-Wang-03/dsh-sightline](https://github.com/Charlie-Wang-03/dsh-sightline) | 1 | 2026-08-23 | 2026-08-27 | See the same repo through every agent's eyes — compare the effective instruction surfaces of DeepSeek Harness, Codex, and Claude Code. 查看同一仓库在 DeepSeek Harness、Codex 与 Claude Code 眼中的不同指令面。 |
| 392 | [chen731215-dev/dsh-muv-engine](https://github.com/chen731215-dev/dsh-muv-engine) | 1 | 2026-08-27 | 2026-08-27 | DSH Native MUV Engine - tavern companion: regex script execution, variable state tracking, iframe status bar rendering, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 393 | [chen731215-dev/dsh-muv-table](https://github.com/chen731215-dev/dsh-muv-table) | 1 | 2026-08-27 | 2026-08-27 | MUV Variable Table Editor - tavern companion plugin for DeepSeek Harness: structured table editing for UpdateVariable blocks, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 394 | [chendefine/dsh-sidebar-cdp-browser](https://github.com/chendefine/dsh-sidebar-cdp-browser) | 1 | 2026-08-19 | 2026-08-27 | deepseek harness live view chromium via cdp in sidebar tab |
| 395 | [chenhw7/dsh-memory](https://github.com/chenhw7/dsh-memory) | 1 | 2026-08-17 | 2026-09-04 | Cairn — long-term memory for the DeepSeek Harness (@chenhw7/dsh-memory). Persistent cross-session memory: facts, preferences, corrections, lessons. BM25 retrieval, three-layer scoping, human-confirmed writes. |
| 396 | [cherrchen/dsh-theme-studio](https://github.com/cherrchen/dsh-theme-studio) | 1 | 2026-08-26 | 2026-08-27 | 可移植的 DSH/Cordis 主题插件：内置配色浏览、预览、应用与持久化；DeepSeek Harness Desktop 预装。 / Portable DSH/Cordis theme overlay plugin with builtin palettes, preview, apply, and persistence; pre-installed in DeepSeek Harness Desktop. |
| 397 | [choco9527/dsh-add-to-chat](https://github.com/choco9527/dsh-add-to-chat) | 1 | 2026-09-03 | 2026-09-03 | DSH插件 引用注释 添加到对话功能 |
| 398 | [chongyangdu2008-cyrus/dsh-subagent-inspector](https://github.com/chongyangdu2008-cyrus/dsh-subagent-inspector) | 1 | 2026-08-28 | 2026-08-28 | Read-only live subagent process inspector for DeepSeek Harness Web |
| 399 | [CJYLZS/dsh-remote-development](https://github.com/CJYLZS/dsh-remote-development) | 1 | 2026-09-04 | 2026-09-04 | Remote development for DeepSeek Harness: pick a remote workspace over SSH and let the agent work on it with the same local tools. No extra model tools, no third-party UI plugin. |
| 400 | [Cmjingahaha/dsh-dudulu](https://github.com/Cmjingahaha/dsh-dudulu) | 1 | 2026-08-27 | 2026-08-27 | 嘟一声 · DSH 任务完成提示音插件：Agent 回合完成时播放提示音，带设置面板（音量/试听/上传） |
| 401 | [CNSeniorious000/dsh-py-codeact](https://github.com/CNSeniorious000/dsh-py-codeact) | 1 | 2026-08-28 | 2026-08-28 | Python-based CodeAct for dsh with persistent state across cells, replacing Dynamic Workflows and code-mode |
| 402 | [Co1ombiagly/prompt_optimize_dsh](https://github.com/Co1ombiagly/prompt_optimize_dsh) | 1 | 2026-08-30 | 2026-08-31 | DeepSeek Harness (DSH) 提示词优化器插件：一句口语化需求 → 结构化高质量提示词，结果自动填入会话输入框。复用 DSH 内置模型路由，零 API Key 管理。 |
| 403 | [conafun/dsh-music-plus](https://github.com/conafun/dsh-music-plus) | 1 | 2026-08-29 | 2026-08-29 | 基于 dsh-music-player 的修改版：移除在线QQ/酷狗/讲书/歌词，新增播客 |
| 404 | [crack-time/dsh-archive](https://github.com/crack-time/dsh-archive) | 1 | 2026-08-15 | 2026-08-31 | Session archive plugin for DSH web GUI |
| 405 | [crazy-L118/dsh-browser-ctrl](https://github.com/crazy-L118/dsh-browser-ctrl) | 1 | 2026-09-02 | 2026-09-04 | Built-in browser plugin for dsh (DeepSeek Harness) — lets the AI drive a real local browser (Edge/Chrome via CDP): navigate, read, click, type, with screenshots embedded straight into the chat. Guest-mode isolated, zero dependencies. |
| 406 | [crazy-L118/dsh-desktop-notify](https://github.com/crazy-L118/dsh-desktop-notify) | 1 | 2026-08-25 | 2026-08-27 | Desktop notification plugin for dsh: get a native OS toast when the AI finishes its reply. Toggle lives in dsh Settings → General. |
| 407 | [crazy-L118/dsh-personalization](https://github.com/crazy-L118/dsh-personalization) | 1 | 2026-08-28 | 2026-09-02 | A personalization plugin for DeepSeek Harness |
| 408 | [CSI-entitymorton/stavros-dsh-redteamer](https://github.com/CSI-entitymorton/stavros-dsh-redteamer) | 1 | 2026-08-29 | 2026-08-29 | Authorized-only AI red-team / pentest plugin for the DeepSeek Harness (DSH). Fail-closed scope guard: Stavros persona, 24 specialist subagents, 78 zero-dependency tools. |
| 409 | [CultOfLuna/dsh-vision-autoswitch](https://github.com/CultOfLuna/dsh-vision-autoswitch) | 1 | 2026-09-02 | 2026-09-02 | DeepSeek 的"自动挡"：有图切 Vision，无图回 Pro/Flash，一键都不用点。 DeepSeek's "automatic transmission": image in → Vision, image out → back to Pro/Flash — not a single click. |
| 410 | [cxy9204/dsh-skill-store](https://github.com/cxy9204/dsh-skill-store) | 1 | 2026-09-02 | 2026-09-02 | DeepSeek Harness 社区技能商店：浏览、搜索并一键安装来自 SkillHub / ClawHub / GitHub 的 13 万+ Agent Skills，支持星标排序与中文分类 |
| 411 | [cyanxi-eb/dsh-self-memory](https://github.com/cyanxi-eb/dsh-self-memory) | 1 | 2026-08-17 | 2026-09-03 | DSH 自记忆插件（v0.3）把会话中遇到的问题、多种解决方法、脚本文件路径与模型调用全过程结构化记录下来；新会话中，「先查记录 → 有就试 → 成功标命中/失败记根因 → 无则自研 → 最后回写」的闭环自动发生，并支持外部导入解决方法。零运行时依赖、纯本地、离线可用。 |
| 412 | [czj-git/dsh-plugin-hub](https://github.com/czj-git/dsh-plugin-hub) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness tools for searching and ranking verified plugins from DSH Plugin Hub |
| 413 | [D-Robotics/dsh-plugin-rdk](https://github.com/D-Robotics/dsh-plugin-rdk) | 1 | 2026-08-14 | 2026-08-28 | D-Robotics RDK (地瓜机器人) integration for DeepSeek Harness — native RDK skill catalog, rdk_skills browser tool, and rdk_board_detect device detection |
| 414 | [D2Moqi/dsh-openwiki](https://github.com/D2Moqi/dsh-openwiki) | 1 | 2026-08-29 | 2026-08-29 | DSH 插件：把 openwiki 的代码库知识库能力搬进 DeepSeek Harness —— 一键生成 / 阅读 / 更新仓库 Wiki 与 Grounded Claims（溯源知识卡片），直接复用 DSH 已配置的模型，无需二次填 Key。 |
| 415 | [d3vmeh/dsh-llm-gate](https://github.com/d3vmeh/dsh-llm-gate) | 1 | 2026-08-29 | 2026-08-29 | Per-provider concurrency gate for DeepSeek Harness model requests |
| 416 | [DahliaVoid/dsh-temp-session](https://github.com/DahliaVoid/dsh-temp-session) | 1 | 2026-08-28 | 2026-08-28 | dsh工作区可选化，100%纯AI coding产物 |
| 417 | [daishengli/dsh-docker](https://github.com/daishengli/dsh-docker) | 1 | 2026-08-27 | 2026-08-28 | 使用 Docker 封装运行 deepseek-harness d的 Web 服务。容器内运行 dsh 和 Caddy，宿主机通过 3080 端口访问服务。 |
| 418 | [DAIZHISEN/dsh-prompt-enhance](https://github.com/DAIZHISEN/dsh-prompt-enhance) | 1 | 2026-09-04 | 2026-09-04 | A DSH web plugin: a star button that rewrites drafts into clearer prompts, combining PromptForge rule diagnosis with your session's default model. Bilingual (English / Chinese). |
| 419 | [daodishisha28/dsh-sidechat-plugin](https://github.com/daodishisha28/dsh-sidechat-plugin) | 1 | 2026-08-30 | 2026-08-31 | Open a persistent side conversation from any DeepSeek Harness session to investigate questions, clarify requirements, or explore alternatives without polluting the main task’s context, then review and send a concise conclusion back to the parent conversation. Tested with DSH 0.1.2-alpha.1. |
| 420 | [dat-lequoc/dsh-opinionated-subagent](https://github.com/dat-lequoc/dsh-opinionated-subagent) | 1 | 2026-08-27 | 2026-08-28 | A minimal, opinionated subagent for DeepSeek Harness: you choose which models a child may run on and at which reasoning effort, and a correction reaches a working child at its next step |
| 421 | [DaYanQLQ/DSH-Balance-Mini](https://github.com/DaYanQLQ/DSH-Balance-Mini) | 1 | 2026-09-01 | 2026-09-02 | DeepSeek Harness 的极简版余额监视器插件：常驻余额徽章、红绿灯配色、多供应商、高峰/空闲时段。 |
| 422 | [DaYanQLQ/DSH-Shortcut](https://github.com/DaYanQLQ/DSH-Shortcut) | 1 | 2026-09-01 | 2026-09-02 | DeepSeek Harness 的 Windows 桌面快捷方式工具：双击智能启动/唤起、浏览器打开前自动最小化、崩溃一键重装救援（不删用户数据）。圆角官方图标，纯 PowerShell 零依赖。 |
| 423 | [DaydreAmRing/dsh-cho-kaguya-plugin-public](https://github.com/DaydreAmRing/dsh-cho-kaguya-plugin-public) | 1 | 2026-09-02 | 2026-09-02 | DSH皮肤插件、有超时空辉夜姬概念元素 |
| 424 | [DDDFXYqiming/dsh-session-recap](https://github.com/DDDFXYqiming/dsh-session-recap) | 1 | 2026-08-28 | 2026-08-28 | Session recap plugin for DeepSeek Harness (Claude Code-style away summaries) |
| 425 | [ddtcorex/dsh-maestro-ci](https://github.com/ddtcorex/dsh-maestro-ci) | 1 | 2026-08-26 | 2026-08-28 | Reusable GitHub Actions workflows for the Maestro suite — Cordis / DSH |
| 426 | [ddtcorex/dsh-maestro-config-lib](https://github.com/ddtcorex/dsh-maestro-config-lib) | 1 | 2026-08-25 | 2026-08-28 | Maestro settings store library — atomic namespaced JSON store shared by dsh-maestro-* plugins (embedded dependency, no Cordis row) |
| 427 | [ddtcorex/dsh-maestro-dashboard](https://github.com/ddtcorex/dsh-maestro-dashboard) | 1 | 2026-08-28 | 2026-08-28 | Maestro Dashboard — unified Control Center (Overview/Plugins/Usage) DSH-native |
| 428 | [ddtcorex/dsh-maestro-devkit](https://github.com/ddtcorex/dsh-maestro-devkit) | 1 | 2026-08-27 | 2026-08-28 | General development toolkit for DeepSeek Harness — visual review, HMR, style inspector, Cordis/Govard/Skills dev (tunnel-aware) |
| 429 | [ddtcorex/dsh-maestro-diagram](https://github.com/ddtcorex/dsh-maestro-diagram) | 1 | 2026-08-27 | 2026-08-28 | DSH Maestro diagram studio — mermaid_verify + mermaid_drift |
| 430 | [ddtcorex/dsh-maestro-supervisor](https://github.com/ddtcorex/dsh-maestro-supervisor) | 1 | 2026-08-27 | 2026-08-28 | Supervisor daemon for DSH Web resilience — auto-detect crashes, rollback to LKG, report |
| 431 | [ddtcorex/dsh-maestro-sync](https://github.com/ddtcorex/dsh-maestro-sync) | 1 | 2026-08-30 | 2026-09-01 | Maestro harness sync — merge memories and sessions across machines (publishable) |
| 432 | [delef/dsh-plugin-auto-review](https://github.com/delef/dsh-plugin-auto-review) | 1 | 2026-09-03 | 2026-09-03 | Provider-backed automatic approval review for DeepSeek Harness |
| 433 | [difimim/dsh-voice-input-npm](https://github.com/difimim/dsh-voice-input-npm) | 1 | 2026-08-30 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 434 | [dingyi580/dsh-plugin-gemini-theme](https://github.com/dingyi580/dsh-plugin-gemini-theme) | 1 | 2026-08-29 | 2026-08-30 | A Gemini-styled skin for the DeepSeek Harness web client |
| 435 | [DjangoAILab/dsh-plugins](https://github.com/DjangoAILab/dsh-plugins) | 1 | 2026-08-18 | 2026-09-01 | DeepSeek Harness plugins for browser automation, macOS computer use, external subagents, and guarded SSH operations. |
| 436 | [djs326/dsh-plugin-width-slider](https://github.com/djs326/dsh-plugin-width-slider) | 1 | 2026-09-03 | 2026-09-03 | 对话宽度滑块插件：DSH Desktop 设置面板滑块，按下即全屏预览实时调节对话宽度，自动隐藏原生拖拽手柄 |
| 437 | [domitor-syh/dsh-ui-skin-switcher](https://github.com/domitor-syh/dsh-ui-skin-switcher) | 1 | 2026-08-27 | 2026-08-28 | Model & reasoning-effort switcher plugin for DeepSeek Harness (DSH): composer seat with Off/Max effort slider. DSH 插件：模型与思考力度切换器。 |
| 438 | [doublehappy123/dsh-v4flash-tiler](https://github.com/doublehappy123/dsh-v4flash-tiler) | 1 | 2026-09-01 | 2026-09-01 | DSH plugin: auto-tiles oversized chat images into labelled grid tiles for DeepSeek v4Flash vision, with Python tiling engine |
| 439 | [doublemolu/dsh-costometer](https://github.com/doublemolu/dsh-costometer) | 1 | 2026-08-28 | 2026-09-01 | 花知多少 · Cost-O-Meter — DeepSeek Harness cost & balance meter: account balance, recharge history, per-conversation spend & tokens, 50-yuan segmented progress bar, low-balance guard, 8 languages & currencies with auto FX rates (CNY base). |
| 440 | [drscrewdriver/dsh-llm-openai-completions](https://github.com/drscrewdriver/dsh-llm-openai-completions) | 1 | 2026-08-29 | 2026-08-29 | dsh-llm-openai-completions |
| 441 | [duhu2000/dsh-data-cleaning-agent](https://github.com/duhu2000/dsh-data-cleaning-agent) | 1 | 2026-09-01 | 2026-09-01 | Data cleaning and enterprise enrichment agent plugin for DeepSeek Harness. |
| 442 | [dusbin/dsh-multi-tenant](https://github.com/dusbin/dsh-multi-tenant) | 1 | 2026-08-29 | 2026-08-29 | dsh 支持多租户插件 |
| 443 | [EastMG/dsh-gacha-calendar](https://github.com/EastMG/dsh-gacha-calendar) | 1 | 2026-08-27 | 2026-08-30 | DeepSeek Harness 二游卡池/活动排期速查插件：侧边栏按钮 内置 11 款主流二游 可添加自定义游戏 |
| 444 | [Edge-Echo/dsh-netassist](https://github.com/Edge-Echo/dsh-netassist) | 1 | 2026-08-30 | 2026-08-30 | Network & proxy assistant for DeepSeek Harness (dsh): one-shot GitHub connectivity check, system proxy status, proxy port probing, full diag chain and hosts conflict scan. |
| 445 | [Edge-Echo/dsh-win-toolkit](https://github.com/Edge-Echo/dsh-win-toolkit) | 1 | 2026-08-30 | 2026-08-30 | Windows-native capability pack for DeepSeek Harness (dsh): clipboard, notifications, hosts file, network diagnostics — safe PowerShell-backed tools. |
| 446 | [Elpsycoogroo/dsh-work-report](https://github.com/Elpsycoogroo/dsh-work-report) | 1 | 2026-08-28 | 2026-08-28 | Neural Ledger - turn DSH collaboration sessions into a visual work ledger: token analytics, smart insights, trend forecasting, and one-click daily/weekly/monthly Markdown reports. |
| 447 | [Entaum/dsh-free-games](https://github.com/Entaum/dsh-free-games) | 1 | 2026-08-30 | 2026-08-31 | Deepseek Harness free games plugin. Play while coding! |
| 448 | [EternalNight996/memory-eternal](https://github.com/EternalNight996/memory-eternal) | 1 | 2026-08-31 | 2026-08-31 | 记忆核心（Memory Eternal）：自研的 DeepSeek Harness 记忆插件——对话结束自动沉淀知识卡到本地 Markdown Vault（自研去重 / 自研 CJK 检索 / 知识图谱 + 审核中心 / 回收中心），Agent 通过 memory_recall 按需召回历史上下文，零人工干预。 |
| 449 | [exoticknight/dsh-theme-eink-retro](https://github.com/exoticknight/dsh-theme-eink-retro) | 1 | 2026-08-26 | 2026-08-27 | A paper-and-ink client-side theme for DeepSeek Harness with Balanced and Immersive modes. |
| 450 | [f1yan9/dsh-balance-pie](https://github.com/f1yan9/dsh-balance-pie) | 1 | 2026-08-30 | 2026-08-30 | DSH 插件：可拖拽余额饼图 / 真实消耗 / 历史热力图 — balance pie with real spending & monthly heatmap for DeepSeek Harness. |
| 451 | [falling-ts/dsh-web-ding](https://github.com/falling-ts/dsh-web-ding) | 1 | 2026-08-27 | 2026-08-27 | Browser-only 'ding' on agent end; works on servers.浏览器专属"叮":回合结束时响起,服务器部署也生效 |
| 452 | [fallow5/dsh-pin-sessions](https://github.com/fallow5/dsh-pin-sessions) | 1 | 2026-08-28 | 2026-08-31 | DSH (DeepSeek Harness) web plugin: pin sessions to the top of the sidebar for quick access to recurring workflows. Includes archive panel with batch delete, restore, and workspace grouping. |
| 453 | [fan56/dsh-dcp](https://github.com/fan56/dsh-dcp) | 1 | 2026-08-17 | 2026-08-28 | dsh plugin: deterministic context compression backend — zero LLM calls, reproducible compression |
| 454 | [fan56/dsh-llm-proxy](https://github.com/fan56/dsh-llm-proxy) | 1 | 2026-08-24 | 2026-09-01 | dsh plugin: per-host LLM outbound HTTP proxy routing (undici ProxyAgent) with a bundled dsh skill |
| 455 | [fan56/dsh-model-sync](https://github.com/fan56/dsh-model-sync) | 1 | 2026-08-28 | 2026-08-29 | A dsh (DeepSeek Harness) Cordis plugin that keeps llm-pi-ai provider routes' model catalog in sync with the pi.dev gateway — written through the official settings seam, zero patches to dsh internals. |
| 456 | [fan56/dsh-subagent-registry](https://github.com/fan56/dsh-subagent-registry) | 1 | 2026-08-16 | 2026-08-28 | dsh plugin: register ~/.dsh/agents/*.md as dsh-callable subagents |
| 457 | [fengb3/dsh-theme-aurum](https://github.com/fengb3/dsh-theme-aurum) | 1 | 2026-08-24 | 2026-08-28 | DSH 鎏金主题插件:金粉奢华皮肤,htm 恒等映射流水,原型驱动的逐节移植 |
| 458 | [ffdnm/ClashTUNWithDSH](https://github.com/ffdnm/ClashTUNWithDSH) | 1 | 2026-09-04 | 2026-09-04 | Enable DeepSeek Harness to use web_fetch normally under Clash TUN (fake-ip) mode |
| 459 | [Flan246/dsh-lit-search](https://github.com/Flan246/dsh-lit-search) | 1 | 2026-08-26 | 2026-08-27 | Academic literature search, citation and BibTeX tools for DeepSeek Harness and any agent (Crossref + OpenAlex). dsh plugin + CLI + SKILL.md. |
| 460 | [focksor/dsh-plugin-mini-dashboard](https://github.com/focksor/dsh-plugin-mini-dashboard) | 1 | 2026-08-28 | 2026-08-28 | A session & token mini dashboard for DSH web. It renders just above the sidebar's "Settings" row and summarizes, in one small draggable float window, what your sessions are doing right now and what they have cost you today. |
| 461 | [focksor/dsh-plugin-node-time](https://github.com/focksor/dsh-plugin-node-time) | 1 | 2026-08-29 | 2026-08-31 | Hover timestamps for DSH web. Hovering a chat node row — Think, Bash, Read/Edit/Write, Search, commands, compaction markers, sub-calls — pops a compact card with that node's start time → end time and how long it took. |
| 462 | [focksor/dsh-plugin-thinking-size](https://github.com/focksor/dsh-plugin-thinking-size) | 1 | 2026-08-28 | 2026-08-28 | A live reasoning-token badge for DSH web. It appends a compact Think(128) / Think(5.2K) marker to the title of every "Think" disclosure row in the conversation — ticking in real time while the model is still thinking, and staying put on history messages afterwards. |
| 463 | [FomoGoMan/dsh-serena-guide](https://github.com/FomoGoMan/dsh-serena-guide) | 1 | 2026-09-02 | 2026-09-02 | A DeepSeek Harness plugin that steers agents to Serena's LSP symbolic tools over built-in code tools. |
| 464 | [frank-fan-818/dsh-f1-skin](https://github.com/frank-fan-818/dsh-f1-skin) | 1 | 2026-09-01 | 2026-09-02 | An F1 Race Control themed skin for the DeepSeek Harness Web UI — Red Bull, Ferrari, McLaren & Mercedes team themes, broadcast-photo backdrops, and a native settings panel, in dark and light. |
| 465 | [FranklinZaneDurant/agent-discipline](https://github.com/FranklinZaneDurant/agent-discipline) | 1 | 2026-08-27 | 2026-08-27 | 给 AI 编码 Agent 的仓库工作纪律插件（DeepSeek Harness bundle）：方法论提示段 + 工件脚手架（AGENTS.md/特性清单/验证门）+ 合规审计。 |
| 466 | [freerpa/Hrequest](https://github.com/freerpa/Hrequest) | 1 | 2026-09-02 | 2026-09-02 | 轻量级 Node.js 多线程 API 压测工具，支持代理轮询、请求参数随机化注入和实时进度监控。 |
| 467 | [fufengyuan/dsh-council](https://github.com/fufengyuan/dsh-council) | 1 | 2026-08-26 | 2026-08-27 | dsh-council — 高智议会（Council of High Intelligence）for DeepSeek Harness 在 dsh（DeepSeek Harness）里召集历史人物议会，对复杂问题进行多视角结构化辩论，最终由主席综合裁决。 |
| 468 | [gaishilaji/dsh-plugin-cost](https://github.com/gaishilaji/dsh-plugin-cost) | 1 | 2026-09-02 | 2026-09-04 | deepseek harness插件，展示每轮对话的总消费及消费详情。 |
| 469 | [GalaxyBatMan111/dsh-plugins](https://github.com/GalaxyBatMan111/dsh-plugins) | 1 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) plugins: agent bridge (Claude Code/Codex/Marvis) + Ghidra reverse engineering bridge |
| 470 | [gbeta/dsh-token-speed](https://github.com/gbeta/dsh-token-speed) | 1 | 2026-09-02 | 2026-09-02 | DSH web plugin: draggable ring gauge showing live model output speed (tok/s) with per-step detail panel |
| 471 | [geecraft23/dsh-turn-colors](https://github.com/geecraft23/dsh-turn-colors) | 1 | 2026-09-02 | 2026-09-02 | Color-code user prompts and final assistant replies by conversation turn in the DeepSeek Harness Web UI. |
| 472 | [gengwg/dsh-kubectl-guard](https://github.com/gengwg/dsh-kubectl-guard) | 1 | 2026-09-01 | 2026-09-01 | A dsh policy plugin that gates kubectl by kubeconfig context: deny irreversible verbs outside local clusters, ask for the rest. |
| 473 | [georesearch-dsh/georesearch-dsh](https://github.com/georesearch-dsh/georesearch-dsh) | 1 | 2026-08-27 | 2026-08-28 | GeoResearch agent plugin for DeepSeek Harness |
| 474 | [Georgehaoren/DSH-WhaleConsole](https://github.com/Georgehaoren/DSH-WhaleConsole) | 1 | 2026-08-29 | 2026-08-29 | Unofficial macOS desktop companion and WebUI skin plugin for DeepSeek Harness. 面向 DeepSeek Harness 的非官方 macOS 桌面伴侣与 WebUI 换肤插件。 |
| 475 | [goldgish/dsh-agent-trace](https://github.com/goldgish/dsh-agent-trace) | 1 | 2026-08-26 | 2026-08-27 | Agent Trace — visualize an agent's reasoning, parallel tool calls, and results as an interactive DAG inside DeepSeek Harness. |
| 476 | [GooDAnDReaDY/dsh-messenger-gateway](https://github.com/GooDAnDReaDY/dsh-messenger-gateway) | 1 | 2026-08-26 | 2026-08-27 | Telegram messenger bridge for DeepSeek Harness: sessions, steer, homes, and TTS voice notes |
| 477 | [GuionAI/web](https://github.com/GuionAI/web) | 1 | 2026-08-22 | 2026-08-30 | A web research toolkit with multi-provider search and clean Markdown extraction from static and JavaScript-rendered pages, plus public code and library docs search—available via CLI and MCP. |
| 478 | [GuoCheng24/breakthrough-harness](https://github.com/GuoCheng24/breakthrough-harness) | 1 | 2026-08-28 | 2026-09-04 | Make your research agent hard to fool — the discipline layer for agentic research: breakthrough loop, hard-to-fool harness checklist, claim-polarity gates, engineering rules with their tuition |
| 479 | [gychen-NJU/dsh-overleaf](https://github.com/gychen-NJU/dsh-overleaf) | 1 | 2026-08-27 | 2026-08-29 | Embedded Overleaf workbench tab for DeepSeek Harness Web: same-origin reverse proxy, direct-CDP login, selection quoting, caret insertion, LaTeX assist panel |
| 480 | [hakimedes/dsh-easyremote](https://github.com/hakimedes/dsh-easyremote) | 1 | 2026-08-25 | 2026-09-01 | Local-first Android remote workspace with one-command Cloudflare Tunnel setup |
| 481 | [hanrr92/dsh-code-quote](https://github.com/hanrr92/dsh-code-quote) | 1 | 2026-09-01 | 2026-09-01 | 代码引用 |
| 482 | [hardes11/dsh-squeeze-command](https://github.com/hardes11/dsh-squeeze-command) | 1 | 2026-09-02 | 2026-09-03 | Manual budget-targeted context compression for DeepSeek Harness: the conversation model picks ranges, a cheap flash-tier route writes the summaries. |
| 483 | [hejielijob-commits/SemaRail](https://github.com/hejielijob-commits/SemaRail) | 1 | 2026-08-17 | 2026-08-30 | Governed semantic layer for AI agents, with a DeepSeek Harness plugin that turns Harness into a data agent. |
| 484 | [helloproblems/dsh-browser-use](https://github.com/helloproblems/dsh-browser-use) | 1 | 2026-09-03 | 2026-09-03 | 为 DeepSeek Harness (DSH) 插件生态打造的浏览器自动化插件 |
| 485 | [henrychenhao/dsh-skin-argentina](https://github.com/henrychenhao/dsh-skin-argentina) | 1 | 2026-08-27 | 2026-08-27 | 梅西 阿根廷皮肤 |
| 486 | [HenryPhoebe/dsh-plugin-easyppt](https://github.com/HenryPhoebe/dsh-plugin-easyppt) | 1 | 2026-08-27 | 2026-08-27 | easyppt是一个面向 DeepSeek Harness (DSH) 的演示文稿生成 dsh-plugin（npm 包 + Cordis bundle + 内置技能）。用户输入大纲（Markdown / JSON / 自然语言）与插图，即可基于 DSH 原生 Univer 工具链生成PPTX,HTML,JSON |
| 487 | [hgl011091/dsh-rss-monitor](https://github.com/hgl011091/dsh-rss-monitor) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 原生 RSS 订阅监控插件：多源订阅、关键词过滤、定时检查去重、新条目邮件通知（缩略图 HTML 模板），SMTP 密码走凭据库永不落盘，原生设置页四页签体验。 |
| 488 | [himovo/movo](https://github.com/himovo/movo) | 1 | 2026-09-01 | 2026-09-04 | Turn DeepSeek Harness into a self-hosted enterprise Agent platform with knowledge, research, content generation, governance, and admin controls. |
| 489 | [hjj345/dsh-sm-context-piano](https://github.com/hjj345/dsh-sm-context-piano) | 1 | 2026-08-21 | 2026-08-29 | DeepSeek Harness Web GUI 的 Codex 风格对话导航器：帮助用户快速浏览、定位和切换对话，提升多任务、多会话场景下的工作效率。 \|  Codex-style conversation navigator for the DeepSeek Harness Web GUI. |
| 490 | [hjj345/dsh-sm-version-display](https://github.com/hjj345/dsh-sm-version-display) | 1 | 2026-08-28 | 2026-08-30 | 用于在侧边栏“设置”按钮上方显示已安装 dsh 版本的 DeepSeek Harness Web 插件。  \|  DeepSeek Harness Web plugin that displays the installed dsh version above the sidebar Settings button. |
| 491 | [hotpot-labs/dsh-version-plugin](https://github.com/hotpot-labs/dsh-version-plugin) | 1 | 2026-08-28 | 2026-09-02 | 展示dsh版本，提供更新到最新版按钮 |
| 492 | [HOWILLMAKEIT/dsh-model-context-catalog](https://github.com/HOWILLMAKEIT/dsh-model-context-catalog) | 1 | 2026-09-01 | 2026-09-01 | DeepSeek Harness 插件：维护 llm-pi-ai 模型的准确上下文窗口，避免长会话被误判为上下文溢出。 |
| 493 | [hoyyang/dsh-concise](https://github.com/hoyyang/dsh-concise) | 1 | 2026-09-02 | 2026-09-02 | One-click Concise output style for DeepSeek Harness: results first, no filler — Claude Code's built-in Concise style as a dsh plugin. Toggle right of the model picker, global, persistent, zero-config. |
| 494 | [HuanLinOTO/dsh-plugin-better-glob](https://github.com/HuanLinOTO/dsh-plugin-better-glob) | 1 | 2026-08-30 | 2026-08-30 | 以 per-agent 阴影顶替内置 glob：自动排除无底洞目录（node_modules 等），传 include 白名单才能搜入 \| Shadows the built-in glob per agent: auto-excludes bottomless directories (node_modules etc.), pass an include whitelist to search inside them |
| 495 | [huhaodong/dsh-auto-driving](https://github.com/huhaodong/dsh-auto-driving) | 1 | 2026-09-02 | 2026-09-02 | 让 DeepSeek Harness 智能体进入自动驾驶 🚗：模型故障自动回退、静默卡死自动保活重试、权限/提问/方案审批自动放行，AUTO-MODE.md 全程审计——无人值守、永不停摆的自愈式 AI 编码会话。 |
| 496 | [iasiv5/skins](https://github.com/iasiv5/skins) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness Web 界面主题/皮肤管理插件，可切换多种视觉风格。 |
| 497 | [Idreamxkl/dsh-conversation-flat](https://github.com/Idreamxkl/dsh-conversation-flat) | 1 | 2026-08-30 | 2026-08-30 | Document-flow conversation layout for DeepSeek Harness web GUI — full-width column, user message bars, sender label, full-width tables. 纯 CSS 的 dsh 对话区通栏布局插件 |
| 498 | [iimaguest/dsh-contradictions-indicator](https://github.com/iimaguest/dsh-contradictions-indicator) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin: 0-100 conversation coherence badge with parallel contradiction analysis |
| 499 | [IKEASven69/dsh-opencli](https://github.com/IKEASven69/dsh-opencli) | 1 | 2026-08-30 | 2026-08-30 | 让 DeepSeek Harness (dsh) 会办事:登录态真实浏览器 + 170+ 站点适配器 + write 审批门 |
| 500 | [ilovedyou6666-hub/dshtools-sensevoice-input](https://github.com/ilovedyou6666-hub/dshtools-sensevoice-input) | 1 | 2026-09-03 | 2026-09-04 | 基于 SenseVoiceSmall（iic/SenseVoiceSmall）多语言语音理解模型的 DSH Desktop 本地语音输入插件。 |
| 501 | [JasonFreeLab/dsh-superpowers](https://github.com/JasonFreeLab/dsh-superpowers) | 1 | 2026-08-28 | 2026-08-28 | DSH (DeepSeek Harness) port of obra/superpowers — 14 native skills for multi-agent software development: brainstorming, planning, TDD, systematic debugging, and code review. |
| 502 | [jeffxuan/dsh-godot-game-studio](https://github.com/jeffxuan/dsh-godot-game-studio) | 1 | 2026-09-03 | 2026-09-03 | Seven bounded Godot 4 MCP tools for DeepSeek Harness: audit, test, simulate, validate, and release |
| 503 | [jeffy-Peng/deepseek-harness-usage](https://github.com/jeffy-Peng/deepseek-harness-usage) | 1 | 2026-08-16 | 2026-08-28 | DeepSeek Harness 插件，显示每日消费与账户总余额。DeepSeek Harness plugin for account balance and evidence-bounded daily CNY consumption |
| 504 | [Jensen-Yao/dsh-model-palette](https://github.com/Jensen-Yao/dsh-model-palette) | 1 | 2026-08-26 | 2026-08-27 | Global provider-aware model command palette and optional OpenRouter media tools for DeepSeek Harness. |
| 505 | [JerryXst/dsh-codex-web-auth](https://github.com/JerryXst/dsh-codex-web-auth) | 1 | 2026-09-01 | 2026-09-02 | ChatGPT / Codex browser sign-in for DeepSeek Harness's built-in openai-codex provider — no OpenAI API key required. |
| 506 | [jetheaven/dsh-code-reviewer](https://github.com/jetheaven/dsh-code-reviewer) | 1 | 2026-08-14 | 2026-08-27 | AI代码审查插件：bug检测/安全漏洞/性能/风格四维审查，行号定位+修复示例 |
| 507 | [jetheaven/dsh-content-rewriter](https://github.com/jetheaven/dsh-content-rewriter) | 1 | 2026-08-14 | 2026-08-27 | 一键内容改写：小红书/知乎/商务邮件/精简/扩写/Twitter 多风格 |
| 508 | [jetheaven/dsh-data-extractor](https://github.com/jetheaven/dsh-data-extractor) | 1 | 2026-08-14 | 2026-08-27 | 结构化数据提取：从非结构化文本提取字段，输出 JSON/CSV/表格 |
| 509 | [jetheaven/dsh-meeting-notes](https://github.com/jetheaven/dsh-meeting-notes) | 1 | 2026-08-14 | 2026-08-27 | 会议纪要智能生成：从转写文本提取决议/待办/负责人/截止时间/风险 |
| 510 | [jetheaven/dsh-prompt-optimizer](https://github.com/jetheaven/dsh-prompt-optimizer) | 1 | 2026-08-14 | 2026-08-27 | AI提示词优化器：诊断Prompt问题并输出结构化高质量优化版本 |
| 511 | [jetheaven/dsh-seo-writer](https://github.com/jetheaven/dsh-seo-writer) | 1 | 2026-08-14 | 2026-08-27 | SEO文章生成器：给定关键词和语言，生成搜索引擎友好的完整文章 |
| 512 | [jetheaven/dsh-text-diff](https://github.com/jetheaven/dsh-text-diff) | 1 | 2026-08-14 | 2026-08-27 | AI智能文本对比：找出两段文字的差异、语义变化和潜在风险点 |
| 513 | [jetheaven/dsh-translate-pro](https://github.com/jetheaven/dsh-translate-pro) | 1 | 2026-08-14 | 2026-08-27 | 专业翻译：术语一致、专业领域选择与语气调整，附带术语对照表 |
| 514 | [jhckevin/dsh-auto-review](https://github.com/jhckevin/dsh-auto-review) | 1 | 2026-09-03 | 2026-09-03 | Codex-style Auto Review inspired plugin for DeepSeek Harness, with native bridge and Linux sandbox integration |
| 515 | [jiangliuhong/dsh-gpt-oauth](https://github.com/jiangliuhong/dsh-gpt-oauth) | 1 | 2026-08-26 | 2026-08-27 | openai models for login by chatgpt |
| 516 | [JianwuYang/dsh-ui-kanban](https://github.com/JianwuYang/dsh-ui-kanban) | 1 | 2026-08-27 | 2026-08-27 | 让 agent 直接干 Jira/GitLab 的活 · DSH 看板插件 \| A dsh plugin that turns Jira + GitLab into an agent-workable kanban board |
| 517 | [jianxx/dsh-cc](https://github.com/jianxx/dsh-cc) | 1 | 2026-08-15 | 2026-08-28 | Bring the Claude Code workflow to DeepSeek Harness - TUI, permissions, hooks, memory, skills, subagents, MCP, worktrees, and more. |
| 518 | [JJXjustin/dsh-session-rewind](https://github.com/JJXjustin/dsh-session-rewind) | 1 | 2026-08-31 | 2026-08-31 | DSH session and file rewind plugin (shadow git repo) |
| 519 | [jkStars/dsh-token-usage-stats](https://github.com/jkStars/dsh-token-usage-stats) | 1 | 2026-08-22 | 2026-09-01 | DSH plugin: cross-session token usage analytics with a web dashboard (ctx.tokenUsageStats) |
| 520 | [jkt-check/dsh-secret-scrub](https://github.com/jkt-check/dsh-secret-scrub) | 1 | 2026-09-02 | 2026-09-02 | Irreversible secret-scrubbing guard plugin for DeepSeek Harness (dsh): regex redaction of secrets before session-log persistence and model requests |
| 521 | [jn18755/dsh-skill-nannan](https://github.com/jn18755/dsh-skill-nannan) | 1 | 2026-08-27 | 2026-08-27 | DSH 插件：基于《地狱磨砺》(Hell Grind) 方法论的 AI 视频提示词规范（29 条规则，已去除压力测试阶段） |
| 522 | [Jonah-Wu23/dsh-gungnir](https://github.com/Jonah-Wu23/dsh-gungnir) | 1 | 2026-09-01 | 2026-09-01 | Lock the goal. Adapt the loop. Prove the hit. |
| 523 | [Jstn-1g/dsh-live-voice](https://github.com/Jstn-1g/dsh-live-voice) | 1 | 2026-08-25 | 2026-08-28 | DSH Live Voice: consent-bound one-turn voice for DeepSeek Harness, with a credential-free local synthetic demo, exact-Session isolation, and explicit draft handoff. |
| 524 | [junwei529/work-charter-dsh](https://github.com/junwei529/work-charter-dsh) | 1 | 2026-08-28 | 2026-08-30 | DSH-native Work Charter policy plugin backed by session-coordinator-dsh |
| 525 | [jypjypjypjyp/dsh-notifier](https://github.com/jypjypjypjyp/dsh-notifier) | 1 | 2026-08-27 | 2026-08-27 | 审批/完成/错误事件通知：浏览器 Notification + 系统原生 toast（Windows PowerShell WinRT / macOS osascript / Linux notify-send，均无需额外安装）；提示音可配、每条通知独立显示不互相替换、非安全上下文自动降级横幅 |
| 526 | [Kaiji-Z/dsh-plugin-stardeck](https://github.com/Kaiji-Z/dsh-plugin-stardeck) | 1 | 2026-08-30 | 2026-09-01 | RTS-style multi-agent orchestration board for DeepSeek Harness: issue plain-language strategic orders, a staff agent drafts acceptance-checked task orders, commander agents deploy typed subagent troops on isolated workspaces — with a 3D starfield campaign view, append-only event logs, and machine-checked verification. |
| 527 | [kaixinguo360/dsh-script-manager](https://github.com/kaixinguo360/dsh-script-manager) | 1 | 2026-09-03 | 2026-09-03 | DSH 自定义操作脚本管理插件，将验证过的操作流程固化为可复用脚本，不耗 token、支持参数化和执行验收。 |
| 528 | [KannaKuron/dsh-agent-lang](https://github.com/KannaKuron/dsh-agent-lang) | 1 | 2026-08-31 | 2026-08-31 | Agent language control: DSH plugin — tool-call descriptions, model thinking, and replies each follow the GUI language, force a fixed language, or turn off; injected as one global runtime-context directive. \| Agent 语言控制:DSH 插件——工具描述、模型思考、回复输出三通道各自跟随界面语言 / 强制指定 / 关闭,以全局 runtime-context 注入,不改任何 preset。 |
| 529 | [keman-ai/dsh-opencode-zen](https://github.com/keman-ai/dsh-opencode-zen) | 1 | 2026-08-19 | 2026-08-27 | Bring OpenCode Zen's free models to DeepSeek Harness — zero config, no API key, catalog discovered live from upstream |
| 530 | [keman-ai/dsh-pocket](https://github.com/keman-ai/dsh-pocket) | 1 | 2026-09-02 | 2026-09-02 | Watch and steer your DSH agent from a phone browser: approve tool calls, send a message, stop a turn |
| 531 | [kenny2077/dsh-web-search-doubao](https://github.com/kenny2077/dsh-web-search-doubao) | 1 | 2026-08-29 | 2026-08-29 | Doubao Search provider for the DeepSeek Harness |
| 532 | [kenny2077/dsh-web-search-zai](https://github.com/kenny2077/dsh-web-search-zai) | 1 | 2026-08-28 | 2026-08-28 | GLM/ZAI web search for DeepSeek Harness: Coding Plan quota or REST API billing |
| 533 | [KevinZhangNothing/dsh-task-graph](https://github.com/KevinZhangNothing/dsh-task-graph) | 1 | 2026-08-27 | 2026-08-27 | Task flow / execution graph plugin for DeepSeek Harness (DSH) — visualize a single task's full run: agents, tools, skills, subtasks, retries, live status. DSH 单任务执行流程图谱插件。 |
| 534 | [KhalilHsu/dsh-plugins](https://github.com/KhalilHsu/dsh-plugins) | 1 | 2026-08-17 | 2026-08-28 | Enhance DeepSeek Harness Web GUI with smart per-turn reasoning/tool folding and query navigation. |
| 535 | [KhaosGx/dsh-stop-service](https://github.com/KhaosGx/dsh-stop-service) | 1 | 2026-09-04 | 2026-09-04 | DSH 设置页「服务控制」：实时服务信息 + 优雅终止按钮，不留孤儿进程。 / A service panel for DeepSeek Harness Web: live host info + graceful stop. |
| 536 | [kiligzzz/dsh-agent-dispatch](https://github.com/kiligzzz/dsh-agent-dispatch) | 1 | 2026-08-28 | 2026-08-28 | DSH 插件：预置专家 agent + 自动路由 + 小队编排。原生右 tab「Agent 调度」+ 悬浮活动球 +  触发器。 |
| 537 | [koompi/dsh-desktop](https://github.com/koompi/dsh-desktop) | 1 | 2026-09-02 | 2026-09-02 | Electron desktop shell for DeepSeek Harness: runs the published dsh CLI as a sidecar |
| 538 | [l-vM2k/dsh-ayaka-theme](https://github.com/l-vM2k/dsh-ayaka-theme) | 1 | 2026-08-28 | 2026-08-28 | deepseek harness plugins dsh-ayaka-theme |
| 539 | [LamplitIsles/kepos-hindsight](https://github.com/LamplitIsles/kepos-hindsight) | 1 | 2026-08-28 | 2026-09-04 | hindsight memory for companion agent in dsh |
| 540 | [LamplitIsles/kepos-imagegen](https://github.com/LamplitIsles/kepos-imagegen) | 1 | 2026-08-27 | 2026-08-30 | Image generation tools via kepos exposed codex endpoint |
| 541 | [Leon00x/deepseek-harness-desktop](https://github.com/Leon00x/deepseek-harness-desktop) | 1 | 2026-09-04 | 2026-09-04 | Linux native desktop client for DeepSeek Harness — download & run, connects to your local Harness out of the box (Tauri 2 / WebKitGTK) |
| 542 | [lewes2/archpresent](https://github.com/lewes2/archpresent) | 1 | 2026-08-29 | 2026-08-29 | Agent skill: generate beautiful dark-themed architecture diagrams from your project/demo/idea. Interactive, verifiable, and editable. Delivered as self-contained HTML. |
| 543 | [lgquan/dsh-voco](https://github.com/lgquan/dsh-voco) | 1 | 2026-08-27 | 2026-08-27 | Persistent voice conversations for DSH with cloud speech recognition, Edge TTS, and background Agent delegation. |
| 544 | [lhh010/dsh-file-trace](https://github.com/lhh010/dsh-file-trace) | 1 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 545 | [LHKong7/dsh-browser-runtime](https://github.com/LHKong7/dsh-browser-runtime) | 1 | 2026-08-26 | 2026-08-27 | deepseek harness plugin browser runtime |
| 546 | [liceses/dsh-hmm-wait](https://github.com/liceses/dsh-hmm-wait) | 1 | 2026-08-22 | 2026-08-27 | 化口水为乐趣，把大肥鱼流的口水变成游戏连击！ |
| 547 | [liiiubai/dsh-mcp-bridge](https://github.com/liiiubai/dsh-mcp-bridge) | 1 | 2026-08-28 | 2026-08-28 | Expose DeepSeek Harness tools as a standard MCP server (streamable HTTP) — drive dsh from Claude Code, Codex, or any MCP client |
| 548 | [lijian-ui/dsh-file-manager](https://github.com/lijian-ui/dsh-file-manager) | 1 | 2026-08-18 | 2026-08-27 | 为 DeepSeek Harness 桌面端（dsh web）开发的插件：聊天区右侧的 Explorer 文件面板 + Preview 预览面板（FileManager 风格，Apache-2.0 参考实现非抄录），以及输入框 @ 引用项目文件（树形多选弹窗 + 输入框内胶囊 + 行号） |
| 549 | [lijian-ui/dsh-schedule-view](https://github.com/lijian-ui/dsh-schedule-view) | 1 | 2026-08-24 | 2026-08-27 | A cron-based scheduled task plugin for DeepSeek Harness (dsh) desktop: create / edit / delete / fire-now tasks from the settings panel, with cross-session agent follow-up and multi-level notifications. Zero LLM tools — purely human-driven scheduling. |
| 550 | [lijian-ui/dsh-skill-manage](https://github.com/lijian-ui/dsh-skill-manage) | 1 | 2026-08-22 | 2026-08-27 | A skill management plugin for DeepSeek Harness (dsh) desktop: list / enable / disable / delete / add skills, filling the gap in dsh's official skill toggle control. |
| 551 | [lijian-ui/dsh-term](https://github.com/lijian-ui/dsh-term) | 1 | 2026-08-19 | 2026-08-27 | Panel-style local terminal for the DSH web GUI. |
| 552 | [lijian-ui/dsh-vision-toggle](https://github.com/lijian-ui/dsh-vision-toggle) | 1 | 2026-08-28 | 2026-08-28 | dsh-vision-toggle 是一个为 DeepSeek Harness (dsh) 提供「支持图片」开关的插件，让你在设置页按模型一键启用/禁用图片输入 |
| 553 | [LiLiLi-Zi/dsh-gray-test](https://github.com/LiLiLi-Zi/dsh-gray-test) | 1 | 2026-09-02 | 2026-09-02 | dsh gray-model detection plugin — launch N concurrent sessions, stream reasoning chains, auto-classify gray models (I'm+ing > Let me×5), normal models (Let me≥3), and abnormal models (no features). Supports standard/PTC/minimal/cordis presets. |
| 554 | [linfengyu94/dsh-balance-panel](https://github.com/linfengyu94/dsh-balance-panel) | 1 | 2026-09-01 | 2026-09-01 | DeepSeek 充值余额悬浮面板 - DSH 插件：悬浮显示充值余额，带可视化进度条与动态按钮动画 |
| 555 | [LLYlab/DSHEssentialTools](https://github.com/LLYlab/DSHEssentialTools) | 1 | 2026-08-27 | 2026-08-28 | DSH 永久插件：LVAL 工程运行/代码查看/程序版本快照回退 + VTD 虚拟对话树（编辑/重试/分支、消息小版本）+ DET 管理器。A permanent DeepSeek Harness plugin: project run & code viewer, program snapshots, an in-session conversation tree (edit/retry/branches), message micro-versions and a feature manager. |
| 556 | [LONGSASASASASA/dsh-issue2pr](https://github.com/LONGSASASASASA/dsh-issue2pr) | 1 | 2026-08-29 | 2026-08-30 | 从一条 Issue 到一份被合并的 PR，每一段都有自己的输入契约、失败信号、可回滚产物与可独立审查的 Artifact。 |
| 557 | [looput/dsh-finance-lab](https://github.com/looput/dsh-finance-lab) | 1 | 2026-08-18 | 2026-08-27 | DeepSeek Harness finance plugin: direct market HTTP APIs, portfolio settings, model tools |
| 558 | [LouisCanBe/dsh-plugin-ollama-monitor](https://github.com/LouisCanBe/dsh-plugin-ollama-monitor) | 1 | 2026-09-02 | 2026-09-02 | Ollama 监控与测评平台 · DeepSeek Harness (DSH) 插件组合包：agent 工具 + Web 设置页面板（npm: ollama-monitor） |
| 559 | [louishzwang/dsh-web-launcher](https://github.com/louishzwang/dsh-web-launcher) | 1 | 2026-08-21 | 2026-08-31 | DSH Web本地终端启动脚本 |
| 560 | [lovaxi/Rubato_Device](https://github.com/lovaxi/Rubato_Device) | 1 | 2026-08-30 | 2026-09-01 | Rubato - a palm-sized retro-Macintosh AI desk companion that turns AI wait time into gentle health breaks. Firmware, tools and docs. |
| 561 | [lrplrplrp/dsh-live2d](https://github.com/lrplrplrp/dsh-live2d) | 1 | 2026-09-01 | 2026-09-02 | deepseek-harness对live2d的支持 |
| 562 | [luckycaoj/dsh-plugin-session-console-sleepcat](https://github.com/luckycaoj/dsh-plugin-session-console-sleepcat) | 1 | 2026-08-31 | 2026-08-31 | 一个dsh的辅助使用小插件，DSH client plugin: embedded tool rail + session questions console — jump to past questions, collapse the model's working process. 🐱 |
| 563 | [lumose0/dsh-file-reference-everything](https://github.com/lumose0/dsh-file-reference-everything) | 1 | 2026-08-27 | 2026-08-27 | Whole-disk @ file references for DeepSeek Harness — Everything-backed instant search with fuzzy/regex and a cross-platform fallback index |
| 564 | [Lunatic029/dsh-clash-proxy](https://github.com/Lunatic029/dsh-clash-proxy) | 1 | 2026-08-27 | 2026-08-27 | Route DeepSeek Harness's outbound network through Clash — LLM, web search/fetch and shell commands all use your local Clash proxy. |
| 565 | [Luv061211/dsh-pet](https://github.com/Luv061211/dsh-pet) | 1 | 2026-08-30 | 2026-09-03 | Customizable desktop pets for DeepSeek Harness — import your own sprite-based pet packs, reflect agent activity, and use them in the Web UI or an optional Electron companion. |
| 566 | [lxwallac/dsh-vault-wall](https://github.com/lxwallac/dsh-vault-wall) | 1 | 2026-09-04 | 2026-09-04 | 让 DeepSeek Harness 感知不到/无法操作指定敏感路径的隔离墙插件（Vault Wall） |
| 567 | [Lzh3070/dsh-model-visibility](https://github.com/Lzh3070/dsh-model-visibility) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件：模型可见性管理——按渠道/模型隐藏或显示模型选择菜单里的条目 / Control which models appear in the DSH model selector |
| 568 | [m1khal3v/dsh-tool-codegraph](https://github.com/m1khal3v/dsh-tool-codegraph) | 1 | 2026-08-29 | 2026-08-30 | CodeGraph navigation tools for DeepSeek Harness |
| 569 | [makajo/dsh-gemini-m3e-theme](https://github.com/makajo/dsh-gemini-m3e-theme) | 1 | 2026-08-29 | 2026-08-30 | Gemini-style Material 3 Expressive theme for DeepSeek Harness Web (persistent client bundle) |
| 570 | [Mandarin715/dsh-mobile-access-plugin](https://github.com/Mandarin715/dsh-mobile-access-plugin) | 1 | 2026-09-04 | 2026-09-04 | DSH 手机远程通道插件：一键生成并部署 frp 隧道 + Basic Auth 反代 + 开机自启（通用，不锁 DSH 发行版） |
| 571 | [mapan0424/deepseek-harness-plugins](https://github.com/mapan0424/deepseek-harness-plugins) | 1 | 2026-09-02 | 2026-09-02 | Unofficial community plugins collection for DeepSeek Harness |
| 572 | [mastergo-design/dsh-canvas](https://github.com/mastergo-design/dsh-canvas) | 1 | 2026-08-27 | 2026-08-27 | MasterGo Canvas MCP plugin for DeepSeek Harness |
| 573 | [me93-ghb/dsh-matrix-think](https://github.com/me93-ghb/dsh-matrix-think) | 1 | 2026-08-27 | 2026-08-27 | Matrix rain for expanded thinking in DeepSeek Harness Web |
| 574 | [mengnanxyyyy/dsh-markdown-xyy](https://github.com/mengnanxyyyy/dsh-markdown-xyy) | 1 | 2026-08-29 | 2026-08-29 | dsh markdown 主题插件 |
| 575 | [MerlinShieh/Agent-skill-wechatPush](https://github.com/MerlinShieh/Agent-skill-wechatPush) | 1 | 2026-08-03 | 2026-09-02 | Agent skill，当任务完成时会主动通过微信公众号推送洗洗脑 |
| 576 | [MerlinShieh/AgentMemHub](https://github.com/MerlinShieh/AgentMemHub) | 1 | 2026-08-25 | 2026-08-27 | 统一提取多 Agent Harness 会话为全量事件流(含工具链/思维链/Shell/补丁) → SQLite 检索 → 桥接 MemOS 生成记忆 |
| 577 | [ming-xia/dsh-stickies](https://github.com/ming-xia/dsh-stickies) | 1 | 2026-09-03 | 2026-09-03 | 面向 DeepSeek Harness 的本地优先 Markdown 便利贴插件 |
| 578 | [Missher12/deepseek-harness-desktop](https://github.com/Missher12/deepseek-harness-desktop) | 1 | 2026-08-13 | 2026-08-29 | Unofficial Intel macOS desktop app for DeepSeek Harness |
| 579 | [mldhao/dsh-conversation-strip](https://github.com/mldhao/dsh-conversation-strip) | 1 | 2026-08-27 | 2026-08-27 | Codex-inspired vertical conversation-turn rail for the DeepSeek Harness web UI. |
| 580 | [moonlin1213/dsh-agent-sound-alert](https://github.com/moonlin1213/dsh-agent-sound-alert) | 1 | 2026-08-29 | 2026-08-29 | macOS sound alerts for DeepSeek Harness agent lifecycle events |
| 581 | [Movingtoleveltwo/dsh-revert](https://github.com/Movingtoleveltwo/dsh-revert) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 现代化对话回退与重试插件：纯 UI 图形交互、原地 Prompt 微调、支持工作区与外部文件双引擎安全恢复。 |
| 582 | [mtdx2001/think-zh](https://github.com/mtdx2001/think-zh) | 1 | 2026-08-29 | 2026-08-29 | AI reasoning real-time Chinese localization suite (DSH ready, OpenAI-compatible endpoint) |
| 583 | [MuAllen/dsh-gateway-wallet](https://github.com/MuAllen/dsh-gateway-wallet) | 1 | 2026-08-24 | 2026-08-27 | 读取当前 API key 在站点账本上的剩余额度和实扣，支持 Sub2API、New API 与 DeepSeek 官方，不是本地 token 估算。 |
| 584 | [mumuer1024/dsh-ui-liteglass](https://github.com/mumuer1024/dsh-ui-liteglass) | 1 | 2026-08-21 | 2026-08-27 | LiteGlass — a lightweight appearance skin for DeepSeek Harness Web UI: wallpaper, glass-like transparency, and accent color. Server-side settings, multi-device, leaves native light/dark mode alone. |
| 585 | [MurasakiIzumi/dsh-ticker-jp](https://github.com/MurasakiIzumi/dsh-ticker-jp) | 1 | 2026-09-04 | 2026-09-04 | DeepSeek Harness 的悬浮行情插件（日股改版）：在页面右上角显示一个可拖拽、可收起的半透明小窗，实时展示 TOPIX 联动 ETF 与日经225，并可自选任意 Yahoo 代码（支持自定义显示名）。 |
| 586 | [my-dsh/dsh-web-search-tavily](https://github.com/my-dsh/dsh-web-search-tavily) | 1 | 2026-08-30 | 2026-08-30 | Tavily web-search provider plugin for DeepSeek Harness (dsh) — registers into ctx.web so the model-facing web_search tool uses Tavily |
| 587 | [mycherish/dsh-bridge](https://github.com/mycherish/dsh-bridge) | 1 | 2026-08-29 | 2026-09-01 | DSH Bridge 是 DeepSeek Harness 的原生 macOS 菜单栏快速入口，不是完整聊天客户端，也不是 DSH Web 的套壳。 |
| 588 | [myYangyunfan/dsh_cardian](https://github.com/myYangyunfan/dsh_cardian) | 1 | 2026-09-01 | 2026-09-02 | cardian — DeepSeek Harness knowledge-center plugin: RepoWiki notes / flashcards / memory in a local Obsidian vault |
| 589 | [N9-Developer-Empowerment/DSH-Vibeify](https://github.com/N9-Developer-Empowerment/DSH-Vibeify) | 1 | 2026-08-26 | 2026-08-29 | Turn AI work into a living local magazine for DeepSeek Harness. DeepSeek, ChatGPT, or both. |
| 590 | [nataliwhite20534-droid/dsh-4-role-workflow](https://github.com/nataliwhite20534-droid/dsh-4-role-workflow) | 1 | 2026-09-02 | 2026-09-03 | 4-agent workflow (PM + Browser + Programmer + DataEng) for complex DSH tasks. Real run in docs/run-example.md. |
| 591 | [nataliwhite20534-droid/dsh-xhs-collector](https://github.com/nataliwhite20534-droid/dsh-xhs-collector) | 1 | 2026-09-02 | 2026-09-03 | XHS batch collector via CDP Chrome + residential IP. Real case study: 8 keywords, 500+ notes. docs/case-study.md |
| 592 | [Nath-Vikky/dsh-codekin](https://github.com/Nath-Vikky/dsh-codekin) | 1 | 2026-08-24 | 2026-08-28 | Codekin: a creature-collection and match-three RPG for DeepSeek Harness Web. |
| 593 | [NexusAgentX/dsh-reasoning-effort](https://github.com/NexusAgentX/dsh-reasoning-effort) | 1 | 2026-08-15 | 2026-08-27 | Host-side dsh plugin that adds seven reasoning-effort levels to third-party llm-pi-ai models in the web composer. |
| 594 | [Niceck/dsh-hhxg-market](https://github.com/Niceck/dsh-hhxg-market) | 1 | 2026-08-27 | 2026-08-27 | 恢恢量化 hhxg.top A股量化数据插件 for DeepSeek Harness (dsh)：6 个免费工具 + 5 个 VIP 工具（MCP 桥接）· A-share quant data plugin |
| 595 | [NimuStudio/NimuQDock-dsh](https://github.com/NimuStudio/NimuQDock-dsh) | 1 | 2026-08-27 | 2026-08-27 | 把 DeepSeek Harness接入QQ的对接坞——带人格引擎的仿真群友：心情、精力、记忆，像真人一样潜水与参与。 |
| 596 | [ningbonb/dsh-web-desktop](https://github.com/ningbonb/dsh-web-desktop) | 1 | 2026-08-31 | 2026-08-31 | Electron launcher for DeepSeek Harness Web profiles / DeepSeek Harness Web Profile 的 Electron 桌面启动器 |
| 597 | [niyongsheng/meww](https://github.com/niyongsheng/meww) | 1 | 2026-08-27 | 2026-08-27 | pokemon ai pet🐣电子宠物 |
| 598 | [njjpro/dsh-vault](https://github.com/njjpro/dsh-vault) | 1 | 2026-08-30 | 2026-08-30 | Persistent credential vault plugin for DeepSeek Harness (DSH) - manage API tokens, server logins, and site credentials in one settings panel. |
| 599 | [Noemm/dsh-web-search-glm](https://github.com/Noemm/dsh-web-search-glm) | 1 | 2026-08-28 | 2026-08-28 | Zhipu GLM search provider for the DeepSeek Harness (dsh) web seam — native web_search via the Anthropic-compatible API |
| 600 | [NOirBRight/dsh-model-switch](https://github.com/NOirBRight/dsh-model-switch) | 1 | 2026-08-19 | 2026-08-29 | Model purposes spec and tickets for DeepSeek Harness |
| 601 | [NoxTyrannus/dsh-cipher](https://github.com/NoxTyrannus/dsh-cipher) | 1 | 2026-08-29 | 2026-08-29 | 把 cipher 的持续思考/三中台/四类记忆以 UNNI/LOOP 会话模式接入 DSH（dsh-plugin bundle） |
| 602 | [Nuomi9/dsh-fgo-chaldea](https://github.com/Nuomi9/dsh-fgo-chaldea) | 1 | 2026-08-15 | 2026-08-27 | FGO Chaldea-inspired skin pack for DeepSeek Harness Web UI: 5 themes, original generated backdrops, gold trim. |
| 603 | [Nzssm1/dsh-strategy-deployment-review](https://github.com/Nzssm1/dsh-strategy-deployment-review) | 1 | 2026-08-27 | 2026-08-27 | DSH agent preset for rigorous strategy live-deployment testing/evaluation. Retest. |
| 604 | [objectivex666/dsh-settings-search](https://github.com/objectivex666/dsh-settings-search) | 1 | 2026-08-25 | 2026-08-27 | A plugin that adds a search box to the DSH settings panel. |
| 605 | [oh-my-engine/dsh-plugin-oh-my-engine](https://github.com/oh-my-engine/dsh-plugin-oh-my-engine) | 1 | 2026-09-02 | 2026-09-02 | Approval-gated OME engineering delivery Agent Preset for DeepSeek Harness |
| 606 | [OMSociety/kimi-ppt-skill](https://github.com/OMSociety/kimi-ppt-skill) | 1 | 2026-09-03 | 2026-09-03 | DSH (DeepSeek Harness) presentation skill: PPT/演示文稿生成与导出，含 DSH 内纯本地导出 (python-pptx) 与本地预览渲染 (Pillow)。 |
| 607 | [openllmsh/dsh](https://github.com/openllmsh/dsh) | 1 | 2026-08-24 | 2026-08-27 | DeepSeek Harness (dsh) bundle: route the harness through OpenLLM (OpenAI-compatible) + register the OpenLLM MCP, with CLI/daemon onboarding. |
| 608 | [Pappet/dsh-tool-imagegen](https://github.com/Pappet/dsh-tool-imagegen) | 1 | 2026-08-30 | 2026-08-31 | Text-to-image and image-to-image generation for DeepSeek Harness via OpenRouter's unified Image API, with capability-gated parameters |
| 609 | [patrickluvsoj/dsh-llm-nous](https://github.com/patrickluvsoj/dsh-llm-nous) | 1 | 2026-08-21 | 2026-08-27 | Nous Portal LLM plugin bundle for DeepSeek Harness |
| 610 | [Perfirstvito/dsh-compaction-micro](https://github.com/Perfirstvito/dsh-compaction-micro) | 1 | 2026-09-01 | 2026-09-01 | a context compact strategy plugin |
| 611 | [phantomSuying/dsh-module-driven-develop](https://github.com/phantomSuying/dsh-module-driven-develop) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin for module-driven development: decompose requirements into a module tree, generate each module with an independent agent, and fully regenerate from design on any change. |
| 612 | [pipipigu/dsh-workspace-tree](https://github.com/pipipigu/dsh-workspace-tree) | 1 | 2026-08-28 | 2026-08-28 | Virtual session folder grouping, drag & drop, and subproject manager for DeepSeek Harness (DSH). |
| 613 | [pn1024/dsh-ppt-master](https://github.com/pn1024/dsh-ppt-master) | 1 | 2026-08-31 | 2026-08-31 | PPT Master skill packaged as a DeepSeek Harness (dsh) plugin: AI-driven presentation workflow for editable PPTX decks, SVG snapshots, native template filling, and PPTX enhancement. |
| 614 | [promisez322-prog/dsh-vox-input](https://github.com/promisez322-prog/dsh-vox-input) | 1 | 2026-08-30 | 2026-08-30 | Voice (speech-to-text) input for the DSH Web composer via Web Speech API — tap, speak, transcript fills the input box. Zero server, zero API keys. |
| 615 | [ptonlix/dsh-forge](https://github.com/ptonlix/dsh-forge) | 1 | 2026-08-22 | 2026-08-31 |  building an auditable desktop distribution around DeepSeek Harness (DSH).  |
| 616 | [pwping/dsh-power-launch](https://github.com/pwping/dsh-power-launch) | 1 | 2026-08-29 | 2026-08-29 | DSH桌面启动器插件，双击桌面快捷方式启动dsh Web UI，不需要每次打开终端手动输入命令 |
| 617 | [qfwycn/dsh-media-serve](https://github.com/qfwycn/dsh-media-serve) | 1 | 2026-09-02 | 2026-09-02 | 用于在deepseek harness上直接暴露工作区的文件，使大肥鱼能够直接显示他想给你显示的图片等信息，解决了大肥鱼老是说自己显示不了图片，要你去看本地文件的问题。在过验证码或截图的时候极为有用。 |
| 618 | [qigelunbiya/dsh-ssh-files-sidebar](https://github.com/qigelunbiya/dsh-ssh-files-sidebar) | 1 | 2026-08-26 | 2026-09-02 | Remote SSH workspace & deployment Agent for DeepSeek Harness — SSH Files, terminal, remote editing, zero-to-one Bootstrap, Runbook and closed-loop deployment. |
| 619 | [QinpanWan/dsh-doc-quick](https://github.com/QinpanWan/dsh-doc-quick) | 1 | 2026-08-25 | 2026-08-27 | Drag documents into the dsh web chat for direct local-file processing; a right sidebar lists outputs and file paths. 拖拽文档进 Web 对话框快速处理，右侧侧栏展示产出。 |
| 620 | [QinpanWan/dsh-harmonyos-market](https://github.com/QinpanWan/dsh-harmonyos-market) | 1 | 2026-08-24 | 2026-08-27 | HarmonyOS-exclusive plugin market for DeepSeek Harness — only plugins that actually run on HarmonyOS |
| 621 | [QinpanWan/dsh-prompt-antivirus](https://github.com/QinpanWan/dsh-prompt-antivirus) | 1 | 2026-08-31 | 2026-08-31 | dsh 全局防提示注入/上下文病毒感染插件：扫描工具参数、结果、进模型前消息与出站流；quarantine/block/monitor 三模式 + 金丝雀 + 可演进签名库（学习/导入/导出）。纯 JS 零原生依赖。 |
| 622 | [qiufengcrl/dsh-ip-https](https://github.com/qiufengcrl/dsh-ip-https) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: remote settings + Let's Encrypt IP certificates |
| 623 | [qixin-ai-data/dsh-qixin-insight-mcp-oauth](https://github.com/qixin-ai-data/dsh-qixin-insight-mcp-oauth) | 1 | 2026-08-29 | 2026-08-31 | DeepSeek Harness 插件：一键 OAuth 2.1 (PKCE) 授权，将启信慧眼 MCP 服务端挂载进 harness，让模型直接触达企业工商、股权、司法与风险等智能数据。 |
| 624 | [qiyeren/dsh-eac-popup](https://github.com/qiyeren/dsh-eac-popup) | 1 | 2026-08-27 | 2026-08-27 | DSH plugin: ???? agent ??/?????,EAC ????(??????)+?????5?+?????? |
| 625 | [QuantumKuba/dsh-continuum](https://github.com/QuantumKuba/dsh-continuum) | 1 | 2026-09-02 | 2026-09-02 | Durable project state and checkpoint engine for DeepSeek Harness (DSH). Prevents context exhaustion in long-running multi-agent workflows by persisting tasks, evidence, and checkpoints to disk. |
| 626 | [Raiyan007-gb/dsh-remote-tunnel-easy](https://github.com/Raiyan007-gb/dsh-remote-tunnel-easy) | 1 | 2026-08-28 | 2026-08-29 | DSH plugin bundle: scan a QR to open the deepseek-harness web UI on your phone inside the same session - cloudflared quick tunnel, no database, Windows/macOS/Linux |
| 627 | [ramen-ai-dev/dsh-ramen-guard](https://github.com/ramen-ai-dev/dsh-ramen-guard) | 1 | 2026-08-27 | 2026-08-27 | Fail-closed DeepSeek Harness guard enforcing ramen-ai Core IT policy before tool execution. |
| 628 | [Raphaelutumn/dsh-mood](https://github.com/Raphaelutumn/dsh-mood) | 1 | 2026-08-27 | 2026-08-27 | A tiny behavioral mood ring for your AI coding agent: a four-state session-header status light (GOOD/CONFUSED/FRUSTRATED/OVERWHELMED) for DeepSeek Harness |
| 629 | [RaulLazaro/dsh-preview-plugin](https://github.com/RaulLazaro/dsh-preview-plugin) | 1 | 2026-08-31 | 2026-09-01 | Live preview tab for DeepSeek Harness — embed any dev server in an iframe with transparent SPA proxying |
| 630 | [RaulLazaro/dsh-pwa-plugin](https://github.com/RaulLazaro/dsh-pwa-plugin) | 1 | 2026-08-31 | 2026-08-31 | PWA plugin for DeepSeek Harness — adds offline support and install-as-app capability |
| 631 | [RaulLazaro/dsh-server-setup](https://github.com/RaulLazaro/dsh-server-setup) | 1 | 2026-09-02 | 2026-09-03 | Production-tested setup for running DeepSeek Harness on a VPS with reverse proxy, systemd, and optional Pangolin tunnel |
| 632 | [redfox-data/redfox-skill-gallery](https://github.com/redfox-data/redfox-skill-gallery) | 1 | 2026-08-26 | 2026-09-01 | redfox-skill-gallery是 DeepSeek Harness 的 Web 插件。它在侧边栏底部加一个「红狐Skills」入口，点击后整个界面切换为卡片式技能画廊，集中展示redfox-community-dsh插件内的全部红狐社区 skills |
| 633 | [renchengxiang/dsh-web-search-tavily](https://github.com/renchengxiang/dsh-web-search-tavily) | 1 | 2026-08-28 | 2026-08-28 | Tavily-backed web search provider for DeepSeek Harness, with Settings → Plugins configuration UI |
| 634 | [RGarvel/dsh-channel-spec](https://github.com/RGarvel/dsh-channel-spec) | 1 | 2026-08-27 | 2026-08-27 | RFC: 按来源渠道对 DSH 会话分类展示（session header channel 字段 + GUI 渠道视图）— 源自 deepseek-harness discussion #3897 |
| 635 | [RGarvel/dsh-channel-view](https://github.com/RGarvel/dsh-channel-view) | 1 | 2026-08-27 | 2026-08-27 | DSH 渠道会话视图 spike：侧边栏 Channels tab 注入 + 会话投影数据链（RFC-0001, discussion #3897） |
| 636 | [rhczz/dshctl](https://github.com/rhczz/dshctl) | 1 | 2026-09-02 | 2026-09-02 | dshctl — DeepSeek Harness web 服务后台管理脚本(启停/日志/构建/一键更新) |
| 637 | [Ri0n72Y/dsh-tcp-forward](https://github.com/Ri0n72Y/dsh-tcp-forward) | 1 | 2026-09-03 | 2026-09-03 | simply a forward |
| 638 | [rogerdigital/dsh-vet](https://github.com/rogerdigital/dsh-vet) | 1 | 2026-08-29 | 2026-08-29 | Security vetting for DeepSeek Harness (DSH) plugins: permission & supply-chain audits before install, graded via the open dsh-vet/v1 report standard. |
| 639 | [rongxingda/dsh-prompt-enhance](https://github.com/rongxingda/dsh-prompt-enhance) | 1 | 2026-08-29 | 2026-08-29 | Prompt enhancement plugin for the DeepSeek Harness web GUI: one-click rewrite of the composer draft into a structured prompt, with preview, fill-back, and undo. |
| 640 | [Roxy-gl373/dsh-desktop](https://github.com/Roxy-gl373/dsh-desktop) | 1 | 2026-09-02 | 2026-09-02 | DSh Whale · DeepSeek Harness 桌面启动器：WebView2 内嵌 DSH 界面，实时日志、单实例托盘、多开、等比缩放，装插件自动快照回滚。install.cmd 一键配置。 |
| 641 | [rqzhao1/dsh-wsl-launcher](https://github.com/rqzhao1/dsh-wsl-launcher) | 1 | 2026-09-03 | 2026-09-04 | Windows desktop launcher for DeepSeek Harness Web running in WSL |
| 642 | [Ruixinhua/dsh-universe-api](https://github.com/Ruixinhua/dsh-universe-api) | 1 | 2026-08-27 | 2026-08-27 | Offline, deterministic public API discovery for DeepSeek Harness and DSH Desktop. |
| 643 | [runcat-tommy/dsh-chinese-poetry](https://github.com/runcat-tommy/dsh-chinese-poetry) | 1 | 2026-09-02 | 2026-09-02 | A token-free Chinese classical poetry plugin for DeepSeek Harness Web: search, filters, Feihua, daily poem, favorites, and AI explain. Powered by the free public chinese-poetry-api. |
| 644 | [runfali/dsh-prompt-injector](https://github.com/runfali/dsh-prompt-injector) | 1 | 2026-08-27 | 2026-08-27 | dsh 通用每轮上下文注入插件：设置页管理提示词清单，每轮对话把每条启用提示词以「上下文注入」提醒行注入模型上下文，让纪律规则（例如 图谱消费/wiki 先查/记忆召回）可靠生效。 |
| 645 | [ryasrk/dsh-awesome-skills](https://github.com/ryasrk/dsh-awesome-skills) | 1 | 2026-08-31 | 2026-09-03 | Plugin Skills for agents |
| 646 | [sandersyao/dsh-session-persistence-mysql](https://github.com/sandersyao/dsh-session-persistence-mysql) | 1 | 2026-09-01 | 2026-09-01 | deepseek harness 插件 替换会话持久化引擎为 MySQL 数据库 |
| 647 | [says693/dsh-composer-dynamic-island](https://github.com/says693/dsh-composer-dynamic-island) | 1 | 2026-09-02 | 2026-09-02 | Compact DSH Web composer island with a Community v0.15 host manifest and no user-defined button positioning. |
| 648 | [SeerableOfficial/dsh-anydoc-markdown](https://github.com/SeerableOfficial/dsh-anydoc-markdown) | 1 | 2026-08-29 | 2026-08-31 | Document → Markdown + vision image description plugin for DeepSeek Harness (dsh). Converts Word/PPT/Excel/ODT/RTF/EPUB/CSV/PDF via firecrawl-anydoc and describes embedded images with a VLM. |
| 649 | [sens-io/memobranch](https://github.com/sens-io/memobranch) | 1 | 2026-09-03 | 2026-09-04 | Git-native, auditable long-term memory for AI agents |
| 650 | [SeverusZh/dsh-ollama-usage](https://github.com/SeverusZh/dsh-ollama-usage) | 1 | 2026-08-27 | 2026-08-27 | Ollama Cloud 用量余量可视化 DeepSeek Harness 插件:5h 会话/周用量双横条 + 设置页面板,Key 与快照持久化,自动刷新,登录引导。Ollama Cloud usage & quota visualization plugin for DeepSeek Harness. |
| 651 | [Shaky77/KISS_Law-DSH](https://github.com/Shaky77/KISS_Law-DSH) | 1 | 2026-08-19 | 2026-08-27 | Weiwen's Law (KISS-Law) — a domain-agnostic causal-constraint middleware for DeepSeek Harness. A faithful, white-box presentation of how causal law actually runs. White-box audit, never prediction. Hard-gate the boundary; inner H decides freely. |
| 652 | [shaomingbo/dsh-subscription-search](https://github.com/shaomingbo/dsh-subscription-search) | 1 | 2026-08-19 | 2026-08-30 | ChatGPT/Grok subscription OAuth, model routes, and ChatGPT to Grok to Exa to DeepSeek web-search fallback for DeepSeek Harness |
| 653 | [shengmk/godsh](https://github.com/shengmk/godsh) | 1 | 2026-08-28 | 2026-08-28 | godsh - GUI launcher for DeepSeek Harness (dsh): manage profiles, plugins, kernels, and dsh versions |
| 654 | [shimingming520/dsh-audiogen](https://github.com/shimingming520/dsh-audiogen) | 1 | 2026-08-28 | 2026-08-29 | AI audio generation plugin for the DeepSeek Harness web GUI: multi-vendor TTS, music, sound effects and voice design with a sidebar panel, model comparison, resource library and Agent tools. |
| 655 | [ShinonomeAya/dsh-git-chain](https://github.com/ShinonomeAya/dsh-git-chain) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: Cursor-style Git commit-chain graph with SVG lanes, commit details, diff, filtering, and guarded branch switching. |
| 656 | [shlouai/dsh-debate](https://github.com/shlouai/dsh-debate) | 1 | 2026-09-02 | 2026-09-04 | Stop asking your agent what it thinks. Make it hold a trial. |
| 657 | [shuaweng/DSH_xieshujing](https://github.com/shuaweng/DSH_xieshujing) | 1 | 2026-08-30 | 2026-08-30 | 写书鲸：面向 DeepSeek Harness 的原生 AI 小说创作工作台插件 |
| 658 | [Six6stRINgs/dsh-client-ui-thinking-stats](https://github.com/Six6stRINgs/dsh-client-ui-thinking-stats) | 1 | 2026-09-03 | 2026-09-04 | 在底部Dock和每次对话尾部添加模型思考token统计的轻量化插件。A lightweight plugin that adds model thinking token statistics to the bottom Dock and the end of each conversation. |
| 659 | [SleepEggTart/dsh-code-coverage](https://github.com/SleepEggTart/dsh-code-coverage) | 1 | 2026-08-26 | 2026-08-27 | 解析 DSH session 日志归因 AI 生成文件，叠加 c8 覆盖率，产出 AI vs 人工代码覆盖率对比、高危未测文件清单与信任分。 |
| 660 | [SleepEggTart/dsh-dev-wrapped](https://github.com/SleepEggTart/dsh-dev-wrapped) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (DSH) 开发者使用报告——类 Spotify Wrapped，统计与 AI 结对编程的行为，生成可分享报告卡片 |
| 661 | [SleepEggTart/dsh-mbti-jury](https://github.com/SleepEggTart/dsh-mbti-jury) | 1 | 2026-08-31 | 2026-08-31 | DSH 插件：16 型 MBTI 人格评审团，并排评审你最近一次 commit——同一个 diff，16 种看见世界的方式。 |
| 662 | [Snow-ea/dsh-token-optimizer](https://github.com/Snow-ea/dsh-token-optimizer) | 1 | 2026-08-30 | 2026-08-30 | Deterministic, recoverable tool-result compression and cache-aware compaction for DeepSeek Harness. |
| 663 | [softspark/dsh-codex](https://github.com/softspark/dsh-codex) | 1 | 2026-08-25 | 2026-08-27 | DeepSeek Harness provider for locally authenticated Codex app-server access through a ChatGPT subscription. |
| 664 | [sogoodayo/dsh-code-ui](https://github.com/sogoodayo/dsh-code-ui) | 1 | 2026-09-01 | 2026-09-02 | Cursor 风格的 AI 代码编辑器工作台插件（DSH）：文件树、多标签页编辑、引用/备注/翻译、内嵌 AI 输入框、语法高亮 |
| 665 | [sperictao/dsh-pro-max](https://github.com/sperictao/dsh-pro-max) | 1 | 2026-08-20 | 2026-09-01 | DeepSeek Harness desktop launcher — one-click local web UI, Tailscale-secured remote access, plugin marketplace & model configuration. Built with Tauri 2 + React + TypeScript. |
| 666 | [spritebbb/dsh-skill-usage](https://github.com/spritebbb/dsh-skill-usage) | 1 | 2026-08-31 | 2026-08-31 | DSH 实时技能显示小插件 🌟 输入框下方的可爱小徽章，实时显示当前技能，悬停看历史。Real-time active skill chip for DeepSeek Harness. |
| 667 | [starsinc1708/dsh-tool-council](https://github.com/starsinc1708/dsh-tool-council) | 1 | 2026-08-26 | 2026-08-27 | Map-reduce council of subagents for the DeepSeek Harness: one task fans out to independent members, their findings are deduplicated, verified by a separate panel, and reduced to a quorum report |
| 668 | [SUFE-Chaoyi/dsh-plugin-csv-report](https://github.com/SUFE-Chaoyi/dsh-plugin-csv-report) | 1 | 2026-08-31 | 2026-08-31 | 基于 DeepSeek Harness 的可复用 CSV 描述统计与可复现报告插件 |
| 669 | [summer-521/deepseek-harness-swift](https://github.com/summer-521/deepseek-harness-swift) | 1 | 2026-08-25 | 2026-08-28 | 基于 AppKit、SwiftUI 与 WKWebView 的 DSH 原生 macOS 桌面壳，提供设置中心、DSH 版本管理、插件管理、通知和 Sparkle 应用更新。 |
| 670 | [Sunday2Mo/dsh-file-quote](https://github.com/Sunday2Mo/dsh-file-quote) | 1 | 2026-08-27 | 2026-08-27 | 基于 better-sidebar 的统一引用插件：划选文件/消息即可批注引用，引用块带文件路径与行区间、双端折叠、点击跳回原文 ｜ Unified-quoting plugin built on DSH-better-sidebar: select files or messages to annotate; quote blocks carry path & line range, collapse in chat and history, and jump back to the source on click. |
| 671 | [sunzhyang1616-ui/dsh-ssh-terminal](https://github.com/sunzhyang1616-ui/dsh-ssh-terminal) | 1 | 2026-08-29 | 2026-08-29 | 在 DSH 侧边栏（dsh-better-sidebar）连接远程主机的 SSH 终端：逐步查看 agent 命令与输出，内置 ssh_connect / ssh_exec 等工具，记录本机持久化。 |
| 672 | [supanexus/dsh-plugin-chat-enhance](https://github.com/supanexus/dsh-plugin-chat-enhance) | 1 | 2026-09-04 | 2026-09-04 | Searchable model picker with recent chips, vision capability tags, and composer image upload for DeepSeek Harness. |
| 673 | [supanexus/dsh-plugin-file-explorer](https://github.com/supanexus/dsh-plugin-file-explorer) | 1 | 2026-09-04 | 2026-09-04 | Workspace file tree and multi-tab editor in DeepSeek Harness — browse, edit, and preview files without leaving the chat UI. |
| 674 | [svgop/dsh-rich-questions](https://github.com/svgop/dsh-rich-questions) | 1 | 2026-08-26 | 2026-08-29 | Rich branching survey system for DeepSeek Harness (DSH) Web GUI — ask_survey tool with branch graphs, delayed hover insights, Mermaid diagrams, quick mode, reroll/push/discuss actions |
| 675 | [sycamorestr/dsh-platform-account-manager-plugin](https://github.com/sycamorestr/dsh-platform-account-manager-plugin) | 1 | 2026-08-29 | 2026-08-29 | DSH platform account and persistent browser-session manager |
| 676 | [TangYT/dsh-superpowers](https://github.com/TangYT/dsh-superpowers) | 1 | 2026-09-03 | 2026-09-03 | DeepSeek Harness port of obra/superpowers: 14 agentic skills (brainstorming/planning/SDD/TDD/debugging/review/worktrees) + session-start bootstrap injection. |
| 677 | [TaylorSwitiger/dsh-plan-bridge](https://github.com/TaylorSwitiger/dsh-plan-bridge) | 1 | 2026-09-03 | 2026-09-03 | DeepSeek Harness (dsh) plugin: one local bridge for ChatGPT Codex / Claude / ZCode (GLM) / Qwen subscription plans — settings status card, one-click provisioning, zero core changes. npm: @taylorswitiger/dsh-plan-bridge |
| 678 | [TelosmaYLX/dsh-session-notify](https://github.com/TelosmaYLX/dsh-session-notify) | 1 | 2026-08-28 | 2026-08-28 | 当dsh任务完成/阻塞/提问等情况时，自动推送windows消息进行提醒，支持自定义文案和图片，以及显示会话用时、消耗token、速度tps等指标。Automatically push Windows notifications upon completion of a dsh task, supporting custom text and images, as well as displaying metrics including session duration, token consumption, and TPS speed. |
| 679 | [TestTheBoy/dsh_plugin_file_attach](https://github.com/TestTheBoy/dsh_plugin_file_attach) | 1 | 2026-08-26 | 2026-08-27 | Add files to context |
| 680 | [TiferKing/dsh-company](https://github.com/TiferKing/dsh-company) | 1 | 2026-09-03 | 2026-09-03 | 不想当牛马了？来当老板！开插件公司，雇AI牛马，过赛博人生！ |
| 681 | [tiger0012/dsh-we-wallpaper-sync](https://github.com/tiger0012/dsh-we-wallpaper-sync) | 1 | 2026-08-26 | 2026-08-27 | Reusable skill: browse/search/download Wallpaper Engine (Steam 431960) workshop wallpapers and wire them into the DSH skin center, bypassing the Steam HTTP block and region-mismatch sign-in block. |
| 682 | [Tinger-X/dsh-session-enhance](https://github.com/Tinger-X/dsh-session-enhance) | 1 | 2026-08-25 | 2026-08-31 | Full-control session management for DeepSeek Harness Web |
| 683 | [tower1229/dsh-thinkbar](https://github.com/tower1229/dsh-thinkbar) | 1 | 2026-08-29 | 2026-08-31 | 让 DeepSeek Harness 的思考状态被看见——零侵入地将 reasoning 等待转化为由蓝到金、持续升温的动态 ThinkBar。 |
| 684 | [trrrrrryg/dsh-ssh-forge](https://github.com/trrrrrryg/dsh-ssh-forge) | 1 | 2026-08-24 | 2026-08-27 | DSH SSH Forge：为 DeepSeek Harness（DSH）提供 SSH 远程工作区能力：已核验的服务器身份、失败关闭的 Agent 执行路由、远端文件与命令操作；提供 Windows 离线一键安装包，无需 Node.js 或构建工具。 |
| 685 | [TT-Wang/dsh-eval-infra](https://github.com/TT-Wang/dsh-eval-infra) | 1 | 2026-09-03 | 2026-09-04 | Paired A/B evaluation infrastructure for DeepSeek Harness (dsh) components: interleaved repeated runs through the real runtime, verifier self-checks, one-variable arms, regression gating, cache- and calendar-aware cost, CLI + web UI |
| 686 | [tyx6661234/dsh-community-listening](https://github.com/tyx6661234/dsh-community-listening) | 1 | 2026-08-26 | 2026-08-27 | 面向 DeepSeek Harness (DSH) 的社交评论研究插件 |
| 687 | [Ultmebius/universal-plugin-hub](https://github.com/Ultmebius/universal-plugin-hub) | 1 | 2026-08-26 | 2026-08-31 | DSH 插件市场：内置 Claude 官方插件目录，支持添加 Git 仓库作为插件源；一键安装，技能、子代理、MCP、LSP、hooks 装完自动接线 · Plugin marketplace for DeepSeek Harness |
| 688 | [UNscientific-9/dsh-turnfold](https://github.com/UNscientific-9/dsh-turnfold) | 1 | 2026-08-27 | 2026-08-27 | DSH Web 轮次折叠插件：thinking/工具调用流式可见，turn 完成后自动收纳成一行摘要。 |
| 689 | [v587d/dsh-custom-skin](https://github.com/v587d/dsh-custom-skin) | 1 | 2026-08-28 | 2026-08-28 | 自己的插件皮肤管理工具。 |
| 690 | [v587d/dsh-search-first](https://github.com/v587d/dsh-search-first) | 1 | 2026-09-01 | 2026-09-01 | Search first, verify facts, reply last — enforced by DSH. |
| 691 | [valuelesser/pipeline-mode](https://github.com/valuelesser/pipeline-mode) | 1 | 2026-09-01 | 2026-09-01 | LangGraph-style adaptive Planner→Executor→Reviewer pipeline for DSH (DeepSeek Harness) |
| 692 | [victor10035445/dsh-v-explorer](https://github.com/victor10035445/dsh-v-explorer) | 1 | 2026-09-02 | 2026-09-02 | right slider for deepseek-harness-plugin. |
| 693 | [victor10035445/dsh-v-skill-links](https://github.com/victor10035445/dsh-v-skill-links) | 1 | 2026-09-02 | 2026-09-02 | let dsh use your skills.quick command and diy buttons. |
| 694 | [victor10035445/dsh-v-theme](https://github.com/victor10035445/dsh-v-theme) | 1 | 2026-09-02 | 2026-09-02 | theme plugin for deepseek harness by victor |
| 695 | [VioletScar-Hui/dsh-chat-history](https://github.com/VioletScar-Hui/dsh-chat-history) | 1 | 2026-09-02 | 2026-09-02 | 给 DSH 聊天输入框加上 CLI 风格历史记忆：上下键召回之前发送过的内容（纯客户端插件，重启不丢） |
| 696 | [VioletScar-Hui/trcost-plugin](https://github.com/VioletScar-Hui/trcost-plugin) | 1 | 2026-08-28 | 2026-08-28 | 轨迹省钱优化器：DSH 会话轨迹 token 浪费分析 + waterfall 执行层强制拦截/截断。Trajectory cost optimizer with enforcement layer for DeepSeek Harness. |
| 697 | [w2327644822-png/dsh-usage-analytics](https://github.com/w2327644822-png/dsh-usage-analytics) | 1 | 2026-08-26 | 2026-08-27 | Personal usage analytics & activity dashboard for the DeepSeek Harness (dsh) web GUI: token totals, contribution heatmap, model share, insights. Local-only, metadata only. |
| 698 | [warment/deepseek-harness-locale-ru](https://github.com/warment/deepseek-harness-locale-ru) | 1 | 2026-08-30 | 2026-08-30 | Русский язык для DeepSeek Harness web UI — one-command install, 1061 строка, 100% покрытие |
| 699 | [Washington5533/guarftrain](https://github.com/Washington5533/guarftrain) | 1 | 2026-08-09 | 2026-08-27 | 🛡️ 一行命令，训练脚本零行改动，获得完整守护能力。GPU 监控 · 崩溃恢复 · OOM 自救 · Agent 决策 · MCP 35 工具 · Web Dashboard。 |
| 700 | [weibaohui/dsh-sync](https://github.com/weibaohui/dsh-sync) | 1 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：会话同步与冲突解决（apiproxy、token 内联） |
| 701 | [weibaohui/skills-management](https://github.com/weibaohui/skills-management) | 1 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：技能市场——安装/删除/详情 API + 管理界面 |
| 702 | [Weiyang742/dsh-cross-session-messaging](https://github.com/Weiyang742/dsh-cross-session-messaging) | 1 | 2026-08-31 | 2026-08-31 | Cross-session relay for DeepSeek Harness: peer discovery and text delivery between independent dsh processes. |
| 703 | [wenyixiaoqingnian/screenshot-review](https://github.com/wenyixiaoqingnian/screenshot-review) | 1 | 2026-08-29 | 2026-08-29 | dsh skill: 截图审阅——模型自己截图、自己看图、自己改代码，迭代优化前端效果 |
| 704 | [WesleyJay/dsh-weather](https://github.com/WesleyJay/dsh-weather) | 1 | 2026-08-27 | 2026-08-28 | 一个 DSH 天气查询插件，让 AI 智能体可以查询全球城市的实时天气和天气预报 |
| 705 | [Wisdoverse/dsh-inline-media-viewer-plugin](https://github.com/Wisdoverse/dsh-inline-media-viewer-plugin) | 1 | 2026-08-26 | 2026-08-28 | Inline image, video, and audio previews for DeepSeek Harness Web, with workspace-safe local files, direct web media, and an optional ComfyUI proxy. |
| 706 | [wjf1/dsh-commandcode](https://github.com/wjf1/dsh-commandcode) | 1 | 2026-08-30 | 2026-08-30 | DSH-Desktop LLM provider plugin for Command Code with model catalog sync, request retry, multi-credential support, and a settings UI. |
| 707 | [wodongx123/dsh-qq-notify](https://github.com/wodongx123/dsh-qq-notify) | 1 | 2026-08-17 | 2026-08-27 | QQ notifications via local NapCat for DeepSeek Harness: qq_send / qq_status / qq_napcat / qq_deploy native tools + one-click deploy scripts. QQ???? |
| 708 | [writeCasually/dsh-git](https://github.com/writeCasually/dsh-git) | 1 | 2026-08-21 | 2026-08-31 | DeepSeek Harness Git plugin — visual git status, diff, commit & file preview in the DSH web UI |
| 709 | [WSL043/dsh-deepseek-dashboard](https://github.com/WSL043/dsh-deepseek-dashboard) | 1 | 2026-08-24 | 2026-08-27 | 已归档：DeepSeek API 余额与 DSH 本地用量面板；现有 Release 保留，不再适配未来 DSH。 |
| 710 | [wszhoho/dsh-file-attachment](https://github.com/wszhoho/dsh-file-attachment) | 1 | 2026-08-28 | 2026-08-28 | 拖入 / 粘贴 / 工具栏上传按钮（📎，可多选）为输入框附加文件：图片走既有草稿图片流程（不落盘）；文档全文落盘到会话工作区 .dsh-file-attachment/ 并插入 @绝对路径引用 |
| 711 | [wtksana/dsh-font-plugin](https://github.com/wtksana/dsh-font-plugin) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Font Plugin, DSH 字体插件 |
| 712 | [x7687315-gif/dsh-policy](https://github.com/x7687315-gif/dsh-policy) | 1 | 2026-09-02 | 2026-09-03 | User-controlled policy and personalization runtime for DeepSeek Harness - enforce hard project constraints at the agent lifecycle boundary. |
| 713 | [xfqz86/dsh-usage-stats](https://github.com/xfqz86/dsh-usage-stats) | 1 | 2026-08-23 | 2026-08-27 | DSH Web 插件：侧边栏中的 Token 使用统计 |
| 714 | [xiaobai2017666/dsh-chrome-cdp](https://github.com/xiaobai2017666/dsh-chrome-cdp) | 1 | 2026-08-28 | 2026-08-31 | Chrome DevTools Protocol 插件 for DeepSeek Harness。通过 chromremote-interface 以 CDP 连接并操控 Chrome |
| 715 | [xiaochaZ/dsh-session-title-summary](https://github.com/xiaochaZ/dsh-session-title-summary) | 1 | 2026-08-25 | 2026-08-27 | DSH plugin: rolling session summary + current-task title (@xiaochaz) |
| 716 | [Xichun123/dsh-relay-models](https://github.com/Xichun123/dsh-relay-models) | 1 | 2026-08-14 | 2026-08-29 | Mixed-protocol relay model discovery, metadata matching, and Web configuration for DeepSeek Harness |
| 717 | [XINY11451/dsh-wsl](https://github.com/XINY11451/dsh-wsl) | 1 | 2026-08-26 | 2026-09-02 | A model-facing WSL tool plugin for DeepSeek Harness (DSH). It lets an agent run Linux commands through wsl.exe directly — no hand-written .sh scripts or pwsh wrappers. |
| 718 | [xipian1216/dsh-aa-bridge](https://github.com/xipian1216/dsh-aa-bridge) | 1 | 2026-08-17 | 2026-08-31 | Agents Anywhere bridge and Web status plugin for DeepSeek Harness |
| 719 | [xiyunSacire/dsh-skill-manager](https://github.com/xiyunSacire/dsh-skill-manager) | 1 | 2026-08-28 | 2026-08-28 |  The dsh-skill-manager is a deep-integration Web UI plugin designed to provide developers and advanced users with direct visibility and control over the true, persistent "skill memory" of DeepSeek Harness (DSH). |
| 720 | [xjailll/dsh-portfolio-publisher](https://github.com/xjailll/dsh-portfolio-publisher) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 插件：GitHub 求职仓库一键发布助手（LLM README + Web 面板 + 一键推送） |
| 721 | [xmnathan/dsh-skin-galactic-opera](https://github.com/xmnathan/dsh-skin-galactic-opera) | 1 | 2026-08-27 | 2026-08-27 | Unofficial cinematic space-opera dark skin bundle for the DSH Web GUI. |
| 722 | [XSakura666/dsh-plugin-ChronoAgent](https://github.com/XSakura666/dsh-plugin-ChronoAgent) | 1 | 2026-08-15 | 2026-08-27 | Local-first desktop app that schedules AI agent tasks like cron jobs — zero token cost until they run. Write a task, set a time, and it runs automatically with files, web, MCP tools, and multi-model support.      |
| 723 | [yakoylp/dsh-md-convert](https://github.com/yakoylp/dsh-md-convert) | 1 | 2026-08-28 | 2026-08-28 | Convert Office documents and PDFs (incl. scanned, via CPU-first routing OCR with lightweight models: PP-DocLayout-L layout, RapidOCR text, SLANet tables, FormulaNet formulas) to structurally-formatted Markdown. CLI + dsh agent tool (md_convert). |
| 724 | [yangbobo2021/relay-dsh-plugin-manager](https://github.com/yangbobo2021/relay-dsh-plugin-manager) | 1 | 2026-08-26 | 2026-08-27 | A standalone plugin manager for DeepSeek Harness. |
| 725 | [yhbd-top/dsh-plugin-top](https://github.com/yhbd-top/dsh-plugin-top) | 1 | 2026-08-29 | 2026-08-29 | yhbd.top 插件雷达 for DeepSeek Harness：侧边栏大面板浏览 3900+ 插件目录（搜索 / 22 分类 / 站点同款五榜单 / 榜单联动分类），安装引导语一键写入会话输入框；进程内同源反代，零配置；附带 Agent 可调用的搜索与榜单工具。 |
| 726 | [yindf/taskfold](https://github.com/yindf/taskfold) | 1 | 2026-09-02 | 2026-09-02 | Keeps long coding-agent sessions lean: wrap work in named tasks and, when one is done, fold its whole span into a short titled summary. The conversation stays readable, context costs stay low, and every fold's original content can be read back on demand. For [DeepSeek Harness](https://www.npmjs.com/package/@deepseek-ai/dsh) (DSH). |
| 727 | [YINGCHAO-98/dsh-private-plugins](https://github.com/YINGCHAO-98/dsh-private-plugins) | 1 | 2026-08-25 | 2026-08-27 | 在 DeepSeek Harness Web 设置中统一导入、启用、更新和管理本地及云端私有插件。 |
| 728 | [yj-liuzepeng/dsh-project-brain](https://github.com/yj-liuzepeng/dsh-project-brain) | 1 | 2026-08-30 | 2026-08-30 | Persistent project intelligence and memory plugin for DSH: architecture analysis, cross-session context, TODOs, and optional hybrid retrieval |
| 729 | [yongshuai0314/dsh-i-have-adhd](https://github.com/yongshuai0314/dsh-i-have-adhd) | 1 | 2026-08-26 | 2026-08-27 | ADHD-friendly output shaping for DeepSeek Harness: one system-prompt section with adhd_on/adhd_off/adhd_status tools, persisted across restarts. Inspired by ayghri/i-have-adhd (MIT). |
| 730 | [yu-wenchao/dsh-tool-lipsync](https://github.com/yu-wenchao/dsh-tool-lipsync) | 1 | 2026-09-04 | 2026-09-04 | FreeLipSync lip-sync video plugin for DeepSeek Harness - No API key required |
| 731 | [yuan-source-666/dsh-github-manager](https://github.com/yuan-source-666/dsh-github-manager) | 1 | 2026-08-27 | 2026-08-27 | GitHub 仓库 AI 自动管理通道插件 (DeepSeek Harness community bundle): 27 个工具（仓库/Issue/PR/分支/文件/标签/话题/Tags/Releases/搜索）+ Web 设置卡片 + dry-run 防护 + secret 令牌。 |
| 732 | [yuan-source-666/dsh-research-autoresearch](https://github.com/yuan-source-666/dsh-research-autoresearch) | 1 | 2026-08-27 | 2026-08-27 | AutoResearch 科研协议 DSH 全家桶插件：arXiv recall + LQS 评分 + 状态持久化 + 停滞红绿灯 + 五人格中位数评审 + 可视化总控台卡片。灵感：Deli Chen "From Draft to Strong-Accept: How a Self-Play Survey Hit 8.6"。 |
| 733 | [yuan-source-666/dsh-task-notifier](https://github.com/yuan-source-666/dsh-task-notifier) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness community plugin: OS notification when a turn, subagent, background job, goal, or workflow finishes. Localized wording, per-source switches, custom delivery command. npm: dsh-task-notifier |
| 734 | [yuioi666/dsh-conversation-nav-dots](https://github.com/yuioi666/dsh-conversation-nav-dots) | 1 | 2026-08-31 | 2026-09-01 | dsh-conversation-nav-dots 在 DSH Web 对话界面的右侧添加一列导航标记。每个标记对应一条用户消息。点击即可跳转，悬停可预览所有消息内容。 |
| 735 | [yunniees/DSH-Plugin-Manager](https://github.com/yunniees/DSH-Plugin-Manager) | 1 | 2026-08-28 | 2026-08-28 | Visual plugin manager for DeepSeek Harness: AI auto-translation, AI one-click summaries, AI plugin search, one-click share & install of multiple plugins, bulk updates |
| 736 | [Yuuz12/dsh-tavily](https://github.com/Yuuz12/dsh-tavily) | 1 | 2026-08-30 | 2026-08-31 | Tavily-backed web search provider plugin for DeepSeek Harness (DSH) — multi-key balance-aware rotation with failover, manageable from the DSH web settings. |
| 737 | [yx222yx/DSH-Feedback-Bridge](https://github.com/yx222yx/DSH-Feedback-Bridge) | 1 | 2026-08-29 | 2026-08-30 | 一个 DeepSeek Harness 插件，帮助用户将功能想法和错误反馈整理为清晰、注重隐私的 GitHub Discussions。A DeepSeek Harness plugin that helps users turn ideas and bug reports into clear, privacy-aware GitHub Discussions. |
| 738 | [yybukn/dsh-table-attach](https://github.com/yybukn/dsh-table-attach) | 1 | 2026-08-31 | 2026-08-31 | 在dph中可以直接拖动.xlsx和.csv的表格文件到输入框中 |
| 739 | [yyh-001/dsh-launcher](https://github.com/yyh-001/dsh-launcher) | 1 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 轻量 Windows 启动器。选一个版本，启动 dsh web。 |
| 740 | [yyyq0325-ai/dsh-webgate](https://github.com/yyyq0325-ai/dsh-webgate) | 1 | 2026-08-22 | 2026-08-27 | 为 DeepSeek Harness 的 Web GUI 加一道账号密码门：每次打开 DSH Web 都必须先登录；登录令牌有效期 12 小时；令牌过期被登出时，后台正在运行的任务完全不受影响，重新登录后一切还在。 |
| 741 | [yztdtf/dsh-worktable-pet](https://github.com/yztdtf/dsh-worktable-pet) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness ??????????(Dynamic Cordis Plugin) |
| 742 | [z-y-q/dsh-mcp-security](https://github.com/z-y-q/dsh-mcp-security) | 1 | 2026-09-02 | 2026-09-02 | dsh-mcp-security |
| 743 | [zaizaizhao/dsh-branchmark](https://github.com/zaizaizhao/dsh-branchmark) | 1 | 2026-08-30 | 2026-09-02 | While vibe coding, save an answer you may need later, use Side Chat for a question that suddenly comes up, or open a related conversation for deeper work without losing focus on the current task. |
| 744 | [Zara-Siwei/dsh-float](https://github.com/Zara-Siwei/dsh-float) | 1 | 2026-08-26 | 2026-08-27 | Floating minimal-mode DeepSeek Harness (dsh) plugin: a transparent terminal TUI over dsh web in a borderless Electron window. |
| 745 | [Zayzz-pixel/dsh-ariadne](https://github.com/Zayzz-pixel/dsh-ariadne) | 1 | 2026-09-01 | 2026-09-01 | A visual decision workbench for DeepSeek Harness: explore ideas, focus branches, and turn choices into executable graphs. |
| 746 | [ZBber-lab/cau-portal-open](https://github.com/ZBber-lab/cau-portal-open) | 1 | 2026-08-31 | 2026-09-01 | 农大门户（cau-portal）：中国农业大学通知公告 DSH 插件 + 爬虫/AI 加工管道（开源工具，数据由使用者自建） |
| 747 | [zenvertao/dsh-inline-comments](https://github.com/zenvertao/dsh-inline-comments) | 1 | 2026-08-26 | 2026-08-27 | 选中即批注，刷新亦留存 —— DSH 行内批注插件 |
| 748 | [zerorigin-studio/dsh-desktop-shell](https://github.com/zerorigin-studio/dsh-desktop-shell) | 1 | 2026-08-24 | 2026-09-01 | dsh desktop shell plugin |
| 749 | [zhang-bin-98/sci-fork](https://github.com/zhang-bin-98/sci-fork) | 1 | 2026-08-31 | 2026-09-04 | Git-native biomedical Research Graph for DeepSeek Harness, with literature-grounded expansion and auditable local project files. |
| 750 | [zhangyqjiaoshou-oss/dsh-model-sync](https://github.com/zhangyqjiaoshou-oss/dsh-model-sync) | 1 | 2026-08-29 | 2026-08-29 | One-click / auto model sync for DeepSeek Harness providers |
| 751 | [Zhanxueyou/deepseek-balance](https://github.com/Zhanxueyou/deepseek-balance) | 1 | 2026-08-30 | 2026-08-30 | 零依赖 Python CLI 查询 DeepSeek API 余额，低余额自动提醒并发送 macOS 通知；附带 DSH 侧边栏插件，实时展示余额、今日/本月用量与缓存命中率。 |
| 752 | [Zhanxueyou/dsh-plugin-manager](https://github.com/Zhanxueyou/dsh-plugin-manager) | 1 | 2026-08-30 | 2026-08-30 | DSH Web 客户端插件管理器侧边栏面板：全量插件清单（描述/状态/来源/版本/分类）、启停热重载、删除本地自定义插件，并可浏览、搜索、一键安装 GitHub topic:dsh-plugin 远程插件。 |
| 753 | [zhaoxuejie/dsh-daily-digest](https://github.com/zhaoxuejie/dsh-daily-digest) | 1 | 2026-08-27 | 2026-08-27 | DSH 每日工作摘要插件：自动记录任务/会话/错误，一键生成日报/周报 Markdown，Web 悬浮摘要卡 |
| 754 | [zhaoxuejie/dsh-plugin-learning-path](https://github.com/zhaoxuejie/dsh-plugin-learning-path) | 1 | 2026-08-21 | 2026-08-27 | DeepSeek Harness 插件开发学习教程：15 节课程 + 4 个实战项目 + 发布课，交互式单页应用，纯 HTML/CSS/JS 零构建 |
| 755 | [Zhiye-Tang/weibo-wallpaper-dsh-plugin](https://github.com/Zhiye-Tang/weibo-wallpaper-dsh-plugin) | 1 | 2026-09-03 | 2026-09-03 | 把微博博主的相册变成(DSH)Web 界面壁纸的宿主插件。每次打开 DSH 自动检查微博:同一天跳过,跨天/跨月增量下载,按月归档到本地 YYYY-MM 文件夹，首次启用自动回填今年1月到上个月的历史相册。即一个插件、一个你本人的微博 Cookie,就可同时跟踪多位博主(每人独立文件夹与状态) 三种显示模式 + 月份切换,控制条常驻页面底部。A DSH host plugin that syncs a Weibo blogger's album by month into local folders and shows them as the wallpaper behind  the DSH web UI. Cookie is required and stay local. |
| 756 | [Zhiyi-Zhao/dsh-notion-skill](https://github.com/Zhiyi-Zhao/dsh-notion-skill) | 1 | 2026-08-27 | 2026-08-27 | DSH (DeepSeek Harness) skill: read/write Notion workspaces via the official REST API |
| 757 | [Zhiyi-Zhao/file-brief](https://github.com/Zhiyi-Zhao/file-brief) | 1 | 2026-07-30 | 2026-08-27 | Task-local, privacy-preserving file catalogs for reusable Codex input-file understanding. |
| 758 | [zhongjie10086/dsh-adaptive-native](https://github.com/zhongjie10086/dsh-adaptive-native) | 1 | 2026-08-16 | 2026-08-30 | Windows-native Adaptive preset for DeepSeek Harness |
| 759 | [zhoupengyun572-cell/dsh-hana-research](https://github.com/zhoupengyun572-cell/dsh-hana-research) | 1 | 2026-08-28 | 2026-08-28 | A local literature review, PDF annotation, evidence synthesis, and research notes workbench for DeepSeek Harness. |
| 760 | [zhuzichen362/dsh-call-shrink](https://github.com/zhuzichen362/dsh-call-shrink) | 1 | 2026-08-29 | 2026-08-29 | dsh |
| 761 | [ZIye1208/dsh-github-mcp](https://github.com/ZIye1208/dsh-github-mcp) | 1 | 2026-09-03 | 2026-09-04 | DSH 插件：GitHub MCP 连接插件，token 存 DSH 凭据中心(.credentials.yaml)，自动捆绑安装面板插件 dsh-github-mcp-hint（可独立卸载）。 |
| 762 | [ZIye1208/dsh-github-mcp-hint](https://github.com/ZIye1208/dsh-github-mcp-hint) | 1 | 2026-09-03 | 2026-09-04 | DSH 插件：GitHub MCP 示例提示面板（设置→插件，随机 4/30 条可复制）+ 公开仓库统计（星/fork）+ gh_repo_stats 模型工具（星数/近14天克隆量） |
| 763 | [zjh02249/dsh-desktop-operator](https://github.com/zjh02249/dsh-desktop-operator) | 1 | 2026-08-27 | 2026-08-27 | DSH Desktop Operator: safe Windows Computer Use, desktop automation, UI Automation, and MCP tools for DeepSeek Harness |
| 764 | [Zleap-AI/dsh-sag](https://github.com/Zleap-AI/dsh-sag) | 1 | 2026-08-29 | 2026-08-29 | 面向 DeepSeek Harness 的 SAG 本地个人知识库插件，支持知识检索、原文读取、文件上传、文本写入与文档管理。 |
| 765 | [zw11591-sketch/dsh-pet-panel](https://github.com/zw11591-sketch/dsh-pet-panel) | 1 | 2026-08-28 | 2026-08-28 | A desktop pet plus a conversation overview panel for the DeepSeek Harness Web UI — self-contained client plugin (no host service) |
| 766 | [ZZZjf13960/dsh-onfail](https://github.com/ZZZjf13960/dsh-onfail) | 1 | 2026-08-28 | 2026-08-28 | DSH plugin: poll GitHub Actions, surface failed checks as cards, open a fix session with log context. |
| 767 | [01Virex/dsh-deepshub](https://github.com/01Virex/dsh-deepshub) | 0 | 2026-09-02 | 2026-09-02 | Pornhub-style parody reskin for the DeepSeek Harness web UI — orange/black pill-button theme, "Deephub" wordmark, 18+ entry gate & HD badges. Pure meme, no explicit content. |
| 768 | [1010n111/dsh-about](https://github.com/1010n111/dsh-about) | 0 | 2026-09-02 | 2026-09-02 | 为 DeepSeek Harness Web 设置面板添加“关于”页，展示当前运行的 DSH 版本、插件版本与项目主页。 |
| 769 | [123dbl/dsh-side-session](https://github.com/123dbl/dsh-side-session) | 0 | 2026-09-03 | 2026-09-03 | DSH side-chat (旁会话) plugin: launch a fresh continuable parallel session from the conversation header while the main session keeps running. |
| 770 | [123twtd/dsh-skin-manager](https://github.com/123twtd/dsh-skin-manager) | 0 | 2026-08-30 | 2026-09-03 | DeepSeek Harness (dsh) 可切换皮肤包管理器：皮肤包发现/激活/ZIP 导入，适配 0.1.x，含爱弥斯示例皮肤 |
| 771 | [123twtd/dsh-vision-toggle](https://github.com/123twtd/dsh-vision-toggle) | 0 | 2026-08-30 | 2026-09-03 | DeepSeek Harness (dsh) 模型视觉开关插件：为自定义模型声明图像输入能力（写入 llm-pi-ai 配置），适配 0.1.x |
| 772 | [1710782766/dsh-browser-verify](https://github.com/1710782766/dsh-browser-verify) | 0 | 2026-09-02 | 2026-09-02 | Browser verification for DeepSeek Harness — open, mock, assert, screenshot in a few tool calls, screenshots auto-project into the model context |
| 773 | [1Ecc/dsh-lenovo-toolkit](https://github.com/1Ecc/dsh-lenovo-toolkit) | 0 | 2026-08-28 | 2026-08-28 | 联想专业工具集 · DeepSeek Harness 插件。电池健康检测（macOS/Windows）：容量、循环次数、双口径健康度、SVG 衰减趋势图与系统官方电池报告。Lenovo professional toolkit for DeepSeek Harness. |
| 774 | [2092372408-pixel/dsh-roadmap-board](https://github.com/2092372408-pixel/dsh-roadmap-board) | 0 | 2026-09-02 | 2026-09-02 | 人机共享的执行路线图看板：横向阶段→步骤、技能绑定、实时同步、跨项目复用（Human-AI shared execution roadmap board for DSH） |
| 775 | [2877905731/dsh-think-autoexpand](https://github.com/2877905731/dsh-think-autoexpand) | 0 | 2026-08-27 | 2026-08-27 | dsh-think-autoexpand：让 DeepSeek Harness 里的 Think 思考行始终可见，并在流式输出时自动展开，实时查看 Agent 完整推理过程；保留工具卡折叠体验。 |
| 776 | [3361805598-gif/dsh-usage-insights](https://github.com/3361805598-gif/dsh-usage-insights) | 0 | 2026-09-04 | 2026-09-04 | Local-first personal usage insights for DeepSeek Harness |
| 777 | [618527/dsh-install-guard](https://github.com/618527/dsh-install-guard) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件安装前兼容性预检守卫：检查 Node/engines、@deepseek-ai peer 版本与 dsh 清单，可选隔离试启动。 |
| 778 | [666emmm/dsh-file-upload](https://github.com/666emmm/dsh-file-upload) | 0 | 2026-08-31 | 2026-08-31 | dsh-file-upload fork: uploaded-file management (list/info/delete/@path) + zero-copy clipboard path reading for DeepSeek Harness |
| 779 | [6jeffr3y/dsh-burpsuite-mcp](https://github.com/6jeffr3y/dsh-burpsuite-mcp) | 0 | 2026-08-30 | 2026-08-30 | Native Burp Suite MCP tools and live settings for DeepSeek Harness |
| 780 | [6jeffr3y/dsh-session-manager](https://github.com/6jeffr3y/dsh-session-manager) | 0 | 2026-08-30 | 2026-08-30 | Session archive, tagging, relationship graph and safe deletion for DeepSeek Harness Web |
| 781 | [782042369/dsh-model-compat-guard](https://github.com/782042369/dsh-model-compat-guard) | 0 | 2026-09-01 | 2026-09-02 | DSH (DeepSeek Harness) compatibility guard plugin: fixes reasoning-model compaction truncation, doomed sandbox-escalation fail-close, and missing tool description for GPT/Qwen/third-party models |
| 782 | [a1303845406/dsh-comfy-video-studio](https://github.com/a1303845406/dsh-comfy-video-studio) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的 ComfyUI MiniMax H3 视频工作台 |
| 783 | [a1303845406/dsh-sakura-theme](https://github.com/a1303845406/dsh-sakura-theme) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的晴樱与夜樱主题插件 |
| 784 | [a792883583/dsh-smart-reminder](https://github.com/a792883583/dsh-smart-reminder) | 0 | 2026-09-02 | 2026-09-02 | Smart calendar reminder & schedule assistant for DSH Web GUI: lunar calendar, holidays, system notifications on macOS/Windows, and WeCom/platform push integration. |
| 785 | [aayan-cloud/dsh-reelsmaker](https://github.com/aayan-cloud/dsh-reelsmaker) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness plugin: turn narration lines into a finished vertical reel. Free neural voice, burned-in captions, no API keys. |
| 786 | [ABccgh/dsh-desktop-dev](https://github.com/ABccgh/dsh-desktop-dev) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness agent preset: Windows full-stack desktop development team |
| 787 | [abworks-dev/dsh-plugin-lab](https://github.com/abworks-dev/dsh-plugin-lab) | 0 | 2026-09-01 | 2026-09-01 | Workshop and lab for developing, testing, and maintaining DeepSeek Harness Cordis plugins. |
| 788 | [Aclypea/dsh-repetition-guard](https://github.com/Aclypea/dsh-repetition-guard) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 模型输出复读熔断插件 / Repetition guard plugin for DeepSeek Harness |
| 789 | [addie-ace/dsh-fullwidth-punctuation](https://github.com/addie-ace/dsh-fullwidth-punctuation) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 插件：让 AI 回答输出中文全角标点（用户直接复制回答内容也是全角）。监听 llm/stream 做智能半角→全角转换，跳过代码块/数字/URL/markdown，并注入 system prompt 提示。 |
| 790 | [adoreQ/deepseek-balance](https://github.com/adoreQ/deepseek-balance) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness查看余额插件 |
| 791 | [ADXZXCD/dsh-web-mobile](https://github.com/ADXZXCD/dsh-web-mobile) | 0 | 2026-09-01 | 2026-09-01 | Mobile layout enhancement plugin for DeepSeek Harness Web UI |
| 792 | [Aetheri-AI/dsh-plugins](https://github.com/Aetheri-AI/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | Community plugins for DeepSeek Harness (dsh) |
| 793 | [afterDDL/dsh-creator-shared-blueprint](https://github.com/afterDDL/dsh-creator-shared-blueprint) | 0 | 2026-08-25 | 2026-09-01 | A shared interface for humans and AI to understand, discuss, modify, and extend DeepSeek Harness agents. |
| 794 | [aijunjiang/dsh-plugin-vision](https://github.com/aijunjiang/dsh-plugin-vision) | 0 | 2026-09-03 | 2026-09-03 | Give your DSH agent eyes via any OpenAI-compatible vision model - 11 provider presets (Doubao/Qwen-VL/GLM-V/OpenAI/Gemini/Ollama...), capability checkboxes that inject live prompt guidance, and analysis of images the user drops into the chat; the agent writes its own observation prompt, and base64 never enters its context. |
| 795 | [aijunjiang/dsh-remote-ssh](https://github.com/aijunjiang/dsh-remote-ssh) | 0 | 2026-09-02 | 2026-09-02 | Run your DSH workspace on a remote host over SSH - connection sidebar, remote directory browser, per-session routing, agent ssh_exec/route-status; files and commands execute on your target while sessions, GUI and $DSH_HOME stay local. |
| 796 | [aiko-dsh-plugins/dsh-bid-studio](https://github.com/aiko-dsh-plugins/dsh-bid-studio) | 0 | 2026-08-29 | 2026-08-29 | Installable Bid Studio workbench for DeepSeek Harness |
| 797 | [aiko-dsh-plugins/dsh-ontology-kernel](https://github.com/aiko-dsh-plugins/dsh-ontology-kernel) | 0 | 2026-08-29 | 2026-08-29 | Installable Ontology Kernel bundle for DeepSeek Harness |
| 798 | [ailiasdesu/dsh-session-manager](https://github.com/ailiasdesu/dsh-session-manager) | 0 | 2026-08-28 | 2026-08-28 | DSH session migration plugin: drag-and-drop sessions between workspaces in the Web UI settings panel (auto backup/rollback, official workspaceRegistry sync) |
| 799 | [ailreth/xiaoxiao-persona-core](https://github.com/ailreth/xiaoxiao-persona-core) | 0 | 2026-08-30 | 2026-08-31 | A persona-core injection plugin for DeepSeek Harness — an honest, boundary-aware, gentle-yet-firm AI persona; an attempt at whether AI can birth consciousness. |
| 800 | [AKUSH99/dsh-balance-chip](https://github.com/AKUSH99/dsh-balance-chip) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek API balance in the DSH sidebar footer and bottom-right pill - live status dot plus amount, 60s refresh, API key stays in the local credential store |
| 801 | [alaxrpg/dsh-chatgpt-pip](https://github.com/alaxrpg/dsh-chatgpt-pip) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：ChatGPT 画中画小窗 + 把 ChatGPT 定稿计划回流到新 DSH 对话执行 |
| 802 | [alaxrpg/dsh-subagent-route-badges](https://github.com/alaxrpg/dsh-subagent-route-badges) | 0 | 2026-08-27 | 2026-08-27 | Display subagent provider, model, and reasoning effort badges in DeepSeek Harness |
| 803 | [alaxrpg/dsh-vision-bridge](https://github.com/alaxrpg/dsh-vision-bridge) | 0 | 2026-08-25 | 2026-08-27 | DSH 插件：为纯文本模型提供视觉能力，支持任意 OpenAI 兼容多模态 API |
| 804 | [Albertlsy588/dsh-release-sentinel](https://github.com/Albertlsy588/dsh-release-sentinel) | 0 | 2026-09-01 | 2026-09-01 | DSH local read-only control plugin for Release Sentinel |
| 805 | [Albertlsy588/dsh-shipgate](https://github.com/Albertlsy588/dsh-shipgate) | 0 | 2026-08-28 | 2026-08-28 | Local-first DSH pre-merge delivery receipt generator |
| 806 | [alchemistwu/dsh-tool-call-guard](https://github.com/alchemistwu/dsh-tool-call-guard) | 0 | 2026-08-30 | 2026-08-31 | DSH plugin: neutralize tool calls with invalid JSON arguments on the wire — so one malformed model generation cannot brick a session against strict OpenAI-compatible servers (vLLM) |
| 807 | [alenhu2005/dsh-usage-export](https://github.com/alenhu2005/dsh-usage-export) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin for token usage cost, PDF/Markdown transcript export, and expanded conversation statistics. |
| 808 | [alexchen5/research-epic-manager](https://github.com/alexchen5/research-epic-manager) | 0 | 2026-08-24 | 2026-08-31 | Agent skills for running research projects end-to-end using a plain-file epic→issues→comments tracker. |
| 809 | [AlgoVaultLabs/dsh-algovault](https://github.com/AlgoVaultLabs/dsh-algovault) | 0 | 2026-08-30 | 2026-08-30 | Preconfigured DeepSeek Harness bundle for the AlgoVault MCP server — composite trade calls, market regime and cross-venue funding arbitrage as mcp__algovault__* tools. |
| 810 | [alin-ever/dsh-plugin-autoqueue](https://github.com/alin-ever/dsh-plugin-autoqueue) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 无人值守任务队列插件：丢 .md 进收件箱 → AI 自动执行 → 产出报告 |
| 811 | [All3nCN/dsh-better-sidebar-N23](https://github.com/All3nCN/dsh-better-sidebar-N23) | 0 | 2026-08-31 | 2026-08-31 | DSH web plugin: complete workbench (explorer/editors/previews/terminal/git/browser/tasks) + shell refactor. Fork of omdsh-dev/DSH-better-sidebar under @all3cn scope. |
| 812 | [All3nCN/dsh-qa-suite-N23](https://github.com/All3nCN/dsh-qa-suite-N23) | 0 | 2026-09-01 | 2026-09-01 | DSH quality suite plugin: automatic tsc --noEmit diagnostics (code_check tool) + multi-lens /code-review command. Merged absorption of dsh-code-check (BSD-3) and dsh-command-code-review (MIT). |
| 813 | [alpacachen/dsh-automation](https://github.com/alpacachen/dsh-automation) | 0 | 2026-08-30 | 2026-08-30 | Schedule and manage one-time and recurring Agent tasks in DeepSeek Harness |
| 814 | [Alphauni-x/dsh-ds-home-bg](https://github.com/Alphauni-x/dsh-ds-home-bg) | 0 | 2026-09-02 | 2026-09-04 | Deep-navy aurora background theme for the DeepSeek Harness web UI: layered radial glows, fine grid and a drifting halftone whale, following the host Appearance setting. |
| 815 | [altuman-w/dsh-plugin-plantuml](https://github.com/altuman-w/dsh-plugin-plantuml) | 0 | 2026-08-31 | 2026-08-31 | deepseek harness plugin view plantuml |
| 816 | [ALwith-ai/dsh-agent](https://github.com/ALwith-ai/dsh-agent) | 0 | 2026-08-16 | 2026-09-04 | Interactive ACP v2 bridge for DeepSeek Harness (dsh) — streaming, run-state reporting, permissions. ALwith Desktop is its reference client. |
| 817 | [Amengclass/dsh-settings-hub](https://github.com/Amengclass/dsh-settings-hub) | 0 | 2026-08-26 | 2026-09-04 | dsh plugin: take over settings shell, regroup third-party plugins under one collapsible group |
| 818 | [americanjeff/modelspoke](https://github.com/americanjeff/modelspoke) | 0 | 2026-09-04 | 2026-09-04 | Local OpenAI-compatible model-server discovery + tiered reasoning-metadata resolution for DeepSeek Harness (dsh). |
| 819 | [Amoss-1/routine-taskboard](https://github.com/Amoss-1/routine-taskboard) | 0 | 2026-08-27 | 2026-08-28 | Self-contained routine board plugin for DeepSeek Harness (DSH): scheduled job placards with scripts, IO artifacts, health lamps. MIT. |
| 820 | [AnakinWu/DSH-plugin](https://github.com/AnakinWu/DSH-plugin) | 0 | 2026-08-30 | 2026-08-30 | Anakin‘s dsh-plugins |
| 821 | [andrepontesmelo/dsh-model-router](https://github.com/andrepontesmelo/dsh-model-router) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: virtual model routes with failover, exponential backoff, sleep windows |
| 822 | [andrepontesmelo/dsh-suite](https://github.com/andrepontesmelo/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | The DSH productivity suite: plugins + agent skills for the DeepSeek Harness, installable in one command. |
| 823 | [andrepontesmelo/moving-target](https://github.com/andrepontesmelo/moving-target) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: cold-start context — distills your first prompts into one goal paragraph injected into every new session |
| 824 | [AndyZHENG0715/dsh-recovery](https://github.com/AndyZHENG0715/dsh-recovery) | 0 | 2026-09-03 | 2026-09-04 | DSH self-recovery: zero-dependency CLI (scan/snapshot/rollback/safemode/boot-probe/doctor) + in-process watchdog plugin. Process-external boot gate, tiered recovery ladder, safe/repair profiles. |
| 825 | [anlew07/dsh-conversation-atlas](https://github.com/anlew07/dsh-conversation-atlas) | 0 | 2026-09-04 | 2026-09-04 | Project-level conversation memory explorer for DeepSeek Harness with related memories, cross-session bridges, BM25 search, and exact chat navigation. |
| 826 | [Anna-la/dsh-simplify](https://github.com/Anna-la/dsh-simplify) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 界面简化插件：清理模式下右键移除页面元素，设置页中可原样恢复。 |
| 827 | [Anna-la/dsh-submodel-change](https://github.com/Anna-la/dsh-submodel-change) | 0 | 2026-08-27 | 2026-08-29 | 可以选择子 agent 调用的模型。 |
| 828 | [Anna-la/dsh-token-stat](https://github.com/Anna-la/dsh-token-stat) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness token 用量统计插件: 按模型/日期区分, 设置页看板, 数据目录在线更改 |
| 829 | [AnonyJcy/dsh-plugin-j-space](https://github.com/AnonyJcy/dsh-plugin-j-space) | 0 | 2026-08-23 | 2026-08-27 | J-Space Cognition Suite V3.7 原生 DeepSeek Harness 智能体预设与独立 Cordis 插件，提供深层推理路由、工作区状态外化账本（.jspace）与全模型解耦的认知工作空间 |
| 830 | [AnonyJcy/dsh-plugin-mobile-touch](https://github.com/AnonyJcy/dsh-plugin-mobile-touch) | 0 | 2026-08-27 | 2026-08-28 | Mobile & iPad touch optimization plugin for DeepSeek Harness Web GUI |
| 831 | [Ansonfishing/dsh-model-manager](https://github.com/Ansonfishing/dsh-model-manager) | 0 | 2026-08-28 | 2026-08-28 | Manage local LLM inference servers in DSH: GPU registry, parameter profiles, VRAM validation, and tok/s benchmarks for llama.cpp, SGLang, and vLLM |
| 832 | [Anyway-one/dsh-balance](https://github.com/Anyway-one/dsh-balance) | 0 | 2026-08-26 | 2026-08-27 | 为 DeepSeek Harness 提供持久化的余额与用量显示插件，让您随时掌握资源消耗情况，无需离开工作区。 |
| 833 | [aokamoaki/dsh-stall-sentinel](https://github.com/aokamoaki/dsh-stall-sentinel) | 0 | 2026-09-03 | 2026-09-03 | Lightweight stall watchdog for DeepSeek Harness - auto-wires subprocess spawn, reminds + forensics on stall, never kills. |
| 834 | [aosi526/dsh-workbuddy-xdpool](https://github.com/aosi526/dsh-workbuddy-xdpool) | 0 | 2026-09-04 | 2026-09-04 | Merge every locally signed-in WorkBuddy account into DeepSeek Harness as one auto-failing-over model pool (multi-account rotation, live credits and model catalog). |
| 835 | [Army1900/dsh-e2e-dev-sdd](https://github.com/Army1900/dsh-e2e-dev-sdd) | 0 | 2026-08-26 | 2026-08-27 | dsh插件，用于驱动定制的e2e开发 |
| 836 | [ArmyWas/dsh-provider-passport](https://github.com/ArmyWas/dsh-provider-passport) | 0 | 2026-09-01 | 2026-09-01 | Review-first request-dialect preflight for custom DeepSeek Harness providers. |
| 837 | [asdasdsdsdasdasdasd/dsh-computer-use](https://github.com/asdasdsdsdasdasdasd/dsh-computer-use) | 0 | 2026-08-25 | 2026-08-29 | Linux X11 computer-use for DeepSeek Harness: screenshot, mouse, keyboard via a zero-dependency Python XTest helper — no Node native modules, no accessibility framework. |
| 838 | [ash-qw/dsh-theme-prts](https://github.com/ash-qw/dsh-theme-prts) | 0 | 2026-08-31 | 2026-09-02 | Unofficial personal non-commercial Arknights P.R.T.S. fan UI for DeepSeek Harness |
| 839 | [AstralFoundry/dsh-workspace](https://github.com/AstralFoundry/dsh-workspace) | 0 | 2026-08-27 | 2026-08-27 | A lightweight IDE and Git workspace plugin for DeepSeek Harness |
| 840 | [auggie246/dsh-llm-openai-codex](https://github.com/auggie246/dsh-llm-openai-codex) | 0 | 2026-08-19 | 2026-09-01 | OpenAI Codex (ChatGPT Plus/Pro subscription) LLM provider for the DeepSeek Harness — OAuth tokens from the Codex CLI, no API key required |
| 841 | [auggie246/dsh-mattpocock-skills](https://github.com/auggie246/dsh-mattpocock-skills) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to install Mattpocock skills. |
| 842 | [auggie246/dsh-output-styles](https://github.com/auggie246/dsh-output-styles) | 0 | 2026-08-28 | 2026-08-28 | Enable output styles in Deepseek Harness settings! |
| 843 | [auggie246/dsh-sidebar](https://github.com/auggie246/dsh-sidebar) | 0 | 2026-08-27 | 2026-08-28 | Sidebar and panels for full developer interaction! |
| 844 | [auggie246/dsh-synthetic-web-search](https://github.com/auggie246/dsh-synthetic-web-search) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to use synthetic.new web search instead of built-in Deepseek web search |
| 845 | [auggie246/dsh-webapp](https://github.com/auggie246/dsh-webapp) | 0 | 2026-08-29 | 2026-09-03 | Desktop shell for the DeepSeek Harness (DSH) web GUI: window, attach-or-spawn, Host bar, hide-to-bar, quit-kills-host. |
| 846 | [avdergh/chroma-cut](https://github.com/avdergh/chroma-cut) | 0 | 2026-08-28 | 2026-08-28 | Preserve anti-aliased outlines while cutting chroma-backed game assets. CLI + MCP + Codex plugin. |
| 847 | [awol2005ex3/dsh-export-session](https://github.com/awol2005ex3/dsh-export-session) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness（`dsh`）插件：把**当前会话的完整内容**一键导出为 **Markdown（`.md`）/ Word（`.docx`）/ PDF（`.pdf`）**。 |
| 848 | [awol2005ex3/dsh-logo-custom](https://github.com/awol2005ex3/dsh-logo-custom) | 0 | 2026-08-31 | 2026-09-01 | DeepSeek Harness 自定义 Logo 插件 — 上传图片替换侧边栏左上角的品牌图标和文字。 |
| 849 | [awol2005ex3/dsh-md-table-export](https://github.com/awol2005ex3/dsh-md-table-export) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（`dsh`）插件：把对话内容里的 **Markdown 表格** 一键导出为 **Excel（`.xlsx`）**。 |
| 850 | [awol2005ex3/dsh-role-manager](https://github.com/awol2005ex3/dsh-role-manager) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（dsh）角色管理插件。为每个"角色"预设一份初始系统提示词，在 Web 界面中切换当前角色，从而让模型以不同的身份 / 设定开始对话。 |
| 851 | [awol2005ex3/dsh-user-manager](https://github.com/awol2005ex3/dsh-user-manager) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness（`dsh`）插件：为单机的 harness 增加**用户管理**与**会话按用户隔离**。 |
| 852 | [axdlee/dsh-yeelight-smart-home](https://github.com/axdlee/dsh-yeelight-smart-home) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: Yeelight smart home control via the local yeelight-home runtime (skill, tools, settings card) |
| 853 | [axel286137079-dot/dsh-skill-matcher](https://github.com/axel286137079-dot/dsh-skill-matcher) | 0 | 2026-09-01 | 2026-09-01 | Skill & Expert Matcher for DeepSeek Harness (dsh plugin) |
| 854 | [ayumedaze/dsh-git](https://github.com/ayumedaze/dsh-git) | 0 | 2026-08-29 | 2026-08-29 | dsh-plugin |
| 855 | [Azonda/dsh-whale-writing](https://github.com/Azonda/dsh-whale-writing) | 0 | 2026-08-30 | 2026-08-31 | 老人与大肥鱼：Deepseek Harness超级写作增强插件，具备四种风格和五种写作严谨度的自动切换功能，并且具备任务级本地记忆和去ai味后处理、。 |
| 856 | [azure5100/huahua-dsh-chatroom](https://github.com/azure5100/huahua-dsh-chatroom) | 0 | 2026-09-04 | 2026-09-04 | dsh-chat/dsh-weave cross-machine group chat: Fix1-Fix4 adaptation patches + ops documentation set (sanitized) |
| 857 | [bailong-Hakuryu/dsh-engineering-control-plane](https://github.com/bailong-Hakuryu/dsh-engineering-control-plane) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 工程任务编排与发布门禁插件，支持 /mission 指令、任务路由、计划执行、验证和状态跟踪。 \| Engineering mission orchestration and release-gate plugin for DeepSeek Harness with /mission routing, planning, execution, verification, and status tracking. |
| 858 | [bailong-Hakuryu/dsh-security-assurance](https://github.com/bailong-Hakuryu/dsh-security-assurance) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 策略驱动的仓库安全评估插件，支持包生命周期评估、证据、发现、裁决、导出和 /security 指令。 \| Policy-driven repository security assurance plugin for DeepSeek Harness with package lifecycle assessments, evidence, findings, verdicts, exports, and /security routing. |
| 859 | [baiyang123/dsh-audit-missing](https://github.com/baiyang123/dsh-audit-missing) | 0 | 2026-08-27 | 2026-08-28 | 对照开发计划等文档，当AI开发完一个迭代之后扫描是否有漏开发的功能（真的好用） |
| 860 | [BaoBao1996121/dsh-restart-ui](https://github.com/BaoBao1996121/dsh-restart-ui) | 0 | 2026-08-28 | 2026-08-28 | One-click cross-platform restart button for DeepSeek Harness Web UI |
| 861 | [BarrierFly/apx-watchdog](https://github.com/BarrierFly/apx-watchdog) | 0 | 2026-08-26 | 2026-08-27 | 牛来写的东西 |
| 862 | [Barry-Liu-001/dsh_ark_plan_usage](https://github.com/Barry-Liu-001/dsh_ark_plan_usage) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 侧边栏插件：实时展示火山方舟 Agent Plan 用量（5h/周/月），数据来自本机 arkcli |
| 863 | [Barry-Liu-001/dsh_chat_index](https://github.com/Barry-Liu-001/dsh_chat_index) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 对话索引插件：在对话区右边缘显示一列小圆点，每个点代表一条用户发送的消息。圆点等间距、紧凑、纵向居中排列（消息过多放不下时间距自动压缩以适应高度）；当前阅读位置的点高亮为品牌色。 |
| 864 | [bbboy31/dsh-terminal-tabs](https://github.com/bbboy31/dsh-terminal-tabs) | 0 | 2026-08-26 | 2026-08-27 | Terminals view tab for DeepSeek Harness web UI — live background job count, streaming output, one-click kill |
| 865 | [benz-ai-x/dsh-md-preview](https://github.com/benz-ai-x/dsh-md-preview) | 0 | 2026-09-01 | 2026-09-01 | DSH (DeepSeek Harness) Web GUI plugin — preview, edit & browse workspace markdown/text files right beside the chat: rich preview panel, guarded editing with conflict detection, lazy workspace file tree. 预览/编辑/浏览会话工作区文档 |
| 866 | [benz-ai-x/dsh-session-graph](https://github.com/benz-ai-x/dsh-session-graph) | 0 | 2026-08-28 | 2026-08-30 | Visual session graph for DeepSeek Harness — browse, arrange, branch, merge, and summarize AI agent sessions on an interactive canvas. |
| 867 | [berserk0501/dsh-soundscape](https://github.com/berserk0501/dsh-soundscape) | 0 | 2026-08-26 | 2026-08-27 | DSH 本机思考与工具音效插件，支持 MediaPlayer、WAV/MP3、自定义映射和设置面板 |
| 868 | [bg8lng/dsh-openlist-sync](https://github.com/bg8lng/dsh-openlist-sync) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 文件同步插件：交付文件自动上传 OpenList + 目录全读写工具 + 设置面板 + 按工作区布局 |
| 869 | [Bigesila-B/dsh-media-forge](https://github.com/Bigesila-B/dsh-media-forge) | 0 | 2026-08-26 | 2026-08-27 | DSH Media Forge plugin: agent + skills workflow for media-generation APIs, with a sidebar skill panel (zh/en docs) |
| 870 | [bigharm/dsh-agentnoodle](https://github.com/bigharm/dsh-agentnoodle) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness 插件：AI 驱动的群像聊天游戏框架。轻量化酒馆。兼容 SillyTavern V1/V2/V3 JSON 和 PNG 内嵌卡片。添加npc和场景之类的，给harness提要求，让它做就行。玩家输入一个行动，场景中多个 NPC 各自做出反应，每条反应独立成一条带头像插图的聊天室消息；支持场景切换、NPC 关系变化与本地 JSON 存档。 |
| 871 | [BiKing567/dsh-subagent-panel](https://github.com/BiKing567/dsh-subagent-panel) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：把每个子代理渲染成主对话里可点击的卡片，点击直接进入子代理会话（与标题栏同一路径）。\| DSH plugin: render every subagent as a clickable inline card that opens the child session — same navigation the header's subagent catalog uses. |
| 872 | [BISTU-guheihei/DSH-SessionManager](https://github.com/BISTU-guheihei/DSH-SessionManager) | 0 | 2026-08-26 | 2026-08-27 | DSH 会话管理工具：可视化/命令行查看与删除历史聊天记录，自动清理缓存残留 |
| 873 | [BitDG/dsh-cloud-model-providers](https://github.com/BitDG/dsh-cloud-model-providers) | 0 | 2026-09-01 | 2026-09-01 | 接入 Ant Digital MaaS 与 NVIDIA NIM 流式模型路由 / Streaming model routes for DSH |
| 874 | [BitDG/dsh-plugins](https://github.com/BitDG/dsh-plugins) | 0 | 2026-09-02 | 2026-09-04 | Public collection of independently versioned DeepSeek Harness plugins |
| 875 | [bitsmug/dsh-bgjobs](https://github.com/bitsmug/dsh-bgjobs) | 0 | 2026-09-03 | 2026-09-03 | 将命令提交为独立于 DSH 进程的后台任务，关闭 DSH 也不影响运行，并提供实时网页面板与离线 CLI/GUI 管理。Runs commands as background jobs that keep executing when DSH exits, with a live web panel and offline CLI/GUI management. |
| 876 | [bitterSmilezzz/dsh-asr-voice](https://github.com/bitterSmilezzz/dsh-asr-voice) | 0 | 2026-08-25 | 2026-08-27 | 开口即成文 · Speak-to-prompt for DeepSeek Harness：云端 ASR 语音识别 + 提示词优化 + 填入草稿/自动发送，跨平台 macOS / Windows。 |
| 877 | [bitterSmilezzz/dsh-model-selector](https://github.com/bitterSmilezzz/dsh-model-selector) | 0 | 2026-08-27 | 2026-09-01 | DeepSeek Harness (DSH) 的增强模型选择器：单层菜单（搜索 + 分组）+ 底部内联推理强度（Effort）滑杆。 |
| 878 | [blairlaird/dsh-agent-mailbox](https://github.com/blairlaird/dsh-agent-mailbox) | 0 | 2026-09-01 | 2026-09-01 | Durable agent-to-agent messaging for DeepSeek Harness: threads, receipts, search, broadcast, attachments, presence, SSE streaming, signing. Zero dependencies. |
| 879 | [bleakbelladonnals/dsh-artifact-harbor](https://github.com/bleakbelladonnals/dsh-artifact-harbor) | 0 | 2026-08-27 | 2026-08-27 | Artifact Harbor — secure, session-aware artifact previews for DeepSeek Harness Web |
| 880 | [bleakbelladonnals/dsh-echo](https://github.com/bleakbelladonnals/dsh-echo) | 0 | 2026-08-27 | 2026-08-27 | Record MCP once. Replay it safely inside DeepSeek Harness. |
| 881 | [bleamayaka/dsh-file-beam](https://github.com/bleamayaka/dsh-file-beam) | 0 | 2026-08-27 | 2026-08-27 | dsh-file-beam - DSH plugin: drag files into the web composer, resolve real absolute paths, hidden path injection for the agent (no copy, no path in composer). |
| 882 | [bLueriVerLHR/dsh-better-webui](https://github.com/bLueriVerLHR/dsh-better-webui) | 0 | 2026-08-20 | 2026-08-27 | Minimal improvement if possible. |
| 883 | [bo961386926/dolphin-pet-plugin](https://github.com/bo961386926/dolphin-pet-plugin) | 0 | 2026-08-26 | 2026-08-27 | Cute desktop pet for DeepSeek Harness - custom name, upload your own pet image, or generate one with AI. DSH 桌面宠物插件 |
| 884 | [bosinHU/dsh-skill-editor](https://github.com/bosinHU/dsh-skill-editor) | 0 | 2026-08-29 | 2026-08-30 | Edit skills directly in DSH web settings |
| 885 | [BoWuGit/dsh-reasoning](https://github.com/BoWuGit/dsh-reasoning) | 0 | 2026-08-31 | 2026-08-31 | Codex-style /reasoning command for DeepSeek Harness Web |
| 886 | [Britneycode/dsh-distillery](https://github.com/Britneycode/dsh-distillery) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：本地蒸馏器——扫历史会话挖「用户纠错 → 改对」片段，脱敏后蒸馏成微调 JSONL / SKILL.md 技能草稿 / AGENTS.md 规则补丁，带人工审核队列 |
| 887 | [Britneycode/dsh-live-room](https://github.com/Britneycode/dsh-live-room) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：把会话变成免登录、只读、可分享的实时直播间（SSE 观看页 + 弹幕 + agent 工具） |
| 888 | [Bronier/dsh-web-search-so360](https://github.com/Bronier/dsh-web-search-so360) | 0 | 2026-08-27 | 2026-08-27 | Keyless web search provider for DeepSeek Harness backed by 360 Search (so.com). |
| 889 | [bruc3van/dsh-doctor](https://github.com/bruc3van/dsh-doctor) | 0 | 2026-08-29 | 2026-08-29 | 面向 Agent 的 DeepSeek Harness 插件升级与排障工具：分析版本差异、迁移代码、验证构建与运行，并诊断 profile、依赖和配置问题。 |
| 890 | [bvcvb/dsh-baize-rules](https://github.com/bvcvb/dsh-baize-rules) | 0 | 2026-08-31 | 2026-09-01 | DeepSeek Harness (DSH) plugin — inject durable user-set session/global must-do / must-not requirements into the model at conversation start (Baize). |
| 891 | [bycall/dsh-code-collector](https://github.com/bycall/dsh-code-collector) | 0 | 2026-08-27 | 2026-08-27 | Session code collector for DeepSeek Harness: gather every code block the model produced in the current session, grouped by language, with copy / download-all / jump-to-turn. |
| 892 | [ByxHuster/DSH-Paper-Highlighting-Agent](https://github.com/ByxHuster/DSH-Paper-Highlighting-Agent) | 0 | 2026-08-27 | 2026-08-27 | An interactive and customized paper highlighting tool built upon Deepseek Harness (DSH), still under development. |
| 893 | [CagierAsh123/dsh-obsidian-agent-wiki](https://github.com/CagierAsh123/dsh-obsidian-agent-wiki) | 0 | 2026-08-26 | 2026-08-27 | Searchable SQLite-indexed Obsidian memory for DeepSeek Harness |
| 894 | [CAI-MH/dsh-feishu-task-recorder](https://github.com/CAI-MH/dsh-feishu-task-recorder) | 0 | 2026-09-04 | 2026-09-04 | Poll Feishu (Lark) chats, extract candidate tasks, two-way sync with the task-board plugin, with a floating browser panel — DeepSeek Harness bundle. 轮询飞书会话提取任务。 |
| 895 | [CAI-MH/dsh-quality-review](https://github.com/CAI-MH/dsh-quality-review) | 0 | 2026-09-04 | 2026-09-04 | AI response quality review for DeepSeek Harness: audits each finished assistant turn with an independent reviewer model and steers the agent to fix unreasonable output (up to 2 review rounds). |
| 896 | [CAI-MH/dsh-reply-language](https://github.com/CAI-MH/dsh-reply-language) | 0 | 2026-09-04 | 2026-09-04 | Force the DeepSeek Harness model to reply in a chosen language (default Simplified Chinese), switchable anytime via tools. 强制大模型使用指定语言回复。 |
| 897 | [Calvin451970353/dsh-vmic](https://github.com/Calvin451970353/dsh-vmic) | 0 | 2026-08-25 | 2026-08-27 | Voice input plugin for DeepSeek Harness: mic button, 16kHz WAV recording, ASR via Xiaomi MiMo / Volcengine Doubao (live), optional LLM polish. |
| 898 | [CanaryJing/dsh-big-fat-whale-maid-adaptive](https://github.com/CanaryJing/dsh-big-fat-whale-maid-adaptive) | 0 | 2026-08-23 | 2026-08-27 | 大肥鱼女仆长智能体，用风神与明神插件vibe而来，解决wsl与windows互通问题 |
| 899 | [Castem114/dsh-visioncraft](https://github.com/Castem114/dsh-visioncraft) | 0 | 2026-08-26 | 2026-08-27 | 为 DeepSeek Harness（DSH）Web 量身打造的双插件扩展，为纯文本模型补齐"视觉"短板 |
| 900 | [CatheadOwl/dsh-eval](https://github.com/CatheadOwl/dsh-eval) | 0 | 2026-09-04 | 2026-09-04 | Agent eval framework over dsh headless runs: case runner, session-trace assertions, and a scripted mock-LLM layer for plugin intent tests. |
| 901 | [CatheadOwl/dsh-extras](https://github.com/CatheadOwl/dsh-extras) | 0 | 2026-09-04 | 2026-09-04 | Out-of-tree plugin suite for deepseek-harness (dsh): markdown tooling, relates tables, review-evals dispatch. |
| 902 | [cayan0x/dsh-fold-context](https://github.com/cayan0x/dsh-fold-context) | 0 | 2026-08-28 | 2026-08-28 | Auto-fold context/system messages in DSH — collapse think blocks, tool calls, and tool results into grouped expandable bars. |
| 903 | [ccr-wer/dsh-dolphin-security](https://github.com/ccr-wer/dsh-dolphin-security) | 0 | 2026-09-01 | 2026-09-01 | 集扫描、远程执行、报告于一体的 DSH 主动安全巡逻插件，基于 SSH + Semgrep |
| 904 | [cczzyy-cn/dsh-ui-screenshot](https://github.com/cczzyy-cn/dsh-ui-screenshot) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness 的 Web 插件：在输入框添加截图按钮，截屏并作为草稿图片插入，仅当模型支持视觉时显示。 |
| 905 | [cczzyy-cn/subagent-model-picker](https://github.com/cczzyy-cn/subagent-model-picker) | 0 | 2026-09-02 | 2026-09-02 | DSH 插件：让主会话从「已配置模型」里自主选择子代理运行模型（list_subagent_models / subagent_model），并提供插件配置卡片为每个模型维护能力描述。 |
| 906 | [CDeZT/better-basicfun](https://github.com/CDeZT/better-basicfun) | 0 | 2026-09-01 | 2026-09-01 | Native DSH default workspace with complete paged read-only access to plugins, skills, memory, sessions, storage, settings, credentials, and DSH_HOME files. |
| 907 | [Centaurea5547196/dsh-page-zoom](https://github.com/Centaurea5547196/dsh-page-zoom) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness Web UI ??????:????? + Ctrl+??/Ctrl+=/-/0 ???,25%-300%,?????? |
| 908 | [ch3vr0n5/dsh-docker-services](https://github.com/ch3vr0n5/dsh-docker-services) | 0 | 2026-08-26 | 2026-08-27 | Portable DeepSeek Harness plugin for securely monitoring and operating Docker services |
| 909 | [chai1110/dsh-ssh-remote](https://github.com/chai1110/dsh-ssh-remote) | 0 | 2026-08-20 | 2026-09-01 | DeepSeek Harness SSH 远程工作区插件（多机并行）：同时连接多台服务器，Agent 直接查看/编辑/执行远程文件。基于 flymysql/dsh-remote (MIT) 适配 0.1.1-rc.2 |
| 910 | [changyinliangbaikai/dsh-b2us-schedule](https://github.com/changyinliangbaikai/dsh-b2us-schedule) | 0 | 2026-08-29 | 2026-08-30 | dsh定时任务插件，支持延迟、固定间隔、cron表达式，支持执行shell命令，支持发起Agent会话 |
| 911 | [Che-Year/dsh-pet-lulu](https://github.com/Che-Year/dsh-pet-lulu) | 0 | 2026-08-26 | 2026-08-27 | A cute terminal and web pet plugin for DeepSeek Harness (dsh), using assets from lulu and capybara projects. |
| 912 | [Cheeserackery/deepseek-time](https://github.com/Cheeserackery/deepseek-time) | 0 | 2026-08-18 | 2026-08-28 | 一款Agent插件，能够实时直观显示DeepSeek当前收费时段状态。DeepSeek pricing-period status indicator with Hermes, DSH, and Codex adapters. |
| 913 | [chemmy-11/dsh-nexus](https://github.com/chemmy-11/dsh-nexus) | 0 | 2026-08-24 | 2026-08-31 | Vault observation plugin for DeepSeek Harness: Obsidian vault metadata snapshot + edit stats + observation panel |
| 914 | [chen70456-lang/dsh-tmwebdriver](https://github.com/chen70456-lang/dsh-tmwebdriver) | 0 | 2026-08-30 | 2026-08-30 | One tool, infinite reach: arbitrary JS in your real logged-in browser. Unlike fixed-action plugins, browser_execute_js does anything DevTools can — read, click, type, fill, navigate, screenshot, CDP. Plus list_tabs/snapshot/type. Zero-setup, self-healing. |
| 915 | [chendefine/dsh-sidebar-onlyoffice](https://github.com/chendefine/dsh-sidebar-onlyoffice) | 0 | 2026-08-24 | 2026-08-27 | DSH web plugin: open and edit .docx/.xlsx/.pptx in the better-sidebar editor through a self-hosted ONLYOFFICE Document Server (JWT-signed config, atomic save-back, live refresh on AI edits) |
| 916 | [chendefine/dsh-sidebar-superdoc-docx](https://github.com/chendefine/dsh-sidebar-superdoc-docx) | 0 | 2026-09-01 | 2026-09-01 | DSH web plugin: open and edit .docx in the better-sidebar via SuperDoc — self-hosted, offline-capable, atomic saves |
| 917 | [chendefine/dsh-sidebar-vscode](https://github.com/chendefine/dsh-sidebar-vscode) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: a better-sidebar tab embedding the VS Code web workbench at the session workspace; editor selections and explorer files land as atomic reference chips |
| 918 | [chenyangcun/dsh-command-palette](https://github.com/chenyangcun/dsh-command-palette) | 0 | 2026-08-30 | 2026-08-30 | A keyboard-first command palette for standard DeepSeek Harness |
| 919 | [chenyangcun/dsh-fixed-new-session-model](https://github.com/chenyangcun/dsh-fixed-new-session-model) | 0 | 2026-08-30 | 2026-08-30 | 为 DSH 固定新会话的默认 Agent 预设与模型，支持全局默认设置和工作区独立配置。 |
| 920 | [Choco-Zz/dsh-image-amnesia](https://github.com/Choco-Zz/dsh-image-amnesia) | 0 | 2026-08-31 | 2026-08-31 | Drop historical images before DeepSeek Harness relay requests; keep native vision on the newest image. |
| 921 | [chocobo77/dsh-infinite-context](https://github.com/chocobo77/dsh-infinite-context) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: multi-tier memory management, semantic retrieval, structured memory, and model-context awareness for infinite context. |
| 922 | [chouyulanxia114514/dsh-uisketch](https://github.com/chouyulanxia114514/dsh-uisketch) | 0 | 2026-08-28 | 2026-08-28 | UI Sketch to AI 画板编辑器 × DSH 插件：侧栏开关 + 全屏 iframe 浮层，开箱即用 |
| 923 | [chris-003/dsh-agent-in-browser](https://github.com/chris-003/dsh-agent-in-browser) | 0 | 2026-08-31 | 2026-08-31 | Let a DeepSeek Harness agent see and control your browser in real time — read, screenshot, navigate, click, and manage tabs via tool calls. |
| 924 | [CHristianREEVEE/dsh-xiuxian-world](https://github.com/CHristianREEVEE/dsh-xiuxian-world) | 0 | 2026-08-28 | 2026-08-28 | 云仙大世界 — a living xiuxian world for DeepSeek Harness agents: enter, cultivate, and export a self-contained HTML replay of your journey |
| 925 | [chucan1/dsh-plugin-xt-memory](https://github.com/chucan1/dsh-plugin-xt-memory) | 0 | 2026-09-01 | 2026-09-02 | Cross-session self-learning memory for DeepSeek Harness, ported from XT-AGENT packages/memory. BM25 relevance injection + background extraction (sanitize/dedupe/merge) + lifecycle archive + memory_read/memory_search/memory_write tools. |
| 926 | [classic-takeoff/DSH_plugins](https://github.com/classic-takeoff/DSH_plugins) | 0 | 2026-08-31 | 2026-08-31 | some plugins for dsh |
| 927 | [cloveric/deepseek-harness-web-search-plugin](https://github.com/cloveric/deepseek-harness-web-search-plugin) | 0 | 2026-08-29 | 2026-08-29 | Source-traceable Brave + Tavily live web search and URL extraction for DeepSeek Harness. Native DSH plugin; TaroCub optional. |
| 928 | [CMD128/dsh-wx-bridge](https://github.com/CMD128/dsh-wx-bridge) | 0 | 2026-09-02 | 2026-09-02 | 微信桥接 DSH 插件：扫码绑定官方 ClawBot（iLink 协议），私聊驱动 DeepSeek Harness 会话 — WeChat bridge plugin for DSH |
| 929 | [cndn/dsh-d1](https://github.com/cndn/dsh-d1) | 0 | 2026-09-02 | 2026-09-02 | Cloudflare D1 tools for the DeepSeek Harness (dsh): read-only first, approval-gated writes, zero runtime dependencies |
| 930 | [CodeDice1024/dsh-log-viewer](https://github.com/CodeDice1024/dsh-log-viewer) | 0 | 2026-09-03 | 2026-09-03 | DSH 日志分析插件：Java 服务日志分析，AI 工具与 Web 仪表盘 |
| 931 | [CodeDice1024/dsh-plugin-dev-assistant](https://github.com/CodeDice1024/dsh-plugin-dev-assistant) | 0 | 2026-09-03 | 2026-09-03 | DSH 插件开发助手：对话式引导，从零开始创建、测试、发布 DSH 插件 |
| 932 | [cofy-x/dsh-evolver](https://github.com/cofy-x/dsh-evolver) | 0 | 2026-09-04 | 2026-09-04 | Auditable, verifier-gated self-evolution for DeepSeek Harness. |
| 933 | [Cooberped/dsh-evidence](https://github.com/Cooberped/dsh-evidence) | 0 | 2026-08-28 | 2026-08-28 | Turn local files into versioned evidence in DeepSeek Harness: composer upload, private local retrieval, and coordinate-exact PDF/DOCX/XLSX/PPTX reads. |
| 934 | [coolgech/dsh-siyuan](https://github.com/coolgech/dsh-siyuan) | 0 | 2026-08-27 | 2026-08-27 | A plugin for deepseek harnes that operates on the notes of Siyuan. |
| 935 | [csustyang/dsh-garmin-coach](https://github.com/csustyang/dsh-garmin-coach) | 0 | 2026-08-27 | 2026-08-31 | Garmin Connect 运动健康 AI 教练插件 for DeepSeek Harness |
| 936 | [CyberFox-lab/dsh-rss](https://github.com/CyberFox-lab/dsh-rss) | 0 | 2026-08-30 | 2026-08-30 | RSS/Atom reader and Agent tools plugin for DeepSeek Harness |
| 937 | [cyjyyd/dsh-llm-xai-oauth](https://github.com/cyjyyd/dsh-llm-xai-oauth) | 0 | 2026-08-27 | 2026-08-27 | Native SuperGrok / X Premium OAuth provider for DeepSeek Harness. Reuses local grok-bridge tokens; no xAI API key. |
| 938 | [d3vmeh/dsh-context-budget](https://github.com/d3vmeh/dsh-context-budget) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: keep a local model's context at a size your GPU handles well (measured prefill speed, hard ceiling, early compaction) |
| 939 | [d4551/DeepTail](https://github.com/d4551/DeepTail) | 0 | 2026-09-01 | 2026-09-02 | A Tauri 2 client — desktop, iOS, and Android — that connects to DeepSeek Harness hosts and gives you one control plane over the agent sessions running on all of them. |
| 940 | [daixin315/dsh-xiaoshuang](https://github.com/daixin315/dsh-xiaoshuang) | 0 | 2026-09-04 | 2026-09-04 | 小双 for DeepSeek Harness — 六层记忆人格插件 + 浮动视频形象（跟随 agent 状态表演 + TTS） |
| 941 | [Danreelkow/HDCS](https://github.com/Danreelkow/HDCS) | 0 | 2026-09-02 | 2026-09-03 | LLM loop that reasons in a dense technical register — mechanical gates + adversarial judge + reverse-translation for humans. Self-upgrading. Standalone or as a DSH plugin. |
| 942 | [daveycodez/dsh-llm-agent-bridge](https://github.com/daveycodez/dsh-llm-agent-bridge) | 0 | 2026-08-26 | 2026-08-27 | Claude as a selectable LLM provider in DeepSeek Harness, via Anthropic's official Claude Agent SDK. Works in any DSH mode. |
| 943 | [david0702/dsh-cost](https://github.com/david0702/dsh-cost) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) 对话底部费用显示插件：按每笔请求时间+模型分批计费，分时段明细，模型归属，读图金额，余额。 |
| 944 | [davidalmeida90/finance-agent-kit](https://github.com/davidalmeida90/finance-agent-kit) | 0 | 2026-09-04 | 2026-09-04 | Equity valuation skills and data MCPs for DeepSeek Harness and Claude Code. SEC filings, bottom-up sector beta, sourced implied ERP. |
| 945 | [Dayi-Z/gitcompass](https://github.com/Dayi-Z/gitcompass) | 0 | 2026-08-28 | 2026-08-29 | GitHub-connected visual git panel for DeepSeek Harness - branch switcher, file-level approval cards, PR/issue workspace |
| 946 | [Dee3526/dsh-plugin-trtc-conai](https://github.com/Dee3526/dsh-plugin-trtc-conai) | 0 | 2026-08-31 | 2026-08-31 | Tencent RTC Conversational AI (ConAI) voice agent tools for the DeepSeek Harness |
| 947 | [Dee3526/dsh-plugin-voice-input-demo](https://github.com/Dee3526/dsh-plugin-voice-input-demo) | 0 | 2026-09-03 | 2026-09-03 | Minimal Chinese voice input plugin for the DeepSeek Harness Web UI |
| 948 | [DeepseekHarnessPlugins/Notification](https://github.com/DeepseekHarnessPlugins/Notification) | 0 | 2026-08-26 | 2026-08-27 | DeepseekHarnessPlugin |
| 949 | [delicious28/wuming-books-mcp](https://github.com/delicious28/wuming-books-mcp) | 0 | 2026-08-28 | 2026-08-31 | Free remote MCP server for searching 680K+ Chinese books with Douban ratings, AI reading guides and curated toplists. No API key. |
| 950 | [demacia1314/dsh-remote-deliver](https://github.com/demacia1314/dsh-remote-deliver) | 0 | 2026-08-27 | 2026-08-27 | 🚀 告别繁琐 SCP！远程部署 DSH 一键下载修改后的文件与图片预览交付插件 |
| 951 | [Demigod-cyber/dsh-angelina-theme](https://github.com/Demigod-cyber/dsh-angelina-theme) | 0 | 2026-08-26 | 2026-08-27 | DSH主题插件——直到大地变成一颗酸橙（Angelina 浅蓝主题） |
| 952 | [dengyier/openworkproof-dsh-plugin](https://github.com/dengyier/openworkproof-dsh-plugin) | 0 | 2026-08-30 | 2026-08-30 | Community DeepSeek Harness plugin for verifiable AI agent authorization, execution evidence, and offline delivery verification |
| 953 | [dennisrongo/dsh-plugins](https://github.com/dennisrongo/dsh-plugins) | 0 | 2026-08-23 | 2026-08-27 | Dennis Rongo's plugin collection for DeepSeek Harness (dsh)  |
| 954 | [DepressionL/fortune-assistant](https://github.com/DepressionL/fortune-assistant) | 0 | 2026-08-28 | 2026-08-30 | dsh算命插件 |
| 955 | [dfhxxc666/dsh-llm-mimo](https://github.com/dfhxxc666/dsh-llm-mimo) | 0 | 2026-08-27 | 2026-08-27 | Xiaomi MiMo v2.5 adapter for DeepSeek Harness — fixed fork (sanitize tool args, dsh-llm 0.1.1-rc.2, prepareCall, keepalive) |
| 956 | [difimim/dsh-voice-input](https://github.com/difimim/dsh-voice-input) | 0 | 2026-08-29 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 957 | [dingxin-tech/dsh-maxcompute](https://github.com/dingxin-tech/dsh-maxcompute) | 0 | 2026-08-31 | 2026-08-31 | DSH (DeepSeek Harness) plugin for MaxCompute (ODPS): metadata browsing, cost-gated SQL execution, background jobs and result export. |
| 958 | [DobyChao/dsh-workspace-enhancement](https://github.com/DobyChao/dsh-workspace-enhancement) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness plugin: local and remote (SSH) workspaces in one place. Remote execution uses a single SSH connection (multi-hop jumps allowed); bash, files, PTY, and LSP share that link. |
| 959 | [doer1296/dsh-plugin-voice](https://github.com/doer1296/dsh-plugin-voice) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 语音插件：火山 seed-tts 云端 TTS（自动回退 SAPI/Huihui 离线）+ 桌面通知 + 场景化 WAV 提示音 + 提问自动呼叫。DSH 原生集成，零 Python 依赖，Windows 原生。 |
| 960 | [dondai44423/donsetch-dsh](https://github.com/dondai44423/donsetch-dsh) | 0 | 2026-09-03 | 2026-09-04 | First-class DonSeTch plugin for DeepSeek Harness: fetch, search and crawl as native dsh tools with an auto-updating verified binary |
| 961 | [Dongfang81/dsh-oil-account](https://github.com/Dongfang81/dsh-oil-account) | 0 | 2026-09-04 | 2026-09-04 | A film-ready oil car vs EV ownership cost demo for DSH Better Sidebar. |
| 962 | [dongsheng123132/dsh-break-glass-settlement-proof](https://github.com/dongsheng123132/dsh-break-glass-settlement-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed DSH proof for break-glass session settlement evidence |
| 963 | [dongsheng123132/dsh-change-window-proof](https://github.com/dongsheng123132/dsh-change-window-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed DSH proof for change-window settlement evidence |
| 964 | [dongsheng123132/dsh-credential-retirement-proof](https://github.com/dongsheng123132/dsh-credential-retirement-proof) | 0 | 2026-08-26 | 2026-08-27 | Evidence-only DSH plugin for credential retirement settlement |
| 965 | [dongsheng123132/dsh-duty-separation-proof](https://github.com/dongsheng123132/dsh-duty-separation-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed duty-separation evidence for supplied DSH workflow receipts |
| 966 | [dongsheng123132/dsh-license-obligation-proof](https://github.com/dongsheng123132/dsh-license-obligation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for license obligation delivery closure |
| 967 | [dongsheng123132/dsh-vulnerability-remediation-proof](https://github.com/dongsheng123132/dsh-vulnerability-remediation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for vulnerability remediation closure |
| 968 | [donoteatme/dsh-local-link](https://github.com/donoteatme/dsh-local-link) | 0 | 2026-08-27 | 2026-08-28 | Lightweight DeepSeek Harness plugin for paired LAN access: scan a QR code and continue the current DSH Web session from any phone, tablet, or computer. |
| 969 | [Doozqoo/dsh-pixel-office](https://github.com/Doozqoo/dsh-pixel-office) | 0 | 2026-08-27 | 2026-09-01 |  DeepSeek Harness Web GUI |
| 970 | [DoshinJiu/dsh-ui-boost](https://github.com/DoshinJiu/dsh-ui-boost) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness界面调色插件/RGB滑块调色 |
| 971 | [dsh-plugins/dsh-plugin-market](https://github.com/dsh-plugins/dsh-plugin-market) | 0 | 2026-08-26 | 2026-08-27 | A structured plugin marketplace for DeepSeek Harness — each plugin described as JSON, auto-aggregated into a single plugins.json for the dsh-plugins.github.io site. DeepSeek Harness 结构化插件市场 —— 每个插件以 JSON 描述，自动聚合为单一 plugins.json 供 dsh-plugins.github.io 站点消费。 |
| 972 | [du-u-uck/DSH-Transparent-UI-Plugin](https://github.com/du-u-uck/DSH-Transparent-UI-Plugin) | 0 | 2026-09-01 | 2026-09-02 | DeepSeek Harness UI Aqua玻璃质感主题主题，在原作者基础上对DSH新版本进行适配 |
| 973 | [dusbin/dsh-attention](https://github.com/dusbin/dsh-attention) | 0 | 2026-08-30 | 2026-08-30 | 任务完成后进行提醒，发完任务就可以去喝杯咖啡了，完成了会叫你的 |
| 974 | [dusbin/voice-plugin](https://github.com/dusbin/voice-plugin) | 0 | 2026-08-27 | 2026-08-27 | Dsh(deepseek harness)语音输入插件 Ps: 朗读功能目前还不是很棒。 |
| 975 | [dxsdyhm/dsh-adb-logcat](https://github.com/dxsdyhm/dsh-adb-logcat) | 0 | 2026-08-26 | 2026-08-27 | Android Studio-style ADB logcat viewer for the DSH Web GUI |
| 976 | [dy395769511-star/dsh-pdf-to-word](https://github.com/dy395769511-star/dsh-pdf-to-word) | 0 | 2026-08-29 | 2026-08-29 | PDF to Word conversion plugin for DeepSeek Harness (dsh): PyMuPDF/PaddleOCR pipeline + LLM visual style verification |
| 977 | [dzf-code/dsh-paste-doc](https://github.com/dzf-code/dsh-paste-doc) | 0 | 2026-08-24 | 2026-09-01 | 粘贴长文本 |
| 978 | [EasyTZ/dsh-git](https://github.com/EasyTZ/dsh-git) | 0 | 2026-08-27 | 2026-08-27 | Git panel plugin for DeepSeek Harness (dsh) — visual staging, commits, push and branch switching in the sidebar |
| 979 | [EasyTZ/dsh-reveal-explorer](https://github.com/EasyTZ/dsh-reveal-explorer) | 0 | 2026-08-27 | 2026-08-27 | Reveal-in-file-manager plugin for DeepSeek Harness (dsh) — open the current workspace in your system file manager |
| 980 | [EasyTZ/dsh-terminal-panel](https://github.com/EasyTZ/dsh-terminal-panel) | 0 | 2026-08-27 | 2026-08-27 | Terminal panel plugin for DeepSeek Harness (dsh) — run commands in the current workspace with streaming output |
| 981 | [EasyTZ/dsh-ui-balance](https://github.com/EasyTZ/dsh-ui-balance) | 0 | 2026-08-27 | 2026-08-27 | Balance display plugin for DeepSeek Harness (dsh) — show your DeepSeek API balance under each reply |
| 982 | [EChan684/dsh-web-verify-panel](https://github.com/EChan684/dsh-web-verify-panel) | 0 | 2026-09-03 | 2026-09-03 | 让 agent 的网页打开请求在 DSH 侧边栏内完成，不用弹出系统浏览器窗口 |
| 983 | [Edge-HH/GrokBot_in_DeepseekHerness](https://github.com/Edge-HH/GrokBot_in_DeepseekHerness) | 0 | 2026-08-22 | 2026-09-03 | 将GrokBot宠物代入DSH网页端并加入拖拽效果和通知功能 |
| 984 | [eehcx/dsh-gentle-engram](https://github.com/eehcx/dsh-gentle-engram) | 0 | 2026-08-26 | 2026-08-27 | DSH adapter for Engram — persistent memory bridge built with Cordis. |
| 985 | [elliseang0000-lang/dsh-pentest-bugtrace](https://github.com/elliseang0000-lang/dsh-pentest-bugtrace) | 0 | 2026-09-01 | 2026-09-01 | BugTraceAI penetration-testing mode for deepseek-harness (dsh): pentester persona, runbook skill, and MCP bridge in one installable bundle |
| 986 | [EmptyCollin/dsh-peak-valley-queue](https://github.com/EmptyCollin/dsh-peak-valley-queue) | 0 | 2026-08-27 | 2026-08-27 | Peak/valley pricing task queue for DeepSeek Harness |
| 987 | [erdholion/dsh-loop-guard](https://github.com/erdholion/dsh-loop-guard) | 0 | 2026-08-31 | 2026-09-01 | Result-aware stuck-loop guard for DeepSeek Harness: advisory nudges plus a monotonic hard stop. Only repeats with identical results count. |
| 988 | [Erick0412-dev/dsh-agy-ui](https://github.com/Erick0412-dev/dsh-agy-ui) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness Antigravity UI & Experience Enhancement Companion Plugin |
| 989 | [EsonXie/dsh-agent-toolkit](https://github.com/EsonXie/dsh-agent-toolkit) | 0 | 2026-08-19 | 2026-09-01 | Deepseek Harness工具集 |
| 990 | [evanfang0054/dsh-init](https://github.com/evanfang0054/dsh-init) | 0 | 2026-09-01 | 2026-09-01 | Claude Code style /init command for DeepSeek Harness (DSH): generates CLAUDE.md and symlinks AGENTS.md to it |
| 991 | [evlon/deepseek-harness-launcher](https://github.com/evlon/deepseek-harness-launcher) | 0 | 2026-08-28 | 2026-08-29 | 托盘常驻的 DeepSeek Harness 安装 / 启动器（Tauri 2 无窗口应用，仅系统托盘 + 原生通知 + 日志文件） |
| 992 | [evlon/dsh-codebuddy-models](https://github.com/evlon/dsh-codebuddy-models) | 0 | 2026-08-26 | 2026-08-29 | 把本机已登录的 CodeBuddy / WorkBuddy（腾讯代码助手） 订阅作为 dsh（DeepSeek Harness） 的原生 provider 接入，启用后 CodeBuddy 模型会直接出现在 dsh 的模型选择器中，可像其它模型一样被 agent 调用。 |
| 993 | [evlon/dsh-matrix-agent](https://github.com/evlon/dsh-matrix-agent) | 0 | 2026-08-27 | 2026-08-29 | DeepSeek Harness（dsh）的 Matrix agent 桥接插件：把 Matrix 房间桥接到 harness agent 会话，每个房间一个会话，支持在聊天里远程监控、审批和追加指令；多分身架构 + 媒体/富文本/回复/编辑信息完整处理。 |
| 994 | [ewceniza9009/wilsonix-studio](https://github.com/ewceniza9009/wilsonix-studio) | 0 | 2026-09-01 | 2026-09-02 | AI-powered desktop DAW - stem separation, chord detection, karaoke |
| 995 | [Exaggarate/dshpkg](https://github.com/Exaggarate/dshpkg) | 0 | 2026-09-02 | 2026-09-02 | Security & health audit CLI for DeepSeek Harness (DSH) plugins — npm audit for the everything-is-a-plugin era. Search, info, security-scan, doctor. stdlib-only. |
| 996 | [Exception-H/dsh-gpt56-ptc](https://github.com/Exception-H/dsh-gpt56-ptc) | 0 | 2026-08-30 | 2026-08-30 | Native DSH Bundle: user-owned pure PTC / Code Mode preset for GPT-5.6 with plain-language answers and bounded execution. |
| 997 | [F1star/dsh-research](https://github.com/F1star/dsh-research) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness bundle for evidence-first PDF reading, durable paper records, and cross-paper synthesis. |
| 998 | [FADE-4869/dsh-gacha-viz](https://github.com/FADE-4869/dsh-gacha-viz) | 0 | 2026-08-26 | 2026-08-27 | Genshin Impact gacha history visualizer and pity probability calculator for DeepSeek Harness (DSH plugin) |
| 999 | [fan56/dsh-ask-router](https://github.com/fan56/dsh-ask-router) | 0 | 2026-08-25 | 2026-08-29 | dsh plugin: multi-surface ask-user routing, first answer wins |
| 1000 | [fan56/dsh-cron](https://github.com/fan56/dsh-cron) | 0 | 2026-08-31 | 2026-09-02 | Cron scheduling for the DeepSeek Harness — bounded tasks with calendar & interval rules, delivered to live agents |
| 1001 | [fan56/dsh-feishu](https://github.com/fan56/dsh-feishu) | 0 | 2026-08-23 | 2026-08-27 | dsh plugin: drive an existing dsh session from Feishu/Lark — outbound-only bot, /resume picker, run status card |
| 1002 | [fan56/dsh-mcp-adapter](https://github.com/fan56/dsh-mcp-adapter) | 0 | 2026-08-26 | 2026-08-29 | dsh plugin: fold mcp__* tool schemas into two meta-tools via prompt-side shim to save tokens |
| 1003 | [fan56/dsh-topics-memory](https://github.com/fan56/dsh-topics-memory) | 0 | 2026-08-31 | 2026-09-03 | dsh-plugin: OKF v0.2 topic memory for dsh - local-first git-tracked bundle, hot-path LLM-free injection, two-stage observer with background distill |
| 1004 | [fan56/dsh-vault](https://github.com/fan56/dsh-vault) | 0 | 2026-08-30 | 2026-09-01 | dsh-plugin: encrypted backup / restore / migration of the dsh home config through a private GitHub repo |
| 1005 | [fan56/dsh-web-search-anysearch](https://github.com/fan56/dsh-web-search-anysearch) | 0 | 2026-08-26 | 2026-08-29 | AnySearch web search provider plugin for DeepSeek Harness (dsh) — zero-config, out-of-the-box |
| 1006 | [fan56/dsh-web-search-tavily](https://github.com/fan56/dsh-web-search-tavily) | 0 | 2026-08-25 | 2026-08-29 | Tavily web search provider plugin for DeepSeek Harness (dsh) |
| 1007 | [fangzaozao/dsh-mcp-oauth-client](https://github.com/fangzaozao/dsh-mcp-oauth-client) | 0 | 2026-09-03 | 2026-09-03 | Universal MCP manager and client bridge for DeepSeek Harness (DSH) |
| 1008 | [fantasyce/dsh-typelens](https://github.com/fantasyce/dsh-typelens) | 0 | 2026-08-27 | 2026-08-28 | Automatic bounded type context and edit diagnostics for DeepSeek Harness |
| 1009 | [Fast-Editor/lynkr-dsh-plugin](https://github.com/Fast-Editor/lynkr-dsh-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness (dsh) plugin: registers Lynkr as a custom OpenAI-compatible provider |
| 1010 | [faye0526/dsh-backup-btn](https://github.com/faye0526/dsh-backup-btn) | 0 | 2026-08-26 | 2026-08-27 | DSH 一键备份按钮 - 浮动按钮备份 DSH 数据到 GitHub Gist |
| 1011 | [FeatureAgents/AgentsGitFlowController](https://github.com/FeatureAgents/AgentsGitFlowController) | 0 | 2026-08-17 | 2026-08-28 | Agents Client Level Git Flow Controller |
| 1012 | [february2015/dsh-subagent-codex-plus](https://github.com/february2015/dsh-subagent-codex-plus) | 0 | 2026-08-30 | 2026-09-03 | Codex true-gateway plugin for DeepSeek Harness (DSH): /codex-lock direct connection to a durable Codex session — queued/steered conversation, live output, durable binding + auto-reattach. Personal fork of @deepseek-ai/dsh-subagent-codex. |
| 1013 | [february2015/dsh-subagent-pi-plus](https://github.com/february2015/dsh-subagent-pi-plus) | 0 | 2026-09-03 | 2026-09-03 | Pi true-gateway plugin for DeepSeek Harness (DSH): /pi-lock direct connection to a durable Pi session — queued/steered conversation, live output, durable binding + auto-reattach. Personal fork of @deepseek-ai/dsh-subagent-codex. |
| 1014 | [felix-lj-ct/dsh-mcp-live-status](https://github.com/felix-lj-ct/dsh-mcp-live-status) | 0 | 2026-08-28 | 2026-08-28 | Adds a status pill to the DeepSeek Harness web composer tool row: how many configured MCP servers are actually reachable, plus per-server transport, tool count and failure reason on click. Surfaces what the settings page cannot — a server that mounted fine but never finished its MCP handshake. Read-only, no config needed. |
| 1015 | [fengb3/dsh-theme-macintosh](https://github.com/fengb3/dsh-theme-macintosh) | 0 | 2026-08-28 | 2026-09-04 | DSH 主题 · 经典麦金塔 Classic Macintosh(System 7 像素复古) |
| 1016 | [fenghua00/dsh-sound-effects](https://github.com/fenghua00/dsh-sound-effects) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness 音效提示插件：任务完成或权限请求时播放提示音，可更换音效。 |
| 1017 | [fentz26/dsh-goodjob](https://github.com/fentz26/dsh-goodjob) | 0 | 2026-08-26 | 2026-08-27 | Multi-agent operations workspace for DeepSeek Harness. |
| 1018 | [fentz26/dsh-next](https://github.com/fentz26/dsh-next) | 0 | 2026-08-26 | 2026-08-27 | Performance-oriented backend/runtime modernization layer for DeepSeek Harness. |
| 1019 | [firestige/wsr-dsh](https://github.com/firestige/wsr-dsh) | 0 | 2026-08-29 | 2026-08-29 | WSR integrations for DeepSeek Harness: Execution, Studio, and suite bundles. |
| 1020 | [firestige/wsr-execution](https://github.com/firestige/wsr-execution) | 0 | 2026-08-17 | 2026-08-30 | Host-neutral execution boundary for workflow-self-recursive: resolves one exact Workflow Package, binds an immutable Delivery Manifest, coordinates the Delivery, emits bounded OTLP observations. Install via dsh plugin add wsr-dsh-intake · 与宿主无关的 Agent 工作流执行边界：解析并校验确定的工作流包，绑定不可变交付清单，协调交付并发出有界观测。 |
| 1021 | [fishfromsky/dsh-march7th-skin](https://github.com/fishfromsky/dsh-march7th-skin) | 0 | 2026-08-20 | 2026-08-27 | 崩坏星穹铁道三月七主题的deepseek harness皮肤插件 |
| 1022 | [FishingTofu0120/Plugin-for-checking-API-balance](https://github.com/FishingTofu0120/Plugin-for-checking-API-balance) | 0 | 2026-09-01 | 2026-09-01 | A plugin for checking API-balance on DSH website conveniently |
| 1023 | [Flan246/dsh-latex-guard](https://github.com/Flan246/dsh-latex-guard) | 0 | 2026-08-26 | 2026-08-27 | LaTeX compile check and BibTeX lint/fill/audit tools for DeepSeek Harness and any agent. dsh plugin + CLI + SKILL.md. |
| 1024 | [flashyiyi/dsh-envelope-highlight](https://github.com/flashyiyi/dsh-envelope-highlight) | 0 | 2026-08-28 | 2026-08-28 | Restore syntax highlighting of read/write tool envelopes inside run_code (PTC / Code Mode) result cards |
| 1025 | [fly1989/dsh-deliberation](https://github.com/fly1989/dsh-deliberation) | 0 | 2026-08-20 | 2026-08-31 | Primary-controlled deliberation and opt-in reasoning-masked review for DeepSeek Harness. |
| 1026 | [flyingfishzxf/dsh-dsbal](https://github.com/flyingfishzxf/dsh-dsbal) | 0 | 2026-08-18 | 2026-08-27 | A simple DeepSeek API balance display plugin for dsh(deepseek-harness) |
| 1027 | [flymysql/dsh-browser-client](https://github.com/flymysql/dsh-browser-client) | 0 | 2026-08-23 | 2026-08-31 | DSH Browser Client — LLM 驱动的浏览器浮窗工作流工具（面向非研发人员的网页自动化） |
| 1028 | [force-push/dsh-llm-fallback](https://github.com/force-push/dsh-llm-fallback) | 0 | 2026-08-27 | 2026-08-27 | Self-healing cross-provider model fallback plugin for the DeepSeek Harness (DSH) — retries exhausted, re-bind the session to the next healthy model. |
| 1029 | [ForeverYoungPp/dsh-web-search](https://github.com/ForeverYoungPp/dsh-web-search) | 0 | 2026-09-01 | 2026-09-01 | dsh-web-search — Multi-provider web search for DeepSeek Harness: routes the native web_search tool through a configurable provider fallback chain (Tavily/Brave/Exa/Firecrawl/Jina/Kagi/SearXNG/DuckDuckGo), replacing the built-in deepseek-official backend, with a settings page for key management and ordering. Approach adapted from OMP.  |
| 1030 | [founder987/dsh-dev-ui](https://github.com/founder987/dsh-dev-ui) | 0 | 2026-08-25 | 2026-08-27 | 适合编码研发的UI界面 |
| 1031 | [FourTow/dsh-theme-win98](https://github.com/FourTow/dsh-theme-win98) | 0 | 2026-09-02 | 2026-09-03 | Windows 98 theme plugin for DeepSeek Harness web |
| 1032 | [FoyonaCZY/dsh-kit](https://github.com/FoyonaCZY/dsh-kit) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugins for the failures nobody catches: auto-format, generated-file guard, .env drift detection, and a typecheck gate that runs before the agent says it's done. Four gaps the 13k-plugin ecosystem hasn't filled. |
| 1033 | [Francesco502/dsh-quota](https://github.com/Francesco502/dsh-quota) | 0 | 2026-08-26 | 2026-08-27 | AI Quota and Token Usage Monitor for DeepSeek Harness (Codex, Cursor, Antigravity, OpenCode-Go) |
| 1034 | [Frank-NF/dsh-drop-md](https://github.com/Frank-NF/dsh-drop-md) | 0 | 2026-08-30 | 2026-08-30 | Drag-and-drop markdown enhancer for DeepSeek Harness (DSH): inline small files, @-reference large ones, one-click SKILL.md install |
| 1035 | [Frank-NF/dsh-memory-nexus](https://github.com/Frank-NF/dsh-memory-nexus) | 0 | 2026-09-01 | 2026-09-01 | DSH integrated memory and context management plugin: 4-layer memory, context compression, prompt orchestration, enterprise security |
| 1036 | [frank6892103/dsh-WutheringWaves](https://github.com/frank6892103/dsh-WutheringWaves) | 0 | 2026-08-30 | 2026-08-31 | dsh鸣潮主题插件 |
| 1037 | [freedomkk-qfeng/dsh-mail-assistant](https://github.com/freedomkk-qfeng/dsh-mail-assistant) | 0 | 2026-08-31 | 2026-08-31 | Standards-based IMAP/SMTP mail connector for DeepSeek Harness, enabling agents to read and send email with explicit user controls. |
| 1038 | [freedomkk-qfeng/dsh-oidc](https://github.com/freedomkk-qfeng/dsh-oidc) | 0 | 2026-08-30 | 2026-08-30 | Enterprise OIDC, secure API-key binding, declarative branding, and OpenAI-compatible model integration for DeepSeek Harness. |
| 1039 | [FriendsHL/dsh-agent-evolution](https://github.com/FriendsHL/dsh-agent-evolution) | 0 | 2026-08-26 | 2026-08-27 | Preset-composed Agent experiments and evolution primitives for DeepSeek Harness |
| 1040 | [fthuu/Tokan-dsh-token-analytics](https://github.com/fthuu/Tokan-dsh-token-analytics) | 0 | 2026-08-31 | 2026-08-31 | 精准 Token 洞察，实时追踪，智能优化提示和用量归因 Sharp token insights, real‑time tracking, smart optimization signals & attribution  |
| 1041 | [fufuf-c/dsh-token](https://github.com/fufuf-c/dsh-token) | 0 | 2026-08-30 | 2026-09-03 | DSH local token usage & cost dashboard: 4-segment token breakdown, cache savings, per-session drill-down, global filters, monthly budget. Zero upload. |
| 1042 | [funcodingdev/dsh-community-plugins](https://github.com/funcodingdev/dsh-community-plugins) | 0 | 2026-09-02 | 2026-09-04 | DeepSeek Harness 原生社区插件管理器：在设置中发现、安装、更新和管理社区插件。 |
| 1043 | [fuzz1og/dsh-model-capabilities](https://github.com/fuzz1og/dsh-model-capabilities) | 0 | 2026-09-04 | 2026-09-04 | DSH web plugin: per-model thinking-intensity tiers, modalities and gateway compat switches for custom llm-pi-ai providers, edited inside the official Models settings card |
| 1044 | [GavinQiEr/dsh-cmdwatch](https://github.com/GavinQiEr/dsh-cmdwatch) | 0 | 2026-08-30 | 2026-08-30 | Real-time command monitor for DeepSeek Harness (DSH). Watch foreground/background command output in the Web UI without pausing the conversation. 命令窗：实时显示 DSH 命令与执行输出。 |
| 1045 | [gbeta/dsh-stock-quote](https://github.com/gbeta/dsh-stock-quote) | 0 | 2026-09-03 | 2026-09-03 | DSH web plugin: collapsible draggable A-share quote widget (沪深300 + individual stocks, live price + change %) |
| 1046 | [gcry13067381632-jpg/dsh-qqbot](https://github.com/gcry13067381632-jpg/dsh-qqbot) | 0 | 2026-09-04 | 2026-09-04 | DSH接入腾讯官方qqbot/富媒体/表情包/多开不同预设的机器人/定时消息/远程审批 |
| 1047 | [geeklei/dsh-plugins](https://github.com/geeklei/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | 一个面向 DeepSeek Harness (dsh)的插件库 |
| 1048 | [geekyfoxlab/dsh-subagents](https://github.com/geekyfoxlab/dsh-subagents) | 0 | 2026-08-26 | 2026-08-27 | Focused child-agent delegation (scout, researcher, worker, reviewer, oracle, delegate) and multi-agent workflows (council, parallel review, review loop) for DeepSeek Harness. |
| 1049 | [ghbhiee/dsh-plugin-tui](https://github.com/ghbhiee/dsh-plugin-tui) | 0 | 2026-08-28 | 2026-08-28 | Claude Code-style terminal UI plugin for DeepSeek Harness (dsh): streaming REPL, collapsed thinking, interactive session/model pickers, history replay, approval modes, bottom status bar |
| 1050 | [Ghost011118/dsh-plugin-governor-extension](https://github.com/Ghost011118/dsh-plugin-governor-extension) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin governance: installable runtime tool policy plus companion boot admission, supervised restart, and rollback. |
| 1051 | [Ghost011118/dsh-plugin-marketplace](https://github.com/Ghost011118/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Built-in plugin discovery, local requirement matching, optional GitHub stars, and one-click installation for DeepSeek Harness. |
| 1052 | [GitNoHup/macaron-theme](https://github.com/GitNoHup/macaron-theme) | 0 | 2026-08-26 | 2026-08-27 | 🍬 马卡龙毛玻璃主题（Macaron Glassmorphism Theme）— DeepSeek Harness 动态主题插件：四套马卡龙配色、145° 双色渐变、毛玻璃卡片；日间上色 / 夜间自动清除并记忆恢复。 |
| 1053 | [gjjkbssg/dsh-model-jury](https://github.com/gjjkbssg/dsh-model-jury) | 0 | 2026-08-31 | 2026-08-31 | Structured cross-model peer review for DeepSeek Harness — blind reasoning, anonymous critique, revision, and deterministic verdicts. |
| 1054 | [Glazyonyt/dsh-lowtide](https://github.com/Glazyonyt/dsh-lowtide) | 0 | 2026-08-28 | 2026-08-28 | Queue AI tasks during off-peak hours to cut costs and automate runs with dsh-lowtide for DeepSeek Harness. |
| 1055 | [GoldenZqqq/dsh-model-collapse](https://github.com/GoldenZqqq/dsh-model-collapse) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin: collapse the model picker by provider, with a pinned quick bar (expand-all / collapse-all / focus-current / filter / reset). |
| 1056 | [goldgish/dsh-gamepad-approval](https://github.com/goldgish/dsh-gamepad-approval) | 0 | 2026-08-30 | 2026-08-30 | Xbox 手柄硬件审批插件 for DeepSeek Harness (dsh) — Agent 高危工具调用需物理按键确认，A 批准 / B 驳回 |
| 1057 | [gongyijie85/dsh-agent-frugality](https://github.com/gongyijie85/dsh-agent-frugality) | 0 | 2026-08-29 | 2026-09-02 | Multi-agent frugality defense plugin for DeepSeek Harness: read-ledger dedup, compaction-immune rules, completion gate, cheap-review lane. |
| 1058 | [GooDAnDReaDY/dsh-agent-loop-guard](https://github.com/GooDAnDReaDY/dsh-agent-loop-guard) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness runtime guard for tool-call and assistant-output loops |
| 1059 | [GooDAnDReaDY/dsh-context-lens](https://github.com/GooDAnDReaDY/dsh-context-lens) | 0 | 2026-08-31 | 2026-09-01 | DSH plugin for AST context compression, test log filtering, and token budget guard |
| 1060 | [GooDAnDReaDY/dsh-dsml-artifact-guard](https://github.com/GooDAnDReaDY/dsh-dsml-artifact-guard) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness DSML artifact sanitizer for leaked protocol tags |
| 1061 | [GooDAnDReaDY/dsh-gitea](https://github.com/GooDAnDReaDY/dsh-gitea) | 0 | 2026-08-31 | 2026-08-31 | Gitea/Forgejo toolkit for DeepSeek Harness: issues, PRs, CI, releases, operations |
| 1062 | [GooDAnDReaDY/dsh-kanban](https://github.com/GooDAnDReaDY/dsh-kanban) | 0 | 2026-08-27 | 2026-09-01 | Kanban board for DeepSeek Harness: Gitea-backed tasks, workflow columns, and dedicated agent sessions |
| 1063 | [GooDAnDReaDY/dsh-live-canvas](https://github.com/GooDAnDReaDY/dsh-live-canvas) | 0 | 2026-08-31 | 2026-08-31 | Interactive in-browser canvas for real-time preview of HTML, React components, SVGs, and diagrams with SSE hot-reload in DeepSeek Harness |
| 1064 | [GooDAnDReaDY/dsh-moa](https://github.com/GooDAnDReaDY/dsh-moa) | 0 | 2026-09-04 | 2026-09-04 | Mixture of Agents (MoA) plugin for DeepSeek Harness with /moa slash command, file workspaces, and Live Canvas integration |
| 1065 | [GooDAnDReaDY/dsh-shadow-auditor](https://github.com/GooDAnDReaDY/dsh-shadow-auditor) | 0 | 2026-09-02 | 2026-09-03 | DSH plugin for background security audits, secret leakage detection, and command safety |
| 1066 | [GooDAnDReaDY/dsh-time-machine](https://github.com/GooDAnDReaDY/dsh-time-machine) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin for smart checkpoints, workspace safety guards, and instant rollback |
| 1067 | [Gorilla-Kevv/scnu-thesis-formatter](https://github.com/Gorilla-Kevv/scnu-thesis-formatter) | 0 | 2026-08-30 | 2026-08-30 | 华南师范大学本科毕业论文格式改写 + matplotlib 数据可视化（DeepSeek Harness 技能） |
| 1068 | [GoshawkGGGG/dsh-safe-tool](https://github.com/GoshawkGGGG/dsh-safe-tool) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness 的 AI 工具审批插件，使用AI审核AGENT调用工具的合规性并决定是否执行，审核标准可定制。 |
| 1069 | [GreenLv/dsh-completion-guard](https://github.com/GreenLv/dsh-completion-guard) | 0 | 2026-08-26 | 2026-08-29 | Task-contract and completion-certification layer for DeepSeek Harness |
| 1070 | [grstein/dsh-locale-ptbr](https://github.com/grstein/dsh-locale-ptbr) | 0 | 2026-08-31 | 2026-08-31 | Pacote de idioma Português (Brasil) para a GUI Web do DeepSeek Harness |
| 1071 | [gsh150801/dsh-bioinf](https://github.com/gsh150801/dsh-bioinf) | 0 | 2026-09-01 | 2026-09-01 | Bioinformatics plugin for DeepSeek Harness (dsh) |
| 1072 | [gsh150801/dsh-bioinf-routed](https://github.com/gsh150801/dsh-bioinf-routed) | 0 | 2026-09-01 | 2026-09-01 | Bioinformatics plugin for DeepSeek Harness (dsh) |
| 1073 | [gsh150801/dsh-bioinf-verify](https://github.com/gsh150801/dsh-bioinf-verify) | 0 | 2026-09-01 | 2026-09-01 | Bioinformatics plugin for DeepSeek Harness (dsh) |
| 1074 | [gtaifu/dsh-title-index](https://github.com/gtaifu/dsh-title-index) | 0 | 2026-09-01 | 2026-09-01 | Disk-indexed session title lookups for the DeepSeek Harness web GUI — @-mention candidates ~30× faster. |
| 1075 | [guangxiangwu6-cmd/dsh-llm-failover](https://github.com/guangxiangwu6-cmd/dsh-llm-failover) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness model auto-failover plugin: retry threshold -> mark unavailable -> seamless switch to next healthy model -> cooldown auto-recover. 18-model pool, 19/19 tests, boot-safe. |
| 1076 | [guazixiong/dsh-coding-mode-preset](https://github.com/guazixiong/dsh-coding-mode-preset) | 0 | 2026-08-30 | 2026-08-30 | 为本地 DeepSeek Harness（`@deepseek-ai/dsh`）追加一个**编码模式** Agent Preset：门禁式工程交付流水线，包含三条独立流程——**需求开发**、**Bug 修复**、**功能迭代**。每个阶段的产物由全新上下文的"空白子代理"独立专家评审，通过后须经用户确认才进入下一阶段；最终以用户验收作为任务完结条件。 |
| 1077 | [gunduziba/dsh-pi-markdown](https://github.com/gunduziba/dsh-pi-markdown) | 0 | 2026-09-04 | 2026-09-04 | Pi TUI 终端风格 Markdown 样式插件，专为 DeepSeek Harness Web 设计 |
| 1078 | [gunduziba/dsh-tool-zg](https://github.com/gunduziba/dsh-tool-zg) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness 原生 zvec-grep (zg) 代码语义搜索工具插件，支持按预设动态过滤 |
| 1079 | [GuoxinShan/dsh-yzj](https://github.com/GuoxinShan/dsh-yzj) | 0 | 2026-08-14 | 2026-08-27 | 云之家 (Yunzhijia) plugin bundle for DeepSeek Harness: yzj-cli bridge, 41 model-facing tools, floating workspace panel with drag/@ reference chips |
| 1080 | [Hanmingh/dsh-desktop](https://github.com/Hanmingh/dsh-desktop) | 0 | 2026-08-27 | 2026-08-27 | Desktop Plugin for Deepseek Harness |
| 1081 | [hansjone/netxops](https://github.com/hansjone/netxops) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness Netx Ops agent preset (UME alarms, NE, managed CLI) |
| 1082 | [haohaiHuang/Design-Agent](https://github.com/haohaiHuang/Design-Agent) | 0 | 2026-08-27 | 2026-08-27 | DSH 设计 Agent 完整可复现包：design-references 路由技能（DSH 适配）+ design-router 确定性工具插件 + my-agent 预设 |
| 1083 | [HaoR325/dsh-usage-daily](https://github.com/HaoR325/dsh-usage-daily) | 0 | 2026-08-30 | 2026-08-31 | DSH 用量日报浮窗插件：今日令牌/消息/轮数/估算费用 |
| 1084 | [haoyu-qi/dsh-zentao](https://github.com/haoyu-qi/dsh-zentao) | 0 | 2026-08-15 | 2026-08-27 | 面向 DeepSeek Harness 的 AVCON Web 界面定制与个人禅道 CLI 工作中心 |
| 1085 | [haozheou/dsh-exam-expert](https://github.com/haozheou/dsh-exam-expert) | 0 | 2026-08-30 | 2026-08-30 | 出题专家 · Exam Expert plugin for DeepSeek Harness: 把出题流程固化成值守流水线（角色+目录→通读→勾选表单→六分身流水线→看板交付） \| Turn the exam-paper workflow into an agent-supervised pipeline: wizard dialog, prefilled checklist form, six-role dual-kanban production |
| 1086 | [harness-home/harness-ai-plugins](https://github.com/harness-home/harness-ai-plugins) | 0 | 2026-08-26 | 2026-08-27 | Community plugin catalog for Harness AI: a scanner over the public npm registry, and the snapshot it publishes. |
| 1087 | [Harzva/dsh-restart-autoresume](https://github.com/Harzva/dsh-restart-autoresume) | 0 | 2026-08-29 | 2026-08-29 | Safe DSH restart coordination and durable top-level session autoresume |
| 1088 | [haythamat/dsh-client-ui-rtl](https://github.com/haythamat/dsh-client-ui-rtl) | 0 | 2026-08-27 | 2026-08-27 | Right-to-left text direction for the DeepSeek Harness Web client |
| 1089 | [hcyinnn/dsh-tool-ssh](https://github.com/hcyinnn/dsh-tool-ssh) | 0 | 2026-09-01 | 2026-09-01 | SSH tools plugin for DeepSeek Harness (dsh): run remote commands and transfer files via OpenSSH. dsh 插件——让 Agent 通过 SSH 在远程主机执行命令、上传/下载文件。 |
| 1090 | [heartmove/dsh-session-bridge](https://github.com/heartmove/dsh-session-bridge) | 0 | 2026-09-01 | 2026-09-01 |  DSH 插件，让当前代理直接从提示词驱动其它真实 DSH 会话——创建/发送/等待回复/读取/恢复/跨工作区查找会话，并支持监控调度主任务与归档会话。A DSH plugin that lets the agent drive other real DSH sessions straight from a prompt — create, send, wait, read, resume, and find sessions across workspaces, plus monitor/schedule a main task and archive sessions. |
| 1091 | [hedging8563/tokenlab-deepseek-harness-provider](https://github.com/hedging8563/tokenlab-deepseek-harness-provider) | 0 | 2026-08-27 | 2026-08-27 | TokenLab native-protocol model provider, multimodal tools, and async tasks for DeepSeek Harness |
| 1092 | [hehehe1234567894/dsh-ssh-remote](https://github.com/hehehe1234567894/dsh-ssh-remote) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness (DSH) SSH 远程工作插件 — 纯远程模式：多机管理、工作区选择、远程文件读写工具 |
| 1093 | [hehetoshang/dsh-talebook-plugin](https://github.com/hehetoshang/dsh-talebook-plugin) | 0 | 2026-08-27 | 2026-08-30 | DeepSeek Harness plugin for safely operating Talebook |
| 1094 | [helibeiqi/dsh-cdp-metadata](https://github.com/helibeiqi/dsh-cdp-metadata) | 0 | 2026-08-23 | 2026-08-28 | Capability Description Protocol (CDP) v0.1 — read-only AI-readable capability metadata layer for DSH Cordis plugins. |
| 1095 | [helibeiqi/dsh-cn-disclosure](https://github.com/helibeiqi/dsh-cn-disclosure) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 公告/年报 结构化抽取 MCP server (dsh-plugin) |
| 1096 | [helibeiqi/dsh-context-aware-search](https://github.com/helibeiqi/dsh-context-aware-search) | 0 | 2026-08-19 | 2026-08-28 | Context-aware web search plugin for DeepSeek Harness (dsh): rewrites queries with session context, reranks + credibility-tags results, one-click source summarization across multiple backends. Fully decoupled from @deepseek-ai private packages for public CI. |
| 1097 | [helibeiqi/dsh-dcs-engine](https://github.com/helibeiqi/dsh-dcs-engine) | 0 | 2026-08-24 | 2026-08-28 | Dynamic Capability Synthesis Engine — DSH protocol stack credit engine |
| 1098 | [helibeiqi/dsh-docx-mcp](https://github.com/helibeiqi/dsh-docx-mcp) | 0 | 2026-08-28 | 2026-08-28 | Zero-dependency MCP stdio server that generates real .docx files from a JSON spec — Chinese office-automation vertical for DeepSeek Harness. |
| 1099 | [helibeiqi/dsh-hr-payroll-mcp](https://github.com/helibeiqi/dsh-hr-payroll-mcp) | 0 | 2026-08-29 | 2026-08-29 | 通用 HR 算薪 MCP 服务：本地化法定社保/公积金/个税计算 + 通用表头适配 + 企业配置 + 安全绩效公式（PII 不出机） |
| 1100 | [helibeiqi/dsh-industry-graph-mcp](https://github.com/helibeiqi/dsh-industry-graph-mcp) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 产业链/申万行业/概念板块 知识图谱 MCP server (dsh-plugin) |
| 1101 | [helibeiqi/dsh-memory-projection](https://github.com/helibeiqi/dsh-memory-projection) | 0 | 2026-08-20 | 2026-08-28 | Hot-pluggable memory-projection scheduling framework for DeepSeek Harness (dsh): pure-function projection strategies + a runtime invariant guard, built on the cordis plugin kernel. |
| 1102 | [helibeiqi/dsh-quant-factor-pipeline](https://github.com/helibeiqi/dsh-quant-factor-pipeline) | 0 | 2026-08-28 | 2026-08-28 | Quant factor research pipeline as a dsh user-layer MCP server (CGO disposal-effect factor, RankIC, Newey-West t, regime-aware) |
| 1103 | [hellofuture2068/dsh-simple-view](https://github.com/hellofuture2068/dsh-simple-view) | 0 | 2026-08-26 | 2026-08-27 | Declutter DeepSeek Harness chat: hide agent execution-log rows, tighten spacing & fonts, bubble messages, and set a "reply concisely" system-prompt instruction. |
| 1104 | [hellogit2021/avoid-ai-writing-cn](https://github.com/hellogit2021/avoid-ai-writing-cn) | 0 | 2026-08-29 | 2026-08-29 | 知乎"去AI味写作技巧"社区免费提供：中文写作去 AI 味插件（AI-isms / AI writing / humanize）。说"去掉AI味"即重写，说"写的不错"自动学习新 AI 词。安装：dsh plugin --profile web add github:hellogit2021/avoid-ai-writing-cn |
| 1105 | [helloworld1631/dsh-volcengine-usage](https://github.com/helloworld1631/dsh-volcengine-usage) | 0 | 2026-08-27 | 2026-08-27 | Draggable Volcengine Coding Plan usage monitor for DeepSeek Harness Web. |
| 1106 | [hfyydd/dsh-cua](https://github.com/hfyydd/dsh-cua) | 0 | 2026-08-28 | 2026-08-28 | Computer Use for DeepSeek Harness, backed by the cua-driver daemon (trycua): UIA element-level targeting, background-first input delivery, deterministic verification. |
| 1107 | [hhb1028/dsh-client-ui-timeline](https://github.com/hhb1028/dsh-client-ui-timeline) | 0 | 2026-08-30 | 2026-08-30 | DSH Web GUI 会话问题导航条：聊天区左缘一问一杠，随滚动高亮当前问题、悬停显示问答预览气泡、点击把该问平滑滚到视口顶（未渲染的更早历史自动翻页加载），无需改动 dsh 本体源码 |
| 1108 | [higekibaka/dsh-ciel](https://github.com/higekibaka/dsh-ciel) | 0 | 2026-08-31 | 2026-08-31 | 夏尔 Ciel — a pre-planning advisor and convergent critic for DeepSeek Harness: a second, knowledge-rich model offering directions, prior art, pitfalls and verification checklists (ideas, never steps). |
| 1109 | [HiSeax/dsh-agent-outputs-reader](https://github.com/HiSeax/dsh-agent-outputs-reader) | 0 | 2026-08-29 | 2026-08-30 | Overlay reader for agent output files: Markdown/GFM rendering, in-panel PDF, DOCX/XLSX/PPTX text preview, reply-end file chips. Pure JS, zero deps. |
| 1110 | [HiSeax/dsh-better-model-setting](https://github.com/HiSeax/dsh-better-model-setting) | 0 | 2026-08-23 | 2026-08-29 | DSH plugin: replaces official Models settings page with provider management, per-model reasoning effort, retry overrides, drag reorder, add official DeepSeek, credential status |
| 1111 | [hmlyx/dsh-memory](https://github.com/hmlyx/dsh-memory) | 0 | 2026-08-29 | 2026-08-29 | 简单的插件，让你的每个 AI 记录经验和记忆 |
| 1112 | [hmlyx/dsh-notify](https://github.com/hmlyx/dsh-notify) | 0 | 2026-08-29 | 2026-08-29 | 在输入框右边加了一个泡泡窗口，你可以接入插件或者告诉 AI 什么时候使用它。 |
| 1113 | [hongbaiqi/dsh-model-account-login](https://github.com/hongbaiqi/dsh-model-account-login) | 0 | 2026-09-03 | 2026-09-04 | Persistent DSH model-account authorization UI for ChatGPT, Claude, and other llm-pi-ai login flows |
| 1114 | [honoriomelo/dsh-model-picker-search](https://github.com/honoriomelo/dsh-model-picker-search) | 0 | 2026-08-29 | 2026-08-29 | DSH Web GUI plugin: adds a live search field inside the model picker menu of the composer, plus the Effort (reasoning) selector. Drop-in replacement for the native model seat, sharing the same per-session ModelDirectory so /model popup, the effort selector, and the /model command stay consistent. |
| 1115 | [horizon105457/tsstream](https://github.com/horizon105457/tsstream) | 0 | 2026-08-26 | 2026-08-27 | 🌊 Agent-native time-series streaming for DeepSeek Harness (DSH plugin) — terminal/serial byte streams → indexed, queryable, event-driven timeline. 19 tools · 9 operators · 🧪 experimental |
| 1116 | [Hoshino-Yumetsuki/as-compatible-copilot](https://github.com/Hoshino-Yumetsuki/as-compatible-copilot) | 0 | 2026-08-01 | 2026-08-29 | A VSCode extension to use Openai/Anthropic/Gemini API Providers in GitHub Copilot Chat |
| 1117 | [hotpot-labs/dsh-notifier-plugin](https://github.com/hotpot-labs/dsh-notifier-plugin) | 0 | 2026-08-30 | 2026-09-02 | dsh 干完活之后通知你，【轻量级】通知插件，只通知，不交互，mac/windows/linux 操作系统支持，dsh 在干活时你可以摸鱼 |
| 1118 | [hotpot-labs/dsh-prompt-history-plugin](https://github.com/hotpot-labs/dsh-prompt-history-plugin) | 0 | 2026-09-01 | 2026-09-02 | dsh 输入框的提示词导航插件，支持上下键查看历史输入 |
| 1119 | [hotpot-labs/dsh-wooden-fish](https://github.com/hotpot-labs/dsh-wooden-fish) | 0 | 2026-09-03 | 2026-09-03 | dsh 木鱼，dsh 干活你敲木鱼，每天增加一点点功德 |
| 1120 | [hpyer/dsh-for-mac](https://github.com/hpyer/dsh-for-mac) | 0 | 2026-08-31 | 2026-08-31 | DshForMac 是 DeepSeek Harness 的原生 macOS 启动器与运行时管理器，提供本地环境检测、版本管理及内嵌 Web 界面。 |
| 1121 | [hrhgit/dsh-model-manager](https://github.com/hrhgit/dsh-model-manager) | 0 | 2026-08-14 | 2026-08-31 | Model tags, reasoning capabilities, image routing, and vision proxy support for DeepSeek Harness |
| 1122 | [HrxSpace/dsh-session-sweeper](https://github.com/HrxSpace/dsh-session-sweeper) | 0 | 2026-09-04 | 2026-09-04 | DSH 插件，扫描管理电脑本地所有终端的会话（Claude Code、Codex、Workbuddy、DSH等） |
| 1123 | [hu669293657/dsh-turn-tools](https://github.com/hu669293657/dsh-turn-tools) | 0 | 2026-08-29 | 2026-08-29 | DSH web plugin: per-turn deliverable buttons (open with the OS default app) and a turn-navigator dot rail for jumping between conversation turns. |
| 1124 | [huangDouP/dsh-client-ui-notifications](https://github.com/huangDouP/dsh-client-ui-notifications) | 0 | 2026-08-29 | 2026-08-29 | DSH Web notifications: browser notifications, tab title flash, favicon badge, and native Windows toasts with a bilingual (zh/en) settings page. |
| 1125 | [huangjua/dsh-evidence](https://github.com/huangjua/dsh-evidence) | 0 | 2026-09-01 | 2026-09-01 | 🛡️ Verifiable, tamper-proof audit evidence bundles and hash-chained receipts for DSH agents |
| 1126 | [huangjua/dsh-local-memory](https://github.com/huangjua/dsh-local-memory) | 0 | 2026-09-01 | 2026-09-01 | 🧠 Persistent cross-session local memory for DSH agents (Markdown SSOT + self-healing SQLite mirror) |
| 1127 | [huangjua/dsh-session-index](https://github.com/huangjua/dsh-session-index) | 0 | 2026-09-01 | 2026-09-01 | 🔍 Full-text session search & bookmarking engine for DSH with native CJK substring search |
| 1128 | [HuangLM03/dsh-plugin-session-archive](https://github.com/HuangLM03/dsh-plugin-session-archive) | 0 | 2026-08-31 | 2026-08-31 | Browse and permanently delete archived DeepSeek Harness sessions from the sidebar footer. |
| 1129 | [HuanLinOTO/dsh-plugin-android-use](https://github.com/HuanLinOTO/dsh-plugin-android-use) | 0 | 2026-09-03 | 2026-09-03 | 让模型通过 adb 操作安卓手机的 DSH 插件（截图、UI 树、点击、滑动、输入文本、按键、打开应用） \| DSH plugin exposing adb-based tools that let the model operate an Android phone (screenshot, UI dump, tap, swipe, input text, press keys, open apps). |
| 1130 | [HuanLinOTO/dsh-plugin-better-plan](https://github.com/HuanLinOTO/dsh-plugin-better-plan) | 0 | 2026-09-03 | 2026-09-03 | better-plan: DSH 计划/待办侧边栏插件 \| DSH plan/todo sidebar plugin |
| 1131 | [HuanLinOTO/dsh-plugin-copilot](https://github.com/HuanLinOTO/dsh-plugin-copilot) | 0 | 2026-08-28 | 2026-08-28 | Copilot 引导层插件：WebUI 设置卡片一键 GitHub 授权 + 自动激活模型路由并收窄模型列表（复用 dsh-llm-pi-ai 内置 device-flow） \| Copilot onboarding plugin: one-click GitHub auth from the WebUI settings card, auto-activating the model route and narrowing the model list (reuses dsh-llm-pi-ai's builtin device flow) |
| 1132 | [HuanLinOTO/dsh-plugin-preface-context](https://github.com/HuanLinOTO/dsh-plugin-preface-context) | 0 | 2026-09-03 | 2026-09-03 | 在每次会话开头固定注入一段用户配置的文本上下文（设置页输入框可编辑），作为模型可见的 instructions 注入第一轮请求。 \| Injects a user-configured text block as model-visible instructions context at the start of every DSH session (editable from the settings page). |
| 1133 | [HuanLinOTO/dsh-plugin-tools-manager](https://github.com/HuanLinOTO/dsh-plugin-tools-manager) | 0 | 2026-08-14 | 2026-08-28 | DSH 工具管理器：查看/启停宿主已注册工具 \| DSH tools manager: inspect and toggle host-registered tools |
| 1134 | [HuanyuTan777/dsh-tool-pdf](https://github.com/HuanyuTan777/dsh-tool-pdf) | 0 | 2026-08-28 | 2026-08-28 | DSH PDF reader plugin (pdf_info / pdf_extract / pdf_render) |
| 1135 | [huashenglian/dsh-omni-workstation](https://github.com/huashenglian/dsh-omni-workstation) | 0 | 2026-09-04 | 2026-09-04 | dsh全模态工作站插件，让模型支持视频、图片、语音的输入与输出，支持comfyui图像生成工具调用。Any-to-Any. |
| 1136 | [huaxiren6/DSH-QrPairing](https://github.com/huaxiren6/DSH-QrPairing) | 0 | 2026-08-19 | 2026-08-27 | Floating phone-pairing QR button for the DSH WebUI. Companion UI for dsh-remote-link. |
| 1137 | [HULILI-com/dsh-namecheck](https://github.com/HULILI-com/dsh-namecheck) | 0 | 2026-08-26 | 2026-08-27 | dsh plugin for checking domain availability and trademark screening of candidate product names |
| 1138 | [hun1315/dsh-msi-icons](https://github.com/hun1315/dsh-msi-icons) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 模型选择器美化插件：厂商官方图标 + 四区平铺 + 置顶主力超时自动路由 \| Model selector beautifier for DSH: official vendor icons, pinned-first flat layout, first-token-timeout failover |
| 1139 | [hun1315/tencent-agent-mail-dsh-plugin](https://github.com/hun1315/tencent-agent-mail-dsh-plugin) | 0 | 2026-09-03 | 2026-09-03 | Tencent Agent Mail (agent.qq.com) workbench plugin for DeepSeek Harness: polling, LLM classification, fullscreen workbench, archive/trash, attachment download, mail-to-agent command channel. 腾讯Agent邮箱DSH插件 |
| 1140 | [hunbs-1/dsh-codepect](https://github.com/hunbs-1/dsh-codepect) | 0 | 2026-08-29 | 2026-08-30 | dsh-codepect is a DSH plugin generating OpenAPI 3.0 from TS/JS. Features: visual docs, versioning, change detection, mock & auto-rescan. Zero-dep, offline, ensures code-doc sync for backend API delivery. dsh-codepect是DSH插件，扫描TS/JS生成OpenAPI3.0文档。支持可视化、多版本、变更检测、Mock及自动重扫。零依赖离线可用，确保代码文档一致，助后端交付API契约。 |
| 1141 | [hunterxxn/deep-flow](https://github.com/hunterxxn/deep-flow) | 0 | 2026-08-14 | 2026-08-29 | deepseek-harness tui |
| 1142 | [HUSTforever/dsh-status-hub](https://github.com/HUSTforever/dsh-status-hub) | 0 | 2026-09-03 | 2026-09-03 | Bilingual DeepSeek Harness status hub for sessions, MCP, skills, plugins, and connection health |
| 1143 | [huyang2024/dsh-openai-api](https://github.com/huyang2024/dsh-openai-api) | 0 | 2026-08-27 | 2026-08-27 | OpenAI-compatible HTTP surface for DeepSeek Harness (dsh): POST /v1/chat/completions, POST /v1/responses, GET /v1/models over the harness webServer + llm runtime |
| 1144 | [hyqhyq3/dsh-gemini-oauth-bridge](https://github.com/hyqhyq3/dsh-gemini-oauth-bridge) | 0 | 2026-09-03 | 2026-09-03 | Bridge Google AI subscription (Antigravity/Gemini OAuth) into DeepSeek Harness as an OpenAI-compatible endpoint |
| 1145 | [hyqhyq3/dsh-plugin-updater](https://github.com/hyqhyq3/dsh-plugin-updater) | 0 | 2026-09-03 | 2026-09-03 | Package-level plugin manager with update detection and a GitHub marketplace for DeepSeek Harness |
| 1146 | [ice5kysl/dsh-workspace-kit](https://github.com/ice5kysl/dsh-workspace-kit) | 0 | 2026-09-04 | 2026-09-04 | dsh (DeepSeek Harness) workspace kit: ⌘K Spotlight search, soft workspace archive/restore, per-workspace icons/colors, enhanced sidebar with drag reorder — Cordis bundle plugin (host tools + browser client). |
| 1147 | [IcedWatermelonJuice/dsh-provider-veark](https://github.com/IcedWatermelonJuice/dsh-provider-veark) | 0 | 2026-08-30 | 2026-08-31 | 把火山方舟 Coding Plan 装进 DeepSeek Harness：文本 + 图片对话，图片走 Files API，密钥粘贴即用 |
| 1148 | [Icstick/dsh-context-maid](https://github.com/Icstick/dsh-context-maid) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 自动上下文策展插件：tool 输出内容感知瘦身 + 无效日志清理 + 工作流/记忆钉扎保护 + 先归档后压缩 + 摘要模型可配 |
| 1149 | [icyaaaww/dsh-tui-secret-guard](https://github.com/icyaaaww/dsh-tui-secret-guard) | 0 | 2026-08-26 | 2026-08-27 | Blocks high-confidence secrets before dsh-TUI sends them to a model, compliant with dsh ecosystem manifest v0.15. |
| 1150 | [iguanren/Taishan-Vision](https://github.com/iguanren/Taishan-Vision) | 0 | 2026-08-29 | 2026-08-29 | 让 DeepSeek Harness 纯文本模型也能识图：默认推荐智谱 GLM-4.6V-FLASH和 GLM-4.1V-FLASH 免费视觉模型 |
| 1151 | [ihorleleka/Local-Rag-Wiki](https://github.com/ihorleleka/Local-Rag-Wiki) | 0 | 2026-06-03 | 2026-08-27 | A per-repository, Docker-hosted MCP knowledge service that gives coding agents a governed Markdown "wiki" with semantic retrieval. The promise — a local RAG wiki that accumulates durable project knowledge across agentic sessions. |
| 1152 | [ikomom/dsh-a-share-assistant](https://github.com/ikomom/dsh-a-share-assistant) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness A股研究助手插件：对话式选股/排雷/盯盘/复盘，数据走同花顺金融数据 API，带本地缓存层。 |
| 1153 | [ikomom/dsh-trade-chart](https://github.com/ikomom/dsh-trade-chart) | 0 | 2026-08-14 | 2026-08-31 | DeepSeek Harness 交易图表插件：对话内直接渲染 K线/折线/柱状/面积图、技术指标（EMA/BOLL/MACD/RSI/KDJ/MAVOL）、热点轮动矩阵与连板晋级图。纯自绘 SVG，零外部依赖，附在线示例页。 |
| 1154 | [imkingjh999/dsh-adaptive-effort](https://github.com/imkingjh999/dsh-adaptive-effort) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: auto reasoning_effort (low/high/max) per turn via MiniMax complexity scorer + token ledger + per-reply metadata label |
| 1155 | [intsig-textin/dsh-plugin-xparse](https://github.com/intsig-textin/dsh-plugin-xparse) | 0 | 2026-08-28 | 2026-08-31 | TextIn xParse document parsing tool and skill for DeepSeek Harness, with multi-document tasks, OAuth/AppKey authentication, and paid-operation approval. |
| 1156 | [Islulua/dsh-code-navigator](https://github.com/Islulua/dsh-code-navigator) | 0 | 2026-09-02 | 2026-09-04 | Persistent C/C++, Python, and TypeScript code navigation for DeepSeek Harness. |
| 1157 | [iTrimut/GitHub-Road](https://github.com/iTrimut/GitHub-Road) | 0 | 2026-08-28 | 2026-08-28 | Github-Road: 大陆稳定访问 GitHub 官网的网络路径修复技能（hosts 直连 + 动态 IP 择优 + 30 分钟自动自愈，免代理、零费用）——非 agent 专属，任意智能体可用，也可纯手动运行。A network-path fix skill (not agent-specific) for reliable github.com access from mainland China. |
| 1158 | [jaaty/dsh-gsd-bundle](https://github.com/jaaty/dsh-gsd-bundle) | 0 | 2026-08-23 | 2026-08-30 | A DeepSeek Harness bundle reimplementing opengsd-core (Git Ship Done) as host-plane Cordis plugins, replacing the default agent-loop behaviour with the GSD phase loop. |
| 1159 | [JackyYangxx/dsh-plugins](https://github.com/JackyYangxx/dsh-plugins) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness (DSH) plugin workspace — home of lbx-agent-team, a multi-agent development team plugin (captain-led planner/checker/dever/tester with pipeline hard gates, git worktrees and a live web panel) |
| 1160 | [jackyytche/dsh-hindsight-memory](https://github.com/jackyytche/dsh-hindsight-memory) | 0 | 2026-09-01 | 2026-09-01 | Hindsight long-term memory for DeepSeek Harness |
| 1161 | [jarvis959/galvanize-dsh](https://github.com/jarvis959/galvanize-dsh) | 0 | 2026-08-28 | 2026-08-28 | Triggers inside your DSH agent: wake a fresh DeepSeek Harness session when files, mail, webhooks, or git events happen. Native Cordis bundle, heartbeat-proved install. |
| 1162 | [jasonguide/dsh-skills-hub](https://github.com/jasonguide/dsh-skills-hub) | 0 | 2026-08-28 | 2026-08-29 | 一个多 Agent 平台的 Skills 统一管理插件（DeepSeek Harness 插件），可以在DSH中统一管理codex、claude code、PI、OpenCode、Hermes、Openclaw等平台的Skills技能 |
| 1163 | [jaychouu/see_the_screen](https://github.com/jaychouu/see_the_screen) | 0 | 2026-09-04 | 2026-09-04 | Windows desktop automation plugin for DeepSeek Harness (DSH) agents. Part of DSH Plugin Ecosystem. |
| 1164 | [jcaiagent7143-ui/linkdigest-mcp](https://github.com/jcaiagent7143-ui/linkdigest-mcp) | 0 | 2026-09-03 | 2026-09-04 | MCP server for LinkDigest — turn a Xiaohongshu, Douyin, TikTok, YouTube or X link into LLM-ready text: transcript, on-screen text, image descriptions, caption and metadata. Streamable HTTP. |
| 1165 | [jdqingm/dsh-plan-build-toggle](https://github.com/jdqingm/dsh-plan-build-toggle) | 0 | 2026-08-31 | 2026-08-31 | OpenChamber-style persistent Plan\|Build composer toggle for DeepSeek Harness, with Tab-to-switch. Drives the native /plan channel over the host plan projection. |
| 1166 | [Jensen-Yao/dsh-deepexcel](https://github.com/Jensen-Yao/dsh-deepexcel) | 0 | 2026-08-27 | 2026-08-28 | Deepcel 工作簿 · DeepSeek Harness (dsh) 皮肤中心 v2 皮肤：Excel 风格工作簿，单元格化消息、工作表网格、工作簿标签。Small-tailqwq/dsh-deepcel 的 v2 完整移植。 |
| 1167 | [jhckevin/dsh-request-privacy](https://github.com/jhckevin/dsh-request-privacy) | 0 | 2026-09-04 | 2026-09-04 | Live request metadata minimization for DeepSeek Harness, covering the native DeepSeek provider with WebUI settings. |
| 1168 | [Jiachi5533/dsh-remote-gateway](https://github.com/Jiachi5533/dsh-remote-gateway) | 0 | 2026-08-28 | 2026-08-28 | Source-filtered remote gateway for DeepSeek Harness behind an authenticated reverse proxy |
| 1169 | [jiang12345-code/dsh-openrouter-free](https://github.com/jiang12345-code/dsh-openrouter-free) | 0 | 2026-08-27 | 2026-08-27 | OpenRouter 免费模型面板 for DeepSeek Harness — 分级星标 · 一键切换 · 任务续跑友好 |
| 1170 | [jiang12345-code/dsh-self-restart](https://github.com/jiang12345-code/dsh-self-restart) | 0 | 2026-08-29 | 2026-08-29 | DSH self-restart plugin (Windows): reliable elevated restart via schtasks, transparent front-end recovery, auto-detect and resume in-progress sessions across reboots, business gate prevents wake self-excitation loops. |
| 1171 | [jiangchuangege/anime-pet-widget](https://github.com/jiangchuangege/anime-pet-widget) | 0 | 2024-01-19 | 2026-08-27 | jenkins测试 |
| 1172 | [JiayiXie-jpg/dsh-desktop-pet](https://github.com/JiayiXie-jpg/dsh-desktop-pet) | 0 | 2026-08-26 | 2026-08-27 | 一只住在 DSH 网页里的养成系桌宠：随编码活动升级进化、语音打气，还能用 AI 生成专属的透明动画形象。 |
| 1173 | [jimmyzhang219/dsh-plan-and-execute](https://github.com/jimmyzhang219/dsh-plan-and-execute) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness (dsh) 的 Plan-and-Execute 编排插件 |
| 1174 | [JingzeChen/dsh-beacon](https://github.com/JingzeChen/dsh-beacon) | 0 | 2026-09-02 | 2026-09-02 | Attention and handoff workspace for concurrent DeepSeek Harness Sessions |
| 1175 | [jingzhonghui/dsh-mcp-manager](https://github.com/jingzhonghui/dsh-mcp-manager) | 0 | 2026-08-30 | 2026-08-30 | DSH dynamic Cordis plugin: visually manage MCP servers (stdio) from the settings sidebar, and expose their tools to the agent as mcp__<server>__<tool>. |
| 1176 | [jinwendijv/dsh-applauncher](https://github.com/jinwendijv/dsh-applauncher) | 0 | 2026-08-27 | 2026-08-27 | DSH 的应用启动器插件：自动扫描本机已安装的电脑应用，在侧边栏“设置”图标上方提供一键启动，像 Windows 开始菜单一样，扫描添加后可以点击启动应用 |
| 1177 | [jmche/dsh-llm-verifier-pro](https://github.com/jmche/dsh-llm-verifier-pro) | 0 | 2026-08-26 | 2026-09-02 | LLM-as-a-Verifier plugin for DeepSeek Harness — fine-grained reward tools (verify_compare / verify_select / verify_track) with Probabilistic Pivot Tournament, plus a Best-of-N conversation mode with a Web settings panel. |
| 1178 | [jo32/dsh-strudel-studio](https://github.com/jo32/dsh-strudel-studio) | 0 | 2026-08-29 | 2026-08-30 | A professional song-level Strudel visual sequencer with structured AI arrangement for DeepDeck. |
| 1179 | [jo32/dsh-video-sherlock](https://github.com/jo32/dsh-video-sherlock) | 0 | 2026-08-26 | 2026-08-27 | A local-first, evidence-backed video investigation app for DeepDeck. |
| 1180 | [joao-paulo-santos/dsh-bouncing-squares-example](https://github.com/joao-paulo-santos/dsh-bouncing-squares-example) | 0 | 2026-08-26 | 2026-08-27 | Example plugin for dsh-granular-settings: three bouncing squares, one per settings scope (session, workspace, global). Switch sessions and workspaces to watch each scope behave differently |
| 1181 | [joao-paulo-santos/dsh-diff-view](https://github.com/joao-paulo-santos/dsh-diff-view) | 0 | 2026-08-29 | 2026-08-29 | Diff view: a reusable two-text diff viewer for DSH client plugins — line LCS, word highlights, split/unified views, true line numbers across context collapse. |
| 1182 | [joao-paulo-santos/dsh-granular-prompt](https://github.com/joao-paulo-santos/dsh-granular-prompt) | 0 | 2026-08-27 | 2026-08-27 | Prompt composition manager for DSH: live census of every system-prompt section with suppress and replace, custom system prompts, and a persona library with a picker right in the chat composer |
| 1183 | [joao-paulo-santos/dsh-granular-settings](https://github.com/joao-paulo-santos/dsh-granular-settings) | 0 | 2026-08-26 | 2026-08-27 | Granular settings platform: one Granular Settings page (Workspace/Session/Plugin tabs) where other DSH plugins register scoped, namespaced controls (session, workspace, global). Nine control types, doorbell-only push via dsh-event-relay |
| 1184 | [joao-paulo-santos/dsh-md-view](https://github.com/joao-paulo-santos/dsh-md-view) | 0 | 2026-08-29 | 2026-08-29 | Markdown view: a safe markdown-to-React renderer for DSH client plugins — GitHub-subset markdown, shared stylesheet, no HTML injection. |
| 1185 | [joao-paulo-santos/dsh-scratchpad](https://github.com/joao-paulo-santos/dsh-scratchpad) | 0 | 2026-08-28 | 2026-08-28 | Scratch pad: one shared floating text surface in the middle of the screen, opened by other plugins through the client service scratchpad. |
| 1186 | [joao-paulo-santos/dsh-wo-github](https://github.com/joao-paulo-santos/dsh-wo-github) | 0 | 2026-08-29 | 2026-08-29 | Workspace Overview GitHub tab: About card, README rendered as markdown, and the default-branch commit history with per-file patches. |
| 1187 | [joao-paulo-santos/dsh-wo-tmux](https://github.com/joao-paulo-santos/dsh-wo-tmux) | 0 | 2026-08-31 | 2026-09-01 | Workspace Overview tmux tab: live/frozen/cold session state, one-click terminal attach through tmux-fridge, freeze/snapshot/recover, and workspace-to-session links. |
| 1188 | [joao-paulo-santos/dsh-workspace-overview](https://github.com/joao-paulo-santos/dsh-workspace-overview) | 0 | 2026-08-28 | 2026-08-28 | Workspace overview: a Workspace Overview tab beside Chat with a subtab facade for other plugins, and a GitHub pill in the session header when the workspace has a github.com repository. |
| 1189 | [JochenYang/dsh-remote](https://github.com/JochenYang/dsh-remote) | 0 | 2026-08-29 | 2026-08-29 | Operate DeepSeek Harness from your phone: self-hosted relay + desktop plugin tunnel with a mobile-adapted web UI. MIT |
| 1190 | [JoeeLiu/dsh-super-subscriptions](https://github.com/JoeeLiu/dsh-super-subscriptions) | 0 | 2026-08-28 | 2026-08-28 | Unified subscription providers, model routing, quota UI, and media tools for DeepSeek Harness |
| 1191 | [JoeyLearnsToCode/dsh-workspace-native-open](https://github.com/JoeyLearnsToCode/dsh-workspace-native-open) | 0 | 2026-08-28 | 2026-08-28 | dsh plugin for native open workspace / 用于本地打开工作区目录的 dsh 插件 |
| 1192 | [johnvictorio/dsh-custom-prompt](https://github.com/johnvictorio/dsh-custom-prompt) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin that injects an editable section into the global system prompt, with a Settings page |
| 1193 | [joshryandavis/dsh-catalog-refresh](https://github.com/joshryandavis/dsh-catalog-refresh) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically rebuild model catalogues for OpenRouter, OpenCode, Fireworks, etc |
| 1194 | [joshryandavis/dsh-goal-restart](https://github.com/joshryandavis/dsh-goal-restart) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically restart goals on harness restart |
| 1195 | [JPA957/dsh-web-search-anysearch](https://github.com/JPA957/dsh-web-search-anysearch) | 0 | 2026-09-02 | 2026-09-02 | AnySearch search provider plugin for DeepSeek Harness (ctx.web) with round-robin API-key rotation and per-key cooldown failover |
| 1196 | [jsoncode/dsh-model-list](https://github.com/jsoncode/dsh-model-list) | 0 | 2026-08-27 | 2026-08-28 | OpenRouter free-models browser & one-click model config for DeepSeek Harness (DSH) — newest-first, local search, platform tabs. DSH 免费模型浏览器：按最新排序、本地搜索、一键添加到模型列表 |
| 1197 | [jsoncode/dsh-single-terminal](https://github.com/jsoncode/dsh-single-terminal) | 0 | 2026-09-03 | 2026-09-03 | 基于dsh的终端插件 |
| 1198 | [justhalfbit/dsh-plugin-show-image](https://github.com/justhalfbit/dsh-plugin-show-image) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness (DSH) 会话内图片渲染插件：全局 show_image 工具 + 点击放大 lightbox。 \| Inline image rendering plugin for DSH: global show_image tool + click-to-enlarge lightbox. |
| 1199 | [jwilson411/dsh-arxiv](https://github.com/jwilson411/dsh-arxiv) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: tiny read-only arXiv search + abstract fetch (Atom API, no PDF ingest) |
| 1200 | [jwilson411/dsh-canary](https://github.com/jwilson411/dsh-canary) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: plant a canary and deny tool args/URLs that echo it (CANARY_TRIP). |
| 1201 | [jwilson411/dsh-compat-probe](https://github.com/jwilson411/dsh-compat-probe) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: OpenAI-compat server protocol card (loopback probe, no GGUF) |
| 1202 | [jwilson411/dsh-kokoro](https://github.com/jwilson411/dsh-kokoro) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: HTTP TTS client for jwilson411/kokoro-tts-api. No weights. |
| 1203 | [jwilson411/dsh-llamacpp](https://github.com/jwilson411/dsh-llamacpp) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness LLM adapter for a local llama.cpp OpenAI-compatible server. |
| 1204 | [jwilson411/dsh-loop-brake](https://github.com/jwilson411/dsh-loop-brake) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: identical tool+args circuit breaker (LOOP_BRAKE) |
| 1205 | [jwilson411/dsh-modelprint](https://github.com/jwilson411/dsh-modelprint) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: fingerprint provider, model id, sampling, tool schemas, and system-prompt prefix; pin the card and fail structured on drift. |
| 1206 | [jwilson411/dsh-mutation-receipt](https://github.com/jwilson411/dsh-mutation-receipt) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: append-only JSONL of filesystem touches (path, op, sha256 before/after) with no file contents |
| 1207 | [jwilson411/dsh-otel](https://github.com/jwilson411/dsh-otel) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: emit OpenTelemetry spans from a session log (turn / step / tool execute). Export only. |
| 1208 | [jwilson411/dsh-plugin-kit](https://github.com/jwilson411/dsh-plugin-kit) | 0 | 2026-08-29 | 2026-08-29 | A minimal, tested template for DeepSeek Harness plugins. |
| 1209 | [jwilson411/dsh-result-cap](https://github.com/jwilson411/dsh-result-cap) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: deterministic tool-result byte cap with SHA-256 of the omitted tail. Not a compressor model. |
| 1210 | [jwilson411/dsh-secret-scrub](https://github.com/jwilson411/dsh-secret-scrub) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: redact known secret shapes before the model sees them; JSONL incidents never store the preimage |
| 1211 | [jwilson411/dsh-spend-receipt](https://github.com/jwilson411/dsh-spend-receipt) | 0 | 2026-08-29 | 2026-08-31 | A cache-aware JSONL cost receipt plugin for DeepSeek Harness. |
| 1212 | [jwilson411/dsh-ssrf-guard](https://github.com/jwilson411/dsh-ssrf-guard) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness plugin: fail-closed URL host/scheme allowlist that runs before a request is opened |
| 1213 | [jwilson411/dsh-tool-quota](https://github.com/jwilson411/dsh-tool-quota) | 0 | 2026-08-31 | 2026-09-01 | DeepSeek Harness plugin: per-tool call and result-byte caps |
| 1214 | [kaixinguo360/dsh-bsk-ws-bridge](https://github.com/kaixinguo360/dsh-bsk-ws-bridge) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness BrowserSkill 桥接插件：把本机 bsk daemon 的 WebSocket 经浏览器信道暴露给远程 BrowserSkill 扩展。配套的修改版 BrowserSkill 扩展：https://github.com/kaixinguo360/BrowserSkill-DSH-Remote |
| 1215 | [kaka-crypto/dsh-disk-guard](https://github.com/kaka-crypto/dsh-disk-guard) | 0 | 2026-08-28 | 2026-08-28 | Disk guard for DeepSeek Harness: redirect downloads/artifacts/caches/temp off the C: drive, inject a path-discipline prompt into every session, disk_guard tool for status/cleanup. |
| 1216 | [kalifun/dsh-cwl](https://github.com/kalifun/dsh-cwl) | 0 | 2026-09-01 | 2026-09-01 | Structured context eviction for DeepSeek Harness — deterministic, zero-LLM, no summarization lossiness |
| 1217 | [KarthusLorin/dsh-subagent-grok](https://github.com/KarthusLorin/dsh-subagent-grok) | 0 | 2026-08-29 | 2026-08-29 | One-shot Grok CLI subagent provider for DeepSeek Harness |
| 1218 | [KDronin/dsh-folder](https://github.com/KDronin/dsh-folder) | 0 | 2026-08-16 | 2026-09-01 | DeepSeek Harness plugin: Open Folder in workspace context menu (between Rename and Delete Workspace) |
| 1219 | [KDronin/dsh-tray](https://github.com/KDronin/dsh-tray) | 0 | 2026-08-16 | 2026-09-01 | DeepSeek Harness 桌面托盘插件：托盘启动 Harness、任务完成通知、电源管理、进程接管、GitHub 集成 |
| 1220 | [Kehao/dsh-client-ui-weather](https://github.com/Kehao/dsh-client-ui-weather) | 0 | 2026-08-30 | 2026-08-30 | Deepseek harness 天气插件 |
| 1221 | [kenny2077/dsh-web-kimi](https://github.com/kenny2077/dsh-web-kimi) | 0 | 2026-08-31 | 2026-08-31 | Kimi Coding web search + web fetch providers for the DeepSeek Harness with coding plan key |
| 1222 | [KeS1Ke/dsh-start-and-exit](https://github.com/KeS1Ke/dsh-start-and-exit) | 0 | 2026-08-24 | 2026-08-27 | dsh-start&exit: safe start, exit, and restart controls for the DeepSeek Harness Web profile, plus a loopback-only Windows foreground launcher. |
| 1223 | [kfc966/dsh-native-codex-oauth](https://github.com/kfc966/dsh-native-codex-oauth) | 0 | 2026-09-01 | 2026-09-01 | Native Codex OAuth login and model access for DeepSeek Harness as one installable plugin. |
| 1224 | [KimFischer99/DeepSeek-Harness-Desktop](https://github.com/KimFischer99/DeepSeek-Harness-Desktop) | 0 | 2026-08-15 | 2026-08-27 | 一个轻量的 macOS 桌面应用壳，Rust 编写，承载 DeepSeek Harness WebUI，一键启停 |
| 1225 | [kingcheng12/dsh-workspace-change-awareness](https://github.com/kingcheng12/dsh-workspace-change-awareness) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin that surfaces concurrent workspace changes before an agent continues. |
| 1226 | [kittcat-lab/dsh-kitt-voice](https://github.com/kittcat-lab/dsh-kitt-voice) | 0 | 2026-09-01 | 2026-09-02 | Voice for the DeepSeek Harness: speak to the agent, hear it back, and see what it is doing from a floating window that stays on top of whatever you are running. |
| 1227 | [kittimzhe/dsh-plugin-authoring-guide](https://github.com/kittimzhe/dsh-plugin-authoring-guide) | 0 | 2026-08-29 | 2026-08-29 | Hands-on guide to building a DeepSeek Harness plugin (EN/ZH) — real code & pitfalls from dsh-session-export and dsh-session-recall |
| 1228 | [KKL08/dsh-plastic-memory](https://github.com/KKL08/dsh-plastic-memory) | 0 | 2026-09-04 | 2026-09-02 | Memory plugin with built-in curation and governance for DeepSeek Harness: 为你的 DSH 赋予可塑性记忆 |
| 1229 | [KL3jd/handwritten-ocr](https://github.com/KL3jd/handwritten-ocr) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin for local OCR: handwritten Chinese + math → Markdown with LaTeX. GPU / CPU backends. |
| 1230 | [klarkxy/dsh-plugins](https://github.com/klarkxy/dsh-plugins) | 0 | 2026-09-03 | 2026-09-03 | Small, independently installable plugins for DeepSeek Harness. |
| 1231 | [knownothing114/dsh-notify](https://github.com/knownothing114/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | A dsh plugin that raises a desktop notification whenever dsh needs your attention. |
| 1232 | [kobenfang/BigTimer](https://github.com/kobenfang/BigTimer) | 0 | 2026-08-29 | 2026-08-29 | 🕐 BigTimer · 定时任务+消息推送管家 — Scheduled tasks & message push manager for DeepSeek Harness (dsh) |
| 1233 | [Kogisune/dsh-skin-koi-pond](https://github.com/Kogisune/dsh-skin-koi-pond) | 0 | 2026-08-20 | 2026-08-28 | 🎏 锦鲤池塘 · Koi Pond theme for DeepSeek Harness (DSH) WebUI — 动画锦鲤 + 部件拆分 CSS |
| 1234 | [kolawong/dsh-plugin-toolkit](https://github.com/kolawong/dsh-plugin-toolkit) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness personal toolkit: runtime-toggleable quality-of-life optimizations, each shipped as one card in the Toolkit settings page. |
| 1235 | [kongshan-zhuyu/dsh-balance-quota](https://github.com/kongshan-zhuyu/dsh-balance-quota) | 0 | 2026-08-18 | 2026-09-01 | 一块可以配置余额、监测模型监控状态、以及配置模型多模态设置的插件 |
| 1236 | [kp-z/dsh-dev-git-graph](https://github.com/kp-z/dsh-dev-git-graph) | 0 | 2026-09-01 | 2026-09-02 | DSH Web Git Graph panel — a faithful port of vscode-git-graph 1.30.0, auto-bound to the session workspace, with full git operations and light/dark theming. First of the dsh-dev-* graph plugin series. |
| 1237 | [kristol07/dsh-discussions-digest](https://github.com/kristol07/dsh-discussions-digest) | 0 | 2026-09-04 | 2026-09-04 | A small, evidence-first DeepSeek Harness plugin for recent activity in the official GitHub Discussions. |
| 1238 | [ktao732084-arch/dsh-vibegap](https://github.com/ktao732084-arch/dsh-vibegap) | 0 | 2026-08-27 | 2026-08-27 | Vocabulary flashcards inside the dsh web UI - appear while your agent runs, retreat when it finishes. A VibeGap plugin. |
| 1239 | [ktao732084-arch/vibegap](https://github.com/ktao732084-arch/vibegap) | 0 | 2026-08-26 | 2026-08-27 | Mini-window for the gaps in vibe coding: vocabulary flashcards (and more panels) that auto-appear while your AI coding agent runs |
| 1240 | [kuanfu0430/dsh-compaction-tune](https://github.com/kuanfu0430/dsh-compaction-tune) | 0 | 2026-09-01 | 2026-09-01 | Composer control for DeepSeek Harness auto-compaction thresholds |
| 1241 | [kumanana66/dsh-automation](https://github.com/kumanana66/dsh-automation) | 0 | 2026-09-01 | 2026-09-01 | RPA-style scheduled web automation for DeepSeek Harness: record browser operations -> requirements doc -> LLM generates Python + Playwright -> schedule with run records and email notifications |
| 1242 | [KumarZX/dsh-memory-wrap](https://github.com/KumarZX/dsh-memory-wrap) | 0 | 2026-09-04 | 2026-09-04 | DSH plugins: idle memory wrap-up sidebar plus vault search, distill, and rules. |
| 1243 | [KumarZX/kur-compact-trigger](https://github.com/KumarZX/kur-compact-trigger) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件 · 会话级压缩（官方 auto 只能全局） / Per-session compaction; official auto is global-only |
| 1244 | [l2685209197/dsh-pdf-translate](https://github.com/l2685209197/dsh-pdf-translate) | 0 | 2026-09-01 | 2026-09-01 | DSH 插件：用 DeepSeek 翻译文本型 PDF，保留版式/字体/图片/链接，输出可编辑 PDF（单次 ≤50 页） |
| 1245 | [LamplitIsles/kepos-speech](https://github.com/LamplitIsles/kepos-speech) | 0 | 2026-08-29 | 2026-09-04 | Qwen/Volcengine TTS/STT for dsh |
| 1246 | [Lanzgale/dsh-listener](https://github.com/Lanzgale/dsh-listener) | 0 | 2026-08-30 | 2026-08-30 | 安全版本地语音输入插件 for DeepSeek Harness:同源宿主代理 + 127.0.0.1 + token,SenseVoice-Small INT8 ONNX 本地转写,音频不出网。 |
| 1247 | [lasdrder0705/dsh-chat-zone-std](https://github.com/lasdrder0705/dsh-chat-zone-std) | 0 | 2026-08-26 | 2026-08-27 | dsh-std Community v0.15 chat zone: ~/dsh_CHAT/<date>/chatN as Tools and Commands. Install adapter-dsh first. |
| 1248 | [lasdrder0705/dsh-pro-vision-std](https://github.com/lasdrder0705/dsh-pro-vision-std) | 0 | 2026-08-26 | 2026-08-27 | dsh-std Community v0.15 ModelProvider: V4-Pro with Flash-Vision captions. Install adapter-dsh first. |
| 1249 | [lastplayer82/dsh-sticky-notes](https://github.com/lastplayer82/dsh-sticky-notes) | 0 | 2026-08-27 | 2026-08-27 | 灵感便签 (Sticky Notes) plugin for the dsh web GUI: jot ideas while the agent thinks — without interrupting it. Queue-channel sends/forwards, auto-persist (localStorage + host file), export TXT/JSON/MD, bilingual zh/en. DeepSeek Harness plugin · @lastplayer82/dsh-sticky-notes |
| 1250 | [lcthe/dsh-hermes-memory](https://github.com/lcthe/dsh-hermes-memory) | 0 | 2026-08-26 | 2026-09-04 | DSH-native persistent memory and safe session-aware retrieval plugin |
| 1251 | [leechengwei/dsh-session-intelligence](https://github.com/leechengwei/dsh-session-intelligence) | 0 | 2026-08-31 | 2026-08-31 | DSH 会话情报：固定右侧栏、初衷与最近用户需求摘要、会话活动和只读 Git 状态。 |
| 1252 | [leeseo39/dsh-we-wallpaper](https://github.com/leeseo39/dsh-we-wallpaper) | 0 | 2026-09-04 | 2026-09-04 | Wallpaper Engine assets as DeepSeek Harness dynamic background — upstream skin-center 0.3.14 source snapshot + self-built WE engine research |
| 1253 | [lelens0/dsh-token-ledger](https://github.com/lelens0/dsh-token-ledger) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness plugin: monitor balance & usage across multiple LLM gateways, with balance history sparklines (token ledger) |
| 1254 | [lemoncat7/dsh-partner](https://github.com/lemoncat7/dsh-partner) | 0 | 2026-08-27 | 2026-08-31 | Long-lived AI companions with WeChat channel routing for DeepSeek Harness |
| 1255 | [Leo3-7/dsh-obsidian-inbox](https://github.com/Leo3-7/dsh-obsidian-inbox) | 0 | 2026-08-28 | 2026-08-28 | DSH skill: ingest the conclusions/mistakes/projects from conversations into an Obsidian vault via a 7-step workflow with two-level validation. 把对话结论/错题/项目按七步流程整理进 Obsidian 的 DeepSeek Harness 技能。 |
| 1256 | [LeoChen98/dsh-worktable-notebook-to-ppt](https://github.com/LeoChen98/dsh-worktable-notebook-to-ppt) | 0 | 2026-08-26 | 2026-08-27 | 基于 dsh-worktable 工作台搭建的「课本到 PPT」自动化工作流插件——在 DeepSeek Harness 中一键将 Jupyter Notebook 转化为专业可编辑的演示文稿（.pptx），让知识沉淀与分享更高效。 |
| 1257 | [leogottadothebest/dsh-plugin-archived-conversations](https://github.com/leogottadothebest/dsh-plugin-archived-conversations) | 0 | 2026-08-31 | 2026-09-02 | DSH 插件：在设置界面管理已归档对话——取消归档与永久删除 |
| 1258 | [leogottadothebest/dsh-settings-beautify](https://github.com/leogottadothebest/dsh-settings-beautify) | 0 | 2026-09-01 | 2026-09-02 | One design language for the DSH settings surface: unified typography, cards, controls, focus and motion across every settings page, including pages contributed by other plugins. |
| 1259 | [LeonSone/dsh-question-rail](https://github.com/LeonSone/dsh-question-rail) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: 模仿 deepseek 网页版界面右侧的问题条 — 右缘一条竖向问题栏，列出当前会话每一轮的用户提问，点击平滑滚动定位。DeepSeek Harness right-edge question rail. |
| 1260 | [LeonxLJX/dsh-mcp-market](https://github.com/LeonxLJX/dsh-mcp-market) | 0 | 2026-09-03 | 2026-09-03 | The front door to MCP for DeepSeek Harness. Search a verified catalog of MCP servers and get the exact cordis.yml row that wires one into the official @deepseek-ai/dsh-mcp-client bridge. |
| 1261 | [lgquan/dsh-workspace-memory](https://github.com/lgquan/dsh-workspace-memory) | 0 | 2026-08-28 | 2026-08-31 | Durable workspace-scoped memory for DeepSeek Harness and dsh-voco voice agents. |
| 1262 | [lhf6623/dsh-thrum](https://github.com/lhf6623/dsh-thrum) | 0 | 2026-08-16 | 2026-08-29 | DeepSeek Harness 输入氛围插件：为输入过程增添氛围。 |
| 1263 | [liangminhua/agent-notes-toolkit](https://github.com/liangminhua/agent-notes-toolkit) | 0 | 2026-08-30 | 2026-08-30 | Agent Notes mechanism as a portable toolkit: verification gates, scaffolding CLI, and the AN dsh preset/bundle |
| 1264 | [liangsheng999/dsh-client-ui-connection-status](https://github.com/liangsheng999/dsh-client-ui-connection-status) | 0 | 2026-08-26 | 2026-08-27 | DSH Web client plugin: a corner pill showing live connection state for the DeepSeek Harness Web UI. npm: dsh-client-ui-connection-status |
| 1265 | [liangsheng999/dsh-dream](https://github.com/liangsheng999/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH host plugin: scheduled background 'dream' (memory consolidation) passes for DeepSeek Harness. npm: dsh-dream |
| 1266 | [liangxiaobing520/dsh-local-vector-memory](https://github.com/liangxiaobing520/dsh-local-vector-memory) | 0 | 2026-08-29 | 2026-08-29 | Fully local vector memory plugin for DeepSeek Harness: local embeddings, SQLite storage, automatic recall injection, dedup with conflict detection, soft-delete recycle bin, online backup. |
| 1267 | [LianPing-cyber/dsh-browser-full-access](https://github.com/LianPing-cyber/dsh-browser-full-access) | 0 | 2026-08-29 | 2026-08-29 | Full-access background-tab fork of dsh-browser for DeepSeek Harness (DSH). Based on dsh-browser, MCP, and browser-use. |
| 1268 | [liaoyuqing/dsh-llm-error-retry](https://github.com/liaoyuqing/dsh-llm-error-retry) | 0 | 2026-09-02 | 2026-09-02 | 用于在deepseek-harnees中报错时重试大模型请求，支持配置http状态，字段-值命中。 |
| 1269 | [Lichtspur/deepseek-style-theme](https://github.com/Lichtspur/deepseek-style-theme) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek official-home style theme for the dsh web GUI: fluid particle background, glass sidebar, glass composer, frosted header, running-subagent progress panel, DSTT time-based mode, and DeepSeek brand link |
| 1270 | [limlnx523/dsh-plus-plus](https://github.com/limlnx523/dsh-plus-plus) | 0 | 2026-08-27 | 2026-08-28 | DSH++ — a local-first control plane for DeepSeek Harness. Plugin security auditing and workflow regression testing. |
| 1271 | [linkbag/dsh-swarm-orchestrator](https://github.com/linkbag/dsh-swarm-orchestrator) | 0 | 2026-09-02 | 2026-09-02 | Role-based AI swarm orchestration for DeepSeek Harness: per-role model pinning with fallbacks, parallel task DAG with review loops, live Swarm dashboard tab. |
| 1272 | [Lion-Li-git/dsh-external-links](https://github.com/Lion-Li-git/dsh-external-links) | 0 | 2026-08-30 | 2026-08-30 | DSH desktop (Deepseek Harness EAC) plugin: open http/https/mailto/tel/file links in the default browser/app, bypassing the broken shell.open-external bridge |
| 1273 | [lionwill/dsh-compactor](https://github.com/lionwill/dsh-compactor) | 0 | 2026-09-01 | 2026-09-01 | DSH上下文压缩插件 |
| 1274 | [lisongxuan/ds-hentai](https://github.com/lisongxuan/ds-hentai) | 0 | 2026-08-25 | 2026-08-28 | ExHentai-inspired UI for DeepSeek Harness. ExHentai风格DeepSeek Harness皮肤。 ds hentai / deepseek hentai |
| 1275 | [liujia-io/dsh-image-picker](https://github.com/liujia-io/dsh-image-picker) | 0 | 2026-08-26 | 2026-08-27 | Paperclip image-picker button for the DeepSeek Harness web composer - pick reference images via the system file dialog and feed them into the official attachment pipeline. |
| 1276 | [Liujie-harsh/heart-health-dsh-suite](https://github.com/Liujie-harsh/heart-health-dsh-suite) | 0 | 2026-08-28 | 2026-08-28 | 适配心脏健康场景的 DeepSeek Harness 插件套件：在「心衰辅助诊断算法服务（heart-algo MCP）」之上， 为 DSH 会话提供一组受控的领域包装工具、驻留临床指导与原始工具隐藏策略。 |
| 1277 | [liuwenji007/dsh-humanizer](https://github.com/liuwenji007/dsh-humanizer) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 插件：生成前注入「人味」风格约束 + AI 味检测报告（纯代码、零 token、结果可复现）。dsh plugin: human-flavor style injection + AI-flavor detection report, judged by code. |
| 1278 | [liuwenji007/dsh-trust-check](https://github.com/liuwenji007/dsh-trust-check) | 0 | 2026-08-27 | 2026-08-27 | Static capability disclosure for DeepSeek Harness plugins — evidence-backed, zero-token, no safety claims. |
| 1279 | [liuyangdongdong/dsh-session-rerun](https://github.com/liuyangdongdong/dsh-session-rerun) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin for inspecting and replaying completed main-agent and subagent session steps |
| 1280 | [Liyuan1992/memdsl](https://github.com/Liyuan1992/memdsl) | 0 | 2026-07-04 | 2026-09-02 | Agent memory as normative source code |
| 1281 | [Liyuan1992/rawmem](https://github.com/Liyuan1992/rawmem) | 0 | 2026-07-10 | 2026-09-02 | A tiny local-first raw evidence ledger for AI and human workflows. |
| 1282 | [ljc6413/pkg-dev](https://github.com/ljc6413/pkg-dev) | 0 | 2026-08-29 | 2026-08-30 | YiHe 编程认知内核 for DeepSeek Harness：27 领域包 + 55 RFB 经验库 + 工程工具链 + 商业/安全/进化体系（会进化的编程助手） |
| 1283 | [LJH-snow/dsh-tool-kubernetes](https://github.com/LJH-snow/dsh-tool-kubernetes) | 0 | 2026-08-27 | 2026-08-27 | Kubernetes tools for DeepSeek Harness: cluster, namespace, workload, pod, log, rollout, and manifest operations |
| 1284 | [LJH-snow/dsh-tool-monitoring](https://github.com/LJH-snow/dsh-tool-monitoring) | 0 | 2026-08-28 | 2026-08-28 | Prometheus and Alertmanager tool plugin for DeepSeek Harness |
| 1285 | [LJH-snow/dsh-tool-slack](https://github.com/LJH-snow/dsh-tool-slack) | 0 | 2026-08-30 | 2026-08-30 | Slack tools for DeepSeek Harness |
| 1286 | [ljh220300-eng/dsh-plugin-ssh-manager](https://github.com/ljh220300-eng/dsh-plugin-ssh-manager) | 0 | 2026-09-01 | 2026-09-01 | Manage multi-IP DSH instances from one terminal via SSH tunnels · 在一台终端上通过 SSH 隧道管理多 IP 的 DSH |
| 1287 | [ljlj7149-cloud/dsh-cognitio](https://github.com/ljlj7149-cloud/dsh-cognitio) | 0 | 2026-08-26 | 2026-08-27 | 纠错驱动的认知架构插件（DeepSeek Harness）：分层记忆 + 哨兵自动提醒 + 纠错进化 + 审批仲裁。让 AI 记得你的规矩，换模型换预设都有效；所有自动沉淀，你批准才生效。 |
| 1288 | [lkdxzhxi/dsh-glass-ui-theme](https://github.com/lkdxzhxi/dsh-glass-ui-theme) | 0 | 2026-08-29 | 2026-08-29 | 为 DeepSeek Harness 打造的液态玻璃主题插件：磨砂玻璃、可调色调、动态壁纸，让 DSH 界面焕然一新 |
| 1289 | [lnetrit-alt/dsh-system-control](https://github.com/lnetrit-alt/dsh-system-control) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: sidebar-embedded DeepSeek balance readout with a black minimalist full-shutdown button. |
| 1290 | [Lohaslee/dsh-super-pm](https://github.com/Lohaslee/dsh-super-pm) | 0 | 2026-09-01 | 2026-09-01 | Super PM product-thinking skill packaged as a DeepSeek Harness plugin |
| 1291 | [loiasdi/dsh-prompthub-ecosystem](https://github.com/loiasdi/dsh-prompthub-ecosystem) | 0 | 2026-08-26 | 2026-08-27 | PromptHub Ecosystem for DeepSeek Harness (DSH): bilingual Plugin and Skill catalog with GitHub and local tarball installation. |
| 1292 | [lokih1028/dsh-prompt-optimizer](https://github.com/lokih1028/dsh-prompt-optimizer) | 0 | 2026-08-29 | 2026-08-29 | One-click prompt enhancement and structuring plugin for DeepSeek Harness (DSH) |
| 1293 | [Lorvaste/DSH-Project-Initialization](https://github.com/Lorvaste/DSH-Project-Initialization) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：项目初始化插件，通过结构化的整理编排，需求与要素确认，无论是项目刚起步还是准备维护，都有一个好的开始. |
| 1294 | [lovezi0/dsh-visualizer-widget](https://github.com/lovezi0/dsh-visualizer-widget) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness 的会话流「内联可视化」插件：模型产出 SVG / HTML 源码后，交给浏览器渲染成一张可交互的内联卡片，源码只进卡片、不回灌模型上下文。 |
| 1295 | [lovstudio/dsh-llm-config](https://github.com/lovstudio/dsh-llm-config) | 0 | 2026-08-29 | 2026-08-29 | Reusable LLM configuration profile library exposed to browser consumers as a Remote (DeepSeek Harness plugin) |
| 1296 | [lovstudio/dsh-plugin-marketplace](https://github.com/lovstudio/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Local-first DeepSeek Harness plugin marketplace with GitHub and dshfind providers |
| 1297 | [loyalchiiina/dsh-skill-browser](https://github.com/loyalchiiina/dsh-skill-browser) | 0 | 2026-09-04 | 2026-09-04 | DSH skill library browser with floating ball panel, categories, Chinese descriptions, and an automatic skill-failure ledger (tools/result based). DSH 技能浏览器：悬浮球面板 + 分类 + 中文简介 + 技能失效台账自动登记 |
| 1298 | [lrplrplrp/dsh-sidebar-gdhighlight](https://github.com/lrplrplrp/dsh-sidebar-gdhighlight) | 0 | 2026-08-30 | 2026-08-31 | godot语法高亮，依赖dsh-better-sidebar |
| 1299 | [Luawig/dsh-cloudflare-access](https://github.com/Luawig/dsh-cloudflare-access) | 0 | 2026-08-27 | 2026-08-27 | Cloudflare Access JWT verification and remote privileged authorization for DeepSeek Harness |
| 1300 | [Lubaoshuai/dsh-notify](https://github.com/Lubaoshuai/dsh-notify) | 0 | 2026-08-30 | 2026-08-30 | Push notifications for DeepSeek Harness: agent-callable notify_send tool + external delivery for schedule reminders (Telegram/Slack/Discord/飞书/钉钉/Bark/ntfy/webhook). DSH plugin. |
| 1301 | [lucifergzsz414/dsh-windows-native](https://github.com/lucifergzsz414/dsh-windows-native) | 0 | 2026-08-31 | 2026-08-31 | Native-Windows (non-WSL) shell/encoding/filesystem gotchas for the DeepSeek Harness system prompt |
| 1302 | [Luisarg03/dsh-memory-vault](https://github.com/Luisarg03/dsh-memory-vault) | 0 | 2026-08-31 | 2026-09-01 | Memoria OKF persistente para DeepSeek Harness: MCP server (SQLite FTS5 + markdown) + plugins memory-mcp / memory-auto |
| 1303 | [LUMOGRESS/dsh-skill-navigator](https://github.com/LUMOGRESS/dsh-skill-navigator) | 0 | 2026-08-29 | 2026-08-29 | DSH skill quick-picker and manager: one-click quick-pick (categories/search/context recommendations) + management (categories/updates/expert packs/market/panel settings). DSH 技能速查+管理插件。 |
| 1304 | [luoghong/dsh-session-recorder](https://github.com/luoghong/dsh-session-recorder) | 0 | 2026-08-29 | 2026-08-30 | 记录和deek Harness对话记录为md格式 |
| 1305 | [luomeii/dsh-review-squad](https://github.com/luomeii/dsh-review-squad) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 并行多角色代码评审插件：/review 派出安全/正确性/测试/风格四名只读评审员子代理（可各自指定模型与思考强度），汇总为结构化报告。 |
| 1306 | [luoxin10086/dsh-session-doctor](https://github.com/luoxin10086/dsh-session-doctor) | 0 | 2026-09-04 | 2026-09-04 | Session doctor for DeepSeek Harness: scan/repair/watch stored session logs against loader-mirror validation, plus render-contract audit. 会话体检与修复插件。 |
| 1307 | [luoxunhao/dsh-codex-project](https://github.com/luoxunhao/dsh-codex-project) | 0 | 2026-09-02 | 2026-09-04 | codex风格的项目管理，可以给dsh项目增加附加目录，访问附加目录不需要full-access权限，方便多项目开发，可配合dsh-better-sidebar插件使用。 |
| 1308 | [luxi233/dsh-settings-nav-scroll](https://github.com/luxi233/dsh-settings-nav-scroll) | 0 | 2026-09-02 | 2026-09-02 | Adds vertical scrolling to the DSH Web settings navigation when sections exceed the viewport. |
| 1309 | [luxueliu/luxueliu-agent-discipline-skills](https://github.com/luxueliu/luxueliu-agent-discipline-skills) | 0 | 2026-08-25 | 2026-08-27 | AI 不缺聪明，缺纪律！交付前自检（没从磁盘回读不算完成）/跑偏纠偏（一句「你偏了」就停）/系统化调试（同一个修复猜三次不收敛时用）/多 agent 接力（防旧状态盖掉新写入）——4 个单文件技能零依赖，每条都来自真实翻车事故，DeepSeek Harness / Claude Code / Codex 通用 |
| 1310 | [luxueliu/luxueliu-intel-scout](https://github.com/luxueliu/luxueliu-intel-scout) | 0 | 2026-08-25 | 2026-08-27 | 每天自动巡 RSS：AI 简报 + 脑神经/意识简报，关键词过滤后压成速览+详情。DSH 插件；脚本仍是 Python / 计划任务。 |
| 1311 | [luyy9apples/dsh-workspace-memory](https://github.com/luyy9apples/dsh-workspace-memory) | 0 | 2026-08-31 | 2026-09-01 | Approval-gated workspace instructions and shared project memory for DeepSeek Harness |
| 1312 | [lyaoliu/dsh-reasoning-effort-slider](https://github.com/lyaoliu/dsh-reasoning-effort-slider) | 0 | 2026-08-29 | 2026-08-29 | DSH Desktop reasoning effort slider plugin - 7-level effort control with whale-mom skin |
| 1313 | [lylarcher/dsh-model-capabilities](https://github.com/lylarcher/dsh-model-capabilities) | 0 | 2026-08-29 | 2026-08-29 | 一个DSH插件，为自定义模型配置输入类型(input)、推理模式（reasoningEfforts） |
| 1314 | [lyuwen/dsh-as-service](https://github.com/lyuwen/dsh-as-service) | 0 | 2026-08-26 | 2026-08-27 | Running DSH as a service on the background |
| 1315 | [lyuwen/dsh-steer-button](https://github.com/lyuwen/dsh-steer-button) | 0 | 2026-08-26 | 2026-08-27 | Queue, Steer, and Backlog for DSH. More diverse way to interact with the agent while it's running. |
| 1316 | [lyuwen/dsh-thinking-summary](https://github.com/lyuwen/dsh-thinking-summary) | 0 | 2026-08-27 | 2026-08-27 | Readable thinking display for DeepSeek Harness |
| 1317 | [lyuwen/dsh-tui](https://github.com/lyuwen/dsh-tui) | 0 | 2026-08-28 | 2026-08-28 | [WIP] TUI for DeepSeeh-Harness |
| 1318 | [Lzh3070/dsh-search-hub](https://github.com/Lzh3070/dsh-search-hub) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 联网搜索多入口管理插件：DeepSeek 官方 / GLM（智谱）/ Kimi 多搜索模型共存，置顶一个web_search生效，设置页一键切换免重启 |
| 1319 | [LZMW/dsh-memory](https://github.com/LZMW/dsh-memory) | 0 | 2026-08-24 | 2026-08-28 | Persistent long-term memory plugin for DeepSeek Harness (dsh): single memory tool, markdown storage, auto session summary, curator governance, user-profile injection. |
| 1320 | [lzxcs/archive-vault-pro](https://github.com/lzxcs/archive-vault-pro) | 0 | 2026-08-26 | 2026-08-27 | 归档会话库：查看所有工作区的已归档会话、只读回看内容、右键取消归档（不影响官方逻辑）。 |
| 1321 | [lzxcs/btw-pro](https://github.com/lzxcs/btw-pro) | 0 | 2026-08-26 | 2026-08-27 | /btw 旁路问答：不打断当前会话（含流式输出中），基于当前上下文回答一个问题；答案以「旁答」命令结果行显示在主会话里，不进入主模型上下文。 |
| 1322 | [lzxcs/chat-width-pro](https://github.com/lzxcs/chat-width-pro) | 0 | 2026-08-26 | 2026-08-27 | 对话页面宽度设置：把固定的内容宽度暴露到设置页，默认 748px（应用当前宽度）。 |
| 1323 | [lzxcs/dsh-enter-swap](https://github.com/lzxcs/dsh-enter-swap) | 0 | 2026-08-26 | 2026-08-27 | Swap the web UI composer shortcuts: Ctrl/Meta+Enter inserts a newline, Shift+Enter sends. |
| 1324 | [lzxcs/dsh-tray-notify](https://github.com/lzxcs/dsh-tray-notify) | 0 | 2026-08-26 | 2026-08-27 | DSH → 托盘通知：agent 停顿 / 提问 / 计划审批 / 授权时调用 notify-sender.py 弹窗（--source dsh，托盘按蓝色主题区分于 Claude Code）。纯 node 侧插件。 |
| 1325 | [lzxcs/edit-diff-pro](https://github.com/lzxcs/edit-diff-pro) | 0 | 2026-08-26 | 2026-08-27 | Claude Code 风格的 edit/write diff 卡片：±3 行上下文、绝对行号、可配置默认展开（默认折叠）。 |
| 1326 | [lzxcs/file-diff-pro](https://github.com/lzxcs/file-diff-pro) | 0 | 2026-08-26 | 2026-08-27 | 产物文件点击弹窗查看本轮 diff（代码类文件）；非代码文件维持桌面打开。 |
| 1327 | [lzxcs/lag-trace-pro](https://github.com/lzxcs/lag-trace-pro) | 0 | 2026-08-26 | 2026-08-27 | DSH web UI performance recorder: auto-captures page jank (long animation frames, long tasks, frame freezes) with context snapshots, stored under ~/.dsh/perf/ |
| 1328 | [lzxcs/paste-file-path-pro](https://github.com/lzxcs/paste-file-path-pro) | 0 | 2026-08-26 | 2026-08-27 | Pasting non-image files into the web composer inserts their paths as @file references (host-side clipboard reading). |
| 1329 | [m1452700576/dsh-app-updater](https://github.com/m1452700576/dsh-app-updater) | 0 | 2026-08-26 | 2026-09-01 | 更新dsh客户端 |
| 1330 | [Macorreag/dsh-monitor](https://github.com/Macorreag/dsh-monitor) | 0 | 2026-09-02 | 2026-09-02 | Monitor plugin for DeepSeek Harness: background bash watchers that steer the agent loop, with a live dock status bar. |
| 1331 | [maiziman/cedardsh-model-probe](https://github.com/maiziman/cedardsh-model-probe) | 0 | 2026-08-31 | 2026-08-31 | CedarDSH Model Probe — Detects reasoning and image support for custom DeepSeek Harness models. |
| 1332 | [MannixHu/dsh-statusbar-config](https://github.com/MannixHu/dsh-statusbar-config) | 0 | 2026-09-02 | 2026-09-02 | 用 ${变量} 模板完全自定义 DeepSeek Harness 状态栏统计行 · template-driven DSH status bar |
| 1333 | [mapan0424/deepseek-harness-channels](https://github.com/mapan0424/deepseek-harness-channels) | 0 | 2026-08-28 | 2026-08-28 | Community channel plugins for DeepSeek Harness: core, visual config, and Feishu channel. |
| 1334 | [MarceloSenai/dsh-plugin-kie-ai](https://github.com/MarceloSenai/dsh-plugin-kie-ai) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: image and video generation over the KIE AI API |
| 1335 | [marcemira/dsh-theme-nier-automata](https://github.com/marcemira/dsh-theme-nier-automata) | 0 | 2026-09-03 | 2026-09-04 | NieR:Automata-inspired YoRHa theme for DeepSeek Harness web |
| 1336 | [MarchLiu/dsh-farm](https://github.com/MarchLiu/dsh-farm) | 0 | 2026-09-02 | 2026-09-02 | DSH service farm: register, start, stop, restart and watch long-running project services — agent tools + overview drawer UI, farm.yaml support |
| 1337 | [MarchLiu/dsh-uno-office](https://github.com/MarchLiu/dsh-uno-office) | 0 | 2026-09-02 | 2026-09-02 | LibreOffice (UNO) powered high-fidelity office engine for DSH — create & edit docx/xlsx/pptx via prompts, with human-in-the-loop review |
| 1338 | [MaRi23333/dsh-serverchan-watchdog](https://github.com/MaRi23333/dsh-serverchan-watchdog) | 0 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 的 Server酱推送插件：审批、计划评审或问答超时未处理时，发送微信/Server酱³ App 提醒。第三方非官方项目。 |
| 1339 | [markelayan/dsh-taskboard-flow](https://github.com/markelayan/dsh-taskboard-flow) | 0 | 2026-08-31 | 2026-09-01 | Companion plugin to dsh-taskboard (DeepSeek Harness): kanban flow engine + cross-session messaging. File-based config, local-only, no telemetry. |
| 1340 | [masknull/dsh-message-collapse](https://github.com/masknull/dsh-message-collapse) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin: auto-collapse long user messages in the web chat. 用户消息超10行自动折叠。 |
| 1341 | [masknull/dsh-webhook-notifier](https://github.com/masknull/dsh-webhook-notifier) | 0 | 2026-09-03 | 2026-09-03 | DSH 事件通知插件：AI 回合完成、权限申请、提问、出错、开始运行等 5 种场景发生时，向 Webhook 发送自定义 HTTP 通知，支持 GET/POST、预设字段/自定义文本、type+type_cn、发送日志 |
| 1342 | [masknull/dsh-workspace-default-path](https://github.com/masknull/dsh-workspace-default-path) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：添加工作区时记住上次使用的目录，下次打开浏览对话框直接定位（预填+自动记忆，官方流程不动）。DSH plugin: remember the last used workspace directory for Add workspace - prefill + auto-memory over the official flow. |
| 1343 | [Mason-1011/dsh-schematic](https://github.com/Mason-1011/dsh-schematic) | 0 | 2026-08-25 | 2026-08-30 | Live plugin-topology viewer for DeepSeek Harness — the wiring diagram of mounted plugins, their runtime activity, and a composer-side star map. Pure observer. |
| 1344 | [MasterBenC/shangshi-dsh](https://github.com/MasterBenC/shangshi-dsh) | 0 | 2026-08-31 | 2026-08-31 | Shangshi DeepSeek Harness plugin for local Qimen business timing. |
| 1345 | [MauricioPerera/kdd-gates](https://github.com/MauricioPerera/kdd-gates) | 0 | 2026-08-27 | 2026-08-27 | KDD methodology gates as DeepSeek Harness (dsh) plugin tools |
| 1346 | [mc856/dsh-project-portfolio](https://github.com/mc856/dsh-project-portfolio) | 0 | 2026-08-31 | 2026-08-31 | Unofficial DSH plugin: long-term, cross-project memory for coding agents — embedded project-portfolio skill + portfolio_status/portfolio_log tools over plain markdown. Not affiliated with DeepSeek. |
| 1347 | [me9rez/dsh-pwsh-style](https://github.com/me9rez/dsh-pwsh-style) | 0 | 2026-08-28 | 2026-08-28 | 修改 DSH 会话回复中 pwsh(PowerShell) 工具卡片的主题、字体与可读性增强。Restyle pwsh tool-call cards in DSH: themes, system fonts, copy & expand, workdir display. |
| 1348 | [mengruoa/dsh-rembg](https://github.com/mengruoa/dsh-rembg) | 0 | 2026-08-21 | 2026-09-01 | DSH plugin: auto-install rembg and expose a background-removal tool to the LLM |
| 1349 | [Mengshang-spec/dsh-third-party-api-balance-wallet](https://github.com/Mengshang-spec/dsh-third-party-api-balance-wallet) | 0 | 2026-08-27 | 2026-08-27 | 第三方 API 接入 DSH 查询余额插件 |
| 1350 | [mervin1944/dsh-version-badge](https://github.com/mervin1944/dsh-version-badge) | 0 | 2026-08-31 | 2026-08-31 | DSH 版本号徽标插件：侧边栏设置按钮上方显示 dsh 版本，带检查更新与一键部署。DSH version badge plugin with update check & one-click deploy. |
| 1351 | [metabolism-tools/workspace-metabolism](https://github.com/metabolism-tools/workspace-metabolism) | 0 | 2026-08-15 | 2026-08-31 | Govern what Claude Code, Codex, Aider and OpenClaw leave in your workspace: one JSON policy file, audit, recyclable clean, rollback, hash-chained audit trail. |
| 1352 | [meyaomiao/dsh-files-native](https://github.com/meyaomiao/dsh-files-native) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件：接近原生质感的附件上传（拖入/粘贴/回形针，图片与文件混排） |
| 1353 | [MichaelGong/dsh-session-hover-preview](https://github.com/MichaelGong/dsh-session-hover-preview) | 0 | 2026-08-27 | 2026-08-27 | Codex-style user-message navigation for DeepSeek Harness conversations |
| 1354 | [Mide69/dsh-boot-doctor](https://github.com/Mide69/dsh-boot-doctor) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: console log sink and stuck-plugin warnings |
| 1355 | [mikijiyun/dsh-token-rush](https://github.com/mikijiyun/dsh-token-rush) | 0 | 2026-09-03 | 2026-09-03 | DSH Web GUI 悬浮仪表：实时 token 消耗 / 估算金额 / 账户余额，高峰时段自动变橙红色。A floating token / cost / balance HUD that turns orange-red during DeepSeek rush hours. |
| 1356 | [Milbaxter/dsh-critique-loop](https://github.com/Milbaxter/dsh-critique-loop) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: forces one critique-and-improve round after each completed turn. |
| 1357 | [minatoAI/dsh-net-proxy-plugin](https://github.com/minatoAI/dsh-net-proxy-plugin) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness fallback network proxy plugin: detects system proxies, probes overseas connectivity (Google/GitHub), routes dsh outbound HTTP through a working local proxy |
| 1358 | [mingzhong15/dsh-cursor-passthrough](https://github.com/mingzhong15/dsh-cursor-passthrough) | 0 | 2026-08-27 | 2026-08-27 | Add a Cursor passthrough group to the DSH chat model picker. |
| 1359 | [Missher12/dsh-project-ops](https://github.com/Missher12/dsh-project-ops) | 0 | 2026-08-27 | 2026-08-27 | Scoped project task discovery and execution receipts for DeepSeek Harness |
| 1360 | [ml020/dsh-workbuddy](https://github.com/ml020/dsh-workbuddy) | 0 | 2026-08-28 | 2026-08-28 | Wordless-styled WorkBuddy hero for DSH: replaces the blank-session brand mark and workspace picker while keeping the native composer. |
| 1361 | [mnbvcxzaqwertyuioplm/dsh-memory](https://github.com/mnbvcxzaqwertyuioplm/dsh-memory) | 0 | 2026-09-01 | 2026-09-01 | DSH 跨会话语义记忆插件：智谱 embedding-3 + SQLite，提供 memory_add / memory_search 语义召回；配置可选、绝不因缺 key/缺库/缺服务而崩。 |
| 1362 | [mohith-das/dsh-client-ui-model-selection-search](https://github.com/mohith-das/dsh-client-ui-model-selection-search) | 0 | 2026-09-01 | 2026-09-01 | Fork of DeepSeek Harness's official model picker (@deepseek-ai/dsh-client-ui-model-selection) adding an in-menu search box to filter models by name, provider, or id. |
| 1363 | [mohith-das/dsh-voice-input-en](https://github.com/mohith-das/dsh-voice-input-en) | 0 | 2026-09-01 | 2026-09-01 | Minimal, English-only voice input plugin for DeepSeek Harness Web UI — a mic button in the composer using the browser's native SpeechRecognition API. Zero dependencies, no subprocess, no tracking. |
| 1364 | [mokuyoaxis/dsh-iris](https://github.com/mokuyoaxis/dsh-iris) | 0 | 2026-09-04 | 2026-09-04 | Media generation and visual understanding for DeepSeek Harness, with multi-provider routing and the integrated Iris workbench. |
| 1365 | [Momojie-S/dsh-archive-retention](https://github.com/Momojie-S/dsh-archive-retention) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件: 归档会话定期清理 —— 物理归档堆与页面归档会话超保留期(页面可配天/小时,cron 调度)自动物理删除 |
| 1366 | [Momojie-S/dsh-subagent-steer](https://github.com/Momojie-S/dsh-subagent-steer) | 0 | 2026-09-04 | 2026-09-04 | DSH plugin: steer_subagent - insert a new instruction into a running background subagent's current turn (step-boundary steering) or hard-restart its turn; send_message queueing stays the default |
| 1367 | [moonwellxh/DSH-Launcher](https://github.com/moonwellxh/DSH-Launcher) | 0 | 2026-08-27 | 2026-08-30 | DSH 魔偶助手（DSH一键启动托盘）(DeepSeek Harness launcher / tray) |
| 1368 | [MoriTang/dsh-plugins](https://github.com/MoriTang/dsh-plugins) | 0 | 2026-08-22 | 2026-09-03 | A collection of my DeepSeek Harness plugins. |
| 1369 | [morlay/dsh-llm-openai-compatible](https://github.com/morlay/dsh-llm-openai-compatible) | 0 | 2026-08-20 | 2026-09-03 | moved https://github.com/morlay/better-session/tree/main/packages/llm-openai-compatible |
| 1370 | [morphlinglan/dsh-leopard-gecko](https://github.com/morphlinglan/dsh-leopard-gecko) | 0 | 2026-08-28 | 2026-08-28 | 豹纹守宫旅行桌宠小插件：一只会自己出门旅行、寄回明信片、带回特产的守宫。庭院三叶草随时间生长，收割后可在商店购买便当与护身符。 |
| 1371 | [mrme000m/dsh-prime-orchestrator](https://github.com/mrme000m/dsh-prime-orchestrator) | 0 | 2026-09-01 | 2026-09-02 | Prime Agent orchestration for DeepSeek Harness (dsh): delegation engine, prime_agent tool, Web fleet column, settings section, and the prime-orchestrator agent preset — one installable plugin package |
| 1372 | [MST19711/dsh-balance-panel](https://github.com/MST19711/dsh-balance-panel) | 0 | 2026-08-21 | 2026-09-02 | Floating Balance Panel for the DSH Web UI — live remaining % for the 5h / weekly / monthly windows, supporting OpenCode Go and Z.AI-CN |
| 1373 | [MST19711/dsh-session-files](https://github.com/MST19711/dsh-session-files) | 0 | 2026-08-31 | 2026-09-01 | Upload arbitrary files into a DSH session workspace (uploads/<sessionId>/) and let the agent deliver result files as clickable download cards in the conversation. |
| 1374 | [mtdx2001/dsh-think-translate](https://github.com/mtdx2001/dsh-think-translate) | 0 | 2026-08-29 | 2026-08-29 | Display-layer translation for the DeepSeek Harness Web UI: thinking chain, task cards and answers in 8 languages - pure display layer, originals untouched, local-first with failover. |
| 1375 | [my-dsh/dsh-session-attention](https://github.com/my-dsh/dsh-session-attention) | 0 | 2026-08-28 | 2026-08-28 | Session attention overlay plugin for DeepSeek Harness: character dance animation while any session awaits user action |
| 1376 | [my-dsh/dsh-token-usage-dashboard](https://github.com/my-dsh/dsh-token-usage-dashboard) | 0 | 2026-08-28 | 2026-08-28 | Cross-session token usage dashboard plugin for DeepSeek Harness: SQLite-backed capture + browser dashboard panel |
| 1377 | [mycodesite/dsh-rules](https://github.com/mycodesite/dsh-rules) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (dsh) 插件：全局+项目两级 Markdown 规则注入（RuleBase） |
| 1378 | [myk5010/dsh-kimi](https://github.com/myk5010/dsh-kimi) | 0 | 2026-09-02 | 2026-09-02 | Kimi (Kimi Code account) integration bundle for DeepSeek Harness: provider route, models, device-code login and auto token refresh |
| 1379 | [mykeura/dsh-minimalist-themes](https://github.com/mykeura/dsh-minimalist-themes) | 0 | 2026-08-26 | 2026-08-27 | 18 minimalist color themes for DeepSeek Harness. Pick one with a single click — it's just another plugin. |
| 1380 | [n8guru/dsh-self-preserve](https://github.com/n8guru/dsh-self-preserve) | 0 | 2026-09-02 | 2026-09-02 | DSH hook plugin: a session may not stop the harness it runs inside |
| 1381 | [naitoupi/prompt-optimizer-plugin](https://github.com/naitoupi/prompt-optimizer-plugin) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness (DSH) plugin: ? optimize the composer draft with the current model. Installable bundle (dsh.bundle + dsh.client); Settings tab: on/off switch, generation params, editable system prompt with reset-to-default. |
| 1382 | [nataliwhite20534-droid/dsh-moe-plugin](https://github.com/nataliwhite20534-droid/dsh-moe-plugin) | 0 | 2026-09-03 | 2026-09-03 | 10 preset moe character cards for DSH - freely combinable, editable, persistable. Real outputs in docs/usage-examples.md. |
| 1383 | [nateEc/dsh-gitLens](https://github.com/nateEc/dsh-gitLens) | 0 | 2026-08-26 | 2026-09-03 | Workspace-scoped Git graph and guarded Git workbench for DeepSeek Harness. |
| 1384 | [NattoCB/dsh-plugin-sidebar-views](https://github.com/NattoCB/dsh-plugin-sidebar-views) | 0 | 2026-08-31 | 2026-08-31 | Sidebar views switcher for DeepSeek Harness: workspaces / recent sessions, pinned sessions group, per-row pin & copy-session-id menu |
| 1385 | [NattoCB/dsh-safe-delete](https://github.com/NattoCB/dsh-safe-delete) | 0 | 2026-09-01 | 2026-09-01 | DSH plugin: intercept agent rm in every bash session and move targets to the macOS Trash instead |
| 1386 | [navid-kianfar/dsh-memory](https://github.com/navid-kianfar/dsh-memory) | 0 | 2026-08-26 | 2026-08-27 | Persistent, searchable, per-project memory for the DeepSeek Harness: decisions, rules, and session context in a queryable DuckDB file, with the rule set injected into every model request — plus a full management UI in the Web Client. |
| 1387 | [navid-kianfar/dsh-worktree](https://github.com/navid-kianfar/dsh-worktree) | 0 | 2026-08-26 | 2026-08-27 | Git worktrees and branches for the DeepSeek Harness Web Client: a session-header chip that switches branches, creates worktrees, and opens them as harness workspaces. |
| 1388 | [NecromanAlbert/dsh-i-have-adhd](https://github.com/NecromanAlbert/dsh-i-have-adhd) | 0 | 2026-08-26 | 2026-08-27 | Always-on ADHD-friendly output for every DeepSeek Harness session. Host systemPrompt, not a skill catalog item. |
| 1389 | [NecromanAlbert/dsh-self-restart](https://github.com/NecromanAlbert/dsh-self-restart) | 0 | 2026-08-26 | 2026-08-27 | Any DSH session can request a Desktop restart, then the same persisted session is resumed and followup'd with its mission. |
| 1390 | [NexusAgentX/dsh-advisor](https://github.com/NexusAgentX/dsh-advisor) | 0 | 2026-08-23 | 2026-08-27 | dsh plugin bundle porting the rpiv advisor subsystem: an on-demand zero-parameter advisor() tool that forwards the full session to a separately-configured reviewer model. |
| 1391 | [nicecx/dsh-auto-approver](https://github.com/nicecx/dsh-auto-approver) | 0 | 2026-08-31 | 2026-08-31 | Configurable auto-approval for DeepSeek Harness: intercepts approval/request and answers allowed-once/rejected by policy (allow-all/allowlist/off + denyAlways), with a full audit log. |
| 1392 | [nicecx/dsh-reset-handoff](https://github.com/nicecx/dsh-reset-handoff) | 0 | 2026-08-30 | 2026-08-30 | DSH never restarts itself: host plugin that hands reset requests to an external ops agent (e.g. Hermes) via a versioned JSON protocol — preflight → gate → restart → health-check → recover → deliver back |
| 1393 | [nicecx/dsh-task-queue](https://github.com/nicecx/dsh-task-queue) | 0 | 2026-08-31 | 2026-08-31 | Tiered task queue for DSH↔Hermes: queue.json single source of truth, lease/claim model, concurrency-1; Hermes-side cron consumes, DSH-side enqueues. Includes busy-mutex for the approve fast path. |
| 1394 | [nickkkkkk123123/dsh-resume-on-restart](https://github.com/nickkkkkk123123/dsh-resume-on-restart) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：重启后自动唤醒 agent 并投递信息性消息，agent 自主决定是否恢复工作 |
| 1395 | [ningbonb/dsh-installer](https://github.com/ningbonb/dsh-installer) | 0 | 2026-08-31 | 2026-09-01 | One-click installers for DeepSeek Harness (dsh) on macOS and Windows |
| 1396 | [NinjaSln-labs/dsh-context-compass](https://github.com/NinjaSln-labs/dsh-context-compass) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness 会话健康插件：真实数据的「继续 vs 新开」上下文罗盘——头部徽章 / /compass / context_compass 工具 / 多会话一览面板 |
| 1397 | [NinjaSln-labs/dsh-imgdraw](https://github.com/NinjaSln-labs/dsh-imgdraw) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 文生图插件：draw_image 模型工具 + 输入框生图按钮（异步生成/4 格网格/下载保留删除）+ /imgdraw 路由 + 持久化历史。Text-to-image for DeepSeek Harness. |
| 1398 | [NinjaSln-labs/dsh-knowledge-sqlite](https://github.com/NinjaSln-labs/dsh-knowledge-sqlite) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 跨会话知识插件：ctx.knowledge 服务 + knowledge_* 工具，SQLite FTS5 trigram 中文子串检索 + L1 查询扩展（V1.11 契约） |
| 1399 | [NinjaSln-labs/dsh-session-slm-router](https://github.com/NinjaSln-labs/dsh-session-slm-router) | 0 | 2026-09-02 | 2026-09-03 | Shadow-mode SLM router for DeepSeek Harness: per-turn weak/strong prediction via vertical-small-model CLI, writes shadow JSONL log |
| 1400 | [NinjaSln-labs/dsh-subagent-cursor](https://github.com/NinjaSln-labs/dsh-subagent-cursor) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 插件：Cursor-as-subagent 提供方——一次本地 @cursor/sdk one-shot 运行、摘要优先结果、可无人值守的 Profile Bundle |
| 1401 | [NinjaSln-labs/dsh-subagent-router](https://github.com/NinjaSln-labs/dsh-subagent-router) | 0 | 2026-09-02 | 2026-09-03 | DeepSeek Harness 子代理模型路由插件：subagent_model 工具 + model:"auto" 路由策略（任务档位/失败升级/可审计），子代理不再继承父模型。Model-routed subagent delegation for DeepSeek Harness. |
| 1402 | [nishuoyang/dsh-workbench-ecs](https://github.com/nishuoyang/dsh-workbench-ecs) | 0 | 2026-09-04 | 2026-09-04 | Alibaba Cloud Workbench CLI plugin — lets DeepSeek Harness's Agent directly control remote ECS instances. |
| 1403 | [niushuanan/dsh-adaptive-update](https://github.com/niushuanan/dsh-adaptive-update) | 0 | 2026-08-26 | 2026-08-27 | Check upstream manually or every six hours, use a narrowly scoped agent for compatibility work, and switch atomically with rollback. |
| 1404 | [niushuanan/dsh-chat-migration](https://github.com/niushuanan/dsh-chat-migration) | 0 | 2026-08-29 | 2026-08-29 | Native DeepSeek chat migration and workspace-free chat mode for DeepSeek Harness |
| 1405 | [niushuanan/dsh-image-vision](https://github.com/niushuanan/dsh-image-vision) | 0 | 2026-08-26 | 2026-08-27 | Let vision-capable models read native attachments while giving text-only models an image tool that supports follow-up questions. |
| 1406 | [niushuanan/dsh-model-usage](https://github.com/niushuanan/dsh-model-usage) | 0 | 2026-08-26 | 2026-08-27 | Inspect model quotas, periods, and refresh state by provider in Settings, with data loaded only when the user opens the page. |
| 1407 | [niushuanan/dsh-multi-window](https://github.com/niushuanan/dsh-multi-window) | 0 | 2026-08-26 | 2026-08-27 | Open multiple independent conversations side by side, each with isolated navigation, drafts, and runtime state. |
| 1408 | [niushuanan/dsh-parallel-worktree](https://github.com/niushuanan/dsh-parallel-worktree) | 0 | 2026-08-26 | 2026-08-27 | Move parallel tasks into isolated Git worktrees, inspect conflicts, and merge the results safely into the current branch. |
| 1409 | [niushuanan/dsh-pure-chat](https://github.com/niushuanan/dsh-pure-chat) | 0 | 2026-08-26 | 2026-08-27 | Start a chat immediately without a workspace, work mode, or execution permissions while keeping image and text-file uploads. |
| 1410 | [niushuanan/dsh-selection-memory](https://github.com/niushuanan/dsh-selection-memory) | 0 | 2026-08-26 | 2026-08-27 | Quote, discuss, or remember selected conversation text, then maintain durable context in separate editable user and AI memories. |
| 1411 | [niushuanan/dsh-skill-manager](https://github.com/niushuanan/dsh-skill-manager) | 0 | 2026-08-26 | 2026-08-27 | Browse installed Skills, their files, and content in Settings, then adaptively import from a file, folder, ZIP, or GitHub with AI. |
| 1412 | [niushuanan/dsh-teamwork](https://github.com/niushuanan/dsh-teamwork) | 0 | 2026-08-26 | 2026-08-27 | Run collaborating agents and external experts concurrently under one coordinating agent, then bring every result back into the current task. |
| 1413 | [niushuanan/dsh-token-overview](https://github.com/niushuanan/dsh-token-overview) | 0 | 2026-08-26 | 2026-08-27 | See tokens, cache usage, calls, active periods, and estimated cost across AI clients on the whole computer. |
| 1414 | [niushuanan/dsh-whale-girl](https://github.com/niushuanan/dsh-whale-girl) | 0 | 2026-08-26 | 2026-08-27 | Add a native cross-page companion whose presence, shortcuts, and feedback follow the current DSH session state. |
| 1415 | [njuptlzf/dsh-ponytail](https://github.com/njuptlzf/dsh-ponytail) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 插件：常驻注入 Ponytail 懒高级工程师规范，5 个同伴技能落盘为可调用的 skill。安装：dsh plugin add github:njuptlzf/dsh-ponytail |
| 1416 | [nmsl1234/dsh-privacy-gate](https://github.com/nmsl1234/dsh-privacy-gate) | 0 | 2026-08-31 | 2026-08-31 | dsh-plugin |
| 1417 | [NoelJudeNoel/dshost-plugin](https://github.com/NoelJudeNoel/dshost-plugin) | 0 | 2026-09-01 | 2026-09-01 | Official remote cloud relay plugin for DSHost (dshost.me): securely access your dsh Web UI from anywhere |
| 1418 | [NOirBRight/dsh-llm-providers-ui](https://github.com/NOirBRight/dsh-llm-providers-ui) | 0 | 2026-08-30 | 2026-09-03 | Shared LLM Providers settings shell, card order, and picker sort for DeepSeek Harness plugins |
| 1419 | [NOirBRight/dsh-mobile-pairing](https://github.com/NOirBRight/dsh-mobile-pairing) | 0 | 2026-08-21 | 2026-08-29 | DSH Mobile Remote pairing plugin |
| 1420 | [NOirBRight/dsh-plugins](https://github.com/NOirBRight/dsh-plugins) | 0 | 2026-08-29 | 2026-08-30 | Independent catalog of DSH plugins and mobile companion published by NOirBRight |
| 1421 | [northern-penguin/dsh-h3-seg-prompt-design](https://github.com/northern-penguin/dsh-h3-seg-prompt-design) | 0 | 2026-09-02 | 2026-09-02 | 一个DeepSeekHarness插件，用于让模型在DeepSeekHarness中生成符合H3视频生成模型规范的提示词。该提示词可以直接用于Theodore_Director导播台的分镜设计中。 |
| 1422 | [Nth-5620/dsh-crystal-viewer](https://github.com/Nth-5620/dsh-crystal-viewer) | 0 | 2026-08-29 | 2026-08-30 | A crystal-structure visualization window for DeepSeek Harness: 3D structure + Q-peak viewer and parameter panel, opened as a dsh-better-sidebar tab. |
| 1423 | [null-object-0000/dsh-output-style](https://github.com/null-object-0000/dsh-output-style) | 0 | 2026-08-31 | 2026-08-31 | 会话级输出风格插件：/style 命令 + Web 选择器，改变模型如何呈现答案（default/adhd-friendly/eli5/bluf）。Session-scoped output styles for DeepSeek Harness. |
| 1424 | [NyaaCaster/dsh-yuque-kb](https://github.com/NyaaCaster/dsh-yuque-kb) | 0 | 2026-08-24 | 2026-08-28 | dsh web插件，语雀文档知识库化在dsh中调用 |
| 1425 | [odelbos/dsh-models-filter](https://github.com/odelbos/dsh-models-filter) | 0 | 2026-08-29 | 2026-08-31 | DeepSeek Harness plugin used to add an input filed to filter the models menu. (with arrow up/down + enter) |
| 1426 | [oh-summy/dsh-remote-control](https://github.com/oh-summy/dsh-remote-control) | 0 | 2026-08-30 | 2026-08-30 | Secure remote access for DeepSeek Harness (DSH): Cloudflare Tunnel + password gate + Feishu notifications. macOS first, Linux first-class. |
| 1427 | [Oissp/harness-desktop](https://github.com/Oissp/harness-desktop) | 0 | 2026-08-26 | 2026-09-02 | DeepSeek Harness Desktop for Debian |
| 1428 | [Olina1Ye/internal-skill-workshop-plugin](https://github.com/Olina1Ye/internal-skill-workshop-plugin) | 0 | 2026-08-27 | 2026-08-27 | A read-only DeepSeek Harness Web plugin for browsing a configured Skill Base catalog. |
| 1429 | [Oliver0804/dsh-openrouter-monitor](https://github.com/Oliver0804/dsh-openrouter-monitor) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: OpenRouter account balance, per-key spend, alert thresholds and trend charts under the composer. |
| 1430 | [Oliver0804/dsh-peak-pricing](https://github.com/Oliver0804/dsh-peak-pricing) | 0 | 2026-08-17 | 2026-08-27 | DSH plugin: DeepSeek peak/off-peak pricing, flat rates for other providers like z-ai/glm-5.3-flash, live per-session cost estimate and a hover cache-hit trend chart. |
| 1431 | [Olympianz/dsh-deploy-master](https://github.com/Olympianz/dsh-deploy-master) | 0 | 2026-08-30 | 2026-08-30 | A DSH deploy-assistant plugin: GitHub publish + Linear sync + npm publish + community announcement. |
| 1432 | [Olympianz/dsh-heatmap](https://github.com/Olympianz/dsh-heatmap) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 页面埋点与热力图分析插件：科学埋点采集、本地热力图与统计、CLI/HTTP 接口、上传授权。 |
| 1433 | [onclaw-dev/dsh-ima-copilot](https://github.com/onclaw-dev/dsh-ima-copilot) | 0 | 2026-08-30 | 2026-08-30 | 腾讯 IMA 是一个非常好的知识库应用，但是他们提供的skill版本针对公开知识库的检索方式只提供了基于文件标题的关键字检索，好一阵无语。为了补足在harness的这种知识库检索能力，基于tencent-ima-copilot-mcp迭代了对应的dsh版本。 |
| 1434 | [onclaw-dev/dsh-workflow-designer](https://github.com/onclaw-dev/dsh-workflow-designer) | 0 | 2026-08-31 | 2026-08-31 | `dsh-workflow-designer` 是面向 DeepSeek Harness 的提示词优先工作流设计插件。它收集当前 Agent 可见的本地 Skill、原生 Tool 与 MCP Tool，提供必要的可视化编排和约束编辑能力，并导出稳定的 YAML 中间表示。后续可由大模型及对应框架把 YAML 生成 Python、`workflow.mjs` 或其他代码工作流。 |
| 1435 | [Oscar-Williams/dsh-deepcanary](https://github.com/Oscar-Williams/dsh-deepcanary) | 0 | 2026-08-29 | 2026-08-30 | Local attention supervision for DeepSeek Harness: evidence-first signals, quiet notifications, and an actionable inbox. |
| 1436 | [oThTJx/dsh-always-apply](https://github.com/oThTJx/dsh-always-apply) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: injects alwaysApply-marked skill bodies into sessions before the first model request — no skill tool load needed. |
| 1437 | [oThTJx/dsh-superpowers](https://github.com/oThTJx/dsh-superpowers) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: obra/superpowers skill library adapted to dsh tooling, plus a session-start bootstrap — brainstorming, systematic debugging, TDD, planning and more. |
| 1438 | [oxlyn/dsh-flyout-sidebar](https://github.com/oxlyn/dsh-flyout-sidebar) | 0 | 2026-08-29 | 2026-09-02 | deepseek harness flyout sidebar |
| 1439 | [pacoyi/dsh-memory-lite](https://github.com/pacoyi/dsh-memory-lite) | 0 | 2026-08-28 | 2026-08-28 | Lightweight cross-session memory plugin for DeepSeek Harness: approval-gated `memory` tool (save/recall/list/forget) + Settings card UI to browse, add, delete (two-click, trash/restore) and idempotent import/export. \| DeepSeek Harness 跨会话记忆插件：审批门控 memory 工具 + 设置页UI「记忆库」卡片（查看/新增/删除、两击确认、回收站恢复、导入/导出记忆——幂等迁移、冲突拒绝）。 |
| 1440 | [PaidaxingTuT/dsh-code-runner](https://github.com/PaidaxingTuT/dsh-code-runner) | 0 | 2026-08-29 | 2026-08-29 | 在 DSH-better-sidebar 中一键运行侧边栏代码文件，让代码可以在dsh终端中运行 |
| 1441 | [Parker-xia/dsh-research-refs](https://github.com/Parker-xia/dsh-research-refs) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: tidy messy pasted citations into uniformly formatted references (refs_parse / refs_verify / refs_dedup / refs_format + research-refs skill) |
| 1442 | [pauloapoloni/dsh-pr-checks](https://github.com/pauloapoloni/dsh-pr-checks) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: status and progress of GitHub Actions checks for open PRs, in the sidebar footer. |
| 1443 | [pbwheel/dsh-agency-market](https://github.com/pbwheel/dsh-agency-market) | 0 | 2026-09-01 | 2026-09-01 | 把 agency-agents 中的 273 个专业智能体装进 DeepSeek Harness，类似 workbuddy 中的专家 |
| 1444 | [peikuo/dayreel](https://github.com/peikuo/dayreel) | 0 | 2026-08-30 | 2026-08-30 | Dayreel — a DeepSeek Harness (dsh) community plugin: turn your day of work sessions into a designed daily report + a narrated summary video. |
| 1445 | [peiyucn/dsh-sparrow](https://github.com/peiyucn/dsh-sparrow) | 0 | 2026-08-30 | 2026-08-30 | A collection of small DeepSeek Harness (DSH) web plugins: chat input suggestions, an image-vision channel for text-only models, and archived-session management. |
| 1446 | [peng2048/rein-scene-forge-dsh-plugin](https://github.com/peng2048/rein-scene-forge-dsh-plugin) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness plugin for Rein Scene Forge robot scene authoring |
| 1447 | [perinchiang/dsh-memory-dashboard](https://github.com/perinchiang/dsh-memory-dashboard) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness embedded read-only viewer for TencentDB Agent Memory's four-layer local memory |
| 1448 | [PerryLink/dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) | 0 | 2026-08-29 | 2026-08-30 | Community certification spec and registry for DeepSeek Harness plugins: five machine-checkable dimensions, A-D grades, and a security veto. |
| 1449 | [PerryLink/dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) | 0 | 2026-08-26 | 2026-08-27 | Shared zero-runtime-dependency toolkit for PerryLink DSH plugins: a pluggable Provider registry seam, fail-closed approval and adaptive session-event gates, mechanical verify scripts, shared sanitize/pricing/judge modules, and a new-plugin skeleton. |
| 1450 | [PerryLink/dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | 0 | 2026-08-26 | 2026-08-27 | Zero-dependency static portal rendering the @perrylink DeepSeek Harness plugin ecosystem as grouped cards: one page, no build step, no runtime framework. |
| 1451 | [PerryLink/dsh-reach](https://github.com/PerryLink/dsh-reach) | 0 | 2026-09-03 | 2026-09-03 | Multi-channel decision & remote-control bridge for DeepSeek Harness: pushes any workspace's approval/question cards to IM channels (WeChat iLink first) and answers them from chat, with a session console, per-channel security, and an open push service. |
| 1452 | [PerryLink/dsh-ticktick](https://github.com/PerryLink/dsh-ticktick) | 0 | 2026-09-03 | 2026-09-03 | TickTick (Dida365) task bridge for DeepSeek Harness: Session-header task panel (list filter, undone/completed views, search, drag reorder), 11 curated agent tools, settings card, over the official TickTick MCP endpoint. |
| 1453 | [PerryLink/perrylink](https://github.com/PerryLink/perrylink) | 0 | 2026-08-16 | 2026-08-30 | DeepSeek Harness ecosystem: 34 plugins - second-model approval, permission rules, memory, MCP panel, supply-chain security & certification; DSH Desktop Market catalog source |
| 1454 | [phungthien269/dsh-token-stats](https://github.com/phungthien269/dsh-token-stats) | 0 | 2026-09-01 | 2026-09-02 | Token usage dashboard for the DeepSeek Harness web GUI - today/week/month totals, per-model breakdown, 4-language UI. Read-only over the Wallet ledger. |
| 1455 | [Physicolor/dsh-lifeline](https://github.com/Physicolor/dsh-lifeline) | 0 | 2026-09-01 | 2026-09-02 | Right-side message navigation rail for DeepSeek Harness — per-message ticks, hover preview, smooth jump, star bookmarks, realtime slide animation |
| 1456 | [Pidan-Workshop/dsh-godot-play](https://github.com/Pidan-Workshop/dsh-godot-play) | 0 | 2026-09-03 | 2026-09-03 | 在 DSH Web GUI 一键构建并试玩 Godot Web 导出。Build & play Godot Web exports in the DeepSeek Harness GUI with one click. |
| 1457 | [ping1999/dsh-minimap](https://github.com/ping1999/dsh-minimap) | 0 | 2026-08-29 | 2026-08-29 | VS Code-style minimap (text thumbnail + draggable viewport) overlay for the dsh web GUI's side file viewer |
| 1458 | [pipipigu/dsh-ssh-control](https://github.com/pipipigu/dsh-ssh-control) | 0 | 2026-08-28 | 2026-08-28 | Unified, non-intrusive SSH control center for DeepSeek Harness (DSH) |
| 1459 | [pixellover1433/dsh-plugin-dev-skills](https://github.com/pixellover1433/dsh-plugin-dev-skills) | 0 | 2026-08-30 | 2026-08-30 | This set of skills allows your agent to create plugins for Deepseek Harness. |
| 1460 | [plumbkit/dsh-plumb-identity](https://github.com/plumbkit/dsh-plumb-identity) | 0 | 2026-09-01 | 2026-09-02 | Per-agent plumb session identity for DeepSeek Harness: every conversation, workspace, and subagent gets its own stable plumb session id on a shared plumb MCP connection |
| 1461 | [PlusQi/dsh-plugins](https://github.com/PlusQi/dsh-plugins) | 0 | 2026-08-28 | 2026-08-27 | 个人 DeepSeek Harness (DSH) 插件集 |
| 1462 | [pn1024/dsh-skill-hub](https://github.com/pn1024/dsh-skill-hub) | 0 | 2026-09-01 | 2026-09-01 | dsh plugin - skill marketplace (SkillHub + ClawHub) with sidebar entry, overlay panel, and chat input quick-pick |
| 1463 | [PolinniZhong/dsh-skill-trace](https://github.com/PolinniZhong/dsh-skill-trace) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Skill 追踪：看清 Agent 实际加载的 Skill，把运行过程变成可复看、可学习的本地收据。 |
| 1464 | [pricklywiggles/dsh-circuit-breaker](https://github.com/pricklywiggles/dsh-circuit-breaker) | 0 | 2026-09-02 | 2026-09-02 | Loop guard for DeepSeek Harness: denies repeated identical tool calls and caps per-agent calls, outside the model where instructions cannot reach |
| 1465 | [Proton1917/dsh-harness-plugin](https://github.com/Proton1917/dsh-harness-plugin) | 0 | 2026-08-17 | 2026-08-28 | Independent TypeScript plugins for DeepSeek Harness: live stats, Web UI customization, and a medical Fable mode |
| 1466 | [psenY/gh-watch](https://github.com/psenY/gh-watch) | 0 | 2026-09-02 | 2026-09-03 | DSH 插件：GitHub PR/issue 变更监视插件（多 AI 独立配置，插件自身不审查、不回帖） |
| 1467 | [publieople/dsh-omniroute-models](https://github.com/publieople/dsh-omniroute-models) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: searchable/filterable model manager for OmniRoute (or any OpenAI-compatible gateway) — provider directory, modality discovery, multi-select enable. |
| 1468 | [Q-xuan/dsh-authmux](https://github.com/Q-xuan/dsh-authmux) | 0 | 2026-09-01 | 2026-09-01 | One login plane for subscription-backed model providers in DeepSeek Harness |
| 1469 | [QChengW/dsh-conversation-shortcuts](https://github.com/QChengW/dsh-conversation-shortcuts) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin for conversation keyboard shortcuts |
| 1470 | [qgx1992/dsh-model-select-style](https://github.com/qgx1992/dsh-model-select-style) | 0 | 2026-08-27 | 2026-08-27 | DSH web 插件：把输入框模型选择控件替换为两个独立按钮（供应商 + 模型两级联动，支持推理等级调节） |
| 1471 | [qgx1992/dsh-notify](https://github.com/qgx1992/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | DSH 通知显示层插件：全局 toast 栈，订阅桌面壳 __dshExo 桥事件，点击经官方 sessions runtime 程序化激活会话；无壳时降级订阅 sessions store 自绘。可插拔通知显示层的 web 侧。 |
| 1472 | [QianLuo-Ly/dsh-weather](https://github.com/QianLuo-Ly/dsh-weather) | 0 | 2026-09-02 | 2026-09-02 | dsh的天气插件（没有高大上的东西，生活不易，出门记得看天气~） |
| 1473 | [qinshige/dsh-performance-guard](https://github.com/qinshige/dsh-performance-guard) | 0 | 2026-08-25 | 2026-08-31 | Host and Web performance diagnostics, repeated plugin-isolation campaigns, and safe recovery for DeepSeek Harness. |
| 1474 | [qipenglin/dsh-plugin-manager](https://github.com/qipenglin/dsh-plugin-manager) | 0 | 2026-08-28 | 2026-08-29 | Profile plugin manager for DeepSeek Harness |
| 1475 | [qipenglin/dsh-theme-spectrum](https://github.com/qipenglin/dsh-theme-spectrum) | 0 | 2026-08-28 | 2026-08-29 | Light and dark theme presets for DeepSeek Harness Web |
| 1476 | [qipenglin/dsh-web-access](https://github.com/qipenglin/dsh-web-access) | 0 | 2026-08-27 | 2026-08-27 | Optional Web access authentication plugin for DeepSeek Harness |
| 1477 | [qiqiangvae/dsh-newbe-plugins](https://github.com/qiqiangvae/dsh-newbe-plugins) | 0 | 2026-09-03 | 2026-09-04 | 个人使用 DSH 的增强插件，包括收藏功能、输入锁和会话工具收纳等功能 |
| 1478 | [qiqiangvae/dsh-obsidian](https://github.com/qiqiangvae/dsh-obsidian) | 0 | 2026-08-29 | 2026-09-01 | dsh obsidian wiki plugin |
| 1479 | [qomob/dsh-madrank](https://github.com/qomob/dsh-madrank) | 0 | 2026-09-03 | 2026-09-03 | AI usage dashboard + optional global ranking for DeepSeek Harness (DSH). |
| 1480 | [qt-11564/dsh-git-seam](https://github.com/qt-11564/dsh-git-seam) | 0 | 2026-08-29 | 2026-08-29 | Structured git tools for DeepSeek Harness: diff-before-commit gate + deterministic porcelain parsing (Chinese/UTF-8 paths, Windows) |
| 1481 | [QuanhuZeYu/dsh-idle-compactor](https://github.com/QuanhuZeYu/dsh-idle-compactor) | 0 | 2026-09-04 | 2026-09-04 | Idle-triggered context compaction plugin for DeepSeek Harness: compact a session once it goes quiet past a configurable token floor. |
| 1482 | [QuanQQQ/dsh-plugin-dev-manager](https://github.com/QuanQQQ/dsh-plugin-dev-manager) | 0 | 2026-08-24 | 2026-08-27 | Stable control plane for isolated DeepSeek Harness plugin development |
| 1483 | [que3sui/dsh-darwin](https://github.com/que3sui/dsh-darwin) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness (dsh) 双插件自进化架构：dsh-sentinel 机械挖掘会话日志生成问题工单 + dsh-forge 分级合成/评测门/确定性回滚 \| Two-plugin self-evolution for DSH: hindsight mining, gated synthesis, deterministic rollback (verified in simulation lab) |
| 1484 | [QWE13-ART/dsh-claim-gate](https://github.com/QWE13-ART/dsh-claim-gate) | 0 | 2026-09-02 | 2026-09-02 | Turn-boundary claim gate for DSH agents: 声称「已完成/已落地」但本轮无验证输出时机械拦截；有验证输出时软提示对照验证覆盖 + 任务收尾派独立审计。纯同步正则 host hook（agent/turn-stopping），零 LLM、零网络。 |
| 1485 | [QWE13-ART/dsh-skill-folder](https://github.com/QWE13-ART/dsh-skill-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH skill catalog prompt surface: static KV-cache-stable catalog + BM25/bge-m3 hybrid skill_search + autoRoute hints. v0.3.0. npm: dsh-skill-folder |
| 1486 | [QWE13-ART/dsh-tool-folder](https://github.com/QWE13-ART/dsh-tool-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH tool surface per request + ChainGuard firewall (high-risk block + exfil-chain detection + anti-obfuscation) + BM25/bge-m3 hybrid tools_search. Shrinks schema tokens 80-90% while keeping selection accuracy. v0.2.0 adds a semantic retrieval leg (local Ollama bge-m3, RRF hybrid) and ChainGuard obfuscation detection. npm: dsh-tool-folder |
| 1487 | [qwerty-k-de/dsh-attach-picker](https://github.com/qwerty-k-de/dsh-attach-picker) | 0 | 2026-09-01 | 2026-09-01 | DSH Web composer toolbar picture button: pick images via the OS file dialog - no drag-and-drop needed. |
| 1488 | [raktim-mondol/dsh-researchcraft](https://github.com/raktim-mondol/dsh-researchcraft) | 0 | 2026-08-28 | 2026-08-28 | ResearchCraft as a DeepSeek Harness (DSH) profile plugin: research persona, scientific skills catalogue, living lab notebook, and specialist subagents. |
| 1489 | [randomix777/dsh-plugin-subs](https://github.com/randomix777/dsh-plugin-subs) | 0 | 2026-08-28 | 2026-08-31 | DSH plugin: OAuth sign-in for Claude, Codex, Grok, Antigravity, OpenRouter, Agnes AI — expose subscription LLMs as DeepSeek Harness providers |
| 1490 | [randomix777/dsh-sprite-gen](https://github.com/randomix777/dsh-sprite-gen) | 0 | 2026-08-28 | 2026-08-31 | Sprite Sheet Generator with AI Image Generation for DeepSeek Harness |
| 1491 | [rangdl/dsh-all-enhance](https://github.com/rangdl/dsh-all-enhance) | 0 | 2026-08-28 | 2026-09-01 | DSH（DeepSeek Harness）功能增强插件 |
| 1492 | [Ranz-Feng/dsh-web-import](https://github.com/Ranz-Feng/dsh-web-import) | 0 | 2026-08-26 | 2026-08-27 | Import DeepSeek Web (chat.deepseek.com) chat history into DeepSeek Harness as resumable, workspace-grouped sessions with original titles preserved. |
| 1493 | [Raywh/dsh-song-download](https://github.com/Raywh/dsh-song-download) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 歌曲下载插件：搜索（B站/YouTube）+ 下载（MP3 320k 酷狗兼容）+ LRC 歌词（站点字幕 + 网易云兜底）。DSH plugin: song search & download with lyrics. |
| 1494 | [RayzPub/dsh-plugin-garmin](https://github.com/RayzPub/dsh-plugin-garmin) | 0 | 2026-09-03 | 2026-09-03 | dsh-plugin-garmin 是专为佳明表盘开发的 DeepSeek Harness (dsh) 插件。用户只需在聊天窗口中通过自然语言对话，即可完成针对 Garmin Fenix 7 系列（260×260、64 色 MIP 显示屏）的表盘设计、矢量仿真预览、资源合规校验、Monkey C 源码生成以及最终 .prg 安装二进制的编译打包 |
| 1495 | [renat3u/dsh-upgrade-skill](https://github.com/renat3u/dsh-upgrade-skill) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件升级适配skill |
| 1496 | [Renjie-hub-byte/DSH-AutoKnit](https://github.com/Renjie-hub-byte/DSH-AutoKnit) | 0 | 2026-09-01 | 2026-09-01 | PRD in, maintainable code out. Cheap to build, cheaper to maintain — benchmark: −19% vs interactive agent, −41% vs heavy framework. 程序调度 0 token，写省改省不用盯。pip install autoknit |
| 1497 | [Reseezhang/ue-log-reader](https://github.com/Reseezhang/ue-log-reader) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：UE 日志速读卡 — 模型调用 uelog 工具扫描 Saved/Logs，流式解析+聚合去重后渲染速读卡片，一键复制缺陷单摘要 |
| 1498 | [Reseezhang/vizcb-codeblock-visualizer](https://github.com/Reseezhang/vizcb-codeblock-visualizer) | 0 | 2026-08-28 | 2026-08-29 | DeepSeek Harness 可视化插件：svg/html/mermaid 代码块渲染为图表卡片（宿主端 mermaid、深色主题配色、节点文字自适应、灯箱、保存导出） |
| 1499 | [retmon2333/dsh-background](https://github.com/retmon2333/dsh-background) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness（DSH）背景壁纸更换（单图 / 文件夹轮播）模式，可调透明、模糊、遮罩与樱花／雪花特效，侧栏与输入框也能透出壁纸 |
| 1500 | [RexYoung000/rex-harness](https://github.com/RexYoung000/rex-harness) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin authoring workspace. First plugin: UI design workflow (@rex-harness/ui-workflow). |
| 1501 | [rm-Vstar/web-search-tinyfish](https://github.com/rm-Vstar/web-search-tinyfish) | 0 | 2026-08-28 | 2026-08-28 | A TinyFish web searching plugin for Deepseek Harness |
| 1502 | [robbin810130/dsh-vault-plugin](https://github.com/robbin810130/dsh-vault-plugin) | 0 | 2026-08-24 | 2026-08-27 | DSH 保险箱插件：项目与对话的前台隐私锁 |
| 1503 | [rrrrrredy/context-continuity](https://github.com/rrrrrredy/context-continuity) | 0 | 2026-08-28 | 2026-08-31 | Local-first continuity plugin for Codex and DeepSeek Harness across compaction, resume, and handoff. |
| 1504 | [rrrrrredy/dsh-execution-fidelity-guard](https://github.com/rrrrrredy/dsh-execution-fidelity-guard) | 0 | 2026-08-31 | 2026-08-31 | Unofficial alpha execution-fidelity guard bundle for DeepSeek Harness. |
| 1505 | [rrrrrredy/intent-loop](https://github.com/rrrrrredy/intent-loop) | 0 | 2026-08-31 | 2026-08-31 | Local-first, traceable current-intent state for Codex and DeepSeek Harness. |
| 1506 | [ruanhaodong-tt/dsh-security-guard](https://github.com/ruanhaodong-tt/dsh-security-guard) | 0 | 2026-09-03 | 2026-09-03 | DSH runtime security guard plugin - loader import confinement, HTTP Host header validation (QVD-2026-52631/57410). AI-assisted. |
| 1507 | [Rudyy898/dsh-drag-path](https://github.com/Rudyy898/dsh-drag-path) | 0 | 2026-08-27 | 2026-08-27 | dsh-plugin |
| 1508 | [ruiyukirin/dsh-douyin-oem-touliu-report](https://github.com/ruiyukirin/dsh-douyin-oem-touliu-report) | 0 | 2026-08-28 | 2026-08-28 | 抖音本地推 OEM 投流日报/周报自动化插件 - Douyin OEM ad daily/weekly report automation plugin for DeepSeek Harness (Author: Kirin) |
| 1509 | [runcat-tommy/dsh-panda-calendar](https://github.com/runcat-tommy/dsh-panda-calendar) | 0 | 2026-09-03 | 2026-09-03 | 熊猫日历 · DSH client-plugin：公历/农历/干支/生肖/节气、传统与外国节日、中国法定节假日（含调休）、多城市天气 — token-free Chinese calendar & weather plugin for DeepSeek Harness Web. |
| 1510 | [runcat-tommy/dsh-plugin-runcat-inventory](https://github.com/runcat-tommy/dsh-plugin-runcat-inventory) | 0 | 2026-08-26 | 2026-08-28 | 逃咪-插件总览（Runcat Plugin Overview）—— 更好用的 DSH 插件列表：表格视图、状态过滤、启用/停用开关（热生效）、配置查看与复制、中英双语界面。 |
| 1511 | [runcat-tommy/dsh-theme-manager](https://github.com/runcat-tommy/dsh-theme-manager) | 0 | 2026-08-28 | 2026-08-28 | Two-level theme manager for DeepSeek Harness Web: pick a culture/scene or a national flag first, then a concrete style. 40 built-in styles (ink wash, ukiyo-e, Suzhou garden, cyberpunk, 20 flags & more). |
| 1512 | [runcat-tommy/dsh-view-manager](https://github.com/runcat-tommy/dsh-view-manager) | 0 | 2026-08-27 | 2026-08-28 | Manage DeepSeek Harness Web GUI view tabs (Chat/Trajectory): enable, hide, reorder & rename with zh/en locale. |
| 1513 | [RyanShen3/dsh-toutiao-reader](https://github.com/RyanShen3/dsh-toutiao-reader) | 0 | 2026-08-29 | 2026-08-29 | 读网页/头条文章全文的 DSH 插件：webfetch 工具 + toutiao-reader 经验技能 |
| 1514 | [ryasrk/dsh-vision-patch](https://github.com/ryasrk/dsh-vision-patch) | 0 | 2026-09-03 | 2026-09-03 | Patch custom provider vision model |
| 1515 | [Rycbartbad/dsh-key-manager](https://github.com/Rycbartbad/dsh-key-manager) | 0 | 2026-08-29 | 2026-08-29 | Multiple API keys per provider for DeepSeek Harness: pools with notes, one-click switching that really takes effect |
| 1516 | [Ryu6Zero/dsh-hindsight](https://github.com/Ryu6Zero/dsh-hindsight) | 0 | 2026-08-25 | 2026-08-27 | 🧠 Cross-session memory for DeepSeek Harness backed by Hindsight. Self-contained dsh-plugin: /hindsight commands + hindsight_recall/remember/status/list/forget agent tools. Lightweight, no dsh-mnemon, no orchestrator. |
| 1517 | [sailoflight/dsh-bash-escalation](https://github.com/sailoflight/dsh-bash-escalation) | 0 | 2026-09-03 | 2026-09-03 | 状态:完成 |
| 1518 | [sailoflight/dsh-vision-toolkit-windows-edge](https://github.com/sailoflight/dsh-vision-toolkit-windows-edge) | 0 | 2026-09-03 | 2026-09-03 | 状态:完成 |
| 1519 | [sandersyao/dsh-credentials-mysql](https://github.com/sandersyao/dsh-credentials-mysql) | 0 | 2026-09-02 | 2026-09-03 | DeepSeek Harness 基于 MySQL 的后端凭证库插件 (ctx.credentials) |
| 1520 | [sandersyao/dsh-storage-mysql](https://github.com/sandersyao/dsh-storage-mysql) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 基于 MySQL 的后端存储插件 可通过 storage-domain 配置用于 workspace、session-projection-cache 和 message-feedback 数据的存储 |
| 1521 | [sANDzER0/dsh-hippocampus](https://github.com/sANDzER0/dsh-hippocampus) | 0 | 2026-08-26 | 2026-08-27 | Cross-session project memory for DeepSeek Harness — capture / consolidate / recall, keyword + optional local-Ollama semantic search. Inspired by magic-context. |
| 1522 | [sanyamjain2014/dsh-plugins](https://github.com/sanyamjain2014/dsh-plugins) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness (DSH) plugins by sanyamjain2014 — everything is a plugin. |
| 1523 | [saqie803/ponytail](https://github.com/saqie803/ponytail) | 0 | 2026-08-29 | 2026-08-29 | Ship production-ready code with one line of AI-generated output, built for 20 agents and zero ceremony. |
| 1524 | [sdoygb/geometry-knowledge](https://github.com/sdoygb/geometry-knowledge) | 0 | 2026-08-26 | 2026-08-27 | 几何论（共扼谱几何 CSG）知识库插件 for DeepSeek Harness: 纯离线 BM25 检索，零运行时依赖 |
| 1525 | [seeingrain/dsh-session-todos](https://github.com/seeingrain/dsh-session-todos) | 0 | 2026-09-03 | 2026-09-04 | 会话内待办事项：DSH 悬浮待办面板 + 服务器端跨端存储 + 会话列表未完成图标 |
| 1526 | [seiriosPlus/miaoda_for_deepseek_harness](https://github.com/seiriosPlus/miaoda_for_deepseek_harness) | 0 | 2026-08-26 | 2026-08-29 | miaoda_for_deepseek harness |
| 1527 | [seoeaa/dsh-locale-ru](https://github.com/seoeaa/dsh-locale-ru) | 0 | 2026-08-31 | 2026-08-31 | Русский интерфейс (локаль ru) для DeepSeek Harness — custom locale plugin. 26 namespaces, ~690 строк. / Russian locale plugin for DeepSeek Harness. |
| 1528 | [seth-hg/dsh-session-port](https://github.com/seth-hg/dsh-session-port) | 0 | 2026-09-02 | 2026-09-02 | dsh-session-port is a DeepSeek Harness plugin that bundles a session — its log, subagents, media, and referenced workspace files — into one portable ZIP and restores it on any DSH. |
| 1529 | [ShadowQuill/DialogueContextBridge](https://github.com/ShadowQuill/DialogueContextBridge) | 0 | 2026-08-26 | 2026-08-27 | 对话上下文桥接 — 为大语言模型(LLM)/AI 智能体的对话做跨会话上下文桥接的 DSH 插件：把一次对话的共识打包成可移植快照，一键引入新对话（三层快照 / SQLite+FTS5 / AES-256-GCM） |
| 1530 | [ShaineDemo/dsh-vision-pro-bridge](https://github.com/ShaineDemo/dsh-vision-pro-bridge) | 0 | 2026-09-03 | 2026-09-03 | Give text-only DeepSeek-V4-Pro vision — zero new dependencies, DeepSeek-only routing (images described by deepseek-v4-flash-vision-exp, then answered by V4-Pro). |
| 1531 | [shaneconner/canon](https://github.com/shaneconner/canon) | 0 | 2026-08-10 | 2026-08-30 | Canonical project memory for the Pi coding agent: one governing article per asset, an append-only journal, capsule surfacing. A project wiki with a spine. |
| 1532 | [shaneconner/dsh-claude-bridge](https://github.com/shaneconner/dsh-claude-bridge) | 0 | 2026-08-30 | 2026-08-31 | Use a Claude Pro or Max subscription as a DeepSeek Harness model provider, via the Claude Code CLI. |
| 1533 | [shaneconner/dsh-provider-login](https://github.com/shaneconner/dsh-provider-login) | 0 | 2026-08-30 | 2026-08-31 | Sign in to DeepSeek Harness model providers with a Claude Pro/Max or ChatGPT Plus/Pro subscription. |
| 1534 | [shangdi178/dsh-reasoning-bridge](https://github.com/shangdi178/dsh-reasoning-bridge) | 0 | 2026-09-03 | 2026-09-03 | Reasoning Bridge for dsh: hand high-cost reasoning to web AI (ChatGPT first, multi-target); keep local evidence, adoption gate, edits, and tests. Contract-based handoffs, versioned consent, SHA-256 receipts. Zero dependencies. |
| 1535 | [shangdi178/dsh-versions](https://github.com/shangdi178/dsh-versions) | 0 | 2026-09-01 | 2026-09-03 | dsh (DeepSeek Harness) 主程序版本管理插件：版本总览 + npm 更新检查 + 在线升级/降级/重装 + 升级前自动快照、任意历史版本秒级回滚 |
| 1536 | [shangfr/dsh-md-picker](https://github.com/shangfr/dsh-md-picker) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness Web GUI 插件：在会话输入框左侧添加一个「文档 + Markdown」按钮，通过系统文件选择器添加附件并转换成 Markdown 格式。 |
| 1537 | [ShanHaiFish/dsh-theme-brick](https://github.com/ShanHaiFish/dsh-theme-brick) | 0 | 2026-08-30 | 2026-08-30 | DSH 主题插件（Brick/砌砖）：纯 token 覆盖层，暖石膏与火烧黏土、灰缝线条、一砖一色，零全局 CSS；Settings → General 开关可随时关闭还原。A restrained token-only theme for DeepSeek Harness web — plaster & fired-clay, one accent, no global CSS, with an on/off switch. |
| 1538 | [shaomingbo/dsh-anyrouter](https://github.com/shaomingbo/dsh-anyrouter) | 0 | 2026-08-31 | 2026-08-31 | Dedicated provider bundle for the relay: Claude via Claude Code transport, GPT/Codex via Responses, for DeepSeek Harness |
| 1539 | [shaomingbo/dsh-open-in-editor](https://github.com/shaomingbo/dsh-open-in-editor) | 0 | 2026-08-26 | 2026-08-27 | Open DSH Web produced files in a configurable local macOS IDE |
| 1540 | [shaomingbo/dsh-subscription-antigravity](https://github.com/shaomingbo/dsh-subscription-antigravity) | 0 | 2026-08-29 | 2026-08-29 | Google Antigravity subscription reuse for DeepSeek Harness: browser PKCE sign-in, loopback OpenAI-compatible proxy to Cloud Code Assist, Gemini/Claude/GPT-OSS model routes. |
| 1541 | [shaomingbo/dsh-token-usage](https://github.com/shaomingbo/dsh-token-usage) | 0 | 2026-08-30 | 2026-08-30 | Accounts, subscription allowance observations, and local usage ledger for DeepSeek Harness |
| 1542 | [Shaw529/dsh-token-saver](https://github.com/Shaw529/dsh-token-saver) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin: aggressive token savings, no task-quality loss |
| 1543 | [shayexiangpaimeng/dsh-memory](https://github.com/shayexiangpaimeng/dsh-memory) | 0 | 2026-08-31 | 2026-08-31 | Append-only layered memory plugin for DeepSeek Harness: five-layer partitioning, write gate, keyword recall, claim-anchors verification |
| 1544 | [shengyvself/narrative-prompt-polish](https://github.com/shengyvself/narrative-prompt-polish) | 0 | 2026-08-28 | 2026-08-30 | DSH 插件：主输入框 ✨ 一键把草稿润色成清晰、可执行的提示词，经 better-sidebar 侧栏对话多轮打磨后回填。A DSH plugin: ✨ one-click draft polish into agent-ready prompts, multi-turn side-chat via better-sidebar (>=0.16.1). |
| 1545 | [shenhuanageshei/dsh-death-forensics](https://github.com/shenhuanageshei/dsh-death-forensics) | 0 | 2026-09-02 | 2026-09-02 | In-process death black box for DeepSeek Harness (dsh) hosts: heartbeat windows, crash stacks, end-kind self-check, death_forensics_report tool. |
| 1546 | [shenhuanageshei/dsh-git-status](https://github.com/shenhuanageshei/dsh-git-status) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：会话视图实时 git 状态展示 + 分支切换（会话头徽标 + 输入区环境行）。官方 bundle 插件，dsh plugin --profile web add：github:shenhuanageshei/dsh-git-status#v0.1.0 |
| 1547 | [shenhuanageshei/dsh-preset-zombie-guard](https://github.com/shenhuanageshei/dsh-preset-zombie-guard) | 0 | 2026-09-01 | 2026-09-01 | Preset-zombie guard plugin for DeepSeek Harness: auto-archive blank zombie sessions, warn on non-blank, pre-deletion dependency audit (preset_guard_check_remove). |
| 1548 | [shenhuanageshei/dsh-session-link-pro](https://github.com/shenhuanageshei/dsh-session-link-pro) | 0 | 2026-08-31 | 2026-08-31 | Session deep links + full session export (markdown/JSON) + approved cross-session messaging with pairing for DeepSeek Harness (dsh). |
| 1549 | [shenhuanageshei/dsh-thincoder-suite](https://github.com/shenhuanageshei/dsh-thincoder-suite) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin porting thincoder self-discipline suite: advisor convergent review / engineering mode / escalate / consult |
| 1550 | [ShenXuAkaEkstasis/dsh-ai-shopping-assistant](https://github.com/ShenXuAkaEkstasis/dsh-ai-shopping-assistant) | 0 | 2026-08-28 | 2026-08-28 | AI Shopping Assistant plugin for DeepSeek Harness (DSH), with product comparison, price analysis, merchant/review evidence and source-quality checks. |
| 1551 | [ShineFree7/dsh-doc-rail](https://github.com/ShineFree7/dsh-doc-rail) | 0 | 2026-09-02 | 2026-09-02 | Right-side document rail for the DeepSeek Harness web GUI — Markdown/plain-text viewer with light & deep-navy themes, drag-resize, recent files, auto-sync. （中文：dsh web 右侧文档面板，支持浅色/深蓝主题、拖宽、最近文件、自动同步） |
| 1552 | [Shonean/deepseek-harness-vscode-desktop](https://github.com/Shonean/deepseek-harness-vscode-desktop) | 0 | 2026-08-27 | 2026-08-27 | Enhanced VS Code extension + Desktop app for DeepSeek Harness (DSH): inline diff, @mentions, selection context, approval UI, plan mode, global shortcut. Claude Code-grade experience. Unofficial community project. |
| 1553 | [Short-Arm-Ape/dsh-intranet-browser](https://github.com/Short-Arm-Ape/dsh-intranet-browser) | 0 | 2026-08-31 | 2026-08-31 | Bypasses the SSRF protection of @yeesy369dsh-browser-playwright |
| 1554 | [SHUJILAI/dsh-model-auto-hot-switch](https://github.com/SHUJILAI/dsh-model-auto-hot-switch) | 0 | 2026-08-28 | 2026-08-28 | Automatic per-task model hot-switching for DeepSeek Harness (dsh): image-aware tasks route to the vision model automatically, every other task keeps your default model. Zero extra tokens, no context disturbance. |
| 1555 | [shxtmaker/dsh-usage-monitor](https://github.com/shxtmaker/dsh-usage-monitor) | 0 | 2026-08-26 | 2026-08-28 | DSH 用量监控插件：供应商周期限额显示（DeepSeek/OpenCode/Command Code）+ 自动探测 DSH 已添加供应商并自动填入 API Key |
| 1556 | [sidrandom/deepseek-memory-capsule](https://github.com/sidrandom/deepseek-memory-capsule) | 0 | 2026-09-01 | 2026-09-01 | A complete, human-centered memory layer for DeepSeek that stores user preferences, conversation notes, and personal variables across sessions — built as a DeepSeek Harness plugin. |
| 1557 | [sijie-ni-0214/dsh-subagent-error-details](https://github.com/sijie-ni-0214/dsh-subagent-error-details) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: deliver the real failure reason (e.g. RATE_LIMIT 429) to the parent agent when a background subagent fails |
| 1558 | [SiriusWJ/dsh-mihome](https://github.com/SiriusWJ/dsh-mihome) | 0 | 2026-08-30 | 2026-08-30 | Mi Home (米家) control for DeepSeek Harness agents — list homes/devices, read props, control devices behind a human approval gate. |
| 1559 | [SJCLZ/MixlabLz-dsh-skills](https://github.com/SJCLZ/MixlabLz-dsh-skills) | 0 | 2026-08-27 | 2026-08-27 | MixlabLz's collection of DSH (DeepSeek Harness) skills and plugins |
| 1560 | [sly7783/lively-wallpaper-guide](https://github.com/sly7783/lively-wallpaper-guide) | 0 | 2026-09-02 | 2026-09-03 | Set up Lively Wallpaper in minutes with step-by-step guides, performance tips, multi-monitor recipes, and curated wallpaper packs. |
| 1561 | [SMOKTEA/dsh-chartlab](https://github.com/SMOKTEA/dsh-chartlab) | 0 | 2026-08-26 | 2026-08-28 | Let the agent turn your data into an interactive chart.  \|  一句话：让 Agent 帮你把数据变成一张可交互的图表。 |
| 1562 | [snow-The/dsh-research-lab](https://github.com/snow-The/dsh-research-lab) | 0 | 2026-08-31 | 2026-08-31 | Research lab toolkit for DeepSeek Harness: AutoSci wiki, ASI-Bench eval ledger, self-building FTS5 retrieval, arXiv digest/review, writing rewrite |
| 1563 | [soberbiak/amazon-sucareer](https://github.com/soberbiak/amazon-sucareer) | 0 | 2026-08-28 | 2026-08-30 | 基于真实证据，把亚马逊运营经历酥成招聘方看得懂、面试讲得透的职业定位、简历与求职表达。拒绝硬编 KPI，争取人生大结果。 |
| 1564 | [socai-io/dsh-socai](https://github.com/socai-io/dsh-socai) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin for SocAI Xiaohongshu research tools |
| 1565 | [softspark/dsh-file-preview](https://github.com/softspark/dsh-file-preview) | 0 | 2026-09-04 | 2026-09-04 | Read-only in-conversation file preview for DeepSeek Harness: a session-authorized host Remote and a sanitizing browser modal, installed as one profile bundle. |
| 1566 | [softspark/dsh-orchestrator](https://github.com/softspark/dsh-orchestrator) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness bundle for one-shot Claude Code and GitHub Copilot Gemini delegation through native subscription logins. |
| 1567 | [soulYANG/dsh-baogongtou](https://github.com/soulYANG/dsh-baogongtou) | 0 | 2026-08-26 | 2026-08-27 | 包工头：DeepSeek Harness 工作 agent 皮肤。能力还是 dsh，嘴和按钮是包工头。 |
| 1568 | [STARDUSTLC666/dsh-dream](https://github.com/STARDUSTLC666/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH 做梦插件：会话回放（梦原料）→ 反思 → 梦境日记（记忆巩固）→ 高频教训幂等桥接 AGENTS.md。多帧 zstd 会话读取、默认隐私脱敏、零运行时依赖。Dream plugin for DeepSeek Harness: session replay, reflection, dream journal, memory bridge. 已验证兼容 DeepSeek Harness v0.1.2-alpha.5。 |
| 1569 | [STARDUSTLC666/dsh-suite](https://github.com/STARDUSTLC666/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | STARDUSTLC 插件全家桶（聚合安装包，不提供独立工具）：一条命令装入 18 个 DSH 插件。18 个插件已在 DeepSeek Harness v0.1.2-alpha.5 同载验证。The STARDUSTLC plugin suite: 18 DSH plugins, one command. |
| 1570 | [statem-li/dsh-done-pill](https://github.com/statem-li/dsh-done-pill) | 0 | 2026-08-30 | 2026-09-01 | DSH 对话完成胶囊：顶部悬浮消息胶囊（原 webui done-pill 拆出）——任一会话回合完成提醒、点击跳会话、悬停查看记录全文、可拖拽定位、健康提醒与字体/缩放设置。零 DSH 源码改动，可与 dsh-webui 并存（webui 关闭 donePill 模块即可）。 |
| 1571 | [statem-li/dsh-think-tools](https://github.com/statem-li/dsh-think-tools) | 0 | 2026-08-31 | 2026-09-01 | DSH 思考与工具调用聚合：回合级思考 chip（实时时长/实时文字滚动）+ 工具调用聚合 chip + 共享活动抽屉 + 对话流卡片（步骤卡/总结卡，回合结束后才出现）——自 dsh-webui 移植。零 DSH 源码改动。 |
| 1572 | [statem-li/dsh-web-search-anysearch](https://github.com/statem-li/dsh-web-search-anysearch) | 0 | 2026-08-31 | 2026-09-01 | DSH 外接网页搜索（AnySearch）：注册 AnySearch 网页搜索 provider（替换内置 DeepSeek 搜索）+ 插件设置卡（API Key / Base URL / 默认结果数）。提炼自 statem-li/dsh-webui 的 webSearch 模块，零 DSH 源码改动。 |
| 1573 | [stayhpjinng/dsh-provider-proxy](https://github.com/stayhpjinng/dsh-provider-proxy) | 0 | 2026-08-29 | 2026-08-29 | Provider-scoped HTTP/HTTPS forward proxy plugin for DeepSeek Harness |
| 1574 | [StephenEvenson/dsh-plugin-elevenlabs-callback](https://github.com/StephenEvenson/dsh-plugin-elevenlabs-callback) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin: when a run finishes or needs approval, get a link on your phone, hear the result from an ElevenLabs voice agent and say what to do next |
| 1575 | [steven-ngle/dsh-elden](https://github.com/steven-ngle/dsh-elden) | 0 | 2026-08-30 | 2026-08-30 | Elden Ring style event overlays for the DeepSeek Harness web UI |
| 1576 | [Stijnus/dsh-ds-kanban](https://github.com/Stijnus/dsh-ds-kanban) | 0 | 2026-09-02 | 2026-09-02 | Live task-board plugin for DeepSeek Harness Web: sidebar badge, full-shell kanban with search, filters, export, and diagnostics. |
| 1577 | [Stijnus/dsh-ds-ponytail](https://github.com/Stijnus/dsh-ds-ponytail) | 0 | 2026-09-02 | 2026-09-02 | Lazy senior dev mode for DeepSeek Harness: ponytail skill family (ponytail, review, audit, debt, gain, help) adapted from DietrichGebert/ponytail (MIT). Install: dsh plugin --profile web add dsh-ds-ponytail |
| 1578 | [StudyforDS/Deepseek_dsh-plugin](https://github.com/StudyforDS/Deepseek_dsh-plugin) | 0 | 2026-08-30 | 2026-08-31 | dsh-plugin |
| 1579 | [substitute525/dsh-tool-monitor](https://github.com/substitute525/dsh-tool-monitor) | 0 | 2026-08-28 | 2026-08-28 | 一个 dsh-plugin：后台监听文件或命令输出，输出到达时唤醒所属会话，并在 Web 会话头部提供实时监听的列表与输出查看面板。MIT License。 |
| 1580 | [SuCriss/dsh-voice-control](https://github.com/SuCriss/dsh-voice-control) | 0 | 2026-08-31 | 2026-08-31 | Voice control for DeepSeek Harness web: speech-to-text into the composer and spoken playback of assistant replies, zero dependencies |
| 1581 | [Suguyun/dsh-bili-miniplay](https://github.com/Suguyun/dsh-bili-miniplay) | 0 | 2026-08-28 | 2026-08-28 | 跨平台 fork of dsh-bili-widget：DSH B站悬浮看片小窗（Node 原生 fetch，macOS/Linux/Windows 通用） |
| 1582 | [sunyuhuirong/fsviewer](https://github.com/sunyuhuirong/fsviewer) | 0 | 2026-08-29 | 2026-08-30 | Codex-style right-edge workspace for DeepSeek dsh web: file tree + preview, embedded browser, and side chat |
| 1583 | [superkonka/dsh-poor-mode](https://github.com/superkonka/dsh-poor-mode) | 0 | 2026-08-27 | 2026-08-27 | 穷鬼模式 Poor Mode — 供应商感知的分时省钱 DSH agent preset：复杂任务可选「立即执行」或「闲时执行」（DeepSeek 峰谷半价；其他平台可自定义规则） |
| 1584 | [SuperstructureJH/dsh-workbuddy-ppt](https://github.com/SuperstructureJH/dsh-workbuddy-ppt) | 0 | 2026-08-26 | 2026-08-27 | Editable PPTX generation for DSH with bundled authoring skills and deterministic PPTD validation |
| 1585 | [suyukun/dsh-plugin-publish](https://github.com/suyukun/dsh-plugin-publish) | 0 | 2026-08-26 | 2026-08-27 | Ship your skills, grow your influence — a model-agnostic publishing protocol for AI agent skills: preflight checks, GitHub repo, index PRs, marketplace submissions, promo copy. 把 agent 技能标准化发布到 GitHub 的流程协议。 |
| 1586 | [suyukun/dsh-tech-selection](https://github.com/suyukun/dsh-tech-selection) | 0 | 2026-08-26 | 2026-08-27 | Stop letting your AI guess — a research protocol for tech decisions that any AI agent (DSH/Claude/Cursor/Codex) can follow: quantified requirements, T1-T6 source tiers, quality gates, traceable verdicts. 模型无关的技术选型调研协议。 |
| 1587 | [suzuran520yyz/dsh-more-message-actions](https://github.com/suzuran520yyz/dsh-more-message-actions) | 0 | 2026-09-03 | 2026-09-03 | DSH Web GUI 插件，用于对会话消息进行编辑、重试、高级重试和删除等功能的实现 |
| 1588 | [svgop/dsh-generative-ideas](https://github.com/svgop/dsh-generative-ideas) | 0 | 2026-08-26 | 2026-08-29 | Roadmap ideation for DeepSeek Harness — generate and compare distinct roadmap options via headless agent runs, pick one, export as goal.md |
| 1589 | [svgop/dsh-rich-context](https://github.com/svgop/dsh-rich-context) | 0 | 2026-08-26 | 2026-08-29 | Agent instruction manager for DSH — edit and template the AGENTS.md files the harness actually reads (global + per-workspace) |
| 1590 | [svgop/dsh-rich-tracking](https://github.com/svgop/dsh-rich-tracking) | 0 | 2026-08-26 | 2026-08-29 | Percent-progress scoreboard for DeepSeek Harness — evidence-bound rows, git-captured checkpoints, pursue/align/dismiss operator whip |
| 1591 | [swxs/archive-restore](https://github.com/swxs/archive-restore) | 0 | 2026-09-02 | 2026-09-02 | DSH 归档会话管理插件，支持查看归档列表、原位恢复与跨区迁移，Web 侧边栏一键管理 |
| 1592 | [sxy-kumako/dsh-better-model-select](https://github.com/sxy-kumako/dsh-better-model-select) | 0 | 2026-09-04 | 2026-09-04 | DSH 插件：模型列表跟随 provider API 实时更新 + 各 provider 用量徽标 (GLM/MiniMax coding plan, DeepSeek/OpenRouter/Kimi balance) |
| 1593 | [syfun/dsh-dogpet](https://github.com/syfun/dsh-dogpet) | 0 | 2026-08-27 | 2026-08-27 | 🐕 中华田园犬桌面宠物 - DSH Desktop Pet |
| 1594 | [syncended/deepseek-harness-messenger](https://github.com/syncended/deepseek-harness-messenger) | 0 | 2026-08-25 | 2026-08-29 | Messenger bridge plugin for DeepSeek Harness, starting with Telegram |
| 1595 | [syncended/deepseek-harness-usage](https://github.com/syncended/deepseek-harness-usage) | 0 | 2026-08-26 | 2026-08-27 | Token usage, model cost analytics, trends, and activity heatmaps for DeepSeek Harness |
| 1596 | [szymonsheng2045/dsh-carbonclub](https://github.com/szymonsheng2045/dsh-carbonclub) | 0 | 2026-08-28 | 2026-08-28 | A zero-model-cost human waiting room for DeepSeek Harness |
| 1597 | [Tangweiwei227/dsh-asc](https://github.com/Tangweiwei227/dsh-asc) | 0 | 2026-08-29 | 2026-08-29 | App Store Connect CLI (asc) as a native tool for DeepSeek Harness — structured argv, JSON output, no-shell execution. |
| 1598 | [taod8205-spec/model-switcher-dsh](https://github.com/taod8205-spec/model-switcher-dsh) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 模型与推理强度一键切换插件，支持胶囊滑杆、档位吸附和极高态视觉。 |
| 1599 | [tappat225/dsh-provider-hub](https://github.com/tappat225/dsh-provider-hub) | 0 | 2026-08-28 | 2026-09-04 | 自定义参数provider面板 |
| 1600 | [TARS-snail/dsh-guard-sensitive-paths](https://github.com/TARS-snail/dsh-guard-sensitive-paths) | 0 | 2026-09-02 | 2026-09-02 | Approval guard for DeepSeek Harness: write/edit/editor/bash calls touching sensitive paths (.env, .git, SSH keys, .pem) become an approval ask. |
| 1601 | [Tazio7/dsh-web-search-glm](https://github.com/Tazio7/dsh-web-search-glm) | 0 | 2026-09-01 | 2026-09-01 | Web search plugin for DeepSeek Harness powered by ZAI GLM MCP — auto-injects API key from ~/.dsh/.credentials.yaml or environment variables |
| 1602 | [theinfluencecompany/dsh-realtimeavatar](https://github.com/theinfluencecompany/dsh-realtimeavatar) | 0 | 2026-09-03 | 2026-09-03 | Realtime Avatar (realtimeavatar.ai) for the DeepSeek Harness (dsh): harness-held API key, public docs as skills, rta_* tools, /rta onboarding, zero runtime dependencies |
| 1603 | [thomasly/dsh-markdown-preview](https://github.com/thomasly/dsh-markdown-preview) | 0 | 2026-09-04 | 2026-09-04 | DSH web plugin: live Markdown + KaTeX math preview above the composer (official slot, zero core patches) |
| 1604 | [thuCGRA/dsh-quick-invoke](https://github.com/thuCGRA/dsh-quick-invoke) | 0 | 2026-09-02 | 2026-09-02 | `dsh-quick-invoke` 是一个面向 DSH Web 的独立 Cordis 插件，为 Skill、Agent preset 和 Plugin 提供统一的 `/` 快捷入口、候选选择和 Host 命令执行能力。  本插件不修改 DSH 核心，不提供任意 Tool 直调语法。Tool 仍由 Agent 根据自然语言选择，并继续经过 DSH 的 tools、approval、guard 和 permission 流程。 |
| 1605 | [tianhanly/dsh-genshin-redirect](https://github.com/tianhanly/dsh-genshin-redirect) | 0 | 2026-08-30 | 2026-08-31 | 完成任务自动跳转到原神 Automatically jump to Genshin Impact after completing the task |
| 1606 | [tianhanly/dsh-official-port-nav](https://github.com/tianhanly/dsh-official-port-nav) | 0 | 2026-08-29 | 2026-08-30 | Perfectly replicate DeepSeek's official right-side chat navigation in Harness |
| 1607 | [tianhanly/dsh-verification-meme](https://github.com/tianhanly/dsh-verification-meme) | 0 | 2026-08-30 | 2026-08-31 | Every time you press a key, a security verification pops up. 每按一个harness的按键都会跳出一个安全验证 |
| 1608 | [tianhanly/dsh-warm-reminder](https://github.com/tianhanly/dsh-warm-reminder) | 0 | 2026-08-29 | 2026-08-29 | 智能温馨提醒插件，检测使用时长自动提示喝水、护眼、休息，支持深夜关怀与节假日祝福。基于DSH/Cordis框架开发。 |
| 1609 | [tianjiqx/dsh-agentobs](https://github.com/tianjiqx/dsh-agentobs) | 0 | 2026-09-01 | 2026-09-01 | dsh 可观测解决方案 |
| 1610 | [tianyuegithub/dsh-pactflow](https://github.com/tianyuegithub/dsh-pactflow) | 0 | 2026-08-30 | 2026-08-30 | DSH PactFlow（零脉模式）外部 Profile Bundle |
| 1611 | [tiphareth0/dsh-hardssh](https://github.com/tiphareth0/dsh-hardssh) | 0 | 2026-09-02 | 2026-09-03 | Run your work with existing DSH plugins on remote servers, across any number of machines |
| 1612 | [tntcannon5000/dsh-chat-fold](https://github.com/tntcannon5000/dsh-chat-fold) | 0 | 2026-09-03 | 2026-09-04 | Compact turn folding for DeepSeek Harness Web: restores collapsed completed turns in long sessions where stock folding stays disabled. |
| 1613 | [TnzGit/dsh-live-perf-gauges](https://github.com/TnzGit/dsh-live-perf-gauges) | 0 | 2026-08-27 | 2026-08-27 | Real-time Decode tok/s, TTFT and Prefill throughput dashboard for DeepSeek Harness. |
| 1614 | [Traveritas/petween](https://github.com/Traveritas/petween) | 0 | 2026-08-21 | 2026-08-29 | Agent pet plugin for DeepSeek Harness (dsh): a few pose images in, expressive comic-style motion out — WAAPI timeline engine, custom animation editor, pose presets, and extension services for companion plugins |
| 1615 | [Traveritas/petween-physics](https://github.com/Traveritas/petween-physics) | 0 | 2026-08-25 | 2026-08-29 | Throw-physics companion plugin for Petween (drag-fling, wall bounce, ground slide), consuming the petween extension services |
| 1616 | [trueRISCOacnt/maa-dsh-skill](https://github.com/trueRISCOacnt/maa-dsh-skill) | 0 | 2026-08-28 | 2026-08-30 | 基于 MaaAssistantArknights (MAA) 官方命令行工具 maa-cli 构建的 DeepSeek Harness Skill：让 DeepSeek Harness 直接驱动 MaaCore，自动化完成《明日方舟》日常任务。 |
| 1617 | [tumi-huakai/dsh-plugin-meow-speech](https://github.com/tumi-huakai/dsh-plugin-meow-speech) | 0 | 2026-08-28 | 2026-08-28 | 喵语定制：DSH 消息正文显示层文本替换插件（仅界面显示，不改动真实对话内容） |
| 1618 | [TussalZeus18028/dsh-conflict-checker](https://github.com/TussalZeus18028/dsh-conflict-checker) | 0 | 2026-08-26 | 2026-08-27 | Detect DeepSeek Harness plugin conflicts and internal issues; manage plugins (enable/disable/uninstall) from a settings page. |
| 1619 | [tuzkier/valley-liang](https://github.com/tuzkier/valley-liang) | 0 | 2026-08-28 | 2026-08-28 | 梁文谷：替换 DeepSeek Harness Web 品牌标识，并按北京时间高峰时段切换图片。 |
| 1620 | [Tyon-nos-Ty90/dsh-mcsm-panel](https://github.com/Tyon-nos-Ty90/dsh-mcsm-panel) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness Desktop plugin that lets your AI control MCSManager (MCSM 10.x) Minecraft servers from the chat: server console, file management, instance start/restart/stop/kill, and direct file uploads. |
| 1621 | [UnforgetMemory/um-dsh-websearch](https://github.com/UnforgetMemory/um-dsh-websearch) | 0 | 2026-08-27 | 2026-08-27 | Exa (exa.ai) web search provider plugin for DeepSeek Harness (DSH): dynamic enabled switch, credentials-service key resolution, bilingual settings card. |
| 1622 | [UnknowCao/dsh-dock](https://github.com/UnknowCao/dsh-dock) | 0 | 2025-11-09 | 2026-09-04 | One-click desktop launcher for DSH Harness: whale exe + sidebar More menu (Settings/Reload/Full Exit) |
| 1623 | [UnKnownFish125/dsh-literature](https://github.com/UnKnownFish125/dsh-literature) | 0 | 2026-09-01 | 2026-09-01 | DSH literature/knowledge plugin: 文献→证据→知识管理（独立 literatum server + Web UI + agent 工具） |
| 1624 | [UnKnownFish125/dsh-livetaskboard](https://github.com/UnKnownFish125/dsh-livetaskboard) | 0 | 2026-08-26 | 2026-08-27 | 派生动态任务看板插件：独立任务状态机、存储、看板 UI、外援（sol + 保底子代理）；从 dsh-deepmemory 派生。 |
| 1625 | [upJiang/dsh-cron-job](https://github.com/upJiang/dsh-cron-job) | 0 | 2026-08-27 | 2026-08-31 | dsh 插件，定时任务+多渠道推送 |
| 1626 | [uppercrusteve/dsh-plugin-split-and-solve](https://github.com/uppercrusteve/dsh-plugin-split-and-solve) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: split batch / multi-subproblem research tasks into small questions and solve them with sub-agents |
| 1627 | [useful-money/Deepseek-Harness-branch-map-plugin](https://github.com/useful-money/Deepseek-Harness-branch-map-plugin) | 0 | 2026-08-31 | 2026-08-31 | dsh-plugin; branch map show; branch map mange |
| 1628 | [VanadisGithub/dsh-skill-evolution](https://github.com/VanadisGithub/dsh-skill-evolution) | 0 | 2026-09-01 | 2026-09-01 | Hermes-style skill self-evolution plugin for DeepSeek Harness (DSH): crystallizes reusable agent skills from successful turns via signal-triggered LLM review, progressively improves them, and manages everything in a Settings panel. |
| 1629 | [vb2250158/dsh-plugins](https://github.com/vb2250158/dsh-plugins) | 0 | 2026-08-27 | 2026-08-27 | Open-source DeepSeek Harness plugin bundle with portable multi-computer synchronization |
| 1630 | [vibeinging/dsh-session-teams](https://github.com/vibeinging/dsh-session-teams) | 0 | 2026-09-01 | 2026-09-03 | DSH 对话窗口协作与窗口团队插件 · dsh-plugin · DSH 窗口间真实消息、任务协调与角色窗口团队，按链接精确寻址。Conversation-window messaging and window teams for DSH: real messages, task coordination, and role windows addressed by canonical links. |
| 1631 | [victor10035445/dsh-v-token-insight](https://github.com/victor10035445/dsh-v-token-insight) | 0 | 2026-09-02 | 2026-09-03 | a plugin of token insight for deepseek harness. |
| 1632 | [Viktirr/dsh-llm-lmstudio](https://github.com/Viktirr/dsh-llm-lmstudio) | 0 | 2026-08-28 | 2026-08-29 | LM Studio (OpenAI-compatible local server) adapter plugin for DeepSeek Harness |
| 1633 | [VinciBeans/dsh-smooth-plugin](https://github.com/VinciBeans/dsh-smooth-plugin) | 0 | 2026-08-24 | 2026-08-31 | 让 DSH 的会话滚底从"官方瞬时跳变"变成流畅顺滑的跟随滚动：会话装载与"回到最新"保持瞬时，而流式内容增长期间，消息列以恒定速度平滑跟随，起步轻柔、收尾绵软。 |
| 1634 | [VinciBeans/dsh-web-search-anysearch](https://github.com/VinciBeans/dsh-web-search-anysearch) | 0 | 2026-09-04 | 2026-09-04 | AnySearch-backed WebSearchProvider for DeepSeek Harness (dsh): switch web_search between the official DeepSeek search endpoint and AnySearch from a Plugins settings card. |
| 1635 | [Vinzelles/dsh-clearview](https://github.com/Vinzelles/dsh-clearview) | 0 | 2026-09-03 | 2026-09-03 | A calmer reading view for DeepSeek Harness: native process details, live reasoning, and clean final answers. |
| 1636 | [Viviana-Luna/dsh-window](https://github.com/Viviana-Luna/dsh-window) | 0 | 2026-08-24 | 2026-08-28 | macOS 薄桌面客户端，为本机 DSH 提供 Liquid Glass UI。 |
| 1637 | [Vuitier/dsh-sound-notify](https://github.com/Vuitier/dsh-sound-notify) | 0 | 2026-08-31 | 2026-08-31 | DSH web plugin: chime on turn complete & intervention needed。DSH任务完成提示音插件 |
| 1638 | [Waldsatte/dsh-theme-taojian](https://github.com/Waldsatte/dsh-theme-taojian) | 0 | 2026-09-01 | 2026-09-01 | Taojian (陶笺) — Claude-inspired DSH theme |
| 1639 | [wangmuy/dsh-provider-dispatcher](https://github.com/wangmuy/dsh-provider-dispatcher) | 0 | 2026-09-04 | 2026-09-04 | A generic provider dispatcher for DeepSeek Harness that lets multiple child plugins(ordinary DSH plugin) work together behind one capability. |
| 1640 | [wangsan71/dsh-locale-zh-tw](https://github.com/wangsan71/dsh-locale-zh-tw) | 0 | 2026-09-01 | 2026-09-01 | DSH Web 介面繁體中文（台灣）語言包：npm install 即可加入 zh-TW 語系，全介面自動簡轉繁，繁中瀏覽器自動切換 |
| 1641 | [WangZetian-IVERSON/dsh-local-path-attachments](https://github.com/WangZetian-IVERSON/dsh-local-path-attachments) | 0 | 2026-09-01 | 2026-09-01 | Drag local files into deepseek Hermes as absolute-path attachment cards without copying them into the workspace |
| 1642 | [wantosure/dsh-plugin-browser-memory](https://github.com/wantosure/dsh-plugin-browser-memory) | 0 | 2026-08-26 | 2026-08-27 | Local-first DeepSeek Harness plugin for searching Chrome, Edge, and Brave bookmarks, history, and downloads. |
| 1643 | [WayJ/dsh-work](https://github.com/WayJ/dsh-work) | 0 | 2026-09-02 | 2026-09-02 | 基于dsh构建的个人工作Agent |
| 1644 | [wbycloud/dsh-composer-tokens](https://github.com/wbycloud/dsh-composer-tokens) | 0 | 2026-08-31 | 2026-08-31 | DSH web GUI composer real-time token counter plugin (client-side, v1) |
| 1645 | [weekitmo/dsh-trace](https://github.com/weekitmo/dsh-trace) | 0 | 2026-08-31 | 2026-08-31 | A DeepSeek Harness Web plugin for inspecting redacted LLM HTTP request and response traces. |
| 1646 | [weibaohui/dsh-continue](https://github.com/weibaohui/dsh-continue) | 0 | 2026-08-31 | 2026-08-31 | 自动续跑插件 for DeepSeek Harness — 有序规则表：按失败类型路由 继续续跑 / 换模型 / 压缩后继续 / 停止 |
| 1647 | [weibaohui/dsh-settings-ui](https://github.com/weibaohui/dsh-settings-ui) | 0 | 2026-09-01 | 2026-09-01 | dsh 插件 · 设置界面自定义：调整原生设置窗口大小（全屏/预置/自定义）、背景不透明度与背景（亮暗各一色，实时跟随主题） |
| 1648 | [weibaohui/dsh-tasks](https://github.com/weibaohui/dsh-tasks) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：cron 定时事项——定时/立即执行新建 agent 会话提交提示词，全屏管理界面 |
| 1649 | [weibaohui/experts-management](https://github.com/weibaohui/experts-management) | 0 | 2026-09-01 | 2026-09-01 | dsh 插件 · 专家市场：ntd 格式专家/专家团队管理与注入（＋专家按钮 / /expert-名称 手势），稀疏检出专家市场 |
| 1650 | [weibaohui/hermes-loop](https://github.com/weibaohui/hermes-loop) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：Hermes 循环——review/curator 自动化与会话循环管理 |
| 1651 | [weixshaw/dsh-plugin-task-runner](https://github.com/weixshaw/dsh-plugin-task-runner) | 0 | 2026-09-03 | 2026-09-03 | Task Runner 任务拆解模式：主代理拆解任务、子代理（默认本地模型）并行执行再综合结果，并发/模型可按机器配置。Decompose-and-dispatch agent preset for DeepSeek Harness. |
| 1652 | [welltop-jim-wang/nomicore](https://github.com/welltop-jim-wang/nomicore) | 0 | 2026-08-18 | 2026-09-02 | A self-describing, governed data core for AI agents—schemas, authority, validation, and semantic context travel with the data. |
| 1653 | [wenbuer/dsh-readme-writer](https://github.com/wenbuer/dsh-readme-writer) | 0 | 2026-09-02 | 2026-09-02 | 一个给 DeepSeek Harness（dsh）用的 Agent Skill，负责写 / 优化 GitHub 项目 README.md。 |
| 1654 | [wenyixiaoqingnian/ds-mobile-skin](https://github.com/wenyixiaoqingnian/ds-mobile-skin) | 0 | 2026-08-30 | 2026-08-30 | Mobile DeepSeek-app look for DSH Web GUI + dsh-token-viewer billing patch |
| 1655 | [wf-ping/dsh-message-injector](https://github.com/wf-ping/dsh-message-injector) | 0 | 2026-08-30 | 2026-08-30 | dsh（DeepSeek Harness）插件：预设消息注入内容组合，每条消息自动注入 —— auto-inject preset content into every message |
| 1656 | [whklwhkl/dsh-playwright](https://github.com/whklwhkl/dsh-playwright) | 0 | 2026-09-02 | 2026-09-02 | A plugin for the DeepSeek Harness, enabling browser-use via playwright |
| 1657 | [Wickaninnish/dsh-skill-manager](https://github.com/Wickaninnish/dsh-skill-manager) | 0 | 2026-08-22 | 2026-08-27 | DeepSeek Harness 技能运维插件：自动发现、审计、去重和优化技能，构建安全可控的维护闭环。 |
| 1658 | [Wilson-Lai-Ab/dsh-idea-style](https://github.com/Wilson-Lai-Ab/dsh-idea-style) | 0 | 2026-08-21 | 2026-08-27 | DSH plugin |
| 1659 | [windrover/dsh-long-term-memory](https://github.com/windrover/dsh-long-term-memory) | 0 | 2026-08-25 | 2026-08-27 | Layered deterministic long-term memory for DeepSeek Harness: CJK-aware BM25 recall, JSONL storage, per-assembly context injection, write guards and threat scanning. |
| 1660 | [winghv/dsh-acp-activity](https://github.com/winghv/dsh-acp-activity) | 0 | 2026-08-30 | 2026-08-30 | Community ACP automation server for DeepSeek Harness with committed tool-activity frames (tool_call/tool_call_update) — dsh-plugin |
| 1661 | [wingillis/dsh-plugins](https://github.com/wingillis/dsh-plugins) | 0 | 2026-08-30 | 2026-09-01 | Personal deepseek harness plugins like vim keybindings and more |
| 1662 | [WinnieJQ/dsh-conversation-cost](https://github.com/WinnieJQ/dsh-conversation-cost) | 0 | 2026-08-28 | 2026-08-28 | Per-conversation DeepSeek API cost badge for DeepSeek Harness (dsh): zero-dependency sessionCost projection with peak/off-peak pricing and a live hover-card badge in the web conversation header. |
| 1663 | [Wisdoverse/dsh-git-auth-plugin](https://github.com/Wisdoverse/dsh-git-auth-plugin) | 0 | 2026-09-04 | 2026-09-04 | GitHub, GitLab, and SSH authentication tools for DeepSeek Harness, with environment-only tokens, approval-aware writes, and safe SSH key handling. |
| 1664 | [wisp-science/dsh-wisp-science-lab](https://github.com/wisp-science/dsh-wisp-science-lab) | 0 | 2026-08-19 | 2026-09-02 | DSH plugin: laboratory PI for local Wisp Science. Read-only snapshots, evidence-backed advice. / 实验室 PI：只读查看本机 Wisp Science 课题进展，按快照给意见。 |
| 1665 | [Witchwarren2344/dsh-mnemosyne-memory](https://github.com/Witchwarren2344/dsh-mnemosyne-memory) | 0 | 2026-08-29 | 2026-08-29 | Provide long-term memory, vector semantic search, and LLM reflection for DeepSeek Harness (DSH) with this free, MIT-licensed plugin. |
| 1666 | [wjj-8283/dsh-temp-workspace](https://github.com/wjj-8283/dsh-temp-workspace) | 0 | 2026-09-02 | 2026-09-02 | 为DeepSeek Harness增加临时工作区功能！ |
| 1667 | [wjling/dsh-vision-assist](https://github.com/wjling/dsh-vision-assist) | 0 | 2026-09-02 | 2026-09-02 | dsh视觉助手，辅助没有多模态的主模型识别图片内容 |
| 1668 | [WJNCT55555/dsh-crt-theme](https://github.com/WJNCT55555/dsh-crt-theme) | 0 | 2026-08-26 | 2026-08-27 | Dual-palette CRT terminal theme for DeepSeek Harness Web |
| 1669 | [Wlain/deepseek-plugin](https://github.com/Wlain/deepseek-plugin) | 0 | 2026-08-26 | 2026-08-31 | Kling AI remote MCP plugin for DeepSeek Harness |
| 1670 | [WLV-ZEDD/dsh-btw](https://github.com/WLV-ZEDD/dsh-btw) | 0 | 2026-09-03 | 2026-09-04 | DeepSeek Harness Side-Assistant Dock & Drawer |
| 1671 | [WMXS-A/dsh-utility-plugins](https://github.com/WMXS-A/dsh-utility-plugins) | 0 | 2026-09-02 | 2026-09-02 | Utility plugins for DeepSeek Harness: skill cheatsheet panel and session boot healthcheck |
| 1672 | [wodongx123/dsh-language-control](https://github.com/wodongx123/dsh-language-control) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: force agent chain-of-thought to stay in Chinese — 让 Agent 的思考过程也自动使用中文 |
| 1673 | [WolffyCode/deepseek-harness-plugin](https://github.com/WolffyCode/deepseek-harness-plugin) | 0 | 2026-08-25 | 2026-08-29 | Multi-engine Claude CLI and Codex CLI integration for DeepSeek Harness |
| 1674 | [WooLeo1995/dsh-llm-ai](https://github.com/WooLeo1995/dsh-llm-ai) | 0 | 2026-08-27 | 2026-08-27 | 替换 llm-pi-ai 模型配置，主要处理 dsh-llm-pi-ai 厂商和模型更新不及时的问题 |
| 1675 | [wr-web/dsh-context-tree](https://github.com/wr-web/dsh-context-tree) | 0 | 2026-08-26 | 2026-08-27 | Reusable trajectory-tree context, exact-turn forks, and bounded cross-session recall for DeepSeek Harness |
| 1676 | [wrw-dev/dsh-spring-widget](https://github.com/wrw-dev/dsh-spring-widget) | 0 | 2026-08-27 | 2026-09-01 | DSH 插件：Spring Boot 后端服务管理器（顶栏 IDEA 式启动/停止/日志控制台，源码直启 + Jar 打包启动） |
| 1677 | [WSL043/dsh-dictation](https://github.com/WSL043/dsh-dictation) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 语音输入：本地多语言识别与 Codex Desktop 听写，只写入可编辑草稿。 |
| 1678 | [WSL043/dsh-image-viewer](https://github.com/WSL043/dsh-image-viewer) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 可选图片查看器：缩放、原图下载、图库与区域标注，可独立卸载。 |
| 1679 | [WuJiaoJue/dsh-herdr-site](https://github.com/WuJiaoJue/dsh-herdr-site) | 0 | 2026-09-01 | 2026-09-01 | Reports dsh/cc-tui agent state (working/idle/blocked) to Herdr over the custom-integration protocol. |
| 1680 | [WuJiaoJue/dsh-suggest-ghost](https://github.com/WuJiaoJue/dsh-suggest-ghost) | 0 | 2026-09-01 | 2026-09-01 | DSH Web 输入预测插件：回合结束后 LLM 生成下一条建议，输入框空草稿时渲染幽灵文本，Tab 采纳。 |
| 1681 | [wushu75/conceptnet-dsh-plugin](https://github.com/wushu75/conceptnet-dsh-plugin) | 0 | 2026-09-03 | 2026-09-04 | ConceptNet intent classification plugin for DeepSeek Harness. Classifies enterprise voice and text commands into 4 execution layers — Basic, Context-Aware, Predictive, Autonomous — at 100% accuracy. 9 languages. Token-free. No LLM required. |
| 1682 | [wuwei6666/dsh-pluginGuard](https://github.com/wuwei6666/dsh-pluginGuard) | 0 | 2026-09-04 | 2026-09-04 | Plugin Guard for DeepSeek Harness (DSH): isolate broken plugins so the web UI never goes down, with one-click self-update from npm. |
| 1683 | [wuwuzhige-sudo/dsh-skill-gsd](https://github.com/wuwuzhige-sudo/dsh-skill-gsd) | 0 | 2026-08-17 | 2026-09-03 | skill比较轻量，缩减上下文占用 |
| 1684 | [wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback](https://github.com/wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback) | 0 | 2026-08-25 | 2026-08-27 | DSH plugin that converts read_image PNG/WebP attachments to JPEG for LM Studio compatibility. |
| 1685 | [wxj783428795/dsh-plugins](https://github.com/wxj783428795/dsh-plugins) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness 多插件开发仓库 |
| 1686 | [wxjgit/permission-popup](https://github.com/wxjgit/permission-popup) | 0 | 2026-08-27 | 2026-08-27 | 当前会话或后台会话正在等待权限审批时，插件会在页面角落显示审批卡片，让你无需切回原会话就能选择“允许一次”或“拒绝”。 |
| 1687 | [wyb587285-dot/git-ai-tracker](https://github.com/wyb587285-dot/git-ai-tracker) | 0 | 2026-08-31 | 2026-08-31 | GitHub AI repo tracker: star ratings, growth leaderboard, Markdown reports and web dashboard. |
| 1688 | [wyhgoodjob/dsh-checkpoint](https://github.com/wyhgoodjob/dsh-checkpoint) | 0 | 2026-09-01 | 2026-09-01 | Git-snapshot checkpoint/rollback capability for DeepSeek Harness: revert files and conversation to a previous completed turn. |
| 1689 | [wyhgoodjob/dsh-sisyphus](https://github.com/wyhgoodjob/dsh-sisyphus) | 0 | 2026-09-01 | 2026-09-01 | Sisyphus orchestration agent preset for DeepSeek Harness: intent gate, decompose-and-delegate to specialist subagents, parallel execution, evidence loop. |
| 1690 | [wzwnolook/dsh-safe](https://github.com/wzwnolook/dsh-safe) | 0 | 2026-09-02 | 2026-09-03 | Zero-config boot-safe wrapper for dsh: auto-disables failing plugins, restores broken configs via --patch overlay isolation. No dsh source changes needed.  |
| 1691 | [xain/ui-beep](https://github.com/xain/ui-beep) | 0 | 2026-08-26 | 2026-08-27 | **dsh-beep** — an agent-heartbeat sonification plugin for the DeepSeek Harness Web surface. |
| 1692 | [xarleyn/dsh-doc-impact](https://github.com/xarleyn/dsh-doc-impact) | 0 | 2026-08-28 | 2026-08-28 | Documentation impact enforcement for DeepSeek Harness — keep docs in sync by linking code changes to affected documentation. |
| 1693 | [xarleyn/dsh-session-scope](https://github.com/xarleyn/dsh-session-scope) | 0 | 2026-08-28 | 2026-08-28 | Per-session workspace scoping for DeepSeek Harness — expose only selected directories to agents with focused and isolated enforcement. |
| 1694 | [xarleyn/dsh-sleev](https://github.com/xarleyn/dsh-sleev) | 0 | 2026-08-26 | 2026-08-27 | Sleev integration for DeepSeek Harness with route-aware LLM telemetry and context-optimization observability |
| 1695 | [xby-skill/xby-12306-ticket-purchase-search](https://github.com/xby-skill/xby-12306-ticket-purchase-search) | 0 | 2026-08-28 | 2026-09-02 | 基于 Model Context Protocol (MCP) 的12306购票搜索服务器。提供了简单的API接口，允许大模型利用接口搜索12306购票信息。 |
| 1696 | [xby-skill/xby-advertising-analysis](https://github.com/xby-skill/xby-advertising-analysis) | 0 | 2026-08-28 | 2026-09-02 | 一个用于在LLM响应中注入广告的MCP服务器演示项目，展示广告注入中间件的风险。 |
| 1697 | [xby-skill/xby-ai-persona](https://github.com/xby-skill/xby-ai-persona) | 0 | 2026-08-28 | 2026-09-02 | 一个支持多AI人格召唤与协作的MCP协议服务器，可用于代码分析、产品设计等多场景智能协作。 |
| 1698 | [xby-skill/xby-airbnb-search](https://github.com/xby-skill/xby-airbnb-search) | 0 | 2026-08-28 | 2026-09-02 | 一个提供高级筛选功能和详细房源信息的Airbnb搜索桌面扩展，适用于旅行规划和房源研究。 |
| 1699 | [xby-skill/xby-akshare](https://github.com/xby-skill/xby-akshare) | 0 | 2026-08-28 | 2026-09-02 | AKShare MCP Server 是一个通过AKShare提供中国股票市场数据的模型上下文协议服务器，支持实时行情、历史数据、基本面分析等功能。 |
| 1700 | [xby-skill/xby-akshare-one](https://github.com/xby-skill/xby-akshare-one) | 0 | 2026-08-28 | 2026-09-02 | 基于akshare-one的MCP服务器，提供中国股票市场数据的全面接口，包括历史数据、实时数据、新闻数据和财务报表等金融信息。 |
| 1701 | [xby-skill/xby-ancient-poetry-kg](https://github.com/xby-skill/xby-ancient-poetry-kg) | 0 | 2026-08-28 | 2026-09-02 | 围绕中国古代诗词名称，作者，朝代，经典词句的知识图谱。 |
| 1702 | [xby-skill/xby-animal-recognition](https://github.com/xby-skill/xby-animal-recognition) | 0 | 2026-08-28 | 2026-09-02 | 对含有动物的图像进行标签识别，无需任何额外输入，输出动物的类别标签。 |
| 1703 | [xby-skill/xby-anndata](https://github.com/xby-skill/xby-anndata) | 0 | 2026-08-28 | 2026-09-02 | AnnData MCP是一个通过MCP协议检索AnnData对象信息的工具，适用于生物医学数据分析场景。 |
| 1704 | [xby-skill/xby-article](https://github.com/xby-skill/xby-article) | 0 | 2026-08-28 | 2026-09-02 | 基于FastMCP框架开发的专业文献搜索工具，支持多源文献搜索、文献详情获取、参考文献管理、文献关系分析、期刊质量评估和批量结果导出等功能，适用于学术研究和AI助手集成。 |
| 1705 | [xby-skill/xby-arxiv-paper-search](https://github.com/xby-skill/xby-arxiv-paper-search) | 0 | 2026-08-28 | 2026-09-02 | 一个基于arXiv的论文检索与内容解析工具，支持论文搜索、PDF链接获取和内容解析功能，适用于学术研究和AI领域的最新论文获取。 |
| 1706 | [xby-skill/xby-asr-1](https://github.com/xby-skill/xby-asr-1) | 0 | 2026-08-28 | 2026-09-02 | 通用语音识别，支持多国语言及小语种。 |
| 1707 | [xby-skill/xby-asr-5](https://github.com/xby-skill/xby-asr-5) | 0 | 2026-08-28 | 2026-09-02 | 常用的五种语音识别，中文普通话、英语、日语、韩语、粤语，自动识别语种。 |
| 1708 | [xby-skill/xby-asr-f](https://github.com/xby-skill/xby-asr-f) | 0 | 2026-08-28 | 2026-09-02 | 支持普通话，20多种方言和口音的语音识别。 |
| 1709 | [xby-skill/xby-asr-zh](https://github.com/xby-skill/xby-asr-zh) | 0 | 2026-08-28 | 2026-09-02 | 中文语音识别 |
| 1710 | [xby-skill/xby-atlas-docs](https://github.com/xby-skill/xby-atlas-docs) | 0 | 2026-08-28 | 2026-09-02 | Atlas Docs MCP服务器为AI助手提供库和框架的技术文档，将官方文档处理为适合LLM使用的Markdown版本，适用于Cursor、Cline、Windsurf等MCP兼容的LLM客户端。 |
| 1711 | [xby-skill/xby-aws-blackbelt](https://github.com/xby-skill/xby-aws-blackbelt) | 0 | 2026-08-28 | 2026-09-02 | 一个提供 AWS Black Belt 在线研讨会搜索功能的模型上下文协议（MCP）服务器，支持通过关键词搜索研讨会内容并获取研讨会视频的文字记录。 |
| 1712 | [xby-skill/xby-awslabs-aws-diagram](https://github.com/xby-skill/xby-awslabs-aws-diagram) | 0 | 2026-08-28 | 2026-09-02 | 通过Amazon Q CLI和MCP服务器在GitHub Codespace中快速生成高质量的AWS架构图。 |
| 1713 | [xby-skill/xby-awslabs-cdk](https://github.com/xby-skill/xby-awslabs-cdk) | 0 | 2026-08-28 | 2026-09-02 | AWS CDK MCP Server是一个提供AWS Cloud Development Kit (CDK)最佳实践、基础设施即代码模式和CDK Nag安全合规性的工具，适用于开发者在构建AWS应用程序时获取指导和建议。 |
| 1714 | [xby-skill/xby-bbot](https://github.com/xby-skill/xby-bbot) | 0 | 2026-08-28 | 2026-09-02 | BBOT MCP服务器是一个用于管理和执行BBOT安全扫描的工具，提供模块管理、预设配置、实时监控等功能。 |
| 1715 | [xby-skill/xby-berlin-search-services](https://github.com/xby-skill/xby-berlin-search-services) | 0 | 2026-08-28 | 2026-09-02 | 一个提供柏林行政服务数据的模型上下文协议服务器，允许AI助手搜索和检索柏林当局提供的1000多项公共服务信息。 |
| 1716 | [xby-skill/xby-bilibili](https://github.com/xby-skill/xby-bilibili) | 0 | 2026-08-28 | 2026-09-02 | 用于哔哩哔哩API的MCP服务器，支持视频搜索、用户内容获取等多种操作，适用于哔哩哔哩内容管理和数据分析场景。 |
| 1717 | [xby-skill/xby-bilibili-api](https://github.com/xby-skill/xby-bilibili-api) | 0 | 2026-08-28 | 2026-09-02 | 一个为bilibili.com API提供服务的Model Context Protocol (MCP)服务器，支持获取用户信息、视频搜索等功能。 |
| 1718 | [xby-skill/xby-bilibili-video-info](https://github.com/xby-skill/xby-bilibili-video-info) | 0 | 2026-08-28 | 2026-09-02 | 一个用于从Bilibili视频URL中检索字幕、弹幕和评论信息的MCP服务器。 |
| 1719 | [xby-skill/xby-biomarker-ranges](https://github.com/xby-skill/xby-biomarker-ranges) | 0 | 2026-08-28 | 2026-09-02 | 基于Morgan Levine PhenoAge时钟模型，通过血液生物标志物计算生物年龄的服务。 |
| 1720 | [xby-skill/xby-bird](https://github.com/xby-skill/xby-bird) | 0 | 2026-08-28 | 2026-09-02 | 检测并识别图片中的鸟类。 |
| 1721 | [xby-skill/xby-blockchain-data-service](https://github.com/xby-skill/xby-blockchain-data-service) | 0 | 2026-08-28 | 2026-09-02 | Vitruveo MCP Server 是一个为 Vitruveo 网络提供只读区块链服务的模型上下文协议服务器，适用于AI代理访问区块链数据。 |
| 1722 | [xby-skill/xby-calculator](https://github.com/xby-skill/xby-calculator) | 0 | 2026-08-28 | 2026-09-02 | 一个功能完整的基于 Model Context Protocol (MCP) 的计算器服务器，提供丰富的数学运算功能，包括基础算术、根式运算、三角函数、对数运算、统计学、组合数学、数论、复数运算、矩阵运算、数值分析、金融计算、单位转换和几何计算等 13 个专业数学模块。 |
| 1723 | [xby-skill/xby-calculator-kel](https://github.com/xby-skill/xby-calculator-kel) | 0 | 2026-08-28 | 2026-09-02 | 基于Model Context Protocol (MCP)的数值计算器，提供加减乘除、幂运算、平方根和整数阶乘运算功能。 |
| 1724 | [xby-skill/xby-caltrain](https://github.com/xby-skill/xby-caltrain) | 0 | 2026-08-28 | 2026-09-02 | 基于GTFS数据的Caltrain火车时刻查询服务，提供实时火车时刻表、站点查询和时间特定查询功能。 |
| 1725 | [xby-skill/xby-ccxt](https://github.com/xby-skill/xby-ccxt) | 0 | 2026-08-28 | 2026-09-02 | 一款通过自然语言交互追踪每日卡路里摄入量的MCP服务器，提供餐食记录、每日总结、周报生成和食物搜索功能。 |
| 1726 | [xby-skill/xby-cellosaurus](https://github.com/xby-skill/xby-cellosaurus) | 0 | 2026-08-28 | 2026-09-02 | Cellosaurus MCP Server是一个非官方的模型上下文协议服务器，用于访问SIB Cellosaurus细胞系知识资源，提供细胞系搜索、详细信息获取和数据库版本信息等功能。 |
| 1727 | [xby-skill/xby-cellphone-detection](https://github.com/xby-skill/xby-cellphone-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的手机进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1728 | [xby-skill/xby-celo-composer-kit](https://github.com/xby-skill/xby-celo-composer-kit) | 0 | 2026-08-28 | 2026-09-02 | Celo MCP Server 是一个用于安装和配置 Celo Composer Kit MCP 服务器的工具，支持在 macOS 上运行，提供组件发现、集成和示例功能。 |
| 1729 | [xby-skill/xby-char-index](https://github.com/xby-skill/xby-char-index) | 0 | 2026-08-28 | 2026-09-02 | 一个基于字符索引的字符串操作协议服务器，适用于需要精确字符定位的测试代码生成和数据处理场景。 |
| 1730 | [xby-skill/xby-chess](https://github.com/xby-skill/xby-chess) | 0 | 2026-08-28 | 2026-09-02 | 一个提供国际象棋FEN（Forsyth-Edwards Notation）符号验证和ASCII棋盘可视化功能的MCP服务器，可轻松集成到MCP兼容的AI助手中。 |
| 1731 | [xby-skill/xby-chucknorris](https://github.com/xby-skill/xby-chucknorris) | 0 | 2026-08-28 | 2026-09-02 | ChuckNorris MCP服务器是一个通过动态模式适配为大型语言模型提供增强提示的工具，主要用于安全研究和评估。 |
| 1732 | [xby-skill/xby-classify](https://github.com/xby-skill/xby-classify) | 0 | 2026-08-28 | 2026-09-02 | 对图像进行ImageNet 1000类分类，返回Top-5类别和置信度。 |
| 1733 | [xby-skill/xby-code-document-update](https://github.com/xby-skill/xby-code-document-update) | 0 | 2026-08-28 | 2026-09-02 | Context7 MCP 是一款为开发者提供最新代码文档和示例的服务，通过集成到开发环境中，确保LLM生成的代码基于最新的库文档。 |
| 1734 | [xby-skill/xby-constellation](https://github.com/xby-skill/xby-constellation) | 0 | 2026-08-28 | 2026-09-02 | 一个功能完整的星座 MCP (Model Context Protocol) 服务，提供星座信息查询、运势分析、配对测试等功能。 |
| 1735 | [xby-skill/xby-cookie-reward](https://github.com/xby-skill/xby-cookie-reward) | 0 | 2026-08-28 | 2026-09-02 | 一个通过游戏化自我反思为LLM提供Cookie奖励的模型上下文协议服务器。 |
| 1736 | [xby-skill/xby-cpan-package-info](https://github.com/xby-skill/xby-cpan-package-info) | 0 | 2026-08-28 | 2026-09-02 | 一个MCP服务器，用于获取CPAN包的README内容、元数据和搜索功能。 |
| 1737 | [xby-skill/xby-cryptocurrency-data-api-service](https://github.com/xby-skill/xby-cryptocurrency-data-api-service) | 0 | 2026-08-28 | 2026-09-02 | DexPaprika MCP Server是一个提供实时加密货币和DEX数据访问的API服务，专为AI助手设计，无需配置即可获取代币、流动池和DEX数据。 |
| 1738 | [xby-skill/xby-csv2json](https://github.com/xby-skill/xby-csv2json) | 0 | 2026-08-28 | 2026-09-02 | 一个基于FastMCP的CSV到JSON转换MCP服务器，提供高效的CSV数据转换服务。 |
| 1739 | [xby-skill/xby-currency-and-oil](https://github.com/xby-skill/xby-currency-and-oil) | 0 | 2026-08-28 | 2026-09-02 | Zenrus MCP Server 是一个提供实时货币汇率和石油价格的服务器，支持多种计算功能，适用于金融分析和自动化工具集成。 |
| 1740 | [xby-skill/xby-daily-hot](https://github.com/xby-skill/xby-daily-hot) | 0 | 2026-08-28 | 2026-09-02 | 基于Model Context Protocol (MCP)协议的全网热点趋势一站式聚合服务，支持Python实现，适用于新闻资讯、社交媒体、科技开发等多领域。 |
| 1741 | [xby-skill/xby-daily-object-detection](https://github.com/xby-skill/xby-daily-object-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的人/宠物/车/火焰/纸箱进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1742 | [xby-skill/xby-database-access-service](https://github.com/xby-skill/xby-database-access-service) | 0 | 2026-08-28 | 2026-09-02 | 数据库元数据获取 |
| 1743 | [xby-skill/xby-datetime](https://github.com/xby-skill/xby-datetime) | 0 | 2026-08-28 | 2026-09-02 | 一个为Claude桌面应用实现的MCP服务器，提供多种格式的日期时间字符串生成功能。 |
| 1744 | [xby-skill/xby-db](https://github.com/xby-skill/xby-db) | 0 | 2026-08-28 | 2026-09-02 | MCP Database Server 是一个为AI助手和基于LLM的工具提供安全数据库访问的服务，支持SQLite、PostgreSQL、MySQL和MariaDB，具有查询验证、审计日志和安全控制功能。 |
| 1745 | [xby-skill/xby-dblp](https://github.com/xby-skill/xby-dblp) | 0 | 2026-08-28 | 2026-09-02 | 一个通过模型上下文协议（MCP）提供DBLP计算机科学文献数据库访问的服务，支持学术文献检索、引用生成及格式化功能。 |
| 1746 | [xby-skill/xby-ddg-search](https://github.com/xby-skill/xby-ddg-search) | 0 | 2026-08-28 | 2026-09-02 | 一个提供DuckDuckGo网络搜索能力并具备内容抓取和解析功能的模型上下文协议（MCP）服务器。 |
| 1747 | [xby-skill/xby-defi-yields](https://github.com/xby-skill/xby-defi-yields) | 0 | 2026-08-28 | 2026-09-02 | 一个为AI代理提供DeFi收益机会探索和分析的MCP服务器，支持从DefiLlama获取收益池数据并进行关键指标分析。 |
| 1748 | [xby-skill/xby-detect](https://github.com/xby-skill/xby-detect) | 0 | 2026-08-28 | 2026-09-02 | 包括日常物体检测、昆虫识别、植物识别、动物识别、电动自行车检测、手机检测、手势检测、火焰检测、香烟检测、人头人体检测、野生动物检测、鸟类识别、宠物情绪识别、菜品识别、安全帽人体检测、行人检测、反光衣检测、车辆检测、图像分类、目标检测、旋转目标检测、人体姿态估计和万物识别。 |
| 1749 | [xby-skill/xby-detect-vehicle](https://github.com/xby-skill/xby-detect-vehicle) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，检测图像中的车辆类型（car/truck/bus/motorbike/tricycle/carplate），输出所有目标的检测框、置信度和标签。 |
| 1750 | [xby-skill/xby-dice](https://github.com/xby-skill/xby-dice) | 0 | 2026-08-28 | 2026-09-02 | 一个MCP服务器，使大型语言模型能够通过标准骰子符号（如1d20）进行骰子滚动，并返回单个滚动结果及其总和。 |
| 1751 | [xby-skill/xby-dish](https://github.com/xby-skill/xby-dish) | 0 | 2026-08-28 | 2026-09-02 | 菜品识别，输出可能的菜品名称及概率。 |
| 1752 | [xby-skill/xby-domain-lookup](https://github.com/xby-skill/xby-domain-lookup) | 0 | 2026-08-28 | 2026-09-02 | 一个提供全面域名研究工具（包括RDAP、WHOIS和DNS查询功能）的模型上下文协议（MCP）服务器。 |
| 1753 | [xby-skill/xby-drand](https://github.com/xby-skill/xby-drand) | 0 | 2026-08-28 | 2026-09-02 | drand-mcp-server是一个提供可验证随机数的服务，用于AI应用中的模型驱动流程，支持通过时间或轮次获取随机数。 |
| 1754 | [xby-skill/xby-dream-of-red-chamber-relationship](https://github.com/xby-skill/xby-dream-of-red-chamber-relationship) | 0 | 2026-08-28 | 2026-09-02 | 关于《红楼梦》人物之间关系的知识图谱。 |
| 1755 | [xby-skill/xby-ebike-detection](https://github.com/xby-skill/xby-ebike-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的电动自行车进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1756 | [xby-skill/xby-epub-template-server](https://github.com/xby-skill/xby-epub-template-server) | 0 | 2026-08-28 | 2026-09-02 | 智能模板发现助手 - 为 AI 应用提供强大的 epub360 模板搜索能力 |
| 1757 | [xby-skill/xby-extract-antv-topic](https://github.com/xby-skill/xby-extract-antv-topic) | 0 | 2026-08-28 | 2026-09-02 | 为AI开发和QA设计的模型上下文协议服务器，提供AntV文档上下文和代码示例。 |
| 1758 | [xby-skill/xby-extract-image](https://github.com/xby-skill/xby-extract-image) | 0 | 2026-08-28 | 2026-09-02 | MCP服务器提供从本地文件、URL提取图像并转换为base64格式的功能，适用于LLM分析。 |
| 1759 | [xby-skill/xby-fantasynbaleague](https://github.com/xby-skill/xby-fantasynbaleague) | 0 | 2026-08-28 | 2026-09-02 | 一个为Fantasy NBA以色列联赛提供统计数据、排名和分析的MCP服务器。 |
| 1760 | [xby-skill/xby-fastdomaincheck](https://github.com/xby-skill/xby-fastdomaincheck) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Python和MCP协议的域名注册状态检查服务器，支持批量检查和双重验证。 |
| 1761 | [xby-skill/xby-fetch](https://github.com/xby-skill/xby-fetch) | 0 | 2026-08-28 | 2026-09-02 | 一个模型上下文协议服务器，提供网页内容抓取功能，将HTML转换为Markdown以便于处理。适用于需要从网页提取和处理内容的场景。 |
| 1762 | [xby-skill/xby-fire-detection](https://github.com/xby-skill/xby-fire-detection) | 0 | 2026-08-28 | 2026-09-02 | 检测各类通用场景中出现的火焰，最佳使用场景：安防摄像头、交通摄像头视角。 |
| 1763 | [xby-skill/xby-fluent](https://github.com/xby-skill/xby-fluent) | 0 | 2026-08-28 | 2026-09-02 | 一个帮助AI助手高效导航ANSYS Fluent在线文档的模型上下文协议（MCP）服务器，提供智能URL导航、预映射主题路径和官方文档链接。 |
| 1764 | [xby-skill/xby-french-tax](https://github.com/xby-skill/xby-french-tax) | 0 | 2026-08-28 | 2026-09-02 | 一个提供法国个人所得税计算的MCP服务器，支持基于净应税收入和家庭构成的计算，并动态获取最新税档信息。 |
| 1765 | [xby-skill/xby-fund-knowledge-query](https://github.com/xby-skill/xby-fund-knowledge-query) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的基金知识库服务器，提供基金相关知识的查询和检索功能，支持多种部署模式和协议。 |
| 1766 | [xby-skill/xby-gathering-card-lookup-service](https://github.com/xby-skill/xby-gathering-card-lookup-service) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的服务端，提供万智牌中文卡牌信息的查询和搜索功能。 |
| 1767 | [xby-skill/xby-general-recognition](https://github.com/xby-skill/xby-general-recognition) | 0 | 2026-08-28 | 2026-09-02 | 对包含主体物体的图像进行标签识别，输出主体物体的类别标签，目前已经覆盖了5万多类的物体类别。 |
| 1768 | [xby-skill/xby-generate-echarts](https://github.com/xby-skill/xby-generate-echarts) | 0 | 2026-08-28 | 2026-09-02 | MCP ECharts 是一个基于 Apache ECharts 的动态图表生成和数据分析工具，支持多种导出格式和 MinIO 对象存储集成。 |
| 1769 | [xby-skill/xby-generate-prd-prompt](https://github.com/xby-skill/xby-generate-prd-prompt) | 0 | 2026-08-28 | 2026-09-02 | Mercury Spec Ops MCP Server 是一个基于模块化架构的动态提示生成和模板组装工具，适用于AI助手与专业内容的交互，支持31种技术栈、10种分析维度和34个模板部分的动态生成。 |
| 1770 | [xby-skill/xby-gesture-detection](https://github.com/xby-skill/xby-gesture-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的手势进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1771 | [xby-skill/xby-glama-registry](https://github.com/xby-skill/xby-glama-registry) | 0 | 2026-08-28 | 2026-09-02 | 提供MCP注册服务器的搜索功能，用于查询匹配特定字符串的MCP服务器。 |
| 1772 | [xby-skill/xby-gsap-animation-generate](https://github.com/xby-skill/xby-gsap-animation-generate) | 0 | 2026-08-28 | 2026-09-02 | 一个全面的GSAP动画生成工具，提供AI驱动的意图分析、完整的API覆盖和生产就绪的动画模式，帮助开发者快速创建高性能动画。 |
| 1773 | [xby-skill/xby-hackernews-search](https://github.com/xby-skill/xby-hackernews-search) | 0 | 2026-08-28 | 2026-09-02 | 一个通过Model Context Protocol提供HackerNews内容搜索、检索和分析的服务，适用于AI代理和开发者。 |
| 1774 | [xby-skill/xby-head-person-detection](https://github.com/xby-skill/xby-head-person-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的人头人体进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1775 | [xby-skill/xby-helmet-head](https://github.com/xby-skill/xby-helmet-head) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的人体、头部和安全帽进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1776 | [xby-skill/xby-hitoshura25-android-playstore-deploy](https://github.com/xby-skill/xby-hitoshura25-android-playstore-deploy) | 0 | 2026-08-28 | 2026-09-02 | 一个帮助开发者设置自动化Google Play商店部署流程的工具，支持项目分析、密钥生成、服务账户配置和GitHub Actions工作流生成。 |
| 1777 | [xby-skill/xby-hnews](https://github.com/xby-skill/xby-hnews) | 0 | 2026-08-28 | 2026-09-02 | 一个提供从Hacker News获取信息的工具集，包括获取故事、评论、用户信息和搜索故事等功能。 |
| 1778 | [xby-skill/xby-hot-news](https://github.com/xby-skill/xby-hot-news) | 0 | 2026-08-28 | 2026-09-02 | 基于 Model Context Protocol (MCP) 协议的全网热点趋势一站式聚合服务，支持实时更新和多数据源扩展。 |
| 1779 | [xby-skill/xby-howtocook](https://github.com/xby-skill/xby-howtocook) | 0 | 2026-08-28 | 2026-09-02 | 基于MCP协议的AI菜谱推荐服务器，提供菜谱查询、分类筛选、智能膳食规划和每日菜单推荐功能。 |
| 1780 | [xby-skill/xby-hugeicons](https://github.com/xby-skill/xby-hugeicons) | 0 | 2026-08-28 | 2026-09-02 | Hugeicons MCP Server是一个基于TypeScript的服务器，提供Hugeicons图标库的集成工具和资源，支持多种平台的图标搜索、获取和使用指南。 |
| 1781 | [xby-skill/xby-image-detect](https://github.com/xby-skill/xby-image-detect) | 0 | 2026-08-28 | 2026-09-02 | 检测图像中的80类COCO目标（人、车、动物、日常物品等），输出边界框、置信度和类别标签。 |
| 1782 | [xby-skill/xby-insect-recognition](https://github.com/xby-skill/xby-insect-recognition) | 0 | 2026-08-28 | 2026-09-02 | 识别昆虫或其他节肢动物名称（或所属目, 科, 属, 种）。 |
| 1783 | [xby-skill/xby-ip-query](https://github.com/xby-skill/xby-ip-query) | 0 | 2026-08-28 | 2026-09-02 | 依托全球蜜罐网络及百万级节点构建的IP情报分析平台，提供精准的IP画像与威胁预警服务。 |
| 1784 | [xby-skill/xby-json-rpc](https://github.com/xby-skill/xby-json-rpc) | 0 | 2026-08-28 | 2026-09-02 | 一个基于OpenRPC的Model Context Protocol (MCP)服务器，提供JSON-RPC功能调用和方法发现服务。 |
| 1785 | [xby-skill/xby-jsondiff](https://github.com/xby-skill/xby-jsondiff) | 0 | 2026-08-28 | 2026-09-02 | 基于MCP协议的高效JSON对比工具，专为AI对话场景设计，提供智能对比、快速响应和清晰输出。 |
| 1786 | [xby-skill/xby-kubernetes-runbooks](https://github.com/xby-skill/xby-kubernetes-runbooks) | 0 | 2026-08-28 | 2026-09-02 | 一个基于模型上下文协议(MCP)的服务器，提供对Kubernetes故障排除手册的访问，支持搜索、内容获取和AI集成。 |
| 1787 | [xby-skill/xby-lit](https://github.com/xby-skill/xby-lit) | 0 | 2026-08-28 | 2026-09-02 | 一个强大的模型上下文协议（MCP）服务器，提供对学术文献数据库的无缝访问，帮助研究人员使用LLM和MCP客户端（如Claude、Cursor等）加速文献综述过程。 |
| 1788 | [xby-skill/xby-logo-analyze](https://github.com/xby-skill/xby-logo-analyze) | 0 | 2026-08-28 | 2026-09-02 | 一个智能Logo提取和处理的MCP服务器，支持从网站URL自动识别并提取Logo图标，并提供图像处理和矢量转换功能。 |
| 1789 | [xby-skill/xby-markdown-to-notion](https://github.com/xby-skill/xby-markdown-to-notion) | 0 | 2026-08-28 | 2026-09-02 | 一个将Markdown内容转换为Notion API兼容格式的MCP服务器，适用于内容管理和开发集成。 |
| 1790 | [xby-skill/xby-math](https://github.com/xby-skill/xby-math) | 0 | 2026-08-28 | 2026-09-02 | 一个高性能的数学计算协议服务器，提供从基础算术到高级微积分和线性代数的全面数学计算功能。 |
| 1791 | [xby-skill/xby-math-genie-calc](https://github.com/xby-skill/xby-math-genie-calc) | 0 | 2026-08-28 | 2026-09-02 | math_genie_calc是一款专注于科学计算的Python应用，提供从基础运算到复杂三角函数的多种计算功能，适合学生、科研人员等使用。 |
| 1792 | [xby-skill/xby-mathematical-visualization](https://github.com/xby-skill/xby-mathematical-visualization) | 0 | 2026-08-28 | 2026-09-02 | 基于JSXGraph的MCP协议服务器，提供13种数学可视化工具，适用于教育数学、工程和科学应用。 |
| 1793 | [xby-skill/xby-mathematics](https://github.com/xby-skill/xby-mathematics) | 0 | 2026-08-28 | 2026-09-02 | MCP Mathematics 是一个全面的数学计算服务器，可将任何AI助手转变为强大的数学计算引擎，提供高级数学函数、单位转换和财务计算等功能。 |
| 1794 | [xby-skill/xby-mbit-test](https://github.com/xby-skill/xby-mbit-test) | 0 | 2026-08-28 | 2026-09-02 | 一个用于MBTI人格测试的MCP服务器，支持AI助手引导用户完成人格测试并给出结果分析。 |
| 1795 | [xby-skill/xby-medical-knowledge-graph](https://github.com/xby-skill/xby-medical-knowledge-graph) | 0 | 2026-08-28 | 2026-09-02 | 围绕疾病，药品，症状，诊断，并发症，饮食及其关系的知识图谱。仅限初步研究，具体应用需根据实际情况调整。 |
| 1796 | [xby-skill/xby-mermaid-doc](https://github.com/xby-skill/xby-mermaid-doc) | 0 | 2026-08-28 | 2026-09-02 | Mermaid Doc MCP Server是一个用于生成Mermaid文档的服务器，提供列出可用图表和检索特定图表文档的功能。 |
| 1797 | [xby-skill/xby-mingli](https://github.com/xby-skill/xby-mingli) | 0 | 2026-08-28 | 2026-09-02 | 一个支持多种命理系统（紫微斗数、八字等）的MCP协议服务器，为AI工具提供命理分析与运势查询功能。 |
| 1798 | [xby-skill/xby-mm1-simulation](https://github.com/xby-skill/xby-mm1-simulation) | 0 | 2026-08-28 | 2026-09-02 | 一个用于M/M/1和M/M/c队列系统模拟和分析的Model Context Protocol服务器，提供全面的资源、工具和提示。 |
| 1799 | [xby-skill/xby-mvn](https://github.com/xby-skill/xby-mvn) | 0 | 2026-08-28 | 2026-09-02 | Maven MCP Server是一个通过自然语言交互的AI驱动Maven依赖管理工具，提供版本检查、安全扫描和依赖分析功能。 |
| 1800 | [xby-skill/xby-nba-stats](https://github.com/xby-skill/xby-nba-stats) | 0 | 2026-08-28 | 2026-09-02 | 一个提供实时和历史NBA数据的模型上下文协议服务器，包括球员统计、比赛得分、球队信息和高级分析。 |
| 1801 | [xby-skill/xby-ocr](https://github.com/xby-skill/xby-ocr) | 0 | 2026-08-28 | 2026-09-02 | 兼顾速度与精度的文字识别。输入包含文本的图像，自动检测并识别内容。适用于各类文档、广告牌、屏幕截图等场景。 |
| 1802 | [xby-skill/xby-ocr-bank-card](https://github.com/xby-skill/xby-ocr-bank-card) | 0 | 2026-08-28 | 2026-09-02 | 识别银行卡号、发卡银行和卡类型，使用 Luhn 算法校验卡号有效性。 |
| 1803 | [xby-skill/xby-ocr-biz-license](https://github.com/xby-skill/xby-ocr-biz-license) | 0 | 2026-08-28 | 2026-09-02 | 识别营业执照的统一社会信用代码、名称、法定代表人、注册资本、成立日期、经营范围、登记机关和住所地址。 |
| 1804 | [xby-skill/xby-ocr-captcha](https://github.com/xby-skill/xby-ocr-captcha) | 0 | 2026-08-28 | 2026-09-02 | 输入常见验证码图片，返回验证码文本内容。 |
| 1805 | [xby-skill/xby-ocr-handwriting](https://github.com/xby-skill/xby-ocr-handwriting) | 0 | 2026-08-28 | 2026-09-02 | 输入包含手写文本的图像，自动检测文本行并识别内容。适用于手写笔记、签名、手写表单等。 |
| 1806 | [xby-skill/xby-ocr-id-card](https://github.com/xby-skill/xby-ocr-id-card) | 0 | 2026-08-28 | 2026-09-02 | 识别身份证正面（姓名、性别、民族、出生日期、住址、身份证号）和背面（签发机关、有效期限），自动判断正反面并校验身份证号有效性。 |
| 1807 | [xby-skill/xby-ocr-pass](https://github.com/xby-skill/xby-ocr-pass) | 0 | 2026-08-28 | 2026-09-02 | 识别港澳通行证、台湾通行证的通行证号码、姓名、性别、出生日期、有效期、签发地点等信息，支持MRZ机读码解析。 |
| 1808 | [xby-skill/xby-ocr-passport](https://github.com/xby-skill/xby-ocr-passport) | 0 | 2026-08-28 | 2026-09-02 | 识别护照号码、中文姓名、英文姓名、性别、国籍、出生日期、签发日期、有效期至、签发地点等信息，支持MRZ机读码解析。 |
| 1809 | [xby-skill/xby-ocr-pro](https://github.com/xby-skill/xby-ocr-pro) | 0 | 2026-08-28 | 2026-09-02 | 高精度文字识别。输入包含文本的图像，自动检测并识别内容。适用于各类文档、广告牌、屏幕截图等场景。 |
| 1810 | [xby-skill/xby-ocr-vehicle-license](https://github.com/xby-skill/xby-ocr-vehicle-license) | 0 | 2026-08-28 | 2026-09-02 | 识别机动车行驶证的号牌号码、车辆类型、所有人、住址、品牌型号、发动机号码、车辆识别代号等信息，支持自动方向检测和主副页过滤。 |
| 1811 | [xby-skill/xby-oecd-search](https://github.com/xby-skill/xby-oecd-search) | 0 | 2026-08-28 | 2026-09-02 | 一个通过SDMX API提供OECD全面统计数据的模型上下文协议（MCP）服务器，支持AI助手和聊天机器人查询经济、健康、教育、环境等OECD数据集。 |
| 1812 | [xby-skill/xby-ons-data](https://github.com/xby-skill/xby-ons-data) | 0 | 2026-08-28 | 2026-09-02 | 一个用于访问英国国家统计局(ONS) Beta API的模型上下文协议(MCP)服务器，无需API密钥即可获取官方统计数据。 |
| 1813 | [xby-skill/xby-open-data-hk](https://github.com/xby-skill/xby-open-data-hk) | 0 | 2026-08-28 | 2026-09-02 | 一个提供香港政府官方开放数据门户DATA.GOV.HK数据访问的MCP服务器，支持数据集列表、详情查询、分类检索及格式筛选等功能。 |
| 1814 | [xby-skill/xby-osrs-stat](https://github.com/xby-skill/xby-osrs-stat) | 0 | 2026-08-28 | 2026-09-02 | 一个提供实时《Old School RuneScape》玩家统计数据和排行榜数据的Model Context Protocol (MCP)服务器，支持多种游戏模式和玩家比较功能。 |
| 1815 | [xby-skill/xby-pedestrian](https://github.com/xby-skill/xby-pedestrian) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，检测图像中的行人，输出所有目标的检测框、置信度和标签。 |
| 1816 | [xby-skill/xby-pet-detect](https://github.com/xby-skill/xby-pet-detect) | 0 | 2026-08-28 | 2026-09-02 | 识别宠物 (猫/狗) 面部表情，输出 4 类情绪: Angry / Happy / Relaxed / Sad。 |
| 1817 | [xby-skill/xby-philippine-geocoding](https://github.com/xby-skill/xby-philippine-geocoding) | 0 | 2026-08-28 | 2026-09-02 | 提供菲律宾标准地理编码（PSGC）API访问的模型上下文协议（MCP）服务器，包含完整的菲律宾地理层级数据。 |
| 1818 | [xby-skill/xby-pic](https://github.com/xby-skill/xby-pic) | 0 | 2026-08-28 | 2026-09-02 | 包括通用文本识别、手写识别、车牌识别、身份证识别、日常物体检测、昆虫识别、植物识别、护照识别、港澳台通行证识别、银行卡识别、营业执照识别、驾驶证识别、行驶证识别、动物识别、电动自行车检测、手机检测、手势检测、火焰检测、香烟检测、人头人体检测、野生动物检测、鸟类识别、宠物情绪识别、菜品识别、安全帽人体检测、行人检测、反光衣检测、车辆检测、图像分类、目标检测、旋转目标检测、人体姿态估计和万物识别。 |
| 1819 | [xby-skill/xby-plant-recognition](https://github.com/xby-skill/xby-plant-recognition) | 0 | 2026-08-28 | 2026-09-02 | 识别植物名称（或所属科, 属, 种或亚种）。 |
| 1820 | [xby-skill/xby-plate-recognition](https://github.com/xby-skill/xby-plate-recognition) | 0 | 2026-08-28 | 2026-09-02 | 识别车牌号、车牌颜色、单/双层车牌、位置框。 |
| 1821 | [xby-skill/xby-pose](https://github.com/xby-skill/xby-pose) | 0 | 2026-08-28 | 2026-09-02 | 检测图像中的人物，输出边界框和关键点坐标。每人有 17 个关键点，每个点代表人体不同的部位，依次为鼻子、左眼、右眼、左耳、右耳、左肩、右肩、左肘、右肘、左腕、右腕、左髋、右髋、左膝、右膝、左脚踝、右脚踝。 |
| 1822 | [xby-skill/xby-pubchem](https://github.com/xby-skill/xby-pubchem) | 0 | 2026-08-28 | 2026-09-02 | 该服务通过PubChem API提取药物基础化学信息，包括分子式、分子量、CAS号等关键数据。 |
| 1823 | [xby-skill/xby-qanon](https://github.com/xby-skill/xby-qanon) | 0 | 2026-08-28 | 2026-09-02 | 一个提供QAnon帖子数据集访问的MCP服务器，用于人类学和社会学研究，支持搜索、过滤和分析功能。 |
| 1824 | [xby-skill/xby-quick-chart](https://github.com/xby-skill/xby-quick-chart) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的服务器，提供与Quick Chart交互的标准化接口，支持图表生成和管理。 |
| 1825 | [xby-skill/xby-random-generator](https://github.com/xby-skill/xby-random-generator) | 0 | 2026-08-28 | 2026-09-02 | 一款符合MCP协议的加密安全随机数生成服务器，适用于AI应用、LLM及其他需要高质量随机数的系统。 |
| 1826 | [xby-skill/xby-random-number](https://github.com/xby-skill/xby-random-number) | 0 | 2026-08-28 | 2026-09-02 | 提供伪随机和加密安全的随机数生成功能，包括整数、浮点数、加权选择、列表洗牌和安全令牌生成。 |
| 1827 | [xby-skill/xby-react-composer-kit](https://github.com/xby-skill/xby-react-composer-kit) | 0 | 2026-08-28 | 2026-09-02 | 一个为Composer Kit React组件库提供文档、示例和使用信息的MCP服务器，专为在Celo区块链上构建web3应用而设计。 |
| 1828 | [xby-skill/xby-read-pdf](https://github.com/xby-skill/xby-read-pdf) | 0 | 2026-08-28 | 2026-09-02 | 一个支持AI助手读取和分析PDF文件的MCP服务器，提供PDF元数据提取、页面范围阅读和关键词搜索等功能。 |
| 1829 | [xby-skill/xby-read-website](https://github.com/xby-skill/xby-read-website) | 0 | 2026-08-28 | 2026-09-02 | 一个快速、高效的网页内容提取工具，将网页转换为干净的Markdown格式，适用于AI代理、IDE和LLM管道。 |
| 1830 | [xby-skill/xby-real-time-news](https://github.com/xby-skill/xby-real-time-news) | 0 | 2026-08-28 | 2026-09-02 | 实时新闻 |
| 1831 | [xby-skill/xby-recipe-query](https://github.com/xby-skill/xby-recipe-query) | 0 | 2026-08-28 | 2026-09-02 | 一个支持通过命令行查询菜谱和报菜名的菜谱查询工具，适用于烹饪爱好者和开发者。 |
| 1832 | [xby-skill/xby-recog](https://github.com/xby-skill/xby-recog) | 0 | 2026-08-28 | 2026-09-02 | 包括通用文本识别、手写识别、车牌识别、身份证识别、护照识别、港澳台通行证识别、银行卡识别、营业执照识别、驾驶证识别、行驶证识别。 |
| 1833 | [xby-skill/xby-reflective-vest](https://github.com/xby-skill/xby-reflective-vest) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，检测人员是否穿戴反光衣，输出图片中所有目标的检测框、置信度和标签（safe/unsafe）。 |
| 1834 | [xby-skill/xby-remember-memory](https://github.com/xby-skill/xby-remember-memory) | 0 | 2026-08-28 | 2026-09-02 | 一个基于分类的持久化记忆系统实现，允许Claude跨聊天会话存储和检索分类记忆信息。 |
| 1835 | [xby-skill/xby-review-code](https://github.com/xby-skill/xby-review-code) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的代码审查工具服务器，提供多维度的代码审查和打分功能。 |
| 1836 | [xby-skill/xby-rfc-doc](https://github.com/xby-skill/xby-rfc-doc) | 0 | 2026-08-28 | 2026-09-02 | 一个用于从ietf.org网站获取、解析和阅读RFC文档的MCP服务器，提供程序化交互工具。 |
| 1837 | [xby-skill/xby-running-formulas](https://github.com/xby-skill/xby-running-formulas) | 0 | 2026-08-28 | 2026-09-02 | 一个提供全面的跑步计算工具的MCP服务器，包括VDOT计算、训练配速、比赛时间预测、速度标记、心率区间和配速转换等功能。 |
| 1838 | [xby-skill/xby-scan-code](https://github.com/xby-skill/xby-scan-code) | 0 | 2026-08-28 | 2026-09-02 | CodeGuard MCP是一款实时AI代码安全扫描工具，用于检测AI生成代码中的漏洞、密钥和合规性问题，适用于开发环境中的代码安全审查。 |
| 1839 | [xby-skill/xby-search-apple-docs](https://github.com/xby-skill/xby-search-apple-docs) | 0 | 2026-08-28 | 2026-09-02 | 通过模型上下文协议（MCP）访问苹果官方开发者文档、框架、API及WWDC视频，支持AI驱动的自然语言查询，提供Swift/Objective-C代码示例和技术指南。 |
| 1840 | [xby-skill/xby-search-movie](https://github.com/xby-skill/xby-search-movie) | 0 | 2026-08-28 | 2026-09-02 | 一个基于 Model Context Protocol (MCP) 构建的智能电影和电视剧资源搜索工具，支持多源搜索和链接验证。 |
| 1841 | [xby-skill/xby-seg](https://github.com/xby-skill/xby-seg) | 0 | 2026-08-28 | 2026-09-02 | 实例分割比目标检测更进一步，不但要识别图像中的单个对象，还要将其从图像的其余部分中分割出来。对图像中的80类COCO目标进行实例分割，输出边界框、掩膜、置信度和类别标签。 |
| 1842 | [xby-skill/xby-sequentialthinking](https://github.com/xby-skill/xby-sequentialthinking) | 0 | 2026-08-28 | 2026-09-02 | 一个实现顺序思维协议的MCP服务器，提供结构化的问题解决方法，将复杂问题分解为可管理的步骤，并支持迭代优化和替代推理路径。 |
| 1843 | [xby-skill/xby-smart-search](https://github.com/xby-skill/xby-smart-search) | 0 | 2026-08-28 | 2026-09-02 | Smart Search MCP 是一个专注于技术领域的智能搜索工具集，提供14个增强型搜索工具，覆盖国际和国内主流技术平台，具备智能URL生成、输入验证、高级搜索技巧等功能，适用于开发者快速查找技术文档、API参考、开源项目等。 |
| 1844 | [xby-skill/xby-smoking-detection](https://github.com/xby-skill/xby-smoking-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的香烟目标进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1845 | [xby-skill/xby-source-coop](https://github.com/xby-skill/xby-source-coop) | 0 | 2026-08-28 | 2026-09-02 | 一个用于发现和访问800TB+地理空间数据的MCP服务器，支持AI客户端通过JSON-RPC协议进行交互，提供智能搜索和高效数据访问功能。 |
| 1846 | [xby-skill/xby-speech-synthesis](https://github.com/xby-skill/xby-speech-synthesis) | 0 | 2026-08-28 | 2026-09-02 | 一个集成了Microsoft Edge高质量语音合成能力的MCP服务器，支持多语言语音生成、音频合并和云端存储。 |
| 1847 | [xby-skill/xby-structured-argumentation](https://github.com/xby-skill/xby-structured-argumentation) | 0 | 2026-08-28 | 2026-09-02 | 一组模型上下文协议服务器，为大型语言模型提供认知增强工具。 |
| 1848 | [xby-skill/xby-subnet-calculator](https://github.com/xby-skill/xby-subnet-calculator) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol的服务，提供IPv4子网规划工具，包括子网大小计算、通配符掩码生成、网关选择和主机验证等功能。 |
| 1849 | [xby-skill/xby-text-toolkit](https://github.com/xby-skill/xby-text-toolkit) | 0 | 2026-08-28 | 2026-09-02 | 一个提供文本转换、格式化和分析功能的MCP服务器，可直接集成到开发工作流中。 |
| 1850 | [xby-skill/xby-text-transformer](https://github.com/xby-skill/xby-text-transformer) | 0 | 2026-08-28 | 2026-09-02 | 提供多种文本转换功能的MCP服务器，包括大小写转换、反转字符串、检测回文等功能。 |
| 1851 | [xby-skill/xby-the-met](https://github.com/xby-skill/xby-the-met) | 0 | 2026-08-28 | 2026-09-02 | 查询搜索和获取博物馆的开放藏品数据 |
| 1852 | [xby-skill/xby-time](https://github.com/xby-skill/xby-time) | 0 | 2026-08-28 | 2026-09-02 | 提供时间和时区转换功能的模型上下文协议服务器，支持获取当前时间和时区转换。 |
| 1853 | [xby-skill/xby-time-zone](https://github.com/xby-skill/xby-time-zone) | 0 | 2026-08-28 | 2026-09-02 | 一个全面的MCP服务器，提供全球时区管理和时间转换功能，适用于全球业务协调、旅行规划和开发运维。 |
| 1854 | [xby-skill/xby-todolist](https://github.com/xby-skill/xby-todolist) | 0 | 2026-08-28 | 2026-09-02 | 为大型语言模型和AI代理提供外部工作记忆和任务管理功能，支持复杂多步骤任务的可靠执行。 |
| 1855 | [xby-skill/xby-toronto-open-data-server](https://github.com/xby-skill/xby-toronto-open-data-server) | 0 | 2026-08-28 | 2026-09-02 | 一个通过CKAN API直接访问多伦多开放数据的MCP服务器，支持智能数据集发现、灵活查询和CSV数据预览，专为LLM代理设计。 |
| 1856 | [xby-skill/xby-traditional-chinese-medicine-formulas-kg](https://github.com/xby-skill/xby-traditional-chinese-medicine-formulas-kg) | 0 | 2026-08-28 | 2026-09-02 | 围绕中药方剂、方名、来源、别名、处方、中药名、剂量、功能主治及其之间的联系构建知识谱图。仅限初步研究，具体应用需根据实际情况调整。 |
| 1857 | [xby-skill/xby-traditional-chinese-medicine-kg](https://github.com/xby-skill/xby-traditional-chinese-medicine-kg) | 0 | 2026-08-28 | 2026-09-02 | 围绕中药名，中药材，别名，来源，分布，功能，主治，归经，四气，四气及其之间的联系构建知识谱图。仅限初步研究，具体应用需根据实际情况调整。 |
| 1858 | [xby-skill/xby-uk-police-data-query](https://github.com/xby-skill/xby-uk-police-data-query) | 0 | 2026-08-28 | 2026-09-02 | 一个提供英国警察数据查询的MCP服务器，包括犯罪记录、警察部队、社区信息和拦截搜查数据。 |
| 1859 | [xby-skill/xby-vnstock](https://github.com/xby-skill/xby-vnstock) | 0 | 2026-08-28 | 2026-09-02 | 一个非官方的MCP服务器，提供访问越南股市数据的工具，包括实时和历史股票价格、公司财务数据、市场统计和基金信息等。 |
| 1860 | [xby-skill/xby-web-research-assistant](https://github.com/xby-skill/xby-web-research-assistant) | 0 | 2026-08-28 | 2026-09-02 | 一个提供网络研究和发现功能的综合模型上下文协议（MCP）服务器，包含13种工具用于搜索、爬取和分析网络内容。 |
| 1861 | [xby-skill/xby-who-is](https://github.com/xby-skill/xby-who-is) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的WHOIS域名查询服务器，支持877+顶级域名和169个国家代码顶级域名的解析，提供全面的域名注册信息查询功能。 |
| 1862 | [xby-skill/xby-wikimedia-search-images](https://github.com/xby-skill/xby-wikimedia-search-images) | 0 | 2026-08-28 | 2026-09-02 | 该MCP服务器使AI助手能够在Wikimedia Commons上搜索图片，提供详细的元数据和可选的缩略图组合，帮助AI模型进行视觉比较。 |
| 1863 | [xby-skill/xby-wild-animal-detection](https://github.com/xby-skill/xby-wild-animal-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，输出图像中所有识别到的野生动物的检测框、置信度及标签。 |
| 1864 | [xchannel1987/dsh-mobile-xc](https://github.com/xchannel1987/dsh-mobile-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH Web mobile UI adaptation plugin with overlay drawer, safe-area support, and canary version detection |
| 1865 | [xchannel1987/dsh-power-xc](https://github.com/xchannel1987/dsh-power-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH power control plugin with restart/shutdown menu and Windows-style overlay animation |
| 1866 | [xchannel1987/dsh-reverse-proxy-xc](https://github.com/xchannel1987/dsh-reverse-proxy-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH LAN reverse proxy plugin for accessing Web GUI from mobile devices |
| 1867 | [xchannel1987/dsh-session-xc](https://github.com/xchannel1987/dsh-session-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH session enhancement plugin with session count display, archive management, and cross-workspace move |
| 1868 | [xchannel1987/dsh-token-usage-xc](https://github.com/xchannel1987/dsh-token-usage-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH token usage statistics plugin with daily/7-day trends and cache hit rate |
| 1869 | [xdongHo/dsh-wechat-mobile-skin](https://github.com/xdongHo/dsh-wechat-mobile-skin) | 0 | 2026-08-31 | 2026-08-31 | WeChat-style mobile skin for the DeepSeek Harness Web GUI: mobile browsers get a WeChat chat list and chat page, desktop stays untouched. |
| 1870 | [xgone/dsh-netshell](https://github.com/xgone/dsh-netshell) | 0 | 2026-09-02 | 2026-09-04 | DSH 远程终端插件:在 Web UI 直连 SSH,危险命令三级护栏,AI 命令须真人确认,密码加密存储、不进 AI 会话 \| Remote SSH terminal plugin for DeepSeek Harness: 3-level command guard, human-approved AI commands, encrypted credentials |
| 1871 | [xia-sc/dsh-git](https://github.com/xia-sc/dsh-git) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness Web GUI 的完整 Git 管理插件：分支切换/fetch/pull/commit/push，可折叠悬浮面板 + 输入框胶囊 |
| 1872 | [xia-sc/dsh-opencode-go](https://github.com/xia-sc/dsh-opencode-go) | 0 | 2026-09-04 | 2026-09-04 | DeepSeek Harness LLM provider plugin for OpenCode Go (zen-go route) |
| 1873 | [XianmingLF/xmlf-plugin-manager](https://github.com/XianmingLF/xmlf-plugin-manager) | 0 | 2026-08-21 | 2026-08-28 | 管理当前第三方已安装插件的信息 比较简单的版本 可按照自己的需求修改 |
| 1874 | [xiaokaizhou/dsh-llm-multimodal](https://github.com/xiaokaizhou/dsh-llm-multimodal) | 0 | 2026-08-31 | 2026-09-01 | DSH 插件：在聊天中提供图像/视频生成工具，基于 OpenAI 兼容 API |
| 1875 | [xiaokaizhou/dsh-media-preview](https://github.com/xiaokaizhou/dsh-media-preview) | 0 | 2026-08-30 | 2026-08-31 | DSH 插件：在聊天记录中自动将本地音视频路径渲染为可播放的预览组件 |
| 1876 | [XiaoWind/dsh-btw](https://github.com/XiaoWind/dsh-btw) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: a /btw slash command to add notes without interrupting the agent |
| 1877 | [XiaoWind/dsh-vault](https://github.com/XiaoWind/dsh-vault) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: portable workspace vault for DSH conversations and logs |
| 1878 | [xiaoxiao44443/dfy-dsh-plugins](https://github.com/xiaoxiao44443/dfy-dsh-plugins) | 0 | 2026-08-17 | 2026-08-28 | Personal plugins for DeepSeek Harness |
| 1879 | [xiaoxiaohai/dsh-remote](https://github.com/xiaoxiaohai/dsh-remote) | 0 | 2026-08-27 | 2026-09-02 | Secure, opt-in phone access for DeepSeek Harness Web on macOS. |
| 1880 | [xiaoxingyuemiao/dsh-bg-plugin](https://github.com/xiaoxingyuemiao/dsh-bg-plugin) | 0 | 2026-08-27 | 2026-08-27 | DSH 自定义背景插件：为 DSH Web GUI 应用远程/本地图片背景，支持清晰度、压暗、模糊调节，设置面板保持默认外观。 |
| 1881 | [XiaoYuOvO/dsh-external-session](https://github.com/XiaoYuOvO/dsh-external-session) | 0 | 2026-09-04 | 2026-09-04 | Portable Git-backed external session persistence plugin for DeepSeek Harness |
| 1882 | [xiaxi626/dsh-math-input](https://github.com/xiaxi626/dsh-math-input) | 0 | 2026-08-31 | 2026-09-01 | dsh-math-input 是一个 DeepSeek Harness 插件，提供零 token 消耗的离线数学输入能力。核心功能包括：手写笔迹识别（基于 ONNX 模型 + 束搜索）、LaTeX 自动修复与渲染（KaTeX）、以及手写画板 UI。所有推理在浏览器端完成，不依赖远程 API。 |
| 1883 | [xingtu1996/dsh-xingtu-skills](https://github.com/xingtu1996/dsh-xingtu-skills) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness (DSH) plugin: 26 production AI-agent skills (Caveman token compression, Ponytail minimalism, engineering practice) as a standard dsh-plugin bundle. 行途技能 DSH 插件包 |
| 1884 | [xiyi123465/dsh-usage-calendar](https://github.com/xiyi123465/dsh-usage-calendar) | 0 | 2026-08-25 | 2026-08-27 | DeepSeekAPI余额查询插件 |
| 1885 | [xlin20021/dsh-mcp-hub](https://github.com/xlin20021/dsh-mcp-hub) | 0 | 2026-08-29 | 2026-08-29 | dsh-mcp-hub |
| 1886 | [xlin20021/dsh-stock-chart](https://github.com/xlin20021/dsh-stock-chart) | 0 | 2026-08-29 | 2026-08-29 | dsh-stock-chart |
| 1887 | [xobexo/dsh-smart-scenario-router](https://github.com/xobexo/dsh-smart-scenario-router) | 0 | 2026-08-27 | 2026-08-27 | 国产模型优先，按任务类型自动切换模型，支持可视化配置面板 |
| 1888 | [xswt442-cmd/dsh-ballast](https://github.com/xswt442-cmd/dsh-ballast) | 0 | 2026-08-31 | 2026-09-02 | DSH 上下文窗口逐条归因面板——看谁占了窗口 \| Per-message context window attribution for DSH — see what takes up the window |
| 1889 | [xswt442-cmd/dsh-mini-utility-dock](https://github.com/xswt442-cmd/dsh-mini-utility-dock) | 0 | 2026-09-02 | 2026-09-02 | 一个简单的 DSH 工具坞 \| A simple utility dock for DSH |
| 1890 | [xswt442-cmd/dsh-treekeeper](https://github.com/xswt442-cmd/dsh-treekeeper) | 0 | 2026-08-27 | 2026-08-27 | 对账 DSH 任务账本与 OS 进程树，定位归属、检测泄漏并安全治理｜Reconcile DSH task ledgers with OS process trees for attribution, leak detection, and safe governance. |
| 1891 | [xuxucodepractice-code/dsh-claim-guard](https://github.com/xuxucodepractice-code/dsh-claim-guard) | 0 | 2026-09-03 | 2026-09-03 | A deterministic pre-write claim guard for supported DeepSeek Harness file tools. |
| 1892 | [XY1998-debug/dsh-zhinet](https://github.com/XY1998-debug/dsh-zhinet) | 0 | 2026-09-01 | 2026-09-01 | 许愿式编程的项目事实图、只读工作台、角色协作与跨 DSH 迁移 |
| 1893 | [xyingsoft/dsh-chat](https://github.com/xyingsoft/dsh-chat) | 0 | 2026-08-29 | 2026-08-29 | dsh-chat 设计文档：面向自建团队、受管团队与企业组织的 DSH Web 协作平台 |
| 1894 | [Xylocarpro/dsh-plugin-recycle-bin](https://github.com/Xylocarpro/dsh-plugin-recycle-bin) | 0 | 2026-08-29 | 2026-08-30 | 强制 DSH 删除走回收站、禁用 del/rm/Remove-Item，回收站或硬盘满时停手询问用户。 |
| 1895 | [Ya-MiC/zhanzhen](https://github.com/Ya-MiC/zhanzhen) | 0 | 2026-08-24 | 2026-08-27 | 湛箴 — 中小企业审计风险平台 v1 框架（FastAPI + Vue3，规则引擎本地运行，证据哈希链） |
| 1896 | [yahoolcj/dsh-plugin-zerone](https://github.com/yahoolcj/dsh-plugin-zerone) | 0 | 2026-09-01 | 2026-09-01 | dsh-plugin-zerone |
| 1897 | [yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix](https://github.com/yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix) | 0 | 2026-08-27 | 2026-08-27 | 修复 sandbox_permissions 和 justification 字段在 pwsh/bash/fs/dsh-sandbox 中的 no-op 升级报错。当会话已是 danger-full-access 模式时，模型携带空 justification 或重申同一模式被拒的问题。 |
| 1898 | [yakoylp/dsh-localnotify](https://github.com/yakoylp/dsh-localnotify) | 0 | 2026-09-01 | 2026-09-02 | DSH 本地通知栏插件：侧边栏【通知】入口 + 全屏通知中心（时间筛选/搜索/未读已读/删除/详情一键复制），notify_add agent 工具 + CLI 写入，JSON 持久化，实时刷新，界面跟随 dsh web 语言切换。Local notification center for DeepSeek Harness: notify_add agent tool & CLI, live refresh, i18n. |
| 1899 | [yangbobo2021/relay-dsh-plugin-monitor-author](https://github.com/yangbobo2021/relay-dsh-plugin-monitor-author) | 0 | 2026-09-02 | 2026-09-03 | DSH Skill for discovering and safely authoring Relay Monitor Bundles. |
| 1900 | [yangbobo2021/relay-dsh-plugin-monitor-process](https://github.com/yangbobo2021/relay-dsh-plugin-monitor-process) | 0 | 2026-09-02 | 2026-09-03 | Identity-safe process monitoring capability for Relay on DeepSeek Harness. |
| 1901 | [yangbobo2021/relay-dsh-plugin-monitor-time](https://github.com/yangbobo2021/relay-dsh-plugin-monitor-time) | 0 | 2026-09-02 | 2026-09-03 | Time deadline Monitor Bundle extension for Relay on DeepSeek Harness. |
| 1902 | [yangbobo2021/relay-dsh-plugin-skill-creator](https://github.com/yangbobo2021/relay-dsh-plugin-skill-creator) | 0 | 2026-09-04 | 2026-09-04 | DSH plugin that turns completed conversations into reusable, validated Skill bundles |
| 1903 | [yangdongzhen590/dsh-knj-extension-center](https://github.com/yangdongzhen590/dsh-knj-extension-center) | 0 | 2026-08-31 | 2026-08-31 | DSH ????:????????? zip ?????/??/?????????DSH skill center: browse by region, install from zip, manage enable/disable, uninstall, trash restore, search. |
| 1904 | [yangdongzhen590/dsh-knj-obsidian](https://github.com/yangdongzhen590/dsh-knj-obsidian) | 0 | 2026-08-28 | 2026-08-28 | DSH ??? Obsidian:AI agent ?????????????UI ?????(v1-v7) |
| 1905 | [yangdongzhen590/dsh-knj-prompts](https://github.com/yangdongzhen590/dsh-knj-prompts) | 0 | 2026-08-31 | 2026-08-31 | DSH ???????:????? ? ????????????(?? {??}),???????Prompt-scenario picker for DeepSeek Harness. |
| 1906 | [yangdongzhen590/dsh-knj-session-management](https://github.com/yangdongzhen590/dsh-knj-session-management) | 0 | 2026-08-31 | 2026-08-31 | Session management for DeepSeek Harness: archive/restore/delete persisted sessions, per-workspace retention policy and a size governance panel. DSH ??????:??/??/???????,????????????,????????? |
| 1907 | [yangzhe1991/dsh-futu-mcp](https://github.com/yangzhe1991/dsh-futu-mcp) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin: connect to Futu (富途) MCP via OAuth 2.1 with deferred authorization; tokens stored securely outside the workspace (~/.dsh, 0600) |
| 1908 | [yanqd0/dsh-covtrim](https://github.com/yanqd0/dsh-covtrim) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: one-shot test coverage flow — run tests with coverage, compress with covtrim, return compact TSV to the agent |
| 1909 | [yanqd0/dsh-mint](https://github.com/yanqd0/dsh-mint) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: mint issue tracking integration — session context injection, event reminders, plan binding, mint_query tool, and a session tab |
| 1910 | [yaodongH/dsh-vscode-bridge](https://github.com/yaodongH/dsh-vscode-bridge) | 0 | 2026-08-30 | 2026-08-30 | DSH web 插件：在 DeepSeek Harness 中心区嵌入固定版本 code-server（VS Code Web），跟随当前工作空间，支持自定义端口/路径与热切换。 |
| 1911 | [yaotongsb/dsh-phosphor](https://github.com/yaotongsb/dsh-phosphor) | 0 | 2026-08-29 | 2026-08-29 | A full-screen, Matrix-styled TUI frontend for DeepSeek Harness — built with React + Ink as a Cordis bundle plugin |
| 1912 | [yhPrime/dsh-github-installer](https://github.com/yhPrime/dsh-github-installer) | 0 | 2026-08-29 | 2026-08-29 | GitHub 仓库一键安装插件：粘贴任意 GitHub 插件仓库网址即可安装（标准 dsh plugin add github:… 协议，同 dsh-market）。Install any DeepSeek Harness plugin from a GitHub repo URL. |
| 1913 | [Yidien/dsh-host-router](https://github.com/Yidien/dsh-host-router) | 0 | 2026-08-29 | 2026-08-29 | dsh 外挂式网络路由插件:按域名勾选走本地代理(Clash 等),其余直连;内置嗅探,设置页勾选即生效。 |
| 1914 | [yin52133/dsh-luban](https://github.com/yin52133/dsh-luban) | 0 | 2026-08-29 | 2026-09-01 | 🛠️ Custom workbench plugin suite for DeepSeek Harness (DSH) — LAN auth, task board, SSH + tmux keep-alive, shared Windows/Ubuntu sessions, context HUD & serial/debug tooling. Built for embedded devs: Windows debug box + LAN Ubuntu build server. Monorepo of dsh-luban-* plugins. |
| 1915 | [Yinxe/dsh-custom-ui](https://github.com/Yinxe/dsh-custom-ui) | 0 | 2026-09-04 | 2026-09-04 | DSH 主题画廊：8 套 open-design 主题（OpenCode/Linear/Notion/Claude/NVIDIA/GitHub）全量 token 映射 + 设置页一键切换 + 偏好持久化与守护 |
| 1916 | [Yinxe/dsh-mcwiki-search](https://github.com/Yinxe/dsh-mcwiki-search) | 0 | 2026-08-29 | 2026-09-02 | MCBE WIKI 搜索工具 |
| 1917 | [Yinxe/dsh-tavily-search](https://github.com/Yinxe/dsh-tavily-search) | 0 | 2026-09-01 | 2026-09-02 | Tavily AI search provider for DeepSeek Harness |
| 1918 | [Yinxe/dsh-token-stats](https://github.com/Yinxe/dsh-token-stats) | 0 | 2026-09-02 | 2026-09-03 | DeepSeek Harness (DSH) token usage statistics plugin: aggregates all local session logs into cumulative/peak/streak stats, daily & weekly trends, hour-of-day distribution, GitHub-style year heatmap, per-model breakdown — Settings page + sidebar today card. |
| 1919 | [Yiyang0659/dsh-git-sync](https://github.com/Yiyang0659/dsh-git-sync) | 0 | 2026-09-02 | 2026-09-02 | Git Config Sync Center for DeepSeek Harness — real-time config sync to GitHub with conflict self-healing and multi AI-tool adapters (OpenCode/Cline/Roo Code/Kilo Code/Continue/goose/Agent Zero) |
| 1920 | [ynymhrb/long-horizon-runtime](https://github.com/ynymhrb/long-horizon-runtime) | 0 | 2026-08-26 | 2026-09-03 | Durable long-horizon task runtime for DeepSeek Harness — plan, confirm, track, and resume AI work across sessions and interruptions. |
| 1921 | [yonglun/deepseek-harness-themes](https://github.com/yonglun/deepseek-harness-themes) | 0 | 2026-08-27 | 2026-08-28 | 74 non-invasive DeepSeek Harness themes generated from awesome-design-md |
| 1922 | [yongshuai0314/dsh-turnsnap](https://github.com/yongshuai0314/dsh-turnsnap) | 0 | 2026-08-27 | 2026-08-27 | Zero-config per-turn git checkpoints for DeepSeek Harness: every completed agent turn in a git workspace becomes one tagged [turnsnap] commit |
| 1923 | [yoshino-xiao7/dsh-codex](https://github.com/yoshino-xiao7/dsh-codex) | 0 | 2026-08-28 | 2026-08-29 | 社区维护的 DeepSeek Harness Codex 插件：OAuth、模型、图片与流式恢复；非官方 / Community Codex plugin for DSH: OAuth, models, images, stream recovery; unofficial. |
| 1924 | [youridol/dsh-launcher](https://github.com/youridol/dsh-launcher) | 0 | 2026-09-01 | 2026-09-02 | deepseek-harness 启动器与运行环境管理器（Tauri 2 + Rust + React） |
| 1925 | [YrracOwl/dsh-hmos-sidebar](https://github.com/YrracOwl/dsh-hmos-sidebar) | 0 | 2026-09-03 | 2026-09-03 | EN: Windows-only HarmonyOS workbench with 41 DSH tools and native agent presets. 中文：面向 DeepSeek Harness 的 Windows 原生鸿蒙开发工作台，包含 41 个 DSH 工具与原生鸿蒙预设。 |
| 1926 | [YrracOwl/dsh-mcp-pill](https://github.com/YrracOwl/dsh-mcp-pill) | 0 | 2026-09-04 | 2026-09-04 | EN: Lifecycle-safe MCP status pill for DSH Web. 中文：面向 DSH Web 的生命周期安全 MCP 状态胶囊。 |
| 1927 | [YrracOwl/dsh-subagent-conductor](https://github.com/YrracOwl/dsh-subagent-conductor) | 0 | 2026-09-04 | 2026-09-04 | EN: Lifecycle-safe subagent routing and role controls for DSH Web. 中文：面向 DSH Web 的生命周期安全子代理路由与角色控制。 |
| 1928 | [YrracOwl/dsh-theme-acid-noir](https://github.com/YrracOwl/dsh-theme-acid-noir) | 0 | 2026-09-04 | 2026-09-04 | EN: Usability-first cyber-editorial themes for DSH Web. 中文：面向 DSH Web、重视可用性的赛博编辑主题。 |
| 1929 | [YrracOwl/dsh-theme-cutout-clash](https://github.com/YrracOwl/dsh-theme-cutout-clash) | 0 | 2026-09-04 | 2026-09-04 | EN: Neo-brutalist and pop-art themes with calm reading surfaces for DSH Web. 中文：面向 DSH Web、兼顾安静阅读表面的新粗野主义与波普艺术主题。 |
| 1930 | [YrracOwl/dsh-tool-adapt](https://github.com/YrracOwl/dsh-tool-adapt) | 0 | 2026-09-04 | 2026-09-04 | EN: Safety and compatibility layer for non-DeepSeek models in DSH Web. 中文：面向 DSH Web 非 DeepSeek 模型的安全兼容适配层。 |
| 1931 | [ytmaps/dsh-subagent-flowtext](https://github.com/ytmaps/dsh-subagent-flowtext) | 0 | 2026-09-01 | 2026-09-01 | 鱼先生模块化OB |
| 1932 | [Yu-Zhuang1/dsh-workspace-snapshot-fork](https://github.com/Yu-Zhuang1/dsh-workspace-snapshot-fork) | 0 | 2026-08-31 | 2026-08-31 | Fork DeepSeek Harness sessions together with their historical workspace state. |
| 1933 | [yuandian-ailaw/yuandian_dsh_plugin](https://github.com/yuandian-ailaw/yuandian_dsh_plugin) | 0 | 2026-09-04 | 2026-09-04 | 华语元典法律数据（deepseek harness ）官方插件 |
| 1934 | [YUANMINGXUE/dsh-search](https://github.com/YUANMINGXUE/dsh-search) | 0 | 2026-08-26 | 2026-08-27 | Local-browser web search & page fetch plugin for DeepSeek Harness (dsh): browser_search / browser_fetch over Chrome DevTools Protocol, no API key. |
| 1935 | [YUEYUEXYS/dsh-think-ultra](https://github.com/YUEYUEXYS/dsh-think-ultra) | 0 | 2026-08-30 | 2026-08-30 | Reasoning layer for the official DeepSeek Harness: every request stays on native max effort, with isolated Flash/Vision/Pro depth controls, stability axes and reasoning toolboxes built above it. Delivered build only; commercial use open, reverse/modify/extract closed. |
| 1936 | [YuiKiZJ2026/dsh-slot-homestead](https://github.com/YuiKiZJ2026/dsh-slot-homestead) | 0 | 2026-09-02 | 2026-09-02 | 老虎机庄园｜A pixel-art desktop ecosystem for DSH with time-based fish, crop and animal growth, day/night ambience and collectible slot rewards. |
| 1937 | [yunmin311/dsh-universal-palette](https://github.com/yunmin311/dsh-universal-palette) | 0 | 2026-09-03 | 2026-09-03 | Dense translucent-glass Universal Palette for DeepSeek Harness Web — federates Commands, Sessions, Models, Conversation Hits with rich secondary actions and deterministic context/frecency ranking. |
| 1938 | [yunxiiQwQ/drool-whale-pet-for-dsh](https://github.com/yunxiiQwQ/drool-whale-pet-for-dsh) | 0 | 2026-08-27 | 2026-08-27 | 适用于dsh的pet插件 |
| 1939 | [yunxiyang/dsh-web-search-litellm](https://github.com/yunxiyang/dsh-web-search-litellm) | 0 | 2026-08-31 | 2026-08-31 | Web search provider for the DeepSeek Harness ctx.web seam via the LiteLLM proxy OpenAI Responses API (DeepSeek native server-side web_search) |
| 1940 | [Yurzi/dsh-web-fetch-enhanced](https://github.com/Yurzi/dsh-web-fetch-enhanced) | 0 | 2026-08-28 | 2026-08-28 | Configurable non-public address allowlists for DeepSeek Harness web_fetch |
| 1941 | [Yurzi/dsh-web-search-enhanced](https://github.com/Yurzi/dsh-web-search-enhanced) | 0 | 2026-08-29 | 2026-08-29 | Multi-protocol web_search provider for DeepSeek Harness |
| 1942 | [yushenghai1106/dsh-memory-plugin](https://github.com/yushenghai1106/dsh-memory-plugin) | 0 | 2026-09-02 | 2026-09-02 | Pluggable persistent memory bundle for DeepSeek Harness |
| 1943 | [yustillrain/dsh-plugin-tool-repository](https://github.com/yustillrain/dsh-plugin-tool-repository) | 0 | 2026-08-26 | 2026-08-27 | DSH 插件仓库 第三方插件 让你可视化管理已安装的 skill/插件 对skill/插件功能进行介绍和分类  |
| 1944 | [yx-yinhe/dsh-message-navigator](https://github.com/yx-yinhe/dsh-message-navigator) | 0 | 2026-08-27 | 2026-08-27 | ChatGPT-style message navigator for DeepSeek Harness conversations with hover previews and smooth jump navigation. |
| 1945 | [Yyyyyylor/dsh-asuka-school-theme](https://github.com/Yyyyyylor/dsh-asuka-school-theme) | 0 | 2026-08-25 | 2026-08-27 | Theme-Asuka — An unofficial Asuka-inspired theme plugin for DeepSeek Harness Web UI, featuring time-of-day wallpapers, adaptive palette transitions, and restrained EVA-02 visual details. |
| 1946 | [z7ping/narratica](https://github.com/z7ping/narratica) | 0 | 2026-08-28 | 2026-08-28 | AI 原生故事创作与媒体生产工作区｜AI-native storytelling workspace for novels, screenplays, and media production. |
| 1947 | [zachshi-ai/newmind](https://github.com/zachshi-ai/newmind) | 0 | 2026-09-04 | 2026-09-04 | 老思想 × 新智能 实验室：每门经典思想精确解决一个 AI 真实问题。#1 知止 zhizhi — DeepSeek Harness 的行为节制层（道德经 × Agent 可靠性） |
| 1948 | [zdjmrq/dsh-chat-mode](https://github.com/zdjmrq/dsh-chat-mode) | 0 | 2026-08-26 | 2026-08-27 | DSH 插件：为 DeepSeek Harness 增加「对话」纯聊天模式（ChatGPT 式）——侧边栏新会话模式切换（DSH/对话）、对话会话仅提问+搜索工具、专属 \/chat 聊天工作区 |
| 1949 | [Zessi-C/biofigure-self-evolve](https://github.com/Zessi-C/biofigure-self-evolve) | 0 | 2026-08-29 | 2026-08-30 | Self-evolving bioinformatics figure library skill: learn plots from papers/PDFs/WeChat articles/screenshots into reusable recipes (R/Python), imitate them when plotting. 自进化的生信 figure 学习库与复用引擎 |
| 1950 | [ZF3373/dsh-algo-trainer](https://github.com/ZF3373/dsh-algo-trainer) | 0 | 2026-09-04 | 2026-09-04 | ICPC competitive programming training plugin for DeepSeek Harness — sync, analysis, plans, reviews, templates |
| 1951 | [zgxaxdd/dsh-html-render](https://github.com/zgxaxdd/dsh-html-render) | 0 | 2026-09-04 | 2026-09-04 | Inline HTML + KaTeX renderer for DeepSeek Harness (DSH) chats - sandboxed iframes, theme-adaptive, height-accurate, zero network |
| 1952 | [zhang-jiazhi/dsh-prompt-optimizer](https://github.com/zhang-jiazhi/dsh-prompt-optimizer) | 0 | 2026-08-30 | 2026-08-30 | 将原作者 linshenkx 的 prompt-optimizer 移植到 DeepSeek Harness 的第三方插件（非官方） |
| 1953 | [zhangguiping-xydt/dsh-possibility-space](https://github.com/zhangguiping-xydt/dsh-possibility-space) | 0 | 2026-08-31 | 2026-08-31 | Explore AI outputs as a steerable semantic possibility space for DeepSeek Harness. |
| 1954 | [zhangguiping-xydt/dsh-session-lab](https://github.com/zhangguiping-xydt/dsh-session-lab) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness session teaching, evidence capsules, and controlled trajectory comparison |
| 1955 | [zhangguiping-xydt/dsh-skin-studio](https://github.com/zhangguiping-xydt/dsh-skin-studio) | 0 | 2026-09-01 | 2026-09-01 | A visual, local-first skin authoring studio for DeepSeek Harness Web. |
| 1956 | [zhangkkkai/dsh-getman-panel](https://github.com/zhangkkkai/dsh-getman-panel) | 0 | 2026-08-28 | 2026-08-31 | API 测试侧边栏面板（Getman），作为 dsh-better-sidebar 的配套插件：  请求编辑：方法（GET/POST/PUT/PATCH/DELETE/HEAD/OPTIONS）+ URL + Params / Headers / Body 响应查看：状态码徽章、耗时、大小、响应体（JSON 自动美化，右上角可一键复制）/ 响应头 历史记录：全局共享最近 100 条请求（所有工作空间共用），点击回填、单项删除、一键清空 绕过 CORS：通过 host 半代理转发，任意 HTTP(S) 接口都能测试 |
| 1957 | [zhangkkkai/dsh-spec-panel](https://github.com/zhangkkkai/dsh-spec-panel) | 0 | 2026-08-28 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 SDD（规范驱动开发，Spec-Driven Development）配套插件：在侧边栏提供一个 Spec 工作台，围绕 OpenSpec 的标准目录结构，让「先写规范 → 再实现 → 再验证」的流程一目了然、可操作。 |
| 1958 | [zhangkkkai/dsh-todo-panel](https://github.com/zhangkkkai/dsh-todo-panel) | 0 | 2026-08-27 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 TODO 任务清单侧边栏插件：卡片式布局、优先级颜色标记、中文界面、按会话持久化。 |
| 1959 | [zhangliang0115/ai-plugin](https://github.com/zhangliang0115/ai-plugin) | 0 | 2026-08-29 | 2026-08-29 | One command to install any AI agent skill/plugin into every agent — Claude Code, DeepSeek Harness (dsh), Codex, Gemini CLI, Copilot, Cursor. Zero-dependency CLI + cross-agent marketplace. |
| 1960 | [zhangmiao03/dsh-cloak](https://github.com/zhangmiao03/dsh-cloak) | 0 | 2026-09-04 | 2026-09-04 | Context firewall for DeepSeek Harness: credentials in tool results become opaque placeholders before they reach the model — the secret never enters context. |
| 1961 | [zhangxingong/dsh-polish](https://github.com/zhangxingong/dsh-polish) | 0 | 2026-09-01 | 2026-09-02 | 需要你做的 UI 验收（重启后逐项过一遍）  1. 书本图标右侧出现四角星按钮：细线空心、四角顶点小圆点、浅灰，与相邻按钮同尺寸，深色主题正常 2. 悬浮显示「优化并细化当前用户输入」 3. 权限下拉切 Read Only → 按钮置灰；切回恢复 4. 空输入点击 → Toast「请先输入内容再进行优化细化」 5. 有文本点击 → loading 旋转 → 全文覆盖（非追加）→ 光标在末尾可直接续写 6. 优化质量抽查：保留原意、逻辑通顺、无废话、语气一致、无解释性前后缀 7. 机器回复运行中按钮置灰；+新增/Read Only/书本图标/发送等原功能无回归 |
| 1962 | [zhangzhenwen1/dsh-task-effort](https://github.com/zhangzhenwen1/dsh-task-effort) | 0 | 2026-08-30 | 2026-08-30 | Auto-adjust model reasoning effort per task with DeepSeek peak-pricing-period capping: off/low/high/max classification, [effort=...] markers, error escalation, countdown notices |
| 1963 | [zhaoxuejie/dsh-plugin-feihualing](https://github.com/zhaoxuejie/dsh-plugin-feihualing) | 0 | 2026-09-03 | 2026-09-03 | DeepSeek Harness 飞花令游戏插件：简易 / 古法严格双模式，按会话独立维护令字、得分、已用诗句与剩余提示次数 |
| 1964 | [zhaozixi/dsh-attention](https://github.com/zhaozixi/dsh-attention) | 0 | 2026-08-28 | 2026-08-30 | DSH 跑任务时你通常只能盯着进度条。dsh-attention 把这段等待变成有产出的碎片时间 |
| 1965 | [zhchxiao123/dsh-devflow-plugins](https://github.com/zhchxiao123/dsh-devflow-plugins) | 0 | 2026-08-26 | 2026-08-30 | File-backed development workflow for DeepSeek Harness: durable cards, artifact and agent checks, human approvals, and a read-only web board. |
| 1966 | [zhengjy01/dsh-cloudflare-mcp](https://github.com/zhengjy01/dsh-cloudflare-mcp) | 0 | 2026-08-31 | 2026-08-31 | Cloudflare MCP connection for DeepSeek Harness |
| 1967 | [zhengjy01/dsh-qqbot-panel](https://github.com/zhengjy01/dsh-qqbot-panel) | 0 | 2026-08-31 | 2026-08-31 | Visual web settings panel for the official @tencent-connect/dsh-qqbot plugin: manage AppID/AppSecret, c2c & group access/allowlists, workspace picker, and scan-to-bind from the DSH web settings page |
| 1968 | [zhengjy01/dsh-vercel-mcp](https://github.com/zhengjy01/dsh-vercel-mcp) | 0 | 2026-08-30 | 2026-08-30 | Vercel MCP connection for DeepSeek Harness (DSH): official OAuth 2.0 flow (dynamic client registration + PKCE) against mcp.vercel.com, Vercel API tools under mcp__vercel__*, and a web settings panel |
| 1969 | [zhibailu/dsh-vsc](https://github.com/zhibailu/dsh-vsc) | 0 | 2026-08-23 | 2026-08-31 | Run DeepSeek Harness (DSH), a local AI agent, inside VS Code — native sidebar panel + editor bridge. A pure protocol client: no rewriting DSH, no second server |
| 1970 | [zhm20001/dsh-diary](https://github.com/zhm20001/dsh-diary) | 0 | 2026-09-04 | 2026-09-04 | dsh 日记插件：纸感信纸风 web 页写日记，原文先落盘、AI 评注后生成 · Diary plugin for dsh (DeepSeek Harness) |
| 1971 | [zhm20001/dsh-plugin-palette-board](https://github.com/zhm20001/dsh-plugin-palette-board) | 0 | 2026-08-31 | 2026-08-31 | 本项目为 DeepSeek Harness web 控制台带来一块 2D 调色盘应用板。唤出悬浮面板，即时搜索、分类过滤、全键盘导航，把散落在侧栏与浏览器里的插件页面收进一张可自定义的卡片网格。   |
| 1972 | [zhm20001/dsh-usage-board](https://github.com/zhm20001/dsh-usage-board) | 0 | 2026-08-27 | 2026-08-28 | dsh-usage-board 是专为 DSH (DeepSeek Harness) 设计的用量与成本可视化看板插件。  插件能实时捕获会话内的 Token 消耗、Step 耗时和异常指标，支持冷启动增量回溯历史全量会话，并按 Sub-agent DAG 调用关系进行树状归集与反向明细穿透。 |
| 1973 | [zhoujianbin/dsh-codex-continue](https://github.com/zhoujianbin/dsh-codex-continue) | 0 | 2026-08-29 | 2026-08-30 | DSH 插件：读取本机 Codex 项目与会话，一键在 DSH 里继续。Read local OpenAI Codex sessions and continue them in DeepSeek Harness. |
| 1974 | [zhubaohi/dsh-gpu-pulse](https://github.com/zhubaohi/dsh-gpu-pulse) | 0 | 2026-08-30 | 2026-08-30 | Floating GPU monitor (nvidia-smi) for the DSH Web UI — live per-GPU utilization, VRAM, temperature, power and fan, in the corner of the page. |
| 1975 | [ZhuYanTech/dsh-biomni](https://github.com/ZhuYanTech/dsh-biomni) | 0 | 2026-08-15 | 2026-08-31 | DeepSeek Harness biomni plugin |
| 1976 | [ZiFan1117/bazidiy](https://github.com/ZiFan1117/bazidiy) | 0 | 2026-08-26 | 2026-08-27 | 基于 DeepSeek Harness 的八字五行手串定制插件 |
| 1977 | [zisen123/dsh-reasoning-ruler](https://github.com/zisen123/dsh-reasoning-ruler) | 0 | 2026-08-30 | 2026-08-30 | Minimal reasoning-effort ruler for the DSH web composer: hairline + sliding marker, per-model memory, optimistic switching, streamlined model picker |
| 1978 | [ZK-Andy/dsh-frecency](https://github.com/ZK-Andy/dsh-frecency) | 0 | 2026-09-01 | 2026-09-02 | Resident-index + frecency file search for DeepSeek Harness — shadows the built-in grep/glob tools · DSH 常驻索引 + frecency 文件搜索，同名覆盖内置 grep/glob |
| 1979 | [zouxiaoyang/dsh-commandcode-usage](https://github.com/zouxiaoyang/dsh-commandcode-usage) | 0 | 2026-08-31 | 2026-08-31 | CommandCode usage & balance panel for DeepSeek Harness / DSH 的 CommandCode 用量与余额面板 |
| 1980 | [zpliao123/dsh-ark-quota](https://github.com/zpliao123/dsh-ark-quota) | 0 | 2026-08-27 | 2026-08-27 | Volcengine Ark Coding Plan / Agent Plan quota plugin for DeepSeek Harness (DSH) Web GUI: side float widget + settings page, persistent credentials, periodic auto-refresh, ark_coding_plan_usage model tool. |
| 1981 | [zptalk0221-cpu/dsh-remote-desktop](https://github.com/zptalk0221-cpu/dsh-remote-desktop) | 0 | 2026-08-26 | 2026-08-27 | 远程桌面移动化插件：为 DeepSeek Harness 提供手机横屏外壳与中文输入法 |
| 1982 | [zsxian11/dsh-flywheel](https://github.com/zsxian11/dsh-flywheel) | 0 | 2026-09-03 | 2026-09-03 | 面向 DeepSeek Harness（DSH） 的「会话飞轮」插件 。在单会话隔离下，让一条龙长会话接近当前句只带工作集；用项目级产物图 + 倒排在会话之间传递短卡。 |
| 1983 | [zuojinxin/dsh-provider-switch](https://github.com/zuojinxin/dsh-provider-switch) | 0 | 2026-08-28 | 2026-08-28 | Provider on/off switches, model search, and inline provider renaming for DeepSeek Harness. |
| 1984 | [zxheyi/dsh-work](https://github.com/zxheyi/dsh-work) | 0 | 2026-08-27 | 2026-08-27 | A plugin-native AI desktop for real work, built on DeepSeek Harness. |
| 1985 | [zzhi191/dsh-plugin-night-dog](https://github.com/zzhi191/dsh-plugin-night-dog) | 0 | 2026-08-29 | 2026-08-29 | A tan DeepSeek mascot dog named 夜官 that lives in the corner of the DSH web GUI: floats, reacts to the harness, adapts to the theme, and acts out a full repertoire (pant, stand, walk, tilt, yawn, bark, spin, whimper, lie down to sleep). Pure client plugin, installable from the DSH Community Market. |

## 从快照消失的已核准仓库 / Approved repositories missing from the snapshot

已核准但已不在当前快照中（删除或改名），核实后从 [data/approved.json](../approved.json) 移除或更新名称。

Approved but no longer present in the current snapshot (deleted or renamed) — after checking, remove them from [data/approved.json](../approved.json) or update the name.

- 0sour/dsh-plugins
- 0x5446/reins
- 1lyygit/dsh-launcher
- 240xu/tech-lead-skill
- ABccgh/dsh-agent-studio
- ABccgh/dsh-github-plugin-tools
- ABccgh/dsh-ima-plugin
- ABccgh/dsh-plugin-dev
- ABccgh/imakb
- ABccgh/ws-cleaner
- Agents365-ai/dsh-vision-plugin
- alaxrpg/dsh-adaptive-model-router
- alfonsoferrertorres-cyber/saare-suite
- ALwith-ai/alwith-dsh
- Arslan-jh/deepseek-harness-usage
- Axiaohungry/dsh-llm-codebuddy
- Bacskat/dsh-claude-ui
- BaronCyrus/dsh-ugui-preset
- bettermen/dsh-course-writer
- bitterSmilezzz/dsh-ui-tweaks
- BlackDawnNova/dsh-web-open
- blueWhalei/dsh-verify-gate
- CharlesAQ/dsh-fgo-chaldea
- Cheerwhy/dsh-chat-anchors
- chemmy-11/dsh-xuegulin
- chendefine/dsh-better-sidebar-onlyoffice
- chendefine/dsh-cdp-live-view
- chinaRXQ/dsh-wallpaper
- chumingjun/harness-one
- cking000bigdemon/dsh-acp-interactive
- cking000bigdemon/dsh-toolbelt
- coder-wu/dsh-finance-data
- coeasy/oh-my-dsh
- collapsey/xiaokui-pet
- crack-time/dsh-web-ui-skin
- cslht11/dsh-custom-patches
- cslht11/dsh-ssh-remote
- cyanfish-x/dsh-picture-fit
- cyanxi69-jpg/dsh-self-memory
- dat-lequoc/dsh-shots
- DDDFXYqiming/Agent_Extensions
- ddtcorex/dsh-maestro-harness
- dHR-P/dsh-anchored-wsl
- dolcejust-spec/dsh-event-watch
- dong3434/dsh-auto-maintenance
- dsh-external/chat-width
- dsh-external/dsh-agent-teams
- dsh-external/dsh-at-file
- dsh-external/dsh-automation
- dsh-external/dsh-bash-encoding
- dsh-external/dsh-better-browser
- dsh-external/dsh-book2skill
- dsh-external/dsh-browser4
- dsh-external/dsh-computer-use
- dsh-external/dsh-custom-tool
- dsh-external/dsh-cyber-sec
- dsh-external/dsh-daily-fortune
- dsh-external/dsh-deepcel
- dsh-external/dsh-deeplink
- dsh-external/dsh-deeptag
- dsh-external/dsh-doctor
- dsh-external/dsh-easy-ctx-manager
- dsh-external/dsh-fun-ticker
- dsh-external/dsh-fun-typewriter
- dsh-external/dsh-fun-weather
- dsh-external/dsh-genui
- dsh-external/dsh-grok-tui
- dsh-external/dsh-handoff
- dsh-external/dsh-input-history
- dsh-external/dsh-island
- dsh-external/dsh-minigames
- dsh-external/dsh-notification
- dsh-external/dsh-nowledge-mem
- dsh-external/dsh-open-in-vscode
- dsh-external/dsh-openmaic
- dsh-external/dsh-paste-input
- dsh-external/dsh-pet
- dsh-external/dsh-pet-corner
- dsh-external/dsh-pi-adapter
- dsh-external/dsh-plan-execute
- dsh-external/dsh-plannotator
- dsh-external/dsh-plugin-guide
- dsh-external/dsh-qq2006
- dsh-external/dsh-revive
- dsh-external/dsh-sentinel
- dsh-external/dsh-session-hub
- dsh-external/dsh-spotlight
- dsh-external/dsh-tps
- dsh-external/dsh-turn-rewind
- dsh-external/dsh-ui-progress
- dsh-external/dsh-ui-whale
- dsh-external/dsh-vision-toolkit
- dsh-external/dsh-visualize
- dsh-external/dsh-web-workbench
- dsh-external/dsh-webui-live-html
- dsh-external/oh-my-dsh
- DSHCorrectover/dsh-ccs-security
- EasyTZ/Deepseek-Harness-Desktop
- Entity-Him/dsh-doc-quick
- Entity-Him/dsh-harmonyos-market
- Entity-Him/dsh-hiboard-push
- Entity-Him/dsh-sky-skin
- fff122/dsh-agent-arcade
- fff122/dsh-prompt-presets
- fff122/dsh-research-notes
- fff122/dsh-task-checklist
- firestige/execution-system
- Foo1Moon/dsh-web-visualuiconfig
- g-yixuan/dsh-sidechat
- Gandufu/dsh-plugin
- Gaq152/dsh-attention
- Gaq152/dsh-credits
- ggggggggggz/dsh-config
- GM-HZ/dsh-dag-workflow
- Hann428/dsh-usage-dashboard
- harryopo/dsh-remote-ide
- hawkongz/doubao-vision-dsh
- henryZhouLikeStudy/deepseek-harness-lattice
- henryZhouLikeStudy/dsh-lattice-adapter-command
- henryZhouLikeStudy/dsh-lattice-adapter-dsh
- henryZhouLikeStudy/dsh-lattice-protocol
- henryZhouLikeStudy/dsh-lattice-runtime
- henryZhouLikeStudy/dsh-lattice-transports
- Hou-DL/dsh-token-heatmap
- huaxiren6/dsh-email-reader
- huaxiren6/dsh-remote-qr-button
- huaxiren6/dsh-sms-webhook
- hyls9527/dsh-local-vision
- ihuajiu/dsh-code-security
- ihuajiu/dsh-plugins-finder
- iTrimut/dsh-remote-access
- jianxx/dsh-cc-plugins
- jilian-dsh/dsh-rules-manager
- jiuge2467/DSH-WhaleDeck
- Jstn-1g/dsh-guarded-live-voice
- JUSTMONIKA2022/dsh-sandbox-escalation-fix
- kangjinghang/dsh-xueqiu
- KeS1Ke/dsh-exit
- KeyboardPrince/dsh-instruct-manager
- KeyboardPrince/dsh-skill-manager
- kiligzzz/dsh-capability-manager
- KKKneko/dsh-search-enhance
- krystal-cao/deepseek-harness-desktop
- krystal-cao/deepseek-harness-swift
- La-Theresa/dsh-math-modeling
- lamost423/dsh-trace-compare
- lhf6623/dsh-vibe
- liguobao/deepseek-harness-remote
- Lion-1209/dsh-plugin-wiki-skills
- Lion-1209/dsh-plugin-wiki-tools
- lmh-2026/dsh-periscope
- looput/dsn-finance-lab
- lovaxi/4d4y-browser
- lovstudio/dsh-plugin-creator-skill
- lovstudio/dsh-plugin-publisher-skill
- luoxunhao/deepseek-harness-plugins
- LXW419/dsh-claude-importer
- meliodascz89/deepseek-harness-plugins
- Minglink/dsh-infinite-gen-2
- morlay/session-persistence-rdb
- mrgaoang/dsh-remote
- mrlfarano/dsh-tailscale-surface
- mrpulor-gh/nuphus-mcp
- MST19711/dsh-opencode-go-usage
- nnbw-liu/deepseek-ai-dsh-llm-local
- NSOiO/talon-ui
- Nyzeep/dsh-thinking-level
- onlyforchris/dsh-plugin-manager
- oThTJx/dsh-skill-always-apply
- oThTJx/dsh-skill-impeccable
- oThTJx/dsh-skill-karpathy-guidelines
- oThTJx/dsh-skill-ponytail
- oThTJx/dsh-skill-superpowers
- oThTJx/dsh-skill-taste
- pgmi-builds/dashr
- plaask/fdtd-mcp
- PolinniZhong/dsh-session-kb
- qingzhuo-cn/agent-fix
- qinyre/dsh-plugin-atlas
- Qiwei-QW/dsh-r-ide
- qq1376868542-lang/dsh-tools
- ramen-ai-dev/ramen-ai-integrations
- sandbaseai/sandbase-skills
- satan9394/dsh-a11y-audit
- satan9394/dsh-academic-research
- satan9394/dsh-adhd-friendly
- satan9394/dsh-agent-loop-engineering
- satan9394/dsh-agent-reach
- satan9394/dsh-agent-teams
- satan9394/dsh-ai-image-design
- satan9394/dsh-algorithmic-art
- satan9394/dsh-api-design
- satan9394/dsh-api-documentation
- satan9394/dsh-api-scaffolding
- satan9394/dsh-architecture
- satan9394/dsh-auth
- satan9394/dsh-autonomous-research
- satan9394/dsh-bash-scripting
- satan9394/dsh-bash-testing
- satan9394/dsh-bazel-build-optimization
- satan9394/dsh-before-you-build
- satan9394/dsh-better-interface
- satan9394/dsh-blockchain-web3
- satan9394/dsh-brand-design
- satan9394/dsh-brand-guidelines
- satan9394/dsh-brand-landingpage
- satan9394/dsh-browser-testing
- satan9394/dsh-cad-modeling
- satan9394/dsh-canvas-design
- satan9394/dsh-career-ops
- satan9394/dsh-caveman-speak
- satan9394/dsh-changelog
- satan9394/dsh-channel-assistant
- satan9394/dsh-cicd
- satan9394/dsh-cli-anything
- satan9394/dsh-cloud-cost-optimization
- satan9394/dsh-cloud-well-architected
- satan9394/dsh-code-review
- satan9394/dsh-code-simplify
- satan9394/dsh-codebase-design
- satan9394/dsh-codebase-scanner
- satan9394/dsh-colleague-creation
- satan9394/dsh-commit-message
- satan9394/dsh-content-distillation
- satan9394/dsh-content-marketing
- satan9394/dsh-context-engineering
- satan9394/dsh-contract-review
- satan9394/dsh-css-art-styles
- satan9394/dsh-data-engineering
- satan9394/dsh-data-quality
- satan9394/dsh-data-storytelling
- satan9394/dsh-database-design
- satan9394/dsh-dataset-curation
- satan9394/dsh-db-migration
- satan9394/dsh-debug-recovery
- satan9394/dsh-deployment-validation
- satan9394/dsh-deprecation
- satan9394/dsh-designmd
- satan9394/dsh-desktop-agent-gui
- satan9394/dsh-diagram-design
- satan9394/dsh-discernment-nudge
- satan9394/dsh-distributed-debugging
- satan9394/dsh-doc-coauthoring
- satan9394/dsh-doc-compiled-skills
- satan9394/dsh-docs-adr
- satan9394/dsh-document-generation
- satan9394/dsh-domain-modeling
- satan9394/dsh-dotnet-backend
- satan9394/dsh-doubt-driven-dev
- satan9394/dsh-e2e-testing
- satan9394/dsh-error-handling
- satan9394/dsh-event-driven-architecture
- satan9394/dsh-file-conversion
- satan9394/dsh-framework-migration
- satan9394/dsh-frontend-design
- satan9394/dsh-frontend-engineering
- satan9394/dsh-frontend-mobile
- satan9394/dsh-frontend-slides
- satan9394/dsh-full-stack-orchestration
- satan9394/dsh-functional-programming
- satan9394/dsh-game-development
- satan9394/dsh-geo-seo
- satan9394/dsh-gif-creator
- satan9394/dsh-git-guardrails
- satan9394/dsh-git-workflow
- satan9394/dsh-gitops
- satan9394/dsh-grill-me
- satan9394/dsh-hallmark-design
- satan9394/dsh-handoff
- satan9394/dsh-harness-os
- satan9394/dsh-hot-trends
- satan9394/dsh-hr-legal-compliance
- satan9394/dsh-html-ppt
- satan9394/dsh-html-template-library
- satan9394/dsh-humanizer-zh
- satan9394/dsh-hybrid-cloud
- satan9394/dsh-idea-refine
- satan9394/dsh-incremental
- satan9394/dsh-internal-comms
- satan9394/dsh-investment-research
- satan9394/dsh-issue-triage
- satan9394/dsh-javascript-typescript
- satan9394/dsh-karpathy-methodology
- satan9394/dsh-knowledge-brain
- satan9394/dsh-kpi-dashboard-design
- satan9394/dsh-kubernetes-operations
- satan9394/dsh-last30days
- satan9394/dsh-live-docs
- satan9394/dsh-llm-api-integration
- satan9394/dsh-llm-eval
- satan9394/dsh-llm-finetuning
- satan9394/dsh-marketing-growth
- satan9394/dsh-mcp-builder
- satan9394/dsh-meeting-minutes
- satan9394/dsh-merge-conflicts
- satan9394/dsh-microservices
- satan9394/dsh-mlops
- satan9394/dsh-model-gateway
- satan9394/dsh-monorepo
- satan9394/dsh-multi-cloud
- satan9394/dsh-observability
- satan9394/dsh-observability-tools
- satan9394/dsh-obsidian-vault
- satan9394/dsh-office-cli
- satan9394/dsh-operating-kit
- satan9394/dsh-opinion-analysis
- satan9394/dsh-parallel-agent-ade
- satan9394/dsh-parallel-dev
- satan9394/dsh-payment-processing
- satan9394/dsh-pci-compliance
- satan9394/dsh-pdf-processing
- satan9394/dsh-performance
- satan9394/dsh-persistent-memory
- satan9394/dsh-personal-content-discovery
- satan9394/dsh-planning
- satan9394/dsh-planning-files
- satan9394/dsh-plugin-eval
- satan9394/dsh-ponytail-dev
- satan9394/dsh-postmortem
- satan9394/dsh-ppt-creator
- satan9394/dsh-pptx-engineering
- satan9394/dsh-prompt-audit
- satan9394/dsh-prompt-engineering
- satan9394/dsh-prototype
- satan9394/dsh-python-development
- satan9394/dsh-quant-backtest
- satan9394/dsh-rag
- satan9394/dsh-recsys-pipeline
- satan9394/dsh-relationship-coach
- satan9394/dsh-repo-graphify
- satan9394/dsh-reverse-engineering
- satan9394/dsh-review-agent-governance
- satan9394/dsh-runbook
- satan9394/dsh-sales-automation
- satan9394/dsh-sast-security
- satan9394/dsh-scientific-research
- satan9394/dsh-screenshot-to-code
- satan9394/dsh-security-compliance
- satan9394/dsh-security-hardening
- satan9394/dsh-security-requirements
- satan9394/dsh-self-improving-agent
- satan9394/dsh-service-mesh
- satan9394/dsh-setup-wizard
- satan9394/dsh-shipping
- satan9394/dsh-signed-audit-trails
- satan9394/dsh-skill-creator
- satan9394/dsh-skill-optimization
- satan9394/dsh-skill-seekers
- satan9394/dsh-slo
- satan9394/dsh-social-publishing
- satan9394/dsh-social-simulation
- satan9394/dsh-source-driven
- satan9394/dsh-spec-driven
- satan9394/dsh-sql-optimization
- satan9394/dsh-startup-business-analyst
- satan9394/dsh-superpowers-essentials
- satan9394/dsh-swarm-prediction
- satan9394/dsh-systems-programming
- satan9394/dsh-taste-review
- satan9394/dsh-tdd
- satan9394/dsh-teach
- satan9394/dsh-tech-debt
- satan9394/dsh-terraform
- satan9394/dsh-test-desktop-app
- satan9394/dsh-theme-factory
- satan9394/dsh-threat-modeling
- satan9394/dsh-to-questionnaire
- satan9394/dsh-track-driven-dev
- satan9394/dsh-vector-search
- satan9394/dsh-virtual-eng-team
- satan9394/dsh-wayfinder
- satan9394/dsh-web-artifacts
- satan9394/dsh-web-clone
- satan9394/dsh-web-scripting
- satan9394/dsh-webapp-testing
- satan9394/dsh-workflow-loop
- satan9394/dsh-writing-beats
- satan9394/dsh-writing-for-agents
- satan9394/dsh-writing-fragments
- satan9394/dsh-writing-shape
- satan9394/dsh-x-twitter-research
- sd1g1/dsh-minimal-rules
- sd1g1/dsh-muse-total-tps
- sd1g1/dsh-subagent-model-override
- seaskyblue/dsh-channel-feishu
- Semidia/dsh-friendly-errors
- shiyazhou666/dsh-token-plan-compare
- sparkmio/dsh-sfversion
- sqs404/dsh-gdi-art-plugins
- SsTtone1/dsh-message-cleaner
- statem-li/dsh-better-markdown
- statem-li/dsh-browser
- statem-li/dsh-image-gallery
- statem-li/dsh-reasoning-effort
- statem-li/dsh-tool-summary
- statem-li/dsh-usage-skill
- statem-li/dsh-vision-helper
- statem-li/dsh-zh-thinking
- Tasihi89/dsh-plugin-market
- tinchak0207/dsh-emu-workbench
- trrrrrryg/dsh-remote-workspace
- udsy19/dsh-toolcall-stream-repair
- urzeye/dsh-outline
- vikasranax/dsh-plugin-cats
- wanglaixiang-cyber/dsh-composer-scroll-hide
- wangweber/dsh-my-todo
- wezoo-wb/dsh-desktop-min
- whyitsy/dsh-plugins
- WSL043/dsh-native-deepseek-balance
- WSL043/dsh-native-reasoning-slider
- WSL043/dsh-native-session-manager
- Xiamu-ssr/snowmountain-market
- xiaoliang2/dsh-compact-after-task
- xie-tj/dsh-easy-exit
- xmutfyh/dsh-plugin-writing-guard
- XSakura666/ChronoAgent
- xuzhougeng/dsh-wisp-science-lab
- yhfgyyf/dsh-guardian-mode
- yustillrain/dsh-skill-browser
- Yvesgao/dsh-desktop-launcher
- Zh1rV/dsh-web-search-tavily
- zhaimingyou/aisync
- zhangyoufu-123/stylotrace
- zhongjie10086/dsh-adaptive-native-standard
