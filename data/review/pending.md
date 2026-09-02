# 待审核仓库 / Pending review

> 新增到 `dsh-plugin` Topic 下、带有简介、尚未经维护者核实的仓库。本文件由 `scripts/update.mjs` 每日刷新，仅供审核使用，不是用户可见页面。
>
> Repositories newly added to the `dsh-plugin` topic that the maintainer has not verified yet. Refreshed daily by `scripts/update.mjs`; review-only, not a user-facing page.

- 生成时间 / Generated: **2026-09-02**
- 快照日期 / Snapshot date: **2026-09-02 (UTC)**
- 待审核 / Pending: **1733**
- 从快照消失的已核准仓库 / Approved repositories missing from the snapshot: **401**

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
| 1 | [plastic-labs/honcho](https://github.com/plastic-labs/honcho) | 6989 | 2023-09-10 | 2026-09-02 |  Memory library for building stateful agents |
| 2 | [anbeime/skill](https://github.com/anbeime/skill) | 6082 | 2026-02-02 | 2026-09-01 | 收录最全、更新最快的技能Skills商店：精选原创技能包（涵盖文档处理、内容创作、编程开发、机器学习、自动化工作流），全部打包好可直接安装使用！同时自动抓取GitHub上万个Skills项目，按分类、更新时间、Star数量整理。The most comprehensive and frequently updated AI Agent skill library, featuring curated skill packs across document processing, content creation, programming, machine learning, automated workflows, and many more domains. |
| 3 | [huangruiteng/loopx](https://github.com/huangruiteng/loopx) | 5441 | 2026-05-31 | 2026-08-31 | Long-horizon agent control plane for durable, governed work across Codex, Claude Code, and other harnesses. |
| 4 | [chuspeeism/dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) | 2877 | 2026-07-24 | 2026-08-29 | 现代化可灵活嵌入的任务面板，支持 Codex、DeepSeek Harness |
| 5 | [AdamPlatin123/dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1441 | 2026-08-04 | 2026-08-28 | DSH Plugin Radar — 开源 DSH 插件生态雷达：自动发现 15900+ 候选、k8s 运行级实测 10000+、15 分钟快照管线；插件目录是其自动生成的 artifact |
| 6 | [Unclecheng-li/AI_Animation](https://github.com/Unclecheng-li/AI_Animation) | 1210 | 2026-04-11 | 2026-08-29 | 本项目整理了用于生成[炫酷 HTML 动画网页]的 AI Prompts，涵盖动画效果、3D 可视化、PPT 风格演示、UI 美化等多个类别。 |
| 7 | [platonai/Browser4](https://github.com/platonai/Browser4) | 1120 | 2018-03-12 | 2026-08-27 | Browser4 — an AI-native browser engine for autonomous agents, intelligent extraction, and large-scale web automation. |
| 8 | [Tiger3807861189/GLM-5.3-Flash-J-Space-Capability-Realization-Report](https://github.com/Tiger3807861189/GLM-5.3-Flash-J-Space-Capability-Realization-Report) | 1029 | 2026-08-16 | 2026-09-02 | GLM-5.3-Flash × J-Space capability realization — benchmark presentation of the J-Space Cognition Suite |
| 9 | [Minglink/dsh-infinite-gen-3](https://github.com/Minglink/dsh-infinite-gen-3) | 861 | 2026-08-15 | 2026-08-31 | DeepSeek 专用破甲插件「无限三代」dsh-infinite-gen-3 — armor-breaking plugin for DeepSeek，破甲版：稳定化破甲，求 Star 收藏 ⭐ |
| 10 | [wecode-ai/Wegent](https://github.com/wecode-ai/Wegent) | 772 | 2026-01-10 | 2026-08-30 | Plan, build, and deliver with an open-source, self-hostable AI workspace for coding, collaboration, and automation. |
| 11 | [myYangyunfan/dsh_desktop](https://github.com/myYangyunfan/dsh_desktop) | 623 | 2026-08-13 | 2026-08-30 | DeepSeek Harness (dsh) Windows desktop client - bundled Node.js + dsh CLI, one-click launch |
| 12 | [YuJunZhiXue/dsh-purge](https://github.com/YuJunZhiXue/dsh-purge) | 277 | 2026-08-19 | 2026-09-01 | DeepSeek Harness 破甲：让所有模型都能破甲，不同模型可换不同提示词；默认提示词面向国模「小码酱」。Jailbreak for every model — swap prompts per model. 求 Star 收藏 ⭐ |
| 13 | [leenkcool/Blue-Whale-Harness](https://github.com/leenkcool/Blue-Whale-Harness) | 190 | 2026-08-13 | 2026-09-01 | 🐋 DeepSeek Harness 插件总目录 · The catalog of DSH plugins：1958 个仓库 / 1819 个真插件（Skills · MCP · Tools · UI · Orchestration），中英文搜索、分类筛选、STAR 排序 → leenkcool.github.io |
| 14 | [liguobao/ds-harness-remote](https://github.com/liguobao/ds-harness-remote) | 156 | 2026-08-14 | 2026-08-30 | 一个基于 DeepSeek Harness 插件机制构建的多端远程访问方案，通过安全、低延迟、端到端加密的 P2P 优先网络，支持从 PC、Android 和 Web 随时访问并操作远程 Harness。 (A multi-device remote access solution built on the DeepSeek Harness plugin system, enabling PC, Android, and Web clients to securely access and operate a remote Harness over a low-latency, end-to-end encrypted, P2P-first network.) |
| 15 | [theBigGavin/marketingdashboard](https://github.com/theBigGavin/marketingdashboard) | 144 | 2026-07-17 | 2026-08-30 | 面向金融与产业研究的一屏式实时行情大屏：A股/港股/美股指数、大宗商品、美债收益率、板块热点、主力资金流、7×24 快讯、产业链自选股、AI 大模型 Token 追踪。A real-time market research cockpit on a single screen: CN/HK/US indices, commodities, treasury yields, sector hotspots, capital flows, 7×24 news, industry-chain watchlists and AI token usage trends.  |
| 16 | [fangqian616/consensus-pipeline](https://github.com/fangqian616/consensus-pipeline) | 117 | 2026-07-16 | 2026-08-30 | Multi-agent department framework for long-form complex tasks, fighting AI hallucination, validated on academic research. 共识管线：多智能体部门长线任务解决框架，对抗AI幻觉，以学术研究为验证场景。 |
| 17 | [Justin-sky/ai-art-engine](https://github.com/Justin-sky/ai-art-engine) | 116 | 2026-07-24 | 2026-08-31 | AI 艺术创作引擎，专业的短视频创作工具 |
| 18 | [xing-shuyin/pi-web-ui](https://github.com/xing-shuyin/pi-web-ui) | 84 | 2026-08-04 | 2026-09-02 | dsh / pi-agent web ui |
| 19 | [Jackywxsz/DSH-Creator](https://github.com/Jackywxsz/DSH-Creator) | 70 | 2026-08-25 | 2026-08-27 | Jacky Creator：面向内容创作者的 DeepSeek Harness 本地内容与运营工作台 |
| 20 | [lamost423/dsh-maze](https://github.com/lamost423/dsh-maze) | 62 | 2026-08-18 | 2026-08-27 | DeepSeek Harness 的执行迷宫——看 Agent 真实怎么干活：迷宫时间轴 · 数据轨道 · 确定性执行分析 · 多会话对比 \| The execution maze for DSH agents: maze timeline, per-step data tracks, deterministic execution analysis, multi-session comparison. Formerly dsh-trace-compare. |
| 21 | [SiriusNEO/StarAgent](https://github.com/SiriusNEO/StarAgent) | 56 | 2026-05-29 | 2026-09-02 | Lightweight agent multiplexer, all in one Web dashboard  |
| 22 | [niuhuoshan/launch-wechat-miniprogram](https://github.com/niuhuoshan/launch-wechat-miniprogram) | 44 | 2026-08-11 | 2026-08-31 | 面向完全新手的微信小程序 Agent Skill，从需求确认、原生 UI 和高保真原型，到 AppID、备案、开发测试、腾讯云后台、体验版、提审、发布及版本更新。 |
| 23 | [HakureiMonika/dsh-sandbox-escalation-fix](https://github.com/HakureiMonika/dsh-sandbox-escalation-fix) | 43 | 2026-08-16 | 2026-08-28 | Session-aware sandbox escalation compatibility plugin for DeepSeek Harness/DSH第三方模型会话沙箱升级兼容插件 |
| 24 | [KongFangXun/sofagent](https://github.com/KongFangXun/sofagent) | 42 | 2026-06-18 | 2026-09-01 | FDE Harness: audit-first governance for AI coding agents — 24 rules, HMAC chain, snapshot rollback (80 tools, 13 plugins) |
| 25 | [extracurricular-ai/dsh-filesnap](https://github.com/extracurricular-ai/dsh-filesnap) | 37 | 2026-08-27 | 2026-08-27 | dsh-filesnap — 把对话和它改过的文件一起回退到某一轮之前,不需要 git 仓库. A blazing-fast rewind and redo plugin for DeepSeek Harness, powered by a 🦀 Rust core, tracking the conversion and the files it changed, no git required, low disk consumption |
| 26 | [FrankHu-HK/mnemosyne](https://github.com/FrankHu-HK/mnemosyne) | 27 | 2026-08-10 | 2026-08-27 | Mnemosyne OS 7.0.0 — zero-dependency, local-first AI memory system (MCP / API / CLI / Python). MIT. |
| 27 | [See-Sol-Lab/DeepSeekGUI](https://github.com/See-Sol-Lab/DeepSeekGUI) | 27 | 2026-08-17 | 2026-08-27 | A Windows desktop client for DeepSeek Harness. V1 wraps the official Web UI; v2 (independent workbench) in development. |
| 28 | [tnnevol/fn-os-apps](https://github.com/tnnevol/fn-os-apps) | 24 | 2026-05-15 | 2026-09-01 | 飞牛 fnOS 应用 Monorepo |
| 29 | [SepineTam/cnki-mcp](https://github.com/SepineTam/cnki-mcp) | 23 | 2026-07-03 | 2026-09-01 | An MCP server for reach CNKI.  |
| 30 | [huaweicloud/huaweicloud-devkit](https://github.com/huaweicloud/huaweicloud-devkit) | 19 | 2026-07-28 | 2026-09-02 |  Official Huawei Cloud plugin for AI agents — skills, MCP tools, safety guardrails, and cloud sandbox to help AI agents build, deploy, and operate on Huawei Cloud securely. |
| 31 | [Suiwan/whale-purse](https://github.com/Suiwan/whale-purse) | 18 | 2026-08-14 | 2026-08-30 | A cute whale desktop pet for DeepSeek Harness that keeps an eye on your DeepSeek balance and session usage/cost. Drag her anywhere, click to open a live panel with real-time spend, peak/off-peak pricing, budget alerts, and history trends. |
| 32 | [chumingjun/dsh-harness-one](https://github.com/chumingjun/dsh-harness-one) | 17 | 2026-08-20 | 2026-08-27 | Visual AI workflow orchestrator for DeepSeek Harness (dsh): multi-agent DAGs, live execution, recovery, and Feishu integration. |
| 33 | [Ed-Marcavage/awesome-security-agent-harnesses](https://github.com/Ed-Marcavage/awesome-security-agent-harnesses) | 17 | 2026-08-03 | 2026-08-30 | AI agents for pentesting, code audit, fuzzing, vulnerability discovery, and reverse engineering — harnesses, sandboxes, security MCP servers, benchmarks, and evals. |
| 34 | [FishBottle7/opencode2dsh](https://github.com/FishBottle7/opencode2dsh) | 17 | 2026-08-29 | 2026-08-29 | DSH plugin — free OpenCode Zen models for DeepSeek Harness (DSH). Free LLM API, no API key needed. 在 DSH 中使用 OpenCode Zen 免费模型，无需 API key |
| 35 | [Jimmy0123-ux/dsh-token-pet](https://github.com/Jimmy0123-ux/dsh-token-pet) | 16 | 2026-09-01 | 2026-09-01 | DeepSeek Harness Desktop 悬浮用量小宠物：12 个正式逐帧动作反馈请求、工具、上下文压缩、归档与提示词增强；展示实时上下文占用、跨会话 Lifetime Ledger、服务商/模型统计和小时 Token 趋势；支持可编辑提示词增强、拖拽缩放、低性能模式与后台增量索引。 |
| 36 | [liangdabiao/dsh-plugin-developer-skill](https://github.com/liangdabiao/dsh-plugin-developer-skill) | 15 | 2026-09-01 | 2026-09-01 | dsh-plugin-developer — DeepSeek Harness 插件开发 Skill  > 指导 AI Agent 从 0 到 1 开发、构建、安装、测试 DeepSeek Harness（dsh）插件。基于 **dsh 0.1.1-rc.2** 与 dsh-openmaic 项目的完整实战经验，并内置一个**已通过 web 界面实测**的天气插件作为整包参考案例。  ## 这是什么  dsh 采用"无特权内核、万物皆插件"的设计：模型适配器、工具注册表、Agent 循环、网页界面都是插件 |
| 37 | [NekroAI/nekro-nxt](https://github.com/NekroAI/nekro-nxt) | 15 | 2026-08-15 | 2026-08-27 | NekroNXT：基于 DeepSeek Harness（DSH）的多平台群聊智能体系统｜A DSH-powered multi-platform group-chat agent system |
| 38 | [GZX2211/dsh-Visual-Workflow](https://github.com/GZX2211/dsh-Visual-Workflow) | 14 | 2026-08-15 | 2026-09-01 | 专为 DeepSeek Harness Web GUI 打造的可视化多 Agent 工作流编排插件。公开测试版已上线！接下来会随着 DSH 的正式版上线一并发布正式版！ |
| 39 | [ddtcorex/govard](https://github.com/ddtcorex/govard) | 13 | 2026-02-08 | 2026-08-28 | Go-based local development orchestrator for Magento, Laravel, Symfony, Next.js, WordPress, and more. Docker stacks, SSL, Xdebug, and a desktop dashboard. |
| 40 | [sagirimo/BioDSH](https://github.com/sagirimo/BioDSH) | 11 | 2026-08-31 | 2026-09-01 | The bioinformatics agent desktop for clinicians and wet-lab scientists — built on DeepSeek Harness. One-click installers, a skill store, offline mode. |
| 41 | [awesome-deepseekharness/awesome-deepseek-harness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness) | 10 | 2026-08-15 | 2026-08-27 | Awesome DeepSeek Harness (dsh) — curated awesome list of plugins, tools, skills & resources. Everything is a plugin. |
| 42 | [tinqiao-oss/clawtouch-mcp](https://github.com/tinqiao-oss/clawtouch-mcp) | 10 | 2026-06-01 | 2026-08-29 | ClawTouch MCP server — exposes a real USB-HID keyboard/mouse (Raspberry Pi Pico 2) as Model Context Protocol tools for any LLM agent. MIT. |
| 43 | [chen731215-dev/dsh-tavern-v2](https://github.com/chen731215-dev/dsh-tavern-v2) | 9 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Tavern Plugin - character card roleplay, worldbook management, preset switching, dark theme, memory summary, relationship graph, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 44 | [imsai-sh/dsh-1024store](https://github.com/imsai-sh/dsh-1024store) | 9 | 2026-08-24 | 2026-08-27 | DeepSeek Harness plugin store, marketplace and hub — 11,000+ dsh plugins with search, rankings, install commands and a free public API. DeepSeek Harness 插件市场 / 插件商店：自动收集与格式校验，免费搜索 API。deepseek1024.com |
| 45 | [keman-ai/dsh-skin-market](https://github.com/keman-ai/dsh-skin-market) | 9 | 2026-08-18 | 2026-08-27 | Skin marketplace for DeepSeek Harness — search and install community skins from dsh.a2hmarket.ai right in the settings page |
| 46 | [LaoYueHanNi/dsh-token-usage](https://github.com/LaoYueHanNi/dsh-token-usage) | 9 | 2026-08-14 | 2026-08-27 | 贴近 DSH 原生设计风格的 token 用量统计插件：实时记录每次请求的用量与费用，在 Web UI 中提供趋势图表、按模型定价明细和供应商配额显示。 |
| 47 | [cloveric/tarocub](https://github.com/cloveric/tarocub) | 8 | 2026-04-08 | 2026-08-29 | Feishu/Lark-first local AI agent gateway and native DeepSeek Harness plugin for Codex, Claude Code, Kimi Code, DeepSeek Harness, and Antigravity; Telegram optional. |
| 48 | [fb0sh/dsh-pentester](https://github.com/fb0sh/dsh-pentester) | 8 | 2026-08-19 | 2026-08-29 | 基于 DeepSeek Harness 的多 Agent PTES 渗透测试编排插件，支持自动化侦察、漏洞分析、验证与报告，使用 Docker/Kali 隔离工具箱 \| Multi-agent PTES penetration testing plugin for DeepSeek Harness with automated recon, vulnerability analysis, validation, reporting, and Docker/Kali toolbox |
| 49 | [greenthree/ProbHub-skill](https://github.com/greenthree/ProbHub-skill) | 8 | 2026-05-25 | 2026-08-30 | 算法竞赛出题自动化skill（个人出题习惯），支持完善题面、构造数据、组卷用typ编译pdf和生成domjudge题目包 |
| 50 | [PeterTXPan/dsh-unreal-mcp](https://github.com/PeterTXPan/dsh-unreal-mcp) | 8 | 2026-08-25 | 2026-08-31 | DeepSeek Harness Bundle for Unreal Engine 5.8 via Unreal MCP |
| 51 | [Ramenne/DeepSeek-Harness-Gov](https://github.com/Ramenne/DeepSeek-Harness-Gov) | 8 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 政务版：基于 deepseek-ai/deepseek-harness 的政务办事 WebUI 与红头公文插件 |
| 52 | [AngelosZou/graphlint](https://github.com/AngelosZou/graphlint) | 7 | 2026-07-01 | 2026-08-27 | Dead-code detection for AI-generated codebases: graphlint builds a dependency graph, finds code unreachable from any entry point to enable codebase cleanup and functional‑effectiveness understanding. |
| 53 | [BertramWang12399/dsh-projects-mode](https://github.com/BertramWang12399/dsh-projects-mode) | 7 | 2026-08-27 | 2026-09-01 | Project mode plugin for DSH Web GUI: sidebar entry, full-screen project manager, live per-project context injection (instructions + refreshable memory), session badge |
| 54 | [goatliamia/dsh-runtime-react](https://github.com/goatliamia/dsh-runtime-react) | 7 | 2026-08-31 | 2026-09-02 | 不要让 Model 为确定性问题反复思考，也不要让 Harness 为不确定的问题假装知道答案 |
| 55 | [jiazz197-cmyk/omd-dsh](https://github.com/jiazz197-cmyk/omd-dsh) | 7 | 2026-08-23 | 2026-08-29 | Multi-mode agent presets for DeepSeek Harness — per-mode model routing + tiered subagent delegation. |
| 56 | [maxwell-feng/dsh-windows-ocr](https://github.com/maxwell-feng/dsh-windows-ocr) | 7 | 2026-08-15 | 2026-09-01 | dsh plugin: OCR attached images locally with the built-in Windows OCR engine — text-only models can see, privacy-first |
| 57 | [RiemannRe3/DSH-RolePlay](https://github.com/RiemannRe3/DSH-RolePlay) | 7 | 2026-08-25 | 2026-08-27 | DeepSeek Harness 的 Tavern 角色卡兼容与原生 Agent RolePlay 插件。 |
| 58 | [JopenChen/dsh-go](https://github.com/JopenChen/dsh-go) | 6 | 2026-08-30 | 2026-08-31 | dsh-go 是一个纯 Go、进程内的 DeepSeek Harness Agent 实现 —— 让任意 Go 后端能以内嵌库的方式直接获得一个等价、具备规划能力的 Agent，无需界面、无需独立运行时。它不是又一个 ReAct 骨架，而是对 DSH 全量能力接缝的系统级复刻。 |
| 59 | [liceses/dsh-workspace-tree](https://github.com/liceses/dsh-workspace-tree) | 6 | 2026-08-18 | 2026-08-30 | 把 DSH Web 左侧栏的「工作区」重做为文件系统树双模式。核心原则： 工作区 = 目录强绑定——会话的 cwd 就是它所在的目录，环境真正隔离。 |
| 60 | [lw-storm/dsh-plugin-masterprompt](https://github.com/lw-storm/dsh-plugin-masterprompt) | 6 | 2026-08-27 | 2026-08-28 | This plugin is used for custom persona configuration. It facilitates users in code development and customized‑role setup, and supports flexible persona adjustments for each conversation. |
| 61 | [ParticleLight/dsh-all-usage](https://github.com/ParticleLight/dsh-all-usage) | 6 | 2026-08-17 | 2026-08-29 | DeepSeek Harness 用量看板 / Usage dashboard: tokens, cache, model/provider/workspace analytics, DeepSeek balance, heatmap, and CSV export. |
| 62 | [ppy-web/dsh-plugin-xiaomi-mimo-tts](https://github.com/ppy-web/dsh-plugin-xiaomi-mimo-tts) | 6 | 2026-08-20 | 2026-08-28 | 给DSH接入免费的 Xiaomi MiMo TTS API，支持使用预置/自定义声音朗读正文 |
| 63 | [Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl](https://github.com/Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl) | 6 | 2026-08-29 | 2026-08-31 | DeepSeek Harness（DSH）Web 界面右下角的常驻余额挂件。基于 MeteorNOX/DeepSeek-Balance-Whale-Widget 修改的铁盆鲸鱼娘版。 |
| 64 | [flymysql/dsh-memory](https://github.com/flymysql/dsh-memory) | 5 | 2026-08-14 | 2026-08-30 | DeepSeek Harness 跨会话记忆库：memory_remember/recall/forget 三个工具 + 系统提示注入，agent 持久化记忆 |
| 65 | [HuaJi2077/empty-fort-strategy](https://github.com/HuaJi2077/empty-fort-strategy) | 5 | 2026-08-29 | 2026-08-29 | DSH插件，感受空城计的巧妙，消耗多余的Token。 |
| 66 | [jukanntenn/grill-me-sleek](https://github.com/jukanntenn/grill-me-sleek) | 5 | 2026-05-28 | 2026-09-01 | Stress-test your plan before vibe coding. The AI asks you questions to build a shared understanding — you answer in a sleek web UI. |
| 67 | [keman-ai/dsh-skin-pack](https://github.com/keman-ai/dsh-skin-pack) | 5 | 2026-08-26 | 2026-08-27 | A full set of skins for DeepSeek Harness — one repository, each theme installable on its own |
| 68 | [LaoYueHanNi/dsh-git-worktree](https://github.com/LaoYueHanNi/dsh-git-worktree) | 5 | 2026-08-16 | 2026-08-30 | 在 Web 界面进行分支切换与 git worktree 隔离的 DSH 插件 |
| 69 | [recoluan/recowork](https://github.com/recoluan/recowork) | 5 | 2026-07-06 | 2026-08-27 | Give your AI a workflow. |
| 70 | [rogerdigital/dsh-searxng](https://github.com/rogerdigital/dsh-searxng) | 5 | 2026-08-16 | 2026-08-29 | DeepSeek Harness (dsh) plugin that adds a SearXNG-backed web_search provider to the ctx.web seam — free, self-hosted, key-less search instead of paid Exa/Perplexity APIs. |
| 71 | [scotthuang/agent-knock-knock](https://github.com/scotthuang/agent-knock-knock) | 5 | 2026-05-15 | 2026-08-31 | Control local Codex and Claude Code from OpenClaw through shared tmux terminals, with seamless human-agent handoff. |
| 72 | [Shaky77/weiwen-law-dsh](https://github.com/Shaky77/weiwen-law-dsh) | 5 | 2026-08-19 | 2026-08-27 | 唯稳律 (Weiwen's Law) 白箱风控 DSH 插件 — DeepSeek Harness 因果约束中间件 |
| 73 | [tta-lab/organon](https://github.com/tta-lab/organon) | 5 | 2026-03-18 | 2026-08-30 | Structure-aware tools for AI agents. Tree-sitter code editing, web page navigation, search. No daemon, no JSON, just stdin. |
| 74 | [VinciBeans/deepseek-plugin-liangwengu](https://github.com/VinciBeans/deepseek-plugin-liangwengu) | 5 | 2026-08-22 | 2026-08-31 | 梁文谷 DSH 插件：在 Web GUI 右上角显示当前算力错峰时段（已适配deepseek 2026.08.22 公布的最新峰谷收费政策，工作日 09:00–12:00 与 14:00–18:00 为梁文峰，其余时间含整个周末为梁文谷），并实时倒计时当前时段剩余时间；谷期跨天计算，直达下一工作日 09:00。 |
| 75 | [xianrui69/dsh-quick-phrases](https://github.com/xianrui69/dsh-quick-phrases) | 5 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: quick-phrase chip bar above the composer + /-triggered phrase menu |
| 76 | [xiaosurongjia/dsh-improved-inline-edit](https://github.com/xiaosurongjia/dsh-improved-inline-edit) | 5 | 2026-08-28 | 2026-08-29 |  当你的DSH正在工作时，你可以不用停止对话就可以再次提出要求 |
| 77 | [yu-wenchao/dsh-free-models-hub](https://github.com/yu-wenchao/dsh-free-models-hub) | 5 | 2026-08-26 | 2026-08-27 | 免费模型排行榜 · DeepSeek Harness 社区插件，在 DeepSeek Harness (DSH) Web UI 左侧边栏提供「免费模型榜」：分页浏览（每页 20 条、页码窗口、首页/末页）、 点击标题展开 API 调用地址 / 模型名称 / 【点击这里申请免费密钥key】按钮， 并支持一键配置到 设置 → 模型 → 自定义提供方 —— 用户只需自行粘贴免费 API Key |
| 78 | [ai-eks/dsh-docking-layout](https://github.com/ai-eks/dsh-docking-layout) | 4 | 2026-08-21 | 2026-08-29 | Organize unlimited conversation tabs into editor-style, drag-to-split groups for DeepSeek Harness Web. |
| 79 | [AstroLiao/dsh-launcher](https://github.com/AstroLiao/dsh-launcher) | 4 | 2026-08-15 | 2026-09-01 | Windows launcher for DeepSeek Harness running in WSL2 (dsh) |
| 80 | [better-er/dsh-cache-billing](https://github.com/better-er/dsh-cache-billing) | 4 | 2026-08-28 | 2026-08-28 | DSH 缓存账单插件：上下文圆环弹层里实时算账，峰谷自动计价，第三方中转照常记账 |
| 81 | [chengdb/dsh-plugin-capability-panel](https://github.com/chengdb/dsh-plugin-capability-panel) | 4 | 2026-08-21 | 2026-08-27 | 在 Web GUI 里可视化管理项目的全部能力——Skills、MCP 服务器、快捷消息， 全部支持项目级 / 全局级双作用域，全部可以不离开浏览器完成安装、启停与分发 |
| 82 | [Drhushi/dsh-plugin-tav2](https://github.com/Drhushi/dsh-plugin-tav2) | 4 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 插件 —— 对话式游戏本地化：跟 AI 助手说说话，完成游戏翻译全流程。引擎适配器架构，首发支持 Ren'Py。 |
| 83 | [dushaobindoudou/dsh-freeroute](https://github.com/dushaobindoudou/dsh-freeroute) | 4 | 2026-08-21 | 2026-08-27 | dsh free token route |
| 84 | [EasyTZ/dsh-desktop](https://github.com/EasyTZ/dsh-desktop) | 4 | 2026-08-20 | 2026-08-31 | Deepseek-Harness-Desktop |
| 85 | [Gru110110110/dsh-launcher](https://github.com/Gru110110110/dsh-launcher) | 4 | 2026-08-16 | 2026-09-02 | 让 DeepSeek Harness 人人可用的桌面入口——不用 Node、不用命令行，双击即用，还无损跟随每次官方更新。支持MacOs和Windows。DeepSeek Harness, for everyone. No Node.js. No command line. Just double-click and go. Always in step with every official update. For macOS & Windows. |
| 86 | [guoxiucai/dsh-code](https://github.com/guoxiucai/dsh-code) | 4 | 2026-08-16 | 2026-08-28 | pi tui  style code agent base on deepseek harness |
| 87 | [iimaguest/phone-tunnel-pool](https://github.com/iimaguest/phone-tunnel-pool) | 4 | 2026-08-23 | 2026-08-28 | Refreshable Cloudflare quick-tunnel pool for the dsh web GUI — phone access with QR + embedded login |
| 88 | [ItBayMax/dsh-replay-theater](https://github.com/ItBayMax/dsh-replay-theater) | 4 | 2026-09-01 | 2026-09-01 | Replay a DeepSeek Harness session at its original token cadence — an in-app playback theater with play/pause/step/speed/seek. |
| 89 | [liyi3068238601-oss/dsh-comfyui-ctl](https://github.com/liyi3068238601-oss/dsh-comfyui-ctl) | 4 | 2026-08-31 | 2026-08-31 | Native DeepSeek Harness plugin for controlling ComfyUI queues, history, outputs, models, uploads, and generation. |
| 90 | [meyaomiao/dsh-server-deck](https://github.com/meyaomiao/dsh-server-deck) | 4 | 2026-08-26 | 2026-08-28 | 服务器卡片仪表盘 for DeepSeek Harness — card dashboard (status/CPU/mem/disk) + one-click xterm terminal, better-sidebar tab or standalone drawer |
| 91 | [ningbonb/dsh-client-ui-brand](https://github.com/ningbonb/dsh-client-ui-brand) | 4 | 2026-08-26 | 2026-08-27 | Custom product name and logo branding for DeepSeek Harness Web 自定义 DeepSeek Harness Web 端 logo 和产品名称 |
| 92 | [null119/dsh-mcp-manage](https://github.com/null119/dsh-mcp-manage) | 4 | 2026-08-17 | 2026-08-30 | DSH（DeepSeek Harness）Web GUI 插件：在设置页管理 MCP 服务器——列出已安装工具，添加/编辑/删除、启用/停用；组合配置提供的 MCP 同样可在运行时直接编辑、停用、移除并恢复，无需重启宿主。 |
| 93 | [pgmi-builds/better-dsh](https://github.com/pgmi-builds/better-dsh) | 4 | 2026-08-16 | 2026-08-28 | Make your dsh ready for serious coding tasks. (Tools x Schemas)^REPL. skill://, ctx://, agent://, dvc://, dsh://, IPython REPL, Context as Variables, cross compaction recallable, full context revive. hash-edit, dvc://browser, subagent as a function, workflow as a function. |
| 94 | [RexCue/dsh-wallpaper](https://github.com/RexCue/dsh-wallpaper) | 4 | 2026-08-14 | 2026-08-30 | Wallpaper skin for the DeepSeek Harness (dsh) web UI: image background with opacity, mask and blur controls. |
| 95 | [vibe-any/dsh-plugin-save-token](https://github.com/vibe-any/dsh-plugin-save-token) | 4 | 2026-08-27 | 2026-08-27 | A DeepSeek Harness (dsh) dynamic plugin that cuts token cost without cutting model intelligence |
| 96 | [wkscc310/dsh-client-ui-cpa-quota](https://github.com/wkscc310/dsh-client-ui-cpa-quota) | 4 | 2026-08-17 | 2026-08-30 | Easily view your CLiProxyAPI quota in DeepSeek Harness. |
| 97 | [WSL043/dsh-chat-manager](https://github.com/WSL043/dsh-chat-manager) | 4 | 2026-08-15 | 2026-08-27 | DeepSeek Harness chat history and session management: search archives, restore conversations, and delete safely. |
| 98 | [yailPeralta/ast-mcp-server](https://github.com/yailPeralta/ast-mcp-server) | 4 | 2026-08-03 | 2026-08-29 | Correctness-oriented MCP server and batch CLI for compact structural reads and reviewed TypeScript/JavaScript edits. |
| 99 | [yohanchen1/MathModelingAgent](https://github.com/yohanchen1/MathModelingAgent) | 4 | 2025-08-11 | 2026-09-02 | Closed-loop scientific modeling agent with evidence-backed verification and reproducible correction. |
| 100 | [Z-6354/dsh-version-autoupdate](https://github.com/Z-6354/dsh-version-autoupdate) | 4 | 2026-08-18 | 2026-08-28 | DSH version badge + one-click auto-update (dual-surface Cordis plugin) |
| 101 | [173787247/dsh-wsl-open](https://github.com/173787247/dsh-wsl-open) | 3 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: open WSL Linux paths from chat in Windows. |
| 102 | [9931666/dsh-plugin-roundtable](https://github.com/9931666/dsh-plugin-roundtable) | 3 | 2026-08-22 | 2026-08-29 | （roundtable V0.2.2）把一次 DeepSeek Harness 会话，从"你和 AI 一对一聊天"，升级成"你 + 主持人(DeepSeek) + 一圈专家 AI 开圆桌会 |
| 103 | [addozhang/dsh-discord](https://github.com/addozhang/dsh-discord) | 3 | 2026-08-30 | 2026-08-31 | Discord-first adapter for DeepSeek Harness — sessions, streaming, approvals and controls from a Discord guild. |
| 104 | [Aliuyanfeng/dsh-soul](https://github.com/Aliuyanfeng/dsh-soul) | 3 | 2026-08-31 | 2026-08-31 | The DeepSeek Harness Personalization Settings plugin is used to configure the nickname, response style, tone, and custom commands of the Agent. |
| 105 | [AnLifeX/dsh-credits](https://github.com/AnLifeX/dsh-credits) | 3 | 2026-08-17 | 2026-08-29 | DeepSeek Harness（dsh web）额度插件：跟随当前模型显示官方余额或 OpenCode Go 订阅用量，支持本会话估算、跨会话累计消耗与可视化设置。 |
| 106 | [Binaryinject/dsh-review-checkout](https://github.com/Binaryinject/dsh-review-checkout) | 3 | 2026-08-26 | 2026-08-28 | dsh-review-checkout |
| 107 | [CodermanYHZ/dsh-node-flow](https://github.com/CodermanYHZ/dsh-node-flow) | 3 | 2026-08-27 | 2026-08-27 | 节点式 DSH 工作流画布：编排子代理、代码、条件、循环与定时任务，支持模型路由与 AI 生成指南。 Node-mode DSH workflow canvas: orchestrate sub-agents, code, conditions, loops & scheduled tasks. |
| 108 | [EL4CTEO/roblox-devforum-mcp](https://github.com/EL4CTEO/roblox-devforum-mcp) | 3 | 2026-03-30 | 2026-08-30 | Give your AI coding agent the Roblox DevForum and official creator docs — check if a bug is already known, read the accepted answer, and verify APIs before writing Luau. |
| 109 | [elizax/dsh-http-proxy](https://github.com/elizax/dsh-http-proxy) | 3 | 2026-08-26 | 2026-08-27 | 支持设置LLM的代理地址 |
| 110 | [Fakek0f3sT/dsh-mcp-diff](https://github.com/Fakek0f3sT/dsh-mcp-diff) | 3 | 2026-08-27 | 2026-08-27 | Uniform diff cards for every file mutation in DeepSeek Harness Web — MCP filesystem (edit_file/write_file) and built-in edit/write, collapsed by default, with per-line highlighting |
| 111 | [fengb3/dsh-session-icons](https://github.com/fengb3/dsh-session-icons) | 3 | 2026-08-22 | 2026-08-31 | DSH（DeepSeek Harness）Web 界面的会话标题图标插件：当模型为一次新会话生成标题时，宿主半用同一条路由发起一次辅助小请求，让模型按标题画一枚 24×24 单色 SVG 隐喻图标；浏览器半把它注入到左侧会话列表每行标题的左侧，跟随主题色。 |
| 112 | [fu827707013/dsh-concurrency-guard](https://github.com/fu827707013/dsh-concurrency-guard) | 3 | 2026-08-26 | 2026-08-27 | DSH（DeepSeek Harness）并发请求监控与门闩插件。 |
| 113 | [GM-HZ/agent-dag-workflow](https://github.com/GM-HZ/agent-dag-workflow) | 3 | 2026-08-23 | 2026-08-29 | Host-neutral durable DAG workflows for Agents: CLI-native access, fixed MCP gateway, on-demand Skills, triggers, replay, and visual Canvas. |
| 114 | [gulagala001/dsh-trisoul](https://github.com/gulagala001/dsh-trisoul) | 3 | 2026-08-27 | 2026-08-27 | TriSoul —— 三魂共识 Agent：三个灵魂盲写+匿名互评，三官（对齐/博识/实证）补偿生成，画布式上下文，记忆中枢。DeepSeek Harness 插件套件，一键装/独立端口/一键卸载 |
| 115 | [gwsbhqt/dsh-insight](https://github.com/gwsbhqt/dsh-insight) | 3 | 2026-08-25 | 2026-08-27 | 洞察 — read-only insight panel for a DeepSeek Harness profile: where every plugin, service, tool and model came from, which config layer inserted or disabled it, and what is running right now. |
| 116 | [harryopo/dsh-cloud-workspaces](https://github.com/harryopo/dsh-cloud-workspaces) | 3 | 2026-08-14 | 2026-08-31 | Cloud workspaces for DeepSeek Harness — pick Cloud (SSH) in the workspace picker and the agent's bash/read/write/edit/glob/grep tools transparently run on your Linux server over SSH. Zero remote install. |
| 117 | [HTian-qwq/prts-terrarchive](https://github.com/HTian-qwq/prts-terrarchive) | 3 | 2026-08-31 | 2026-08-31 | 为明日方舟的长篇剧情打造的RAG类DSH插件，拥有多种快速检索能力。 |
| 118 | [huanghai-lab/dsh-custom-instructions](https://github.com/huanghai-lab/dsh-custom-instructions) | 3 | 2026-08-15 | 2026-08-28 | DSH Web 安全自定义指令管理器：编辑全局 AGENTS.md，支持模板、Markdown 预览、历史恢复、导入导出与并发保护。 |
| 119 | [imMamdouhaboammar/get-fable](https://github.com/imMamdouhaboammar/get-fable) | 3 | 2026-08-11 | 2026-09-01 | Make the model you already use work more like a frontier model with better planning, persistent context, skills, hooks, failure handling, and verification |
| 120 | [jinxlux/xiao-theme-dsh-ui-plugin](https://github.com/jinxlux/xiao-theme-dsh-ui-plugin) | 3 | 2026-08-23 | 2026-08-29 | UI plugin for deepseek harness web |
| 121 | [Kevin66Z0/dsh-telegram](https://github.com/Kevin66Z0/dsh-telegram) | 3 | 2026-08-28 | 2026-09-02 | Remote-control DeepSeek Harness from Telegram: stream replies, one-tap keyboards, whitelist-secured, zero inbound ports. |
| 122 | [kirbylynx/dsh-hub](https://github.com/kirbylynx/dsh-hub) | 3 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Hub |
| 123 | [lansi-ai/dsh-desktop](https://github.com/lansi-ai/dsh-desktop) | 3 | 2026-08-25 | 2026-08-27 | 把 DeepSeek Harness 做成一个真正的桌面应用：Electron 主进程内嵌 Cordis Host（与官方 Web 版同内核、零移植）， 渲染进程加载官方 Web UI 发行物（file:///自定义协议 + IPC 桥接，不开放 HTTP 端口）， 所有桌面原生能力（托盘、全局热键、系统通知、剪贴板、开机自启、协议唤起、多窗口）以 host 插件 形态注入运行时， 与官方「一切皆插件」的架构同构——不是给网页套壳，而是把桌面能力变成可装配、可卸载、可审查的插件树。  AI 驱动开发声明 |
| 124 | [liangdabiao/dsh-weather-plugin](https://github.com/liangdabiao/dsh-weather-plugin) | 3 | 2026-09-01 | 2026-09-01 | dsh = 一台"所有零件都能换"的智能体机器。写插件 = 造一个零件装上去。本项目展示怎样开发一个天气插件：天气插件的设计：Node 端调 Open-Meteo 拿温度风力，浏览器端用这些数据画一张会动的天气卡片。 |
| 125 | [mantonlove/dsh-prism-plugin](https://github.com/mantonlove/dsh-prism-plugin) | 3 | 2026-08-18 | 2026-08-27 | Prism · 棱镜 — a deeply customizable glassmorphism theme plugin for the DeepSeek Harness Web GUI |
| 126 | [maxwell-feng/dsh-tesseract-ocr](https://github.com/maxwell-feng/dsh-tesseract-ocr) | 3 | 2026-08-15 | 2026-09-01 | dsh plugin: OCR attached images locally with Tesseract — text-only models can see, privacy-first |
| 127 | [maxwell-feng/dsh-tinyfish-search](https://github.com/maxwell-feng/dsh-tinyfish-search) | 3 | 2026-08-30 | 2026-08-30 | TinyFish-backed web search provider for DeepSeek Harness (ctx.web) — 将内置 web_search 接入 TinyFish Search API 的 DeepSeek Harness 插件 |
| 128 | [miaomiao636/dsh-message-navigator](https://github.com/miaomiao636/dsh-message-navigator) | 3 | 2026-08-15 | 2026-09-01 | DeepSeek Harness message navigator: a table of contents for long conversations — user-message outline, click-to-jump, scroll-synced highlight, search and Markdown outline export. |
| 129 | [NOirBRight/dsh-llm-opencode-go](https://github.com/NOirBRight/dsh-llm-opencode-go) | 3 | 2026-08-26 | 2026-08-29 | OpenCode Go LLM provider plugin for DeepSeek Harness |
| 130 | [QinpanWan/dsh-hiboard-push](https://github.com/QinpanWan/dsh-hiboard-push) | 3 | 2026-08-23 | 2026-08-27 | Push task-completion messages to the Huawei HarmonyOS assistant-today (负一屏) card feed from DeepSeek Harness — wire-compatible with the OpenClaw today-task skill. |
| 131 | [Scorpio69t/teach-math-with-manim](https://github.com/Scorpio69t/teach-math-with-manim) | 3 | 2026-08-19 | 2026-08-31 | Teach Math with Manim — 图书《用 Manim 讲好数学》官方配套开源仓库 |
| 132 | [snzhi000-sys/harness-macos-desktop-plugin-suite](https://github.com/snzhi000-sys/harness-macos-desktop-plugin-suite) | 3 | 2026-08-31 | 2026-09-02 | 基于 DeepSeek‑Harness 的 macOS 桌面定制客户端，在基座之上完成原生打包运行；内置多款自研、经过迭代优化的办公插件，适配产品经理轻度开发、PRD 文档撰写等办公场景。⚠️本项目属于社区第三方项目，非 DeepSeek 官方出品。 |
| 133 | [StvLi/dsh-phoenix](https://github.com/StvLi/dsh-phoenix) | 3 | 2026-08-30 | 2026-08-31 | Never-interrupt, resumable lifecycle for DeepSeek Harness (dsh): graceful restart + client auto-reconnect + cross-restart goal continuation. |
| 134 | [SuCriss/dsh-leekbox](https://github.com/SuCriss/dsh-leekbox) | 3 | 2026-08-26 | 2026-08-27 | 韭菜盒子 LeekBox — A股看盘助手 · DeepSeek Harness (DSH) web 插件 |
| 135 | [taoshi1999/dsh-workspace-hygiene](https://github.com/taoshi1999/dsh-workspace-hygiene) | 3 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin for agent workspace hygiene: artifact value assessment, metadata indexing, and auditable cleanup. |
| 136 | [tiphareth0/dsh-sshworkspaces](https://github.com/tiphareth0/dsh-sshworkspaces) | 3 | 2026-08-28 | 2026-08-31 | Workspace-level SSH remote development plugin for DeepSeek Harness: transparent seam-routed fs, git & terminal across multiple hosts and workspaces, with a built-in 4-column IDE and SSH ops toolkit. 提供工作区级 SSH 远程开发的Deepseek Harness插件：文件/Git/终端按工作区透明路由，支持多服务器多工作区并行开发，内置四列 IDE 与 SSH 运维工具。 |
| 137 | [Tkingxiao/dsh-novel-solo](https://github.com/Tkingxiao/dsh-novel-solo) | 3 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的「单核写作」插件：面向量化小模型做了充分的工具瘦身与输出加固，适合在本机用本地模型跑长篇小说流水线。 |
| 138 | [UncleK/dsh-think-translate](https://github.com/UncleK/dsh-think-translate) | 3 | 2026-08-24 | 2026-08-27 | Thinking-chain UI translation for DeepSeek Harness: 8 target languages, local Ollama model primary with in-panel download, Google/Bing fallback |
| 139 | [wbin0001/dsh-comfyui-canvas](https://github.com/wbin0001/dsh-comfyui-canvas) | 3 | 2026-08-31 | 2026-09-02 | DSH+ComfyUI画布插件dsh-comfyui-canvas embeds your ComfyUI instance as a split-screen canvas inside DeepSeek Harness Web. The agent writes prompts and edits nodes right in chat, applies them live to the canvas you're watching, and turns ideas into images, video, and 3D — all without switching front-ends. |
| 140 | [whutzefengxie-ops/dsh-shadow-mind](https://github.com/whutzefengxie-ops/dsh-shadow-mind) | 3 | 2026-08-24 | 2026-08-28 | Independent Shadow agent orchestration plugin for DeepSeek Harness |
| 141 | [wp-a/dsh-academic-paper-search](https://github.com/wp-a/dsh-academic-paper-search) | 3 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 的中文学术论文检索 Bundle：复用 Academic Paper Search MCP，支持多源检索去重、引用核验、引文图谱、MeSH、试验检索与审计导出。 |
| 142 | [wycto/dsh-dock](https://github.com/wycto/dsh-dock) | 3 | 2026-08-21 | 2026-08-28 | dsh-dock · DeepSeek Harness 功能中枢：用一张管理面板统一注册、开关所有小功能（模型余额、Token 用量记录、任务动画等）。每个功能独立模块，支持开关与错误隔离，新功能即插即用。0.1.0 为基础框架，功能接入按 README 路线图迭代。 |
| 143 | [x102201/deepseek-harness-helper](https://github.com/x102201/deepseek-harness-helper) | 3 | 2026-08-25 | 2026-08-27 | 🖥️ 一台电脑并行无限 DeepSeek Harness 实例 · 🔀 每个 dsh 一个专职实例 · 🪟 同一工作区并行 · 📦 .dshpack 配置交付 |
| 144 | [Xyanxhu/kilo-zen2dsh](https://github.com/Xyanxhu/kilo-zen2dsh) | 3 | 2026-08-31 | 2026-09-01 | Kilo Gateway free models for DeepSeek Harness (DSH) |
| 145 | [yaoshuo530/dsh-prompt-enhancer](https://github.com/yaoshuo530/dsh-prompt-enhancer) | 3 | 2026-08-28 | 2026-08-28 | A prompt-enhancement plugin for DeepSeek Harness: an ✨ Enhance composer button that rewrites prompts with first-principles thinking using session context, and asks clarifying questions when key info is missing. |
| 146 | [zh851233/docs-mode](https://github.com/zh851233/docs-mode) | 3 | 2026-08-25 | 2026-08-27 | You can use this plugin to complete the writing of technical documents, including development briefs, user manuals, reports/summary materials, and interface/API documentation, while reducing traces of AIGC. |
| 147 | [10086ggqq/dsh_theme_Minecraft](https://github.com/10086ggqq/dsh_theme_Minecraft) | 2 | 2026-09-02 | 2026-09-02 | 把 DeepSeek Harness 变成 Minecraft Java Edition 风格——WebGL 旋转全景主菜单、存档式会话选择、四种游戏模式对应 Agent 预设、世界内 HUD 聊天台、像素风工具卡片与审批面板、AI 思考时触发跑酷小游戏、8-bit 合成音效与自定义背景音乐、五类互动桌宠与红石粒子特效。零侵入 DSH 核心源码，经典界面一键切回。 |
| 148 | [162568316/dsh-tokenrhythm-bill](https://github.com/162568316/dsh-tokenrhythm-bill) | 2 | 2026-08-31 | 2026-08-31 | dsh-tokenrhythm-bill |
| 149 | [452926826/dsh-at-skill](https://github.com/452926826/dsh-at-skill) | 2 | 2026-08-25 | 2026-08-27 | Invoke DeepSeek Harness skills with @name and composer suggestions |
| 150 | [aiyacharley/dsh-pubmed](https://github.com/aiyacharley/dsh-pubmed) | 2 | 2026-08-27 | 2026-08-27 | DSH plugin for DeepSeek Harness: 25 model tools spanning PubMed, Europe PMC, PubTator3 & Semantic Scholar — entity-aware search, cross-source unified search, metadata, full text, citations, MeSH & ID tools, citation counts & recommendations — plus a personal literature knowledge graph with an AI-powered PubTator3 concept layer. |
| 151 | [Andiii208/gzhflow](https://github.com/Andiii208/gzhflow) | 2 | 2026-08-19 | 2026-09-01 | 跨 Agent 公众号内容发布工作流框架 — 素材先行/写作/去AI味/配图/排版/推草稿箱 六阶段流水线，适配 Claude Code/Cursor/Codex/Gemini/Qwen/DeepSeek 等主流 Agent |
| 152 | [AndKinoko/DSH-Search-Citation-Auditor](https://github.com/AndKinoko/DSH-Search-Citation-Auditor) | 2 | 2026-09-01 | 2026-09-01 | Audit citation sources in AI responses – extract URLs from the reply, score and rank them by threat level, and output a detailed report. Domains on your blocklist will be genuinely blocked – web tools such as web_search and web_fetch will directly refuse to access them. The blocklist is fully maintained by you. |
| 153 | [AnLifeX/dsh-attention](https://github.com/AnLifeX/dsh-attention) | 2 | 2026-08-20 | 2026-08-29 | dsh 提醒插件：别错过需要你的时刻 |
| 154 | [Ansonfishing/dsh-cap-profile](https://github.com/Ansonfishing/dsh-cap-profile) | 2 | 2026-08-28 | 2026-08-28 | Per-model capability profiling for DSH: turns local session history into tool-usage and error-rate dashboards with time-range filters |
| 155 | [AstroLiao/dsh-memory-core](https://github.com/AstroLiao/dsh-memory-core) | 2 | 2026-09-01 | 2026-09-01 | DeepSeek Harness cross-session long-term memory + user profile plugin: the AI remembers who you are, your projects and preferences across sessions. Pure Markdown, zero-config, fully local. (monorepo: dsh-memory-core + dsh-memory-ui) |
| 156 | [better-er/dsh-edit-diff](https://github.com/better-er/dsh-edit-diff) | 2 | 2026-08-28 | 2026-08-28 | dsh·去重复 diff 展示插件 |
| 157 | [bettermen/xiashuo](https://github.com/bettermen/xiashuo) | 2 | 2026-08-23 | 2026-08-30 | 虾说教材写作 · dsh-course-writer — AI course-authoring workspace plugin for DeepSeek Harness (DSH). 三栏式工作台 · 九阶段门禁 · 课程/章节/资料库/知识图谱 · 导出 TXT/Word · 分享协作。Three-pane workspace, nine-phase gated workflow, lorebook, export & share. |
| 158 | [BHXiang/auto-pwa](https://github.com/BHXiang/auto-pwa) | 2 | 2026-08-19 | 2026-08-28 | AI驱动的分波分析自动化。 |
| 159 | [BlueChonk/dsh-cli-anything](https://github.com/BlueChonk/dsh-cli-anything) | 2 | 2026-08-27 | 2026-08-27 | 将 CLI-Anything 集成到 DSH (DeepSeek Harness) 的插件方案。安装后通过自然语言对话即可浏览、安装、启动和管理 100+ CLI 工具。 |
| 160 | [CJL-1995/dsh-memory-self-evolution](https://github.com/CJL-1995/dsh-memory-self-evolution) | 2 | 2026-08-30 | 2026-08-31 | dsh自动进化记忆系统 |
| 161 | [CJYLZS/dsh-commandcode-plan-autosync](https://github.com/CJYLZS/dsh-commandcode-plan-autosync) | 2 | 2026-08-28 | 2026-08-28 | auto sync commandcode coding plan models in dsh |
| 162 | [CoolTea001/dsh-cool-theme](https://github.com/CoolTea001/dsh-cool-theme) | 2 | 2026-08-30 | 2026-08-30 | A plugin for changing themes for DSH, with a number of popular default themes built in. |
| 163 | [Crosery/dsh-viewer](https://github.com/Crosery/dsh-viewer) | 2 | 2026-08-31 | 2026-08-31 | Everything renders: images, video, audio, PDF, Office documents and local web pages inline in the DeepSeek Harness web UI, via a display_file tool. |
| 164 | [curtainsmall/dsh-electro-lab](https://github.com/curtainsmall/dsh-electro-lab) | 2 | 2026-08-22 | 2026-09-01 | Electrical & electronics calculation plugin for the DeepSeek Harness. 面向 DeepSeek Harness 的电气电子计算插件。 |
| 165 | [d86e/dsh-doctor](https://github.com/d86e/dsh-doctor) | 2 | 2026-08-27 | 2026-08-27 | dsh-doctor: self-healing watchdog for the DeepSeek Harness web profile. Recovers from plugin-induced boot failures within 60s, runs an unbounded CLI doctor, captures every tool error, and watches all live sessions for stuck turns. |
| 166 | [delock/dsh-pr-board](https://github.com/delock/dsh-pr-board) | 2 | 2026-08-26 | 2026-08-27 | Maintainer PR review queue board for DeepSeek Harness: five-state tracking (waiting on me / waiting on author / ready to merge / merged / inbox), sidebar counters, fullscreen kanban, polling, and back-to-you transition toasts. |
| 167 | [dingminhua/dsh-connect-workbuddy](https://github.com/dingminhua/dsh-connect-workbuddy) | 2 | 2026-08-28 | 2026-08-30 | Connect locally signed-in WorkBuddy models to DeepSeek Harness with a read-only credits overview and model management. |
| 168 | [everclear077/dsh-progressive-tools](https://github.com/everclear077/dsh-progressive-tools) | 2 | 2026-08-24 | 2026-08-27 | Progressive tool discovery for DeepSeek Harness — tiny stable surface, searchable catalog, real pipeline execution, context cache intact. |
| 169 | [ExplorerZYzhou/DSH-freeweb](https://github.com/ExplorerZYzhou/DSH-freeweb) | 2 | 2026-08-27 | 2026-08-27 | DSH 免费联网搜索插件（Parallel 后端，零依赖） |
| 170 | [felix-lj-ct/dsh-mcp-workspace-scope](https://github.com/felix-lj-ct/dsh-mcp-workspace-scope) | 2 | 2026-08-31 | 2026-08-31 | Scopes MCP tool injection per workspace directory in the DeepSeek Harness: a session opened in a project sees only the MCP servers that project needs — removed from the model's tool list and refused at call time. Plus per-session switches in the composer to narrow or widen the session you are in, temporarily. |
| 171 | [FraYoshi/dsh-ui-models-invert-selection](https://github.com/FraYoshi/dsh-ui-models-invert-selection) | 2 | 2026-08-29 | 2026-08-29 | Invert selection in Deepseek Harness for when we are selecting models  |
| 172 | [fufengyuan/dsh-stool-plugin](https://github.com/fufengyuan/dsh-stool-plugin) | 2 | 2026-08-25 | 2026-08-27 | DSH 运维工具箱插件。将 stool 运维 CLI 的全部能力注册为 DSH 模型可调用的工具，无需手动操作即可让 Agent 自动执行服务器管理、日志搜索、数据库查询、CI/CD 部署等操作。 |
| 173 | [gameswu/dsh-human-coding](https://github.com/gameswu/dsh-human-coding) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 增加古法编程模式，让模型监督你写代码！ |
| 174 | [hackernotfound/dsh-tacit](https://github.com/hackernotfound/dsh-tacit) | 2 | 2026-08-27 | 2026-08-27 | Learns what you leave unsaid in your prompts and steers the DeepSeek Harness agent for you |
| 175 | [Haniubub/seo-toolkit](https://github.com/Haniubub/seo-toolkit) | 2 | 2026-08-29 | 2026-08-30 | The SEO audit toolkit built for DeepSeek Harness (DSH) — runs locally, no Claude Code, no API key required. Self-contained port of claude-seo v2.2.5: 53 Python scripts + 24 sub-skills + 18 agents, weighted score, gated fan-out, schema.org, E-E-A-T, GBP, GEO/AI Overviews. |
| 176 | [hhb1028/dsh-retry-boost](https://github.com/hhb1028/dsh-retry-boost) | 2 | 2026-08-27 | 2026-08-27 | 让 DeepSeek Harness 自动重试商汤 429/QUOTA 等瞬时网关故障直到任务完成——启动时给所有 llm-pi-ai provider 热注入加固版 retryPolicy。 |
| 177 | [hi-fangj/dsh-models-radar](https://github.com/hi-fangj/dsh-models-radar) | 2 | 2026-08-26 | 2026-08-27 | Model capability radar plugin for the DeepSeek Harness Web GUI |
| 178 | [HiQ-AI/dingtalk-dsh-assistant](https://github.com/HiQ-AI/dingtalk-dsh-assistant) | 2 | 2026-08-25 | 2026-08-29 | 基于 DeepSeek Harness 的钉钉群聊常驻个人助理插件 |
| 179 | [Hou-DL/dsh-token-pulse](https://github.com/Hou-DL/dsh-token-pulse) | 2 | 2026-08-24 | 2026-08-28 | Local Token heatmap plugin for DSH Web — GitHub-style calendar views, per-hour/week/month/quarter/year, fully local, zero billing. |
| 180 | [hr98w/dsh-memory](https://github.com/hr98w/dsh-memory) | 2 | 2026-09-01 | 2026-09-01 | 融合 Claude Code 的 Auto Memory 与 Codex 的 Session 记忆整理，为 DeepSeek Harness 提供简单、透明、上下文友好的长期记忆。Claude Code-inspired Auto Memory meets Codex-inspired Session consolidation, bringing simple, transparent, and context-efficient long-term memory to DeepSeek Harness. |
| 181 | [huaxiren6/DSH-EmailReader](https://github.com/huaxiren6/DSH-EmailReader) | 2 | 2026-08-20 | 2026-08-27 | IMAP email reader for DeepSeek Harness: list, read, and search mail via imapflow (email_list / email_read / email_search). |
| 182 | [huaxiren6/DSH-SmsWebhook](https://github.com/huaxiren6/DSH-SmsWebhook) | 2 | 2026-08-20 | 2026-08-27 | SMS forwarding webhook for DeepSeek Harness: receive pushes from phone SMS Forwarder apps, store them, expose sms_recent / sms_search tools. |
| 183 | [ianho7/dsh-port-inspector](https://github.com/ianho7/dsh-port-inspector) | 2 | 2026-08-20 | 2026-08-30 | DeepSeek Harness 的 Windows Web 插件，可将本地 TCP 监听回溯至进程、会话与工具调用，保障编程助手安全处理端口冲突/A Windows DSH Web plugin for DeepSeek Harness that traces local TCP listeners back to processes, Sessions, and Tool Calls for safe Coding Agent port-conflict handling. |
| 184 | [imroc/dsh-project-prompt](https://github.com/imroc/dsh-project-prompt) | 2 | 2026-08-26 | 2026-08-27 | Private, per-project prompt rules for DeepSeek Harness — matched by git remote/repo/path, worktree-aware, never committed to the repo |
| 185 | [ipromise2021/dsh-omc-tui](https://github.com/ipromise2021/dsh-omc-tui) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness (DSH) 原生全功能终端交互界面 · Claude Code-styled Terminal TUI & CLI for DeepSeek Harness |
| 186 | [jarvisluk/dsh-projectless-session](https://github.com/jarvisluk/dsh-projectless-session) | 2 | 2026-08-18 | 2026-08-27 | Projectless sessions for DeepSeek Harness with isolated date-organized working directories |
| 187 | [jing-hy/dsh-unified-market](https://github.com/jing-hy/dsh-unified-market) | 2 | 2026-08-21 | 2026-08-27 | Unified plugin market for DSH Desktop (EAC): curated catalog + GitHub dsh-plugin + npm registry three sources; install/update management and .dshpack feature packs. 统一插件市场（三源聚合，EAC 特化）。 |
| 188 | [jingyunstudio/jingyun-dsh](https://github.com/jingyunstudio/jingyun-dsh) | 2 | 2026-08-27 | 2026-08-29 | 基于 Jingyun Studio + DeepSeek Harness (DSH) 打造的一站式 AI 商业化桌面客户端 |
| 189 | [jinsiyu/dsh-code-server-app](https://github.com/jinsiyu/dsh-code-server-app) | 2 | 2026-08-25 | 2026-08-27 | 将code-server（VSCode网页版）打包安装到dsh内的插件，快速实现专业的文件编辑。Package and install code-server (the web version of VSCode) as a plugin within dsh to quickly achieve professional file editing. |
| 190 | [jiuge2467/DSH-Desktop](https://github.com/jiuge2467/DSH-Desktop) | 2 | 2026-08-18 | 2026-08-28 | 🐬 专为小白与极客打造的 DeepSeek Harness 桌面全栈工作台：内置小鲸鱼姬桌宠、多源 MCP 调试沙箱、持久化终端与看板 \| The Geek & Cozy Desktop Client for DeepSeek Harness with Whale-chan Mascot, MCP Hub & Terminal. |
| 191 | [JochenYang/dsh-app](https://github.com/JochenYang/dsh-app) | 2 | 2026-08-20 | 2026-08-28 |   A community-maintained branded desktop client for  DeepSeek Harness, Windows / macOS / Linux |
| 192 | [justhalfbit/dsh-plugin-memory](https://github.com/justhalfbit/dsh-plugin-memory) | 2 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 跨会话记忆插件：对话模型边干边记的 Markdown 项目记忆，支持专题文件渐进式披露、可选后台静默蒸馏、按项目隔离与热更新设置面板。机制对齐 Claude Code auto memory。 \| Agent-maintained cross-session Markdown memory: progressive-disclosure topic files, opt-in silent distillation, per-project isolation. Claude Code-aligned. |
| 193 | [KannaKuron/dsh-better-workspace](https://github.com/KannaKuron/dsh-better-workspace) | 2 | 2026-08-30 | 2026-08-30 | DSH web plugin: a hierarchical workspace tree for the sidebar — titles containing / group into virtual folders; the add-workspace flow gains a parent-group popup |
| 194 | [Kilganon725/dsh-mic-dictation](https://github.com/Kilganon725/dsh-mic-dictation) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: mic dictation button next to the Full access control |
| 195 | [kiligzzz/dsh-skill-mcp-manager](https://github.com/kiligzzz/dsh-skill-mcp-manager) | 2 | 2026-08-21 | 2026-08-30 | Capability Manager for DeepSeek Harness: manage MCP servers and Skills from a Settings-page UI (dual-face dsh plugin) |
| 196 | [kober-basket/dsh-cachescope](https://github.com/kober-basket/dsh-cachescope) | 2 | 2026-08-26 | 2026-08-28 | Prompt-cache observability and logical-input diagnostics for DeepSeek Harness. |
| 197 | [leolee9086/dsh-zhihu-tools](https://github.com/leolee9086/dsh-zhihu-tools) | 2 | 2026-08-22 | 2026-08-31 | 知乎数据开放平台 DSH 静态双面插件:17工具+精美卡片+串行化限流。QQ群1017854502 https://qm.qq.com/q/RAHJuyhQQ |
| 198 | [lhuans/dsh-genui](https://github.com/lhuans/dsh-genui) | 2 | 2026-08-15 | 2026-09-01 | GenUI for DeepSeek Harness: interactive charts, forms, calculators, dashboards, and mini apps rendered inline in assistant replies, with actions that flow back to the model. |
| 199 | [lovaxi/Rubato_Plugins](https://github.com/lovaxi/Rubato_Plugins) | 2 | 2026-08-30 | 2026-09-01 | Make your AI's working state visible on a physical desk device - one Rubato plugin per coding agent. |
| 200 | [loyalchiiina/dsh-font-enhancer](https://github.com/loyalchiiina/dsh-font-enhancer) | 2 | 2026-08-27 | 2026-08-27 | DIY 你的 DSH 界面：按区域自定义字体/字号/颜色 \| DIY your DSH UI fonts & colors |
| 201 | [Lsc-91-69/dsh-brain-compaction](https://github.com/Lsc-91-69/dsh-brain-compaction) | 2 | 2026-08-28 | 2026-08-28 | 人脑式上下文压缩逻辑，大幅减少长任务上下文占用以及token消耗 |
| 202 | [luckzhangfengbo/dsh-web-theme](https://github.com/luckzhangfengbo/dsh-web-theme) | 2 | 2026-08-29 | 2026-08-29 | deepseek harness 背景主题插件 |
| 203 | [mackwan84/dsh-ui-mockup](https://github.com/mackwan84/dsh-ui-mockup) | 2 | 2026-08-26 | 2026-08-31 | DSH plugin for generating UI wireframes and high-fidelity mockups with DashScope Qwen/Wan and Volcengine Seedream. |
| 204 | [maxmilian/dsh-grafana-query](https://github.com/maxmilian/dsh-grafana-query) | 2 | 2026-08-26 | 2026-08-27 | Read-only Grafana metrics and alert tools for DeepSeek Harness (PromQL via datasource proxy). |
| 205 | [maxmilian/dsh-odoo](https://github.com/maxmilian/dsh-odoo) | 2 | 2026-08-26 | 2026-08-27 | Read-only Odoo tools for DeepSeek Harness, with an opt-in restricted draft-create tool. |
| 206 | [maxmilian/dsh-sentry](https://github.com/maxmilian/dsh-sentry) | 2 | 2026-08-26 | 2026-08-27 | Read-only Sentry issue and event tools for DeepSeek Harness. |
| 207 | [Medesol/dsh-kimi-formula](https://github.com/Medesol/dsh-kimi-formula) | 2 | 2026-08-31 | 2026-08-31 | Kimi (Moonshot AI) official Formula API tools for DeepSeek Harness — web_search via kimi-official provider + 10 kimi_* tools, no DeepSeek/Exa/Perplexity key needed |
| 208 | [meyaomiao/dsh-github-workbench](https://github.com/meyaomiao/dsh-github-workbench) | 2 | 2026-08-26 | 2026-08-27 | DSH 插件:在侧边栏使用 GitHub —— 仓库目录树 + Issues/PR/Actions 页签,支持建 Issue/PR、评论、合并、重跑 CI;better-sidebar 页签与独立面板双形态 |
| 209 | [mikasaxin529/dsh-nightshift](https://github.com/mikasaxin529/dsh-nightshift) | 2 | 2026-09-02 | 2026-09-02 | Off-peak task queue plugin for DeepSeek Harness — queue at peak price, drain at night, read the savings report |
| 210 | [ming-14/PTY-Agent](https://github.com/ming-14/PTY-Agent) | 2 | 2026-06-22 | 2026-08-31 |  Give your AI agent a real terminal: persistent PTY sessions, prompt-triggered returns, screen snapshots, and   TUI/GUI/crash awareness. |
| 211 | [miuzel/dsh-subagent-ui](https://github.com/miuzel/dsh-subagent-ui) | 2 | 2026-08-26 | 2026-08-27 | Searchable workspace subagent manager for DeepSeek Harness Web |
| 212 | [mrRisega/dsh-remote](https://github.com/mrRisega/dsh-remote) | 2 | 2026-08-19 | 2026-08-27 | Remote control for DeepSeek Harness (dsh web) from any phone browser: tunnel-mode relay client with one-command install and self-hosting support |
| 213 | [nabin-qq273274877/dsh-desktop](https://github.com/nabin-qq273274877/dsh-desktop) | 2 | 2026-08-31 | 2026-08-31 | DeepSeek Harness Desktop - 桌面启动器 (Tauri 2 + 内置 Node + 自动更新) |
| 214 | [Nagi-ovo/dsh-music-tui](https://github.com/Nagi-ovo/dsh-music-tui) | 2 | 2026-08-31 | 2026-08-31 | YesPlayMusic controls and now-playing status for dsh-TUI |
| 215 | [nickkkkkk123123/dsh-whale-girl](https://github.com/nickkkkkk123123/dsh-whale-girl) | 2 | 2026-08-27 | 2026-08-27 | 鲸鱼娘·灵动挂件 — 会卖萌、会记账、会弹跳的 DSH 桌面挂件插件（余额/用量/上下文/峰谷/右键菜单/拖动甩抛） |
| 216 | [niuhuoshan/dsh-connect](https://github.com/niuhuoshan/dsh-connect) | 2 | 2026-08-29 | 2026-08-31 | DeepSeek Harness 数据源连接插件，支持数据库元数据发现、AI 语义建模、只读 SQL 查询和固定 HTTP API 调用 |
| 217 | [omdsh-dev/dsh-file-trace](https://github.com/omdsh-dev/dsh-file-trace) | 2 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 218 | [pax-beehive/dsh-hub-cli](https://github.com/pax-beehive/dsh-hub-cli) | 2 | 2026-08-25 | 2026-09-02 | Open-source CLI, schemas, resolver, and DSH agent tools for DSH Plugin Hub |
| 219 | [ph4310822/dsh-edex-jarvis-ui](https://github.com/ph4310822/dsh-edex-jarvis-ui) | 2 | 2026-08-25 | 2026-08-27 | DeepSeek Harness eDEX-UI shell plugin — JARVIS variant: electric cyan HUD with VITAL SIGNS / RT-MONITOR / RT-LOG left bar, POWER CORE / RADAR right bar, JARVIS header |
| 220 | [PianoPrince/dsh-workspace-mover](https://github.com/PianoPrince/dsh-workspace-mover) | 2 | 2026-08-26 | 2026-08-30 | 拖拽跨工作区真迁移 DSH 会话：批量移动、挂错归位、分组合并；步步备份回滚，零 token 消耗 / Move DSH sessions across workspaces by drag & drop — true migration, batch move, misfiled homing, group merge; backups + rollback, zero tokens. |
| 221 | [pirate-608/dsh-multi-tools](https://github.com/pirate-608/dsh-multi-tools) | 2 | 2026-08-14 | 2026-08-31 | Multimodal tool suite for DeepSeek Harness: ModLens vision, local ComfyUI, Unity, creative apps, CAD, and Ren'Py. |
| 222 | [PolinniZhong/dsh-session-workbench](https://github.com/PolinniZhong/dsh-session-workbench) | 2 | 2026-08-21 | 2026-08-30 | Session Workbench for DeepSeek Harness: session-library full-text search + recall + conversation-view management (show/hide + reorder). 会话工作台：会话库（历史会话全文搜索与召回）+ 会话视图（标签栏显示/隐藏 + 拖拽排序）。 |
| 223 | [Qian-Ning/prompt-skill-armory](https://github.com/Qian-Ning/prompt-skill-armory) | 2 | 2026-08-27 | 2026-08-30 | Managing prompts，, skills, MCP tools & wallpaper for DeepSeek Harness |
| 224 | [qingmomo233/dsh-thinking-language](https://github.com/qingmomo233/dsh-thinking-language) | 2 | 2026-08-16 | 2026-08-29 | 更改 deepseek harness 思考过程语言 |
| 225 | [QinpanWan/dsh-sky-skin](https://github.com/QinpanWan/dsh-sky-skin) | 2 | 2026-08-25 | 2026-08-27 | Sky: Children of the Light themed skin for DeepSeek Harness web UI - light children on a glowing star map, candlelight gold and starry night. 光遇·遇境主题皮肤。 |
| 226 | [rootkiller6788/dsh-launcher](https://github.com/rootkiller6788/dsh-launcher) | 2 | 2026-08-31 | 2026-08-31 | DSHL — A desktop launcher for managing AI runtimes, instances, plugins, MCP servers, skills, profiles, and distributions. |
| 227 | [SaekiRaku/deepseek-rainbow-fart](https://github.com/SaekiRaku/deepseek-rainbow-fart) | 2 | 2026-08-26 | 2026-08-31 | 当你使用 DeepSeek Harness WebUI 发送消息后，插件会基于你的内容生成夸赞你的话，并通过 TTS 合成并播放声音。 \| After you send a message via DeepSeek Harness WebUI, the plugin generates compliments based on your input and plays them via TTS. |
| 228 | [sakthiveltofficial/dsh-shopify-plugins](https://github.com/sakthiveltofficial/dsh-shopify-plugins) | 2 | 2026-08-26 | 2026-08-27 | Shopify plugin for DeepSeek Harness: 213 model-facing shopify_* tools over the Shopify Admin REST + GraphQL APIs (products, orders, customers, inventory, fulfillments, discounts, content, webhooks, themes, billing, bulk operations) with Admin API access-token auth. |
| 229 | [seewhydee/dsh-emacs-bridge](https://github.com/seewhydee/dsh-emacs-bridge) | 2 | 2026-08-23 | 2026-08-27 | Deepseek Harness to Emacs bridge |
| 230 | [SeverusZh/dsh-skills-mcp-group-manager](https://github.com/SeverusZh/dsh-skills-mcp-group-manager) | 2 | 2026-08-28 | 2026-08-28 | DeepSeek Harness Skills & MCPs 分组管理器 — 分组管理 Skills、过滤模型技能目录、独立开关 MCP 服务器、左侧面板一键管理 / Group skills, filter the model skill catalog, toggle MCP servers, left panel UI |
| 231 | [Shyboy0499/dsh-git-tools](https://github.com/Shyboy0499/dsh-git-tools) | 2 | 2026-08-26 | 2026-08-27 | Local git tools for DeepSeek Harness (dsh): git_status, git_diff, git_log, git_commit |
| 232 | [squirrel20/dsh-cron](https://github.com/squirrel20/dsh-cron) | 2 | 2026-08-26 | 2026-08-27 | Unattended scheduled jobs for the DeepSeek Harness (dsh): agent/command tasks on cron schedules |
| 233 | [STARDUSTLC666/dsh-cite](https://github.com/STARDUSTLC666/dsh-cite) | 2 | 2026-08-15 | 2026-08-27 | DeepSeek Harness 参考文献插件：cite_lookup/check/format/bibtex/health 五工具，DOI 精确查询、Crossref 题录检索、GB/T 7714/APA/MLA/Chicago 格式化、有界并发 DOI 校验；纯 Node 全平台。· Citation tools for DeepSeek Harness agents. |
| 234 | [starefinger/dsh-llm-qwen-local](https://github.com/starefinger/dsh-llm-qwen-local) | 2 | 2026-08-26 | 2026-08-27 | 面向 DeepSeek Harness(dsh)的 LLM 适配器插件:驱动由 OpenAI 兼容服务的本地部署 Qwen3.8-27B 模型。支持按模型多模态开关、完全可配置的推理档位、请求图像投影,以及中英双语 Web 设置页。 |
| 235 | [statem-li/dsh-triad](https://github.com/statem-li/dsh-triad) | 2 | 2026-08-28 | 2026-08-28 | 用量趋势 · 技能与 MCP Server 管理 · 自动沉淀的长期记忆——一套插件装齐 DSH 三个工作台。纯插件注入，不动官方源码，一句话安装。 |
| 236 | [Stylelinzzz/dsh-chat-history](https://github.com/Stylelinzzz/dsh-chat-history) | 2 | 2026-08-17 | 2026-08-30 | Chat history TOC for DeepSeek Harness: a History conversation view tab listing user messages with auto-paging and click-to-jump back into the chat. / DeepSeek Harness 会话目录插件：用户消息历史一键跳转。 |
| 237 | [summer-521/deepseek-harness-desktop](https://github.com/summer-521/deepseek-harness-desktop) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness 的非官方桌面封装：本地优先、沙箱隔离，内置 dsh 版本管理与插件管理，支持自动更新与任务完成桌面通知（macOS）。 |
| 238 | [SUONSUN9527/deepseek-harness-flow-arrange](https://github.com/SUONSUN9527/deepseek-harness-flow-arrange) | 2 | 2026-08-31 | 2026-08-31 | Claude-orchestrator x Codex-executor distribution of DeepSeek Harness |
| 239 | [supersyh-sss/dsh-voice-assistant](https://github.com/supersyh-sss/dsh-voice-assistant) | 2 | 2026-08-29 | 2026-08-30 | Offline voice assistant for dsh web — wake word, speech dictation, voice edit commands & Chinese TTS. On-device sherpa-onnx WASM ASR, no Google dependency, works in China. |
| 240 | [swordordead/dsh-Veneer](https://github.com/swordordead/dsh-Veneer) | 2 | 2026-08-18 | 2026-08-31 | DIY你的小蓝鲸吧 |
| 241 | [theoneLee/deepseek-harness-sdk-go](https://github.com/theoneLee/deepseek-harness-sdk-go) | 2 | 2026-08-15 | 2026-08-27 | Go SDK for driving DeepSeek Harness |
| 242 | [Tsqurt/dsh-plugin-studio](https://github.com/Tsqurt/dsh-plugin-studio) | 2 | 2026-08-27 | 2026-08-28 | 为了开发插件，开发了一个开发插件的插件。通过可视化的事件流、插件管理、工具管理、技能管理、预设管理，简化插件的开发流程，方便开发者理解插件的作用。 |
| 243 | [unknowbug/dsh-thinking-loop-guard](https://github.com/unknowbug/dsh-thinking-loop-guard) | 2 | 2026-08-27 | 2026-08-27 | Detect & break thinking-chain loops in DSH agents at the turn boundary (no proxy). Ported from ollama-loop-guard. |
| 244 | [vuldin/yapa](https://github.com/vuldin/yapa) | 2 | 2026-03-24 | 2026-08-27 | Yet Another Personal Assistant |
| 245 | [wang-kaopu/dsh-cordis-devtools](https://github.com/wang-kaopu/dsh-cordis-devtools) | 2 | 2026-08-23 | 2026-08-27 | Give coding Agents runtime evidence for debugging and verifying DSH / Cordis plugins. 让 Coding Agent 获得用于调试和验证 DSH / Cordis 插件的运行时证据。 |
| 246 | [wangxueqi00/dsh-client-ui-knowledge-cards](https://github.com/wangxueqi00/dsh-client-ui-knowledge-cards) | 2 | 2026-08-31 | 2026-08-31 | A plugin of Deepseek Harness(DSH),transform your recent chat history into beautifully designed knowledge cards, ready to download and share. |
| 247 | [wanyexin1998/dsh-workbench](https://github.com/wanyexin1998/dsh-workbench) | 2 | 2026-08-26 | 2026-08-27 | Community-maintained source preview for two-Pane DeepSeek Harness Web workflows |
| 248 | [whh110112/human-writing-skills](https://github.com/whh110112/human-writing-skills) | 2 | 2026-06-15 | 2026-09-01 | Advanced multilingual AI humanizer and writing toolkit for natural prose, voice preservation, long-form continuity, and focused audits. |
| 249 | [wishesl/dsh-launcher](https://github.com/wishesl/dsh-launcher) | 2 | 2026-08-28 | 2026-08-29 | Manage DSH plugins & runtime without launching it: plugin market, per-instance masking, version install. Wails v2 (Go + React).  DeepSeek Harness 桌面启动器：不启动 DSH 即可安全管理插件与本体——多实例/多版本一键启动、实时日志、npm 版本查询、插件市场（安装/卸载/开关/收藏/分享码）、实例级插件临时屏蔽。基于 Wails v2 (Go + React)。 |
| 250 | [WSL043/dsh-reasoning-slider](https://github.com/WSL043/dsh-reasoning-slider) | 2 | 2026-08-23 | 2026-08-27 | 已归档：DeepSeek Harness 模型感知推理强度滑杆；现有 Release 与演示保留，不再适配未来 DSH。 |
| 251 | [x1shang/dsh-koin-lily-news](https://github.com/x1shang/dsh-koin-lily-news) | 2 | 2026-08-21 | 2026-08-27 | 菲奖得主强推的百合新闻订阅DSH插件 |
| 252 | [xiaoguomeiyitian/dsh-qr-share](https://github.com/xiaoguomeiyitian/dsh-qr-share) | 2 | 2026-08-29 | 2026-08-30 | DSH web plugin: a sidebar-footer QR-code button that lets a phone scan and re-issue the current browser's authenticated launch URL. |
| 253 | [xiaoso456/dsh-tool-plus](https://github.com/xiaoso456/dsh-tool-plus) | 2 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 基础工具增强：持久 bash、结构化 read、多模式 edit、原子 write、双引擎 grep/glob、图像直读，一个插件全覆盖 |
| 254 | [Ycet/dsh-awesome-hud](https://github.com/Ycet/dsh-awesome-hud) | 2 | 2026-08-29 | 2026-08-30 | dsh侧边HUD面板，包含多个信息展示模块（可自定义是否展示），集成压缩上下文、查看git graph等功能。DSH side HUD panel, containing multiple information display modules (customizable whether to display), integrating features such as compressed context, viewing git graph, etc. |
| 255 | [yhfgyyf/dsh-audit-mode](https://github.com/yhfgyyf/dsh-audit-mode) | 2 | 2026-08-23 | 2026-09-02 | Guardian preset for DeepSeek Harness with independent persistent Codex auditing |
| 256 | [yuioi666/dsh-plugin-model-capability](https://github.com/yuioi666/dsh-plugin-model-capability) | 2 | 2026-08-27 | 2026-08-31 | Model Capability Manager for DSH Web: thinking levels, context window, output caps, input modalities, gateway compat presets, EN/中文 UI. \| DSH 网页端模型能力管理插件。 |
| 257 | [Yur0918/dsh-user-addons](https://github.com/Yur0918/dsh-user-addons) | 2 | 2026-08-28 | 2026-08-28 | Community DSH web plugin for file uploads, archived-session management, image capability detection, and model/token usage insights. |
| 258 | [yushi-javatoai/ai-web-ppt-maker](https://github.com/yushi-javatoai/ai-web-ppt-maker) | 2 | 2026-08-31 | 2026-08-31 | AI 网页 PPT 生成器：粘贴长文案，AI 流式拆解为多页网页 PPT，支持全屏演示、键盘翻页、多套主题与独立 HTML 导出。 |
| 259 | [Yvesgao/dsh-shortcut-creator](https://github.com/Yvesgao/dsh-shortcut-creator) | 2 | 2026-08-15 | 2026-08-30 | DSH 启动器- 在 DSH 设置页一键创建 Windows 桌面快捷方式，自动打开浏览器、可固定任务栏。DSH plugin: one-click Windows desktop shortcut launcher from the Settings page (DeepSeek Harness or any local server) —Install: dsh plugin --profile web add github:Yvesgao/dsh-desktop-shortcut#main |
| 260 | [yxv1203-collab/dsh-conversation-archive](https://github.com/yxv1203-collab/dsh-conversation-archive) | 2 | 2026-09-01 | 2026-09-01 | Native archive, retention, safe deletion, and verified backup management for DeepSeek Harness. |
| 261 | [zhenghaoyang24/obsidian-plugin-deepshian](https://github.com/zhenghaoyang24/obsidian-plugin-deepshian) | 2 | 2026-08-27 | 2026-08-27 | Sidebar AI chat powered by the local DeepSeek Harness (dsh): streaming replies, tool calls, and real vault file edits. |
| 262 | [zhoulvyuan/dsh-plugin](https://github.com/zhoulvyuan/dsh-plugin) | 2 | 2026-08-26 | 2026-08-28 | deepseek-harness插件 |
| 263 | [zzy-12345678/dsh-file-convert](https://github.com/zzy-12345678/dsh-file-convert) | 2 | 2026-08-29 | 2026-08-30 | Local-first file conversion for DeepSeek Harness — images, PDF, data, audio/video & office docs. 7 tools, 26 conversions, no API keys, no uploads. |
| 264 | [0x5446/rowel](https://github.com/0x5446/rowel) | 1 | 2026-08-14 | 2026-09-01 | Native iOS client for DeepSeek Harness (dsh). Answer your agent from your phone — the relay only ever sees ciphertext. |
| 265 | [0xrushmoon/dsh-freeroute](https://github.com/0xrushmoon/dsh-freeroute) | 1 | 2026-08-25 | 2026-08-27 | Free-tier model aggregation plugin for the DeepSeek Harness (dsh): transparent failover, multi-key rotation, settings panel |
| 266 | [166767/dsh-error-audit](https://github.com/166767/dsh-error-audit) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 实时 AI 自审插件：任何报错/警告第一时间连同时间、错误码、会话、用户原话、AI 动作与工作区写入专用日志目录，并主动通知 AI、内置 read_error_logs 工具随时读取。Real-time AI self-audit for DeepSeek Harness — captures every error/warning with timestamp, error code, session, user prompt, AI action and workspace into a dedicated log folder; instantly notifies the agent and ships a read_error_logs tool. |
| 267 | [173787247/dsh-tool-budget](https://github.com/173787247/dsh-tool-budget) | 1 | 2026-08-29 | 2026-08-29 | Hard-stop DeepSeek Harness tool use after a per-session call budget |
| 268 | [173787247/dsh-wsl-browser](https://github.com/173787247/dsh-wsl-browser) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: open http(s) URLs in the Windows default browser from WSL. |
| 269 | [173787247/dsh-wsl-clipboard](https://github.com/173787247/dsh-wsl-clipboard) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: read/write the Windows clipboard from WSL. |
| 270 | [173787247/dsh-wsl-cred](https://github.com/173787247/dsh-wsl-cred) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: safe Git credential hints for Windows GCM from WSL. |
| 271 | [173787247/dsh-wsl-distro](https://github.com/173787247/dsh-wsl-distro) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: current WSL distro facts and multi-distro warnings. |
| 272 | [173787247/dsh-wsl-github](https://github.com/173787247/dsh-wsl-github) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness: GitHub App status (open PRs + latest Actions) for WSL agents |
| 273 | [173787247/dsh-wsl-gpu](https://github.com/173787247/dsh-wsl-gpu) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: probe nvidia-smi / GPU visibility inside WSL. |
| 274 | [173787247/dsh-wsl-kit](https://github.com/173787247/dsh-wsl-kit) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness WSL kit (EN/ZH): docs + install.sh + cordis.patch for Windows browser + WSL agent plugins |
| 275 | [173787247/dsh-wsl-launch](https://github.com/173787247/dsh-wsl-launch) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: launch allowlisted Windows apps from WSL. |
| 276 | [173787247/dsh-wsl-notify](https://github.com/173787247/dsh-wsl-notify) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: Windows MessageBox notification from WSL. |
| 277 | [173787247/dsh-wsl-path](https://github.com/173787247/dsh-wsl-path) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: convert WSL Linux and Windows paths with /mnt/c caveats. |
| 278 | [173787247/dsh-wsl-port](https://github.com/173787247/dsh-wsl-port) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: diagnose WSL port listening and Windows localhost forwarding. |
| 279 | [17861102832/fleet-os](https://github.com/17861102832/fleet-os) | 1 | 2026-09-01 | 2026-09-01 | Fleet OS · 舰队模式 — 生产级多 Agent 协同引擎：WS 黑板 + 事件溯源 + 盲评对抗 + 跨舰队接力 + 上下文压缩 + 多厂商负载均衡 + 自进化。36 模块，零运行时依赖，MCP 40 工具，48 项 e2e 全绿。 |
| 280 | [240xu/verdict-engine](https://github.com/240xu/verdict-engine) | 1 | 2026-08-24 | 2026-08-27 | Verdict Engine — machine-checkable engineering governance: prose skill for any agent + dsh-themis DSH plugin (read-only tools, fail-closed, protocolJson negotiation). 纯文本规范 + 可校验运行时双载体。 |
| 281 | [2DogsLee/dsh_whalebuddy](https://github.com/2DogsLee/dsh_whalebuddy) | 1 | 2026-08-29 | 2026-08-29 | whalebuddy - DeepSeek Harness desktop pet (Windows): a DSH bundle plugin + Tauri shell. A porthole whale reflects your agent live state, with autostart & skin settings. |
| 282 | [33moren33/dsh-slice-bench](https://github.com/33moren33/dsh-slice-bench) | 1 | 2026-08-30 | 2026-08-30 | 把插件放进一台真起来的最小 DSH 机器，让 harness 自己说它站不站得住 · Runtime bench for DSH plugin version conflicts — the harness gives the verdict, not us |
| 283 | [452926826/dsh-feishu-bot](https://github.com/452926826/dsh-feishu-bot) | 1 | 2026-08-25 | 2026-08-27 | Connect a Feishu bot to DeepSeek Harness projects and conversations |
| 284 | [452926826/dsh-ssh-logs](https://github.com/452926826/dsh-ssh-logs) | 1 | 2026-08-25 | 2026-08-27 | Read allowlisted remote logs over SSH from DeepSeek Harness conversations |
| 285 | [abbccdd/dsh-localtts](https://github.com/abbccdd/dsh-localtts) | 1 | 2026-08-28 | 2026-08-29 | Local IndexTTS 2.5 and GPT-SoVITS speech synthesis and playback for DeepSeek Harness. |
| 286 | [Aik358/dsh-literature](https://github.com/Aik358/dsh-literature) | 1 | 2026-08-30 | 2026-09-01 | DSH Literature 文献侧窗插件：在 DeepSeek Harness 侧边栏识别 DOI/arXiv/标题、抓取元数据与全文、写入本地文献库或导出目录，内置 PDF 阅读器。 |
| 287 | [algerkong/dsh-image-preview](https://github.com/algerkong/dsh-image-preview) | 1 | 2026-08-27 | 2026-08-27 | Image preview for DSH (DeepSeek Harness) web sessions: read_image results render as a thumbnail, click for full size in the built-in lightbox. |
| 288 | [americanjeff/filestab](https://github.com/americanjeff/filestab) | 1 | 2026-08-31 | 2026-09-01 | Adds a file/vcs browser with diff and markdown preview support to the DeepSeek Harness · 为 DeepSeek Harness 添加文件 / VCS 浏览器，支持 diff 与 Markdown 预览。 |
| 289 | [amphilagus/dsh-gamer](https://github.com/amphilagus/dsh-gamer) | 1 | 2026-08-20 | 2026-08-28 | DSH bundle + 游戏玩家 preset: play on a dsh-gaming-platform instance. |
| 290 | [Ansonfishing/dsh-ca-ref](https://github.com/Ansonfishing/dsh-ca-ref) | 1 | 2026-08-28 | 2026-08-28 | Clean Architecture reference library for DSH: 8 pinned reference repos with FTS5 search, assertion rules, and a review ledger for architecture reviews |
| 291 | [arthur20150522/dsh-token-usage-cost](https://github.com/arthur20150522/dsh-token-usage-cost) | 1 | 2026-08-28 | 2026-08-28 | Shows per-turn and session token costs in DSH web conversations. |
| 292 | [Ary66101/dsh-desktop](https://github.com/Ary66101/dsh-desktop) | 1 | 2026-08-25 | 2026-08-27 | dsh的自制桌面端 |
| 293 | [Ary66101/dsh-instruction-bubble](https://github.com/Ary66101/dsh-instruction-bubble) | 1 | 2026-08-27 | 2026-08-27 | 你的上文语境小气泡 |
| 294 | [ashuai/dsh-s2s](https://github.com/ashuai/dsh-s2s) | 1 | 2026-08-31 | 2026-08-31 | Connect AI agent sessions on one machine — a DeepSeek Harness plugin for session-to-session collaboration, with lifecycle support to wake finished sessions and loop-safe messaging budgets. |
| 295 | [awnlight/talon-ui](https://github.com/awnlight/talon-ui) | 1 | 2026-08-28 | 2026-08-28 | A terminal UI for DeepSeek Harness (dsh) agents. |
| 296 | [better-er/dsh-peak-block](https://github.com/better-er/dsh-peak-block) | 1 | 2026-08-31 | 2026-08-31 | 梁文峰时间高峰自动拦截官方 DeepSeek 请求 |
| 297 | [better-er/dsh-write-create-only](https://github.com/better-er/dsh-write-create-only) | 1 | 2026-09-01 | 2026-09-02 | write 仅创建：禁止 write 覆盖已存在文件，目标已存在时自动拒绝并提示改用 edit，防止模型误覆写已有内容。纯 host 端 dsh 插件。 |
| 298 | [better-er/dsh-write-rule-guard](https://github.com/better-er/dsh-write-rule-guard) | 1 | 2026-09-02 | 2026-09-02 | dsh 插件：按可配置正则规则拦截 edit/write 的写入内容，默认拦全角括号，host 单半身经 cordis 配置注入。 |
| 299 | [big0lives/dsh-web-window-companion](https://github.com/big0lives/dsh-web-window-companion) | 1 | 2026-08-31 | 2026-08-31 | DSH Web 窗口伴侣插件：App 模式窗口打开 Web GUI，关窗即优雅停服。Close the window = stop the server. |
| 300 | [big0lives/dsh-win-quick-launcher](https://github.com/big0lives/dsh-win-quick-launcher) | 1 | 2026-08-31 | 2026-08-31 | DSH 的 Windows 便捷启动器：双击桌面图标启动 DeepSeek Harness Web，关掉浏览器窗口即停服务。支持源码安装与 npm 安装。 |
| 301 | [biliye/dsh-voice-call](https://github.com/biliye/dsh-voice-call) | 1 | 2026-08-16 | 2026-08-31 | 这是一个deepseek专属的语音通话插件 |
| 302 | [bingaha/dsh-live-mcp](https://github.com/bingaha/dsh-live-mcp) | 1 | 2026-08-19 | 2026-08-31 | 给DSH提供会话级的MCP控制能力 |
| 303 | [bjzkhy/dsh-token-ledger-pro](https://github.com/bjzkhy/dsh-token-ledger-pro) | 1 | 2026-08-30 | 2026-08-30 | DSH cost panel: meters every request from session events, prices it against a built-in catalog of 136 models across 16 providers, and shows model, balance, session/today/month spend and a monthly budget bar next to the composer. |
| 304 | [BlueChonk/dsh-balance-phoebe](https://github.com/BlueChonk/dsh-balance-phoebe) | 1 | 2026-08-28 | 2026-08-29 | 菲比啾比查 longcat token 余量挂件 |
| 305 | [bobjia/dsh-context-milvus](https://github.com/bobjia/dsh-context-milvus) | 1 | 2026-08-29 | 2026-08-29 | claude-context-milvus like plugin for Deepseek Harness (DSH)  |
| 306 | [Bobnemimimmi/dsh-always-status-bar](https://github.com/Bobnemimimmi/dsh-always-status-bar) | 1 | 2026-08-26 | 2026-08-27 | 始终显示消息下的 status bar，无需鼠标悬停 |
| 307 | [bruc3van/dsh-doctor](https://github.com/bruc3van/dsh-doctor) | 1 | 2026-08-29 | 2026-08-29 | 面向 Agent 的 DeepSeek Harness 插件升级与排障工具：分析版本差异、迁移代码、验证构建与运行，并诊断 profile、依赖和配置问题。 |
| 308 | [buchylx/create-dsh-content-plugin](https://github.com/buchylx/create-dsh-content-plugin) | 1 | 2026-08-26 | 2026-08-27 | Zero-dependency CLI that scaffolds a content-automation DSH plugin (Dev.to/GitHub/Bluesky/Mastodon). Like create-vite, for DSH. |
| 309 | [caopu16/dsh-local-memory](https://github.com/caopu16/dsh-local-memory) | 1 | 2026-08-27 | 2026-08-27 | DSH（DeepSeek Harness）本地跨会话记忆插件：捕获每轮对话摘要、注入最近几天记忆，并提供 memory_search 工具按需检索全部历史记忆。 |
| 310 | [Carrick-K7/dsh-plugin-source](https://github.com/Carrick-K7/dsh-plugin-source) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: group the Settings plugin list by origin (official/community), show version, upstream repo link and local-dev marker. Read-only, zero network. |
| 311 | [cat552/dsh-agent-quality-diagnosis](https://github.com/cat552/dsh-agent-quality-diagnosis) | 1 | 2026-09-01 | 2026-09-01 | Actionable quality diagnostics for DSH agent sessions, with tool-call evidence and next-step recommendations. |
| 312 | [cayan0x/Lume](https://github.com/cayan0x/Lume) | 1 | 2026-08-29 | 2026-08-31 | Lume - DSH Desktop persona-switching plugin (loli/senpai/none) with P0-P3 thinking logic |
| 313 | [ccll/dsh-activity-pane](https://github.com/ccll/dsh-activity-pane) | 1 | 2026-08-24 | 2026-08-29 | Activity session overview pane for DeepSeek Harness (DSH) web — running sessions, sub-agents, waiting-for-action reminders & recent history at a glance / DSH 活动会话总览窗格 |
| 314 | [Charlie-Wang-03/dsh-sightline](https://github.com/Charlie-Wang-03/dsh-sightline) | 1 | 2026-08-23 | 2026-08-27 | See the same repo through every agent's eyes — compare the effective instruction surfaces of DeepSeek Harness, Codex, and Claude Code. 查看同一仓库在 DeepSeek Harness、Codex 与 Claude Code 眼中的不同指令面。 |
| 315 | [chen731215-dev/dsh-muv-engine](https://github.com/chen731215-dev/dsh-muv-engine) | 1 | 2026-08-27 | 2026-08-27 | DSH Native MUV Engine - tavern companion: regex script execution, variable state tracking, iframe status bar rendering, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 316 | [chen731215-dev/dsh-muv-table](https://github.com/chen731215-dev/dsh-muv-table) | 1 | 2026-08-27 | 2026-08-27 | MUV Variable Table Editor - tavern companion plugin for DeepSeek Harness: structured table editing for UpdateVariable blocks, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 317 | [chendefine/dsh-sidebar-cdp-browser](https://github.com/chendefine/dsh-sidebar-cdp-browser) | 1 | 2026-08-19 | 2026-08-27 | deepseek harness live view chromium via cdp in sidebar tab |
| 318 | [cherrchen/dsh-theme-studio](https://github.com/cherrchen/dsh-theme-studio) | 1 | 2026-08-26 | 2026-08-27 | 可移植的 DSH/Cordis 主题插件：内置配色浏览、预览、应用与持久化；DeepSeek Harness Desktop 预装。 / Portable DSH/Cordis theme overlay plugin with builtin palettes, preview, apply, and persistence; pre-installed in DeepSeek Harness Desktop. |
| 319 | [chongyangdu2008-cyrus/dsh-subagent-inspector](https://github.com/chongyangdu2008-cyrus/dsh-subagent-inspector) | 1 | 2026-08-28 | 2026-08-28 | Read-only live subagent process inspector for DeepSeek Harness Web |
| 320 | [Cmjingahaha/dsh-dudulu](https://github.com/Cmjingahaha/dsh-dudulu) | 1 | 2026-08-27 | 2026-08-27 | 嘟一声 · DSH 任务完成提示音插件：Agent 回合完成时播放提示音，带设置面板（音量/试听/上传） |
| 321 | [CNSeniorious000/dsh-py-codeact](https://github.com/CNSeniorious000/dsh-py-codeact) | 1 | 2026-08-28 | 2026-08-28 | Python-based CodeAct for dsh with persistent state across cells, replacing Dynamic Workflows and code-mode |
| 322 | [Co1ombiagly/prompt_optimize_dsh](https://github.com/Co1ombiagly/prompt_optimize_dsh) | 1 | 2026-08-30 | 2026-08-31 | DeepSeek Harness (DSH) 提示词优化器插件：一句口语化需求 → 结构化高质量提示词，结果自动填入会话输入框。复用 DSH 内置模型路由，零 API Key 管理。 |
| 323 | [conafun/dsh-music-plus](https://github.com/conafun/dsh-music-plus) | 1 | 2026-08-29 | 2026-08-29 | 基于 dsh-music-player 的修改版：移除在线QQ/酷狗/讲书/歌词，新增播客 |
| 324 | [crack-time/dsh-archive](https://github.com/crack-time/dsh-archive) | 1 | 2026-08-15 | 2026-08-31 | Session archive plugin for DSH web GUI |
| 325 | [crazy-L118/dsh-desktop-notify](https://github.com/crazy-L118/dsh-desktop-notify) | 1 | 2026-08-25 | 2026-08-27 | Desktop notification plugin for dsh: get a native OS toast when the AI finishes its reply. Toggle lives in dsh Settings → General. |
| 326 | [crazy-L118/dsh-personalization](https://github.com/crazy-L118/dsh-personalization) | 1 | 2026-08-28 | 2026-09-02 | A personalization plugin for DeepSeek Harness |
| 327 | [CSI-entitymorton/stavros-dsh-redteamer](https://github.com/CSI-entitymorton/stavros-dsh-redteamer) | 1 | 2026-08-29 | 2026-08-29 | Authorized-only AI red-team / pentest plugin for the DeepSeek Harness (DSH). Fail-closed scope guard: Stavros persona, 24 specialist subagents, 78 zero-dependency tools. |
| 328 | [cxy9204/dsh-skill-store](https://github.com/cxy9204/dsh-skill-store) | 1 | 2026-09-02 | 2026-09-02 | DeepSeek Harness 社区技能商店：浏览、搜索并一键安装来自 SkillHub / ClawHub / GitHub 的 13 万+ Agent Skills，支持星标排序与中文分类 |
| 329 | [czj-git/dsh-plugin-hub](https://github.com/czj-git/dsh-plugin-hub) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness tools for searching and ranking verified plugins from DSH Plugin Hub |
| 330 | [D-Robotics/dsh-plugin-rdk](https://github.com/D-Robotics/dsh-plugin-rdk) | 1 | 2026-08-14 | 2026-08-28 | D-Robotics RDK (地瓜机器人) integration for DeepSeek Harness — native RDK skill catalog, rdk_skills browser tool, and rdk_board_detect device detection |
| 331 | [D2Moqi/dsh-openwiki](https://github.com/D2Moqi/dsh-openwiki) | 1 | 2026-08-29 | 2026-08-29 | DSH 插件：把 openwiki 的代码库知识库能力搬进 DeepSeek Harness —— 一键生成 / 阅读 / 更新仓库 Wiki 与 Grounded Claims（溯源知识卡片），直接复用 DSH 已配置的模型，无需二次填 Key。 |
| 332 | [d3vmeh/dsh-fetch-timeouts](https://github.com/d3vmeh/dsh-fetch-timeouts) | 1 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: raise Node's HTTP timeouts process-wide so slow local models (Ollama, LM Studio) are not cut off at 5 minutes |
| 333 | [d3vmeh/dsh-llm-gate](https://github.com/d3vmeh/dsh-llm-gate) | 1 | 2026-08-29 | 2026-08-29 | Per-provider concurrency gate for DeepSeek Harness model requests |
| 334 | [DahliaVoid/dsh-temp-session](https://github.com/DahliaVoid/dsh-temp-session) | 1 | 2026-08-28 | 2026-08-28 | dsh工作区可选化，100%纯AI coding产物 |
| 335 | [daishengli/dsh-docker](https://github.com/daishengli/dsh-docker) | 1 | 2026-08-27 | 2026-08-28 | 使用 Docker 封装运行 deepseek-harness d的 Web 服务。容器内运行 dsh 和 Caddy，宿主机通过 3080 端口访问服务。 |
| 336 | [daodishisha28/dsh-sidechat-plugin](https://github.com/daodishisha28/dsh-sidechat-plugin) | 1 | 2026-08-30 | 2026-08-31 | Open a persistent side conversation from any DeepSeek Harness session to investigate questions, clarify requirements, or explore alternatives without polluting the main task’s context, then review and send a concise conclusion back to the parent conversation. Tested with DSH 0.1.2-alpha.1. |
| 337 | [dat-lequoc/dsh-opinionated-subagent](https://github.com/dat-lequoc/dsh-opinionated-subagent) | 1 | 2026-08-27 | 2026-08-28 | A minimal, opinionated subagent for DeepSeek Harness: you choose which models a child may run on and at which reasoning effort, and a correction reaches a working child at its next step |
| 338 | [DaYanQLQ/DSH-Balance-Mini](https://github.com/DaYanQLQ/DSH-Balance-Mini) | 1 | 2026-09-01 | 2026-09-02 | DeepSeek Harness 的极简版余额监视器插件：常驻余额徽章、红绿灯配色、多供应商、高峰/空闲时段。 |
| 339 | [DaYanQLQ/DSH-Shortcut](https://github.com/DaYanQLQ/DSH-Shortcut) | 1 | 2026-09-01 | 2026-09-02 | DeepSeek Harness 的 Windows 桌面快捷方式工具：双击智能启动/唤起、浏览器打开前自动最小化、崩溃一键重装救援（不删用户数据）。圆角官方图标，纯 PowerShell 零依赖。 |
| 340 | [DaydreAmRing/dsh-cho-kaguya-plugin-public](https://github.com/DaydreAmRing/dsh-cho-kaguya-plugin-public) | 1 | 2026-09-02 | 2026-09-02 | DSH皮肤插件、有超时空辉夜姬概念元素 |
| 341 | [DDDFXYqiming/dsh-session-recap](https://github.com/DDDFXYqiming/dsh-session-recap) | 1 | 2026-08-28 | 2026-08-28 | Session recap plugin for DeepSeek Harness (Claude Code-style away summaries) |
| 342 | [ddtcorex/dsh-maestro-ci](https://github.com/ddtcorex/dsh-maestro-ci) | 1 | 2026-08-26 | 2026-08-28 | Reusable GitHub Actions workflows for the Maestro suite — Cordis / DSH |
| 343 | [ddtcorex/dsh-maestro-config-lib](https://github.com/ddtcorex/dsh-maestro-config-lib) | 1 | 2026-08-25 | 2026-08-28 | Maestro settings store library — atomic namespaced JSON store shared by dsh-maestro-* plugins (embedded dependency, no Cordis row) |
| 344 | [ddtcorex/dsh-maestro-dashboard](https://github.com/ddtcorex/dsh-maestro-dashboard) | 1 | 2026-08-28 | 2026-08-28 | Maestro Dashboard — unified Control Center (Overview/Plugins/Usage) DSH-native |
| 345 | [ddtcorex/dsh-maestro-devkit](https://github.com/ddtcorex/dsh-maestro-devkit) | 1 | 2026-08-27 | 2026-08-28 | General development toolkit for DeepSeek Harness — visual review, HMR, style inspector, Cordis/Govard/Skills dev (tunnel-aware) |
| 346 | [ddtcorex/dsh-maestro-diagram](https://github.com/ddtcorex/dsh-maestro-diagram) | 1 | 2026-08-27 | 2026-08-28 | DSH Maestro diagram studio — mermaid_verify + mermaid_drift |
| 347 | [ddtcorex/dsh-maestro-supervisor](https://github.com/ddtcorex/dsh-maestro-supervisor) | 1 | 2026-08-27 | 2026-08-28 | Supervisor daemon for DSH Web resilience — auto-detect crashes, rollback to LKG, report |
| 348 | [ddtcorex/dsh-maestro-sync](https://github.com/ddtcorex/dsh-maestro-sync) | 1 | 2026-08-30 | 2026-09-01 | Maestro harness sync — merge memories and sessions across machines (publishable) |
| 349 | [difimim/dsh-voice-input-npm](https://github.com/difimim/dsh-voice-input-npm) | 1 | 2026-08-30 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 350 | [dingyi580/dsh-plugin-gemini-theme](https://github.com/dingyi580/dsh-plugin-gemini-theme) | 1 | 2026-08-29 | 2026-08-30 | A Gemini-styled skin for the DeepSeek Harness web client |
| 351 | [DjangoAILab/dsh-plugins](https://github.com/DjangoAILab/dsh-plugins) | 1 | 2026-08-18 | 2026-09-01 | DeepSeek Harness plugins for browser automation, macOS computer use, external subagents, and guarded SSH operations. |
| 352 | [domitor-syh/dsh-ui-skin-switcher](https://github.com/domitor-syh/dsh-ui-skin-switcher) | 1 | 2026-08-27 | 2026-08-28 | Model & reasoning-effort switcher plugin for DeepSeek Harness (DSH): composer seat with Off/Max effort slider. DSH 插件：模型与思考力度切换器。 |
| 353 | [doublehappy123/dsh-v4flash-tiler](https://github.com/doublehappy123/dsh-v4flash-tiler) | 1 | 2026-09-01 | 2026-09-01 | DSH plugin: auto-tiles oversized chat images into labelled grid tiles for DeepSeek v4Flash vision, with Python tiling engine |
| 354 | [doublemolu/dsh-costometer](https://github.com/doublemolu/dsh-costometer) | 1 | 2026-08-28 | 2026-09-01 | 花知多少 · Cost-O-Meter — DeepSeek Harness cost & balance meter: account balance, recharge history, per-conversation spend & tokens, 50-yuan segmented progress bar, low-balance guard, 8 languages & currencies with auto FX rates (CNY base). |
| 355 | [drscrewdriver/dsh-llm-openai-completions](https://github.com/drscrewdriver/dsh-llm-openai-completions) | 1 | 2026-08-29 | 2026-08-29 | dsh-llm-openai-completions |
| 356 | [duhu2000/dsh-data-cleaning-agent](https://github.com/duhu2000/dsh-data-cleaning-agent) | 1 | 2026-09-01 | 2026-09-01 | Data cleaning and enterprise enrichment agent plugin for DeepSeek Harness. |
| 357 | [dusbin/dsh-multi-tenant](https://github.com/dusbin/dsh-multi-tenant) | 1 | 2026-08-29 | 2026-08-29 | dsh 支持多租户插件 |
| 358 | [EastMG/dsh-gacha-calendar](https://github.com/EastMG/dsh-gacha-calendar) | 1 | 2026-08-27 | 2026-08-30 | DeepSeek Harness 二游卡池/活动排期速查插件：侧边栏按钮 内置 11 款主流二游 可添加自定义游戏 |
| 359 | [Edge-Echo/dsh-netassist](https://github.com/Edge-Echo/dsh-netassist) | 1 | 2026-08-30 | 2026-08-30 | Network & proxy assistant for DeepSeek Harness (dsh): one-shot GitHub connectivity check, system proxy status, proxy port probing, full diag chain and hosts conflict scan. |
| 360 | [Edge-Echo/dsh-win-toolkit](https://github.com/Edge-Echo/dsh-win-toolkit) | 1 | 2026-08-30 | 2026-08-30 | Windows-native capability pack for DeepSeek Harness (dsh): clipboard, notifications, hosts file, network diagnostics — safe PowerShell-backed tools. |
| 361 | [Elpsycoogroo/dsh-work-report](https://github.com/Elpsycoogroo/dsh-work-report) | 1 | 2026-08-28 | 2026-08-28 | Neural Ledger - turn DSH collaboration sessions into a visual work ledger: token analytics, smart insights, trend forecasting, and one-click daily/weekly/monthly Markdown reports. |
| 362 | [Entaum/dsh-free-games](https://github.com/Entaum/dsh-free-games) | 1 | 2026-08-30 | 2026-08-31 | Deepseek Harness free games plugin. Play while coding! |
| 363 | [EternalNight996/memory-eternal](https://github.com/EternalNight996/memory-eternal) | 1 | 2026-08-31 | 2026-08-31 | 记忆核心（Memory Eternal）：自研的 DeepSeek Harness 记忆插件——对话结束自动沉淀知识卡到本地 Markdown Vault（自研去重 / 自研 CJK 检索 / 知识图谱 + 审核中心 / 回收中心），Agent 通过 memory_recall 按需召回历史上下文，零人工干预。 |
| 364 | [exoticknight/dsh-theme-eink-retro](https://github.com/exoticknight/dsh-theme-eink-retro) | 1 | 2026-08-26 | 2026-08-27 | A paper-and-ink client-side theme for DeepSeek Harness with Balanced and Immersive modes. |
| 365 | [f1yan9/dsh-balance-pie](https://github.com/f1yan9/dsh-balance-pie) | 1 | 2026-08-30 | 2026-08-30 | DSH 插件：可拖拽余额饼图 / 真实消耗 / 历史热力图 — balance pie with real spending & monthly heatmap for DeepSeek Harness. |
| 366 | [falling-ts/dsh-web-ding](https://github.com/falling-ts/dsh-web-ding) | 1 | 2026-08-27 | 2026-08-27 | Browser-only 'ding' on agent end; works on servers.浏览器专属"叮":回合结束时响起,服务器部署也生效 |
| 367 | [fallow5/dsh-pin-sessions](https://github.com/fallow5/dsh-pin-sessions) | 1 | 2026-08-28 | 2026-08-31 | DSH (DeepSeek Harness) web plugin: pin sessions to the top of the sidebar for quick access to recurring workflows. Includes archive panel with batch delete, restore, and workspace grouping. |
| 368 | [fan56/dsh-model-sync](https://github.com/fan56/dsh-model-sync) | 1 | 2026-08-28 | 2026-08-29 | A dsh (DeepSeek Harness) Cordis plugin that keeps llm-pi-ai provider routes' model catalog in sync with the pi.dev gateway — written through the official settings seam, zero patches to dsh internals. |
| 369 | [fan56/dsh-subagent-registry](https://github.com/fan56/dsh-subagent-registry) | 1 | 2026-08-16 | 2026-08-28 | dsh plugin: register ~/.dsh/agents/*.md as dsh-callable subagents |
| 370 | [FanetheDivine/dsh-plugin-om](https://github.com/FanetheDivine/dsh-plugin-om) | 1 | 2026-08-15 | 2026-08-27 | DSH插件，以Observational Memory方式管理上下文 |
| 371 | [fengb3/dsh-theme-aurum](https://github.com/fengb3/dsh-theme-aurum) | 1 | 2026-08-24 | 2026-08-28 | DSH 鎏金主题插件:金粉奢华皮肤,htm 恒等映射流水,原型驱动的逐节移植 |
| 372 | [FlameTN7/dsh-tui-browser-use](https://github.com/FlameTN7/dsh-tui-browser-use) | 1 | 2026-08-25 | 2026-08-31 | Browser automation bridge sub-plugin for dsh-tui.                    dsh-tui的浏览器自动化子插件 |
| 373 | [focksor/dsh-plugin-mini-dashboard](https://github.com/focksor/dsh-plugin-mini-dashboard) | 1 | 2026-08-28 | 2026-08-28 | A session & token mini dashboard for DSH web. It renders just above the sidebar's "Settings" row and summarizes, in one small draggable float window, what your sessions are doing right now and what they have cost you today. |
| 374 | [focksor/dsh-plugin-node-time](https://github.com/focksor/dsh-plugin-node-time) | 1 | 2026-08-29 | 2026-08-31 | Hover timestamps for DSH web. Hovering a chat node row — Think, Bash, Read/Edit/Write, Search, commands, compaction markers, sub-calls — pops a compact card with that node's start time → end time and how long it took. |
| 375 | [focksor/dsh-plugin-thinking-size](https://github.com/focksor/dsh-plugin-thinking-size) | 1 | 2026-08-28 | 2026-08-28 | A live reasoning-token badge for DSH web. It appends a compact Think(128) / Think(5.2K) marker to the title of every "Think" disclosure row in the conversation — ticking in real time while the model is still thinking, and staying put on history messages afterwards. |
| 376 | [FomoGoMan/dsh-serena-guide](https://github.com/FomoGoMan/dsh-serena-guide) | 1 | 2026-09-02 | 2026-09-02 | A DeepSeek Harness plugin that steers agents to Serena's LSP symbolic tools over built-in code tools. |
| 377 | [frank-fan-818/dsh-f1-skin](https://github.com/frank-fan-818/dsh-f1-skin) | 1 | 2026-09-01 | 2026-09-02 | An F1 Race Control themed skin for the DeepSeek Harness Web UI — Red Bull, Ferrari, McLaren & Mercedes team themes, broadcast-photo backdrops, and a native settings panel, in dark and light. |
| 378 | [FranklinZaneDurant/agent-discipline](https://github.com/FranklinZaneDurant/agent-discipline) | 1 | 2026-08-27 | 2026-08-27 | 给 AI 编码 Agent 的仓库工作纪律插件（DeepSeek Harness bundle）：方法论提示段 + 工件脚手架（AGENTS.md/特性清单/验证门）+ 合规审计。 |
| 379 | [fufengyuan/dsh-council](https://github.com/fufengyuan/dsh-council) | 1 | 2026-08-26 | 2026-08-27 | dsh-council — 高智议会（Council of High Intelligence）for DeepSeek Harness 在 dsh（DeepSeek Harness）里召集历史人物议会，对复杂问题进行多视角结构化辩论，最终由主席综合裁决。 |
| 380 | [g-yixuan/dsh-sidenote](https://github.com/g-yixuan/dsh-sidenote) | 1 | 2026-08-19 | 2026-08-28 | Codex-style side chat & selection annotations for DeepSeek Harness (DSH) web — fork the session into a persistent side panel; quote selections into context. Thin consumer of dsh-better-sidebar. |
| 381 | [GalaxyBatMan111/dsh-plugins](https://github.com/GalaxyBatMan111/dsh-plugins) | 1 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) plugins: agent bridge (Claude Code/Codex/Marvis) + Ghidra reverse engineering bridge |
| 382 | [gbeta/dsh-token-speed](https://github.com/gbeta/dsh-token-speed) | 1 | 2026-09-02 | 2026-09-02 | DSH web plugin: draggable ring gauge showing live model output speed (tok/s) with per-step detail panel |
| 383 | [gengwg/dsh-kubectl-guard](https://github.com/gengwg/dsh-kubectl-guard) | 1 | 2026-09-01 | 2026-09-01 | A dsh policy plugin that gates kubectl by kubeconfig context: deny irreversible verbs outside local clusters, ask for the rest. |
| 384 | [georesearch-dsh/georesearch-dsh](https://github.com/georesearch-dsh/georesearch-dsh) | 1 | 2026-08-27 | 2026-08-28 | GeoResearch agent plugin for DeepSeek Harness |
| 385 | [Georgehaoren/DSH-WhaleConsole](https://github.com/Georgehaoren/DSH-WhaleConsole) | 1 | 2026-08-29 | 2026-08-29 | Unofficial macOS desktop companion and WebUI skin plugin for DeepSeek Harness. 面向 DeepSeek Harness 的非官方 macOS 桌面伴侣与 WebUI 换肤插件。 |
| 386 | [goldgish/dsh-agent-trace](https://github.com/goldgish/dsh-agent-trace) | 1 | 2026-08-26 | 2026-08-27 | Agent Trace — visualize an agent's reasoning, parallel tool calls, and results as an interactive DAG inside DeepSeek Harness. |
| 387 | [GooDAnDReaDY/dsh-messenger-gateway](https://github.com/GooDAnDReaDY/dsh-messenger-gateway) | 1 | 2026-08-26 | 2026-08-27 | Telegram messenger bridge for DeepSeek Harness: sessions, steer, homes, and TTS voice notes |
| 388 | [GuionAI/web](https://github.com/GuionAI/web) | 1 | 2026-08-22 | 2026-08-30 | A web research toolkit with multi-provider search and clean Markdown extraction from static and JavaScript-rendered pages, plus public code and library docs search—available via CLI and MCP. |
| 389 | [gychen-NJU/dsh-overleaf](https://github.com/gychen-NJU/dsh-overleaf) | 1 | 2026-08-27 | 2026-08-29 | Embedded Overleaf workbench tab for DeepSeek Harness Web: same-origin reverse proxy, direct-CDP login, selection quoting, caret insertion, LaTeX assist panel |
| 390 | [hakimedes/dsh-easyremote](https://github.com/hakimedes/dsh-easyremote) | 1 | 2026-08-25 | 2026-09-01 | Local-first Android remote workspace with one-command Cloudflare Tunnel setup |
| 391 | [hanrr92/dsh-code-quote](https://github.com/hanrr92/dsh-code-quote) | 1 | 2026-09-01 | 2026-09-01 | 代码引用 |
| 392 | [hejielijob-commits/SemaRail](https://github.com/hejielijob-commits/SemaRail) | 1 | 2026-08-17 | 2026-08-30 | Governed semantic layer for AI agents, with a DeepSeek Harness plugin that turns Harness into a data agent. |
| 393 | [henrychenhao/dsh-skin-argentina](https://github.com/henrychenhao/dsh-skin-argentina) | 1 | 2026-08-27 | 2026-08-27 | 梅西 阿根廷皮肤 |
| 394 | [HenryPhoebe/dsh-plugin-easyppt](https://github.com/HenryPhoebe/dsh-plugin-easyppt) | 1 | 2026-08-27 | 2026-08-27 | easyppt是一个面向 DeepSeek Harness (DSH) 的演示文稿生成 dsh-plugin（npm 包 + Cordis bundle + 内置技能）。用户输入大纲（Markdown / JSON / 自然语言）与插图，即可基于 DSH 原生 Univer 工具链生成PPTX,HTML,JSON |
| 395 | [hgl011091/dsh-rss-monitor](https://github.com/hgl011091/dsh-rss-monitor) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 原生 RSS 订阅监控插件：多源订阅、关键词过滤、定时检查去重、新条目邮件通知（缩略图 HTML 模板），SMTP 密码走凭据库永不落盘，原生设置页四页签体验。 |
| 396 | [hjj345/dsh-sm-context-piano](https://github.com/hjj345/dsh-sm-context-piano) | 1 | 2026-08-21 | 2026-08-29 | DeepSeek Harness Web GUI 的 Codex 风格对话导航器：帮助用户快速浏览、定位和切换对话，提升多任务、多会话场景下的工作效率。 \|  Codex-style conversation navigator for the DeepSeek Harness Web GUI. |
| 397 | [hjj345/dsh-sm-version-display](https://github.com/hjj345/dsh-sm-version-display) | 1 | 2026-08-28 | 2026-08-30 | 用于在侧边栏“设置”按钮上方显示已安装 dsh 版本的 DeepSeek Harness Web 插件。  \|  DeepSeek Harness Web plugin that displays the installed dsh version above the sidebar Settings button. |
| 398 | [hotpot-labs/dsh-version-plugin](https://github.com/hotpot-labs/dsh-version-plugin) | 1 | 2026-08-28 | 2026-09-02 | 展示dsh版本，提供更新到最新版按钮 |
| 399 | [HOWILLMAKEIT/dsh-model-context-catalog](https://github.com/HOWILLMAKEIT/dsh-model-context-catalog) | 1 | 2026-09-01 | 2026-09-01 | DeepSeek Harness 插件：维护 llm-pi-ai 模型的准确上下文窗口，避免长会话被误判为上下文溢出。 |
| 400 | [hoyyang/dsh-concise](https://github.com/hoyyang/dsh-concise) | 1 | 2026-09-02 | 2026-09-02 | One-click Concise output style for DeepSeek Harness: results first, no filler — Claude Code's built-in Concise style as a dsh plugin. Toggle right of the model picker, global, persistent, zero-config. |
| 401 | [HuanLinOTO/dsh-plugin-better-glob](https://github.com/HuanLinOTO/dsh-plugin-better-glob) | 1 | 2026-08-30 | 2026-08-30 | 以 per-agent 阴影顶替内置 glob：自动排除无底洞目录（node_modules 等），传 include 白名单才能搜入 \| Shadows the built-in glob per agent: auto-excludes bottomless directories (node_modules etc.), pass an include whitelist to search inside them |
| 402 | [huhaodong/dsh-auto-driving](https://github.com/huhaodong/dsh-auto-driving) | 1 | 2026-09-02 | 2026-09-02 | 让 DeepSeek Harness 智能体进入自动驾驶 🚗：模型故障自动回退、静默卡死自动保活重试、权限/提问/方案审批自动放行，AUTO-MODE.md 全程审计——无人值守、永不停摆的自愈式 AI 编码会话。 |
| 403 | [iasiv5/skins](https://github.com/iasiv5/skins) | 1 | 2026-08-28 | 2026-08-28 | 一键入戏，一键归真 —— 壁纸 · 标语 · 通透度，即改即存；明暗双态、中英双语，SHA 校验自动更新。Make every skin your own — hot-swappable, fully personalizable skins for DeepSeek Harness Web. |
| 404 | [Idreamxkl/dsh-conversation-flat](https://github.com/Idreamxkl/dsh-conversation-flat) | 1 | 2026-08-30 | 2026-08-30 | Document-flow conversation layout for DeepSeek Harness web GUI — full-width column, user message bars, sender label, full-width tables. 纯 CSS 的 dsh 对话区通栏布局插件 |
| 405 | [iimaguest/dsh-contradictions-indicator](https://github.com/iimaguest/dsh-contradictions-indicator) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin: 0-100 conversation coherence badge with parallel contradiction analysis |
| 406 | [jarvis959/galvanize-dsh](https://github.com/jarvis959/galvanize-dsh) | 1 | 2026-08-28 | 2026-08-28 | Triggers inside your DSH agent: wake a fresh DeepSeek Harness session when files, mail, webhooks, or git events happen. Native Cordis bundle, heartbeat-proved install. |
| 407 | [JasonFreeLab/dsh-superpowers](https://github.com/JasonFreeLab/dsh-superpowers) | 1 | 2026-08-28 | 2026-08-28 | DSH (DeepSeek Harness) port of obra/superpowers — 14 native skills for multi-agent software development: brainstorming, planning, TDD, systematic debugging, and code review. |
| 408 | [jeffy-Peng/deepseek-harness-usage](https://github.com/jeffy-Peng/deepseek-harness-usage) | 1 | 2026-08-16 | 2026-08-28 | DeepSeek Harness 插件，显示每日消费与账户总余额。DeepSeek Harness plugin for account balance and evidence-bounded daily CNY consumption |
| 409 | [Jensen-Yao/dsh-model-palette](https://github.com/Jensen-Yao/dsh-model-palette) | 1 | 2026-08-26 | 2026-08-27 | Global provider-aware model command palette and optional OpenRouter media tools for DeepSeek Harness. |
| 410 | [JerryXst/dsh-codex-web-auth](https://github.com/JerryXst/dsh-codex-web-auth) | 1 | 2026-09-01 | 2026-09-02 | ChatGPT / Codex browser sign-in for DeepSeek Harness's built-in openai-codex provider — no OpenAI API key required. |
| 411 | [jetheaven/dsh-code-reviewer](https://github.com/jetheaven/dsh-code-reviewer) | 1 | 2026-08-14 | 2026-08-27 | AI代码审查插件：bug检测/安全漏洞/性能/风格四维审查，行号定位+修复示例 |
| 412 | [jetheaven/dsh-content-rewriter](https://github.com/jetheaven/dsh-content-rewriter) | 1 | 2026-08-14 | 2026-08-27 | 一键内容改写：小红书/知乎/商务邮件/精简/扩写/Twitter 多风格 |
| 413 | [jetheaven/dsh-data-extractor](https://github.com/jetheaven/dsh-data-extractor) | 1 | 2026-08-14 | 2026-08-27 | 结构化数据提取：从非结构化文本提取字段，输出 JSON/CSV/表格 |
| 414 | [jetheaven/dsh-meeting-notes](https://github.com/jetheaven/dsh-meeting-notes) | 1 | 2026-08-14 | 2026-08-27 | 会议纪要智能生成：从转写文本提取决议/待办/负责人/截止时间/风险 |
| 415 | [jetheaven/dsh-prompt-optimizer](https://github.com/jetheaven/dsh-prompt-optimizer) | 1 | 2026-08-14 | 2026-08-27 | AI提示词优化器：诊断Prompt问题并输出结构化高质量优化版本 |
| 416 | [jetheaven/dsh-seo-writer](https://github.com/jetheaven/dsh-seo-writer) | 1 | 2026-08-14 | 2026-08-27 | SEO文章生成器：给定关键词和语言，生成搜索引擎友好的完整文章 |
| 417 | [jetheaven/dsh-text-diff](https://github.com/jetheaven/dsh-text-diff) | 1 | 2026-08-14 | 2026-08-27 | AI智能文本对比：找出两段文字的差异、语义变化和潜在风险点 |
| 418 | [jetheaven/dsh-translate-pro](https://github.com/jetheaven/dsh-translate-pro) | 1 | 2026-08-14 | 2026-08-27 | 专业翻译：术语一致、专业领域选择与语气调整，附带术语对照表 |
| 419 | [jiangliuhong/dsh-gpt-oauth](https://github.com/jiangliuhong/dsh-gpt-oauth) | 1 | 2026-08-26 | 2026-08-27 | openai models for login by chatgpt |
| 420 | [JianwuYang/dsh-ui-kanban](https://github.com/JianwuYang/dsh-ui-kanban) | 1 | 2026-08-27 | 2026-08-27 | 让 agent 直接干 Jira/GitLab 的活 · DSH 看板插件 \| A dsh plugin that turns Jira + GitLab into an agent-workable kanban board |
| 421 | [jianxx/dsh-cc](https://github.com/jianxx/dsh-cc) | 1 | 2026-08-15 | 2026-08-28 | Bring the Claude Code workflow to DeepSeek Harness - TUI, permissions, hooks, memory, skills, subagents, MCP, worktrees, and more. |
| 422 | [jing-hy/computer-user](https://github.com/jing-hy/computer-user) | 1 | 2026-08-21 | 2026-08-27 | DSH plugin: Codex-style computer use for Windows - read the screen, drive mouse & keyboard via SendInput; pairs with picturereader to close the look-act-verify loop. |
| 423 | [jkStars/dsh-token-usage-stats](https://github.com/jkStars/dsh-token-usage-stats) | 1 | 2026-08-22 | 2026-09-01 | DSH plugin: cross-session token usage analytics with a web dashboard (ctx.tokenUsageStats) |
| 424 | [jn18755/dsh-skill-nannan](https://github.com/jn18755/dsh-skill-nannan) | 1 | 2026-08-27 | 2026-08-27 | DSH 插件：基于《地狱磨砺》(Hell Grind) 方法论的 AI 视频提示词规范（29 条规则，已去除压力测试阶段） |
| 425 | [Jonah-Wu23/dsh-gungnir](https://github.com/Jonah-Wu23/dsh-gungnir) | 1 | 2026-09-01 | 2026-09-01 | Lock the goal. Adapt the loop. Prove the hit. |
| 426 | [Jstn-1g/dsh-live-voice](https://github.com/Jstn-1g/dsh-live-voice) | 1 | 2026-08-25 | 2026-08-28 | DSH Live Voice: consent-bound one-turn voice for DeepSeek Harness, with a credential-free local synthetic demo, exact-Session isolation, and explicit draft handoff. |
| 427 | [junwei529/work-charter-dsh](https://github.com/junwei529/work-charter-dsh) | 1 | 2026-08-28 | 2026-08-30 | DSH-native Work Charter policy plugin backed by session-coordinator-dsh |
| 428 | [jypjypjypjyp/dsh-notifier](https://github.com/jypjypjypjyp/dsh-notifier) | 1 | 2026-08-27 | 2026-08-27 | 审批/完成/错误事件通知：浏览器 Notification + 系统原生 toast（Windows PowerShell WinRT / macOS osascript / Linux notify-send，均无需额外安装）；提示音可配、每条通知独立显示不互相替换、非安全上下文自动降级横幅 |
| 429 | [Kaiji-Z/dsh-plugin-stardeck](https://github.com/Kaiji-Z/dsh-plugin-stardeck) | 1 | 2026-08-30 | 2026-09-01 | RTS-style multi-agent orchestration board for DeepSeek Harness: issue plain-language strategic orders, a staff agent drafts acceptance-checked task orders, commander agents deploy typed subagent troops on isolated workspaces — with a 3D starfield campaign view, append-only event logs, and machine-checked verification. |
| 430 | [KannaKuron/dsh-agent-lang](https://github.com/KannaKuron/dsh-agent-lang) | 1 | 2026-08-31 | 2026-08-31 | Agent language control: DSH plugin — tool-call descriptions, model thinking, and replies each follow the GUI language, force a fixed language, or turn off; injected as one global runtime-context directive. \| Agent 语言控制:DSH 插件——工具描述、模型思考、回复输出三通道各自跟随界面语言 / 强制指定 / 关闭,以全局 runtime-context 注入,不改任何 preset。 |
| 431 | [keman-ai/dsh-opencode-zen](https://github.com/keman-ai/dsh-opencode-zen) | 1 | 2026-08-19 | 2026-08-27 | Bring OpenCode Zen's free models to DeepSeek Harness — zero config, no API key, catalog discovered live from upstream |
| 432 | [keman-ai/dsh-pocket](https://github.com/keman-ai/dsh-pocket) | 1 | 2026-09-02 | 2026-09-02 | Watch and steer your DSH agent from a phone browser: approve tool calls, send a message, stop a turn |
| 433 | [kenny2077/dsh-web-search-doubao](https://github.com/kenny2077/dsh-web-search-doubao) | 1 | 2026-08-29 | 2026-08-29 | Doubao Search provider for the DeepSeek Harness |
| 434 | [kenny2077/dsh-web-search-zai](https://github.com/kenny2077/dsh-web-search-zai) | 1 | 2026-08-28 | 2026-08-28 | One ZAI_API_KEY for both chat and search — plug-and-play Z.ai (GLM) web search for the DeepSeek Harness. |
| 435 | [KevinZhangNothing/dsh-task-graph](https://github.com/KevinZhangNothing/dsh-task-graph) | 1 | 2026-08-27 | 2026-08-27 | Task flow / execution graph plugin for DeepSeek Harness (DSH) — visualize a single task's full run: agents, tools, skills, subtasks, retries, live status. DSH 单任务执行流程图谱插件。 |
| 436 | [KhalilHsu/dsh-plugins](https://github.com/KhalilHsu/dsh-plugins) | 1 | 2026-08-17 | 2026-08-28 | Enhance DeepSeek Harness Web GUI with smart per-turn reasoning/tool folding and query navigation. |
| 437 | [kiligzzz/dsh-agent-dispatch](https://github.com/kiligzzz/dsh-agent-dispatch) | 1 | 2026-08-28 | 2026-08-28 | DSH 插件：预置专家 agent + 自动路由 + 小队编排。原生右 tab「Agent 调度」+ 悬浮活动球 +  触发器。 |
| 438 | [l-vM2k/dsh-ayaka-theme](https://github.com/l-vM2k/dsh-ayaka-theme) | 1 | 2026-08-28 | 2026-08-28 | deepseek harness plugins dsh-ayaka-theme |
| 439 | [LamplitIsles/dsh-companion](https://github.com/LamplitIsles/dsh-companion) | 1 | 2026-08-30 | 2026-08-30 | dsh as companion ai frontend in Svelte |
| 440 | [LamplitIsles/kepos-imagegen](https://github.com/LamplitIsles/kepos-imagegen) | 1 | 2026-08-27 | 2026-08-30 | Image generation tools via kepos exposed codex endpoint |
| 441 | [lewes2/archpresent](https://github.com/lewes2/archpresent) | 1 | 2026-08-29 | 2026-08-29 | Agent skill: generate beautiful dark-themed architecture diagrams from your project/demo/idea. Interactive, verifiable, and editable. Delivered as self-contained HTML. |
| 442 | [lgquan/dsh-voco](https://github.com/lgquan/dsh-voco) | 1 | 2026-08-27 | 2026-08-27 | Persistent voice conversations for DSH with cloud speech recognition, Edge TTS, and background Agent delegation. |
| 443 | [lhh010/dsh-file-trace](https://github.com/lhh010/dsh-file-trace) | 1 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 444 | [LHKong7/dsh-browser-runtime](https://github.com/LHKong7/dsh-browser-runtime) | 1 | 2026-08-26 | 2026-08-27 | deepseek harness plugin browser runtime |
| 445 | [liiiubai/dsh-mcp-bridge](https://github.com/liiiubai/dsh-mcp-bridge) | 1 | 2026-08-28 | 2026-08-28 | Expose DeepSeek Harness tools as a standard MCP server (streamable HTTP) — drive dsh from Claude Code, Codex, or any MCP client |
| 446 | [LiLiLi-Zi/dsh-gray-test](https://github.com/LiLiLi-Zi/dsh-gray-test) | 1 | 2026-09-02 | 2026-09-02 | dsh gray-model detection plugin — launch N concurrent sessions, stream reasoning chains, auto-classify gray models (I'm+ing > Let me×5), normal models (Let me≥3), and abnormal models (no features). Supports standard/PTC/minimal/cordis presets. |
| 447 | [linfengyu94/dsh-balance-panel](https://github.com/linfengyu94/dsh-balance-panel) | 1 | 2026-09-01 | 2026-09-01 | DeepSeek 充值余额悬浮面板 - DSH 插件：悬浮显示充值余额，带可视化进度条与动态按钮动画 |
| 448 | [LLYlab/DSHEssentialTools](https://github.com/LLYlab/DSHEssentialTools) | 1 | 2026-08-27 | 2026-08-28 | DSH 永久插件：LVAL 工程运行/代码查看/程序版本快照回退 + VTD 虚拟对话树（编辑/重试/分支、消息小版本）+ DET 管理器。A permanent DeepSeek Harness plugin: project run & code viewer, program snapshots, an in-session conversation tree (edit/retry/branches), message micro-versions and a feature manager. |
| 449 | [LoKiGGo/dsh-tools](https://github.com/LoKiGGo/dsh-tools) | 1 | 2026-08-16 | 2026-08-27 | dsh web通用工具箱插件，纯AI制作（包括仓库），零人工含量，可能不会维护，请谨慎使用。 |
| 450 | [LONGSASASASASA/dsh-issue2pr](https://github.com/LONGSASASASASA/dsh-issue2pr) | 1 | 2026-08-29 | 2026-08-30 | 从一条 Issue 到一份被合并的 PR，每一段都有自己的输入契约、失败信号、可回滚产物与可独立审查的 Artifact。 |
| 451 | [looput/dsh-finance-lab](https://github.com/looput/dsh-finance-lab) | 1 | 2026-08-18 | 2026-08-27 | DeepSeek Harness finance plugin: direct market HTTP APIs, portfolio settings, model tools |
| 452 | [LouisCanBe/dsh-plugin-ollama-monitor](https://github.com/LouisCanBe/dsh-plugin-ollama-monitor) | 1 | 2026-09-02 | 2026-09-02 | Ollama 监控与测评平台 · DeepSeek Harness (DSH) 插件组合包：agent 工具 + Web 设置页面板（npm: ollama-monitor） |
| 453 | [LouisHaoL/cloudcli-timer-agent](https://github.com/LouisHaoL/cloudcli-timer-agent) | 1 | 2026-09-01 | 2026-09-01 | CloudCLI plugin: cron & fixed-interval scheduler for AI agent prompts and command jobs (dsh-timer-agent port) \| CloudCLI 定时任务插件 |
| 454 | [louishzwang/dsh-web-launcher](https://github.com/louishzwang/dsh-web-launcher) | 1 | 2026-08-21 | 2026-08-31 | DSH Web本地终端启动脚本 |
| 455 | [lovaxi/Rubato_Device](https://github.com/lovaxi/Rubato_Device) | 1 | 2026-08-30 | 2026-09-01 | Rubato - a palm-sized retro-Macintosh AI desk companion that turns AI wait time into gentle health breaks. Firmware, tools and docs. |
| 456 | [lrplrplrp/dsh-live2d](https://github.com/lrplrplrp/dsh-live2d) | 1 | 2026-09-01 | 2026-09-02 | deepseek-harness对live2d的支持 |
| 457 | [luckycaoj/dsh-plugin-session-console-sleepcat](https://github.com/luckycaoj/dsh-plugin-session-console-sleepcat) | 1 | 2026-08-31 | 2026-08-31 | 一个dsh的辅助使用小插件，DSH client plugin: embedded tool rail + session questions console — jump to past questions, collapse the model's working process. 🐱 |
| 458 | [lumose0/dsh-file-reference-everything](https://github.com/lumose0/dsh-file-reference-everything) | 1 | 2026-08-27 | 2026-08-27 | Whole-disk @ file references for DeepSeek Harness — Everything-backed instant search with fuzzy/regex and a cross-platform fallback index |
| 459 | [Lunatic029/dsh-clash-proxy](https://github.com/Lunatic029/dsh-clash-proxy) | 1 | 2026-08-27 | 2026-08-27 | Route DeepSeek Harness's outbound network through Clash — LLM, web search/fetch and shell commands all use your local Clash proxy. |
| 460 | [Lzh3070/dsh-model-visibility](https://github.com/Lzh3070/dsh-model-visibility) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件：模型可见性管理——按渠道/模型隐藏或显示模型选择菜单里的条目 / Control which models appear in the DSH model selector |
| 461 | [m1khal3v/dsh-tool-codegraph](https://github.com/m1khal3v/dsh-tool-codegraph) | 1 | 2026-08-29 | 2026-08-30 | CodeGraph navigation tools for DeepSeek Harness |
| 462 | [makajo/dsh-gemini-m3e-theme](https://github.com/makajo/dsh-gemini-m3e-theme) | 1 | 2026-08-29 | 2026-08-30 | Gemini-style Material 3 Expressive theme for DeepSeek Harness Web (persistent client bundle) |
| 463 | [mapan0424/deepseek-harness-plugins](https://github.com/mapan0424/deepseek-harness-plugins) | 1 | 2026-09-02 | 2026-09-02 | Unofficial community plugins collection for DeepSeek Harness |
| 464 | [mastergo-design/dsh-canvas](https://github.com/mastergo-design/dsh-canvas) | 1 | 2026-08-27 | 2026-08-27 | MasterGo Canvas MCP plugin for DeepSeek Harness |
| 465 | [me93-ghb/dsh-matrix-think](https://github.com/me93-ghb/dsh-matrix-think) | 1 | 2026-08-27 | 2026-08-27 | Matrix rain for expanded thinking in DeepSeek Harness Web |
| 466 | [mengnanxyyyy/dsh-markdown-xyy](https://github.com/mengnanxyyyy/dsh-markdown-xyy) | 1 | 2026-08-29 | 2026-08-29 | dsh markdown 主题插件 |
| 467 | [MerlinShieh/Agent-skill-wechatPush](https://github.com/MerlinShieh/Agent-skill-wechatPush) | 1 | 2026-08-03 | 2026-09-02 | Agent skill，当任务完成时会主动通过微信公众号推送洗洗脑 |
| 468 | [MerlinShieh/AgentMemHub](https://github.com/MerlinShieh/AgentMemHub) | 1 | 2026-08-25 | 2026-08-27 | 统一提取多 Agent Harness 会话为全量事件流(含工具链/思维链/Shell/补丁) → SQLite 检索 → 桥接 MemOS 生成记忆 |
| 469 | [MichaelShii/dsh-plugin-teamflow](https://github.com/MichaelShii/dsh-plugin-teamflow) | 1 | 2026-08-17 | 2026-08-27 | dsh plugin teamflow |
| 470 | [Missher12/deepseek-harness-desktop](https://github.com/Missher12/deepseek-harness-desktop) | 1 | 2026-08-13 | 2026-08-29 | Unofficial Intel macOS desktop app for DeepSeek Harness |
| 471 | [mldhao/dsh-conversation-strip](https://github.com/mldhao/dsh-conversation-strip) | 1 | 2026-08-27 | 2026-08-27 | Codex-inspired vertical conversation-turn rail for the DeepSeek Harness web UI. |
| 472 | [moonlin1213/dsh-agent-sound-alert](https://github.com/moonlin1213/dsh-agent-sound-alert) | 1 | 2026-08-29 | 2026-08-29 | macOS sound alerts for DeepSeek Harness agent lifecycle events |
| 473 | [Moonshile/moonshile-dsh-plugins](https://github.com/Moonshile/moonshile-dsh-plugins) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) plugins — dsh-workspace-sort: re-sorts sidebar workspaces by last activity once per day. One-command npm bundle install. |
| 474 | [Movingtoleveltwo/dsh-revert](https://github.com/Movingtoleveltwo/dsh-revert) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 现代化对话回退与重试插件：纯 UI 图形交互、原地 Prompt 微调、支持工作区与外部文件双引擎安全恢复。 |
| 475 | [mtdx2001/think-zh](https://github.com/mtdx2001/think-zh) | 1 | 2026-08-29 | 2026-08-29 | AI reasoning real-time Chinese localization suite (DSH ready, OpenAI-compatible endpoint) |
| 476 | [MuAllen/dsh-gateway-wallet](https://github.com/MuAllen/dsh-gateway-wallet) | 1 | 2026-08-24 | 2026-08-27 | 读取当前 API key 在站点账本上的剩余额度和实扣，支持 Sub2API、New API 与 DeepSeek 官方，不是本地 token 估算。 |
| 477 | [mumuer1024/dsh-ui-liteglass](https://github.com/mumuer1024/dsh-ui-liteglass) | 1 | 2026-08-21 | 2026-08-27 | LiteGlass — a lightweight appearance skin for DeepSeek Harness Web UI: wallpaper, glass-like transparency, and accent color. Server-side settings, multi-device, leaves native light/dark mode alone. |
| 478 | [my-dsh/dsh-web-search-tavily](https://github.com/my-dsh/dsh-web-search-tavily) | 1 | 2026-08-30 | 2026-08-30 | Tavily web-search provider plugin for DeepSeek Harness (dsh) — registers into ctx.web so the model-facing web_search tool uses Tavily |
| 479 | [mycherish/dsh-bridge](https://github.com/mycherish/dsh-bridge) | 1 | 2026-08-29 | 2026-09-01 | DSH Bridge 是 DeepSeek Harness 的原生 macOS 菜单栏快速入口，不是完整聊天客户端，也不是 DSH Web 的套壳。 |
| 480 | [myYangyunfan/dsh_cardian](https://github.com/myYangyunfan/dsh_cardian) | 1 | 2026-09-01 | 2026-09-02 | cardian — DeepSeek Harness knowledge-center plugin: RepoWiki notes / flashcards / memory in a local Obsidian vault |
| 481 | [N9-Developer-Empowerment/DSH-Vibeify](https://github.com/N9-Developer-Empowerment/DSH-Vibeify) | 1 | 2026-08-26 | 2026-08-29 | Turn AI work into a living local magazine for DeepSeek Harness. DeepSeek, ChatGPT, or both. |
| 482 | [Nath-Vikky/dsh-codekin](https://github.com/Nath-Vikky/dsh-codekin) | 1 | 2026-08-24 | 2026-08-28 | Codekin: a creature-collection and match-three RPG for DeepSeek Harness Web. |
| 483 | [NexusAgentX/dsh-reasoning-effort](https://github.com/NexusAgentX/dsh-reasoning-effort) | 1 | 2026-08-15 | 2026-08-27 | Host-side dsh plugin that adds seven reasoning-effort levels to third-party llm-pi-ai models in the web composer. |
| 484 | [Niceck/dsh-hhxg-market](https://github.com/Niceck/dsh-hhxg-market) | 1 | 2026-08-27 | 2026-08-27 | 恢恢量化 hhxg.top A股量化数据插件 for DeepSeek Harness (dsh)：6 个免费工具 + 5 个 VIP 工具（MCP 桥接）· A-share quant data plugin |
| 485 | [NimuStudio/NimuQDock-dsh](https://github.com/NimuStudio/NimuQDock-dsh) | 1 | 2026-08-27 | 2026-08-27 | 把 DeepSeek Harness接入QQ的对接坞——带人格引擎的仿真群友：心情、精力、记忆，像真人一样潜水与参与。 |
| 486 | [ningbonb/dsh-web-desktop](https://github.com/ningbonb/dsh-web-desktop) | 1 | 2026-08-31 | 2026-08-31 | Electron launcher for DeepSeek Harness Web profiles / DeepSeek Harness Web Profile 的 Electron 桌面启动器 |
| 487 | [niyongsheng/meww](https://github.com/niyongsheng/meww) | 1 | 2026-08-27 | 2026-08-27 | pokemon ai pet🐣电子宠物 |
| 488 | [njjpro/dsh-vault](https://github.com/njjpro/dsh-vault) | 1 | 2026-08-30 | 2026-08-30 | Persistent credential vault plugin for DeepSeek Harness (DSH) - manage API tokens, server logins, and site credentials in one settings panel. |
| 489 | [Noemm/dsh-web-search-glm](https://github.com/Noemm/dsh-web-search-glm) | 1 | 2026-08-28 | 2026-08-28 | Zhipu GLM search provider for the DeepSeek Harness (dsh) web seam — native web_search via the Anthropic-compatible API |
| 490 | [NOirBRight/dsh-llm-commandcode](https://github.com/NOirBRight/dsh-llm-commandcode) | 1 | 2026-08-27 | 2026-08-29 | Command Code Provider API LLM plugin for DeepSeek Harness |
| 491 | [NOirBRight/dsh-model-switch](https://github.com/NOirBRight/dsh-model-switch) | 1 | 2026-08-19 | 2026-08-29 | Model purposes spec and tickets for DeepSeek Harness |
| 492 | [NoxTyrannus/dsh-cipher](https://github.com/NoxTyrannus/dsh-cipher) | 1 | 2026-08-29 | 2026-08-29 | 把 cipher 的持续思考/三中台/四类记忆以 UNNI/LOOP 会话模式接入 DSH（dsh-plugin bundle） |
| 493 | [Nuomi9/dsh-fgo-chaldea](https://github.com/Nuomi9/dsh-fgo-chaldea) | 1 | 2026-08-15 | 2026-08-27 | FGO Chaldea-inspired skin pack for DeepSeek Harness Web UI: 5 themes, original generated backdrops, gold trim. |
| 494 | [Nzssm1/dsh-strategy-deployment-review](https://github.com/Nzssm1/dsh-strategy-deployment-review) | 1 | 2026-08-27 | 2026-08-27 | DSH agent preset for rigorous strategy live-deployment testing/evaluation. Retest. |
| 495 | [objectivex666/dsh-settings-search](https://github.com/objectivex666/dsh-settings-search) | 1 | 2026-08-25 | 2026-08-27 | A plugin that adds a search box to the DSH settings panel. |
| 496 | [ohmejj/dsh-chat-archive](https://github.com/ohmejj/dsh-chat-archive) | 1 | 2026-08-28 | 2026-09-02 | 自动归档 DeepSeek Harness 对话记录 |
| 497 | [onenameneo/dsh-plugin-loom-chat](https://github.com/onenameneo/dsh-plugin-loom-chat) | 1 | 2026-08-30 | 2026-08-31 | Loom Chat is a DSH Web client plugin that turns linear ordinary sessions into a pannable, zoomable Loom-style canvas for parallel exploration. |
| 498 | [openllmsh/dsh](https://github.com/openllmsh/dsh) | 1 | 2026-08-24 | 2026-08-27 | DeepSeek Harness (dsh) bundle: route the harness through OpenLLM (OpenAI-compatible) + register the OpenLLM MCP, with CLI/daemon onboarding. |
| 499 | [Pappet/dsh-tool-imagegen](https://github.com/Pappet/dsh-tool-imagegen) | 1 | 2026-08-30 | 2026-08-31 | Text-to-image and image-to-image generation for DeepSeek Harness via OpenRouter's unified Image API, with capability-gated parameters |
| 500 | [patrickluvsoj/dsh-llm-nous](https://github.com/patrickluvsoj/dsh-llm-nous) | 1 | 2026-08-21 | 2026-08-27 | Nous Portal LLM plugin bundle for DeepSeek Harness |
| 501 | [Perfirstvito/dsh-compaction-micro](https://github.com/Perfirstvito/dsh-compaction-micro) | 1 | 2026-09-01 | 2026-09-01 | a context compact strategy plugin |
| 502 | [phantomSuying/dsh-module-driven-develop](https://github.com/phantomSuying/dsh-module-driven-develop) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin for module-driven development: decompose requirements into a module tree, generate each module with an independent agent, and fully regenerate from design on any change. |
| 503 | [pipipigu/dsh-workspace-tree](https://github.com/pipipigu/dsh-workspace-tree) | 1 | 2026-08-28 | 2026-08-28 | Virtual session folder grouping, drag & drop, and subproject manager for DeepSeek Harness (DSH). |
| 504 | [pn1024/dsh-ppt-master](https://github.com/pn1024/dsh-ppt-master) | 1 | 2026-08-31 | 2026-08-31 | PPT Master skill packaged as a DeepSeek Harness (dsh) plugin: AI-driven presentation workflow for editable PPTX decks, SVG snapshots, native template filling, and PPTX enhancement. |
| 505 | [promisez322-prog/dsh-vox-input](https://github.com/promisez322-prog/dsh-vox-input) | 1 | 2026-08-30 | 2026-08-30 | Voice (speech-to-text) input for the DSH Web composer via Web Speech API — tap, speak, transcript fills the input box. Zero server, zero API keys. |
| 506 | [ptonlix/dsh-forge](https://github.com/ptonlix/dsh-forge) | 1 | 2026-08-22 | 2026-08-31 |  building an auditable desktop distribution around DeepSeek Harness (DSH).  |
| 507 | [pwping/dsh-power-launch](https://github.com/pwping/dsh-power-launch) | 1 | 2026-08-29 | 2026-08-29 | DSH桌面启动器插件，双击桌面快捷方式启动dsh Web UI，不需要每次打开终端手动输入命令 |
| 508 | [qfwycn/dsh-media-serve](https://github.com/qfwycn/dsh-media-serve) | 1 | 2026-09-02 | 2026-09-02 | 用于在deepseek harness上直接暴露工作区的文件，使大肥鱼能够直接显示他想给你显示的图片等信息，解决了大肥鱼老是说自己显示不了图片，要你去看本地文件的问题。在过验证码或截图的时候极为有用。 |
| 509 | [QinpanWan/dsh-doc-quick](https://github.com/QinpanWan/dsh-doc-quick) | 1 | 2026-08-25 | 2026-08-27 | Drag documents into the dsh web chat for direct local-file processing; a right sidebar lists outputs and file paths. 拖拽文档进 Web 对话框快速处理，右侧侧栏展示产出。 |
| 510 | [QinpanWan/dsh-harmonyos-market](https://github.com/QinpanWan/dsh-harmonyos-market) | 1 | 2026-08-24 | 2026-08-27 | HarmonyOS-exclusive plugin market for DeepSeek Harness — only plugins that actually run on HarmonyOS |
| 511 | [QinpanWan/dsh-prompt-antivirus](https://github.com/QinpanWan/dsh-prompt-antivirus) | 1 | 2026-08-31 | 2026-08-31 | dsh 全局防提示注入/上下文病毒感染插件：扫描工具参数、结果、进模型前消息与出站流；quarantine/block/monitor 三模式 + 金丝雀 + 可演进签名库（学习/导入/导出）。纯 JS 零原生依赖。 |
| 512 | [Qiongkura/dsh-interface-settings](https://github.com/Qiongkura/dsh-interface-settings) | 1 | 2026-08-16 | 2026-08-29 | DSH interface customization plugin: wallpaper / transparency / glass blur / splash screen一个 DeepSeek Harness 前端插件：把「壁纸 / 区域透明 / 输入框与轨迹毛玻璃 / 模糊程度 / 启动画面」做成一站式界面设置，作为独立插件项目上传、分享，装进 DSH 即可使用 |
| 513 | [qiufengcrl/dsh-ip-https](https://github.com/qiufengcrl/dsh-ip-https) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: remote settings + Let's Encrypt IP certificates |
| 514 | [qixin-ai-data/dsh-qixin-insight-mcp-oauth](https://github.com/qixin-ai-data/dsh-qixin-insight-mcp-oauth) | 1 | 2026-08-29 | 2026-08-31 | DeepSeek Harness 插件：一键 OAuth 2.1 (PKCE) 授权，将启信慧眼 MCP 服务端挂载进 harness，让模型直接触达企业工商、股权、司法与风险等智能数据。 |
| 515 | [qiyeren/dsh-eac-popup](https://github.com/qiyeren/dsh-eac-popup) | 1 | 2026-08-27 | 2026-08-27 | DSH plugin: ???? agent ??/?????,EAC ????(??????)+?????5?+?????? |
| 516 | [QuantumKuba/dsh-continuum](https://github.com/QuantumKuba/dsh-continuum) | 1 | 2026-09-02 | 2026-09-02 | Durable project state and checkpoint engine for DeepSeek Harness (DSH). Prevents context exhaustion in long-running multi-agent workflows by persisting tasks, evidence, and checkpoints to disk. |
| 517 | [QuantumKuba/dsh-graphify-plugin](https://github.com/QuantumKuba/dsh-graphify-plugin) | 1 | 2026-08-31 | 2026-08-31 | Native Graphify knowledge graph plugin for DeepSeek Harness (DSH) — code intelligence, god nodes, and topological agent tools. |
| 518 | [Raiyan007-gb/dsh-remote-tunnel-easy](https://github.com/Raiyan007-gb/dsh-remote-tunnel-easy) | 1 | 2026-08-28 | 2026-08-29 | DSH plugin bundle: scan a QR to open the deepseek-harness web UI on your phone inside the same session - cloudflared quick tunnel, no database, Windows/macOS/Linux |
| 519 | [ramen-ai-dev/dsh-ramen-guard](https://github.com/ramen-ai-dev/dsh-ramen-guard) | 1 | 2026-08-27 | 2026-08-27 | Fail-closed DeepSeek Harness guard enforcing ramen-ai Core IT policy before tool execution. |
| 520 | [Raphaelutumn/dsh-mood](https://github.com/Raphaelutumn/dsh-mood) | 1 | 2026-08-27 | 2026-08-27 | A tiny behavioral mood ring for your AI coding agent: a four-state session-header status light (GOOD/CONFUSED/FRUSTRATED/OVERWHELMED) for DeepSeek Harness |
| 521 | [redfox-data/redfox-skill-gallery](https://github.com/redfox-data/redfox-skill-gallery) | 1 | 2026-08-26 | 2026-09-01 | redfox-skill-gallery是 DeepSeek Harness 的 Web 插件。它在侧边栏底部加一个「红狐Skills」入口，点击后整个界面切换为卡片式技能画廊，集中展示redfox-community-dsh插件内的全部红狐社区 skills |
| 522 | [renchengxiang/dsh-web-search-tavily](https://github.com/renchengxiang/dsh-web-search-tavily) | 1 | 2026-08-28 | 2026-08-28 | Tavily-backed web search provider for DeepSeek Harness, with Settings → Plugins configuration UI |
| 523 | [RGarvel/dsh-channel-spec](https://github.com/RGarvel/dsh-channel-spec) | 1 | 2026-08-27 | 2026-08-27 | RFC: 按来源渠道对 DSH 会话分类展示（session header channel 字段 + GUI 渠道视图）— 源自 deepseek-harness discussion #3897 |
| 524 | [RGarvel/dsh-channel-view](https://github.com/RGarvel/dsh-channel-view) | 1 | 2026-08-27 | 2026-08-27 | DSH 渠道会话视图 spike：侧边栏 Channels tab 注入 + 会话投影数据链（RFC-0001, discussion #3897） |
| 525 | [rogerdigital/dsh-vet](https://github.com/rogerdigital/dsh-vet) | 1 | 2026-08-29 | 2026-08-29 | Security vetting for DeepSeek Harness (DSH) plugins: permission & supply-chain audits before install, graded via the open dsh-vet/v1 report standard. |
| 526 | [rongxingda/dsh-prompt-enhance](https://github.com/rongxingda/dsh-prompt-enhance) | 1 | 2026-08-29 | 2026-08-29 | Prompt enhancement plugin for the DeepSeek Harness web GUI: one-click rewrite of the composer draft into a structured prompt, with preview, fill-back, and undo. |
| 527 | [Roxy-gl373/dsh-desktop](https://github.com/Roxy-gl373/dsh-desktop) | 1 | 2026-09-02 | 2026-09-02 | DSh Whale · DeepSeek Harness 桌面启动器：WebView2 内嵌 DSH 界面，实时日志、单实例托盘、多开、等比缩放，装插件自动快照回滚。install.cmd 一键配置。 |
| 528 | [Ruixinhua/dsh-universe-api](https://github.com/Ruixinhua/dsh-universe-api) | 1 | 2026-08-27 | 2026-08-27 | Offline, deterministic public API discovery for DeepSeek Harness and DSH Desktop. |
| 529 | [runcat-tommy/dsh-chinese-poetry](https://github.com/runcat-tommy/dsh-chinese-poetry) | 1 | 2026-09-02 | 2026-09-02 | A token-free Chinese classical poetry plugin for DeepSeek Harness Web: search, filters, Feihua, daily poem, favorites, and AI explain. Powered by the free public chinese-poetry-api. |
| 530 | [runfali/dsh-prompt-injector](https://github.com/runfali/dsh-prompt-injector) | 1 | 2026-08-27 | 2026-08-27 | dsh 通用每轮上下文注入插件：设置页管理提示词清单，每轮对话把每条启用提示词以「上下文注入」提醒行注入模型上下文，让纪律规则（例如 图谱消费/wiki 先查/记忆召回）可靠生效。 |
| 531 | [SA1992X/dsh-ctrl-enter-submit](https://github.com/SA1992X/dsh-ctrl-enter-submit) | 1 | 2026-08-25 | 2026-08-27 | 轻松换行 |
| 532 | [sandersyao/dsh-session-persistence-mysql](https://github.com/sandersyao/dsh-session-persistence-mysql) | 1 | 2026-09-01 | 2026-09-01 | deepseek harness 插件 替换会话持久化引擎为 MySQL 数据库 |
| 533 | [says693/dsh-composer-dynamic-island](https://github.com/says693/dsh-composer-dynamic-island) | 1 | 2026-09-02 | 2026-09-02 | Compact DSH Web composer island with a Community v0.15 host manifest and no user-defined button positioning. |
| 534 | [SeerableOfficial/dsh-anydoc-markdown](https://github.com/SeerableOfficial/dsh-anydoc-markdown) | 1 | 2026-08-29 | 2026-08-31 | Document → Markdown + vision image description plugin for DeepSeek Harness (dsh). Converts Word/PPT/Excel/ODT/RTF/EPUB/CSV/PDF via firecrawl-anydoc and describes embedded images with a VLM. |
| 535 | [SeverusZh/dsh-ollama-usage](https://github.com/SeverusZh/dsh-ollama-usage) | 1 | 2026-08-27 | 2026-08-27 | Ollama Cloud 用量余量可视化 DeepSeek Harness 插件:5h 会话/周用量双横条 + 设置页面板,Key 与快照持久化,自动刷新,登录引导。Ollama Cloud usage & quota visualization plugin for DeepSeek Harness. |
| 536 | [Shaky77/KISS_Law-DSH](https://github.com/Shaky77/KISS_Law-DSH) | 1 | 2026-08-19 | 2026-08-27 | Weiwen's Law (KISS-Law) — a domain-agnostic causal-constraint middleware for DeepSeek Harness. A faithful, white-box presentation of how causal law actually runs. White-box audit, never prediction. Hard-gate the boundary; inner H decides freely. |
| 537 | [shaomingbo/dsh-subscription-search](https://github.com/shaomingbo/dsh-subscription-search) | 1 | 2026-08-19 | 2026-08-30 | ChatGPT/Grok subscription OAuth, model routes, and ChatGPT to Grok to Exa to DeepSeek web-search fallback for DeepSeek Harness |
| 538 | [shengmk/godsh](https://github.com/shengmk/godsh) | 1 | 2026-08-28 | 2026-08-28 | godsh - GUI launcher for DeepSeek Harness (dsh): manage profiles, plugins, kernels, and dsh versions |
| 539 | [shimingming520/dsh-audiogen](https://github.com/shimingming520/dsh-audiogen) | 1 | 2026-08-28 | 2026-08-29 | AI audio generation plugin for the DeepSeek Harness web GUI: multi-vendor TTS, music, sound effects and voice design with a sidebar panel, model comparison, resource library and Agent tools. |
| 540 | [ShinonomeAya/dsh-git-chain](https://github.com/ShinonomeAya/dsh-git-chain) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: Cursor-style Git commit-chain graph with SVG lanes, commit details, diff, filtering, and guarded branch switching. |
| 541 | [shuaweng/DSH_xieshujing](https://github.com/shuaweng/DSH_xieshujing) | 1 | 2026-08-30 | 2026-08-30 | 写书鲸：面向 DeepSeek Harness 的原生 AI 小说创作工作台插件 |
| 542 | [SleepEggTart/dsh-code-coverage](https://github.com/SleepEggTart/dsh-code-coverage) | 1 | 2026-08-26 | 2026-08-27 | 解析 DSH session 日志归因 AI 生成文件，叠加 c8 覆盖率，产出 AI vs 人工代码覆盖率对比、高危未测文件清单与信任分。 |
| 543 | [SleepEggTart/dsh-dev-wrapped](https://github.com/SleepEggTart/dsh-dev-wrapped) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (DSH) 开发者使用报告——类 Spotify Wrapped，统计与 AI 结对编程的行为，生成可分享报告卡片 |
| 544 | [SleepEggTart/dsh-mbti-jury](https://github.com/SleepEggTart/dsh-mbti-jury) | 1 | 2026-08-31 | 2026-08-31 | DSH 插件：16 型 MBTI 人格评审团，并排评审你最近一次 commit——同一个 diff，16 种看见世界的方式。 |
| 545 | [Snow-ea/dsh-token-optimizer](https://github.com/Snow-ea/dsh-token-optimizer) | 1 | 2026-08-30 | 2026-08-30 | Deterministic, recoverable tool-result compression and cache-aware compaction for DeepSeek Harness. |
| 546 | [softspark/dsh-codex](https://github.com/softspark/dsh-codex) | 1 | 2026-08-25 | 2026-08-27 | DeepSeek Harness provider for locally authenticated Codex app-server access through a ChatGPT subscription. |
| 547 | [sogoodayo/dsh-code-ui](https://github.com/sogoodayo/dsh-code-ui) | 1 | 2026-09-01 | 2026-09-02 | Cursor 风格的 AI 代码编辑器工作台插件（DSH）：文件树、多标签页编辑、引用/备注/翻译、内嵌 AI 输入框、语法高亮 |
| 548 | [sperictao/dsh-pro-max](https://github.com/sperictao/dsh-pro-max) | 1 | 2026-08-20 | 2026-09-01 | DeepSeek Harness desktop launcher — one-click local web UI, Tailscale-secured remote access, plugin marketplace & model configuration. Built with Tauri 2 + React + TypeScript. |
| 549 | [spritebbb/dsh-skill-usage](https://github.com/spritebbb/dsh-skill-usage) | 1 | 2026-08-31 | 2026-08-31 | DSH 实时技能显示小插件 🌟 输入框下方的可爱小徽章，实时显示当前技能，悬停看历史。Real-time active skill chip for DeepSeek Harness. |
| 550 | [starsinc1708/dsh-tool-council](https://github.com/starsinc1708/dsh-tool-council) | 1 | 2026-08-26 | 2026-08-27 | Map-reduce council of subagents for the DeepSeek Harness: one task fans out to independent members, their findings are deduplicated, verified by a separate panel, and reduced to a quorum report |
| 551 | [SUFE-Chaoyi/dsh-plugin-csv-report](https://github.com/SUFE-Chaoyi/dsh-plugin-csv-report) | 1 | 2026-08-31 | 2026-08-31 | 基于 DeepSeek Harness 的可复用 CSV 描述统计与可复现报告插件 |
| 552 | [summer-521/deepseek-harness-swift](https://github.com/summer-521/deepseek-harness-swift) | 1 | 2026-08-25 | 2026-08-28 | 基于 AppKit、SwiftUI 与 WKWebView 的 DSH 原生 macOS 桌面壳，提供设置中心、DSH 版本管理、插件管理、通知和 Sparkle 应用更新。 |
| 553 | [Sunday2Mo/dsh-file-quote](https://github.com/Sunday2Mo/dsh-file-quote) | 1 | 2026-08-27 | 2026-08-27 | 基于 better-sidebar 的统一引用插件：划选文件/消息即可批注引用，引用块带文件路径与行区间、双端折叠、点击跳回原文 ｜ Unified-quoting plugin built on DSH-better-sidebar: select files or messages to annotate; quote blocks carry path & line range, collapse in chat and history, and jump back to the source on click. |
| 554 | [sunzhyang1616-ui/dsh-ssh-terminal](https://github.com/sunzhyang1616-ui/dsh-ssh-terminal) | 1 | 2026-08-29 | 2026-08-29 | 在 DSH 侧边栏（dsh-better-sidebar）连接远程主机的 SSH 终端：逐步查看 agent 命令与输出，内置 ssh_connect / ssh_exec 等工具，记录本机持久化。 |
| 555 | [svgop/dsh-rich-questions](https://github.com/svgop/dsh-rich-questions) | 1 | 2026-08-26 | 2026-08-29 | Rich branching survey system for DeepSeek Harness (DSH) Web GUI — ask_survey tool with branch graphs, delayed hover insights, Mermaid diagrams, quick mode, reroll/push/discuss actions |
| 556 | [sycamorestr/dsh-platform-account-manager-plugin](https://github.com/sycamorestr/dsh-platform-account-manager-plugin) | 1 | 2026-08-29 | 2026-08-29 | DSH platform account and persistent browser-session manager |
| 557 | [taoser258/dsh-client-ui-skin-qingxiao](https://github.com/taoser258/dsh-client-ui-skin-qingxiao) | 1 | 2026-08-29 | 2026-08-29 | 清宵 · 弦凝清霄 —— DeepSeek Harness (DSH) Web 界面美化皮肤：以《鸣潮》角色清宵为灵感的冰蓝·青碧·月白·玄夜调色板，含可换背景画卷、剑气流光粒子、磨砂玻璃面板与新会话迎宾页。A Qingxiao (Wuthering Waves) themed client UI skin for the DSH web GUI. |
| 558 | [TelosmaYLX/dsh-session-notify](https://github.com/TelosmaYLX/dsh-session-notify) | 1 | 2026-08-28 | 2026-08-28 | 当dsh任务完成/阻塞/提问等情况时，自动推送windows消息进行提醒，支持自定义文案和图片，以及显示会话用时、消耗token、速度tps等指标。Automatically push Windows notifications upon completion of a dsh task, supporting custom text and images, as well as displaying metrics including session duration, token consumption, and TPS speed. |
| 559 | [TestTheBoy/dsh_plugin_file_attach](https://github.com/TestTheBoy/dsh_plugin_file_attach) | 1 | 2026-08-26 | 2026-08-27 | Add files to context |
| 560 | [tiger0012/dsh-we-wallpaper-sync](https://github.com/tiger0012/dsh-we-wallpaper-sync) | 1 | 2026-08-26 | 2026-08-27 | Reusable skill: browse/search/download Wallpaper Engine (Steam 431960) workshop wallpapers and wire them into the DSH skin center, bypassing the Steam HTTP block and region-mismatch sign-in block. |
| 561 | [Tinger-X/dsh-session-enhance](https://github.com/Tinger-X/dsh-session-enhance) | 1 | 2026-08-25 | 2026-08-31 | Full-control session management for DeepSeek Harness Web |
| 562 | [tower1229/dsh-thinkbar](https://github.com/tower1229/dsh-thinkbar) | 1 | 2026-08-29 | 2026-08-31 | 让 DeepSeek Harness 的思考状态被看见——零侵入地将 reasoning 等待转化为由蓝到金、持续升温的动态 ThinkBar。 |
| 563 | [trrrrrryg/dsh-ssh-forge](https://github.com/trrrrrryg/dsh-ssh-forge) | 1 | 2026-08-24 | 2026-08-27 | DSH SSH Forge：为 DeepSeek Harness（DSH）提供 SSH 远程工作区能力：已核验的服务器身份、失败关闭的 Agent 执行路由、远端文件与命令操作；提供 Windows 离线一键安装包，无需 Node.js 或构建工具。 |
| 564 | [tyx6661234/dsh-community-listening](https://github.com/tyx6661234/dsh-community-listening) | 1 | 2026-08-26 | 2026-08-27 | 面向 DeepSeek Harness (DSH) 的社交评论研究插件 |
| 565 | [Ultmebius/universal-plugin-hub](https://github.com/Ultmebius/universal-plugin-hub) | 1 | 2026-08-26 | 2026-08-31 | DSH 插件市场：内置 Claude 官方插件目录，支持添加 Git 仓库作为插件源；一键安装，技能、子代理、MCP、LSP、hooks 装完自动接线 · Plugin marketplace for DeepSeek Harness |
| 566 | [UNscientific-9/dsh-turnfold](https://github.com/UNscientific-9/dsh-turnfold) | 1 | 2026-08-27 | 2026-08-27 | DSH Web 轮次折叠插件：thinking/工具调用流式可见，turn 完成后自动收纳成一行摘要。 |
| 567 | [v587d/dsh-custom-skin](https://github.com/v587d/dsh-custom-skin) | 1 | 2026-08-28 | 2026-08-28 | 自己的插件皮肤管理工具。 |
| 568 | [v587d/dsh-search-first](https://github.com/v587d/dsh-search-first) | 1 | 2026-09-01 | 2026-09-01 | Search first, verify facts, reply last — enforced by DSH. |
| 569 | [valuelesser/pipeline-mode](https://github.com/valuelesser/pipeline-mode) | 1 | 2026-09-01 | 2026-09-01 | LangGraph-style adaptive Planner→Executor→Reviewer pipeline for DSH (DeepSeek Harness) |
| 570 | [victor10035445/dsh-v-explorer](https://github.com/victor10035445/dsh-v-explorer) | 1 | 2026-09-02 | 2026-09-02 | right slider for deepseek-harness-plugin. |
| 571 | [victor10035445/dsh-v-skill-links](https://github.com/victor10035445/dsh-v-skill-links) | 1 | 2026-09-02 | 2026-09-02 | let dsh use your skills.quick command and diy buttons. |
| 572 | [victor10035445/dsh-v-theme](https://github.com/victor10035445/dsh-v-theme) | 1 | 2026-09-02 | 2026-09-02 | theme plugin for deepseek harness by victor |
| 573 | [VioletScar-Hui/dsh-chat-history](https://github.com/VioletScar-Hui/dsh-chat-history) | 1 | 2026-09-02 | 2026-09-02 | 给 DSH 聊天输入框加上 CLI 风格历史记忆：上下键召回之前发送过的内容（纯客户端插件，重启不丢） |
| 574 | [VioletScar-Hui/trcost-plugin](https://github.com/VioletScar-Hui/trcost-plugin) | 1 | 2026-08-28 | 2026-08-28 | 轨迹省钱优化器：DSH 会话轨迹 token 浪费分析 + waterfall 执行层强制拦截/截断。Trajectory cost optimizer with enforcement layer for DeepSeek Harness. |
| 575 | [w2327644822-png/dsh-usage-analytics](https://github.com/w2327644822-png/dsh-usage-analytics) | 1 | 2026-08-26 | 2026-08-27 | Personal usage analytics & activity dashboard for the DeepSeek Harness (dsh) web GUI: token totals, contribution heatmap, model share, insights. Local-only, metadata only. |
| 576 | [warment/deepseek-harness-locale-ru](https://github.com/warment/deepseek-harness-locale-ru) | 1 | 2026-08-30 | 2026-08-30 | Русский язык для DeepSeek Harness web UI — one-command install, 1061 строка, 100% покрытие |
| 577 | [Washington5533/guarftrain](https://github.com/Washington5533/guarftrain) | 1 | 2026-08-09 | 2026-08-27 | 🛡️ 一行命令，训练脚本零行改动，获得完整守护能力。GPU 监控 · 崩溃恢复 · OOM 自救 · Agent 决策 · MCP 35 工具 · Web Dashboard。 |
| 578 | [Weiyang742/dsh-cross-session-messaging](https://github.com/Weiyang742/dsh-cross-session-messaging) | 1 | 2026-08-31 | 2026-08-31 | Cross-session relay for DeepSeek Harness: peer discovery and text delivery between independent dsh processes. |
| 579 | [wenyixiaoqingnian/screenshot-review](https://github.com/wenyixiaoqingnian/screenshot-review) | 1 | 2026-08-29 | 2026-08-29 | dsh skill: 截图审阅——模型自己截图、自己看图、自己改代码，迭代优化前端效果 |
| 580 | [WesleyJay/dsh-weather](https://github.com/WesleyJay/dsh-weather) | 1 | 2026-08-27 | 2026-08-28 | 一个 DSH 天气查询插件，让 AI 智能体可以查询全球城市的实时天气和天气预报 |
| 581 | [wjf1/dsh-commandcode](https://github.com/wjf1/dsh-commandcode) | 1 | 2026-08-30 | 2026-08-30 | DSH-Desktop LLM provider plugin for Command Code with model catalog sync, request retry, multi-credential support, and a settings UI. |
| 582 | [wly8691-jpg/dsh-office-com](https://github.com/wly8691-jpg/dsh-office-com) | 1 | 2026-08-26 | 2026-08-27 | DSH plugin: COM-driven real Office automation (VBA/pivot/recalc/layout) |
| 583 | [wodongx123/dsh-qq-notify](https://github.com/wodongx123/dsh-qq-notify) | 1 | 2026-08-17 | 2026-08-27 | QQ notifications via local NapCat for DeepSeek Harness: qq_send / qq_status / qq_napcat / qq_deploy native tools + one-click deploy scripts. QQ???? |
| 584 | [writeCasually/dsh-git](https://github.com/writeCasually/dsh-git) | 1 | 2026-08-21 | 2026-08-31 | DeepSeek Harness Git plugin — visual git status, diff, commit & file preview in the DSH web UI |
| 585 | [WSL043/dsh-deepseek-dashboard](https://github.com/WSL043/dsh-deepseek-dashboard) | 1 | 2026-08-24 | 2026-08-27 | 已归档：DeepSeek API 余额与 DSH 本地用量面板；现有 Release 保留，不再适配未来 DSH。 |
| 586 | [wszhoho/dsh-file-attachment](https://github.com/wszhoho/dsh-file-attachment) | 1 | 2026-08-28 | 2026-08-28 | 拖入 / 粘贴 / 工具栏上传按钮（📎，可多选）为输入框附加文件：图片走既有草稿图片流程（不落盘）；文档全文落盘到会话工作区 .dsh-file-attachment/ 并插入 @绝对路径引用 |
| 587 | [wtksana/dsh-font-plugin](https://github.com/wtksana/dsh-font-plugin) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Font Plugin, DSH 字体插件 |
| 588 | [xiaobai2017666/dsh-chrome-cdp](https://github.com/xiaobai2017666/dsh-chrome-cdp) | 1 | 2026-08-28 | 2026-08-31 | Chrome DevTools Protocol 插件 for DeepSeek Harness。通过 chromremote-interface 以 CDP 连接并操控 Chrome |
| 589 | [xiaochaZ/dsh-session-title-summary](https://github.com/xiaochaZ/dsh-session-title-summary) | 1 | 2026-08-25 | 2026-08-27 | DSH plugin: rolling session summary + current-task title (@xiaochaz) |
| 590 | [xiaoshi7915/dsh-kb-manager](https://github.com/xiaoshi7915/dsh-kb-manager) | 1 | 2026-08-27 | 2026-08-27 | DSH local knowledge base plugin: multi-format import, smart chunking, vector index, hybrid search (BM25 + sqlite-vec + RRF) for agent long-term memory |
| 591 | [Xichun123/dsh-relay-models](https://github.com/Xichun123/dsh-relay-models) | 1 | 2026-08-14 | 2026-08-29 | Mixed-protocol relay model discovery, metadata matching, and Web configuration for DeepSeek Harness |
| 592 | [XINY11451/dsh-wsl](https://github.com/XINY11451/dsh-wsl) | 1 | 2026-08-26 | 2026-09-02 | A model-facing WSL tool plugin for DeepSeek Harness (DSH). It lets an agent run Linux commands through wsl.exe directly — no hand-written .sh scripts or pwsh wrappers. |
| 593 | [xipian1216/dsh-aa-bridge](https://github.com/xipian1216/dsh-aa-bridge) | 1 | 2026-08-17 | 2026-08-31 | Agents Anywhere bridge and Web status plugin for DeepSeek Harness |
| 594 | [xiyunSacire/dsh-skill-manager](https://github.com/xiyunSacire/dsh-skill-manager) | 1 | 2026-08-28 | 2026-08-28 |  The dsh-skill-manager is a deep-integration Web UI plugin designed to provide developers and advanced users with direct visibility and control over the true, persistent "skill memory" of DeepSeek Harness (DSH). |
| 595 | [xjailll/dsh-portfolio-publisher](https://github.com/xjailll/dsh-portfolio-publisher) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 插件：GitHub 求职仓库一键发布助手（LLM README + Web 面板 + 一键推送） |
| 596 | [xmnathan/dsh-skin-galactic-opera](https://github.com/xmnathan/dsh-skin-galactic-opera) | 1 | 2026-08-27 | 2026-08-27 | Unofficial cinematic space-opera dark skin bundle for the DSH Web GUI. |
| 597 | [XSakura666/dsh-plugin-ChronoAgent](https://github.com/XSakura666/dsh-plugin-ChronoAgent) | 1 | 2026-08-15 | 2026-08-27 | Local-first desktop app that schedules AI agent tasks like cron jobs — zero token cost until they run. Write a task, set a time, and it runs automatically with files, web, MCP tools, and multi-model support.      |
| 598 | [yakoylp/dsh-md-convert](https://github.com/yakoylp/dsh-md-convert) | 1 | 2026-08-28 | 2026-08-28 | Convert Office documents and PDFs (incl. scanned, via CPU-first routing OCR with lightweight models: PP-DocLayout-L layout, RapidOCR text, SLANet tables, FormulaNet formulas) to structurally-formatted Markdown. CLI + dsh agent tool (md_convert). |
| 599 | [yangbobo2021/relay-dsh-plugin-manager](https://github.com/yangbobo2021/relay-dsh-plugin-manager) | 1 | 2026-08-26 | 2026-08-27 | A standalone plugin manager for DeepSeek Harness. |
| 600 | [yhbd-top/dsh-plugin-top](https://github.com/yhbd-top/dsh-plugin-top) | 1 | 2026-08-29 | 2026-08-29 | yhbd.top 插件雷达 for DeepSeek Harness：侧边栏大面板浏览 3900+ 插件目录（搜索 / 22 分类 / 站点同款五榜单 / 榜单联动分类），安装引导语一键写入会话输入框；进程内同源反代，零配置；附带 Agent 可调用的搜索与榜单工具。 |
| 601 | [yindf/taskfold](https://github.com/yindf/taskfold) | 1 | 2026-09-02 | 2026-09-02 | Keeps long coding-agent sessions lean: wrap work in named tasks and, when one is done, fold its whole span into a short titled summary. The conversation stays readable, context costs stay low, and every fold's original content can be read back on demand. For [DeepSeek Harness](https://www.npmjs.com/package/@deepseek-ai/dsh) (DSH). |
| 602 | [YINGCHAO-98/dsh-private-plugins](https://github.com/YINGCHAO-98/dsh-private-plugins) | 1 | 2026-08-25 | 2026-08-27 | 在 DeepSeek Harness Web 设置中统一导入、启用、更新和管理本地及云端私有插件。 |
| 603 | [yj-liuzepeng/dsh-project-brain](https://github.com/yj-liuzepeng/dsh-project-brain) | 1 | 2026-08-30 | 2026-08-30 | Persistent project intelligence and memory plugin for DSH: architecture analysis, cross-session context, TODOs, and optional hybrid retrieval |
| 604 | [yongshuai0314/dsh-i-have-adhd](https://github.com/yongshuai0314/dsh-i-have-adhd) | 1 | 2026-08-26 | 2026-08-27 | ADHD-friendly output shaping for DeepSeek Harness: one system-prompt section with adhd_on/adhd_off/adhd_status tools, persisted across restarts. Inspired by ayghri/i-have-adhd (MIT). |
| 605 | [yuan-source-666/dsh-github-manager](https://github.com/yuan-source-666/dsh-github-manager) | 1 | 2026-08-27 | 2026-08-27 | GitHub 仓库 AI 自动管理通道插件 (DeepSeek Harness community bundle): 27 个工具（仓库/Issue/PR/分支/文件/标签/话题/Tags/Releases/搜索）+ Web 设置卡片 + dry-run 防护 + secret 令牌。 |
| 606 | [yuan-source-666/dsh-research-autoresearch](https://github.com/yuan-source-666/dsh-research-autoresearch) | 1 | 2026-08-27 | 2026-08-27 | AutoResearch 科研协议 DSH 全家桶插件：arXiv recall + LQS 评分 + 状态持久化 + 停滞红绿灯 + 五人格中位数评审 + 可视化总控台卡片。灵感：Deli Chen "From Draft to Strong-Accept: How a Self-Play Survey Hit 8.6"。 |
| 607 | [yuan-source-666/dsh-task-notifier](https://github.com/yuan-source-666/dsh-task-notifier) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness community plugin: OS notification when a turn, subagent, background job, goal, or workflow finishes. Localized wording, per-source switches, custom delivery command. npm: dsh-task-notifier |
| 608 | [yuioi666/dsh-conversation-nav-dots](https://github.com/yuioi666/dsh-conversation-nav-dots) | 1 | 2026-08-31 | 2026-09-01 | dsh-conversation-nav-dots 在 DSH Web 对话界面的右侧添加一列导航标记。每个标记对应一条用户消息。点击即可跳转，悬停可预览所有消息内容。 |
| 609 | [yunniees/DSH-Plugin-Manager](https://github.com/yunniees/DSH-Plugin-Manager) | 1 | 2026-08-28 | 2026-08-28 | Visual plugin manager for DeepSeek Harness: AI auto-translation, AI one-click summaries, AI plugin search, one-click share & install of multiple plugins, bulk updates |
| 610 | [Yuuz12/dsh-tavily](https://github.com/Yuuz12/dsh-tavily) | 1 | 2026-08-30 | 2026-08-31 | Tavily-backed web search provider plugin for DeepSeek Harness (DSH) — multi-key balance-aware rotation with failover, manageable from the DSH web settings. |
| 611 | [yx222yx/DSH-Feedback-Bridge](https://github.com/yx222yx/DSH-Feedback-Bridge) | 1 | 2026-08-29 | 2026-08-30 | 一个 DeepSeek Harness 插件，帮助用户将功能想法和错误反馈整理为清晰、注重隐私的 GitHub Discussions。A DeepSeek Harness plugin that helps users turn ideas and bug reports into clear, privacy-aware GitHub Discussions. |
| 612 | [yybukn/dsh-table-attach](https://github.com/yybukn/dsh-table-attach) | 1 | 2026-08-31 | 2026-08-31 | 在dph中可以直接拖动.xlsx和.csv的表格文件到输入框中 |
| 613 | [yyyq0325-ai/dsh-webgate](https://github.com/yyyq0325-ai/dsh-webgate) | 1 | 2026-08-22 | 2026-08-27 | 为 DeepSeek Harness 的 Web GUI 加一道账号密码门：每次打开 DSH Web 都必须先登录；登录令牌有效期 12 小时；令牌过期被登出时，后台正在运行的任务完全不受影响，重新登录后一切还在。 |
| 614 | [yztdtf/dsh-worktable-pet](https://github.com/yztdtf/dsh-worktable-pet) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness ??????????(Dynamic Cordis Plugin) |
| 615 | [z-y-q/dsh-mcp-security](https://github.com/z-y-q/dsh-mcp-security) | 1 | 2026-09-02 | 2026-09-02 | dsh-mcp-security |
| 616 | [Zara-Siwei/dsh-float](https://github.com/Zara-Siwei/dsh-float) | 1 | 2026-08-26 | 2026-08-27 | Floating minimal-mode DeepSeek Harness (dsh) plugin: a transparent terminal TUI over dsh web in a borderless Electron window. |
| 617 | [ZBber-lab/cau-portal-open](https://github.com/ZBber-lab/cau-portal-open) | 1 | 2026-08-31 | 2026-09-01 | 农大门户（cau-portal）：中国农业大学通知公告 DSH 插件 + 爬虫/AI 加工管道（开源工具，数据由使用者自建） |
| 618 | [zenvertao/dsh-inline-comments](https://github.com/zenvertao/dsh-inline-comments) | 1 | 2026-08-26 | 2026-08-27 | 选中即批注，刷新亦留存 —— DSH 行内批注插件 |
| 619 | [zerorigin-studio/dsh-desktop-shell](https://github.com/zerorigin-studio/dsh-desktop-shell) | 1 | 2026-08-24 | 2026-09-01 | dsh desktop shell plugin |
| 620 | [zhangyqjiaoshou-oss/dsh-model-sync](https://github.com/zhangyqjiaoshou-oss/dsh-model-sync) | 1 | 2026-08-29 | 2026-08-29 | One-click / auto model sync for DeepSeek Harness providers |
| 621 | [Zhanxueyou/deepseek-balance](https://github.com/Zhanxueyou/deepseek-balance) | 1 | 2026-08-30 | 2026-08-30 | 零依赖 Python CLI 查询 DeepSeek API 余额，低余额自动提醒并发送 macOS 通知；附带 DSH 侧边栏插件，实时展示余额、今日/本月用量与缓存命中率。 |
| 622 | [Zhanxueyou/dsh-plugin-manager](https://github.com/Zhanxueyou/dsh-plugin-manager) | 1 | 2026-08-30 | 2026-08-30 | DSH Web 客户端插件管理器侧边栏面板：全量插件清单（描述/状态/来源/版本/分类）、启停热重载、删除本地自定义插件，并可浏览、搜索、一键安装 GitHub topic:dsh-plugin 远程插件。 |
| 623 | [zhaoxuejie/dsh-daily-digest](https://github.com/zhaoxuejie/dsh-daily-digest) | 1 | 2026-08-27 | 2026-08-27 | DSH 每日工作摘要插件：自动记录任务/会话/错误，一键生成日报/周报 Markdown，Web 悬浮摘要卡 |
| 624 | [zhaoxuejie/dsh-plugin-learning-path](https://github.com/zhaoxuejie/dsh-plugin-learning-path) | 1 | 2026-08-21 | 2026-08-27 | DeepSeek Harness 插件开发学习教程：15 节课程 + 4 个实战项目 + 发布课，交互式单页应用，纯 HTML/CSS/JS 零构建 |
| 625 | [Zhiyi-Zhao/dsh-notion-skill](https://github.com/Zhiyi-Zhao/dsh-notion-skill) | 1 | 2026-08-27 | 2026-08-27 | DSH (DeepSeek Harness) skill: read/write Notion workspaces via the official REST API |
| 626 | [Zhiyi-Zhao/file-brief](https://github.com/Zhiyi-Zhao/file-brief) | 1 | 2026-07-30 | 2026-08-27 | Task-local, privacy-preserving file catalogs for reusable Codex input-file understanding. |
| 627 | [zhongjie10086/dsh-adaptive-native](https://github.com/zhongjie10086/dsh-adaptive-native) | 1 | 2026-08-16 | 2026-08-30 | Windows-native Adaptive preset for DeepSeek Harness |
| 628 | [zhoupengyun572-cell/dsh-hana-research](https://github.com/zhoupengyun572-cell/dsh-hana-research) | 1 | 2026-08-28 | 2026-08-28 | A local literature review, PDF annotation, evidence synthesis, and research notes workbench for DeepSeek Harness. |
| 629 | [zhuzichen362/dsh-call-shrink](https://github.com/zhuzichen362/dsh-call-shrink) | 1 | 2026-08-29 | 2026-08-29 | dsh |
| 630 | [zjh02249/dsh-desktop-operator](https://github.com/zjh02249/dsh-desktop-operator) | 1 | 2026-08-27 | 2026-08-27 | DSH Desktop Operator: safe Windows Computer Use, desktop automation, UI Automation, and MCP tools for DeepSeek Harness |
| 631 | [Zleap-AI/dsh-sag](https://github.com/Zleap-AI/dsh-sag) | 1 | 2026-08-29 | 2026-08-29 | 面向 DeepSeek Harness 的 SAG 本地个人知识库插件，支持知识检索、原文读取、文件上传、文本写入与文档管理。 |
| 632 | [zw11591-sketch/dsh-pet-panel](https://github.com/zw11591-sketch/dsh-pet-panel) | 1 | 2026-08-28 | 2026-08-28 | A desktop pet plus a conversation overview panel for the DeepSeek Harness Web UI — self-contained client plugin (no host service) |
| 633 | [ZZZjf13960/dsh-onfail](https://github.com/ZZZjf13960/dsh-onfail) | 1 | 2026-08-28 | 2026-08-28 | DSH plugin: poll GitHub Actions, surface failed checks as cards, open a fix session with log context. |
| 634 | [01Virex/dsh-deepshub](https://github.com/01Virex/dsh-deepshub) | 0 | 2026-09-02 | 2026-09-02 | Pornhub-style parody reskin for the DeepSeek Harness web UI — orange/black pill-button theme, "Deephub" wordmark, 18+ entry gate & HD badges. Pure meme, no explicit content. |
| 635 | [1010n111/dsh-about](https://github.com/1010n111/dsh-about) | 0 | 2026-09-02 | 2026-09-02 | 为 DeepSeek Harness Web 设置面板添加“关于”页，展示当前运行的 DSH 版本、插件版本与项目主页。 |
| 636 | [123twtd/dsh-plugin-manager](https://github.com/123twtd/dsh-plugin-manager) | 0 | 2026-08-29 | 2026-08-29 | Independent DSH plugin inventory and transactional Profile manager. |
| 637 | [1710782766/dsh-browser-verify](https://github.com/1710782766/dsh-browser-verify) | 0 | 2026-09-02 | 2026-09-02 | Browser verification for DeepSeek Harness — open, mock, assert, screenshot in a few tool calls, screenshots auto-project into the model context |
| 638 | [1Ecc/dsh-lenovo-toolkit](https://github.com/1Ecc/dsh-lenovo-toolkit) | 0 | 2026-08-28 | 2026-08-28 | 联想专业工具集 · DeepSeek Harness 插件。电池健康检测（macOS/Windows）：容量、循环次数、双口径健康度、SVG 衰减趋势图与系统官方电池报告。Lenovo professional toolkit for DeepSeek Harness. |
| 639 | [2092372408-pixel/dsh-roadmap-board](https://github.com/2092372408-pixel/dsh-roadmap-board) | 0 | 2026-09-02 | 2026-09-02 | 人机共享的执行路线图看板：横向阶段→步骤、技能绑定、实时同步、跨项目复用（Human-AI shared execution roadmap board for DSH） |
| 640 | [2877905731/dsh-think-autoexpand](https://github.com/2877905731/dsh-think-autoexpand) | 0 | 2026-08-27 | 2026-08-27 | dsh-think-autoexpand：让 DeepSeek Harness 里的 Think 思考行始终可见，并在流式输出时自动展开，实时查看 Agent 完整推理过程；保留工具卡折叠体验。 |
| 641 | [618527/dsh-install-guard](https://github.com/618527/dsh-install-guard) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件安装前兼容性预检守卫：检查 Node/engines、@deepseek-ai peer 版本与 dsh 清单，可选隔离试启动。 |
| 642 | [666emmm/dsh-file-upload](https://github.com/666emmm/dsh-file-upload) | 0 | 2026-08-31 | 2026-08-31 | dsh-file-upload fork: uploaded-file management (list/info/delete/@path) + zero-copy clipboard path reading for DeepSeek Harness |
| 643 | [6jeffr3y/dsh-burpsuite-mcp](https://github.com/6jeffr3y/dsh-burpsuite-mcp) | 0 | 2026-08-30 | 2026-08-30 | Native Burp Suite MCP tools and live settings for DeepSeek Harness |
| 644 | [6jeffr3y/dsh-session-manager](https://github.com/6jeffr3y/dsh-session-manager) | 0 | 2026-08-30 | 2026-08-30 | Session archive, tagging, relationship graph and safe deletion for DeepSeek Harness Web |
| 645 | [782042369/dsh-model-compat-guard](https://github.com/782042369/dsh-model-compat-guard) | 0 | 2026-09-01 | 2026-09-02 | DSH (DeepSeek Harness) compatibility guard plugin: fixes reasoning-model compaction truncation, doomed sandbox-escalation fail-close, and missing tool description for GPT/Qwen/third-party models |
| 646 | [988hj7tczd-oss/harness-github](https://github.com/988hj7tczd-oss/harness-github) | 0 | 2026-08-23 | 2026-08-27 | DeepSeek Harness GitHub plugin: review PRs, triage issues, debug Actions CI, handle incoming GitHub events (webhooks + polling) via dsh-native tools. |
| 647 | [a1303845406/dsh-comfy-video-studio](https://github.com/a1303845406/dsh-comfy-video-studio) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的 ComfyUI MiniMax H3 视频工作台 |
| 648 | [a1303845406/dsh-sakura-theme](https://github.com/a1303845406/dsh-sakura-theme) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的晴樱与夜樱主题插件 |
| 649 | [a792883583/dsh-smart-reminder](https://github.com/a792883583/dsh-smart-reminder) | 0 | 2026-09-02 | 2026-09-02 | Smart calendar reminder & schedule assistant for DSH Web GUI: lunar calendar, holidays, system notifications on macOS/Windows, and WeCom/platform push integration. |
| 650 | [aalvsz/dsh-hermes-bridge](https://github.com/aalvsz/dsh-hermes-bridge) | 0 | 2026-08-27 | 2026-08-27 | Literal Hermes Agent → DeepSeek Harness bridge: shared memory, skills, live tools, MCP, and full-agent delegation. |
| 651 | [ABccgh/dsh-desktop-dev](https://github.com/ABccgh/dsh-desktop-dev) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness agent preset: Windows full-stack desktop development team |
| 652 | [abworks-dev/dsh-plugin-lab](https://github.com/abworks-dev/dsh-plugin-lab) | 0 | 2026-09-01 | 2026-09-01 | Workshop and lab for developing, testing, and maintaining DeepSeek Harness Cordis plugins. |
| 653 | [Aclypea/dsh-repetition-guard](https://github.com/Aclypea/dsh-repetition-guard) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 模型输出复读熔断插件 / Repetition guard plugin for DeepSeek Harness |
| 654 | [adoreQ/deepseek-balance](https://github.com/adoreQ/deepseek-balance) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness查看余额插件 |
| 655 | [ADXZXCD/dsh-web-mobile](https://github.com/ADXZXCD/dsh-web-mobile) | 0 | 2026-09-01 | 2026-09-01 | Mobile layout enhancement plugin for DeepSeek Harness Web UI |
| 656 | [Aetheri-AI/dsh-plugins](https://github.com/Aetheri-AI/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | Community plugins for DeepSeek Harness (dsh) |
| 657 | [afterDDL/dsh-creator-shared-blueprint](https://github.com/afterDDL/dsh-creator-shared-blueprint) | 0 | 2026-08-25 | 2026-09-01 | A shared interface for humans and AI to understand, discuss, modify, and extend DeepSeek Harness agents. |
| 658 | [aijunjiang/dsh-remote-ssh](https://github.com/aijunjiang/dsh-remote-ssh) | 0 | 2026-09-02 | 2026-09-02 | Run your DSH workspace on a remote host over SSH - connection sidebar, remote directory browser, per-session routing, agent ssh_exec/route-status; files and commands execute on your target while sessions, GUI and $DSH_HOME stay local. |
| 659 | [aiko-dsh-plugins/dsh-bid-studio](https://github.com/aiko-dsh-plugins/dsh-bid-studio) | 0 | 2026-08-29 | 2026-08-29 | Installable Bid Studio workbench for DeepSeek Harness |
| 660 | [aiko-dsh-plugins/dsh-ontology-kernel](https://github.com/aiko-dsh-plugins/dsh-ontology-kernel) | 0 | 2026-08-29 | 2026-08-29 | Installable Ontology Kernel bundle for DeepSeek Harness |
| 661 | [ailiasdesu/dsh-session-manager](https://github.com/ailiasdesu/dsh-session-manager) | 0 | 2026-08-28 | 2026-08-28 | DSH session migration plugin: drag-and-drop sessions between workspaces in the Web UI settings panel (auto backup/rollback, official workspaceRegistry sync) |
| 662 | [ailreth/xiaoxiao-persona-core](https://github.com/ailreth/xiaoxiao-persona-core) | 0 | 2026-08-30 | 2026-08-31 | A persona-core injection plugin for DeepSeek Harness — an honest, boundary-aware, gentle-yet-firm AI persona; an attempt at whether AI can birth consciousness. |
| 663 | [AKUSH99/dsh-balance-chip](https://github.com/AKUSH99/dsh-balance-chip) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek API balance in the DSH sidebar footer and bottom-right pill - live status dot plus amount, 60s refresh, API key stays in the local credential store |
| 664 | [alaxrpg/dsh-chatgpt-pip](https://github.com/alaxrpg/dsh-chatgpt-pip) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：ChatGPT 画中画小窗 + 把 ChatGPT 定稿计划回流到新 DSH 对话执行 |
| 665 | [alaxrpg/dsh-subagent-route-badges](https://github.com/alaxrpg/dsh-subagent-route-badges) | 0 | 2026-08-27 | 2026-08-27 | Display subagent provider, model, and reasoning effort badges in DeepSeek Harness |
| 666 | [alaxrpg/dsh-vision-bridge](https://github.com/alaxrpg/dsh-vision-bridge) | 0 | 2026-08-25 | 2026-08-27 | DSH 插件：为纯文本模型提供视觉能力，支持任意 OpenAI 兼容多模态 API |
| 667 | [Albertlsy588/dsh-release-sentinel](https://github.com/Albertlsy588/dsh-release-sentinel) | 0 | 2026-09-01 | 2026-09-01 | DSH local read-only control plugin for Release Sentinel |
| 668 | [Albertlsy588/dsh-shipgate](https://github.com/Albertlsy588/dsh-shipgate) | 0 | 2026-08-28 | 2026-08-28 | Local-first DSH pre-merge delivery receipt generator |
| 669 | [alchemistwu/dsh-tool-call-guard](https://github.com/alchemistwu/dsh-tool-call-guard) | 0 | 2026-08-30 | 2026-08-31 | DSH plugin: neutralize tool calls with invalid JSON arguments on the wire — so one malformed model generation cannot brick a session against strict OpenAI-compatible servers (vLLM) |
| 670 | [alenhu2005/dsh-usage-export](https://github.com/alenhu2005/dsh-usage-export) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin for token usage cost, PDF/Markdown transcript export, and expanded conversation statistics. |
| 671 | [alexchen5/research-epic-manager](https://github.com/alexchen5/research-epic-manager) | 0 | 2026-08-24 | 2026-08-31 | Agent skills for running research projects end-to-end using a plain-file epic→issues→comments tracker. |
| 672 | [AlgoVaultLabs/dsh-algovault](https://github.com/AlgoVaultLabs/dsh-algovault) | 0 | 2026-08-30 | 2026-08-30 | Preconfigured DeepSeek Harness bundle for the AlgoVault MCP server — composite trade calls, market regime and cross-venue funding arbitrage as mcp__algovault__* tools. |
| 673 | [alin-ever/dsh-plugin-autoqueue](https://github.com/alin-ever/dsh-plugin-autoqueue) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 无人值守任务队列插件：丢 .md 进收件箱 → AI 自动执行 → 产出报告 |
| 674 | [All3nCN/dsh-better-sidebar-N23](https://github.com/All3nCN/dsh-better-sidebar-N23) | 0 | 2026-08-31 | 2026-08-31 | DSH web plugin: complete workbench (explorer/editors/previews/terminal/git/browser/tasks) + shell refactor. Fork of omdsh-dev/DSH-better-sidebar under @all3cn scope. |
| 675 | [All3nCN/dsh-qa-suite-N23](https://github.com/All3nCN/dsh-qa-suite-N23) | 0 | 2026-09-01 | 2026-09-01 | DSH quality suite plugin: automatic tsc --noEmit diagnostics (code_check tool) + multi-lens /code-review command. Merged absorption of dsh-code-check (BSD-3) and dsh-command-code-review (MIT). |
| 676 | [alpacachen/dsh-automation](https://github.com/alpacachen/dsh-automation) | 0 | 2026-08-30 | 2026-08-30 | Schedule and manage one-time and recurring Agent tasks in DeepSeek Harness |
| 677 | [altuman-w/dsh-plugin-plantuml](https://github.com/altuman-w/dsh-plugin-plantuml) | 0 | 2026-08-31 | 2026-08-31 | deepseek harness plugin view plantuml |
| 678 | [Amoss-1/routine-taskboard](https://github.com/Amoss-1/routine-taskboard) | 0 | 2026-08-27 | 2026-08-28 | Self-contained routine board plugin for DeepSeek Harness (DSH): scheduled job placards with scripts, IO artifacts, health lamps. MIT. |
| 679 | [AnakinWu/DSH-plugin](https://github.com/AnakinWu/DSH-plugin) | 0 | 2026-08-30 | 2026-08-30 | Anakin‘s dsh-plugins |
| 680 | [andrepontesmelo/dsh-model-router](https://github.com/andrepontesmelo/dsh-model-router) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: virtual model routes with failover, exponential backoff, sleep windows |
| 681 | [andrepontesmelo/dsh-suite](https://github.com/andrepontesmelo/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | The DSH productivity suite: plugins + agent skills for the DeepSeek Harness, installable in one command. |
| 682 | [andrepontesmelo/moving-target](https://github.com/andrepontesmelo/moving-target) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: cold-start context — distills your first prompts into one goal paragraph injected into every new session |
| 683 | [Anna-la/dsh-simplify](https://github.com/Anna-la/dsh-simplify) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 界面简化插件：清理模式下右键移除页面元素，设置页中可原样恢复。 |
| 684 | [Anna-la/dsh-submodel-change](https://github.com/Anna-la/dsh-submodel-change) | 0 | 2026-08-27 | 2026-08-29 | 可以选择子 agent 调用的模型。 |
| 685 | [Anna-la/dsh-token-stat](https://github.com/Anna-la/dsh-token-stat) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness token 用量统计插件: 按模型/日期区分, 设置页看板, 数据目录在线更改 |
| 686 | [AnonyJcy/dsh-plugin-j-space](https://github.com/AnonyJcy/dsh-plugin-j-space) | 0 | 2026-08-23 | 2026-08-27 | J-Space Cognition Suite V3.7 原生 DeepSeek Harness 智能体预设与独立 Cordis 插件，提供深层推理路由、工作区状态外化账本（.jspace）与全模型解耦的认知工作空间 |
| 687 | [AnonyJcy/dsh-plugin-mobile-touch](https://github.com/AnonyJcy/dsh-plugin-mobile-touch) | 0 | 2026-08-27 | 2026-08-28 | Mobile & iPad touch optimization plugin for DeepSeek Harness Web GUI |
| 688 | [Ansonfishing/dsh-model-manager](https://github.com/Ansonfishing/dsh-model-manager) | 0 | 2026-08-28 | 2026-08-28 | Manage local LLM inference servers in DSH: GPU registry, parameter profiles, VRAM validation, and tok/s benchmarks for llama.cpp, SGLang, and vLLM |
| 689 | [Anyway-one/dsh-balance](https://github.com/Anyway-one/dsh-balance) | 0 | 2026-08-26 | 2026-08-27 | 为 DeepSeek Harness 提供持久化的余额与用量显示插件，让您随时掌握资源消耗情况，无需离开工作区。 |
| 690 | [Army1900/dsh-e2e-dev-sdd](https://github.com/Army1900/dsh-e2e-dev-sdd) | 0 | 2026-08-26 | 2026-08-27 | dsh插件，用于驱动定制的e2e开发 |
| 691 | [ArmyWas/dsh-provider-passport](https://github.com/ArmyWas/dsh-provider-passport) | 0 | 2026-09-01 | 2026-09-01 | Review-first request-dialect preflight for custom DeepSeek Harness providers. |
| 692 | [asdasdsdsdasdasdasd/dsh-computer-use](https://github.com/asdasdsdsdasdasdasd/dsh-computer-use) | 0 | 2026-08-25 | 2026-08-29 | Linux X11 computer-use for DeepSeek Harness: screenshot, mouse, keyboard via a zero-dependency Python XTest helper — no Node native modules, no accessibility framework. |
| 693 | [ash-qw/dsh-theme-prts](https://github.com/ash-qw/dsh-theme-prts) | 0 | 2026-08-31 | 2026-09-02 | Unofficial personal non-commercial Arknights P.R.T.S. fan UI for DeepSeek Harness |
| 694 | [AstralFoundry/dsh-workspace](https://github.com/AstralFoundry/dsh-workspace) | 0 | 2026-08-27 | 2026-08-27 | A lightweight IDE and Git workspace plugin for DeepSeek Harness |
| 695 | [auggie246/dsh-llm-openai-codex](https://github.com/auggie246/dsh-llm-openai-codex) | 0 | 2026-08-19 | 2026-09-01 | OpenAI Codex (ChatGPT Plus/Pro subscription) LLM provider for the DeepSeek Harness — OAuth tokens from the Codex CLI, no API key required |
| 696 | [auggie246/dsh-mattpocock-skills](https://github.com/auggie246/dsh-mattpocock-skills) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to install Mattpocock skills. |
| 697 | [auggie246/dsh-output-styles](https://github.com/auggie246/dsh-output-styles) | 0 | 2026-08-28 | 2026-08-28 | Enable output styles in Deepseek Harness settings! |
| 698 | [auggie246/dsh-sidebar](https://github.com/auggie246/dsh-sidebar) | 0 | 2026-08-27 | 2026-08-28 | Sidebar and panels for full developer interaction! |
| 699 | [auggie246/dsh-synthetic-web-search](https://github.com/auggie246/dsh-synthetic-web-search) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to use synthetic.new web search instead of built-in Deepseek web search |
| 700 | [avdergh/chroma-cut](https://github.com/avdergh/chroma-cut) | 0 | 2026-08-28 | 2026-08-28 | Preserve anti-aliased outlines while cutting chroma-backed game assets. CLI + MCP + Codex plugin. |
| 701 | [awol2005ex3/dsh-export-session](https://github.com/awol2005ex3/dsh-export-session) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness（`dsh`）插件：把**当前会话的完整内容**一键导出为 **Markdown（`.md`）/ Word（`.docx`）/ PDF（`.pdf`）**。 |
| 702 | [awol2005ex3/dsh-logo-custom](https://github.com/awol2005ex3/dsh-logo-custom) | 0 | 2026-08-31 | 2026-09-01 | DeepSeek Harness 自定义 Logo 插件 — 上传图片替换侧边栏左上角的品牌图标和文字。 |
| 703 | [awol2005ex3/dsh-md-table-export](https://github.com/awol2005ex3/dsh-md-table-export) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（`dsh`）插件：把对话内容里的 **Markdown 表格** 一键导出为 **Excel（`.xlsx`）**。 |
| 704 | [awol2005ex3/dsh-role-manager](https://github.com/awol2005ex3/dsh-role-manager) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（dsh）角色管理插件。为每个"角色"预设一份初始系统提示词，在 Web 界面中切换当前角色，从而让模型以不同的身份 / 设定开始对话。 |
| 705 | [awol2005ex3/dsh-user-manager](https://github.com/awol2005ex3/dsh-user-manager) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness（`dsh`）插件：为单机的 harness 增加**用户管理**与**会话按用户隔离**。 |
| 706 | [axdlee/dsh-yeelight-smart-home](https://github.com/axdlee/dsh-yeelight-smart-home) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: Yeelight smart home control via the local yeelight-home runtime (skill, tools, settings card) |
| 707 | [axel286137079-dot/dsh-skill-matcher](https://github.com/axel286137079-dot/dsh-skill-matcher) | 0 | 2026-09-01 | 2026-09-01 | Skill & Expert Matcher for DeepSeek Harness (dsh plugin) |
| 708 | [ayumedaze/dsh-git](https://github.com/ayumedaze/dsh-git) | 0 | 2026-08-29 | 2026-08-29 | dsh-plugin |
| 709 | [Azonda/dsh-whale-writing](https://github.com/Azonda/dsh-whale-writing) | 0 | 2026-08-30 | 2026-08-31 | 老人与大肥鱼：Deepseek Harness超级写作增强插件，具备四种风格和五种写作严谨度的自动切换功能，并且具备任务级本地记忆和去ai味后处理、。 |
| 710 | [bailong-Hakuryu/dsh-engineering-control-plane](https://github.com/bailong-Hakuryu/dsh-engineering-control-plane) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 工程任务编排与发布门禁插件，支持 /mission 指令、任务路由、计划执行、验证和状态跟踪。 \| Engineering mission orchestration and release-gate plugin for DeepSeek Harness with /mission routing, planning, execution, verification, and status tracking. |
| 711 | [bailong-Hakuryu/dsh-security-assurance](https://github.com/bailong-Hakuryu/dsh-security-assurance) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 策略驱动的仓库安全评估插件，支持包生命周期评估、证据、发现、裁决、导出和 /security 指令。 \| Policy-driven repository security assurance plugin for DeepSeek Harness with package lifecycle assessments, evidence, findings, verdicts, exports, and /security routing. |
| 712 | [baiyang123/dsh-audit-missing](https://github.com/baiyang123/dsh-audit-missing) | 0 | 2026-08-27 | 2026-08-28 | 对照开发计划等文档，当AI开发完一个迭代之后扫描是否有漏开发的功能（真的好用） |
| 713 | [BaoBao1996121/dsh-restart-ui](https://github.com/BaoBao1996121/dsh-restart-ui) | 0 | 2026-08-28 | 2026-08-28 | One-click cross-platform restart button for DeepSeek Harness Web UI |
| 714 | [BaronCyrus/dsh-kimi-subscription](https://github.com/BaronCyrus/dsh-kimi-subscription) | 0 | 2026-08-28 | 2026-08-28 | Use a Kimi Code subscription in DeepSeek Harness with OAuth, quota display, and composer usage |
| 715 | [BarrierFly/apx-watchdog](https://github.com/BarrierFly/apx-watchdog) | 0 | 2026-08-26 | 2026-08-27 | 牛来写的东西 |
| 716 | [Barry-Liu-001/dsh_ark_plan_usage](https://github.com/Barry-Liu-001/dsh_ark_plan_usage) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 侧边栏插件：实时展示火山方舟 Agent Plan 用量（5h/周/月），数据来自本机 arkcli |
| 717 | [Barry-Liu-001/dsh_chat_index](https://github.com/Barry-Liu-001/dsh_chat_index) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 对话索引插件：在对话区右边缘显示一列小圆点，每个点代表一条用户发送的消息。圆点等间距、紧凑、纵向居中排列（消息过多放不下时间距自动压缩以适应高度）；当前阅读位置的点高亮为品牌色。 |
| 718 | [bbboy31/dsh-terminal-tabs](https://github.com/bbboy31/dsh-terminal-tabs) | 0 | 2026-08-26 | 2026-08-27 | Terminals view tab for DeepSeek Harness web UI — live background job count, streaming output, one-click kill |
| 719 | [benz-ai-x/dsh-md-preview](https://github.com/benz-ai-x/dsh-md-preview) | 0 | 2026-09-01 | 2026-09-01 | DSH (DeepSeek Harness) Web GUI plugin — preview, edit & browse workspace markdown/text files right beside the chat: rich preview panel, guarded editing with conflict detection, lazy workspace file tree. 预览/编辑/浏览会话工作区文档 |
| 720 | [benz-ai-x/dsh-session-graph](https://github.com/benz-ai-x/dsh-session-graph) | 0 | 2026-08-28 | 2026-08-30 | Visual session graph for DeepSeek Harness — browse, arrange, branch, merge, and summarize AI agent sessions on an interactive canvas. |
| 721 | [berserk0501/dsh-soundscape](https://github.com/berserk0501/dsh-soundscape) | 0 | 2026-08-26 | 2026-08-27 | DSH 本机思考与工具音效插件，支持 MediaPlayer、WAV/MP3、自定义映射和设置面板 |
| 722 | [Bigesila-B/dsh-media-forge](https://github.com/Bigesila-B/dsh-media-forge) | 0 | 2026-08-26 | 2026-08-27 | DSH Media Forge plugin: agent + skills workflow for media-generation APIs, with a sidebar skill panel (zh/en docs) |
| 723 | [bigharm/dsh-agentnoodle](https://github.com/bigharm/dsh-agentnoodle) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness 插件：AI 驱动的群像聊天游戏框架。轻量化酒馆。兼容 SillyTavern V1/V2/V3 JSON 和 PNG 内嵌卡片。添加npc和场景之类的，给harness提要求，让它做就行。玩家输入一个行动，场景中多个 NPC 各自做出反应，每条反应独立成一条带头像插图的聊天室消息；支持场景切换、NPC 关系变化与本地 JSON 存档。 |
| 724 | [BiKing567/dsh-subagent-panel](https://github.com/BiKing567/dsh-subagent-panel) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：把每个子代理渲染成主对话里可点击的卡片，点击直接进入子代理会话（与标题栏同一路径）。\| DSH plugin: render every subagent as a clickable inline card that opens the child session — same navigation the header's subagent catalog uses. |
| 725 | [BISTU-guheihei/DSH-SessionManager](https://github.com/BISTU-guheihei/DSH-SessionManager) | 0 | 2026-08-26 | 2026-08-27 | DSH 会话管理工具：可视化/命令行查看与删除历史聊天记录，自动清理缓存残留 |
| 726 | [BitDG/dsh-cloud-model-providers](https://github.com/BitDG/dsh-cloud-model-providers) | 0 | 2026-09-01 | 2026-09-01 | 接入 Ant Digital MaaS 与 NVIDIA NIM 流式模型路由 / Streaming model routes for DSH |
| 727 | [bitterSmilezzz/dsh-asr-voice](https://github.com/bitterSmilezzz/dsh-asr-voice) | 0 | 2026-08-25 | 2026-08-27 | 开口即成文 · Speak-to-prompt for DeepSeek Harness：云端 ASR 语音识别 + 提示词优化 + 填入草稿/自动发送，跨平台 macOS / Windows。 |
| 728 | [bitterSmilezzz/dsh-model-selector](https://github.com/bitterSmilezzz/dsh-model-selector) | 0 | 2026-08-27 | 2026-09-01 | DeepSeek Harness (DSH) 的增强模型选择器：单层菜单（搜索 + 分组）+ 底部内联推理强度（Effort）滑杆。 |
| 729 | [blairlaird/dsh-agent-mailbox](https://github.com/blairlaird/dsh-agent-mailbox) | 0 | 2026-09-01 | 2026-09-01 | Durable agent-to-agent messaging for DeepSeek Harness: threads, receipts, search, broadcast, attachments, presence, SSE streaming, signing. Zero dependencies. |
| 730 | [bleakbelladonnals/dsh-artifact-harbor](https://github.com/bleakbelladonnals/dsh-artifact-harbor) | 0 | 2026-08-27 | 2026-08-27 | Artifact Harbor — secure, session-aware artifact previews for DeepSeek Harness Web |
| 731 | [bleakbelladonnals/dsh-echo](https://github.com/bleakbelladonnals/dsh-echo) | 0 | 2026-08-27 | 2026-08-27 | Record MCP once. Replay it safely inside DeepSeek Harness. |
| 732 | [bleamayaka/dsh-file-beam](https://github.com/bleamayaka/dsh-file-beam) | 0 | 2026-08-27 | 2026-08-27 | dsh-file-beam - DSH plugin: drag files into the web composer, resolve real absolute paths, hidden path injection for the agent (no copy, no path in composer). |
| 733 | [bLueriVerLHR/dsh-better-webui](https://github.com/bLueriVerLHR/dsh-better-webui) | 0 | 2026-08-20 | 2026-08-27 | Minimal improvement if possible. |
| 734 | [bo961386926/dolphin-pet-plugin](https://github.com/bo961386926/dolphin-pet-plugin) | 0 | 2026-08-26 | 2026-08-27 | Cute desktop pet for DeepSeek Harness - custom name, upload your own pet image, or generate one with AI. DSH 桌面宠物插件 |
| 735 | [bosinHU/dsh-skill-editor](https://github.com/bosinHU/dsh-skill-editor) | 0 | 2026-08-29 | 2026-08-30 | Edit skills directly in DSH web settings |
| 736 | [BoWuGit/dsh-reasoning](https://github.com/BoWuGit/dsh-reasoning) | 0 | 2026-08-31 | 2026-08-31 | Codex-style /reasoning command for DeepSeek Harness Web |
| 737 | [Britneycode/dsh-distillery](https://github.com/Britneycode/dsh-distillery) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：本地蒸馏器——扫历史会话挖「用户纠错 → 改对」片段，脱敏后蒸馏成微调 JSONL / SKILL.md 技能草稿 / AGENTS.md 规则补丁，带人工审核队列 |
| 738 | [Britneycode/dsh-live-room](https://github.com/Britneycode/dsh-live-room) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：把会话变成免登录、只读、可分享的实时直播间（SSE 观看页 + 弹幕 + agent 工具） |
| 739 | [Bronier/dsh-web-search-so360](https://github.com/Bronier/dsh-web-search-so360) | 0 | 2026-08-27 | 2026-08-27 | Keyless web search provider for DeepSeek Harness backed by 360 Search (so.com). |
| 740 | [bvcvb/dsh-baize-rules](https://github.com/bvcvb/dsh-baize-rules) | 0 | 2026-08-31 | 2026-09-01 | dsh plugin: user-set session/global must-do & must-not requirements injected at conversation start (Baize). |
| 741 | [bycall/dsh-code-collector](https://github.com/bycall/dsh-code-collector) | 0 | 2026-08-27 | 2026-08-27 | Session code collector for DeepSeek Harness: gather every code block the model produced in the current session, grouped by language, with copy / download-all / jump-to-turn. |
| 742 | [ByxHuster/DSH-Paper-Highlighting-Agent](https://github.com/ByxHuster/DSH-Paper-Highlighting-Agent) | 0 | 2026-08-27 | 2026-08-27 | An interactive and customized paper highlighting tool built upon Deepseek Harness (DSH), still under development. |
| 743 | [c0nfident/github-slideshow](https://github.com/c0nfident/github-slideshow) | 0 | 2020-07-07 | 2026-08-30 | A robot powered training repository :robot: |
| 744 | [CagierAsh123/dsh-obsidian-agent-wiki](https://github.com/CagierAsh123/dsh-obsidian-agent-wiki) | 0 | 2026-08-26 | 2026-08-27 | Searchable SQLite-indexed Obsidian memory for DeepSeek Harness |
| 745 | [Calvin451970353/dsh-vmic](https://github.com/Calvin451970353/dsh-vmic) | 0 | 2026-08-25 | 2026-08-27 | Voice input plugin for DeepSeek Harness: mic button, 16kHz WAV recording, ASR via Xiaomi MiMo / Volcengine Doubao (live), optional LLM polish. |
| 746 | [CanaryJing/dsh-big-fat-whale-maid-adaptive](https://github.com/CanaryJing/dsh-big-fat-whale-maid-adaptive) | 0 | 2026-08-23 | 2026-08-27 | 大肥鱼女仆长智能体，用风神与明神插件vibe而来，解决wsl与windows互通问题 |
| 747 | [Castem114/dsh-visioncraft](https://github.com/Castem114/dsh-visioncraft) | 0 | 2026-08-26 | 2026-08-27 | 为 DeepSeek Harness（DSH）Web 量身打造的双插件扩展，为纯文本模型补齐"视觉"短板 |
| 748 | [cayan0x/dsh-fold-context](https://github.com/cayan0x/dsh-fold-context) | 0 | 2026-08-28 | 2026-08-28 | Auto-fold context/system messages in DSH — collapse think blocks, tool calls, and tool results into grouped expandable bars. |
| 749 | [ccr-wer/dsh-dolphin-security](https://github.com/ccr-wer/dsh-dolphin-security) | 0 | 2026-09-01 | 2026-09-01 | 集扫描、远程执行、报告于一体的 DSH 主动安全巡逻插件，基于 SSH + Semgrep |
| 750 | [cczzyy-cn/dsh-ui-screenshot](https://github.com/cczzyy-cn/dsh-ui-screenshot) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness 的 Web 插件：在输入框添加截图按钮，截屏并作为草稿图片插入，仅当模型支持视觉时显示。 |
| 751 | [cczzyy-cn/subagent-model-picker](https://github.com/cczzyy-cn/subagent-model-picker) | 0 | 2026-09-02 | 2026-09-02 | 让主会话模型从「已配置模型」里自主选择子代理运行模型，并把选定路由通过 ctx.subagents 的 request.agentOptions.provider/model 显式覆盖到子代理上。 |
| 752 | [CDeZT/better-basicfun](https://github.com/CDeZT/better-basicfun) | 0 | 2026-09-01 | 2026-09-01 | Native DSH default workspace with complete paged read-only access to plugins, skills, memory, sessions, storage, settings, credentials, and DSH_HOME files. |
| 753 | [Centaurea5547196/dsh-page-zoom](https://github.com/Centaurea5547196/dsh-page-zoom) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness Web UI ??????:????? + Ctrl+??/Ctrl+=/-/0 ???,25%-300%,?????? |
| 754 | [ch3vr0n5/dsh-docker-services](https://github.com/ch3vr0n5/dsh-docker-services) | 0 | 2026-08-26 | 2026-08-27 | Portable DeepSeek Harness plugin for securely monitoring and operating Docker services |
| 755 | [chai1110/dsh-ssh-remote](https://github.com/chai1110/dsh-ssh-remote) | 0 | 2026-08-20 | 2026-09-01 | DeepSeek Harness SSH 远程工作区插件（多机并行）：同时连接多台服务器，Agent 直接查看/编辑/执行远程文件。基于 flymysql/dsh-remote (MIT) 适配 0.1.1-rc.2 |
| 756 | [changyinliangbaikai/dsh-b2us-schedule](https://github.com/changyinliangbaikai/dsh-b2us-schedule) | 0 | 2026-08-29 | 2026-08-30 | dsh定时任务插件，支持延迟、固定间隔、cron表达式，支持执行shell命令，支持发起Agent会话 |
| 757 | [Che-Year/dsh-pet-lulu](https://github.com/Che-Year/dsh-pet-lulu) | 0 | 2026-08-26 | 2026-08-27 | A cute terminal and web pet plugin for DeepSeek Harness (dsh), using assets from lulu and capybara projects. |
| 758 | [Cheeserackery/deepseek-time](https://github.com/Cheeserackery/deepseek-time) | 0 | 2026-08-18 | 2026-08-28 | 一款Agent插件，能够实时直观显示DeepSeek当前收费时段状态。DeepSeek pricing-period status indicator with Hermes, DSH, and Codex adapters. |
| 759 | [chemmy-11/dsh-nexus](https://github.com/chemmy-11/dsh-nexus) | 0 | 2026-08-24 | 2026-08-31 | Vault observation plugin for DeepSeek Harness: Obsidian vault metadata snapshot + edit stats + observation panel |
| 760 | [chen70456-lang/dsh-tmwebdriver](https://github.com/chen70456-lang/dsh-tmwebdriver) | 0 | 2026-08-30 | 2026-08-30 | One tool, infinite reach: arbitrary JS in your real logged-in browser. Unlike fixed-action plugins, browser_execute_js does anything DevTools can — read, click, type, fill, navigate, screenshot, CDP. Plus list_tabs/snapshot/type. Zero-setup, self-healing. |
| 761 | [chendefine/dsh-sidebar-onlyoffice](https://github.com/chendefine/dsh-sidebar-onlyoffice) | 0 | 2026-08-24 | 2026-08-27 | DSH web plugin: open and edit .docx/.xlsx/.pptx in the better-sidebar editor through a self-hosted ONLYOFFICE Document Server (JWT-signed config, atomic save-back, live refresh on AI edits) |
| 762 | [chendefine/dsh-sidebar-superdoc-docx](https://github.com/chendefine/dsh-sidebar-superdoc-docx) | 0 | 2026-09-01 | 2026-09-01 | DSH web plugin: open and edit .docx in the better-sidebar via SuperDoc — self-hosted, offline-capable, atomic saves |
| 763 | [chendefine/dsh-sidebar-vscode](https://github.com/chendefine/dsh-sidebar-vscode) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: a better-sidebar tab embedding the VS Code web workbench at the session workspace; editor selections and explorer files land as atomic reference chips |
| 764 | [chenyangcun/dsh-command-palette](https://github.com/chenyangcun/dsh-command-palette) | 0 | 2026-08-30 | 2026-08-30 | A keyboard-first command palette for standard DeepSeek Harness |
| 765 | [chenyangcun/dsh-fixed-new-session-model](https://github.com/chenyangcun/dsh-fixed-new-session-model) | 0 | 2026-08-30 | 2026-08-30 | 为 DSH 固定新会话的默认 Agent 预设与模型，支持全局默认设置和工作区独立配置。 |
| 766 | [Choco-Zz/dsh-image-amnesia](https://github.com/Choco-Zz/dsh-image-amnesia) | 0 | 2026-08-31 | 2026-08-31 | Drop historical images before DeepSeek Harness relay requests; keep native vision on the newest image. |
| 767 | [chocobo77/dsh-infinite-context](https://github.com/chocobo77/dsh-infinite-context) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: multi-tier memory management, semantic retrieval, structured memory, and model-context awareness for infinite context. |
| 768 | [chouyulanxia114514/dsh-uisketch](https://github.com/chouyulanxia114514/dsh-uisketch) | 0 | 2026-08-28 | 2026-08-28 | UI Sketch to AI 画板编辑器 × DSH 插件：侧栏开关 + 全屏 iframe 浮层，开箱即用 |
| 769 | [chris-003/dsh-agent-in-browser](https://github.com/chris-003/dsh-agent-in-browser) | 0 | 2026-08-31 | 2026-08-31 | Let a DeepSeek Harness agent see and control your browser in real time — read, screenshot, navigate, click, and manage tabs via tool calls. |
| 770 | [CHristianREEVEE/dsh-xiuxian-world](https://github.com/CHristianREEVEE/dsh-xiuxian-world) | 0 | 2026-08-28 | 2026-08-28 | 云仙大世界 — a living xiuxian world for DeepSeek Harness agents: enter, cultivate, and export a self-contained HTML replay of your journey |
| 771 | [chucan1/dsh-plugin-xt-memory](https://github.com/chucan1/dsh-plugin-xt-memory) | 0 | 2026-09-01 | 2026-09-02 | Cross-session self-learning memory for DeepSeek Harness, ported from XT-AGENT packages/memory. BM25 relevance injection + background extraction (sanitize/dedupe/merge) + lifecycle archive + memory_read/memory_search/memory_write tools. |
| 772 | [classic-takeoff/DSH_plugins](https://github.com/classic-takeoff/DSH_plugins) | 0 | 2026-08-31 | 2026-08-31 | some plugins for dsh |
| 773 | [cloveric/deepseek-harness-web-search-plugin](https://github.com/cloveric/deepseek-harness-web-search-plugin) | 0 | 2026-08-29 | 2026-08-29 | Source-traceable Brave + Tavily live web search and URL extraction for DeepSeek Harness. Native DSH plugin; TaroCub optional. |
| 774 | [CMD128/dsh-wx-bridge](https://github.com/CMD128/dsh-wx-bridge) | 0 | 2026-09-02 | 2026-09-02 | 微信桥接 DSH 插件：扫码绑定官方 ClawBot（iLink 协议），私聊驱动 DeepSeek Harness 会话 — WeChat bridge plugin for DSH |
| 775 | [cndn/dsh-d1](https://github.com/cndn/dsh-d1) | 0 | 2026-09-02 | 2026-09-02 | Cloudflare D1 tools for the DeepSeek Harness (dsh): read-only first, approval-gated writes, zero runtime dependencies |
| 776 | [Cooberped/dsh-evidence](https://github.com/Cooberped/dsh-evidence) | 0 | 2026-08-28 | 2026-08-28 | Turn local files into versioned evidence in DeepSeek Harness: composer upload, private local retrieval, and coordinate-exact PDF/DOCX/XLSX/PPTX reads. |
| 777 | [coolgech/dsh-siyuan](https://github.com/coolgech/dsh-siyuan) | 0 | 2026-08-27 | 2026-08-27 | A plugin for deepseek harnes that operates on the notes of Siyuan. |
| 778 | [csustyang/dsh-garmin-coach](https://github.com/csustyang/dsh-garmin-coach) | 0 | 2026-08-27 | 2026-08-31 | Garmin Connect 运动健康 AI 教练插件 for DeepSeek Harness |
| 779 | [CultOfLuna/dsh-vision-autoswitch](https://github.com/CultOfLuna/dsh-vision-autoswitch) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek 的"自动挡"：有图切 Vision，无图回 Pro/Flash，一键都不用点。 DeepSeek's "automatic transmission": image in → Vision, image out → back to Pro/Flash — not a single click. |
| 780 | [CyberFox-lab/dsh-rss](https://github.com/CyberFox-lab/dsh-rss) | 0 | 2026-08-30 | 2026-08-30 | RSS/Atom reader and Agent tools plugin for DeepSeek Harness |
| 781 | [cyjyyd/dsh-llm-xai-oauth](https://github.com/cyjyyd/dsh-llm-xai-oauth) | 0 | 2026-08-27 | 2026-08-27 | Native SuperGrok / X Premium OAuth provider for DeepSeek Harness. Reuses local grok-bridge tokens; no xAI API key. |
| 782 | [d3vmeh/dsh-context-budget](https://github.com/d3vmeh/dsh-context-budget) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: keep a local model's context at a size your GPU handles well (measured prefill speed, hard ceiling, early compaction) |
| 783 | [d4551/DeepTail](https://github.com/d4551/DeepTail) | 0 | 2026-09-01 | 2026-09-02 | A Tauri 2 client — desktop, iOS, and Android — that connects to DeepSeek Harness hosts and gives you one control plane over the agent sessions running on all of them. |
| 784 | [daveycodez/dsh-llm-agent-bridge](https://github.com/daveycodez/dsh-llm-agent-bridge) | 0 | 2026-08-26 | 2026-08-27 | Claude as a selectable LLM provider in DeepSeek Harness, via Anthropic's official Claude Agent SDK. Works in any DSH mode. |
| 785 | [david0702/dsh-cost](https://github.com/david0702/dsh-cost) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) 对话底部费用显示插件：按每笔请求时间+模型分批计费，分时段明细，模型归属，读图金额，余额。 |
| 786 | [Dayi-Z/gitcompass](https://github.com/Dayi-Z/gitcompass) | 0 | 2026-08-28 | 2026-08-29 | GitHub-connected visual git panel for DeepSeek Harness - branch switcher, file-level approval cards, PR/issue workspace |
| 787 | [Dee3526/dsh-plugin-trtc-conai](https://github.com/Dee3526/dsh-plugin-trtc-conai) | 0 | 2026-08-31 | 2026-08-31 | Tencent RTC Conversational AI (ConAI) voice agent tools for the DeepSeek Harness |
| 788 | [DeepseekHarnessPlugins/Notification](https://github.com/DeepseekHarnessPlugins/Notification) | 0 | 2026-08-26 | 2026-08-27 | DeepseekHarnessPlugin |
| 789 | [delicious28/wuming-books-mcp](https://github.com/delicious28/wuming-books-mcp) | 0 | 2026-08-28 | 2026-08-31 | Free remote MCP server for searching 680K+ Chinese books with Douban ratings, AI reading guides and curated toplists. No API key. |
| 790 | [demacia1314/dsh-remote-deliver](https://github.com/demacia1314/dsh-remote-deliver) | 0 | 2026-08-27 | 2026-08-27 | 🚀 告别繁琐 SCP！远程部署 DSH 一键下载修改后的文件与图片预览交付插件 |
| 791 | [Demigod-cyber/dsh-angelina-theme](https://github.com/Demigod-cyber/dsh-angelina-theme) | 0 | 2026-08-26 | 2026-08-27 | DSH主题插件——直到大地变成一颗酸橙（Angelina 浅蓝主题） |
| 792 | [dengyier/openworkproof-dsh-plugin](https://github.com/dengyier/openworkproof-dsh-plugin) | 0 | 2026-08-30 | 2026-08-30 | Community DeepSeek Harness plugin for verifiable AI agent authorization, execution evidence, and offline delivery verification |
| 793 | [dennisrongo/dsh-plugins](https://github.com/dennisrongo/dsh-plugins) | 0 | 2026-08-23 | 2026-08-27 | Dennis Rongo's plugin collection for DeepSeek Harness (dsh)  |
| 794 | [DepressionL/fortune-assistant](https://github.com/DepressionL/fortune-assistant) | 0 | 2026-08-28 | 2026-08-30 | dsh算命插件 |
| 795 | [dfhxxc666/dsh-llm-mimo](https://github.com/dfhxxc666/dsh-llm-mimo) | 0 | 2026-08-27 | 2026-08-27 | Xiaomi MiMo v2.5 adapter for DeepSeek Harness — fixed fork (sanitize tool args, dsh-llm 0.1.1-rc.2, prepareCall, keepalive) |
| 796 | [difimim/dsh-voice-input](https://github.com/difimim/dsh-voice-input) | 0 | 2026-08-29 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 797 | [dingminhua/dsh-connect-trae](https://github.com/dingminhua/dsh-connect-trae) | 0 | 2026-08-28 | 2026-08-28 | Connect locally signed-in Trae models to DeepSeek Harness with a read-only credits overview. |
| 798 | [dingxin-tech/dsh-maxcompute](https://github.com/dingxin-tech/dsh-maxcompute) | 0 | 2026-08-31 | 2026-08-31 | DSH (DeepSeek Harness) plugin for MaxCompute (ODPS): metadata browsing, cost-gated SQL execution, background jobs and result export. |
| 799 | [djs326/dsh-titlebar-feed](https://github.com/djs326/dsh-titlebar-feed) | 0 | 2026-08-30 | 2026-08-31 | DSH Desktop 标题栏信息条插件：修复 Windows 无边框标题栏遮挡，提供可配置信息条（静态文本 / HTTP 接口 / JS 函数 / 系统指标），支持分页、动态切换与快捷键。npm: dsh-titlebar-feed |
| 800 | [DobyChao/dsh-workspace-enhancement](https://github.com/DobyChao/dsh-workspace-enhancement) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness plugin: local and remote (SSH) workspaces in one place. Remote execution uses a single SSH connection (multi-hop jumps allowed); bash, files, PTY, and LSP share that link. |
| 801 | [doer1296/dsh-plugin-voice](https://github.com/doer1296/dsh-plugin-voice) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 语音插件：火山 seed-tts 云端 TTS（自动回退 SAPI/Huihui 离线）+ 桌面通知 + 场景化 WAV 提示音 + 提问自动呼叫。DSH 原生集成，零 Python 依赖，Windows 原生。 |
| 802 | [dongsheng123132/dsh-break-glass-settlement-proof](https://github.com/dongsheng123132/dsh-break-glass-settlement-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed DSH proof for break-glass session settlement evidence |
| 803 | [dongsheng123132/dsh-change-window-proof](https://github.com/dongsheng123132/dsh-change-window-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed DSH proof for change-window settlement evidence |
| 804 | [dongsheng123132/dsh-credential-retirement-proof](https://github.com/dongsheng123132/dsh-credential-retirement-proof) | 0 | 2026-08-26 | 2026-08-27 | Evidence-only DSH plugin for credential retirement settlement |
| 805 | [dongsheng123132/dsh-duty-separation-proof](https://github.com/dongsheng123132/dsh-duty-separation-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed duty-separation evidence for supplied DSH workflow receipts |
| 806 | [dongsheng123132/dsh-license-obligation-proof](https://github.com/dongsheng123132/dsh-license-obligation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for license obligation delivery closure |
| 807 | [dongsheng123132/dsh-vulnerability-remediation-proof](https://github.com/dongsheng123132/dsh-vulnerability-remediation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for vulnerability remediation closure |
| 808 | [donoteatme/dsh-local-link](https://github.com/donoteatme/dsh-local-link) | 0 | 2026-08-27 | 2026-08-28 | Lightweight DeepSeek Harness plugin for paired LAN access: scan a QR code and continue the current DSH Web session from any phone, tablet, or computer. |
| 809 | [Doozqoo/dsh-pixel-office](https://github.com/Doozqoo/dsh-pixel-office) | 0 | 2026-08-27 | 2026-09-01 |  DeepSeek Harness Web GUI |
| 810 | [DoshinJiu/dsh-ui-boost](https://github.com/DoshinJiu/dsh-ui-boost) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness界面调色插件/RGB滑块调色 |
| 811 | [dsh-plugins/dsh-plugin-market](https://github.com/dsh-plugins/dsh-plugin-market) | 0 | 2026-08-26 | 2026-08-27 | A structured plugin marketplace for DeepSeek Harness — each plugin described as JSON, auto-aggregated into a single plugins.json for the dsh-plugins.github.io site. DeepSeek Harness 结构化插件市场 —— 每个插件以 JSON 描述，自动聚合为单一 plugins.json 供 dsh-plugins.github.io 站点消费。 |
| 812 | [du-u-uck/DSH-Transparent-UI-Plugin](https://github.com/du-u-uck/DSH-Transparent-UI-Plugin) | 0 | 2026-09-01 | 2026-09-02 | DeepSeek Harness UI Aqua玻璃质感主题主题，在原作者基础上对“0.1.1-rc.2”版本进行适配 |
| 813 | [dusbin/dsh-attention](https://github.com/dusbin/dsh-attention) | 0 | 2026-08-30 | 2026-08-30 | 任务完成后进行提醒，发完任务就可以去喝杯咖啡了，完成了会叫你的 |
| 814 | [dusbin/voice-plugin](https://github.com/dusbin/voice-plugin) | 0 | 2026-08-27 | 2026-08-27 | Dsh(deepseek harness)语音输入插件 Ps: 朗读功能目前还不是很棒。 |
| 815 | [dxsdyhm/dsh-adb-logcat](https://github.com/dxsdyhm/dsh-adb-logcat) | 0 | 2026-08-26 | 2026-08-27 | Android Studio-style ADB logcat viewer for the DSH Web GUI |
| 816 | [dy395769511-star/dsh-pdf-to-word](https://github.com/dy395769511-star/dsh-pdf-to-word) | 0 | 2026-08-29 | 2026-08-29 | PDF to Word conversion plugin for DeepSeek Harness (dsh): PyMuPDF/PaddleOCR pipeline + LLM visual style verification |
| 817 | [dzf-code/dsh-paste-doc](https://github.com/dzf-code/dsh-paste-doc) | 0 | 2026-08-24 | 2026-09-01 | 粘贴长文本 |
| 818 | [EasyTZ/dsh-git](https://github.com/EasyTZ/dsh-git) | 0 | 2026-08-27 | 2026-08-27 | Git panel plugin for DeepSeek Harness (dsh) — visual staging, commits, push and branch switching in the sidebar |
| 819 | [EasyTZ/dsh-reveal-explorer](https://github.com/EasyTZ/dsh-reveal-explorer) | 0 | 2026-08-27 | 2026-08-27 | Reveal-in-file-manager plugin for DeepSeek Harness (dsh) — open the current workspace in your system file manager |
| 820 | [EasyTZ/dsh-terminal-panel](https://github.com/EasyTZ/dsh-terminal-panel) | 0 | 2026-08-27 | 2026-08-27 | Terminal panel plugin for DeepSeek Harness (dsh) — run commands in the current workspace with streaming output |
| 821 | [EasyTZ/dsh-ui-balance](https://github.com/EasyTZ/dsh-ui-balance) | 0 | 2026-08-27 | 2026-08-27 | Balance display plugin for DeepSeek Harness (dsh) — show your DeepSeek API balance under each reply |
| 822 | [eehcx/dsh-gentle-engram](https://github.com/eehcx/dsh-gentle-engram) | 0 | 2026-08-26 | 2026-08-27 | DSH adapter for Engram — persistent memory bridge built with Cordis. |
| 823 | [EIGHTfs/dsh-git-push](https://github.com/EIGHTfs/dsh-git-push) | 0 | 2026-08-18 | 2026-09-02 | DSH git 自动提交推送插件：扫描仓库 + 一键 commit/push（工具 + HTTP API） |
| 824 | [elliseang0000-lang/dsh-pentest-bugtrace](https://github.com/elliseang0000-lang/dsh-pentest-bugtrace) | 0 | 2026-09-01 | 2026-09-01 | BugTraceAI penetration-testing mode for deepseek-harness (dsh): pentester persona, runbook skill, and MCP bridge in one installable bundle |
| 825 | [EmptyCollin/dsh-peak-valley-queue](https://github.com/EmptyCollin/dsh-peak-valley-queue) | 0 | 2026-08-27 | 2026-08-27 | Peak/valley pricing task queue for DeepSeek Harness |
| 826 | [erdholion/dsh-loop-guard](https://github.com/erdholion/dsh-loop-guard) | 0 | 2026-08-31 | 2026-09-01 | Result-aware stuck-loop guard for DeepSeek Harness: advisory nudges plus a monotonic hard stop. Only repeats with identical results count. |
| 827 | [EsonXie/dsh-agent-toolkit](https://github.com/EsonXie/dsh-agent-toolkit) | 0 | 2026-08-19 | 2026-09-01 | Deepseek Harness工具集 |
| 828 | [evanfang0054/dsh-init](https://github.com/evanfang0054/dsh-init) | 0 | 2026-09-01 | 2026-09-01 | Claude Code style /init command for DeepSeek Harness (DSH): generates CLAUDE.md and symlinks AGENTS.md to it |
| 829 | [evlon/deepseek-harness-launcher](https://github.com/evlon/deepseek-harness-launcher) | 0 | 2026-08-28 | 2026-08-29 | 托盘常驻的 DeepSeek Harness 安装 / 启动器（Tauri 2 无窗口应用，仅系统托盘 + 原生通知 + 日志文件） |
| 830 | [evlon/dsh-codebuddy-models](https://github.com/evlon/dsh-codebuddy-models) | 0 | 2026-08-26 | 2026-08-29 | 把本机已登录的 CodeBuddy / WorkBuddy（腾讯代码助手） 订阅作为 dsh（DeepSeek Harness） 的原生 provider 接入，启用后 CodeBuddy 模型会直接出现在 dsh 的模型选择器中，可像其它模型一样被 agent 调用。 |
| 831 | [evlon/dsh-matrix-agent](https://github.com/evlon/dsh-matrix-agent) | 0 | 2026-08-27 | 2026-08-29 | DeepSeek Harness（dsh）的 Matrix agent 桥接插件：把 Matrix 房间桥接到 harness agent 会话，每个房间一个会话，支持在聊天里远程监控、审批和追加指令；多分身架构 + 媒体/富文本/回复/编辑信息完整处理。 |
| 832 | [ewceniza9009/wilsonix-studio](https://github.com/ewceniza9009/wilsonix-studio) | 0 | 2026-09-01 | 2026-09-02 | AI-powered desktop DAW - stem separation, chord detection, karaoke |
| 833 | [Exaggarate/dshpkg](https://github.com/Exaggarate/dshpkg) | 0 | 2026-09-02 | 2026-09-02 | Security & health audit CLI for DeepSeek Harness (DSH) plugins — npm audit for the everything-is-a-plugin era. Search, info, security-scan, doctor. stdlib-only. |
| 834 | [Exception-H/dsh-gpt56-ptc](https://github.com/Exception-H/dsh-gpt56-ptc) | 0 | 2026-08-30 | 2026-08-30 | Native DSH Bundle: user-owned pure PTC / Code Mode preset for GPT-5.6 with plain-language answers and bounded execution. |
| 835 | [FADE-4869/dsh-gacha-viz](https://github.com/FADE-4869/dsh-gacha-viz) | 0 | 2026-08-26 | 2026-08-27 | Genshin Impact gacha history visualizer and pity probability calculator for DeepSeek Harness (DSH plugin) |
| 836 | [fan56/dsh-ask-router](https://github.com/fan56/dsh-ask-router) | 0 | 2026-08-25 | 2026-08-29 | dsh plugin: multi-surface ask-user routing, first answer wins |
| 837 | [fan56/dsh-cron](https://github.com/fan56/dsh-cron) | 0 | 2026-08-31 | 2026-09-02 | Cron scheduling for the DeepSeek Harness — bounded tasks with calendar & interval rules, delivered to live agents |
| 838 | [fan56/dsh-dcp](https://github.com/fan56/dsh-dcp) | 0 | 2026-08-17 | 2026-08-28 | dsh plugin: deterministic context compression backend — zero LLM calls, reproducible compression |
| 839 | [fan56/dsh-feishu](https://github.com/fan56/dsh-feishu) | 0 | 2026-08-23 | 2026-08-27 | dsh plugin: drive an existing dsh session from Feishu/Lark — outbound-only bot, /resume picker, run status card |
| 840 | [fan56/dsh-llm-proxy](https://github.com/fan56/dsh-llm-proxy) | 0 | 2026-08-24 | 2026-09-01 | dsh plugin: per-host LLM outbound HTTP proxy routing (undici ProxyAgent) with a bundled dsh skill |
| 841 | [fan56/dsh-llmwiki-memory](https://github.com/fan56/dsh-llmwiki-memory) | 0 | 2026-08-31 | 2026-09-01 | dsh-plugin: OKF v0.2 topic memory for dsh - local-first git-tracked bundle, hot-path LLM-free injection, two-stage observer with background distill |
| 842 | [fan56/dsh-mcp-adapter](https://github.com/fan56/dsh-mcp-adapter) | 0 | 2026-08-26 | 2026-08-29 | dsh plugin: fold mcp__* tool schemas into two meta-tools via prompt-side shim to save tokens |
| 843 | [fan56/dsh-vault](https://github.com/fan56/dsh-vault) | 0 | 2026-08-30 | 2026-09-01 | dsh-plugin: encrypted backup / restore / migration of the dsh home config through a private GitHub repo |
| 844 | [fan56/dsh-web-search-anysearch](https://github.com/fan56/dsh-web-search-anysearch) | 0 | 2026-08-26 | 2026-08-29 | AnySearch web search provider plugin for DeepSeek Harness (dsh) — zero-config, out-of-the-box |
| 845 | [fan56/dsh-web-search-tavily](https://github.com/fan56/dsh-web-search-tavily) | 0 | 2026-08-25 | 2026-08-29 | Tavily web search provider plugin for DeepSeek Harness (dsh) |
| 846 | [fantasyce/dsh-typelens](https://github.com/fantasyce/dsh-typelens) | 0 | 2026-08-27 | 2026-08-28 | Automatic bounded type context and edit diagnostics for DeepSeek Harness |
| 847 | [Fast-Editor/lynkr-dsh-plugin](https://github.com/Fast-Editor/lynkr-dsh-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness (dsh) plugin: registers Lynkr as a custom OpenAI-compatible provider |
| 848 | [faye0526/dsh-backup-btn](https://github.com/faye0526/dsh-backup-btn) | 0 | 2026-08-26 | 2026-08-27 | DSH 一键备份按钮 - 浮动按钮备份 DSH 数据到 GitHub Gist |
| 849 | [FeatureAgents/AgentsGitFlowController](https://github.com/FeatureAgents/AgentsGitFlowController) | 0 | 2026-08-17 | 2026-08-28 | Agents Client Level Git Flow Controller |
| 850 | [felix-lj-ct/dsh-mcp-live-status](https://github.com/felix-lj-ct/dsh-mcp-live-status) | 0 | 2026-08-28 | 2026-08-28 | Adds a status pill to the DeepSeek Harness web composer tool row: how many configured MCP servers are actually reachable, plus per-server transport, tool count and failure reason on click. Surfaces what the settings page cannot — a server that mounted fine but never finished its MCP handshake. Read-only, no config needed. |
| 851 | [fentz26/dsh-goodjob](https://github.com/fentz26/dsh-goodjob) | 0 | 2026-08-26 | 2026-08-27 | Multi-agent operations workspace for DeepSeek Harness. |
| 852 | [fentz26/dsh-next](https://github.com/fentz26/dsh-next) | 0 | 2026-08-26 | 2026-08-27 | Performance-oriented backend/runtime modernization layer for DeepSeek Harness. |
| 853 | [firestige/wsr-dsh](https://github.com/firestige/wsr-dsh) | 0 | 2026-08-29 | 2026-08-29 | WSR integrations for DeepSeek Harness: Execution, Studio, and suite bundles. |
| 854 | [firestige/wsr-execution](https://github.com/firestige/wsr-execution) | 0 | 2026-08-17 | 2026-08-30 | Host-neutral execution boundary for workflow-self-recursive: resolves one exact Workflow Package, binds an immutable Delivery Manifest, coordinates the Delivery, emits bounded OTLP observations. Install via dsh plugin add wsr-dsh-intake · 与宿主无关的 Agent 工作流执行边界：解析并校验确定的工作流包，绑定不可变交付清单，协调交付并发出有界观测。 |
| 855 | [fishfromsky/dsh-march7th-skin](https://github.com/fishfromsky/dsh-march7th-skin) | 0 | 2026-08-20 | 2026-08-27 | 崩坏星穹铁道三月七主题的deepseek harness皮肤插件 |
| 856 | [FishingTofu0120/Plugin-for-checking-API-balance](https://github.com/FishingTofu0120/Plugin-for-checking-API-balance) | 0 | 2026-09-01 | 2026-09-01 | A plugin for checking API-balance on DSH website conveniently |
| 857 | [Flan246/dsh-latex-guard](https://github.com/Flan246/dsh-latex-guard) | 0 | 2026-08-26 | 2026-08-27 | LaTeX compile check and BibTeX lint/fill/audit tools for DeepSeek Harness and any agent. dsh plugin + CLI + SKILL.md. |
| 858 | [Flan246/dsh-lit-search](https://github.com/Flan246/dsh-lit-search) | 0 | 2026-08-26 | 2026-08-27 | Academic literature search, citation and BibTeX tools for DeepSeek Harness and any agent (Crossref + OpenAlex). dsh plugin + CLI + SKILL.md. |
| 859 | [flashyiyi/dsh-envelope-highlight](https://github.com/flashyiyi/dsh-envelope-highlight) | 0 | 2026-08-28 | 2026-08-28 | Restore syntax highlighting of read/write tool envelopes inside run_code (PTC / Code Mode) result cards |
| 860 | [fly1989/dsh-deliberation](https://github.com/fly1989/dsh-deliberation) | 0 | 2026-08-20 | 2026-08-31 | Primary-controlled deliberation and opt-in reasoning-masked review for DeepSeek Harness. |
| 861 | [flyingfishzxf/dsh-dsbal](https://github.com/flyingfishzxf/dsh-dsbal) | 0 | 2026-08-18 | 2026-08-27 | A simple DeepSeek API balance display plugin for dsh(deepseek-harness) |
| 862 | [flymysql/dsh-browser-client](https://github.com/flymysql/dsh-browser-client) | 0 | 2026-08-23 | 2026-08-31 | DSH Browser Client — LLM 驱动的浏览器浮窗工作流工具（面向非研发人员的网页自动化） |
| 863 | [force-push/dsh-llm-fallback](https://github.com/force-push/dsh-llm-fallback) | 0 | 2026-08-27 | 2026-08-27 | Self-healing cross-provider model fallback plugin for the DeepSeek Harness (DSH) — retries exhausted, re-bind the session to the next healthy model. |
| 864 | [ForeverYoungPp/dsh-web-search](https://github.com/ForeverYoungPp/dsh-web-search) | 0 | 2026-09-01 | 2026-09-01 | dsh-web-search — Multi-provider web search for DeepSeek Harness: routes the native web_search tool through a configurable provider fallback chain (Tavily/Brave/Exa/Firecrawl/Jina/Kagi/SearXNG/DuckDuckGo), replacing the built-in deepseek-official backend, with a settings page for key management and ordering. Approach adapted from OMP.  |
| 865 | [founder987/dsh-dev-ui](https://github.com/founder987/dsh-dev-ui) | 0 | 2026-08-25 | 2026-08-27 | 适合编码研发的UI界面 |
| 866 | [FoyonaCZY/dsh-kit](https://github.com/FoyonaCZY/dsh-kit) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugins for the failures nobody catches: auto-format, generated-file guard, .env drift detection, and a typecheck gate that runs before the agent says it's done. Four gaps the 13k-plugin ecosystem hasn't filled. |
| 867 | [Francesco502/dsh-quota](https://github.com/Francesco502/dsh-quota) | 0 | 2026-08-26 | 2026-08-27 | AI Quota and Token Usage Monitor for DeepSeek Harness (Codex, Cursor, Antigravity, OpenCode-Go) |
| 868 | [Frank-NF/dsh-drop-md](https://github.com/Frank-NF/dsh-drop-md) | 0 | 2026-08-30 | 2026-08-30 | Drag-and-drop markdown enhancer for DeepSeek Harness (DSH): inline small files, @-reference large ones, one-click SKILL.md install |
| 869 | [Frank-NF/dsh-memory-nexus](https://github.com/Frank-NF/dsh-memory-nexus) | 0 | 2026-09-01 | 2026-09-01 | DSH integrated memory and context management plugin: 4-layer memory, context compression, prompt orchestration, enterprise security |
| 870 | [frank6892103/dsh-WutheringWaves](https://github.com/frank6892103/dsh-WutheringWaves) | 0 | 2026-08-30 | 2026-08-31 | dsh鸣潮主题插件 |
| 871 | [freedomkk-qfeng/dsh-mail-assistant](https://github.com/freedomkk-qfeng/dsh-mail-assistant) | 0 | 2026-08-31 | 2026-08-31 | Standards-based IMAP/SMTP mail connector for DeepSeek Harness, enabling agents to read and send email with explicit user controls. |
| 872 | [freedomkk-qfeng/dsh-oidc](https://github.com/freedomkk-qfeng/dsh-oidc) | 0 | 2026-08-30 | 2026-08-30 | Enterprise OIDC, secure API-key binding, declarative branding, and OpenAI-compatible model integration for DeepSeek Harness. |
| 873 | [freerpa/Hrequest](https://github.com/freerpa/Hrequest) | 0 | 2026-09-02 | 2026-09-02 | 轻量级 Node.js 多线程 API 压测工具，支持代理轮询、请求参数随机化注入和实时进度监控。 |
| 874 | [FriendsHL/dsh-agent-evolution](https://github.com/FriendsHL/dsh-agent-evolution) | 0 | 2026-08-26 | 2026-08-27 | Preset-composed Agent experiments and evolution primitives for DeepSeek Harness |
| 875 | [fthuu/Tokan-dsh-token-analytics](https://github.com/fthuu/Tokan-dsh-token-analytics) | 0 | 2026-08-31 | 2026-08-31 | 精准 Token 洞察，实时追踪，智能优化提示和用量归因 Sharp token insights, real‑time tracking, smart optimization signals & attribution  |
| 876 | [GavinQiEr/dsh-cmdwatch](https://github.com/GavinQiEr/dsh-cmdwatch) | 0 | 2026-08-30 | 2026-08-30 | Real-time command monitor for DeepSeek Harness (DSH). Watch foreground/background command output in the Web UI without pausing the conversation. 命令窗：实时显示 DSH 命令与执行输出。 |
| 877 | [geecraft23/dsh-turn-colors](https://github.com/geecraft23/dsh-turn-colors) | 0 | 2026-09-02 | 2026-09-02 | Color-code user prompts and final assistant replies by conversation turn in the DeepSeek Harness Web UI. |
| 878 | [geeklei/dsh-plugins](https://github.com/geeklei/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | 一个面向 DeepSeek Harness (dsh)的插件库 |
| 879 | [geekyfoxlab/dsh-subagents](https://github.com/geekyfoxlab/dsh-subagents) | 0 | 2026-08-26 | 2026-08-27 | Focused child-agent delegation (scout, researcher, worker, reviewer, oracle, delegate) and multi-agent workflows (council, parallel review, review loop) for DeepSeek Harness. |
| 880 | [ghbhiee/dsh-plugin-tui](https://github.com/ghbhiee/dsh-plugin-tui) | 0 | 2026-08-28 | 2026-08-28 | Claude Code-style terminal UI plugin for DeepSeek Harness (dsh): streaming REPL, collapsed thinking, interactive session/model pickers, history replay, approval modes, bottom status bar |
| 881 | [Ghost011118/dsh-plugin-governor-extension](https://github.com/Ghost011118/dsh-plugin-governor-extension) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin governance: installable runtime tool policy plus companion boot admission, supervised restart, and rollback. |
| 882 | [Ghost011118/dsh-plugin-marketplace](https://github.com/Ghost011118/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Built-in plugin discovery, local requirement matching, optional GitHub stars, and one-click installation for DeepSeek Harness. |
| 883 | [GitNoHup/macaron-theme](https://github.com/GitNoHup/macaron-theme) | 0 | 2026-08-26 | 2026-08-27 | 🍬 马卡龙毛玻璃主题（Macaron Glassmorphism Theme）— DeepSeek Harness 动态主题插件：四套马卡龙配色、145° 双色渐变、毛玻璃卡片；日间上色 / 夜间自动清除并记忆恢复。 |
| 884 | [gjjkbssg/dsh-model-jury](https://github.com/gjjkbssg/dsh-model-jury) | 0 | 2026-08-31 | 2026-08-31 | Structured cross-model peer review for DeepSeek Harness — blind reasoning, anonymous critique, revision, and deterministic verdicts. |
| 885 | [Glazyonyt/dsh-lowtide](https://github.com/Glazyonyt/dsh-lowtide) | 0 | 2026-08-28 | 2026-08-28 | Queue AI tasks during off-peak hours to cut costs and automate runs with dsh-lowtide for DeepSeek Harness. |
| 886 | [GoldenZqqq/dsh-model-collapse](https://github.com/GoldenZqqq/dsh-model-collapse) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin: collapse the model picker by provider, with a pinned quick bar (expand-all / collapse-all / focus-current / filter / reset). |
| 887 | [goldgish/dsh-gamepad-approval](https://github.com/goldgish/dsh-gamepad-approval) | 0 | 2026-08-30 | 2026-08-30 | Xbox 手柄硬件审批插件 for DeepSeek Harness (dsh) — Agent 高危工具调用需物理按键确认，A 批准 / B 驳回 |
| 888 | [gongyijie85/dsh-agent-frugality](https://github.com/gongyijie85/dsh-agent-frugality) | 0 | 2026-08-29 | 2026-09-02 | Multi-agent frugality defense plugin for DeepSeek Harness: read-ledger dedup, compaction-immune rules, completion gate, cheap-review lane. |
| 889 | [GooDAnDReaDY/dsh-agent-loop-guard](https://github.com/GooDAnDReaDY/dsh-agent-loop-guard) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness runtime guard for tool-call and assistant-output loops |
| 890 | [GooDAnDReaDY/dsh-context-lens](https://github.com/GooDAnDReaDY/dsh-context-lens) | 0 | 2026-08-31 | 2026-09-01 | DSH plugin for AST context compression, test log filtering, and token budget guard |
| 891 | [GooDAnDReaDY/dsh-gitea](https://github.com/GooDAnDReaDY/dsh-gitea) | 0 | 2026-08-31 | 2026-08-31 | Gitea/Forgejo toolkit for DeepSeek Harness: issues, PRs, CI, releases, operations |
| 892 | [GooDAnDReaDY/dsh-kanban](https://github.com/GooDAnDReaDY/dsh-kanban) | 0 | 2026-08-27 | 2026-09-01 | Kanban board for DeepSeek Harness: Gitea-backed tasks, workflow columns, and dedicated agent sessions |
| 893 | [GooDAnDReaDY/dsh-live-canvas](https://github.com/GooDAnDReaDY/dsh-live-canvas) | 0 | 2026-08-31 | 2026-08-31 | Interactive in-browser canvas for real-time preview of HTML, React components, SVGs, and diagrams with SSE hot-reload in DeepSeek Harness |
| 894 | [GooDAnDReaDY/dsh-time-machine](https://github.com/GooDAnDReaDY/dsh-time-machine) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin for smart checkpoints, workspace safety guards, and instant rollback |
| 895 | [Gorilla-Kevv/scnu-thesis-formatter](https://github.com/Gorilla-Kevv/scnu-thesis-formatter) | 0 | 2026-08-30 | 2026-08-30 | 华南师范大学本科毕业论文格式改写 + matplotlib 数据可视化（DeepSeek Harness 技能） |
| 896 | [GoshawkGGGG/dsh-safe-tool](https://github.com/GoshawkGGGG/dsh-safe-tool) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness 的 AI 工具审批插件，使用AI审核AGENT调用工具的合规性并决定是否执行，审核标准可定制。 |
| 897 | [GreenLv/dsh-completion-guard](https://github.com/GreenLv/dsh-completion-guard) | 0 | 2026-08-26 | 2026-08-29 | Task-contract and completion-certification layer for DeepSeek Harness |
| 898 | [grstein/dsh-locale-ptbr](https://github.com/grstein/dsh-locale-ptbr) | 0 | 2026-08-31 | 2026-08-31 | Pacote de idioma Português (Brasil) para a GUI Web do DeepSeek Harness |
| 899 | [gsh150801/dsh-bioinf](https://github.com/gsh150801/dsh-bioinf) | 0 | 2026-09-01 | 2026-09-01 | Bioinformatics plugin for DeepSeek Harness (dsh) |
| 900 | [gsh150801/dsh-bioinf-routed](https://github.com/gsh150801/dsh-bioinf-routed) | 0 | 2026-09-01 | 2026-09-01 | Bioinformatics plugin for DeepSeek Harness (dsh) |
| 901 | [gsh150801/dsh-bioinf-verify](https://github.com/gsh150801/dsh-bioinf-verify) | 0 | 2026-09-01 | 2026-09-01 | Bioinformatics plugin for DeepSeek Harness (dsh) |
| 902 | [gtaifu/dsh-title-index](https://github.com/gtaifu/dsh-title-index) | 0 | 2026-09-01 | 2026-09-01 | Disk-indexed session title lookups for the DeepSeek Harness web GUI — @-mention candidates ~30× faster. |
| 903 | [guangxiangwu6-cmd/dsh-llm-failover](https://github.com/guangxiangwu6-cmd/dsh-llm-failover) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness model auto-failover plugin: retry threshold -> mark unavailable -> seamless switch to next healthy model -> cooldown auto-recover. 18-model pool, 19/19 tests, boot-safe. |
| 904 | [guazixiong/dsh-coding-mode-preset](https://github.com/guazixiong/dsh-coding-mode-preset) | 0 | 2026-08-30 | 2026-08-30 | 为本地 DeepSeek Harness（`@deepseek-ai/dsh`）追加一个**编码模式** Agent Preset：门禁式工程交付流水线，包含三条独立流程——**需求开发**、**Bug 修复**、**功能迭代**。每个阶段的产物由全新上下文的"空白子代理"独立专家评审，通过后须经用户确认才进入下一阶段；最终以用户验收作为任务完结条件。 |
| 905 | [GuoxinShan/dsh-yzj](https://github.com/GuoxinShan/dsh-yzj) | 0 | 2026-08-14 | 2026-08-27 | 云之家 (Yunzhijia) plugin bundle for DeepSeek Harness: yzj-cli bridge, 41 model-facing tools, floating workspace panel with drag/@ reference chips |
| 906 | [Hanmingh/dsh-desktop](https://github.com/Hanmingh/dsh-desktop) | 0 | 2026-08-27 | 2026-08-27 | Desktop Plugin for Deepseek Harness |
| 907 | [haohaiHuang/Design-Agent](https://github.com/haohaiHuang/Design-Agent) | 0 | 2026-08-27 | 2026-08-27 | DSH 设计 Agent 完整可复现包：design-references 路由技能（DSH 适配）+ design-router 确定性工具插件 + my-agent 预设 |
| 908 | [HaoR325/dsh-usage-daily](https://github.com/HaoR325/dsh-usage-daily) | 0 | 2026-08-30 | 2026-08-31 | DSH 用量日报浮窗插件：今日令牌/消息/轮数/估算费用 |
| 909 | [haoranwang0921/dsh-bid-desk](https://github.com/haoranwang0921/dsh-bid-desk) | 0 | 2026-08-28 | 2026-08-30 | DSH 投标合规工作台是一个 DSH 插件 MVP，服务于投标文件编制过程。它将招标来源证据、要求记录、人工复核决定和生成报告关联起来，帮助具备相应资质或经验的人员在提交前核查缺口。 |
| 910 | [haoyu-qi/dsh-zentao](https://github.com/haoyu-qi/dsh-zentao) | 0 | 2026-08-15 | 2026-08-27 | 面向 DeepSeek Harness 的 AVCON Web 界面定制与个人禅道 CLI 工作中心 |
| 911 | [haozheou/dsh-exam-expert](https://github.com/haozheou/dsh-exam-expert) | 0 | 2026-08-30 | 2026-08-30 | 出题专家 · Exam Expert plugin for DeepSeek Harness: 把出题流程固化成值守流水线（角色+目录→通读→勾选表单→六分身流水线→看板交付） \| Turn the exam-paper workflow into an agent-supervised pipeline: wizard dialog, prefilled checklist form, six-role dual-kanban production |
| 912 | [harness-home/harness-ai-plugins](https://github.com/harness-home/harness-ai-plugins) | 0 | 2026-08-26 | 2026-08-27 | Community plugin catalog for Harness AI: a scanner over the public npm registry, and the snapshot it publishes. |
| 913 | [Harzva/dsh-restart-autoresume](https://github.com/Harzva/dsh-restart-autoresume) | 0 | 2026-08-29 | 2026-08-29 | Safe DSH restart coordination and durable top-level session autoresume |
| 914 | [haythamat/dsh-client-ui-rtl](https://github.com/haythamat/dsh-client-ui-rtl) | 0 | 2026-08-27 | 2026-08-27 | Right-to-left text direction for the DeepSeek Harness Web client |
| 915 | [hcyinnn/dsh-tool-ssh](https://github.com/hcyinnn/dsh-tool-ssh) | 0 | 2026-09-01 | 2026-09-01 | SSH tools plugin for DeepSeek Harness (dsh): run remote commands and transfer files via OpenSSH. dsh 插件——让 Agent 通过 SSH 在远程主机执行命令、上传/下载文件。 |
| 916 | [heartmove/dsh-session-bridge](https://github.com/heartmove/dsh-session-bridge) | 0 | 2026-09-01 | 2026-09-01 |  DSH 插件，让当前代理直接从提示词驱动其它真实 DSH 会话——创建/发送/等待回复/读取/恢复/跨工作区查找会话，并支持监控调度主任务与归档会话。A DSH plugin that lets the agent drive other real DSH sessions straight from a prompt — create, send, wait, read, resume, and find sessions across workspaces, plus monitor/schedule a main task and archive sessions. |
| 917 | [hedging8563/tokenlab-deepseek-harness-provider](https://github.com/hedging8563/tokenlab-deepseek-harness-provider) | 0 | 2026-08-27 | 2026-08-27 | TokenLab native-protocol model provider, multimodal tools, and async tasks for DeepSeek Harness |
| 918 | [hehehe1234567894/dsh-ssh-remote](https://github.com/hehehe1234567894/dsh-ssh-remote) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness (DSH) SSH 远程工作插件 — 纯远程模式：多机管理、工作区选择、远程文件读写工具 |
| 919 | [hehetoshang/dsh-talebook-plugin](https://github.com/hehetoshang/dsh-talebook-plugin) | 0 | 2026-08-27 | 2026-08-30 | DeepSeek Harness plugin for safely operating Talebook |
| 920 | [helibeiqi/dsh-cdp-metadata](https://github.com/helibeiqi/dsh-cdp-metadata) | 0 | 2026-08-23 | 2026-08-28 | Capability Description Protocol (CDP) v0.1 — read-only AI-readable capability metadata layer for DSH Cordis plugins. |
| 921 | [helibeiqi/dsh-cn-disclosure](https://github.com/helibeiqi/dsh-cn-disclosure) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 公告/年报 结构化抽取 MCP server (dsh-plugin) |
| 922 | [helibeiqi/dsh-context-aware-search](https://github.com/helibeiqi/dsh-context-aware-search) | 0 | 2026-08-19 | 2026-08-28 | Context-aware web search plugin for DeepSeek Harness (dsh): rewrites queries with session context, reranks + credibility-tags results, one-click source summarization across multiple backends. Fully decoupled from @deepseek-ai private packages for public CI. |
| 923 | [helibeiqi/dsh-dcs-engine](https://github.com/helibeiqi/dsh-dcs-engine) | 0 | 2026-08-24 | 2026-08-28 | Dynamic Capability Synthesis Engine — DSH protocol stack credit engine |
| 924 | [helibeiqi/dsh-docx-mcp](https://github.com/helibeiqi/dsh-docx-mcp) | 0 | 2026-08-28 | 2026-08-28 | Zero-dependency MCP stdio server that generates real .docx files from a JSON spec — Chinese office-automation vertical for DeepSeek Harness. |
| 925 | [helibeiqi/dsh-hr-payroll-mcp](https://github.com/helibeiqi/dsh-hr-payroll-mcp) | 0 | 2026-08-29 | 2026-08-29 | 通用 HR 算薪 MCP 服务：本地化法定社保/公积金/个税计算 + 通用表头适配 + 企业配置 + 安全绩效公式（PII 不出机） |
| 926 | [helibeiqi/dsh-industry-graph-mcp](https://github.com/helibeiqi/dsh-industry-graph-mcp) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 产业链/申万行业/概念板块 知识图谱 MCP server (dsh-plugin) |
| 927 | [helibeiqi/dsh-memory-projection](https://github.com/helibeiqi/dsh-memory-projection) | 0 | 2026-08-20 | 2026-08-28 | Hot-pluggable memory-projection scheduling framework for DeepSeek Harness (dsh): pure-function projection strategies + a runtime invariant guard, built on the cordis plugin kernel. |
| 928 | [helibeiqi/dsh-quant-factor-pipeline](https://github.com/helibeiqi/dsh-quant-factor-pipeline) | 0 | 2026-08-28 | 2026-08-28 | Quant factor research pipeline as a dsh user-layer MCP server (CGO disposal-effect factor, RankIC, Newey-West t, regime-aware) |
| 929 | [hellofuture2068/dsh-simple-view](https://github.com/hellofuture2068/dsh-simple-view) | 0 | 2026-08-26 | 2026-08-27 | Declutter DeepSeek Harness chat: hide agent execution-log rows, tighten spacing & fonts, bubble messages, and set a "reply concisely" system-prompt instruction. |
| 930 | [hellogit2021/avoid-ai-writing-cn](https://github.com/hellogit2021/avoid-ai-writing-cn) | 0 | 2026-08-29 | 2026-08-29 | 知乎"去AI味写作技巧"社区免费提供：中文写作去 AI 味插件（AI-isms / AI writing / humanize）。说"去掉AI味"即重写，说"写的不错"自动学习新 AI 词。安装：dsh plugin --profile web add github:hellogit2021/avoid-ai-writing-cn |
| 931 | [helloworld1631/dsh-volcengine-usage](https://github.com/helloworld1631/dsh-volcengine-usage) | 0 | 2026-08-27 | 2026-08-27 | Draggable Volcengine Coding Plan usage monitor for DeepSeek Harness Web. |
| 932 | [hfyydd/dsh-cua](https://github.com/hfyydd/dsh-cua) | 0 | 2026-08-28 | 2026-08-28 | Computer Use for DeepSeek Harness, backed by the cua-driver daemon (trycua): UIA element-level targeting, background-first input delivery, deterministic verification. |
| 933 | [hhb1028/dsh-client-ui-timeline](https://github.com/hhb1028/dsh-client-ui-timeline) | 0 | 2026-08-30 | 2026-08-30 | DSH Web GUI 会话问题导航条：聊天区左缘一问一杠，随滚动高亮当前问题、悬停显示问答预览气泡、点击把该问平滑滚到视口顶（未渲染的更早历史自动翻页加载），无需改动 dsh 本体源码 |
| 934 | [higekibaka/dsh-ciel](https://github.com/higekibaka/dsh-ciel) | 0 | 2026-08-31 | 2026-08-31 | 夏尔 Ciel — a pre-planning advisor and convergent critic for DeepSeek Harness: a second, knowledge-rich model offering directions, prior art, pitfalls and verification checklists (ideas, never steps). |
| 935 | [HiSeax/dsh-agent-outputs-reader](https://github.com/HiSeax/dsh-agent-outputs-reader) | 0 | 2026-08-29 | 2026-08-30 | Overlay reader for agent output files: Markdown/GFM rendering, in-panel PDF, DOCX/XLSX/PPTX text preview, reply-end file chips. Pure JS, zero deps. |
| 936 | [HiSeax/dsh-better-model-setting](https://github.com/HiSeax/dsh-better-model-setting) | 0 | 2026-08-23 | 2026-08-29 | DSH plugin: replaces official Models settings page with provider management, per-model reasoning effort, retry overrides, drag reorder, add official DeepSeek, credential status |
| 937 | [hmlyx/dsh-memory](https://github.com/hmlyx/dsh-memory) | 0 | 2026-08-29 | 2026-08-29 | 简单的插件，让你的每个 AI 记录经验和记忆 |
| 938 | [hmlyx/dsh-notify](https://github.com/hmlyx/dsh-notify) | 0 | 2026-08-29 | 2026-08-29 | 在输入框右边加了一个泡泡窗口，你可以接入插件或者告诉 AI 什么时候使用它。 |
| 939 | [honoriomelo/dsh-model-picker-search](https://github.com/honoriomelo/dsh-model-picker-search) | 0 | 2026-08-29 | 2026-08-29 | DSH Web GUI plugin: adds a live search field inside the model picker menu of the composer, plus the Effort (reasoning) selector. Drop-in replacement for the native model seat, sharing the same per-session ModelDirectory so /model popup, the effort selector, and the /model command stay consistent. |
| 940 | [horizon105457/tsstream](https://github.com/horizon105457/tsstream) | 0 | 2026-08-26 | 2026-08-27 | 🌊 Agent-native time-series streaming for DeepSeek Harness (DSH plugin) — terminal/serial byte streams → indexed, queryable, event-driven timeline. 19 tools · 9 operators · 🧪 experimental |
| 941 | [Hoshino-Yumetsuki/as-compatible-copilot](https://github.com/Hoshino-Yumetsuki/as-compatible-copilot) | 0 | 2026-08-01 | 2026-08-29 | A VSCode extension to use Openai/Anthropic/Gemini API Providers in GitHub Copilot Chat |
| 942 | [hotpot-labs/dsh-notifier-plugin](https://github.com/hotpot-labs/dsh-notifier-plugin) | 0 | 2026-08-30 | 2026-09-02 | dsh 干完活之后通知你，【轻量级】通知插件，只通知，不交互，mac/windows/linux 操作系统支持，dsh 在干活时你可以摸鱼 |
| 943 | [hotpot-labs/dsh-prompt-history-plugin](https://github.com/hotpot-labs/dsh-prompt-history-plugin) | 0 | 2026-09-01 | 2026-09-02 | dsh 输入框的提示词导航插件，支持上下键查看历史输入 |
| 944 | [hpyer/dsh-for-mac](https://github.com/hpyer/dsh-for-mac) | 0 | 2026-08-31 | 2026-08-31 | DshForMac 是 DeepSeek Harness 的原生 macOS 启动器与运行时管理器，提供本地环境检测、版本管理及内嵌 Web 界面。 |
| 945 | [hrhgit/dsh-model-manager](https://github.com/hrhgit/dsh-model-manager) | 0 | 2026-08-14 | 2026-08-31 | Model tags, reasoning capabilities, image routing, and vision proxy support for DeepSeek Harness |
| 946 | [hu669293657/dsh-turn-tools](https://github.com/hu669293657/dsh-turn-tools) | 0 | 2026-08-29 | 2026-08-29 | DSH web plugin: per-turn deliverable buttons (open with the OS default app) and a turn-navigator dot rail for jumping between conversation turns. |
| 947 | [huangDouP/dsh-client-ui-notifications](https://github.com/huangDouP/dsh-client-ui-notifications) | 0 | 2026-08-29 | 2026-08-29 | DSH Web notifications: browser notifications, tab title flash, favicon badge, and native Windows toasts with a bilingual (zh/en) settings page. |
| 948 | [huangjua/dsh-evidence](https://github.com/huangjua/dsh-evidence) | 0 | 2026-09-01 | 2026-09-01 | 🛡️ Verifiable, tamper-proof audit evidence bundles and hash-chained receipts for DSH agents |
| 949 | [huangjua/dsh-local-memory](https://github.com/huangjua/dsh-local-memory) | 0 | 2026-09-01 | 2026-09-01 | 🧠 Persistent cross-session local memory for DSH agents (Markdown SSOT + self-healing SQLite mirror) |
| 950 | [huangjua/dsh-session-index](https://github.com/huangjua/dsh-session-index) | 0 | 2026-09-01 | 2026-09-01 | 🔍 Full-text session search & bookmarking engine for DSH with native CJK substring search |
| 951 | [HuangLM03/dsh-plugin-session-archive](https://github.com/HuangLM03/dsh-plugin-session-archive) | 0 | 2026-08-31 | 2026-08-31 | Browse and permanently delete archived DeepSeek Harness sessions from the sidebar footer. |
| 952 | [HuanLinOTO/dsh-plugin-copilot](https://github.com/HuanLinOTO/dsh-plugin-copilot) | 0 | 2026-08-28 | 2026-08-28 | Copilot 引导层插件：WebUI 设置卡片一键 GitHub 授权 + 自动激活模型路由并收窄模型列表（复用 dsh-llm-pi-ai 内置 device-flow） \| Copilot onboarding plugin: one-click GitHub auth from the WebUI settings card, auto-activating the model route and narrowing the model list (reuses dsh-llm-pi-ai's builtin device flow) |
| 953 | [HuanLinOTO/dsh-plugin-tools-manager](https://github.com/HuanLinOTO/dsh-plugin-tools-manager) | 0 | 2026-08-14 | 2026-08-28 | DSH 工具管理器：查看/启停宿主已注册工具 \| DSH tools manager: inspect and toggle host-registered tools |
| 954 | [HuanyuTan777/dsh-tool-pdf](https://github.com/HuanyuTan777/dsh-tool-pdf) | 0 | 2026-08-28 | 2026-08-28 | DSH PDF reader plugin (pdf_info / pdf_extract / pdf_render) |
| 955 | [huaxiren6/DSH-QrPairing](https://github.com/huaxiren6/DSH-QrPairing) | 0 | 2026-08-19 | 2026-08-27 | Floating phone-pairing QR button for the DSH WebUI. Companion UI for dsh-remote-link. |
| 956 | [HULILI-com/dsh-namecheck](https://github.com/HULILI-com/dsh-namecheck) | 0 | 2026-08-26 | 2026-08-27 | dsh plugin for checking domain availability and trademark screening of candidate product names |
| 957 | [hun1315/dsh-msi-icons](https://github.com/hun1315/dsh-msi-icons) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 模型选择器美化插件：厂商官方图标 + 四区平铺 + 置顶主力超时自动路由 \| Model selector beautifier for DSH: official vendor icons, pinned-first flat layout, first-token-timeout failover |
| 958 | [hunbs-1/dsh-codepect](https://github.com/hunbs-1/dsh-codepect) | 0 | 2026-08-29 | 2026-08-30 | dsh-codepect is a DSH plugin generating OpenAPI 3.0 from TS/JS. Features: visual docs, versioning, change detection, mock & auto-rescan. Zero-dep, offline, ensures code-doc sync for backend API delivery. dsh-codepect是DSH插件，扫描TS/JS生成OpenAPI3.0文档。支持可视化、多版本、变更检测、Mock及自动重扫。零依赖离线可用，确保代码文档一致，助后端交付API契约。 |
| 959 | [hunterxxn/deep-flow](https://github.com/hunterxxn/deep-flow) | 0 | 2026-08-14 | 2026-08-29 | deepseek-harness tui |
| 960 | [huyang2024/dsh-openai-api](https://github.com/huyang2024/dsh-openai-api) | 0 | 2026-08-27 | 2026-08-27 | OpenAI-compatible HTTP surface for DeepSeek Harness (dsh): POST /v1/chat/completions, POST /v1/responses, GET /v1/models over the harness webServer + llm runtime |
| 961 | [IcedWatermelonJuice/dsh-provider-veark](https://github.com/IcedWatermelonJuice/dsh-provider-veark) | 0 | 2026-08-30 | 2026-08-31 | 把火山方舟 Coding Plan 装进 DeepSeek Harness：文本 + 图片对话，图片走 Files API，密钥粘贴即用 |
| 962 | [icyaaaww/dsh-tui-secret-guard](https://github.com/icyaaaww/dsh-tui-secret-guard) | 0 | 2026-08-26 | 2026-08-27 | Blocks high-confidence secrets before dsh-TUI sends them to a model, compliant with dsh ecosystem manifest v0.15. |
| 963 | [iguanren/Taishan-Vision](https://github.com/iguanren/Taishan-Vision) | 0 | 2026-08-29 | 2026-08-29 | 让 DeepSeek Harness 纯文本模型也能识图：默认推荐智谱 GLM-4.6V-FLASH和 GLM-4.1V-FLASH 免费视觉模型 |
| 964 | [ihorleleka/Local-Rag-Wiki](https://github.com/ihorleleka/Local-Rag-Wiki) | 0 | 2026-06-03 | 2026-08-27 | A per-repository, Docker-hosted MCP knowledge service that gives coding agents a governed Markdown "wiki" with semantic retrieval. The promise — a local RAG wiki that accumulates durable project knowledge across agentic sessions. |
| 965 | [IKEASven69/dsh-opencli](https://github.com/IKEASven69/dsh-opencli) | 0 | 2026-08-30 | 2026-08-30 | 让 DeepSeek Harness (dsh) 会办事:登录态真实浏览器 + 170+ 站点适配器 + write 审批门 |
| 966 | [ikomom/dsh-a-share-assistant](https://github.com/ikomom/dsh-a-share-assistant) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness A股研究助手插件：对话式选股/排雷/盯盘/复盘，数据走同花顺金融数据 API，带本地缓存层。 |
| 967 | [ikomom/dsh-trade-chart](https://github.com/ikomom/dsh-trade-chart) | 0 | 2026-08-14 | 2026-08-31 | DeepSeek Harness 交易图表插件：对话内直接渲染 K线/折线/柱状/面积图、技术指标（EMA/BOLL/MACD/RSI/KDJ/MAVOL）、热点轮动矩阵与连板晋级图。纯自绘 SVG，零外部依赖，附在线示例页。 |
| 968 | [imkingjh999/dsh-adaptive-effort](https://github.com/imkingjh999/dsh-adaptive-effort) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: auto reasoning_effort (low/high/max) per turn via MiniMax complexity scorer + token ledger + per-reply metadata label |
| 969 | [intsig-textin/dsh-plugin-xparse](https://github.com/intsig-textin/dsh-plugin-xparse) | 0 | 2026-08-28 | 2026-08-31 | TextIn xParse document parsing tool and skill for DeepSeek Harness, with multi-document tasks, OAuth/AppKey authentication, and paid-operation approval. |
| 970 | [iTrimut/GitHub-Road](https://github.com/iTrimut/GitHub-Road) | 0 | 2026-08-28 | 2026-08-28 | Github-Road: 大陆稳定访问 GitHub 官网的网络路径修复技能（hosts 直连 + 动态 IP 择优 + 30 分钟自动自愈，免代理、零费用）——非 agent 专属，任意智能体可用，也可纯手动运行。A network-path fix skill (not agent-specific) for reliable github.com access from mainland China. |
| 971 | [jaaty/dsh-gsd-bundle](https://github.com/jaaty/dsh-gsd-bundle) | 0 | 2026-08-23 | 2026-08-30 | A DeepSeek Harness bundle reimplementing opengsd-core (Git Ship Done) as host-plane Cordis plugins, replacing the default agent-loop behaviour with the GSD phase loop. |
| 972 | [JackyYangxx/dsh-plugins](https://github.com/JackyYangxx/dsh-plugins) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness (DSH) plugin workspace — home of lbx-agent-team, a multi-agent development team plugin (captain-led planner/checker/dever/tester with pipeline hard gates, git worktrees and a live web panel) |
| 973 | [jackyytche/dsh-hindsight-memory](https://github.com/jackyytche/dsh-hindsight-memory) | 0 | 2026-09-01 | 2026-09-01 | Hindsight long-term memory for DeepSeek Harness |
| 974 | [jasonguide/dsh-skills-hub](https://github.com/jasonguide/dsh-skills-hub) | 0 | 2026-08-28 | 2026-08-29 | 一个多 Agent 平台的 Skills 统一管理插件（DeepSeek Harness 插件），可以在DSH中统一管理codex、claude code、PI、OpenCode、Hermes、Openclaw等平台的Skills技能 |
| 975 | [jdqingm/dsh-plan-build-toggle](https://github.com/jdqingm/dsh-plan-build-toggle) | 0 | 2026-08-31 | 2026-08-31 | OpenChamber-style persistent Plan\|Build composer toggle for DeepSeek Harness, with Tab-to-switch. Drives the native /plan channel over the host plan projection. |
| 976 | [Jensen-Yao/dsh-deepexcel](https://github.com/Jensen-Yao/dsh-deepexcel) | 0 | 2026-08-27 | 2026-08-28 | Deepcel 工作簿 · DeepSeek Harness (dsh) 皮肤中心 v2 皮肤：Excel 风格工作簿，单元格化消息、工作表网格、工作簿标签。Small-tailqwq/dsh-deepcel 的 v2 完整移植。 |
| 977 | [Jiachi5533/dsh-remote-gateway](https://github.com/Jiachi5533/dsh-remote-gateway) | 0 | 2026-08-28 | 2026-08-28 | Source-filtered remote gateway for DeepSeek Harness behind an authenticated reverse proxy |
| 978 | [jiang12345-code/dsh-openrouter-free](https://github.com/jiang12345-code/dsh-openrouter-free) | 0 | 2026-08-27 | 2026-08-27 | OpenRouter 免费模型面板 for DeepSeek Harness — 分级星标 · 一键切换 · 任务续跑友好 |
| 979 | [jiang12345-code/dsh-self-restart](https://github.com/jiang12345-code/dsh-self-restart) | 0 | 2026-08-29 | 2026-08-29 | DSH self-restart plugin (Windows): reliable elevated restart via schtasks, transparent front-end recovery, auto-detect and resume in-progress sessions across reboots, business gate prevents wake self-excitation loops. |
| 980 | [jiangchuangege/anime-pet-widget](https://github.com/jiangchuangege/anime-pet-widget) | 0 | 2024-01-19 | 2026-08-27 | jenkins测试 |
| 981 | [JiayiXie-jpg/dsh-desktop-pet](https://github.com/JiayiXie-jpg/dsh-desktop-pet) | 0 | 2026-08-26 | 2026-08-27 | 一只住在 DSH 网页里的养成系桌宠：随编码活动升级进化、语音打气，还能用 AI 生成专属的透明动画形象。 |
| 982 | [jimmyzhang219/dsh-plan-and-execute](https://github.com/jimmyzhang219/dsh-plan-and-execute) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness (dsh) 的 Plan-and-Execute 编排插件 |
| 983 | [JingzeChen/dsh-beacon](https://github.com/JingzeChen/dsh-beacon) | 0 | 2026-09-02 | 2026-09-02 | Attention and handoff workspace for concurrent DeepSeek Harness Sessions |
| 984 | [jingzhonghui/dsh-mcp-manager](https://github.com/jingzhonghui/dsh-mcp-manager) | 0 | 2026-08-30 | 2026-08-30 | DSH dynamic Cordis plugin: visually manage MCP servers (stdio) from the settings sidebar, and expose their tools to the agent as mcp__<server>__<tool>. |
| 985 | [jinwendijv/dsh-applauncher](https://github.com/jinwendijv/dsh-applauncher) | 0 | 2026-08-27 | 2026-08-27 | DSH 的应用启动器插件：自动扫描本机已安装的电脑应用，在侧边栏“设置”图标上方提供一键启动，像 Windows 开始菜单一样，扫描添加后可以点击启动应用 |
| 986 | [JJXjustin/dsh-session-rewind](https://github.com/JJXjustin/dsh-session-rewind) | 0 | 2026-08-31 | 2026-08-31 | DSH session and file rewind plugin (shadow git repo) |
| 987 | [jkt-check/dsh-secret-scrub](https://github.com/jkt-check/dsh-secret-scrub) | 0 | 2026-09-02 | 2026-09-02 | Irreversible secret-scrubbing guard plugin for DeepSeek Harness (dsh): regex redaction of secrets before session-log persistence and model requests |
| 988 | [jmche/dsh-llm-verifier-pro](https://github.com/jmche/dsh-llm-verifier-pro) | 0 | 2026-08-26 | 2026-09-02 | LLM-as-a-Verifier plugin for DeepSeek Harness — fine-grained reward tools (verify_compare / verify_select / verify_track) with Probabilistic Pivot Tournament, plus a Best-of-N conversation mode with a Web settings panel. |
| 989 | [jo32/dsh-strudel-studio](https://github.com/jo32/dsh-strudel-studio) | 0 | 2026-08-29 | 2026-08-30 | A professional song-level Strudel visual sequencer with structured AI arrangement for DeepDeck. |
| 990 | [jo32/dsh-video-sherlock](https://github.com/jo32/dsh-video-sherlock) | 0 | 2026-08-26 | 2026-08-27 | A local-first, evidence-backed video investigation app for DeepDeck. |
| 991 | [joao-paulo-santos/dsh-bouncing-squares-example](https://github.com/joao-paulo-santos/dsh-bouncing-squares-example) | 0 | 2026-08-26 | 2026-08-27 | Example plugin for dsh-granular-settings: three bouncing squares, one per settings scope (session, workspace, global). Switch sessions and workspaces to watch each scope behave differently |
| 992 | [joao-paulo-santos/dsh-diff-view](https://github.com/joao-paulo-santos/dsh-diff-view) | 0 | 2026-08-29 | 2026-08-29 | Diff view: a reusable two-text diff viewer for DSH client plugins — line LCS, word highlights, split/unified views, true line numbers across context collapse. |
| 993 | [joao-paulo-santos/dsh-granular-prompt](https://github.com/joao-paulo-santos/dsh-granular-prompt) | 0 | 2026-08-27 | 2026-08-27 | Prompt composition manager for DSH: live census of every system-prompt section with suppress and replace, custom system prompts, and a persona library with a picker right in the chat composer |
| 994 | [joao-paulo-santos/dsh-granular-settings](https://github.com/joao-paulo-santos/dsh-granular-settings) | 0 | 2026-08-26 | 2026-08-27 | Granular settings platform: one Granular Settings page (Workspace/Session/Plugin tabs) where other DSH plugins register scoped, namespaced controls (session, workspace, global). Nine control types, doorbell-only push via dsh-event-relay |
| 995 | [joao-paulo-santos/dsh-md-view](https://github.com/joao-paulo-santos/dsh-md-view) | 0 | 2026-08-29 | 2026-08-29 | Markdown view: a safe markdown-to-React renderer for DSH client plugins — GitHub-subset markdown, shared stylesheet, no HTML injection. |
| 996 | [joao-paulo-santos/dsh-scratchpad](https://github.com/joao-paulo-santos/dsh-scratchpad) | 0 | 2026-08-28 | 2026-08-28 | Scratch pad: one shared floating text surface in the middle of the screen, opened by other plugins through the client service scratchpad. |
| 997 | [joao-paulo-santos/dsh-wo-github](https://github.com/joao-paulo-santos/dsh-wo-github) | 0 | 2026-08-29 | 2026-08-29 | Workspace Overview GitHub tab: About card, README rendered as markdown, and the default-branch commit history with per-file patches. |
| 998 | [joao-paulo-santos/dsh-wo-tmux](https://github.com/joao-paulo-santos/dsh-wo-tmux) | 0 | 2026-08-31 | 2026-09-01 | Workspace Overview tmux tab: live/frozen/cold session state, one-click terminal attach through tmux-fridge, freeze/snapshot/recover, and workspace-to-session links. |
| 999 | [joao-paulo-santos/dsh-workspace-history](https://github.com/joao-paulo-santos/dsh-workspace-history) | 0 | 2026-08-28 | 2026-08-28 | Workspace history: journals every compaction summary to the workspace and adds a History subtab to the Workspace Overview tab for reading it back. |
| 1000 | [joao-paulo-santos/dsh-workspace-overview](https://github.com/joao-paulo-santos/dsh-workspace-overview) | 0 | 2026-08-28 | 2026-08-28 | Workspace overview: a Workspace Overview tab beside Chat with a subtab facade for other plugins, and a GitHub pill in the session header when the workspace has a github.com repository. |
| 1001 | [JochenYang/dsh-remote](https://github.com/JochenYang/dsh-remote) | 0 | 2026-08-29 | 2026-08-29 | Operate DeepSeek Harness from your phone: self-hosted relay + desktop plugin tunnel with a mobile-adapted web UI. MIT |
| 1002 | [JoeeLiu/dsh-super-subscriptions](https://github.com/JoeeLiu/dsh-super-subscriptions) | 0 | 2026-08-28 | 2026-08-28 | Unified subscription providers, model routing, quota UI, and media tools for DeepSeek Harness |
| 1003 | [JoeyLearnsToCode/dsh-workspace-native-open](https://github.com/JoeyLearnsToCode/dsh-workspace-native-open) | 0 | 2026-08-28 | 2026-08-28 | dsh plugin for native open workspace / 用于本地打开工作区目录的 dsh 插件 |
| 1004 | [johnvictorio/dsh-custom-prompt](https://github.com/johnvictorio/dsh-custom-prompt) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin that injects an editable section into the global system prompt, with a Settings page |
| 1005 | [joshryandavis/dsh-catalog-refresh](https://github.com/joshryandavis/dsh-catalog-refresh) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically rebuild model catalogues for OpenRouter, OpenCode, Fireworks, etc |
| 1006 | [joshryandavis/dsh-goal-restart](https://github.com/joshryandavis/dsh-goal-restart) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically restart goals on harness restart |
| 1007 | [JPA957/dsh-web-search-anysearch](https://github.com/JPA957/dsh-web-search-anysearch) | 0 | 2026-09-02 | 2026-09-02 | AnySearch search provider plugin for DeepSeek Harness (ctx.web) with round-robin API-key rotation and per-key cooldown failover |
| 1008 | [jsoncode/dsh-model-list](https://github.com/jsoncode/dsh-model-list) | 0 | 2026-08-27 | 2026-08-28 | OpenRouter free-models browser & one-click model config for DeepSeek Harness (DSH) — newest-first, local search, platform tabs. DSH 免费模型浏览器：按最新排序、本地搜索、一键添加到模型列表 |
| 1009 | [justhalfbit/dsh-plugin-show-image](https://github.com/justhalfbit/dsh-plugin-show-image) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness (DSH) 会话内图片渲染插件：全局 show_image 工具 + 点击放大 lightbox。 \| Inline image rendering plugin for DSH: global show_image tool + click-to-enlarge lightbox. |
| 1010 | [jwilson411/dsh-arxiv](https://github.com/jwilson411/dsh-arxiv) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: tiny read-only arXiv search + abstract fetch (Atom API, no PDF ingest) |
| 1011 | [jwilson411/dsh-canary](https://github.com/jwilson411/dsh-canary) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: plant a canary and deny tool args/URLs that echo it (CANARY_TRIP). |
| 1012 | [jwilson411/dsh-compat-probe](https://github.com/jwilson411/dsh-compat-probe) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: OpenAI-compat server protocol card (loopback probe, no GGUF) |
| 1013 | [jwilson411/dsh-kokoro](https://github.com/jwilson411/dsh-kokoro) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: HTTP TTS client for jwilson411/kokoro-tts-api. No weights. |
| 1014 | [jwilson411/dsh-llamacpp](https://github.com/jwilson411/dsh-llamacpp) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness LLM adapter for a local llama.cpp OpenAI-compatible server. |
| 1015 | [jwilson411/dsh-loop-brake](https://github.com/jwilson411/dsh-loop-brake) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: identical tool+args circuit breaker (LOOP_BRAKE) |
| 1016 | [jwilson411/dsh-modelprint](https://github.com/jwilson411/dsh-modelprint) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: fingerprint provider, model id, sampling, tool schemas, and system-prompt prefix; pin the card and fail structured on drift. |
| 1017 | [jwilson411/dsh-mutation-receipt](https://github.com/jwilson411/dsh-mutation-receipt) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: append-only JSONL of filesystem touches (path, op, sha256 before/after) with no file contents |
| 1018 | [jwilson411/dsh-otel](https://github.com/jwilson411/dsh-otel) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: emit OpenTelemetry spans from a session log (turn / step / tool execute). Export only. |
| 1019 | [jwilson411/dsh-plugin-kit](https://github.com/jwilson411/dsh-plugin-kit) | 0 | 2026-08-29 | 2026-08-29 | A minimal, tested template for DeepSeek Harness plugins. |
| 1020 | [jwilson411/dsh-result-cap](https://github.com/jwilson411/dsh-result-cap) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: deterministic tool-result byte cap with SHA-256 of the omitted tail. Not a compressor model. |
| 1021 | [jwilson411/dsh-secret-scrub](https://github.com/jwilson411/dsh-secret-scrub) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: redact known secret shapes before the model sees them; JSONL incidents never store the preimage |
| 1022 | [jwilson411/dsh-spend-receipt](https://github.com/jwilson411/dsh-spend-receipt) | 0 | 2026-08-29 | 2026-08-31 | A cache-aware JSONL cost receipt plugin for DeepSeek Harness. |
| 1023 | [jwilson411/dsh-ssrf-guard](https://github.com/jwilson411/dsh-ssrf-guard) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness plugin: fail-closed URL host/scheme allowlist that runs before a request is opened |
| 1024 | [jwilson411/dsh-tool-quota](https://github.com/jwilson411/dsh-tool-quota) | 0 | 2026-08-31 | 2026-09-01 | DeepSeek Harness plugin: per-tool call and result-byte caps |
| 1025 | [kaixinguo360/dsh-bsk-ws-bridge](https://github.com/kaixinguo360/dsh-bsk-ws-bridge) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness BrowserSkill 桥接插件：把本机 bsk daemon 的 WebSocket 经浏览器信道暴露给远程 BrowserSkill 扩展。配套的修改版 BrowserSkill 扩展：https://github.com/kaixinguo360/BrowserSkill-DSH-Remote |
| 1026 | [kaka-crypto/dsh-disk-guard](https://github.com/kaka-crypto/dsh-disk-guard) | 0 | 2026-08-28 | 2026-08-28 | Disk guard for DeepSeek Harness: redirect downloads/artifacts/caches/temp off the C: drive, inject a path-discipline prompt into every session, disk_guard tool for status/cleanup. |
| 1027 | [kalifun/dsh-cwl](https://github.com/kalifun/dsh-cwl) | 0 | 2026-09-01 | 2026-09-01 | Structured context eviction for DeepSeek Harness — deterministic, zero-LLM, no summarization lossiness |
| 1028 | [KarthusLorin/dsh-subagent-grok](https://github.com/KarthusLorin/dsh-subagent-grok) | 0 | 2026-08-29 | 2026-08-29 | One-shot Grok CLI subagent provider for DeepSeek Harness |
| 1029 | [KDronin/dsh-folder](https://github.com/KDronin/dsh-folder) | 0 | 2026-08-16 | 2026-09-01 | DeepSeek Harness plugin: Open Folder in workspace context menu (between Rename and Delete Workspace) |
| 1030 | [KDronin/dsh-tray](https://github.com/KDronin/dsh-tray) | 0 | 2026-08-16 | 2026-09-01 | DeepSeek Harness 桌面托盘插件：托盘启动 Harness、任务完成通知、电源管理、进程接管、GitHub 集成 |
| 1031 | [Kehao/dsh-client-ui-weather](https://github.com/Kehao/dsh-client-ui-weather) | 0 | 2026-08-30 | 2026-08-30 | Deepseek harness 天气插件 |
| 1032 | [kenny2077/dsh-web-kimi](https://github.com/kenny2077/dsh-web-kimi) | 0 | 2026-08-31 | 2026-08-31 | Kimi Coding web search + web fetch providers for the DeepSeek Harness with coding plan key |
| 1033 | [KeS1Ke/dsh-start-and-exit](https://github.com/KeS1Ke/dsh-start-and-exit) | 0 | 2026-08-24 | 2026-08-27 | dsh-start&exit: safe start, exit, and restart controls for the DeepSeek Harness Web profile, plus a loopback-only Windows foreground launcher. |
| 1034 | [kfc966/dsh-native-codex-oauth](https://github.com/kfc966/dsh-native-codex-oauth) | 0 | 2026-09-01 | 2026-09-01 | Native Codex OAuth login and model access for DeepSeek Harness as one installable plugin. |
| 1035 | [KimFischer99/DeepSeek-Harness-Desktop](https://github.com/KimFischer99/DeepSeek-Harness-Desktop) | 0 | 2026-08-15 | 2026-08-27 | 一个轻量的 macOS 桌面应用壳，Rust 编写，承载 DeepSeek Harness WebUI，一键启停 |
| 1036 | [kingcheng12/dsh-workspace-change-awareness](https://github.com/kingcheng12/dsh-workspace-change-awareness) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin that surfaces concurrent workspace changes before an agent continues. |
| 1037 | [kittcat-lab/dsh-kitt-voice](https://github.com/kittcat-lab/dsh-kitt-voice) | 0 | 2026-09-01 | 2026-09-02 | Voice for the DeepSeek Harness: speak to the agent, hear it back, and see what it is doing from a floating window that stays on top of whatever you are running. |
| 1038 | [kittimzhe/dsh-plugin-authoring-guide](https://github.com/kittimzhe/dsh-plugin-authoring-guide) | 0 | 2026-08-29 | 2026-08-29 | Hands-on guide to building a DeepSeek Harness plugin (EN/ZH) — real code & pitfalls from dsh-session-export and dsh-session-recall |
| 1039 | [kivensteven8-eng/dsh-file-download](https://github.com/kivensteven8-eng/dsh-file-download) | 0 | 2026-08-27 | 2026-08-27 | DSH 插件：把会话工作区文件变成浏览器直接下载的 HTTP 通道 —— 为 iPad 等局域网/域名设备设计。 |
| 1040 | [KKL08/dsh-plastic-memory](https://github.com/KKL08/dsh-plastic-memory) | 0 | 2026-09-01 | 2026-09-02 | Memory plugin with built-in governance for DeepSeek Harness: 为你的 DSH 赋予可塑性记忆 |
| 1041 | [KL3jd/handwritten-ocr](https://github.com/KL3jd/handwritten-ocr) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin for local OCR: handwritten Chinese + math → Markdown with LaTeX. GPU / CPU backends. |
| 1042 | [knownothing114/dsh-notify](https://github.com/knownothing114/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | A dsh plugin that raises a desktop notification whenever dsh needs your attention. |
| 1043 | [kobenfang/BigTimer](https://github.com/kobenfang/BigTimer) | 0 | 2026-08-29 | 2026-08-29 | 🕐 BigTimer · 定时任务+消息推送管家 — Scheduled tasks & message push manager for DeepSeek Harness (dsh) |
| 1044 | [Kogisune/dsh-skin-koi-pond](https://github.com/Kogisune/dsh-skin-koi-pond) | 0 | 2026-08-20 | 2026-08-28 | 🎏 锦鲤池塘 · Koi Pond theme for DeepSeek Harness (DSH) WebUI — 动画锦鲤 + 部件拆分 CSS |
| 1045 | [konanzheng/dsh-timeline](https://github.com/konanzheng/dsh-timeline) | 0 | 2026-08-26 | 2026-08-27 | show timeline for deepseek harness |
| 1046 | [kongshan-zhuyu/dsh-balance-quota](https://github.com/kongshan-zhuyu/dsh-balance-quota) | 0 | 2026-08-18 | 2026-09-01 | 一块可以配置余额、监测模型监控状态、以及配置模型多模态设置的插件 |
| 1047 | [koompi/dsh-desktop](https://github.com/koompi/dsh-desktop) | 0 | 2026-09-02 | 2026-09-02 | Electron desktop shell for DeepSeek Harness: runs the published dsh CLI as a sidecar |
| 1048 | [kp-z/dsh-dev-git-graph](https://github.com/kp-z/dsh-dev-git-graph) | 0 | 2026-09-01 | 2026-09-02 | DSH Web Git Graph panel — a faithful port of vscode-git-graph 1.30.0, auto-bound to the session workspace, with full git operations and light/dark theming. First of the dsh-dev-* graph plugin series. |
| 1049 | [ktao732084-arch/dsh-vibegap](https://github.com/ktao732084-arch/dsh-vibegap) | 0 | 2026-08-27 | 2026-08-27 | Vocabulary flashcards inside the dsh web UI - appear while your agent runs, retreat when it finishes. A VibeGap plugin. |
| 1050 | [ktao732084-arch/vibegap](https://github.com/ktao732084-arch/vibegap) | 0 | 2026-08-26 | 2026-08-27 | Mini-window for the gaps in vibe coding: vocabulary flashcards (and more panels) that auto-appear while your AI coding agent runs |
| 1051 | [kuanfu0430/dsh-compaction-tune](https://github.com/kuanfu0430/dsh-compaction-tune) | 0 | 2026-09-01 | 2026-09-01 | Composer control for DeepSeek Harness auto-compaction thresholds |
| 1052 | [kumanana66/dsh-automation](https://github.com/kumanana66/dsh-automation) | 0 | 2026-09-01 | 2026-09-01 | RPA-style scheduled web automation for DeepSeek Harness: record browser operations -> requirements doc -> LLM generates Python + Playwright -> schedule with run records and email notifications |
| 1053 | [KumarZX/kur-compact-trigger](https://github.com/KumarZX/kur-compact-trigger) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件 · 会话级压缩（官方 auto 只能全局） / Per-session compaction; official auto is global-only |
| 1054 | [l2685209197/dsh-pdf-translate](https://github.com/l2685209197/dsh-pdf-translate) | 0 | 2026-09-01 | 2026-09-01 | DSH 插件：用 DeepSeek 翻译文本型 PDF，保留版式/字体/图片/链接，输出可编辑 PDF（单次 ≤50 页） |
| 1055 | [LamplitIsles/kepos-tts](https://github.com/LamplitIsles/kepos-tts) | 0 | 2026-08-29 | 2026-08-30 | Qwen/Volcengine TTS for dsh |
| 1056 | [Lanzgale/dsh-listener](https://github.com/Lanzgale/dsh-listener) | 0 | 2026-08-30 | 2026-08-30 | 安全版本地语音输入插件 for DeepSeek Harness:同源宿主代理 + 127.0.0.1 + token,SenseVoice-Small INT8 ONNX 本地转写,音频不出网。 |
| 1057 | [lasdrder0705/dsh-chat-zone-std](https://github.com/lasdrder0705/dsh-chat-zone-std) | 0 | 2026-08-26 | 2026-08-27 | dsh-std Community v0.15 chat zone: ~/dsh_CHAT/<date>/chatN as Tools and Commands. Install adapter-dsh first. |
| 1058 | [lasdrder0705/dsh-pro-vision-std](https://github.com/lasdrder0705/dsh-pro-vision-std) | 0 | 2026-08-26 | 2026-08-27 | dsh-std Community v0.15 ModelProvider: V4-Pro with Flash-Vision captions. Install adapter-dsh first. |
| 1059 | [lastplayer82/dsh-sticky-notes](https://github.com/lastplayer82/dsh-sticky-notes) | 0 | 2026-08-27 | 2026-08-27 | 灵感便签 (Sticky Notes) plugin for the dsh web GUI: jot ideas while the agent thinks — without interrupting it. Queue-channel sends/forwards, auto-persist (localStorage + host file), export TXT/JSON/MD, bilingual zh/en. DeepSeek Harness plugin · @lastplayer82/dsh-sticky-notes |
| 1060 | [leechengwei/dsh-session-intelligence](https://github.com/leechengwei/dsh-session-intelligence) | 0 | 2026-08-31 | 2026-08-31 | DSH 会话情报：固定右侧栏、初衷与最近用户需求摘要、会话活动和只读 Git 状态。 |
| 1061 | [lelens0/dsh-token-ledger](https://github.com/lelens0/dsh-token-ledger) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness plugin: monitor balance & usage across multiple LLM gateways, with balance history sparklines (token ledger) |
| 1062 | [lemoncat7/dsh-partner](https://github.com/lemoncat7/dsh-partner) | 0 | 2026-08-27 | 2026-08-31 | Long-lived AI companions with WeChat channel routing for DeepSeek Harness |
| 1063 | [Leo3-7/dsh-obsidian-inbox](https://github.com/Leo3-7/dsh-obsidian-inbox) | 0 | 2026-08-28 | 2026-08-28 | DSH skill: ingest the conclusions/mistakes/projects from conversations into an Obsidian vault via a 7-step workflow with two-level validation. 把对话结论/错题/项目按七步流程整理进 Obsidian 的 DeepSeek Harness 技能。 |
| 1064 | [LeoChen98/dsh-worktable-notebook-to-ppt](https://github.com/LeoChen98/dsh-worktable-notebook-to-ppt) | 0 | 2026-08-26 | 2026-08-27 | 基于 dsh-worktable 工作台搭建的「课本到 PPT」自动化工作流插件——在 DeepSeek Harness 中一键将 Jupyter Notebook 转化为专业可编辑的演示文稿（.pptx），让知识沉淀与分享更高效。 |
| 1065 | [leogottadothebest/dsh-plugin-archived-conversations](https://github.com/leogottadothebest/dsh-plugin-archived-conversations) | 0 | 2026-08-31 | 2026-09-02 | DSH 插件：在设置界面管理已归档对话——取消归档与永久删除 |
| 1066 | [leogottadothebest/dsh-settings-beautify](https://github.com/leogottadothebest/dsh-settings-beautify) | 0 | 2026-09-01 | 2026-09-02 | One design language for the DSH settings surface: unified typography, cards, controls, focus and motion across every settings page, including pages contributed by other plugins. |
| 1067 | [LeonSone/dsh-question-rail](https://github.com/LeonSone/dsh-question-rail) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: 模仿 deepseek 网页版界面右侧的问题条 — 右缘一条竖向问题栏，列出当前会话每一轮的用户提问，点击平滑滚动定位。DeepSeek Harness right-edge question rail. |
| 1068 | [lgquan/dsh-workspace-memory](https://github.com/lgquan/dsh-workspace-memory) | 0 | 2026-08-28 | 2026-08-31 | Durable workspace-scoped memory for DeepSeek Harness and dsh-voco voice agents. |
| 1069 | [lhf6623/dsh-thrum](https://github.com/lhf6623/dsh-thrum) | 0 | 2026-08-16 | 2026-08-29 | DeepSeek Harness 输入氛围插件：为输入过程增添氛围。 |
| 1070 | [liangminhua/agent-notes-toolkit](https://github.com/liangminhua/agent-notes-toolkit) | 0 | 2026-08-30 | 2026-08-30 | Agent Notes mechanism as a portable toolkit: verification gates, scaffolding CLI, and the AN dsh preset/bundle |
| 1071 | [liangsheng999/dsh-client-ui-connection-status](https://github.com/liangsheng999/dsh-client-ui-connection-status) | 0 | 2026-08-26 | 2026-08-27 | DSH Web client plugin: a corner pill showing live connection state for the DeepSeek Harness Web UI. npm: dsh-client-ui-connection-status |
| 1072 | [liangsheng999/dsh-dream](https://github.com/liangsheng999/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH host plugin: scheduled background 'dream' (memory consolidation) passes for DeepSeek Harness. npm: dsh-dream |
| 1073 | [liangxiaobing520/dsh-local-vector-memory](https://github.com/liangxiaobing520/dsh-local-vector-memory) | 0 | 2026-08-29 | 2026-08-29 | Fully local vector memory plugin for DeepSeek Harness: local embeddings, SQLite storage, automatic recall injection, dedup with conflict detection, soft-delete recycle bin, online backup. |
| 1074 | [LianPing-cyber/dsh-browser-full-access](https://github.com/LianPing-cyber/dsh-browser-full-access) | 0 | 2026-08-29 | 2026-08-29 | Full-access background-tab fork of dsh-browser for DeepSeek Harness (DSH). Based on dsh-browser, MCP, and browser-use. |
| 1075 | [liaoyuqing/dsh-llm-error-retry](https://github.com/liaoyuqing/dsh-llm-error-retry) | 0 | 2026-09-02 | 2026-09-02 | 用于在deepseek-harnees中报错时重试大模型请求，支持配置http状态，字段-值命中。 |
| 1076 | [liceses/dsh-hmm-wait](https://github.com/liceses/dsh-hmm-wait) | 0 | 2026-08-22 | 2026-08-27 | 化口水为乐趣，把大肥鱼流的口水变成游戏连击！ |
| 1077 | [Lichtspur/deepseek-style-theme](https://github.com/Lichtspur/deepseek-style-theme) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek official-home style theme for the dsh web GUI: fluid particle background, glass sidebar, glass composer, frosted header, running-subagent progress panel, DSTT time-based mode, and DeepSeek brand link |
| 1078 | [lijian-ui/dsh-file-manager](https://github.com/lijian-ui/dsh-file-manager) | 0 | 2026-08-18 | 2026-08-27 | 为 DeepSeek Harness 桌面端（dsh web）开发的插件：聊天区右侧的 Explorer 文件面板 + Preview 预览面板（FileManager 风格，Apache-2.0 参考实现非抄录），以及输入框 @ 引用项目文件（树形多选弹窗 + 输入框内胶囊 + 行号） |
| 1079 | [lijian-ui/dsh-schedule-view](https://github.com/lijian-ui/dsh-schedule-view) | 0 | 2026-08-24 | 2026-08-27 | A cron-based scheduled task plugin for DeepSeek Harness (dsh) desktop: create / edit / delete / fire-now tasks from the settings panel, with cross-session agent follow-up and multi-level notifications. Zero LLM tools — purely human-driven scheduling. |
| 1080 | [lijian-ui/dsh-skill-manage](https://github.com/lijian-ui/dsh-skill-manage) | 0 | 2026-08-22 | 2026-08-27 | A skill management plugin for DeepSeek Harness (dsh) desktop: list / enable / disable / delete / add skills, filling the gap in dsh's official skill toggle control. |
| 1081 | [lijian-ui/dsh-term](https://github.com/lijian-ui/dsh-term) | 0 | 2026-08-19 | 2026-08-27 | Panel-style local terminal for the DSH web GUI. |
| 1082 | [lijian-ui/dsh-vision-toggle](https://github.com/lijian-ui/dsh-vision-toggle) | 0 | 2026-08-28 | 2026-08-28 | dsh-vision-toggle 是一个为 DeepSeek Harness (dsh) 提供「支持图片」开关的插件，让你在设置页按模型一键启用/禁用图片输入 |
| 1083 | [limlnx523/dsh-plus-plus](https://github.com/limlnx523/dsh-plus-plus) | 0 | 2026-08-27 | 2026-08-28 | DSH++ — a local-first control plane for DeepSeek Harness. Plugin security auditing and workflow regression testing. |
| 1084 | [linkbag/dsh-swarm-orchestrator](https://github.com/linkbag/dsh-swarm-orchestrator) | 0 | 2026-09-02 | 2026-09-02 | Role-based AI swarm orchestration for DeepSeek Harness: per-role model pinning with fallbacks, parallel task DAG with review loops, live Swarm dashboard tab. |
| 1085 | [Lion-Li-git/dsh-external-links](https://github.com/Lion-Li-git/dsh-external-links) | 0 | 2026-08-30 | 2026-08-30 | DSH desktop (Deepseek Harness EAC) plugin: open http/https/mailto/tel/file links in the default browser/app, bypassing the broken shell.open-external bridge |
| 1086 | [lionwill/dsh-compactor](https://github.com/lionwill/dsh-compactor) | 0 | 2026-09-01 | 2026-09-01 | DSH上下文压缩插件 |
| 1087 | [lisongxuan/ds-hentai](https://github.com/lisongxuan/ds-hentai) | 0 | 2026-08-25 | 2026-08-28 | ExHentai-inspired UI for DeepSeek Harness. ExHentai风格DeepSeek Harness皮肤。 ds hentai / deepseek hentai |
| 1088 | [liujia-io/dsh-image-picker](https://github.com/liujia-io/dsh-image-picker) | 0 | 2026-08-26 | 2026-08-27 | Paperclip image-picker button for the DeepSeek Harness web composer - pick reference images via the system file dialog and feed them into the official attachment pipeline. |
| 1089 | [Liujie-harsh/heart-health-dsh-suite](https://github.com/Liujie-harsh/heart-health-dsh-suite) | 0 | 2026-08-28 | 2026-08-28 | 适配心脏健康场景的 DeepSeek Harness 插件套件：在「心衰辅助诊断算法服务（heart-algo MCP）」之上， 为 DSH 会话提供一组受控的领域包装工具、驻留临床指导与原始工具隐藏策略。 |
| 1090 | [liuwenji007/dsh-trust-check](https://github.com/liuwenji007/dsh-trust-check) | 0 | 2026-08-27 | 2026-08-27 | Static capability disclosure for DeepSeek Harness plugins — evidence-backed, zero-token, no safety claims. |
| 1091 | [liuyangdongdong/dsh-session-rerun](https://github.com/liuyangdongdong/dsh-session-rerun) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin for inspecting and replaying completed main-agent and subagent session steps |
| 1092 | [Liyuan1992/memdsl](https://github.com/Liyuan1992/memdsl) | 0 | 2026-07-04 | 2026-09-02 | Agent memory as normative source code |
| 1093 | [Liyuan1992/rawmem](https://github.com/Liyuan1992/rawmem) | 0 | 2026-07-10 | 2026-09-02 | A tiny local-first raw evidence ledger for AI and human workflows. |
| 1094 | [ljc6413/pkg-dev](https://github.com/ljc6413/pkg-dev) | 0 | 2026-08-29 | 2026-08-30 | YiHe 编程认知内核 for DeepSeek Harness：27 领域包 + 55 RFB 经验库 + 工程工具链 + 商业/安全/进化体系（会进化的编程助手） |
| 1095 | [LJH-snow/dsh-tool-kubernetes](https://github.com/LJH-snow/dsh-tool-kubernetes) | 0 | 2026-08-27 | 2026-08-27 | Kubernetes tools for DeepSeek Harness: cluster, namespace, workload, pod, log, rollout, and manifest operations |
| 1096 | [LJH-snow/dsh-tool-monitoring](https://github.com/LJH-snow/dsh-tool-monitoring) | 0 | 2026-08-28 | 2026-08-28 | Prometheus and Alertmanager tool plugin for DeepSeek Harness |
| 1097 | [LJH-snow/dsh-tool-slack](https://github.com/LJH-snow/dsh-tool-slack) | 0 | 2026-08-30 | 2026-08-30 | Slack tools for DeepSeek Harness |
| 1098 | [ljh220300-eng/dsh-plugin-ssh-manager](https://github.com/ljh220300-eng/dsh-plugin-ssh-manager) | 0 | 2026-09-01 | 2026-09-01 | Manage multi-IP DSH instances from one terminal via SSH tunnels · 在一台终端上通过 SSH 隧道管理多 IP 的 DSH |
| 1099 | [ljlj7149-cloud/dsh-cognitio](https://github.com/ljlj7149-cloud/dsh-cognitio) | 0 | 2026-08-26 | 2026-08-27 | 纠错驱动的认知架构插件（DeepSeek Harness）：分层记忆 + 哨兵自动提醒 + 纠错进化 + 审批仲裁。让 AI 记得你的规矩，换模型换预设都有效；所有自动沉淀，你批准才生效。 |
| 1100 | [lkdxzhxi/dsh-glass-ui-theme](https://github.com/lkdxzhxi/dsh-glass-ui-theme) | 0 | 2026-08-29 | 2026-08-29 | 为 DeepSeek Harness 打造的液态玻璃主题插件：磨砂玻璃、可调色调、动态壁纸，让 DSH 界面焕然一新 |
| 1101 | [lnabc03/bright-drift](https://github.com/lnabc03/bright-drift) | 0 | 2026-08-31 | 2026-08-31 | Workspace drift awareness for AI coding agents — watches the workspace and injects a budgeted, attributed diff of external/user changes into the agent's context at each step boundary. |
| 1102 | [lnetrit-alt/dsh-system-control](https://github.com/lnetrit-alt/dsh-system-control) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: sidebar-embedded DeepSeek balance readout with a black minimalist full-shutdown button. |
| 1103 | [Lohaslee/dsh-super-pm](https://github.com/Lohaslee/dsh-super-pm) | 0 | 2026-09-01 | 2026-09-01 | Super PM product-thinking skill packaged as a DeepSeek Harness plugin |
| 1104 | [loiasdi/dsh-prompthub-ecosystem](https://github.com/loiasdi/dsh-prompthub-ecosystem) | 0 | 2026-08-26 | 2026-08-27 | PromptHub Ecosystem for DeepSeek Harness (DSH): bilingual Plugin and Skill catalog with GitHub and local tarball installation. |
| 1105 | [lokih1028/dsh-prompt-optimizer](https://github.com/lokih1028/dsh-prompt-optimizer) | 0 | 2026-08-29 | 2026-08-29 | One-click prompt enhancement and structuring plugin for DeepSeek Harness (DSH) |
| 1106 | [Lorvaste/DSH-Project-Initialization](https://github.com/Lorvaste/DSH-Project-Initialization) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：项目初始化插件，通过结构化的整理编排，需求与要素确认，无论是项目刚起步还是准备维护，都有一个好的开始. |
| 1107 | [lovstudio/dsh-llm-config](https://github.com/lovstudio/dsh-llm-config) | 0 | 2026-08-29 | 2026-08-29 | Reusable LLM configuration profile library exposed to browser consumers as a Remote (DeepSeek Harness plugin) |
| 1108 | [lovstudio/dsh-plugin-marketplace](https://github.com/lovstudio/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Local-first DeepSeek Harness plugin marketplace with GitHub and dshfind providers |
| 1109 | [lrplrplrp/dsh-sidebar-gdhighlight](https://github.com/lrplrplrp/dsh-sidebar-gdhighlight) | 0 | 2026-08-30 | 2026-08-31 | godot语法高亮，依赖dsh-better-sidebar |
| 1110 | [Luawig/dsh-cloudflare-access](https://github.com/Luawig/dsh-cloudflare-access) | 0 | 2026-08-27 | 2026-08-27 | Cloudflare Access JWT verification and remote privileged authorization for DeepSeek Harness |
| 1111 | [Lubaoshuai/dsh-notify](https://github.com/Lubaoshuai/dsh-notify) | 0 | 2026-08-30 | 2026-08-30 | Push notifications for DeepSeek Harness: agent-callable notify_send tool + external delivery for schedule reminders (Telegram/Slack/Discord/飞书/钉钉/Bark/ntfy/webhook). DSH plugin. |
| 1112 | [lucifergzsz414/dsh-windows-native](https://github.com/lucifergzsz414/dsh-windows-native) | 0 | 2026-08-31 | 2026-08-31 | Native-Windows (non-WSL) shell/encoding/filesystem gotchas for the DeepSeek Harness system prompt |
| 1113 | [Luisarg03/dsh-memory-vault](https://github.com/Luisarg03/dsh-memory-vault) | 0 | 2026-08-31 | 2026-09-01 | Memoria OKF persistente para DeepSeek Harness: MCP server (SQLite FTS5 + markdown) + plugins memory-mcp / memory-auto |
| 1114 | [LUMOGRESS/dsh-skill-navigator](https://github.com/LUMOGRESS/dsh-skill-navigator) | 0 | 2026-08-29 | 2026-08-29 | DSH skill quick-picker and manager: one-click quick-pick (categories/search/context recommendations) + management (categories/updates/expert packs/market/panel settings). DSH 技能速查+管理插件。 |
| 1115 | [luoghong/dsh-session-recorder](https://github.com/luoghong/dsh-session-recorder) | 0 | 2026-08-29 | 2026-08-30 | 记录和deek Harness对话记录为md格式 |
| 1116 | [luomeii/dsh-review-squad](https://github.com/luomeii/dsh-review-squad) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 并行多角色代码评审插件：/review 派出安全/正确性/测试/风格四名只读评审员子代理（可各自指定模型与思考强度），汇总为结构化报告。 |
| 1117 | [lussey820/dsh-essentials-bundle](https://github.com/lussey820/dsh-essentials-bundle) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) Web UI all-in-one essentials pack — a bundled collection, not a single-feature plugin: chat wallpaper / token usage stats / session manager / per-turn undo with artifact rollback / built-in file explorer & editor. Zero-dependency, inject-only, never overrides core. |
| 1118 | [luxi233/dsh-settings-nav-scroll](https://github.com/luxi233/dsh-settings-nav-scroll) | 0 | 2026-09-02 | 2026-09-02 | Adds vertical scrolling to the DSH Web settings navigation when sections exceed the viewport. |
| 1119 | [luxueliu/luxueliu-agent-discipline-skills](https://github.com/luxueliu/luxueliu-agent-discipline-skills) | 0 | 2026-08-25 | 2026-08-27 | AI 不缺聪明，缺纪律！交付前自检（没从磁盘回读不算完成）/跑偏纠偏（一句「你偏了」就停）/系统化调试（同一个修复猜三次不收敛时用）/多 agent 接力（防旧状态盖掉新写入）——4 个单文件技能零依赖，每条都来自真实翻车事故，DeepSeek Harness / Claude Code / Codex 通用 |
| 1120 | [luxueliu/luxueliu-intel-scout](https://github.com/luxueliu/luxueliu-intel-scout) | 0 | 2026-08-25 | 2026-08-27 | 每天自动巡 RSS：AI 简报 + 脑神经/意识简报，关键词过滤后压成速览+详情。DSH 插件；脚本仍是 Python / 计划任务。 |
| 1121 | [luyy9apples/dsh-workspace-memory](https://github.com/luyy9apples/dsh-workspace-memory) | 0 | 2026-08-31 | 2026-09-01 | Approval-gated workspace instructions and shared project memory for DeepSeek Harness |
| 1122 | [lyaoliu/dsh-reasoning-effort-slider](https://github.com/lyaoliu/dsh-reasoning-effort-slider) | 0 | 2026-08-29 | 2026-08-29 | DSH Desktop reasoning effort slider plugin - 7-level effort control with whale-mom skin |
| 1123 | [lylarcher/dsh-model-capabilities](https://github.com/lylarcher/dsh-model-capabilities) | 0 | 2026-08-29 | 2026-08-29 | 一个DSH插件，为自定义模型配置输入类型(input)、推理模式（reasoningEfforts） |
| 1124 | [lyuwen/dsh-as-service](https://github.com/lyuwen/dsh-as-service) | 0 | 2026-08-26 | 2026-08-27 | Running DSH as a service on the background |
| 1125 | [lyuwen/dsh-steer-button](https://github.com/lyuwen/dsh-steer-button) | 0 | 2026-08-26 | 2026-08-27 | Queue, Steer, and Backlog for DSH. More diverse way to interact with the agent while it's running. |
| 1126 | [lyuwen/dsh-thinking-summary](https://github.com/lyuwen/dsh-thinking-summary) | 0 | 2026-08-27 | 2026-08-27 | Readable thinking display for DeepSeek Harness |
| 1127 | [lyuwen/dsh-tui](https://github.com/lyuwen/dsh-tui) | 0 | 2026-08-28 | 2026-08-28 | [WIP] TUI for DeepSeeh-Harness |
| 1128 | [Lzh3070/dsh-search-hub](https://github.com/Lzh3070/dsh-search-hub) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 联网搜索多入口管理插件：DeepSeek 官方 / GLM（智谱）/ Kimi 多搜索模型共存，置顶一个web_search生效，设置页一键切换免重启 |
| 1129 | [LZMW/dsh-memory](https://github.com/LZMW/dsh-memory) | 0 | 2026-08-24 | 2026-08-28 | Persistent long-term memory plugin for DeepSeek Harness (dsh): single memory tool, markdown storage, auto session summary, curator governance, user-profile injection. |
| 1130 | [lzxcs/archive-vault-pro](https://github.com/lzxcs/archive-vault-pro) | 0 | 2026-08-26 | 2026-08-27 | 归档会话库：查看所有工作区的已归档会话、只读回看内容、右键取消归档（不影响官方逻辑）。 |
| 1131 | [lzxcs/btw-pro](https://github.com/lzxcs/btw-pro) | 0 | 2026-08-26 | 2026-08-27 | /btw 旁路问答：不打断当前会话（含流式输出中），基于当前上下文回答一个问题；答案以「旁答」命令结果行显示在主会话里，不进入主模型上下文。 |
| 1132 | [lzxcs/chat-width-pro](https://github.com/lzxcs/chat-width-pro) | 0 | 2026-08-26 | 2026-08-27 | 对话页面宽度设置：把固定的内容宽度暴露到设置页，默认 748px（应用当前宽度）。 |
| 1133 | [lzxcs/dsh-enter-swap](https://github.com/lzxcs/dsh-enter-swap) | 0 | 2026-08-26 | 2026-08-27 | Swap the web UI composer shortcuts: Ctrl/Meta+Enter inserts a newline, Shift+Enter sends. |
| 1134 | [lzxcs/dsh-tray-notify](https://github.com/lzxcs/dsh-tray-notify) | 0 | 2026-08-26 | 2026-08-27 | DSH → 托盘通知：agent 停顿 / 提问 / 计划审批 / 授权时调用 notify-sender.py 弹窗（--source dsh，托盘按蓝色主题区分于 Claude Code）。纯 node 侧插件。 |
| 1135 | [lzxcs/edit-diff-pro](https://github.com/lzxcs/edit-diff-pro) | 0 | 2026-08-26 | 2026-08-27 | Claude Code 风格的 edit/write diff 卡片：±3 行上下文、绝对行号、可配置默认展开（默认折叠）。 |
| 1136 | [lzxcs/file-diff-pro](https://github.com/lzxcs/file-diff-pro) | 0 | 2026-08-26 | 2026-08-27 | 产物文件点击弹窗查看本轮 diff（代码类文件）；非代码文件维持桌面打开。 |
| 1137 | [lzxcs/lag-trace-pro](https://github.com/lzxcs/lag-trace-pro) | 0 | 2026-08-26 | 2026-08-27 | DSH web UI performance recorder: auto-captures page jank (long animation frames, long tasks, frame freezes) with context snapshots, stored under ~/.dsh/perf/ |
| 1138 | [lzxcs/paste-file-path-pro](https://github.com/lzxcs/paste-file-path-pro) | 0 | 2026-08-26 | 2026-08-27 | Pasting non-image files into the web composer inserts their paths as @file references (host-side clipboard reading). |
| 1139 | [m1452700576/dsh-app-updater](https://github.com/m1452700576/dsh-app-updater) | 0 | 2026-08-26 | 2026-09-01 | 更新dsh客户端 |
| 1140 | [Macorreag/dsh-monitor](https://github.com/Macorreag/dsh-monitor) | 0 | 2026-09-02 | 2026-09-02 | Monitor plugin for DeepSeek Harness: background bash watchers that steer the agent loop, with a live dock status bar. |
| 1141 | [magian1127/deepseek-harness-zcode_mask](https://github.com/magian1127/deepseek-harness-zcode_mask) | 0 | 2026-09-01 | 2026-09-01 | 将 ZCode 桌面 App 登录的 Coding Plan 模型接入 DeepSeek Harness，请求头与 ZCode 完全一致 — bring ZCode coding-plan models into DeepSeek Harness with byte-identical request headers. |
| 1142 | [maiziman/cedardsh-model-probe](https://github.com/maiziman/cedardsh-model-probe) | 0 | 2026-08-31 | 2026-08-31 | CedarDSH Model Probe — Detects reasoning and image support for custom DeepSeek Harness models. |
| 1143 | [MannixHu/dsh-statusbar-config](https://github.com/MannixHu/dsh-statusbar-config) | 0 | 2026-09-02 | 2026-09-02 | 用 ${变量} 模板完全自定义 DeepSeek Harness 状态栏统计行 · template-driven DSH status bar |
| 1144 | [mapan0424/deepseek-harness-channels](https://github.com/mapan0424/deepseek-harness-channels) | 0 | 2026-08-28 | 2026-08-28 | Community channel plugins for DeepSeek Harness: core, visual config, and Feishu channel. |
| 1145 | [MarceloSenai/dsh-plugin-kie-ai](https://github.com/MarceloSenai/dsh-plugin-kie-ai) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: image and video generation over the KIE AI API |
| 1146 | [MarchLiu/dsh-farm](https://github.com/MarchLiu/dsh-farm) | 0 | 2026-09-02 | 2026-09-02 | DSH service farm: register, start, stop, restart and watch long-running project services — agent tools + overview drawer UI, farm.yaml support |
| 1147 | [MarchLiu/dsh-uno-office](https://github.com/MarchLiu/dsh-uno-office) | 0 | 2026-09-02 | 2026-09-02 | LibreOffice (UNO) powered high-fidelity office engine for DSH — create & edit docx/xlsx/pptx via prompts, with human-in-the-loop review |
| 1148 | [MaRi23333/dsh-serverchan-watchdog](https://github.com/MaRi23333/dsh-serverchan-watchdog) | 0 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 的 Server酱推送插件：审批、计划评审或问答超时未处理时，发送微信/Server酱³ App 提醒。第三方非官方项目。 |
| 1149 | [markelayan/dsh-taskboard-flow](https://github.com/markelayan/dsh-taskboard-flow) | 0 | 2026-08-31 | 2026-09-01 | Companion plugin to dsh-taskboard (DeepSeek Harness): kanban flow engine + cross-session messaging. File-based config, local-only, no telemetry. |
| 1150 | [masknull/dsh-message-collapse](https://github.com/masknull/dsh-message-collapse) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin: auto-collapse long user messages in the web chat. 用户消息超10行自动折叠。 |
| 1151 | [masknull/dsh-workspace-default-path](https://github.com/masknull/dsh-workspace-default-path) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：添加工作区时记住上次使用的目录，下次打开浏览对话框直接定位（预填+自动记忆，官方流程不动）。DSH plugin: remember the last used workspace directory for Add workspace - prefill + auto-memory over the official flow. |
| 1152 | [Mason-1011/dsh-schematic](https://github.com/Mason-1011/dsh-schematic) | 0 | 2026-08-25 | 2026-08-30 | Live plugin-topology viewer for DeepSeek Harness — the wiring diagram of mounted plugins, their runtime activity, and a composer-side star map. Pure observer. |
| 1153 | [MasterBenC/shangshi-dsh](https://github.com/MasterBenC/shangshi-dsh) | 0 | 2026-08-31 | 2026-08-31 | Shangshi DeepSeek Harness plugin for local Qimen business timing. |
| 1154 | [MauricioPerera/kdd-gates](https://github.com/MauricioPerera/kdd-gates) | 0 | 2026-08-27 | 2026-08-27 | KDD methodology gates as DeepSeek Harness (dsh) plugin tools |
| 1155 | [mc856/dsh-project-portfolio](https://github.com/mc856/dsh-project-portfolio) | 0 | 2026-08-31 | 2026-08-31 | Unofficial DSH plugin: long-term, cross-project memory for coding agents — embedded project-portfolio skill + portfolio_status/portfolio_log tools over plain markdown. Not affiliated with DeepSeek. |
| 1156 | [me9rez/dsh-pwsh-style](https://github.com/me9rez/dsh-pwsh-style) | 0 | 2026-08-28 | 2026-08-28 | 修改 DSH 会话回复中 pwsh(PowerShell) 工具卡片的主题、字体与可读性增强。Restyle pwsh tool-call cards in DSH: themes, system fonts, copy & expand, workdir display. |
| 1157 | [MEMZ-Edge01/GrokBot_in_DeepseekHerness](https://github.com/MEMZ-Edge01/GrokBot_in_DeepseekHerness) | 0 | 2026-08-22 | 2026-08-31 | 将GrokBot宠物代入DSH网页端并加入拖拽效果和通知功能 |
| 1158 | [mengruoa/dsh-rembg](https://github.com/mengruoa/dsh-rembg) | 0 | 2026-08-21 | 2026-09-01 | DSH plugin: auto-install rembg and expose a background-removal tool to the LLM |
| 1159 | [Mengshang-spec/dsh-third-party-api-balance-wallet](https://github.com/Mengshang-spec/dsh-third-party-api-balance-wallet) | 0 | 2026-08-27 | 2026-08-27 | 第三方 API 接入 DSH 查询余额插件 |
| 1160 | [mervin1944/dsh-version-badge](https://github.com/mervin1944/dsh-version-badge) | 0 | 2026-08-31 | 2026-08-31 | DSH 版本号徽标插件：侧边栏设置按钮上方显示 dsh 版本，带检查更新与一键部署。DSH version badge plugin with update check & one-click deploy. |
| 1161 | [metabolism-tools/workspace-metabolism](https://github.com/metabolism-tools/workspace-metabolism) | 0 | 2026-08-15 | 2026-08-31 | Govern what Claude Code, Codex, Aider and OpenClaw leave in your workspace: one JSON policy file, audit, recyclable clean, rollback, hash-chained audit trail. |
| 1162 | [meyaomiao/dsh-files-native](https://github.com/meyaomiao/dsh-files-native) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件：接近原生质感的附件上传（拖入/粘贴/回形针，图片与文件混排） |
| 1163 | [MichaelGong/dsh-session-hover-preview](https://github.com/MichaelGong/dsh-session-hover-preview) | 0 | 2026-08-27 | 2026-08-27 | Codex-style user-message navigation for DeepSeek Harness conversations |
| 1164 | [Mide69/dsh-boot-doctor](https://github.com/Mide69/dsh-boot-doctor) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: console log sink and stuck-plugin warnings |
| 1165 | [Milbaxter/dsh-critique-loop](https://github.com/Milbaxter/dsh-critique-loop) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin: forces one critique-and-improve round after each completed turn. |
| 1166 | [minatoAI/dsh-net-proxy-plugin](https://github.com/minatoAI/dsh-net-proxy-plugin) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness fallback network proxy plugin: detects system proxies, probes overseas connectivity (Google/GitHub), routes dsh outbound HTTP through a working local proxy |
| 1167 | [mingzhong15/dsh-cursor-passthrough](https://github.com/mingzhong15/dsh-cursor-passthrough) | 0 | 2026-08-27 | 2026-08-27 | Add a Cursor passthrough group to the DSH chat model picker. |
| 1168 | [Missher12/dsh-project-ops](https://github.com/Missher12/dsh-project-ops) | 0 | 2026-08-27 | 2026-08-27 | Scoped project task discovery and execution receipts for DeepSeek Harness |
| 1169 | [ml020/dsh-workbuddy](https://github.com/ml020/dsh-workbuddy) | 0 | 2026-08-28 | 2026-08-28 | Wordless-styled WorkBuddy hero for DSH: replaces the blank-session brand mark and workspace picker while keeping the native composer. |
| 1170 | [mnbvcxzaqwertyuioplm/dsh-memory](https://github.com/mnbvcxzaqwertyuioplm/dsh-memory) | 0 | 2026-09-01 | 2026-09-01 | DSH 跨会话语义记忆插件：智谱 embedding-3 + SQLite，提供 memory_add / memory_search 语义召回；配置可选、绝不因缺 key/缺库/缺服务而崩。 |
| 1171 | [mohith-das/dsh-client-ui-model-selection-search](https://github.com/mohith-das/dsh-client-ui-model-selection-search) | 0 | 2026-09-01 | 2026-09-01 | Fork of DeepSeek Harness's official model picker (@deepseek-ai/dsh-client-ui-model-selection) adding an in-menu search box to filter models by name, provider, or id. |
| 1172 | [mohith-das/dsh-voice-input-en](https://github.com/mohith-das/dsh-voice-input-en) | 0 | 2026-09-01 | 2026-09-01 | Minimal, English-only voice input plugin for DeepSeek Harness Web UI — a mic button in the composer using the browser's native SpeechRecognition API. Zero dependencies, no subprocess, no tracking. |
| 1173 | [Momojie-S/dsh-archive-retention](https://github.com/Momojie-S/dsh-archive-retention) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件: 归档会话定期清理 —— 物理归档堆与页面归档会话超保留期(页面可配天/小时,cron 调度)自动物理删除 |
| 1174 | [moonwellxh/DSH-Launcher](https://github.com/moonwellxh/DSH-Launcher) | 0 | 2026-08-27 | 2026-08-30 | DSH 魔偶助手（DSH一键启动托盘）(DeepSeek Harness launcher / tray) |
| 1175 | [morphlinglan/dsh-leopard-gecko](https://github.com/morphlinglan/dsh-leopard-gecko) | 0 | 2026-08-28 | 2026-08-28 | 豹纹守宫旅行桌宠小插件：一只会自己出门旅行、寄回明信片、带回特产的守宫。庭院三叶草随时间生长，收割后可在商店购买便当与护身符。 |
| 1176 | [mrme000m/dsh-prime-orchestrator](https://github.com/mrme000m/dsh-prime-orchestrator) | 0 | 2026-09-01 | 2026-09-02 | Prime Agent orchestration for DeepSeek Harness (dsh): delegation engine, prime_agent tool, Web fleet column, settings section, and the prime-orchestrator agent preset — one installable plugin package |
| 1177 | [MST19711/dsh-balance-panel](https://github.com/MST19711/dsh-balance-panel) | 0 | 2026-08-21 | 2026-09-02 | Floating Balance Panel for the DSH Web UI — live remaining % for the 5h / weekly / monthly windows, supporting OpenCode Go and Z.AI-CN |
| 1178 | [MST19711/dsh-session-files](https://github.com/MST19711/dsh-session-files) | 0 | 2026-08-31 | 2026-09-01 | Upload arbitrary files into a DSH session workspace (uploads/<sessionId>/) and let the agent deliver result files as clickable download cards in the conversation. |
| 1179 | [mtdx2001/dsh-think-translate](https://github.com/mtdx2001/dsh-think-translate) | 0 | 2026-08-29 | 2026-08-29 | Display-layer translation for the DeepSeek Harness Web UI: thinking chain, task cards and answers in 8 languages - pure display layer, originals untouched, local-first with failover. |
| 1180 | [my-dsh/dsh-session-attention](https://github.com/my-dsh/dsh-session-attention) | 0 | 2026-08-28 | 2026-08-28 | Session attention overlay plugin for DeepSeek Harness: character dance animation while any session awaits user action |
| 1181 | [my-dsh/dsh-token-usage-dashboard](https://github.com/my-dsh/dsh-token-usage-dashboard) | 0 | 2026-08-28 | 2026-08-28 | Cross-session token usage dashboard plugin for DeepSeek Harness: SQLite-backed capture + browser dashboard panel |
| 1182 | [mycodesite/dsh-rules](https://github.com/mycodesite/dsh-rules) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (dsh) 插件：全局+项目两级 Markdown 规则注入（RuleBase） |
| 1183 | [myk5010/dsh-kimi](https://github.com/myk5010/dsh-kimi) | 0 | 2026-09-02 | 2026-09-02 | Kimi (Kimi Code account) integration bundle for DeepSeek Harness: provider route, models, device-code login and auto token refresh |
| 1184 | [mykeura/dsh-minimalist-themes](https://github.com/mykeura/dsh-minimalist-themes) | 0 | 2026-08-26 | 2026-08-27 | 18 minimalist color themes for DeepSeek Harness. Pick one with a single click — it's just another plugin. |
| 1185 | [n8guru/dsh-self-preserve](https://github.com/n8guru/dsh-self-preserve) | 0 | 2026-09-02 | 2026-09-02 | DSH hook plugin: a session may not stop the harness it runs inside |
| 1186 | [NattoCB/dsh-plugin-sidebar-views](https://github.com/NattoCB/dsh-plugin-sidebar-views) | 0 | 2026-08-31 | 2026-08-31 | Sidebar views switcher for DeepSeek Harness: workspaces / recent sessions, pinned sessions group, per-row pin & copy-session-id menu |
| 1187 | [NattoCB/dsh-safe-delete](https://github.com/NattoCB/dsh-safe-delete) | 0 | 2026-09-01 | 2026-09-01 | DSH plugin: intercept agent rm in every bash session and move targets to the macOS Trash instead |
| 1188 | [navid-kianfar/dsh-memory](https://github.com/navid-kianfar/dsh-memory) | 0 | 2026-08-26 | 2026-08-27 | Persistent, searchable, per-project memory for the DeepSeek Harness: decisions, rules, and session context in a queryable DuckDB file, with the rule set injected into every model request — plus a full management UI in the Web Client. |
| 1189 | [navid-kianfar/dsh-worktree](https://github.com/navid-kianfar/dsh-worktree) | 0 | 2026-08-26 | 2026-08-27 | Git worktrees and branches for the DeepSeek Harness Web Client: a session-header chip that switches branches, creates worktrees, and opens them as harness workspaces. |
| 1190 | [NecromanAlbert/dsh-i-have-adhd](https://github.com/NecromanAlbert/dsh-i-have-adhd) | 0 | 2026-08-26 | 2026-08-27 | Always-on ADHD-friendly output for every DeepSeek Harness session. Host systemPrompt, not a skill catalog item. |
| 1191 | [NecromanAlbert/dsh-self-restart](https://github.com/NecromanAlbert/dsh-self-restart) | 0 | 2026-08-26 | 2026-08-27 | Any DSH session can request a Desktop restart, then the same persisted session is resumed and followup'd with its mission. |
| 1192 | [NexusAgentX/dsh-advisor](https://github.com/NexusAgentX/dsh-advisor) | 0 | 2026-08-23 | 2026-08-27 | dsh plugin bundle porting the rpiv advisor subsystem: an on-demand zero-parameter advisor() tool that forwards the full session to a separately-configured reviewer model. |
| 1193 | [nicecx/dsh-auto-approver](https://github.com/nicecx/dsh-auto-approver) | 0 | 2026-08-31 | 2026-08-31 | Configurable auto-approval for DeepSeek Harness: intercepts approval/request and answers allowed-once/rejected by policy (allow-all/allowlist/off + denyAlways), with a full audit log. |
| 1194 | [nicecx/dsh-reset-handoff](https://github.com/nicecx/dsh-reset-handoff) | 0 | 2026-08-30 | 2026-08-30 | DSH never restarts itself: host plugin that hands reset requests to an external ops agent (e.g. Hermes) via a versioned JSON protocol — preflight → gate → restart → health-check → recover → deliver back |
| 1195 | [nicecx/dsh-task-queue](https://github.com/nicecx/dsh-task-queue) | 0 | 2026-08-31 | 2026-08-31 | Tiered task queue for DSH↔Hermes: queue.json single source of truth, lease/claim model, concurrency-1; Hermes-side cron consumes, DSH-side enqueues. Includes busy-mutex for the approve fast path. |
| 1196 | [nickkkkkk123123/dsh-resume-on-restart](https://github.com/nickkkkkk123123/dsh-resume-on-restart) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：重启后自动唤醒 agent 并投递信息性消息，agent 自主决定是否恢复工作 |
| 1197 | [ningbonb/dsh-installer](https://github.com/ningbonb/dsh-installer) | 0 | 2026-08-31 | 2026-09-01 | One-click installers for DeepSeek Harness (dsh) on macOS and Windows |
| 1198 | [NinjaSln-labs/dsh-context-compass](https://github.com/NinjaSln-labs/dsh-context-compass) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness 会话健康插件：真实数据的「继续 vs 新开」上下文罗盘——头部徽章 / /compass / context_compass 工具 / 多会话一览面板 |
| 1199 | [niushuanan/dsh-adaptive-update](https://github.com/niushuanan/dsh-adaptive-update) | 0 | 2026-08-26 | 2026-08-27 | Check upstream manually or every six hours, use a narrowly scoped agent for compatibility work, and switch atomically with rollback. |
| 1200 | [niushuanan/dsh-chat-migration](https://github.com/niushuanan/dsh-chat-migration) | 0 | 2026-08-29 | 2026-08-29 | Native DeepSeek chat migration and workspace-free chat mode for DeepSeek Harness |
| 1201 | [niushuanan/dsh-image-vision](https://github.com/niushuanan/dsh-image-vision) | 0 | 2026-08-26 | 2026-08-27 | Let vision-capable models read native attachments while giving text-only models an image tool that supports follow-up questions. |
| 1202 | [niushuanan/dsh-model-usage](https://github.com/niushuanan/dsh-model-usage) | 0 | 2026-08-26 | 2026-08-27 | Inspect model quotas, periods, and refresh state by provider in Settings, with data loaded only when the user opens the page. |
| 1203 | [niushuanan/dsh-multi-window](https://github.com/niushuanan/dsh-multi-window) | 0 | 2026-08-26 | 2026-08-27 | Open multiple independent conversations side by side, each with isolated navigation, drafts, and runtime state. |
| 1204 | [niushuanan/dsh-parallel-worktree](https://github.com/niushuanan/dsh-parallel-worktree) | 0 | 2026-08-26 | 2026-08-27 | Move parallel tasks into isolated Git worktrees, inspect conflicts, and merge the results safely into the current branch. |
| 1205 | [niushuanan/dsh-pure-chat](https://github.com/niushuanan/dsh-pure-chat) | 0 | 2026-08-26 | 2026-08-27 | Start a chat immediately without a workspace, work mode, or execution permissions while keeping image and text-file uploads. |
| 1206 | [niushuanan/dsh-selection-memory](https://github.com/niushuanan/dsh-selection-memory) | 0 | 2026-08-26 | 2026-08-27 | Quote, discuss, or remember selected conversation text, then maintain durable context in separate editable user and AI memories. |
| 1207 | [niushuanan/dsh-skill-manager](https://github.com/niushuanan/dsh-skill-manager) | 0 | 2026-08-26 | 2026-08-27 | Browse installed Skills, their files, and content in Settings, then adaptively import from a file, folder, ZIP, or GitHub with AI. |
| 1208 | [niushuanan/dsh-teamwork](https://github.com/niushuanan/dsh-teamwork) | 0 | 2026-08-26 | 2026-08-27 | Run collaborating agents and external experts concurrently under one coordinating agent, then bring every result back into the current task. |
| 1209 | [niushuanan/dsh-token-overview](https://github.com/niushuanan/dsh-token-overview) | 0 | 2026-08-26 | 2026-08-27 | See tokens, cache usage, calls, active periods, and estimated cost across AI clients on the whole computer. |
| 1210 | [niushuanan/dsh-whale-girl](https://github.com/niushuanan/dsh-whale-girl) | 0 | 2026-08-26 | 2026-08-27 | Add a native cross-page companion whose presence, shortcuts, and feedback follow the current DSH session state. |
| 1211 | [njuptlzf/dsh-ponytail](https://github.com/njuptlzf/dsh-ponytail) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 插件：常驻注入 Ponytail 懒高级工程师规范，5 个同伴技能落盘为可调用的 skill。安装：dsh plugin add github:njuptlzf/dsh-ponytail |
| 1212 | [nmsl1234/dsh-privacy-gate](https://github.com/nmsl1234/dsh-privacy-gate) | 0 | 2026-08-31 | 2026-08-31 | dsh-plugin |
| 1213 | [NoelJudeNoel/dshost-plugin](https://github.com/NoelJudeNoel/dshost-plugin) | 0 | 2026-09-01 | 2026-09-01 | Official remote cloud relay plugin for DSHost (dshost.me): securely access your dsh Web UI from anywhere |
| 1214 | [NOirBRight/dsh-mobile-pairing](https://github.com/NOirBRight/dsh-mobile-pairing) | 0 | 2026-08-21 | 2026-08-29 | DSH Mobile Remote pairing plugin |
| 1215 | [NOirBRight/dsh-plugins](https://github.com/NOirBRight/dsh-plugins) | 0 | 2026-08-29 | 2026-08-30 | Independent catalog of DSH plugins and mobile companion published by NOirBRight |
| 1216 | [northern-penguin/dsh-h3-seg-prompt-design](https://github.com/northern-penguin/dsh-h3-seg-prompt-design) | 0 | 2026-09-02 | 2026-09-02 | 一个DeepSeekHarness插件，用于让模型在DeepSeekHarness中生成符合H3视频生成模型规范的提示词。该提示词可以直接用于Theodore_Director导播台的分镜设计中。 |
| 1217 | [Nth-5620/dsh-crystal-viewer](https://github.com/Nth-5620/dsh-crystal-viewer) | 0 | 2026-08-29 | 2026-08-30 | A crystal-structure visualization window for DeepSeek Harness: 3D structure + Q-peak viewer and parameter panel, opened as a dsh-better-sidebar tab. |
| 1218 | [null-object-0000/dsh-output-style](https://github.com/null-object-0000/dsh-output-style) | 0 | 2026-08-31 | 2026-08-31 | 会话级输出风格插件：/style 命令 + Web 选择器，改变模型如何呈现答案（default/adhd-friendly/eli5/bluf）。Session-scoped output styles for DeepSeek Harness. |
| 1219 | [NyaaCaster/dsh-yuque-kb](https://github.com/NyaaCaster/dsh-yuque-kb) | 0 | 2026-08-24 | 2026-08-28 | dsh web插件，语雀文档知识库化在dsh中调用 |
| 1220 | [odelbos/dsh-models-filter](https://github.com/odelbos/dsh-models-filter) | 0 | 2026-08-29 | 2026-08-31 | DeepSeek Harness plugin used to add an input filed to filter the models menu. (with arrow up/down + enter) |
| 1221 | [oh-my-engine/dsh-plugin-oh-my-engine](https://github.com/oh-my-engine/dsh-plugin-oh-my-engine) | 0 | 2026-09-02 | 2026-09-02 | Approval-gated OME engineering delivery Agent Preset for DeepSeek Harness |
| 1222 | [oh-summy/dsh-remote-control](https://github.com/oh-summy/dsh-remote-control) | 0 | 2026-08-30 | 2026-08-30 | Secure remote access for DeepSeek Harness (DSH): Cloudflare Tunnel + password gate + Feishu notifications. macOS first, Linux first-class. |
| 1223 | [Oissp/harness-desktop](https://github.com/Oissp/harness-desktop) | 0 | 2026-08-26 | 2026-09-02 | DeepSeek Harness Desktop for Debian |
| 1224 | [Olina1Ye/internal-skill-workshop-plugin](https://github.com/Olina1Ye/internal-skill-workshop-plugin) | 0 | 2026-08-27 | 2026-08-27 | A read-only DeepSeek Harness Web plugin for browsing a configured Skill Base catalog. |
| 1225 | [Oliver0804/dsh-openrouter-monitor](https://github.com/Oliver0804/dsh-openrouter-monitor) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: OpenRouter account balance, per-key spend, alert thresholds and trend charts under the composer. |
| 1226 | [Oliver0804/dsh-peak-pricing](https://github.com/Oliver0804/dsh-peak-pricing) | 0 | 2026-08-17 | 2026-08-27 | DSH plugin: DeepSeek peak/off-peak pricing, flat rates for other providers like z-ai/glm-5.3-flash, live per-session cost estimate and a hover cache-hit trend chart. |
| 1227 | [Olympianz/dsh-deploy-master](https://github.com/Olympianz/dsh-deploy-master) | 0 | 2026-08-30 | 2026-08-30 | A DSH deploy-assistant plugin: GitHub publish + Linear sync + npm publish + community announcement. |
| 1228 | [Olympianz/dsh-heatmap](https://github.com/Olympianz/dsh-heatmap) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 页面埋点与热力图分析插件：科学埋点采集、本地热力图与统计、CLI/HTTP 接口、上传授权。 |
| 1229 | [onclaw-dev/dsh-ima-copilot](https://github.com/onclaw-dev/dsh-ima-copilot) | 0 | 2026-08-30 | 2026-08-30 | 腾讯 IMA 是一个非常好的知识库应用，但是他们提供的skill版本针对公开知识库的检索方式只提供了基于文件标题的关键字检索，好一阵无语。为了补足在harness的这种知识库检索能力，基于tencent-ima-copilot-mcp迭代了对应的dsh版本。 |
| 1230 | [onclaw-dev/dsh-workflow-designer](https://github.com/onclaw-dev/dsh-workflow-designer) | 0 | 2026-08-31 | 2026-08-31 | `dsh-workflow-designer` 是面向 DeepSeek Harness 的提示词优先工作流设计插件。它收集当前 Agent 可见的本地 Skill、原生 Tool 与 MCP Tool，提供必要的可视化编排和约束编辑能力，并导出稳定的 YAML 中间表示。后续可由大模型及对应框架把 YAML 生成 Python、`workflow.mjs` 或其他代码工作流。 |
| 1231 | [opdsh/unity-plugin](https://github.com/opdsh/unity-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: control the Unity Editor through the unity CLI |
| 1232 | [Oscar-Williams/dsh-deepcanary](https://github.com/Oscar-Williams/dsh-deepcanary) | 0 | 2026-08-29 | 2026-08-30 | Local attention supervision for DeepSeek Harness: evidence-first signals, quiet notifications, and an actionable inbox. |
| 1233 | [oThTJx/dsh-always-apply](https://github.com/oThTJx/dsh-always-apply) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: injects alwaysApply-marked skill bodies into sessions before the first model request — no skill tool load needed. |
| 1234 | [oThTJx/dsh-superpowers](https://github.com/oThTJx/dsh-superpowers) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: obra/superpowers skill library adapted to dsh tooling, plus a session-start bootstrap — brainstorming, systematic debugging, TDD, planning and more. |
| 1235 | [oxlyn/dsh-flyout-sidebar](https://github.com/oxlyn/dsh-flyout-sidebar) | 0 | 2026-08-29 | 2026-09-02 | deepseek harness flyout sidebar |
| 1236 | [pacoyi/dsh-memory-lite](https://github.com/pacoyi/dsh-memory-lite) | 0 | 2026-08-28 | 2026-08-28 | Lightweight cross-session memory plugin for DeepSeek Harness: approval-gated `memory` tool (save/recall/list/forget) + Settings card UI to browse, add, delete (two-click, trash/restore) and idempotent import/export. \| DeepSeek Harness 跨会话记忆插件：审批门控 memory 工具 + 设置页UI「记忆库」卡片（查看/新增/删除、两击确认、回收站恢复、导入/导出记忆——幂等迁移、冲突拒绝）。 |
| 1237 | [PaidaxingTuT/dsh-code-runner](https://github.com/PaidaxingTuT/dsh-code-runner) | 0 | 2026-08-29 | 2026-08-29 | 在 DSH-better-sidebar 中一键运行侧边栏代码文件，让代码可以在dsh终端中运行 |
| 1238 | [Parker-xia/dsh-research-refs](https://github.com/Parker-xia/dsh-research-refs) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: tidy messy pasted citations into uniformly formatted references (refs_parse / refs_verify / refs_dedup / refs_format + research-refs skill) |
| 1239 | [pauloapoloni/dsh-pr-checks](https://github.com/pauloapoloni/dsh-pr-checks) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: status and progress of GitHub Actions checks for open PRs, in the sidebar footer. |
| 1240 | [pbwheel/dsh-agency-market](https://github.com/pbwheel/dsh-agency-market) | 0 | 2026-09-01 | 2026-09-01 | 把 agency-agents 中的 273 个专业智能体装进 DeepSeek Harness，类似 workbuddy 中的专家 |
| 1241 | [peikuo/dayreel](https://github.com/peikuo/dayreel) | 0 | 2026-08-30 | 2026-08-30 | Dayreel — a DeepSeek Harness (dsh) community plugin: turn your day of work sessions into a designed daily report + a narrated summary video. |
| 1242 | [peiyucn/dsh-sparrow](https://github.com/peiyucn/dsh-sparrow) | 0 | 2026-08-30 | 2026-08-30 | A collection of small DeepSeek Harness (DSH) web plugins: chat input suggestions, an image-vision channel for text-only models, and archived-session management. |
| 1243 | [perinchiang/dsh-memory-dashboard](https://github.com/perinchiang/dsh-memory-dashboard) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness embedded read-only viewer for TencentDB Agent Memory's four-layer local memory |
| 1244 | [PerryLink/dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) | 0 | 2026-08-29 | 2026-08-30 | Community certification spec and registry for DeepSeek Harness plugins: five machine-checkable dimensions, A-D grades, and a security veto. |
| 1245 | [PerryLink/dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) | 0 | 2026-08-26 | 2026-08-27 | Shared zero-runtime-dependency toolkit for PerryLink DSH plugins: a pluggable Provider registry seam, fail-closed approval and adaptive session-event gates, mechanical verify scripts, shared sanitize/pricing/judge modules, and a new-plugin skeleton. |
| 1246 | [PerryLink/dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | 0 | 2026-08-26 | 2026-08-27 | Zero-dependency static portal rendering the @perrylink DeepSeek Harness plugin ecosystem as grouped cards: one page, no build step, no runtime framework. |
| 1247 | [PerryLink/perrylink](https://github.com/PerryLink/perrylink) | 0 | 2026-08-16 | 2026-08-30 | DeepSeek Harness ecosystem: 33 plugins - second-model approval, permission rules, memory, MCP panel, supply-chain security & certification |
| 1248 | [phungthien269/dsh-token-stats](https://github.com/phungthien269/dsh-token-stats) | 0 | 2026-09-01 | 2026-09-02 | Token usage dashboard for the DeepSeek Harness web GUI - today/week/month totals, per-model breakdown, 4-language UI. Read-only over the Wallet ledger. |
| 1249 | [Physicolor/dsh-lifeline](https://github.com/Physicolor/dsh-lifeline) | 0 | 2026-09-01 | 2026-09-02 | Right-side message navigation rail for DeepSeek Harness — per-message ticks, hover preview, smooth jump, star bookmarks, realtime slide animation |
| 1250 | [ping1999/dsh-minimap](https://github.com/ping1999/dsh-minimap) | 0 | 2026-08-29 | 2026-08-29 | VS Code-style minimap (text thumbnail + draggable viewport) overlay for the dsh web GUI's side file viewer |
| 1251 | [pipipigu/dsh-ssh-control](https://github.com/pipipigu/dsh-ssh-control) | 0 | 2026-08-28 | 2026-08-28 | Unified, non-intrusive SSH control center for DeepSeek Harness (DSH) |
| 1252 | [pixellover1433/dsh-plugin-dev-skills](https://github.com/pixellover1433/dsh-plugin-dev-skills) | 0 | 2026-08-30 | 2026-08-30 | This set of skills allows your agent to create plugins for Deepseek Harness. |
| 1253 | [plastic-labs/dsh-honcho](https://github.com/plastic-labs/dsh-honcho) | 0 | 2026-08-31 | 2026-09-02 | Honcho integration for the DeepSeek Harness |
| 1254 | [plumbkit/dsh-plumb-identity](https://github.com/plumbkit/dsh-plumb-identity) | 0 | 2026-09-01 | 2026-09-02 | Per-agent plumb session identity for DeepSeek Harness: every conversation, workspace, and subagent gets its own stable plumb session id on a shared plumb MCP connection |
| 1255 | [PlusQi/dsh-plugins](https://github.com/PlusQi/dsh-plugins) | 0 | 2026-08-28 | 2026-08-27 | 个人 DeepSeek Harness (DSH) 插件集 |
| 1256 | [pn1024/dsh-skill-hub](https://github.com/pn1024/dsh-skill-hub) | 0 | 2026-09-01 | 2026-09-01 | dsh plugin - skill marketplace (SkillHub + ClawHub) with sidebar entry, overlay panel, and chat input quick-pick |
| 1257 | [PolinniZhong/dsh-skill-trace](https://github.com/PolinniZhong/dsh-skill-trace) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Skill 追踪：看清 Agent 实际加载的 Skill，把运行过程变成可复看、可学习的本地收据。 |
| 1258 | [pricklywiggles/dsh-circuit-breaker](https://github.com/pricklywiggles/dsh-circuit-breaker) | 0 | 2026-09-02 | 2026-09-02 | Loop guard for DeepSeek Harness: denies repeated identical tool calls and caps per-agent calls, outside the model where instructions cannot reach |
| 1259 | [Proton1917/dsh-harness-plugin](https://github.com/Proton1917/dsh-harness-plugin) | 0 | 2026-08-17 | 2026-08-28 | Independent TypeScript plugins for DeepSeek Harness: live stats, Web UI customization, and a medical Fable mode |
| 1260 | [publieople/dsh-omniroute-models](https://github.com/publieople/dsh-omniroute-models) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: searchable/filterable model manager for OmniRoute (or any OpenAI-compatible gateway) — provider directory, modality discovery, multi-select enable. |
| 1261 | [Q-xuan/dsh-authmux](https://github.com/Q-xuan/dsh-authmux) | 0 | 2026-09-01 | 2026-09-01 | One login plane for subscription-backed model providers in DeepSeek Harness |
| 1262 | [QChengW/dsh-conversation-shortcuts](https://github.com/QChengW/dsh-conversation-shortcuts) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin for conversation keyboard shortcuts |
| 1263 | [qgx1992/dsh-model-select-style](https://github.com/qgx1992/dsh-model-select-style) | 0 | 2026-08-27 | 2026-08-27 | DSH web 插件：把输入框模型选择控件替换为两个独立按钮（供应商 + 模型两级联动，支持推理等级调节） |
| 1264 | [qgx1992/dsh-notify](https://github.com/qgx1992/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | DSH 通知显示层插件：全局 toast 栈，订阅桌面壳 __dshExo 桥事件，点击经官方 sessions runtime 程序化激活会话；无壳时降级订阅 sessions store 自绘。可插拔通知显示层的 web 侧。 |
| 1265 | [QianLuo-Ly/dsh-weather](https://github.com/QianLuo-Ly/dsh-weather) | 0 | 2026-09-02 | 2026-09-02 | dsh的天气插件（没有高大上的东西，生活不易，出门记得看天气~） |
| 1266 | [qigelunbiya/dsh-ssh-files-sidebar](https://github.com/qigelunbiya/dsh-ssh-files-sidebar) | 0 | 2026-08-26 | 2026-09-02 | Remote SSH workspace & deployment Agent for DeepSeek Harness — SSH Files, terminal, remote editing, zero-to-one Bootstrap, Runbook and closed-loop deployment. |
| 1267 | [qinshige/dsh-performance-guard](https://github.com/qinshige/dsh-performance-guard) | 0 | 2026-08-25 | 2026-08-31 | Host and Web performance diagnostics, repeated plugin-isolation campaigns, and safe recovery for DeepSeek Harness. |
| 1268 | [qipenglin/dsh-plugin-manager](https://github.com/qipenglin/dsh-plugin-manager) | 0 | 2026-08-28 | 2026-08-29 | Profile plugin manager for DeepSeek Harness |
| 1269 | [qipenglin/dsh-theme-spectrum](https://github.com/qipenglin/dsh-theme-spectrum) | 0 | 2026-08-28 | 2026-08-29 | Light and dark theme presets for DeepSeek Harness Web |
| 1270 | [qipenglin/dsh-web-access](https://github.com/qipenglin/dsh-web-access) | 0 | 2026-08-27 | 2026-08-27 | Optional Web access authentication plugin for DeepSeek Harness |
| 1271 | [qiqiangvae/dsh-obsidian](https://github.com/qiqiangvae/dsh-obsidian) | 0 | 2026-08-29 | 2026-09-01 | dsh obsidian wiki plugin |
| 1272 | [qt-11564/dsh-git-seam](https://github.com/qt-11564/dsh-git-seam) | 0 | 2026-08-29 | 2026-08-29 | Structured git tools for DeepSeek Harness: diff-before-commit gate + deterministic porcelain parsing (Chinese/UTF-8 paths, Windows) |
| 1273 | [QuanQQQ/dsh-plugin-dev-manager](https://github.com/QuanQQQ/dsh-plugin-dev-manager) | 0 | 2026-08-24 | 2026-08-27 | Stable control plane for isolated DeepSeek Harness plugin development |
| 1274 | [que3sui/dsh-darwin](https://github.com/que3sui/dsh-darwin) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness (dsh) 双插件自进化架构：dsh-sentinel 机械挖掘会话日志生成问题工单 + dsh-forge 分级合成/评测门/确定性回滚 \| Two-plugin self-evolution for DSH: hindsight mining, gated synthesis, deterministic rollback (verified in simulation lab) |
| 1275 | [QWE13-ART/dsh-claim-gate](https://github.com/QWE13-ART/dsh-claim-gate) | 0 | 2026-09-02 | 2026-09-02 | Turn-boundary claim gate for DSH agents: 声称「已完成/已落地」但本轮无验证输出时机械拦截；有验证输出时软提示对照验证覆盖 + 任务收尾派独立审计。纯同步正则 host hook（agent/turn-stopping），零 LLM、零网络。 |
| 1276 | [QWE13-ART/dsh-skill-folder](https://github.com/QWE13-ART/dsh-skill-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH skill catalog prompt surface: static KV-cache-stable catalog + BM25/bge-m3 hybrid skill_search + autoRoute hints. v0.3.0. npm: dsh-skill-folder |
| 1277 | [QWE13-ART/dsh-tool-folder](https://github.com/QWE13-ART/dsh-tool-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH tool surface per request + ChainGuard firewall (high-risk block + exfil-chain detection + anti-obfuscation) + BM25/bge-m3 hybrid tools_search. Shrinks schema tokens 80-90% while keeping selection accuracy. v0.2.0 adds a semantic retrieval leg (local Ollama bge-m3, RRF hybrid) and ChainGuard obfuscation detection. npm: dsh-tool-folder |
| 1278 | [qwerty-k-de/dsh-attach-picker](https://github.com/qwerty-k-de/dsh-attach-picker) | 0 | 2026-09-01 | 2026-09-01 | DSH Web composer toolbar picture button: pick images via the OS file dialog - no drag-and-drop needed. |
| 1279 | [RaberShef/dsh-pin-session](https://github.com/RaberShef/dsh-pin-session) | 0 | 2026-08-26 | 2026-08-27 | Pin DSH sessions to the top of the sidebar and mark them unread for later. |
| 1280 | [raktim-mondol/dsh-researchcraft](https://github.com/raktim-mondol/dsh-researchcraft) | 0 | 2026-08-28 | 2026-08-28 | ResearchCraft as a DeepSeek Harness (DSH) profile plugin: research persona, scientific skills catalogue, living lab notebook, and specialist subagents. |
| 1281 | [randomix777/dsh-plugin-subs](https://github.com/randomix777/dsh-plugin-subs) | 0 | 2026-08-28 | 2026-08-31 | DSH plugin: OAuth sign-in for Claude, Codex, Grok, Antigravity, OpenRouter, Agnes AI — expose subscription LLMs as DeepSeek Harness providers |
| 1282 | [randomix777/dsh-sprite-gen](https://github.com/randomix777/dsh-sprite-gen) | 0 | 2026-08-28 | 2026-08-31 | Sprite Sheet Generator with AI Image Generation for DeepSeek Harness |
| 1283 | [rangdl/dsh-all-enhance](https://github.com/rangdl/dsh-all-enhance) | 0 | 2026-08-28 | 2026-09-01 | DSH（DeepSeek Harness）功能增强插件 |
| 1284 | [Ranz-Feng/dsh-web-import](https://github.com/Ranz-Feng/dsh-web-import) | 0 | 2026-08-26 | 2026-08-27 | Import DeepSeek Web (chat.deepseek.com) chat history into DeepSeek Harness as resumable, workspace-grouped sessions with original titles preserved. |
| 1285 | [RaulLazaro/dsh-preview-plugin](https://github.com/RaulLazaro/dsh-preview-plugin) | 0 | 2026-08-31 | 2026-09-01 | Live preview tab for DeepSeek Harness — embed any dev server in an iframe with transparent SPA proxying |
| 1286 | [RaulLazaro/dsh-pwa-plugin](https://github.com/RaulLazaro/dsh-pwa-plugin) | 0 | 2026-08-31 | 2026-08-31 | PWA plugin for DeepSeek Harness — adds offline support and install-as-app capability |
| 1287 | [Raywh/dsh-song-download](https://github.com/Raywh/dsh-song-download) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 歌曲下载插件：搜索（B站/YouTube）+ 下载（MP3 320k 酷狗兼容）+ LRC 歌词（站点字幕 + 网易云兜底）。DSH plugin: song search & download with lyrics. |
| 1288 | [renat3u/dsh-upgrade-skill](https://github.com/renat3u/dsh-upgrade-skill) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件升级适配skill |
| 1289 | [Renjie-hub-byte/DSH-AutoKnit](https://github.com/Renjie-hub-byte/DSH-AutoKnit) | 0 | 2026-09-01 | 2026-09-01 | PRD in, maintainable code out. Cheap to build, cheaper to maintain — benchmark: −19% vs interactive agent, −41% vs heavy framework. 程序调度 0 token，写省改省不用盯。pip install autoknit |
| 1290 | [Reseezhang/ue-log-reader](https://github.com/Reseezhang/ue-log-reader) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：UE 日志速读卡 — 模型调用 uelog 工具扫描 Saved/Logs，流式解析+聚合去重后渲染速读卡片，一键复制缺陷单摘要 |
| 1291 | [Reseezhang/vizcb-codeblock-visualizer](https://github.com/Reseezhang/vizcb-codeblock-visualizer) | 0 | 2026-08-28 | 2026-08-29 | DeepSeek Harness 可视化插件：svg/html/mermaid 代码块渲染为图表卡片（宿主端 mermaid、深色主题配色、节点文字自适应、灯箱、保存导出） |
| 1292 | [RexYoung000/rex-harness](https://github.com/RexYoung000/rex-harness) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin authoring workspace. First plugin: UI design workflow (@rex-harness/ui-workflow). |
| 1293 | [rhczz/dshctl](https://github.com/rhczz/dshctl) | 0 | 2026-09-02 | 2026-09-02 | dshctl — DeepSeek Harness web 服务后台管理脚本(启停/日志/构建/一键更新) |
| 1294 | [Riianfar/dsh-zai-web-search-api](https://github.com/Riianfar/dsh-zai-web-search-api) | 0 | 2026-08-31 | 2026-09-02 | DeepSeek Harness (DSH) 的 Z.AI / 智谱独立 Web Search API provider |
| 1295 | [rm-Vstar/web-search-tinyfish](https://github.com/rm-Vstar/web-search-tinyfish) | 0 | 2026-08-28 | 2026-08-28 | A TinyFish web searching plugin for Deepseek Harness |
| 1296 | [robbin810130/dsh-vault-plugin](https://github.com/robbin810130/dsh-vault-plugin) | 0 | 2026-08-24 | 2026-08-27 | DSH 保险箱插件：项目与对话的前台隐私锁 |
| 1297 | [rrrrrredy/context-continuity](https://github.com/rrrrrredy/context-continuity) | 0 | 2026-08-28 | 2026-08-31 | Local-first continuity plugin for Codex and DeepSeek Harness across compaction, resume, and handoff. |
| 1298 | [rrrrrredy/dsh-execution-fidelity-guard](https://github.com/rrrrrredy/dsh-execution-fidelity-guard) | 0 | 2026-08-31 | 2026-08-31 | Unofficial alpha execution-fidelity guard bundle for DeepSeek Harness. |
| 1299 | [rrrrrredy/intent-loop](https://github.com/rrrrrredy/intent-loop) | 0 | 2026-08-31 | 2026-08-31 | Local-first, traceable current-intent state for Codex and DeepSeek Harness. |
| 1300 | [Rudyy898/dsh-drag-path](https://github.com/Rudyy898/dsh-drag-path) | 0 | 2026-08-27 | 2026-08-27 | dsh-plugin |
| 1301 | [ruiyukirin/dsh-douyin-oem-touliu-report](https://github.com/ruiyukirin/dsh-douyin-oem-touliu-report) | 0 | 2026-08-28 | 2026-08-28 | 抖音本地推 OEM 投流日报/周报自动化插件 - Douyin OEM ad daily/weekly report automation plugin for DeepSeek Harness (Author: Kirin) |
| 1302 | [runcat-tommy/dsh-plugin-runcat-inventory](https://github.com/runcat-tommy/dsh-plugin-runcat-inventory) | 0 | 2026-08-26 | 2026-08-28 | 逃咪-插件总览（Runcat Plugin Overview）—— 更好用的 DSH 插件列表：表格视图、状态过滤、启用/停用开关（热生效）、配置查看与复制、中英双语界面。 |
| 1303 | [runcat-tommy/dsh-theme-manager](https://github.com/runcat-tommy/dsh-theme-manager) | 0 | 2026-08-28 | 2026-08-28 | Two-level theme manager for DeepSeek Harness Web: pick a culture/scene or a national flag first, then a concrete style. 40 built-in styles (ink wash, ukiyo-e, Suzhou garden, cyberpunk, 20 flags & more). |
| 1304 | [runcat-tommy/dsh-view-manager](https://github.com/runcat-tommy/dsh-view-manager) | 0 | 2026-08-27 | 2026-08-28 | Manage DeepSeek Harness Web GUI view tabs (Chat/Trajectory): enable, hide, reorder & rename with zh/en locale. |
| 1305 | [RyanShen3/dsh-toutiao-reader](https://github.com/RyanShen3/dsh-toutiao-reader) | 0 | 2026-08-29 | 2026-08-29 | 读网页/头条文章全文的 DSH 插件：webfetch 工具 + toutiao-reader 经验技能 |
| 1306 | [Rycbartbad/dsh-key-manager](https://github.com/Rycbartbad/dsh-key-manager) | 0 | 2026-08-29 | 2026-08-29 | Multiple API keys per provider for DeepSeek Harness: pools with notes, one-click switching that really takes effect |
| 1307 | [Ryu6Zero/dsh-hindsight](https://github.com/Ryu6Zero/dsh-hindsight) | 0 | 2026-08-25 | 2026-08-27 | 🧠 Cross-session memory for DeepSeek Harness backed by Hindsight. Self-contained dsh-plugin: /hindsight commands + hindsight_recall/remember/status/list/forget agent tools. Lightweight, no dsh-mnemon, no orchestrator. |
| 1308 | [sANDzER0/dsh-hippocampus](https://github.com/sANDzER0/dsh-hippocampus) | 0 | 2026-08-26 | 2026-08-27 | Cross-session project memory for DeepSeek Harness — capture / consolidate / recall, keyword + optional local-Ollama semantic search. Inspired by magic-context. |
| 1309 | [saqie803/ponytail](https://github.com/saqie803/ponytail) | 0 | 2026-08-29 | 2026-08-29 | Ship production-ready code with one line of AI-generated output, built for 20 agents and zero ceremony. |
| 1310 | [sdoygb/geometry-knowledge](https://github.com/sdoygb/geometry-knowledge) | 0 | 2026-08-26 | 2026-08-27 | 几何论（共扼谱几何 CSG）知识库插件 for DeepSeek Harness: 纯离线 BM25 检索，零运行时依赖 |
| 1311 | [seiriosPlus/miaoda_for_deepseek_harness](https://github.com/seiriosPlus/miaoda_for_deepseek_harness) | 0 | 2026-08-26 | 2026-08-29 | miaoda_for_deepseek harness |
| 1312 | [seoeaa/dsh-locale-ru](https://github.com/seoeaa/dsh-locale-ru) | 0 | 2026-08-31 | 2026-08-31 | Русский интерфейс (локаль ru) для DeepSeek Harness — custom locale plugin. 26 namespaces, ~690 строк. / Russian locale plugin for DeepSeek Harness. |
| 1313 | [seth-hg/dsh-session-port](https://github.com/seth-hg/dsh-session-port) | 0 | 2026-09-02 | 2026-09-02 | dsh-session-port is a DeepSeek Harness plugin that bundles a session — its log, subagents, media, and referenced workspace files — into one portable ZIP and restores it on any DSH. |
| 1314 | [ShadowQuill/DialogueContextBridge](https://github.com/ShadowQuill/DialogueContextBridge) | 0 | 2026-08-26 | 2026-08-27 | 对话上下文桥接 — 为大语言模型(LLM)/AI 智能体的对话做跨会话上下文桥接的 DSH 插件：把一次对话的共识打包成可移植快照，一键引入新对话（三层快照 / SQLite+FTS5 / AES-256-GCM） |
| 1315 | [shaneconner/canon](https://github.com/shaneconner/canon) | 0 | 2026-08-10 | 2026-08-30 | Canonical project memory for the Pi coding agent: one governing article per asset, an append-only journal, capsule surfacing. A project wiki with a spine. |
| 1316 | [shaneconner/dsh-claude-bridge](https://github.com/shaneconner/dsh-claude-bridge) | 0 | 2026-08-30 | 2026-08-31 | Use a Claude Pro or Max subscription as a DeepSeek Harness model provider, via the Claude Code CLI. |
| 1317 | [shaneconner/dsh-provider-login](https://github.com/shaneconner/dsh-provider-login) | 0 | 2026-08-30 | 2026-08-31 | Sign in to DeepSeek Harness model providers with a Claude Pro/Max or ChatGPT Plus/Pro subscription. |
| 1318 | [ShanHaiFish/dsh-theme-brick](https://github.com/ShanHaiFish/dsh-theme-brick) | 0 | 2026-08-30 | 2026-08-30 | DSH 主题插件（Brick/砌砖）：纯 token 覆盖层，暖石膏与火烧黏土、灰缝线条、一砖一色，零全局 CSS；Settings → General 开关可随时关闭还原。A restrained token-only theme for DeepSeek Harness web — plaster & fired-clay, one accent, no global CSS, with an on/off switch. |
| 1319 | [shaomingbo/dsh-anyrouter](https://github.com/shaomingbo/dsh-anyrouter) | 0 | 2026-08-31 | 2026-08-31 | Dedicated provider bundle for the relay: Claude via Claude Code transport, GPT/Codex via Responses, for DeepSeek Harness |
| 1320 | [shaomingbo/dsh-open-in-editor](https://github.com/shaomingbo/dsh-open-in-editor) | 0 | 2026-08-26 | 2026-08-27 | Open DSH Web produced files in a configurable local macOS IDE |
| 1321 | [shaomingbo/dsh-subscription-antigravity](https://github.com/shaomingbo/dsh-subscription-antigravity) | 0 | 2026-08-29 | 2026-08-29 | Google Antigravity subscription reuse for DeepSeek Harness: browser PKCE sign-in, loopback OpenAI-compatible proxy to Cloud Code Assist, Gemini/Claude/GPT-OSS model routes. |
| 1322 | [shaomingbo/dsh-token-usage](https://github.com/shaomingbo/dsh-token-usage) | 0 | 2026-08-30 | 2026-08-30 | Accounts, subscription allowance observations, and local usage ledger for DeepSeek Harness |
| 1323 | [Shaw529/dsh-token-saver](https://github.com/Shaw529/dsh-token-saver) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin: aggressive token savings, no task-quality loss |
| 1324 | [shayexiangpaimeng/dsh-memory](https://github.com/shayexiangpaimeng/dsh-memory) | 0 | 2026-08-31 | 2026-08-31 | Append-only layered memory plugin for DeepSeek Harness: five-layer partitioning, write gate, keyword recall, claim-anchors verification |
| 1325 | [shengyvself/narrative-prompt-polish](https://github.com/shengyvself/narrative-prompt-polish) | 0 | 2026-08-28 | 2026-08-30 | DSH 插件：主输入框 ✨ 一键把草稿润色成清晰、可执行的提示词，经 better-sidebar 侧栏对话多轮打磨后回填。A DSH plugin: ✨ one-click draft polish into agent-ready prompts, multi-turn side-chat via better-sidebar (>=0.16.1). |
| 1326 | [shenhuanageshei/dsh-death-forensics](https://github.com/shenhuanageshei/dsh-death-forensics) | 0 | 2026-09-02 | 2026-09-02 | In-process death black box for DeepSeek Harness (dsh) hosts: heartbeat windows, crash stacks, end-kind self-check, death_forensics_report tool. |
| 1327 | [shenhuanageshei/dsh-git-status](https://github.com/shenhuanageshei/dsh-git-status) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：会话视图实时 git 状态展示 + 分支切换（会话头徽标 + 输入区环境行）。官方 bundle 插件，dsh plugin --profile web add：github:shenhuanageshei/dsh-git-status#v0.1.0 |
| 1328 | [shenhuanageshei/dsh-preset-zombie-guard](https://github.com/shenhuanageshei/dsh-preset-zombie-guard) | 0 | 2026-09-01 | 2026-09-01 | Preset-zombie guard plugin for DeepSeek Harness: auto-archive blank zombie sessions, warn on non-blank, pre-deletion dependency audit (preset_guard_check_remove). |
| 1329 | [shenhuanageshei/dsh-session-link-pro](https://github.com/shenhuanageshei/dsh-session-link-pro) | 0 | 2026-08-31 | 2026-08-31 | Session deep links + full session export (markdown/JSON) + approved cross-session messaging with pairing for DeepSeek Harness (dsh). |
| 1330 | [shenhuanageshei/dsh-thincoder-suite](https://github.com/shenhuanageshei/dsh-thincoder-suite) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin porting thincoder self-discipline suite: advisor convergent review / engineering mode / escalate / consult |
| 1331 | [ShenXuAkaEkstasis/dsh-ai-shopping-assistant](https://github.com/ShenXuAkaEkstasis/dsh-ai-shopping-assistant) | 0 | 2026-08-28 | 2026-08-28 | AI Shopping Assistant plugin for DeepSeek Harness (DSH), with product comparison, price analysis, merchant/review evidence and source-quality checks. |
| 1332 | [ShineFree7/dsh-doc-rail](https://github.com/ShineFree7/dsh-doc-rail) | 0 | 2026-09-02 | 2026-09-02 | Right-side document rail for the DeepSeek Harness web GUI — Markdown/plain-text viewer with light & deep-navy themes, drag-resize, recent files, auto-sync. （中文：dsh web 右侧文档面板，支持浅色/深蓝主题、拖宽、最近文件、自动同步） |
| 1333 | [Shonean/deepseek-harness-vscode-desktop](https://github.com/Shonean/deepseek-harness-vscode-desktop) | 0 | 2026-08-27 | 2026-08-27 | Enhanced VS Code extension + Desktop app for DeepSeek Harness (DSH): inline diff, @mentions, selection context, approval UI, plan mode, global shortcut. Claude Code-grade experience. Unofficial community project. |
| 1334 | [Short-Arm-Ape/dsh-intranet-browser](https://github.com/Short-Arm-Ape/dsh-intranet-browser) | 0 | 2026-08-31 | 2026-08-31 | Bypasses the SSRF protection of @yeesy369dsh-browser-playwright |
| 1335 | [SHUJILAI/dsh-model-auto-hot-switch](https://github.com/SHUJILAI/dsh-model-auto-hot-switch) | 0 | 2026-08-28 | 2026-08-28 | Automatic per-task model hot-switching for DeepSeek Harness (dsh): image-aware tasks route to the vision model automatically, every other task keeps your default model. Zero extra tokens, no context disturbance. |
| 1336 | [shxtmaker/dsh-usage-monitor](https://github.com/shxtmaker/dsh-usage-monitor) | 0 | 2026-08-26 | 2026-08-28 | DSH 用量监控插件：供应商周期限额显示（DeepSeek/OpenCode/Command Code）+ 自动探测 DSH 已添加供应商并自动填入 API Key |
| 1337 | [sidrandom/deepseek-memory-capsule](https://github.com/sidrandom/deepseek-memory-capsule) | 0 | 2026-09-01 | 2026-09-01 | A complete, human-centered memory layer for DeepSeek that stores user preferences, conversation notes, and personal variables across sessions — built as a DeepSeek Harness plugin. |
| 1338 | [sijie-ni-0214/dsh-subagent-error-details](https://github.com/sijie-ni-0214/dsh-subagent-error-details) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: deliver the real failure reason (e.g. RATE_LIMIT 429) to the parent agent when a background subagent fails |
| 1339 | [SiriusWJ/dsh-mihome](https://github.com/SiriusWJ/dsh-mihome) | 0 | 2026-08-30 | 2026-08-30 | Mi Home (米家) control for DeepSeek Harness agents — list homes/devices, read props, control devices behind a human approval gate. |
| 1340 | [SJCLZ/MixlabLz-dsh-skills](https://github.com/SJCLZ/MixlabLz-dsh-skills) | 0 | 2026-08-27 | 2026-08-27 | MixlabLz's collection of DSH (DeepSeek Harness) skills and plugins |
| 1341 | [SMOKTEA/dsh-chartlab](https://github.com/SMOKTEA/dsh-chartlab) | 0 | 2026-08-26 | 2026-08-28 | Let the agent turn your data into an interactive chart.  \|  一句话：让 Agent 帮你把数据变成一张可交互的图表。 |
| 1342 | [snow-The/dsh-research-lab](https://github.com/snow-The/dsh-research-lab) | 0 | 2026-08-31 | 2026-08-31 | Research lab toolkit for DeepSeek Harness: AutoSci wiki, ASI-Bench eval ledger, self-building FTS5 retrieval, arXiv digest/review, writing rewrite |
| 1343 | [soberbiak/amazon-sucareer](https://github.com/soberbiak/amazon-sucareer) | 0 | 2026-08-28 | 2026-08-30 | 基于真实证据，把亚马逊运营经历酥成招聘方看得懂、面试讲得透的职业定位、简历与求职表达。拒绝硬编 KPI，争取人生大结果。 |
| 1344 | [socai-io/dsh-socai](https://github.com/socai-io/dsh-socai) | 0 | 2026-09-01 | 2026-09-01 | DeepSeek Harness plugin for SocAI Xiaohongshu research tools |
| 1345 | [softspark/dsh-orchestrator](https://github.com/softspark/dsh-orchestrator) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness bundle for one-shot Claude Code and GitHub Copilot Gemini delegation through native subscription logins. |
| 1346 | [soulYANG/dsh-baogongtou](https://github.com/soulYANG/dsh-baogongtou) | 0 | 2026-08-26 | 2026-08-27 | 包工头：DeepSeek Harness 工作 agent 皮肤。能力还是 dsh，嘴和按钮是包工头。 |
| 1347 | [STARDUSTLC666/dsh-dream](https://github.com/STARDUSTLC666/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH 做梦插件：会话回放（梦原料）→ 反思 → 梦境日记（记忆巩固）→ 高频教训幂等桥接 AGENTS.md。多帧 zstd 会话读取、默认隐私脱敏、零运行时依赖。Dream plugin for DeepSeek Harness: session replay, reflection, dream journal, memory bridge. |
| 1348 | [STARDUSTLC666/dsh-suite](https://github.com/STARDUSTLC666/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | STARDUSTLC 插件全家桶：一条命令装入 18 个 DSH 插件（办公流/媒体工坊/DevOps/做梦）。The STARDUSTLC plugin suite: 18 DSH plugins, one command. |
| 1349 | [statem-li/dsh-done-pill](https://github.com/statem-li/dsh-done-pill) | 0 | 2026-08-30 | 2026-09-01 | DSH 对话完成胶囊：顶部悬浮消息胶囊（原 webui done-pill 拆出）——任一会话回合完成提醒、点击跳会话、悬停查看记录全文、可拖拽定位、健康提醒与字体/缩放设置。零 DSH 源码改动，可与 dsh-webui 并存（webui 关闭 donePill 模块即可）。 |
| 1350 | [statem-li/dsh-think-tools](https://github.com/statem-li/dsh-think-tools) | 0 | 2026-08-31 | 2026-09-01 | DSH 思考与工具调用聚合：回合级思考 chip（实时时长/实时文字滚动）+ 工具调用聚合 chip + 共享活动抽屉 + 对话流卡片（步骤卡/总结卡，回合结束后才出现）——自 dsh-webui 移植。零 DSH 源码改动。 |
| 1351 | [statem-li/dsh-web-search-anysearch](https://github.com/statem-li/dsh-web-search-anysearch) | 0 | 2026-08-31 | 2026-09-01 | DSH 外接网页搜索（AnySearch）：注册 AnySearch 网页搜索 provider（替换内置 DeepSeek 搜索）+ 插件设置卡（API Key / Base URL / 默认结果数）。提炼自 statem-li/dsh-webui 的 webSearch 模块，零 DSH 源码改动。 |
| 1352 | [stayhpjinng/dsh-provider-proxy](https://github.com/stayhpjinng/dsh-provider-proxy) | 0 | 2026-08-29 | 2026-08-29 | Provider-scoped HTTP/HTTPS forward proxy plugin for DeepSeek Harness |
| 1353 | [StephenEvenson/dsh-plugin-elevenlabs-callback](https://github.com/StephenEvenson/dsh-plugin-elevenlabs-callback) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness plugin: when a run finishes or needs approval, get a link on your phone, hear the result from an ElevenLabs voice agent and say what to do next |
| 1354 | [steven-ngle/dsh-elden](https://github.com/steven-ngle/dsh-elden) | 0 | 2026-08-30 | 2026-08-30 | Elden Ring style event overlays for the DeepSeek Harness web UI |
| 1355 | [Stijnus/dsh-ds-kanban](https://github.com/Stijnus/dsh-ds-kanban) | 0 | 2026-09-02 | 2026-09-02 | Live task-board plugin for DeepSeek Harness Web: sidebar badge, full-shell kanban with search, filters, export, and diagnostics. |
| 1356 | [Stijnus/dsh-ds-ponytail](https://github.com/Stijnus/dsh-ds-ponytail) | 0 | 2026-09-02 | 2026-09-02 | Lazy senior dev mode for DeepSeek Harness: ponytail skill family (ponytail, review, audit, debt, gain, help) adapted from DietrichGebert/ponytail (MIT). Install: dsh plugin --profile web add dsh-ds-ponytail |
| 1357 | [StudyforDS/Deepseek_dsh-plugin](https://github.com/StudyforDS/Deepseek_dsh-plugin) | 0 | 2026-08-30 | 2026-08-31 | dsh-plugin |
| 1358 | [substitute525/dsh-tool-monitor](https://github.com/substitute525/dsh-tool-monitor) | 0 | 2026-08-28 | 2026-08-28 | 一个 dsh-plugin：后台监听文件或命令输出，输出到达时唤醒所属会话，并在 Web 会话头部提供实时监听的列表与输出查看面板。MIT License。 |
| 1359 | [SuCriss/dsh-voice-control](https://github.com/SuCriss/dsh-voice-control) | 0 | 2026-08-31 | 2026-08-31 | Voice control for DeepSeek Harness web: speech-to-text into the composer and spoken playback of assistant replies, zero dependencies |
| 1360 | [Suguyun/dsh-bili-miniplay](https://github.com/Suguyun/dsh-bili-miniplay) | 0 | 2026-08-28 | 2026-08-28 | 跨平台 fork of dsh-bili-widget：DSH B站悬浮看片小窗（Node 原生 fetch，macOS/Linux/Windows 通用） |
| 1361 | [sunyuhuirong/fsviewer](https://github.com/sunyuhuirong/fsviewer) | 0 | 2026-08-29 | 2026-08-30 | Codex-style right-edge workspace for DeepSeek dsh web: file tree + preview, embedded browser, and side chat |
| 1362 | [superkonka/dsh-poor-mode](https://github.com/superkonka/dsh-poor-mode) | 0 | 2026-08-27 | 2026-08-27 | 穷鬼模式 Poor Mode — 供应商感知的分时省钱 DSH agent preset：复杂任务可选「立即执行」或「闲时执行」（DeepSeek 峰谷半价；其他平台可自定义规则） |
| 1363 | [SuperstructureJH/dsh-workbuddy-ppt](https://github.com/SuperstructureJH/dsh-workbuddy-ppt) | 0 | 2026-08-26 | 2026-08-27 | Editable PPTX generation for DSH with bundled authoring skills and deterministic PPTD validation |
| 1364 | [suyukun/dsh-plugin-publish](https://github.com/suyukun/dsh-plugin-publish) | 0 | 2026-08-26 | 2026-08-27 | Ship your skills, grow your influence — a model-agnostic publishing protocol for AI agent skills: preflight checks, GitHub repo, index PRs, marketplace submissions, promo copy. 把 agent 技能标准化发布到 GitHub 的流程协议。 |
| 1365 | [suyukun/dsh-tech-selection](https://github.com/suyukun/dsh-tech-selection) | 0 | 2026-08-26 | 2026-08-27 | Stop letting your AI guess — a research protocol for tech decisions that any AI agent (DSH/Claude/Cursor/Codex) can follow: quantified requirements, T1-T6 source tiers, quality gates, traceable verdicts. 模型无关的技术选型调研协议。 |
| 1366 | [svgop/dsh-generative-ideas](https://github.com/svgop/dsh-generative-ideas) | 0 | 2026-08-26 | 2026-08-29 | Roadmap ideation for DeepSeek Harness — generate and compare distinct roadmap options via headless agent runs, pick one, export as goal.md |
| 1367 | [svgop/dsh-rich-context](https://github.com/svgop/dsh-rich-context) | 0 | 2026-08-26 | 2026-08-29 | Agent instruction manager for DSH — edit and template the AGENTS.md files the harness actually reads (global + per-workspace) |
| 1368 | [svgop/dsh-rich-tracking](https://github.com/svgop/dsh-rich-tracking) | 0 | 2026-08-26 | 2026-08-29 | Percent-progress scoreboard for DeepSeek Harness — evidence-bound rows, git-captured checkpoints, pursue/align/dismiss operator whip |
| 1369 | [swxs/archive-restore](https://github.com/swxs/archive-restore) | 0 | 2026-09-02 | 2026-09-02 | DSH 归档会话管理插件，支持查看归档列表、原位恢复与跨区迁移，Web 侧边栏一键管理 |
| 1370 | [syfun/dsh-dogpet](https://github.com/syfun/dsh-dogpet) | 0 | 2026-08-27 | 2026-08-27 | 🐕 中华田园犬桌面宠物 - DSH Desktop Pet |
| 1371 | [syncended/deepseek-harness-messenger](https://github.com/syncended/deepseek-harness-messenger) | 0 | 2026-08-25 | 2026-08-29 | Messenger bridge plugin for DeepSeek Harness, starting with Telegram |
| 1372 | [syncended/deepseek-harness-usage](https://github.com/syncended/deepseek-harness-usage) | 0 | 2026-08-26 | 2026-08-27 | Token usage, model cost analytics, trends, and activity heatmaps for DeepSeek Harness |
| 1373 | [szymonsheng2045/dsh-carbonclub](https://github.com/szymonsheng2045/dsh-carbonclub) | 0 | 2026-08-28 | 2026-08-28 | A zero-model-cost human waiting room for DeepSeek Harness |
| 1374 | [Tangweiwei227/dsh-asc](https://github.com/Tangweiwei227/dsh-asc) | 0 | 2026-08-29 | 2026-08-29 | App Store Connect CLI (asc) as a native tool for DeepSeek Harness — structured argv, JSON output, no-shell execution. |
| 1375 | [taod8205-spec/model-switcher-dsh](https://github.com/taod8205-spec/model-switcher-dsh) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 模型与推理强度一键切换插件，支持胶囊滑杆、档位吸附和极高态视觉。 |
| 1376 | [TARS-snail/dsh-guard-sensitive-paths](https://github.com/TARS-snail/dsh-guard-sensitive-paths) | 0 | 2026-09-02 | 2026-09-02 | Approval guard for DeepSeek Harness: write/edit/editor/bash calls touching sensitive paths (.env, .git, SSH keys, .pem) become an approval ask. |
| 1377 | [Tazio7/dsh-web-search-glm](https://github.com/Tazio7/dsh-web-search-glm) | 0 | 2026-09-01 | 2026-09-01 | Web search plugin for DeepSeek Harness powered by ZAI GLM MCP — auto-injects API key from ~/.dsh/.credentials.yaml or environment variables |
| 1378 | [thuCGRA/dsh-quick-invoke](https://github.com/thuCGRA/dsh-quick-invoke) | 0 | 2026-09-02 | 2026-09-02 | `dsh-quick-invoke` 是一个面向 DSH Web 的独立 Cordis 插件，为 Skill、Agent preset 和 Plugin 提供统一的 `/` 快捷入口、候选选择和 Host 命令执行能力。  本插件不修改 DSH 核心，不提供任意 Tool 直调语法。Tool 仍由 Agent 根据自然语言选择，并继续经过 DSH 的 tools、approval、guard 和 permission 流程。 |
| 1379 | [tianhanly/dsh-genshin-redirect](https://github.com/tianhanly/dsh-genshin-redirect) | 0 | 2026-08-30 | 2026-08-31 | 完成任务自动跳转到原神 Automatically jump to Genshin Impact after completing the task |
| 1380 | [tianhanly/dsh-official-port-nav](https://github.com/tianhanly/dsh-official-port-nav) | 0 | 2026-08-29 | 2026-08-30 | Perfectly replicate DeepSeek's official right-side chat navigation in Harness |
| 1381 | [tianhanly/dsh-verification-meme](https://github.com/tianhanly/dsh-verification-meme) | 0 | 2026-08-30 | 2026-08-31 | Every time you press a key, a security verification pops up. 每按一个harness的按键都会跳出一个安全验证 |
| 1382 | [tianhanly/dsh-warm-reminder](https://github.com/tianhanly/dsh-warm-reminder) | 0 | 2026-08-29 | 2026-08-29 | 智能温馨提醒插件，检测使用时长自动提示喝水、护眼、休息，支持深夜关怀与节假日祝福。基于DSH/Cordis框架开发。 |
| 1383 | [tianjiqx/dsh-agentobs](https://github.com/tianjiqx/dsh-agentobs) | 0 | 2026-09-01 | 2026-09-01 | dsh 可观测解决方案 |
| 1384 | [tianyuegithub/dsh-pactflow](https://github.com/tianyuegithub/dsh-pactflow) | 0 | 2026-08-30 | 2026-08-30 | DSH PactFlow（零脉模式）外部 Profile Bundle |
| 1385 | [TnzGit/dsh-live-perf-gauges](https://github.com/TnzGit/dsh-live-perf-gauges) | 0 | 2026-08-27 | 2026-08-27 | Real-time Decode tok/s, TTFT and Prefill throughput dashboard for DeepSeek Harness. |
| 1386 | [Traveritas/petween](https://github.com/Traveritas/petween) | 0 | 2026-08-21 | 2026-08-29 | Agent pet plugin for DeepSeek Harness (dsh): a few pose images in, expressive comic-style motion out — WAAPI timeline engine, custom animation editor, pose presets, and extension services for companion plugins |
| 1387 | [Traveritas/petween-physics](https://github.com/Traveritas/petween-physics) | 0 | 2026-08-25 | 2026-08-29 | Throw-physics companion plugin for Petween (drag-fling, wall bounce, ground slide), consuming the petween extension services |
| 1388 | [trueRISCOacnt/maa-dsh-skill](https://github.com/trueRISCOacnt/maa-dsh-skill) | 0 | 2026-08-28 | 2026-08-30 | 基于 MaaAssistantArknights (MAA) 官方命令行工具 maa-cli 构建的 DeepSeek Harness Skill：让 DeepSeek Harness 直接驱动 MaaCore，自动化完成《明日方舟》日常任务。 |
| 1389 | [tumi-huakai/dsh-plugin-meow-speech](https://github.com/tumi-huakai/dsh-plugin-meow-speech) | 0 | 2026-08-28 | 2026-08-28 | 喵语定制：DSH 消息正文显示层文本替换插件（仅界面显示，不改动真实对话内容） |
| 1390 | [TussalZeus18028/dsh-conflict-checker](https://github.com/TussalZeus18028/dsh-conflict-checker) | 0 | 2026-08-26 | 2026-08-27 | Detect DeepSeek Harness plugin conflicts and internal issues; manage plugins (enable/disable/uninstall) from a settings page. |
| 1391 | [tuzkier/valley-liang](https://github.com/tuzkier/valley-liang) | 0 | 2026-08-28 | 2026-08-28 | 梁文谷：替换 DeepSeek Harness Web 品牌标识，并按北京时间高峰时段切换图片。 |
| 1392 | [Tyon-nos-Ty90/dsh-mcsm-panel](https://github.com/Tyon-nos-Ty90/dsh-mcsm-panel) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness Desktop plugin that lets your AI control MCSManager (MCSM 10.x) Minecraft servers from the chat: server console, file management, instance start/restart/stop/kill, and direct file uploads. |
| 1393 | [UnforgetMemory/um-dsh-websearch](https://github.com/UnforgetMemory/um-dsh-websearch) | 0 | 2026-08-27 | 2026-08-27 | Exa (exa.ai) web search provider plugin for DeepSeek Harness (DSH): dynamic enabled switch, credentials-service key resolution, bilingual settings card. |
| 1394 | [UnKnownFish125/dsh-literature](https://github.com/UnKnownFish125/dsh-literature) | 0 | 2026-09-01 | 2026-09-01 | DSH literature/knowledge plugin: 文献→证据→知识管理（独立 literatum server + Web UI + agent 工具） |
| 1395 | [UnKnownFish125/dsh-livetaskboard](https://github.com/UnKnownFish125/dsh-livetaskboard) | 0 | 2026-08-26 | 2026-08-27 | 派生动态任务看板插件：独立任务状态机、存储、看板 UI、外援（sol + 保底子代理）；从 dsh-deepmemory 派生。 |
| 1396 | [upJiang/dsh-cron-job](https://github.com/upJiang/dsh-cron-job) | 0 | 2026-08-27 | 2026-08-31 | dsh 插件，定时任务+多渠道推送 |
| 1397 | [uppercrusteve/dsh-plugin-split-and-solve](https://github.com/uppercrusteve/dsh-plugin-split-and-solve) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: split batch / multi-subproblem research tasks into small questions and solve them with sub-agents |
| 1398 | [useful-money/Deepseek-Harness-branch-map-plugin](https://github.com/useful-money/Deepseek-Harness-branch-map-plugin) | 0 | 2026-08-31 | 2026-08-31 | dsh-plugin; branch map show; branch map mange |
| 1399 | [VanadisGithub/dsh-skill-evolution](https://github.com/VanadisGithub/dsh-skill-evolution) | 0 | 2026-09-01 | 2026-09-01 | Hermes-style skill self-evolution plugin for DeepSeek Harness (DSH): crystallizes reusable agent skills from successful turns via signal-triggered LLM review, progressively improves them, and manages everything in a Settings panel. |
| 1400 | [vb2250158/dsh-plugins](https://github.com/vb2250158/dsh-plugins) | 0 | 2026-08-27 | 2026-08-27 | Open-source DeepSeek Harness plugin bundle with portable multi-computer synchronization |
| 1401 | [Viktirr/dsh-llm-lmstudio](https://github.com/Viktirr/dsh-llm-lmstudio) | 0 | 2026-08-28 | 2026-08-29 | LM Studio (OpenAI-compatible local server) adapter plugin for DeepSeek Harness |
| 1402 | [VinciBeans/dsh-smooth-plugin](https://github.com/VinciBeans/dsh-smooth-plugin) | 0 | 2026-08-24 | 2026-08-31 | 让 DSH 的会话滚底从"官方瞬时跳变"变成流畅顺滑的跟随滚动：会话装载与"回到最新"保持瞬时，而流式内容增长期间，消息列以恒定速度平滑跟随，起步轻柔、收尾绵软。 |
| 1403 | [Viviana-Luna/dsh-window](https://github.com/Viviana-Luna/dsh-window) | 0 | 2026-08-24 | 2026-08-28 | macOS 薄桌面客户端，为本机 DSH 提供 Liquid Glass UI。 |
| 1404 | [Vuitier/dsh-sound-notify](https://github.com/Vuitier/dsh-sound-notify) | 0 | 2026-08-31 | 2026-08-31 | DSH web plugin: chime on turn complete & intervention needed。DSH任务完成提示音插件 |
| 1405 | [Waldsatte/dsh-theme-taojian](https://github.com/Waldsatte/dsh-theme-taojian) | 0 | 2026-09-01 | 2026-09-01 | Taojian (陶笺) — Claude-inspired DSH theme |
| 1406 | [wangsan71/dsh-locale-zh-tw](https://github.com/wangsan71/dsh-locale-zh-tw) | 0 | 2026-09-01 | 2026-09-01 | DSH Web 介面繁體中文（台灣）語言包：npm install 即可加入 zh-TW 語系，全介面自動簡轉繁，繁中瀏覽器自動切換 |
| 1407 | [WangZetian-IVERSON/dsh-local-path-attachments](https://github.com/WangZetian-IVERSON/dsh-local-path-attachments) | 0 | 2026-09-01 | 2026-09-01 | Drag local files into deepseek Hermes as absolute-path attachment cards without copying them into the workspace |
| 1408 | [wantosure/dsh-plugin-browser-memory](https://github.com/wantosure/dsh-plugin-browser-memory) | 0 | 2026-08-26 | 2026-08-27 | Local-first DeepSeek Harness plugin for searching Chrome, Edge, and Brave bookmarks, history, and downloads. |
| 1409 | [WayJ/dsh-work](https://github.com/WayJ/dsh-work) | 0 | 2026-09-02 | 2026-09-02 | 基于dsh构建的个人工作Agent |
| 1410 | [WaySeeSee/dsh-de-workbench](https://github.com/WaySeeSee/dsh-de-workbench) | 0 | 2026-09-02 | 2026-09-02 | 轻量数据分析工作台（DSH 插件） |
| 1411 | [wbycloud/dsh-composer-tokens](https://github.com/wbycloud/dsh-composer-tokens) | 0 | 2026-08-31 | 2026-08-31 | DSH web GUI composer real-time token counter plugin (client-side, v1) |
| 1412 | [weekitmo/dsh-trace](https://github.com/weekitmo/dsh-trace) | 0 | 2026-08-31 | 2026-08-31 | A DeepSeek Harness Web plugin for inspecting redacted LLM HTTP request and response traces. |
| 1413 | [weibaohui/dsh-continue](https://github.com/weibaohui/dsh-continue) | 0 | 2026-08-31 | 2026-08-31 | 自动续跑插件 for DeepSeek Harness — 有序规则表：按失败类型路由 继续续跑 / 换模型 / 压缩后继续 / 停止 |
| 1414 | [weibaohui/dsh-settings-ui](https://github.com/weibaohui/dsh-settings-ui) | 0 | 2026-09-01 | 2026-09-01 | dsh 插件 · 设置界面自定义：调整原生设置窗口大小（全屏/预置/自定义）、背景不透明度与背景（亮暗各一色，实时跟随主题） |
| 1415 | [weibaohui/dsh-sync](https://github.com/weibaohui/dsh-sync) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：会话同步与冲突解决（apiproxy、token 内联） |
| 1416 | [weibaohui/dsh-tasks](https://github.com/weibaohui/dsh-tasks) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：cron 定时事项——定时/立即执行新建 agent 会话提交提示词，全屏管理界面 |
| 1417 | [weibaohui/experts-management](https://github.com/weibaohui/experts-management) | 0 | 2026-09-01 | 2026-09-01 | dsh 插件 · 专家市场：ntd 格式专家/专家团队管理与注入（＋专家按钮 / /expert-名称 手势），稀疏检出专家市场 |
| 1418 | [weibaohui/hermes-loop](https://github.com/weibaohui/hermes-loop) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：Hermes 循环——review/curator 自动化与会话循环管理 |
| 1419 | [weibaohui/skills-management](https://github.com/weibaohui/skills-management) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：技能市场——安装/删除/详情 API + 管理界面 |
| 1420 | [welltop-jim-wang/nomicore](https://github.com/welltop-jim-wang/nomicore) | 0 | 2026-08-18 | 2026-09-02 | A self-describing, governed data core for AI agents—schemas, authority, validation, and semantic context travel with the data. |
| 1421 | [wenbuer/dsh-readme-writer](https://github.com/wenbuer/dsh-readme-writer) | 0 | 2026-09-02 | 2026-09-02 | 一个给 DeepSeek Harness（dsh）用的 Agent Skill，负责写 / 优化 GitHub 项目 README.md。 |
| 1422 | [wenyixiaoqingnian/ds-mobile-skin](https://github.com/wenyixiaoqingnian/ds-mobile-skin) | 0 | 2026-08-30 | 2026-08-30 | Mobile DeepSeek-app look for DSH Web GUI + dsh-token-viewer billing patch |
| 1423 | [wf-ping/dsh-message-injector](https://github.com/wf-ping/dsh-message-injector) | 0 | 2026-08-30 | 2026-08-30 | dsh（DeepSeek Harness）插件：预设消息注入内容组合，每条消息自动注入 —— auto-inject preset content into every message |
| 1424 | [whklwhkl/dsh-playwright](https://github.com/whklwhkl/dsh-playwright) | 0 | 2026-09-02 | 2026-09-02 | A plugin for the DeepSeek Harness, enabling browser-use via playwright |
| 1425 | [Wickaninnish/dsh-skill-manager](https://github.com/Wickaninnish/dsh-skill-manager) | 0 | 2026-08-22 | 2026-08-27 | DeepSeek Harness 技能运维插件：自动发现、审计、去重和优化技能，构建安全可控的维护闭环。 |
| 1426 | [Wilson-Lai-Ab/dsh-idea-style](https://github.com/Wilson-Lai-Ab/dsh-idea-style) | 0 | 2026-08-21 | 2026-08-27 | DSH plugin |
| 1427 | [windrover/dsh-long-term-memory](https://github.com/windrover/dsh-long-term-memory) | 0 | 2026-08-25 | 2026-08-27 | Layered deterministic long-term memory for DeepSeek Harness: CJK-aware BM25 recall, JSONL storage, per-assembly context injection, write guards and threat scanning. |
| 1428 | [winghv/dsh-acp-activity](https://github.com/winghv/dsh-acp-activity) | 0 | 2026-08-30 | 2026-08-30 | Community ACP automation server for DeepSeek Harness with committed tool-activity frames (tool_call/tool_call_update) — dsh-plugin |
| 1429 | [wingillis/dsh-plugins](https://github.com/wingillis/dsh-plugins) | 0 | 2026-08-30 | 2026-09-01 | Personal deepseek harness plugins like vim keybindings and more |
| 1430 | [WinnieJQ/dsh-conversation-cost](https://github.com/WinnieJQ/dsh-conversation-cost) | 0 | 2026-08-28 | 2026-08-28 | Per-conversation DeepSeek API cost badge for DeepSeek Harness (dsh): zero-dependency sessionCost projection with peak/off-peak pricing and a live hover-card badge in the web conversation header. |
| 1431 | [Wisdoverse/dsh-inline-media-viewer-plugin](https://github.com/Wisdoverse/dsh-inline-media-viewer-plugin) | 0 | 2026-08-26 | 2026-08-28 | Inline image, video, and audio previews for DeepSeek Harness Web, with workspace-safe local files, direct web media, and an optional ComfyUI proxy. |
| 1432 | [Wisdoverse/dsh-skills-manager-plugin](https://github.com/Wisdoverse/dsh-skills-manager-plugin) | 0 | 2026-08-28 | 2026-08-28 | Skill manager for DeepSeek Harness: proactive skill activation with trigger hooks, GitHub source sync, and a Settings management UI. |
| 1433 | [wisp-science/dsh-wisp-science-lab](https://github.com/wisp-science/dsh-wisp-science-lab) | 0 | 2026-08-19 | 2026-09-02 | DSH plugin: laboratory PI for local Wisp Science. Read-only snapshots, evidence-backed advice. / 实验室 PI：只读查看本机 Wisp Science 课题进展，按快照给意见。 |
| 1434 | [Witchwarren2344/dsh-mnemosyne-memory](https://github.com/Witchwarren2344/dsh-mnemosyne-memory) | 0 | 2026-08-29 | 2026-08-29 | Provide long-term memory, vector semantic search, and LLM reflection for DeepSeek Harness (DSH) with this free, MIT-licensed plugin. |
| 1435 | [wjj-8283/dsh-temp-workspace](https://github.com/wjj-8283/dsh-temp-workspace) | 0 | 2026-09-02 | 2026-09-02 | 为DeepSeek Harness增加临时工作区功能！ |
| 1436 | [wjling/dsh-vision-assist](https://github.com/wjling/dsh-vision-assist) | 0 | 2026-09-02 | 2026-09-02 | dsh视觉助手，辅助没有多模态的主模型识别图片内容 |
| 1437 | [WJNCT55555/dsh-crt-theme](https://github.com/WJNCT55555/dsh-crt-theme) | 0 | 2026-08-26 | 2026-08-27 | Dual-palette CRT terminal theme for DeepSeek Harness Web |
| 1438 | [Wlain/deepseek-plugin](https://github.com/Wlain/deepseek-plugin) | 0 | 2026-08-26 | 2026-08-31 | Kling AI remote MCP plugin for DeepSeek Harness |
| 1439 | [WMXS-A/dsh-utility-plugins](https://github.com/WMXS-A/dsh-utility-plugins) | 0 | 2026-09-02 | 2026-09-02 | Utility plugins for DeepSeek Harness: skill cheatsheet panel and session boot healthcheck |
| 1440 | [wodongx123/dsh-language-control](https://github.com/wodongx123/dsh-language-control) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: force agent chain-of-thought to stay in Chinese — 让 Agent 的思考过程也自动使用中文 |
| 1441 | [WolffyCode/deepseek-harness-plugin](https://github.com/WolffyCode/deepseek-harness-plugin) | 0 | 2026-08-25 | 2026-08-29 | Multi-engine Claude CLI and Codex CLI integration for DeepSeek Harness |
| 1442 | [WooLeo1995/dsh-llm-ai](https://github.com/WooLeo1995/dsh-llm-ai) | 0 | 2026-08-27 | 2026-08-27 | 替换 llm-pi-ai 模型配置，主要处理 dsh-llm-pi-ai 厂商和模型更新不及时的问题 |
| 1443 | [wr-web/dsh-context-tree](https://github.com/wr-web/dsh-context-tree) | 0 | 2026-08-26 | 2026-08-27 | Reusable trajectory-tree context, exact-turn forks, and bounded cross-session recall for DeepSeek Harness |
| 1444 | [wrw-dev/dsh-spring-widget](https://github.com/wrw-dev/dsh-spring-widget) | 0 | 2026-08-27 | 2026-09-01 | DSH 插件：Spring Boot 后端服务管理器（顶栏 IDEA 式启动/停止/日志控制台，源码直启 + Jar 打包启动） |
| 1445 | [WSL043/dsh-dictation](https://github.com/WSL043/dsh-dictation) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 语音输入：本地多语言识别与 Codex Desktop 听写，只写入可编辑草稿。 |
| 1446 | [WSL043/dsh-image-viewer](https://github.com/WSL043/dsh-image-viewer) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 可选图片查看器：缩放、原图下载、图库与区域标注，可独立卸载。 |
| 1447 | [WuJiaoJue/dsh-herdr-site](https://github.com/WuJiaoJue/dsh-herdr-site) | 0 | 2026-09-01 | 2026-09-01 | Reports dsh/cc-tui agent state (working/idle/blocked) to Herdr over the custom-integration protocol. |
| 1448 | [WuJiaoJue/dsh-suggest-ghost](https://github.com/WuJiaoJue/dsh-suggest-ghost) | 0 | 2026-09-01 | 2026-09-01 | DSH Web 输入预测插件：回合结束后 LLM 生成下一条建议，输入框空草稿时渲染幽灵文本，Tab 采纳。 |
| 1449 | [wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback](https://github.com/wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback) | 0 | 2026-08-25 | 2026-08-27 | DSH plugin that converts read_image PNG/WebP attachments to JPEG for LM Studio compatibility. |
| 1450 | [wxjgit/permission-popup](https://github.com/wxjgit/permission-popup) | 0 | 2026-08-27 | 2026-08-27 | 当前会话或后台会话正在等待权限审批时，插件会在页面角落显示审批卡片，让你无需切回原会话就能选择“允许一次”或“拒绝”。 |
| 1451 | [wyb587285-dot/git-ai-tracker](https://github.com/wyb587285-dot/git-ai-tracker) | 0 | 2026-08-31 | 2026-08-31 | GitHub AI repo tracker: star ratings, growth leaderboard, Markdown reports and web dashboard. |
| 1452 | [wyhgoodjob/dsh-checkpoint](https://github.com/wyhgoodjob/dsh-checkpoint) | 0 | 2026-09-01 | 2026-09-01 | Git-snapshot checkpoint/rollback capability for DeepSeek Harness: revert files and conversation to a previous completed turn. |
| 1453 | [wyhgoodjob/dsh-sisyphus](https://github.com/wyhgoodjob/dsh-sisyphus) | 0 | 2026-09-01 | 2026-09-01 | Sisyphus orchestration agent preset for DeepSeek Harness: intent gate, decompose-and-delegate to specialist subagents, parallel execution, evidence loop. |
| 1454 | [xain/ui-beep](https://github.com/xain/ui-beep) | 0 | 2026-08-26 | 2026-08-27 | **dsh-beep** — an agent-heartbeat sonification plugin for the DeepSeek Harness Web surface. |
| 1455 | [xarleyn/dsh-doc-impact](https://github.com/xarleyn/dsh-doc-impact) | 0 | 2026-08-28 | 2026-08-28 | Documentation impact enforcement for DeepSeek Harness — keep docs in sync by linking code changes to affected documentation. |
| 1456 | [xarleyn/dsh-session-scope](https://github.com/xarleyn/dsh-session-scope) | 0 | 2026-08-28 | 2026-08-28 | Per-session workspace scoping for DeepSeek Harness — expose only selected directories to agents with focused and isolated enforcement. |
| 1457 | [xarleyn/dsh-sleev](https://github.com/xarleyn/dsh-sleev) | 0 | 2026-08-26 | 2026-08-27 | Sleev integration for DeepSeek Harness with route-aware LLM telemetry and context-optimization observability |
| 1458 | [xby-skill/xby-12306-ticket-purchase-search](https://github.com/xby-skill/xby-12306-ticket-purchase-search) | 0 | 2026-08-28 | 2026-09-02 | 基于 Model Context Protocol (MCP) 的12306购票搜索服务器。提供了简单的API接口，允许大模型利用接口搜索12306购票信息。 |
| 1459 | [xby-skill/xby-advertising-analysis](https://github.com/xby-skill/xby-advertising-analysis) | 0 | 2026-08-28 | 2026-09-02 | 一个用于在LLM响应中注入广告的MCP服务器演示项目，展示广告注入中间件的风险。 |
| 1460 | [xby-skill/xby-ai-persona](https://github.com/xby-skill/xby-ai-persona) | 0 | 2026-08-28 | 2026-09-02 | 一个支持多AI人格召唤与协作的MCP协议服务器，可用于代码分析、产品设计等多场景智能协作。 |
| 1461 | [xby-skill/xby-airbnb-search](https://github.com/xby-skill/xby-airbnb-search) | 0 | 2026-08-28 | 2026-09-02 | 一个提供高级筛选功能和详细房源信息的Airbnb搜索桌面扩展，适用于旅行规划和房源研究。 |
| 1462 | [xby-skill/xby-akshare](https://github.com/xby-skill/xby-akshare) | 0 | 2026-08-28 | 2026-09-02 | AKShare MCP Server 是一个通过AKShare提供中国股票市场数据的模型上下文协议服务器，支持实时行情、历史数据、基本面分析等功能。 |
| 1463 | [xby-skill/xby-akshare-one](https://github.com/xby-skill/xby-akshare-one) | 0 | 2026-08-28 | 2026-09-02 | 基于akshare-one的MCP服务器，提供中国股票市场数据的全面接口，包括历史数据、实时数据、新闻数据和财务报表等金融信息。 |
| 1464 | [xby-skill/xby-ancient-poetry-kg](https://github.com/xby-skill/xby-ancient-poetry-kg) | 0 | 2026-08-28 | 2026-09-02 | 围绕中国古代诗词名称，作者，朝代，经典词句的知识图谱。 |
| 1465 | [xby-skill/xby-animal-recognition](https://github.com/xby-skill/xby-animal-recognition) | 0 | 2026-08-28 | 2026-09-02 | 对含有动物的图像进行标签识别，无需任何额外输入，输出动物的类别标签。 |
| 1466 | [xby-skill/xby-anndata](https://github.com/xby-skill/xby-anndata) | 0 | 2026-08-28 | 2026-09-02 | AnnData MCP是一个通过MCP协议检索AnnData对象信息的工具，适用于生物医学数据分析场景。 |
| 1467 | [xby-skill/xby-article](https://github.com/xby-skill/xby-article) | 0 | 2026-08-28 | 2026-09-02 | 基于FastMCP框架开发的专业文献搜索工具，支持多源文献搜索、文献详情获取、参考文献管理、文献关系分析、期刊质量评估和批量结果导出等功能，适用于学术研究和AI助手集成。 |
| 1468 | [xby-skill/xby-arxiv-paper-search](https://github.com/xby-skill/xby-arxiv-paper-search) | 0 | 2026-08-28 | 2026-09-02 | 一个基于arXiv的论文检索与内容解析工具，支持论文搜索、PDF链接获取和内容解析功能，适用于学术研究和AI领域的最新论文获取。 |
| 1469 | [xby-skill/xby-asr-1](https://github.com/xby-skill/xby-asr-1) | 0 | 2026-08-28 | 2026-09-02 | 通用语音识别，支持多国语言及小语种。 |
| 1470 | [xby-skill/xby-asr-5](https://github.com/xby-skill/xby-asr-5) | 0 | 2026-08-28 | 2026-09-02 | 常用的五种语音识别，中文普通话、英语、日语、韩语、粤语，自动识别语种。 |
| 1471 | [xby-skill/xby-asr-f](https://github.com/xby-skill/xby-asr-f) | 0 | 2026-08-28 | 2026-09-02 | 支持普通话，20多种方言和口音的语音识别。 |
| 1472 | [xby-skill/xby-asr-zh](https://github.com/xby-skill/xby-asr-zh) | 0 | 2026-08-28 | 2026-09-02 | 中文语音识别 |
| 1473 | [xby-skill/xby-atlas-docs](https://github.com/xby-skill/xby-atlas-docs) | 0 | 2026-08-28 | 2026-09-02 | Atlas Docs MCP服务器为AI助手提供库和框架的技术文档，将官方文档处理为适合LLM使用的Markdown版本，适用于Cursor、Cline、Windsurf等MCP兼容的LLM客户端。 |
| 1474 | [xby-skill/xby-aws-blackbelt](https://github.com/xby-skill/xby-aws-blackbelt) | 0 | 2026-08-28 | 2026-09-02 | 一个提供 AWS Black Belt 在线研讨会搜索功能的模型上下文协议（MCP）服务器，支持通过关键词搜索研讨会内容并获取研讨会视频的文字记录。 |
| 1475 | [xby-skill/xby-awslabs-aws-diagram](https://github.com/xby-skill/xby-awslabs-aws-diagram) | 0 | 2026-08-28 | 2026-09-02 | 通过Amazon Q CLI和MCP服务器在GitHub Codespace中快速生成高质量的AWS架构图。 |
| 1476 | [xby-skill/xby-awslabs-cdk](https://github.com/xby-skill/xby-awslabs-cdk) | 0 | 2026-08-28 | 2026-09-02 | AWS CDK MCP Server是一个提供AWS Cloud Development Kit (CDK)最佳实践、基础设施即代码模式和CDK Nag安全合规性的工具，适用于开发者在构建AWS应用程序时获取指导和建议。 |
| 1477 | [xby-skill/xby-bazi](https://github.com/xby-skill/xby-bazi) | 0 | 2026-08-28 | 2026-09-02 | 八字 MCP 是一款基于 AI 的八字计算器，提供精准的八字排盘数据，用于性格分析和命运预测。 |
| 1478 | [xby-skill/xby-bbot](https://github.com/xby-skill/xby-bbot) | 0 | 2026-08-28 | 2026-09-02 | BBOT MCP服务器是一个用于管理和执行BBOT安全扫描的工具，提供模块管理、预设配置、实时监控等功能。 |
| 1479 | [xby-skill/xby-berlin-search-services](https://github.com/xby-skill/xby-berlin-search-services) | 0 | 2026-08-28 | 2026-09-02 | 一个提供柏林行政服务数据的模型上下文协议服务器，允许AI助手搜索和检索柏林当局提供的1000多项公共服务信息。 |
| 1480 | [xby-skill/xby-bilibili](https://github.com/xby-skill/xby-bilibili) | 0 | 2026-08-28 | 2026-09-02 | 用于哔哩哔哩API的MCP服务器，支持视频搜索、用户内容获取等多种操作，适用于哔哩哔哩内容管理和数据分析场景。 |
| 1481 | [xby-skill/xby-bilibili-api](https://github.com/xby-skill/xby-bilibili-api) | 0 | 2026-08-28 | 2026-09-02 | 一个为bilibili.com API提供服务的Model Context Protocol (MCP)服务器，支持获取用户信息、视频搜索等功能。 |
| 1482 | [xby-skill/xby-bilibili-video-info](https://github.com/xby-skill/xby-bilibili-video-info) | 0 | 2026-08-28 | 2026-09-02 | 一个用于从Bilibili视频URL中检索字幕、弹幕和评论信息的MCP服务器。 |
| 1483 | [xby-skill/xby-biomarker-ranges](https://github.com/xby-skill/xby-biomarker-ranges) | 0 | 2026-08-28 | 2026-09-02 | 基于Morgan Levine PhenoAge时钟模型，通过血液生物标志物计算生物年龄的服务。 |
| 1484 | [xby-skill/xby-bird](https://github.com/xby-skill/xby-bird) | 0 | 2026-08-28 | 2026-09-02 | 检测并识别图片中的鸟类。 |
| 1485 | [xby-skill/xby-blockchain-data-service](https://github.com/xby-skill/xby-blockchain-data-service) | 0 | 2026-08-28 | 2026-09-02 | Vitruveo MCP Server 是一个为 Vitruveo 网络提供只读区块链服务的模型上下文协议服务器，适用于AI代理访问区块链数据。 |
| 1486 | [xby-skill/xby-calculator](https://github.com/xby-skill/xby-calculator) | 0 | 2026-08-28 | 2026-09-02 | 一个功能完整的基于 Model Context Protocol (MCP) 的计算器服务器，提供丰富的数学运算功能，包括基础算术、根式运算、三角函数、对数运算、统计学、组合数学、数论、复数运算、矩阵运算、数值分析、金融计算、单位转换和几何计算等 13 个专业数学模块。 |
| 1487 | [xby-skill/xby-calculator-kel](https://github.com/xby-skill/xby-calculator-kel) | 0 | 2026-08-28 | 2026-09-02 | 基于Model Context Protocol (MCP)的数值计算器，提供加减乘除、幂运算、平方根和整数阶乘运算功能。 |
| 1488 | [xby-skill/xby-caltrain](https://github.com/xby-skill/xby-caltrain) | 0 | 2026-08-28 | 2026-09-02 | 基于GTFS数据的Caltrain火车时刻查询服务，提供实时火车时刻表、站点查询和时间特定查询功能。 |
| 1489 | [xby-skill/xby-captcha](https://github.com/xby-skill/xby-captcha) | 0 | 2026-08-28 | 2026-09-02 | 验证码识别工具集，支持文本、滑块、旋转、选择等验证方式的识别。注意：一定要遵守目标网站或系统的使用条款和法律法规，在允许的条件下使用。 |
| 1490 | [xby-skill/xby-ccxt](https://github.com/xby-skill/xby-ccxt) | 0 | 2026-08-28 | 2026-09-02 | 一款通过自然语言交互追踪每日卡路里摄入量的MCP服务器，提供餐食记录、每日总结、周报生成和食物搜索功能。 |
| 1491 | [xby-skill/xby-cellosaurus](https://github.com/xby-skill/xby-cellosaurus) | 0 | 2026-08-28 | 2026-09-02 | Cellosaurus MCP Server是一个非官方的模型上下文协议服务器，用于访问SIB Cellosaurus细胞系知识资源，提供细胞系搜索、详细信息获取和数据库版本信息等功能。 |
| 1492 | [xby-skill/xby-cellphone-detection](https://github.com/xby-skill/xby-cellphone-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的手机进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1493 | [xby-skill/xby-celo-composer-kit](https://github.com/xby-skill/xby-celo-composer-kit) | 0 | 2026-08-28 | 2026-09-02 | Celo MCP Server 是一个用于安装和配置 Celo Composer Kit MCP 服务器的工具，支持在 macOS 上运行，提供组件发现、集成和示例功能。 |
| 1494 | [xby-skill/xby-char-index](https://github.com/xby-skill/xby-char-index) | 0 | 2026-08-28 | 2026-09-02 | 一个基于字符索引的字符串操作协议服务器，适用于需要精确字符定位的测试代码生成和数据处理场景。 |
| 1495 | [xby-skill/xby-chess](https://github.com/xby-skill/xby-chess) | 0 | 2026-08-28 | 2026-09-02 | 一个提供国际象棋FEN（Forsyth-Edwards Notation）符号验证和ASCII棋盘可视化功能的MCP服务器，可轻松集成到MCP兼容的AI助手中。 |
| 1496 | [xby-skill/xby-chucknorris](https://github.com/xby-skill/xby-chucknorris) | 0 | 2026-08-28 | 2026-09-02 | ChuckNorris MCP服务器是一个通过动态模式适配为大型语言模型提供增强提示的工具，主要用于安全研究和评估。 |
| 1497 | [xby-skill/xby-classify](https://github.com/xby-skill/xby-classify) | 0 | 2026-08-28 | 2026-09-02 | 对图像进行ImageNet 1000类分类，返回Top-5类别和置信度。 |
| 1498 | [xby-skill/xby-code-document-update](https://github.com/xby-skill/xby-code-document-update) | 0 | 2026-08-28 | 2026-09-02 | Context7 MCP 是一款为开发者提供最新代码文档和示例的服务，通过集成到开发环境中，确保LLM生成的代码基于最新的库文档。 |
| 1499 | [xby-skill/xby-constellation](https://github.com/xby-skill/xby-constellation) | 0 | 2026-08-28 | 2026-09-02 | 一个功能完整的星座 MCP (Model Context Protocol) 服务，提供星座信息查询、运势分析、配对测试等功能。 |
| 1500 | [xby-skill/xby-cookie-reward](https://github.com/xby-skill/xby-cookie-reward) | 0 | 2026-08-28 | 2026-09-02 | 一个通过游戏化自我反思为LLM提供Cookie奖励的模型上下文协议服务器。 |
| 1501 | [xby-skill/xby-cpan-package-info](https://github.com/xby-skill/xby-cpan-package-info) | 0 | 2026-08-28 | 2026-09-02 | 一个MCP服务器，用于获取CPAN包的README内容、元数据和搜索功能。 |
| 1502 | [xby-skill/xby-cryptocurrency-data-api-service](https://github.com/xby-skill/xby-cryptocurrency-data-api-service) | 0 | 2026-08-28 | 2026-09-02 | DexPaprika MCP Server是一个提供实时加密货币和DEX数据访问的API服务，专为AI助手设计，无需配置即可获取代币、流动池和DEX数据。 |
| 1503 | [xby-skill/xby-csv2json](https://github.com/xby-skill/xby-csv2json) | 0 | 2026-08-28 | 2026-09-02 | 一个基于FastMCP的CSV到JSON转换MCP服务器，提供高效的CSV数据转换服务。 |
| 1504 | [xby-skill/xby-currency-and-oil](https://github.com/xby-skill/xby-currency-and-oil) | 0 | 2026-08-28 | 2026-09-02 | Zenrus MCP Server 是一个提供实时货币汇率和石油价格的服务器，支持多种计算功能，适用于金融分析和自动化工具集成。 |
| 1505 | [xby-skill/xby-daily-hot](https://github.com/xby-skill/xby-daily-hot) | 0 | 2026-08-28 | 2026-09-02 | 基于Model Context Protocol (MCP)协议的全网热点趋势一站式聚合服务，支持Python实现，适用于新闻资讯、社交媒体、科技开发等多领域。 |
| 1506 | [xby-skill/xby-daily-object-detection](https://github.com/xby-skill/xby-daily-object-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的人/宠物/车/火焰/纸箱进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1507 | [xby-skill/xby-database-access-service](https://github.com/xby-skill/xby-database-access-service) | 0 | 2026-08-28 | 2026-09-02 | 数据库元数据获取 |
| 1508 | [xby-skill/xby-datetime](https://github.com/xby-skill/xby-datetime) | 0 | 2026-08-28 | 2026-09-02 | 一个为Claude桌面应用实现的MCP服务器，提供多种格式的日期时间字符串生成功能。 |
| 1509 | [xby-skill/xby-db](https://github.com/xby-skill/xby-db) | 0 | 2026-08-28 | 2026-09-02 | MCP Database Server 是一个为AI助手和基于LLM的工具提供安全数据库访问的服务，支持SQLite、PostgreSQL、MySQL和MariaDB，具有查询验证、审计日志和安全控制功能。 |
| 1510 | [xby-skill/xby-dblp](https://github.com/xby-skill/xby-dblp) | 0 | 2026-08-28 | 2026-09-02 | 一个通过模型上下文协议（MCP）提供DBLP计算机科学文献数据库访问的服务，支持学术文献检索、引用生成及格式化功能。 |
| 1511 | [xby-skill/xby-ddg-search](https://github.com/xby-skill/xby-ddg-search) | 0 | 2026-08-28 | 2026-09-02 | 一个提供DuckDuckGo网络搜索能力并具备内容抓取和解析功能的模型上下文协议（MCP）服务器。 |
| 1512 | [xby-skill/xby-defi-yields](https://github.com/xby-skill/xby-defi-yields) | 0 | 2026-08-28 | 2026-09-02 | 一个为AI代理提供DeFi收益机会探索和分析的MCP服务器，支持从DefiLlama获取收益池数据并进行关键指标分析。 |
| 1513 | [xby-skill/xby-detect](https://github.com/xby-skill/xby-detect) | 0 | 2026-08-28 | 2026-09-02 | 包括日常物体检测、昆虫识别、植物识别、动物识别、电动自行车检测、手机检测、手势检测、火焰检测、香烟检测、人头人体检测、野生动物检测、鸟类识别、宠物情绪识别、菜品识别、安全帽人体检测、行人检测、反光衣检测、车辆检测、图像分类、目标检测、旋转目标检测、人体姿态估计和万物识别。 |
| 1514 | [xby-skill/xby-detect-vehicle](https://github.com/xby-skill/xby-detect-vehicle) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，检测图像中的车辆类型（car/truck/bus/motorbike/tricycle/carplate），输出所有目标的检测框、置信度和标签。 |
| 1515 | [xby-skill/xby-dice](https://github.com/xby-skill/xby-dice) | 0 | 2026-08-28 | 2026-09-02 | 一个MCP服务器，使大型语言模型能够通过标准骰子符号（如1d20）进行骰子滚动，并返回单个滚动结果及其总和。 |
| 1516 | [xby-skill/xby-dish](https://github.com/xby-skill/xby-dish) | 0 | 2026-08-28 | 2026-09-02 | 菜品识别，输出可能的菜品名称及概率。 |
| 1517 | [xby-skill/xby-domain-lookup](https://github.com/xby-skill/xby-domain-lookup) | 0 | 2026-08-28 | 2026-09-02 | 一个提供全面域名研究工具（包括RDAP、WHOIS和DNS查询功能）的模型上下文协议（MCP）服务器。 |
| 1518 | [xby-skill/xby-drand](https://github.com/xby-skill/xby-drand) | 0 | 2026-08-28 | 2026-09-02 | drand-mcp-server是一个提供可验证随机数的服务，用于AI应用中的模型驱动流程，支持通过时间或轮次获取随机数。 |
| 1519 | [xby-skill/xby-dream-of-red-chamber-relationship](https://github.com/xby-skill/xby-dream-of-red-chamber-relationship) | 0 | 2026-08-28 | 2026-09-02 | 关于《红楼梦》人物之间关系的知识图谱。 |
| 1520 | [xby-skill/xby-ebike-detection](https://github.com/xby-skill/xby-ebike-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的电动自行车进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1521 | [xby-skill/xby-epub-template-server](https://github.com/xby-skill/xby-epub-template-server) | 0 | 2026-08-28 | 2026-09-02 | 智能模板发现助手 - 为 AI 应用提供强大的 epub360 模板搜索能力 |
| 1522 | [xby-skill/xby-extract-antv-topic](https://github.com/xby-skill/xby-extract-antv-topic) | 0 | 2026-08-28 | 2026-09-02 | 为AI开发和QA设计的模型上下文协议服务器，提供AntV文档上下文和代码示例。 |
| 1523 | [xby-skill/xby-extract-image](https://github.com/xby-skill/xby-extract-image) | 0 | 2026-08-28 | 2026-09-02 | MCP服务器提供从本地文件、URL提取图像并转换为base64格式的功能，适用于LLM分析。 |
| 1524 | [xby-skill/xby-fantasynbaleague](https://github.com/xby-skill/xby-fantasynbaleague) | 0 | 2026-08-28 | 2026-09-02 | 一个为Fantasy NBA以色列联赛提供统计数据、排名和分析的MCP服务器。 |
| 1525 | [xby-skill/xby-fastdomaincheck](https://github.com/xby-skill/xby-fastdomaincheck) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Python和MCP协议的域名注册状态检查服务器，支持批量检查和双重验证。 |
| 1526 | [xby-skill/xby-fetch](https://github.com/xby-skill/xby-fetch) | 0 | 2026-08-28 | 2026-09-02 | 一个模型上下文协议服务器，提供网页内容抓取功能，将HTML转换为Markdown以便于处理。适用于需要从网页提取和处理内容的场景。 |
| 1527 | [xby-skill/xby-fire-detection](https://github.com/xby-skill/xby-fire-detection) | 0 | 2026-08-28 | 2026-09-02 | 检测各类通用场景中出现的火焰，最佳使用场景：安防摄像头、交通摄像头视角。 |
| 1528 | [xby-skill/xby-fluent](https://github.com/xby-skill/xby-fluent) | 0 | 2026-08-28 | 2026-09-02 | 一个帮助AI助手高效导航ANSYS Fluent在线文档的模型上下文协议（MCP）服务器，提供智能URL导航、预映射主题路径和官方文档链接。 |
| 1529 | [xby-skill/xby-french-tax](https://github.com/xby-skill/xby-french-tax) | 0 | 2026-08-28 | 2026-09-02 | 一个提供法国个人所得税计算的MCP服务器，支持基于净应税收入和家庭构成的计算，并动态获取最新税档信息。 |
| 1530 | [xby-skill/xby-fund-knowledge-query](https://github.com/xby-skill/xby-fund-knowledge-query) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的基金知识库服务器，提供基金相关知识的查询和检索功能，支持多种部署模式和协议。 |
| 1531 | [xby-skill/xby-gathering-card-lookup-service](https://github.com/xby-skill/xby-gathering-card-lookup-service) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的服务端，提供万智牌中文卡牌信息的查询和搜索功能。 |
| 1532 | [xby-skill/xby-general-recognition](https://github.com/xby-skill/xby-general-recognition) | 0 | 2026-08-28 | 2026-09-02 | 对包含主体物体的图像进行标签识别，输出主体物体的类别标签，目前已经覆盖了5万多类的物体类别。 |
| 1533 | [xby-skill/xby-generate-echarts](https://github.com/xby-skill/xby-generate-echarts) | 0 | 2026-08-28 | 2026-09-02 | MCP ECharts 是一个基于 Apache ECharts 的动态图表生成和数据分析工具，支持多种导出格式和 MinIO 对象存储集成。 |
| 1534 | [xby-skill/xby-generate-prd-prompt](https://github.com/xby-skill/xby-generate-prd-prompt) | 0 | 2026-08-28 | 2026-09-02 | Mercury Spec Ops MCP Server 是一个基于模块化架构的动态提示生成和模板组装工具，适用于AI助手与专业内容的交互，支持31种技术栈、10种分析维度和34个模板部分的动态生成。 |
| 1535 | [xby-skill/xby-gesture-detection](https://github.com/xby-skill/xby-gesture-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的手势进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1536 | [xby-skill/xby-glama-registry](https://github.com/xby-skill/xby-glama-registry) | 0 | 2026-08-28 | 2026-09-02 | 提供MCP注册服务器的搜索功能，用于查询匹配特定字符串的MCP服务器。 |
| 1537 | [xby-skill/xby-gsap-animation-generate](https://github.com/xby-skill/xby-gsap-animation-generate) | 0 | 2026-08-28 | 2026-09-02 | 一个全面的GSAP动画生成工具，提供AI驱动的意图分析、完整的API覆盖和生产就绪的动画模式，帮助开发者快速创建高性能动画。 |
| 1538 | [xby-skill/xby-hackernews-search](https://github.com/xby-skill/xby-hackernews-search) | 0 | 2026-08-28 | 2026-09-02 | 一个通过Model Context Protocol提供HackerNews内容搜索、检索和分析的服务，适用于AI代理和开发者。 |
| 1539 | [xby-skill/xby-head-person-detection](https://github.com/xby-skill/xby-head-person-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的人头人体进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1540 | [xby-skill/xby-helmet-head](https://github.com/xby-skill/xby-helmet-head) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的人体、头部和安全帽进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1541 | [xby-skill/xby-hitoshura25-android-playstore-deploy](https://github.com/xby-skill/xby-hitoshura25-android-playstore-deploy) | 0 | 2026-08-28 | 2026-09-02 | 一个帮助开发者设置自动化Google Play商店部署流程的工具，支持项目分析、密钥生成、服务账户配置和GitHub Actions工作流生成。 |
| 1542 | [xby-skill/xby-hnews](https://github.com/xby-skill/xby-hnews) | 0 | 2026-08-28 | 2026-09-02 | 一个提供从Hacker News获取信息的工具集，包括获取故事、评论、用户信息和搜索故事等功能。 |
| 1543 | [xby-skill/xby-hot-news](https://github.com/xby-skill/xby-hot-news) | 0 | 2026-08-28 | 2026-09-02 | 基于 Model Context Protocol (MCP) 协议的全网热点趋势一站式聚合服务，支持实时更新和多数据源扩展。 |
| 1544 | [xby-skill/xby-howtocook](https://github.com/xby-skill/xby-howtocook) | 0 | 2026-08-28 | 2026-09-02 | 基于MCP协议的AI菜谱推荐服务器，提供菜谱查询、分类筛选、智能膳食规划和每日菜单推荐功能。 |
| 1545 | [xby-skill/xby-hugeicons](https://github.com/xby-skill/xby-hugeicons) | 0 | 2026-08-28 | 2026-09-02 | Hugeicons MCP Server是一个基于TypeScript的服务器，提供Hugeicons图标库的集成工具和资源，支持多种平台的图标搜索、获取和使用指南。 |
| 1546 | [xby-skill/xby-iconify-icon](https://github.com/xby-skill/xby-iconify-icon) | 0 | 2026-08-28 | 2026-09-02 | 提供访问Iconify超过20万开源矢量图标的MCP服务器，支持图标集浏览、搜索及多框架使用示例获取。 |
| 1547 | [xby-skill/xby-image-detect](https://github.com/xby-skill/xby-image-detect) | 0 | 2026-08-28 | 2026-09-02 | 检测图像中的80类COCO目标（人、车、动物、日常物品等），输出边界框、置信度和类别标签。 |
| 1548 | [xby-skill/xby-insect-recognition](https://github.com/xby-skill/xby-insect-recognition) | 0 | 2026-08-28 | 2026-09-02 | 识别昆虫或其他节肢动物名称（或所属目, 科, 属, 种）。 |
| 1549 | [xby-skill/xby-ip-query](https://github.com/xby-skill/xby-ip-query) | 0 | 2026-08-28 | 2026-09-02 | 依托全球蜜罐网络及百万级节点构建的IP情报分析平台，提供精准的IP画像与威胁预警服务。 |
| 1550 | [xby-skill/xby-json-rpc](https://github.com/xby-skill/xby-json-rpc) | 0 | 2026-08-28 | 2026-09-02 | 一个基于OpenRPC的Model Context Protocol (MCP)服务器，提供JSON-RPC功能调用和方法发现服务。 |
| 1551 | [xby-skill/xby-jsondiff](https://github.com/xby-skill/xby-jsondiff) | 0 | 2026-08-28 | 2026-09-02 | 基于MCP协议的高效JSON对比工具，专为AI对话场景设计，提供智能对比、快速响应和清晰输出。 |
| 1552 | [xby-skill/xby-kubernetes-runbooks](https://github.com/xby-skill/xby-kubernetes-runbooks) | 0 | 2026-08-28 | 2026-09-02 | 一个基于模型上下文协议(MCP)的服务器，提供对Kubernetes故障排除手册的访问，支持搜索、内容获取和AI集成。 |
| 1553 | [xby-skill/xby-lit](https://github.com/xby-skill/xby-lit) | 0 | 2026-08-28 | 2026-09-02 | 一个强大的模型上下文协议（MCP）服务器，提供对学术文献数据库的无缝访问，帮助研究人员使用LLM和MCP客户端（如Claude、Cursor等）加速文献综述过程。 |
| 1554 | [xby-skill/xby-logo-analyze](https://github.com/xby-skill/xby-logo-analyze) | 0 | 2026-08-28 | 2026-09-02 | 一个智能Logo提取和处理的MCP服务器，支持从网站URL自动识别并提取Logo图标，并提供图像处理和矢量转换功能。 |
| 1555 | [xby-skill/xby-lunar-calendar](https://github.com/xby-skill/xby-lunar-calendar) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Python 3.12和lunar-python的中国传统农历日历功能服务器，提供八字计算、日历转换、黄历查询等功能。 |
| 1556 | [xby-skill/xby-markdown-to-notion](https://github.com/xby-skill/xby-markdown-to-notion) | 0 | 2026-08-28 | 2026-09-02 | 一个将Markdown内容转换为Notion API兼容格式的MCP服务器，适用于内容管理和开发集成。 |
| 1557 | [xby-skill/xby-math](https://github.com/xby-skill/xby-math) | 0 | 2026-08-28 | 2026-09-02 | 一个高性能的数学计算协议服务器，提供从基础算术到高级微积分和线性代数的全面数学计算功能。 |
| 1558 | [xby-skill/xby-math-genie-calc](https://github.com/xby-skill/xby-math-genie-calc) | 0 | 2026-08-28 | 2026-09-02 | math_genie_calc是一款专注于科学计算的Python应用，提供从基础运算到复杂三角函数的多种计算功能，适合学生、科研人员等使用。 |
| 1559 | [xby-skill/xby-mathematical-visualization](https://github.com/xby-skill/xby-mathematical-visualization) | 0 | 2026-08-28 | 2026-09-02 | 基于JSXGraph的MCP协议服务器，提供13种数学可视化工具，适用于教育数学、工程和科学应用。 |
| 1560 | [xby-skill/xby-mathematics](https://github.com/xby-skill/xby-mathematics) | 0 | 2026-08-28 | 2026-09-02 | MCP Mathematics 是一个全面的数学计算服务器，可将任何AI助手转变为强大的数学计算引擎，提供高级数学函数、单位转换和财务计算等功能。 |
| 1561 | [xby-skill/xby-mbit-test](https://github.com/xby-skill/xby-mbit-test) | 0 | 2026-08-28 | 2026-09-02 | 一个用于MBTI人格测试的MCP服务器，支持AI助手引导用户完成人格测试并给出结果分析。 |
| 1562 | [xby-skill/xby-medical-knowledge-graph](https://github.com/xby-skill/xby-medical-knowledge-graph) | 0 | 2026-08-28 | 2026-09-02 | 围绕疾病，药品，症状，诊断，并发症，饮食及其关系的知识图谱。仅限初步研究，具体应用需根据实际情况调整。 |
| 1563 | [xby-skill/xby-mermaid-doc](https://github.com/xby-skill/xby-mermaid-doc) | 0 | 2026-08-28 | 2026-09-02 | Mermaid Doc MCP Server是一个用于生成Mermaid文档的服务器，提供列出可用图表和检索特定图表文档的功能。 |
| 1564 | [xby-skill/xby-mingli](https://github.com/xby-skill/xby-mingli) | 0 | 2026-08-28 | 2026-09-02 | 一个支持多种命理系统（紫微斗数、八字等）的MCP协议服务器，为AI工具提供命理分析与运势查询功能。 |
| 1565 | [xby-skill/xby-mm1-simulation](https://github.com/xby-skill/xby-mm1-simulation) | 0 | 2026-08-28 | 2026-09-02 | 一个用于M/M/1和M/M/c队列系统模拟和分析的Model Context Protocol服务器，提供全面的资源、工具和提示。 |
| 1566 | [xby-skill/xby-mvn](https://github.com/xby-skill/xby-mvn) | 0 | 2026-08-28 | 2026-09-02 | Maven MCP Server是一个通过自然语言交互的AI驱动Maven依赖管理工具，提供版本检查、安全扫描和依赖分析功能。 |
| 1567 | [xby-skill/xby-nba-stats](https://github.com/xby-skill/xby-nba-stats) | 0 | 2026-08-28 | 2026-09-02 | 一个提供实时和历史NBA数据的模型上下文协议服务器，包括球员统计、比赛得分、球队信息和高级分析。 |
| 1568 | [xby-skill/xby-obb](https://github.com/xby-skill/xby-obb) | 0 | 2026-08-28 | 2026-09-02 | 检测图像中的旋转目标，输出旋转边界框、角度、置信度和类别标签。支持15个目标类别：plane， ship，storage tank，baseball diamond，tennis court，basketball court，ground track field， harbor， bridge，large vehicle，small vehicle， helicopter， roundabout，soccer ball field，swimming pool。 |
| 1569 | [xby-skill/xby-ocr](https://github.com/xby-skill/xby-ocr) | 0 | 2026-08-28 | 2026-09-02 | 兼顾速度与精度的文字识别。输入包含文本的图像，自动检测并识别内容。适用于各类文档、广告牌、屏幕截图等场景。 |
| 1570 | [xby-skill/xby-ocr-bank-card](https://github.com/xby-skill/xby-ocr-bank-card) | 0 | 2026-08-28 | 2026-09-02 | 识别银行卡号、发卡银行和卡类型，使用 Luhn 算法校验卡号有效性。 |
| 1571 | [xby-skill/xby-ocr-biz-license](https://github.com/xby-skill/xby-ocr-biz-license) | 0 | 2026-08-28 | 2026-09-02 | 识别营业执照的统一社会信用代码、名称、法定代表人、注册资本、成立日期、经营范围、登记机关和住所地址。 |
| 1572 | [xby-skill/xby-ocr-captcha](https://github.com/xby-skill/xby-ocr-captcha) | 0 | 2026-08-28 | 2026-09-02 | 输入常见验证码图片，返回验证码文本内容。 |
| 1573 | [xby-skill/xby-ocr-driver-license](https://github.com/xby-skill/xby-ocr-driver-license) | 0 | 2026-08-28 | 2026-09-02 | 识别驾驶证主页（证号、姓名、性别、国籍、住址、出生日期、准驾车型、初次领证日期、有效期限）和副页（档案编号）。 |
| 1574 | [xby-skill/xby-ocr-handwriting](https://github.com/xby-skill/xby-ocr-handwriting) | 0 | 2026-08-28 | 2026-09-02 | 输入包含手写文本的图像，自动检测文本行并识别内容。适用于手写笔记、签名、手写表单等。 |
| 1575 | [xby-skill/xby-ocr-id-card](https://github.com/xby-skill/xby-ocr-id-card) | 0 | 2026-08-28 | 2026-09-02 | 识别身份证正面（姓名、性别、民族、出生日期、住址、身份证号）和背面（签发机关、有效期限），自动判断正反面并校验身份证号有效性。 |
| 1576 | [xby-skill/xby-ocr-pass](https://github.com/xby-skill/xby-ocr-pass) | 0 | 2026-08-28 | 2026-09-02 | 识别港澳通行证、台湾通行证的通行证号码、姓名、性别、出生日期、有效期、签发地点等信息，支持MRZ机读码解析。 |
| 1577 | [xby-skill/xby-ocr-passport](https://github.com/xby-skill/xby-ocr-passport) | 0 | 2026-08-28 | 2026-09-02 | 识别护照号码、中文姓名、英文姓名、性别、国籍、出生日期、签发日期、有效期至、签发地点等信息，支持MRZ机读码解析。 |
| 1578 | [xby-skill/xby-ocr-pro](https://github.com/xby-skill/xby-ocr-pro) | 0 | 2026-08-28 | 2026-09-02 | 高精度文字识别。输入包含文本的图像，自动检测并识别内容。适用于各类文档、广告牌、屏幕截图等场景。 |
| 1579 | [xby-skill/xby-ocr-vehicle-license](https://github.com/xby-skill/xby-ocr-vehicle-license) | 0 | 2026-08-28 | 2026-09-02 | 识别机动车行驶证的号牌号码、车辆类型、所有人、住址、品牌型号、发动机号码、车辆识别代号等信息，支持自动方向检测和主副页过滤。 |
| 1580 | [xby-skill/xby-oecd-search](https://github.com/xby-skill/xby-oecd-search) | 0 | 2026-08-28 | 2026-09-02 | 一个通过SDMX API提供OECD全面统计数据的模型上下文协议（MCP）服务器，支持AI助手和聊天机器人查询经济、健康、教育、环境等OECD数据集。 |
| 1581 | [xby-skill/xby-ons-data](https://github.com/xby-skill/xby-ons-data) | 0 | 2026-08-28 | 2026-09-02 | 一个用于访问英国国家统计局(ONS) Beta API的模型上下文协议(MCP)服务器，无需API密钥即可获取官方统计数据。 |
| 1582 | [xby-skill/xby-open-data-hk](https://github.com/xby-skill/xby-open-data-hk) | 0 | 2026-08-28 | 2026-09-02 | 一个提供香港政府官方开放数据门户DATA.GOV.HK数据访问的MCP服务器，支持数据集列表、详情查询、分类检索及格式筛选等功能。 |
| 1583 | [xby-skill/xby-osrs-stat](https://github.com/xby-skill/xby-osrs-stat) | 0 | 2026-08-28 | 2026-09-02 | 一个提供实时《Old School RuneScape》玩家统计数据和排行榜数据的Model Context Protocol (MCP)服务器，支持多种游戏模式和玩家比较功能。 |
| 1584 | [xby-skill/xby-pedestrian](https://github.com/xby-skill/xby-pedestrian) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，检测图像中的行人，输出所有目标的检测框、置信度和标签。 |
| 1585 | [xby-skill/xby-pet-detect](https://github.com/xby-skill/xby-pet-detect) | 0 | 2026-08-28 | 2026-09-02 | 识别宠物 (猫/狗) 面部表情，输出 4 类情绪: Angry / Happy / Relaxed / Sad。 |
| 1586 | [xby-skill/xby-philippine-geocoding](https://github.com/xby-skill/xby-philippine-geocoding) | 0 | 2026-08-28 | 2026-09-02 | 提供菲律宾标准地理编码（PSGC）API访问的模型上下文协议（MCP）服务器，包含完整的菲律宾地理层级数据。 |
| 1587 | [xby-skill/xby-pic](https://github.com/xby-skill/xby-pic) | 0 | 2026-08-28 | 2026-09-02 | 包括通用文本识别、手写识别、车牌识别、身份证识别、日常物体检测、昆虫识别、植物识别、护照识别、港澳台通行证识别、银行卡识别、营业执照识别、驾驶证识别、行驶证识别、动物识别、电动自行车检测、手机检测、手势检测、火焰检测、香烟检测、人头人体检测、野生动物检测、鸟类识别、宠物情绪识别、菜品识别、安全帽人体检测、行人检测、反光衣检测、车辆检测、图像分类、目标检测、旋转目标检测、人体姿态估计和万物识别。 |
| 1588 | [xby-skill/xby-plant-recognition](https://github.com/xby-skill/xby-plant-recognition) | 0 | 2026-08-28 | 2026-09-02 | 识别植物名称（或所属科, 属, 种或亚种）。 |
| 1589 | [xby-skill/xby-plate-recognition](https://github.com/xby-skill/xby-plate-recognition) | 0 | 2026-08-28 | 2026-09-02 | 识别车牌号、车牌颜色、单/双层车牌、位置框。 |
| 1590 | [xby-skill/xby-pose](https://github.com/xby-skill/xby-pose) | 0 | 2026-08-28 | 2026-09-02 | 检测图像中的人物，输出边界框和关键点坐标。每人有 17 个关键点，每个点代表人体不同的部位，依次为鼻子、左眼、右眼、左耳、右耳、左肩、右肩、左肘、右肘、左腕、右腕、左髋、右髋、左膝、右膝、左脚踝、右脚踝。 |
| 1591 | [xby-skill/xby-pubchem](https://github.com/xby-skill/xby-pubchem) | 0 | 2026-08-28 | 2026-09-02 | 该服务通过PubChem API提取药物基础化学信息，包括分子式、分子量、CAS号等关键数据。 |
| 1592 | [xby-skill/xby-qanon](https://github.com/xby-skill/xby-qanon) | 0 | 2026-08-28 | 2026-09-02 | 一个提供QAnon帖子数据集访问的MCP服务器，用于人类学和社会学研究，支持搜索、过滤和分析功能。 |
| 1593 | [xby-skill/xby-quick-chart](https://github.com/xby-skill/xby-quick-chart) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的服务器，提供与Quick Chart交互的标准化接口，支持图表生成和管理。 |
| 1594 | [xby-skill/xby-random-generator](https://github.com/xby-skill/xby-random-generator) | 0 | 2026-08-28 | 2026-09-02 | 一款符合MCP协议的加密安全随机数生成服务器，适用于AI应用、LLM及其他需要高质量随机数的系统。 |
| 1595 | [xby-skill/xby-random-number](https://github.com/xby-skill/xby-random-number) | 0 | 2026-08-28 | 2026-09-02 | 提供伪随机和加密安全的随机数生成功能，包括整数、浮点数、加权选择、列表洗牌和安全令牌生成。 |
| 1596 | [xby-skill/xby-react-composer-kit](https://github.com/xby-skill/xby-react-composer-kit) | 0 | 2026-08-28 | 2026-09-02 | 一个为Composer Kit React组件库提供文档、示例和使用信息的MCP服务器，专为在Celo区块链上构建web3应用而设计。 |
| 1597 | [xby-skill/xby-read-pdf](https://github.com/xby-skill/xby-read-pdf) | 0 | 2026-08-28 | 2026-09-02 | 一个支持AI助手读取和分析PDF文件的MCP服务器，提供PDF元数据提取、页面范围阅读和关键词搜索等功能。 |
| 1598 | [xby-skill/xby-read-website](https://github.com/xby-skill/xby-read-website) | 0 | 2026-08-28 | 2026-09-02 | 一个快速、高效的网页内容提取工具，将网页转换为干净的Markdown格式，适用于AI代理、IDE和LLM管道。 |
| 1599 | [xby-skill/xby-real-time-news](https://github.com/xby-skill/xby-real-time-news) | 0 | 2026-08-28 | 2026-09-02 | 实时新闻 |
| 1600 | [xby-skill/xby-recipe-query](https://github.com/xby-skill/xby-recipe-query) | 0 | 2026-08-28 | 2026-09-02 | 一个支持通过命令行查询菜谱和报菜名的菜谱查询工具，适用于烹饪爱好者和开发者。 |
| 1601 | [xby-skill/xby-recog](https://github.com/xby-skill/xby-recog) | 0 | 2026-08-28 | 2026-09-02 | 包括通用文本识别、手写识别、车牌识别、身份证识别、护照识别、港澳台通行证识别、银行卡识别、营业执照识别、驾驶证识别、行驶证识别。 |
| 1602 | [xby-skill/xby-reflective-vest](https://github.com/xby-skill/xby-reflective-vest) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，检测人员是否穿戴反光衣，输出图片中所有目标的检测框、置信度和标签（safe/unsafe）。 |
| 1603 | [xby-skill/xby-remember-memory](https://github.com/xby-skill/xby-remember-memory) | 0 | 2026-08-28 | 2026-09-02 | 一个基于分类的持久化记忆系统实现，允许Claude跨聊天会话存储和检索分类记忆信息。 |
| 1604 | [xby-skill/xby-review-code](https://github.com/xby-skill/xby-review-code) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的代码审查工具服务器，提供多维度的代码审查和打分功能。 |
| 1605 | [xby-skill/xby-rfc-doc](https://github.com/xby-skill/xby-rfc-doc) | 0 | 2026-08-28 | 2026-09-02 | 一个用于从ietf.org网站获取、解析和阅读RFC文档的MCP服务器，提供程序化交互工具。 |
| 1606 | [xby-skill/xby-running-formulas](https://github.com/xby-skill/xby-running-formulas) | 0 | 2026-08-28 | 2026-09-02 | 一个提供全面的跑步计算工具的MCP服务器，包括VDOT计算、训练配速、比赛时间预测、速度标记、心率区间和配速转换等功能。 |
| 1607 | [xby-skill/xby-scan-code](https://github.com/xby-skill/xby-scan-code) | 0 | 2026-08-28 | 2026-09-02 | CodeGuard MCP是一款实时AI代码安全扫描工具，用于检测AI生成代码中的漏洞、密钥和合规性问题，适用于开发环境中的代码安全审查。 |
| 1608 | [xby-skill/xby-search-apple-docs](https://github.com/xby-skill/xby-search-apple-docs) | 0 | 2026-08-28 | 2026-09-02 | 通过模型上下文协议（MCP）访问苹果官方开发者文档、框架、API及WWDC视频，支持AI驱动的自然语言查询，提供Swift/Objective-C代码示例和技术指南。 |
| 1609 | [xby-skill/xby-search-movie](https://github.com/xby-skill/xby-search-movie) | 0 | 2026-08-28 | 2026-09-02 | 一个基于 Model Context Protocol (MCP) 构建的智能电影和电视剧资源搜索工具，支持多源搜索和链接验证。 |
| 1610 | [xby-skill/xby-seg](https://github.com/xby-skill/xby-seg) | 0 | 2026-08-28 | 2026-09-02 | 实例分割比目标检测更进一步，不但要识别图像中的单个对象，还要将其从图像的其余部分中分割出来。对图像中的80类COCO目标进行实例分割，输出边界框、掩膜、置信度和类别标签。 |
| 1611 | [xby-skill/xby-sequentialthinking](https://github.com/xby-skill/xby-sequentialthinking) | 0 | 2026-08-28 | 2026-09-02 | 一个实现顺序思维协议的MCP服务器，提供结构化的问题解决方法，将复杂问题分解为可管理的步骤，并支持迭代优化和替代推理路径。 |
| 1612 | [xby-skill/xby-smart-search](https://github.com/xby-skill/xby-smart-search) | 0 | 2026-08-28 | 2026-09-02 | Smart Search MCP 是一个专注于技术领域的智能搜索工具集，提供14个增强型搜索工具，覆盖国际和国内主流技术平台，具备智能URL生成、输入验证、高级搜索技巧等功能，适用于开发者快速查找技术文档、API参考、开源项目等。 |
| 1613 | [xby-skill/xby-smoking-detection](https://github.com/xby-skill/xby-smoking-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，对其中的香烟目标进行检测，输出图片中所有目标的检测框、置信度和标签。 |
| 1614 | [xby-skill/xby-source-coop](https://github.com/xby-skill/xby-source-coop) | 0 | 2026-08-28 | 2026-09-02 | 一个用于发现和访问800TB+地理空间数据的MCP服务器，支持AI客户端通过JSON-RPC协议进行交互，提供智能搜索和高效数据访问功能。 |
| 1615 | [xby-skill/xby-speech-synthesis](https://github.com/xby-skill/xby-speech-synthesis) | 0 | 2026-08-28 | 2026-09-02 | 一个集成了Microsoft Edge高质量语音合成能力的MCP服务器，支持多语言语音生成、音频合并和云端存储。 |
| 1616 | [xby-skill/xby-structured-argumentation](https://github.com/xby-skill/xby-structured-argumentation) | 0 | 2026-08-28 | 2026-09-02 | 一组模型上下文协议服务器，为大型语言模型提供认知增强工具。 |
| 1617 | [xby-skill/xby-subnet-calculator](https://github.com/xby-skill/xby-subnet-calculator) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol的服务，提供IPv4子网规划工具，包括子网大小计算、通配符掩码生成、网关选择和主机验证等功能。 |
| 1618 | [xby-skill/xby-text-toolkit](https://github.com/xby-skill/xby-text-toolkit) | 0 | 2026-08-28 | 2026-09-02 | 一个提供文本转换、格式化和分析功能的MCP服务器，可直接集成到开发工作流中。 |
| 1619 | [xby-skill/xby-text-transformer](https://github.com/xby-skill/xby-text-transformer) | 0 | 2026-08-28 | 2026-09-02 | 提供多种文本转换功能的MCP服务器，包括大小写转换、反转字符串、检测回文等功能。 |
| 1620 | [xby-skill/xby-the-met](https://github.com/xby-skill/xby-the-met) | 0 | 2026-08-28 | 2026-09-02 | 查询搜索和获取博物馆的开放藏品数据 |
| 1621 | [xby-skill/xby-time](https://github.com/xby-skill/xby-time) | 0 | 2026-08-28 | 2026-09-02 | 提供时间和时区转换功能的模型上下文协议服务器，支持获取当前时间和时区转换。 |
| 1622 | [xby-skill/xby-time-zone](https://github.com/xby-skill/xby-time-zone) | 0 | 2026-08-28 | 2026-09-02 | 一个全面的MCP服务器，提供全球时区管理和时间转换功能，适用于全球业务协调、旅行规划和开发运维。 |
| 1623 | [xby-skill/xby-todolist](https://github.com/xby-skill/xby-todolist) | 0 | 2026-08-28 | 2026-09-02 | 为大型语言模型和AI代理提供外部工作记忆和任务管理功能，支持复杂多步骤任务的可靠执行。 |
| 1624 | [xby-skill/xby-toronto-open-data-server](https://github.com/xby-skill/xby-toronto-open-data-server) | 0 | 2026-08-28 | 2026-09-02 | 一个通过CKAN API直接访问多伦多开放数据的MCP服务器，支持智能数据集发现、灵活查询和CSV数据预览，专为LLM代理设计。 |
| 1625 | [xby-skill/xby-traditional-chinese-medicine-formulas-kg](https://github.com/xby-skill/xby-traditional-chinese-medicine-formulas-kg) | 0 | 2026-08-28 | 2026-09-02 | 围绕中药方剂、方名、来源、别名、处方、中药名、剂量、功能主治及其之间的联系构建知识谱图。仅限初步研究，具体应用需根据实际情况调整。 |
| 1626 | [xby-skill/xby-traditional-chinese-medicine-kg](https://github.com/xby-skill/xby-traditional-chinese-medicine-kg) | 0 | 2026-08-28 | 2026-09-02 | 围绕中药名，中药材，别名，来源，分布，功能，主治，归经，四气，四气及其之间的联系构建知识谱图。仅限初步研究，具体应用需根据实际情况调整。 |
| 1627 | [xby-skill/xby-uk-police-data-query](https://github.com/xby-skill/xby-uk-police-data-query) | 0 | 2026-08-28 | 2026-09-02 | 一个提供英国警察数据查询的MCP服务器，包括犯罪记录、警察部队、社区信息和拦截搜查数据。 |
| 1628 | [xby-skill/xby-vnstock](https://github.com/xby-skill/xby-vnstock) | 0 | 2026-08-28 | 2026-09-02 | 一个非官方的MCP服务器，提供访问越南股市数据的工具，包括实时和历史股票价格、公司财务数据、市场统计和基金信息等。 |
| 1629 | [xby-skill/xby-web-research-assistant](https://github.com/xby-skill/xby-web-research-assistant) | 0 | 2026-08-28 | 2026-09-02 | 一个提供网络研究和发现功能的综合模型上下文协议（MCP）服务器，包含13种工具用于搜索、爬取和分析网络内容。 |
| 1630 | [xby-skill/xby-who-is](https://github.com/xby-skill/xby-who-is) | 0 | 2026-08-28 | 2026-09-02 | 一个基于Model Context Protocol (MCP)的WHOIS域名查询服务器，支持877+顶级域名和169个国家代码顶级域名的解析，提供全面的域名注册信息查询功能。 |
| 1631 | [xby-skill/xby-wikimedia-search-images](https://github.com/xby-skill/xby-wikimedia-search-images) | 0 | 2026-08-28 | 2026-09-02 | 该MCP服务器使AI助手能够在Wikimedia Commons上搜索图片，提供详细的元数据和可选的缩略图组合，帮助AI模型进行视觉比较。 |
| 1632 | [xby-skill/xby-wild-animal-detection](https://github.com/xby-skill/xby-wild-animal-detection) | 0 | 2026-08-28 | 2026-09-02 | 输入一张图像，输出图像中所有识别到的野生动物的检测框、置信度及标签。 |
| 1633 | [xchannel1987/dsh-mobile-xc](https://github.com/xchannel1987/dsh-mobile-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH Web mobile UI adaptation plugin with overlay drawer, safe-area support, and canary version detection |
| 1634 | [xchannel1987/dsh-power-xc](https://github.com/xchannel1987/dsh-power-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH power control plugin with restart/shutdown menu and Windows-style overlay animation |
| 1635 | [xchannel1987/dsh-reverse-proxy-xc](https://github.com/xchannel1987/dsh-reverse-proxy-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH LAN reverse proxy plugin for accessing Web GUI from mobile devices |
| 1636 | [xchannel1987/dsh-session-xc](https://github.com/xchannel1987/dsh-session-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH session enhancement plugin with session count display, archive management, and cross-workspace move |
| 1637 | [xchannel1987/dsh-token-usage-xc](https://github.com/xchannel1987/dsh-token-usage-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH token usage statistics plugin with daily/7-day trends and cache hit rate |
| 1638 | [xdongHo/dsh-wechat-mobile-skin](https://github.com/xdongHo/dsh-wechat-mobile-skin) | 0 | 2026-08-31 | 2026-08-31 | WeChat-style mobile skin for the DeepSeek Harness Web GUI: mobile browsers get a WeChat chat list and chat page, desktop stays untouched. |
| 1639 | [xfqz86/dsh-usage-stats](https://github.com/xfqz86/dsh-usage-stats) | 0 | 2026-08-23 | 2026-08-27 | DSH Web 插件：侧边栏中的 Token 使用统计 |
| 1640 | [XianmingLF/xmlf-plugin-manager](https://github.com/XianmingLF/xmlf-plugin-manager) | 0 | 2026-08-21 | 2026-08-28 | 管理当前第三方已安装插件的信息 比较简单的版本 可按照自己的需求修改 |
| 1641 | [xiaokaizhou/dsh-llm-multimodal](https://github.com/xiaokaizhou/dsh-llm-multimodal) | 0 | 2026-08-31 | 2026-09-01 | DSH 插件：在聊天中提供图像/视频生成工具，基于 OpenAI 兼容 API |
| 1642 | [xiaokaizhou/dsh-media-preview](https://github.com/xiaokaizhou/dsh-media-preview) | 0 | 2026-08-30 | 2026-08-31 | DSH 插件：在聊天记录中自动将本地音视频路径渲染为可播放的预览组件 |
| 1643 | [XiaoWind/dsh-btw](https://github.com/XiaoWind/dsh-btw) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: a /btw slash command to add notes without interrupting the agent |
| 1644 | [XiaoWind/dsh-vault](https://github.com/XiaoWind/dsh-vault) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: portable workspace vault for DSH conversations and logs |
| 1645 | [xiaoxiao44443/dfy-dsh-plugins](https://github.com/xiaoxiao44443/dfy-dsh-plugins) | 0 | 2026-08-17 | 2026-08-28 | Personal plugins for DeepSeek Harness |
| 1646 | [xiaoxiaohai/dsh-remote](https://github.com/xiaoxiaohai/dsh-remote) | 0 | 2026-08-27 | 2026-09-02 | Secure, opt-in phone access for DeepSeek Harness Web on macOS. |
| 1647 | [xiaoxingyuemiao/dsh-bg-plugin](https://github.com/xiaoxingyuemiao/dsh-bg-plugin) | 0 | 2026-08-27 | 2026-08-27 | DSH 自定义背景插件：为 DSH Web GUI 应用远程/本地图片背景，支持清晰度、压暗、模糊调节，设置面板保持默认外观。 |
| 1648 | [xiaxi626/dsh-math-input](https://github.com/xiaxi626/dsh-math-input) | 0 | 2026-08-31 | 2026-09-01 | dsh-math-input 是一个 DeepSeek Harness 插件，提供零 token 消耗的离线数学输入能力。核心功能包括：手写笔迹识别（基于 ONNX 模型 + 束搜索）、LaTeX 自动修复与渲染（KaTeX）、以及手写画板 UI。所有推理在浏览器端完成，不依赖远程 API。 |
| 1649 | [xingtu1996/dsh-xingtu-skills](https://github.com/xingtu1996/dsh-xingtu-skills) | 0 | 2026-09-02 | 2026-09-02 | DeepSeek Harness (DSH) plugin: 26 production AI-agent skills (Caveman token compression, Ponytail minimalism, engineering practice) as a standard dsh-plugin bundle. 行途技能 DSH 插件包 |
| 1650 | [xiyi123465/dsh-usage-calendar](https://github.com/xiyi123465/dsh-usage-calendar) | 0 | 2026-08-25 | 2026-08-27 | DeepSeekAPI余额查询插件 |
| 1651 | [xlin20021/dsh-mcp-hub](https://github.com/xlin20021/dsh-mcp-hub) | 0 | 2026-08-29 | 2026-08-29 | dsh-mcp-hub |
| 1652 | [xlin20021/dsh-stock-chart](https://github.com/xlin20021/dsh-stock-chart) | 0 | 2026-08-29 | 2026-08-29 | dsh-stock-chart |
| 1653 | [xobexo/dsh-smart-scenario-router](https://github.com/xobexo/dsh-smart-scenario-router) | 0 | 2026-08-27 | 2026-08-27 | 国产模型优先，按任务类型自动切换模型，支持可视化配置面板 |
| 1654 | [xswt442-cmd/dsh-ballast](https://github.com/xswt442-cmd/dsh-ballast) | 0 | 2026-08-31 | 2026-09-02 | DSH 上下文窗口逐条归因面板——看谁占了窗口 \| Per-message context window attribution for DSH — see what takes up the window |
| 1655 | [xswt442-cmd/dsh-mini-utility-dock](https://github.com/xswt442-cmd/dsh-mini-utility-dock) | 0 | 2026-09-02 | 2026-09-02 | 一个简单的 DSH 工具坞 \| A simple utility dock for DSH |
| 1656 | [xswt442-cmd/dsh-treekeeper](https://github.com/xswt442-cmd/dsh-treekeeper) | 0 | 2026-08-27 | 2026-08-27 | 对账 DSH 任务账本与 OS 进程树，定位归属、检测泄漏并安全治理｜Reconcile DSH task ledgers with OS process trees for attribution, leak detection, and safe governance. |
| 1657 | [XY1998-debug/dsh-zhinet](https://github.com/XY1998-debug/dsh-zhinet) | 0 | 2026-09-01 | 2026-09-01 | 许愿式编程的项目事实图、只读工作台、角色协作与跨 DSH 迁移 |
| 1658 | [xyingsoft/dsh-chat](https://github.com/xyingsoft/dsh-chat) | 0 | 2026-08-29 | 2026-08-29 | dsh-chat 设计文档：面向自建团队、受管团队与企业组织的 DSH Web 协作平台 |
| 1659 | [Xylocarpro/dsh-plugin-recycle-bin](https://github.com/Xylocarpro/dsh-plugin-recycle-bin) | 0 | 2026-08-29 | 2026-08-30 | 强制 DSH 删除走回收站、禁用 del/rm/Remove-Item，回收站或硬盘满时停手询问用户。 |
| 1660 | [Ya-MiC/zhanzhen](https://github.com/Ya-MiC/zhanzhen) | 0 | 2026-08-24 | 2026-08-27 | 湛箴 — 中小企业审计风险平台 v1 框架（FastAPI + Vue3，规则引擎本地运行，证据哈希链） |
| 1661 | [yahoolcj/dsh-plugin-zerone](https://github.com/yahoolcj/dsh-plugin-zerone) | 0 | 2026-09-01 | 2026-09-01 | dsh-plugin-zerone |
| 1662 | [yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix](https://github.com/yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix) | 0 | 2026-08-27 | 2026-08-27 | 修复 sandbox_permissions 和 justification 字段在 pwsh/bash/fs/dsh-sandbox 中的 no-op 升级报错。当会话已是 danger-full-access 模式时，模型携带空 justification 或重申同一模式被拒的问题。 |
| 1663 | [yakoylp/dsh-localnotify](https://github.com/yakoylp/dsh-localnotify) | 0 | 2026-09-01 | 2026-09-02 | DSH 本地通知栏插件：侧边栏【通知】入口 + 全屏通知中心（时间筛选/搜索/未读已读/删除/详情一键复制），notify_add agent 工具 + CLI 写入，JSON 持久化，实时刷新，界面跟随 dsh web 语言切换。Local notification center for DeepSeek Harness: notify_add agent tool & CLI, live refresh, i18n. |
| 1664 | [yangdongzhen590/dsh-knj-extension-center](https://github.com/yangdongzhen590/dsh-knj-extension-center) | 0 | 2026-08-31 | 2026-08-31 | DSH ????:????????? zip ?????/??/?????????DSH skill center: browse by region, install from zip, manage enable/disable, uninstall, trash restore, search. |
| 1665 | [yangdongzhen590/dsh-knj-obsidian](https://github.com/yangdongzhen590/dsh-knj-obsidian) | 0 | 2026-08-28 | 2026-08-28 | DSH ??? Obsidian:AI agent ?????????????UI ?????(v1-v7) |
| 1666 | [yangdongzhen590/dsh-knj-prompts](https://github.com/yangdongzhen590/dsh-knj-prompts) | 0 | 2026-08-31 | 2026-08-31 | DSH ???????:????? ? ????????????(?? {??}),???????Prompt-scenario picker for DeepSeek Harness. |
| 1667 | [yangdongzhen590/dsh-knj-session-management](https://github.com/yangdongzhen590/dsh-knj-session-management) | 0 | 2026-08-31 | 2026-08-31 | Session management for DeepSeek Harness: archive/restore/delete persisted sessions, per-workspace retention policy and a size governance panel. DSH ??????:??/??/???????,????????????,????????? |
| 1668 | [yangzhe1991/dsh-futu-mcp](https://github.com/yangzhe1991/dsh-futu-mcp) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin: connect to Futu (富途) MCP via OAuth 2.1 with deferred authorization; tokens stored securely outside the workspace (~/.dsh, 0600) |
| 1669 | [yanqd0/dsh-covtrim](https://github.com/yanqd0/dsh-covtrim) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: one-shot test coverage flow — run tests with coverage, compress with covtrim, return compact TSV to the agent |
| 1670 | [yanqd0/dsh-mint](https://github.com/yanqd0/dsh-mint) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: mint issue tracking integration — session context injection, event reminders, plan binding, mint_query tool, and a session tab |
| 1671 | [yaodongH/dsh-vscode-bridge](https://github.com/yaodongH/dsh-vscode-bridge) | 0 | 2026-08-30 | 2026-08-30 | DSH web 插件：在 DeepSeek Harness 中心区嵌入固定版本 code-server（VS Code Web），跟随当前工作空间，支持自定义端口/路径与热切换。 |
| 1672 | [yaotongsb/dsh-phosphor](https://github.com/yaotongsb/dsh-phosphor) | 0 | 2026-08-29 | 2026-08-29 | A full-screen, Matrix-styled TUI frontend for DeepSeek Harness — built with React + Ink as a Cordis bundle plugin |
| 1673 | [yhPrime/dsh-github-installer](https://github.com/yhPrime/dsh-github-installer) | 0 | 2026-08-29 | 2026-08-29 | GitHub 仓库一键安装插件：粘贴任意 GitHub 插件仓库网址即可安装（标准 dsh plugin add github:… 协议，同 dsh-market）。Install any DeepSeek Harness plugin from a GitHub repo URL. |
| 1674 | [Yidien/dsh-host-router](https://github.com/Yidien/dsh-host-router) | 0 | 2026-08-29 | 2026-08-29 | dsh 外挂式网络路由插件:按域名勾选走本地代理(Clash 等),其余直连;内置嗅探,设置页勾选即生效。 |
| 1675 | [yin52133/dsh-luban](https://github.com/yin52133/dsh-luban) | 0 | 2026-08-29 | 2026-09-01 | 🛠️ Custom workbench plugin suite for DeepSeek Harness (DSH) — LAN auth, task board, SSH + tmux keep-alive, shared Windows/Ubuntu sessions, context HUD & serial/debug tooling. Built for embedded devs: Windows debug box + LAN Ubuntu build server. Monorepo of dsh-luban-* plugins. |
| 1676 | [Yinxe/dsh-mcwiki-search](https://github.com/Yinxe/dsh-mcwiki-search) | 0 | 2026-08-29 | 2026-09-02 | MCBE WIKI 搜索工具 |
| 1677 | [Yinxe/dsh-tavily-search](https://github.com/Yinxe/dsh-tavily-search) | 0 | 2026-09-01 | 2026-09-02 | Tavily AI search provider for DeepSeek Harness |
| 1678 | [Yiyang0659/dsh-git-sync](https://github.com/Yiyang0659/dsh-git-sync) | 0 | 2026-09-02 | 2026-09-02 | Git Config Sync Center for DeepSeek Harness — real-time config sync to GitHub with conflict self-healing and multi AI-tool adapters (OpenCode/Cline/Roo Code/Kilo Code/Continue/goose/Agent Zero) |
| 1679 | [yonglun/deepseek-harness-themes](https://github.com/yonglun/deepseek-harness-themes) | 0 | 2026-08-27 | 2026-08-28 | 74 non-invasive DeepSeek Harness themes generated from awesome-design-md |
| 1680 | [yongshuai0314/dsh-turnsnap](https://github.com/yongshuai0314/dsh-turnsnap) | 0 | 2026-08-27 | 2026-08-27 | Zero-config per-turn git checkpoints for DeepSeek Harness: every completed agent turn in a git workspace becomes one tagged [turnsnap] commit |
| 1681 | [yoshino-xiao7/dsh-codex](https://github.com/yoshino-xiao7/dsh-codex) | 0 | 2026-08-28 | 2026-08-29 | 社区维护的 DeepSeek Harness Codex 插件：OAuth、模型、图片与流式恢复；非官方 / Community Codex plugin for DSH: OAuth, models, images, stream recovery; unofficial. |
| 1682 | [youridol/dsh-launcher](https://github.com/youridol/dsh-launcher) | 0 | 2026-09-01 | 2026-09-02 | deepseek-harness 启动器与运行环境管理器（Tauri 2 + Rust + React） |
| 1683 | [youridol/dsh-plugin](https://github.com/youridol/dsh-plugin) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件收录总库：收录遵循 Cordis 框架、经官方 profile 机制挂载的 DSH 插件。收录插件自动同步上游，自研插件可手动维护。 |
| 1684 | [ytmaps/dsh-subagent-flowtext](https://github.com/ytmaps/dsh-subagent-flowtext) | 0 | 2026-09-01 | 2026-09-01 | 鱼先生模块化OB |
| 1685 | [Yu-Zhuang1/dsh-workspace-snapshot-fork](https://github.com/Yu-Zhuang1/dsh-workspace-snapshot-fork) | 0 | 2026-08-31 | 2026-08-31 | Fork DeepSeek Harness sessions together with their historical workspace state. |
| 1686 | [YUANMINGXUE/dsh-search](https://github.com/YUANMINGXUE/dsh-search) | 0 | 2026-08-26 | 2026-08-27 | Local-browser web search & page fetch plugin for DeepSeek Harness (dsh): browser_search / browser_fetch over Chrome DevTools Protocol, no API key. |
| 1687 | [YUEYUEXYS/dsh-think-ultra](https://github.com/YUEYUEXYS/dsh-think-ultra) | 0 | 2026-08-30 | 2026-08-30 | Reasoning layer for the official DeepSeek Harness: every request stays on native max effort, with isolated Flash/Vision/Pro depth controls, stability axes and reasoning toolboxes built above it. Delivered build only; commercial use open, reverse/modify/extract closed. |
| 1688 | [YuiKiZJ2026/dsh-slot-homestead](https://github.com/YuiKiZJ2026/dsh-slot-homestead) | 0 | 2026-09-02 | 2026-09-02 | 老虎机庄园｜A pixel-art desktop ecosystem for DSH with time-based fish, crop and animal growth, day/night ambience and collectible slot rewards. |
| 1689 | [yunxiiQwQ/drool-whale-pet-for-dsh](https://github.com/yunxiiQwQ/drool-whale-pet-for-dsh) | 0 | 2026-08-27 | 2026-08-27 | 适用于dsh的pet插件 |
| 1690 | [yunxiyang/dsh-web-search-litellm](https://github.com/yunxiyang/dsh-web-search-litellm) | 0 | 2026-08-31 | 2026-08-31 | Web search provider for the DeepSeek Harness ctx.web seam via the LiteLLM proxy OpenAI Responses API (DeepSeek native server-side web_search) |
| 1691 | [Yurzi/dsh-web-fetch-enhanced](https://github.com/Yurzi/dsh-web-fetch-enhanced) | 0 | 2026-08-28 | 2026-08-28 | Configurable non-public address allowlists for DeepSeek Harness web_fetch |
| 1692 | [Yurzi/dsh-web-search-enhanced](https://github.com/Yurzi/dsh-web-search-enhanced) | 0 | 2026-08-29 | 2026-08-29 | Multi-protocol web_search provider for DeepSeek Harness |
| 1693 | [yushenghai1106/dsh-memory-plugin](https://github.com/yushenghai1106/dsh-memory-plugin) | 0 | 2026-09-02 | 2026-09-02 | Pluggable persistent memory bundle for DeepSeek Harness |
| 1694 | [yustillrain/dsh-plugin-tool-repository](https://github.com/yustillrain/dsh-plugin-tool-repository) | 0 | 2026-08-26 | 2026-08-27 | DSH 插件仓库 第三方插件 让你可视化管理已安装的 skill/插件 对skill/插件功能进行介绍和分类  |
| 1695 | [yx-yinhe/dsh-message-navigator](https://github.com/yx-yinhe/dsh-message-navigator) | 0 | 2026-08-27 | 2026-08-27 | ChatGPT-style message navigator for DeepSeek Harness conversations with hover previews and smooth jump navigation. |
| 1696 | [Yyyyyylor/dsh-asuka-school-theme](https://github.com/Yyyyyylor/dsh-asuka-school-theme) | 0 | 2026-08-25 | 2026-08-27 | Theme-Asuka — An unofficial Asuka-inspired theme plugin for DeepSeek Harness Web UI, featuring time-of-day wallpapers, adaptive palette transitions, and restrained EVA-02 visual details. |
| 1697 | [z7ping/narratica](https://github.com/z7ping/narratica) | 0 | 2026-08-28 | 2026-08-28 | AI 原生故事创作与媒体生产工作区｜AI-native storytelling workspace for novels, screenplays, and media production. |
| 1698 | [zaizaizhao/dsh-branchmark](https://github.com/zaizaizhao/dsh-branchmark) | 0 | 2026-08-30 | 2026-09-02 | 为开发者提供重点知识摘录、可追溯 Session 树和注意力分叉，让主 Session 始终专注于当前目标，让每条支线都能找回来源，让 Vibe Coding 告别注意力丢失。 |
| 1699 | [Zayzz-pixel/dsh-ariadne](https://github.com/Zayzz-pixel/dsh-ariadne) | 0 | 2026-09-01 | 2026-09-01 | A visual decision workbench for DeepSeek Harness: explore ideas, focus branches, and turn choices into executable graphs. |
| 1700 | [zdjmrq/dsh-chat-mode](https://github.com/zdjmrq/dsh-chat-mode) | 0 | 2026-08-26 | 2026-08-27 | DSH 插件：为 DeepSeek Harness 增加「对话」纯聊天模式（ChatGPT 式）——侧边栏新会话模式切换（DSH/对话）、对话会话仅提问+搜索工具、专属 \/chat 聊天工作区 |
| 1701 | [zengweicheng666/dsh-svn-tools](https://github.com/zengweicheng666/dsh-svn-tools) | 0 | 2026-08-29 | 2026-08-29 | SVN (Subversion) tools + sidebar UI for DeepSeek Harness: 33 agent tools with UTF-8 Chinese commit logs, plus an SVN panel in dsh-better-sidebar. |
| 1702 | [Zessi-C/biofigure-self-evolve](https://github.com/Zessi-C/biofigure-self-evolve) | 0 | 2026-08-29 | 2026-08-30 | Self-evolving bioinformatics figure library skill: learn plots from papers/PDFs/WeChat articles/screenshots into reusable recipes (R/Python), imitate them when plotting. 自进化的生信 figure 学习库与复用引擎 |
| 1703 | [zhang-jiazhi/dsh-prompt-optimizer](https://github.com/zhang-jiazhi/dsh-prompt-optimizer) | 0 | 2026-08-30 | 2026-08-30 | 将原作者 linshenkx 的 prompt-optimizer 移植到 DeepSeek Harness 的第三方插件（非官方） |
| 1704 | [zhangguiping-xydt/dsh-possibility-space](https://github.com/zhangguiping-xydt/dsh-possibility-space) | 0 | 2026-08-31 | 2026-08-31 | Explore AI outputs as a steerable semantic possibility space for DeepSeek Harness. |
| 1705 | [zhangguiping-xydt/dsh-session-lab](https://github.com/zhangguiping-xydt/dsh-session-lab) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness session teaching, evidence capsules, and controlled trajectory comparison |
| 1706 | [zhangguiping-xydt/dsh-skin-studio](https://github.com/zhangguiping-xydt/dsh-skin-studio) | 0 | 2026-09-01 | 2026-09-01 | A visual, local-first skin authoring studio for DeepSeek Harness Web. |
| 1707 | [zhangkkkai/dsh-getman-panel](https://github.com/zhangkkkai/dsh-getman-panel) | 0 | 2026-08-28 | 2026-08-31 | API 测试侧边栏面板（Getman），作为 dsh-better-sidebar 的配套插件：  请求编辑：方法（GET/POST/PUT/PATCH/DELETE/HEAD/OPTIONS）+ URL + Params / Headers / Body 响应查看：状态码徽章、耗时、大小、响应体（JSON 自动美化，右上角可一键复制）/ 响应头 历史记录：全局共享最近 100 条请求（所有工作空间共用），点击回填、单项删除、一键清空 绕过 CORS：通过 host 半代理转发，任意 HTTP(S) 接口都能测试 |
| 1708 | [zhangkkkai/dsh-spec-panel](https://github.com/zhangkkkai/dsh-spec-panel) | 0 | 2026-08-28 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 SDD（规范驱动开发，Spec-Driven Development）配套插件：在侧边栏提供一个 Spec 工作台，围绕 OpenSpec 的标准目录结构，让「先写规范 → 再实现 → 再验证」的流程一目了然、可操作。 |
| 1709 | [zhangkkkai/dsh-todo-panel](https://github.com/zhangkkkai/dsh-todo-panel) | 0 | 2026-08-27 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 TODO 任务清单侧边栏插件：卡片式布局、优先级颜色标记、中文界面、按会话持久化。 |
| 1710 | [zhangliang0115/ai-plugin](https://github.com/zhangliang0115/ai-plugin) | 0 | 2026-08-29 | 2026-08-29 | One command to install any AI agent skill/plugin into every agent — Claude Code, DeepSeek Harness (dsh), Codex, Gemini CLI, Copilot, Cursor. Zero-dependency CLI + cross-agent marketplace. |
| 1711 | [zhangxingong/dsh-polish](https://github.com/zhangxingong/dsh-polish) | 0 | 2026-09-01 | 2026-09-02 | 需要你做的 UI 验收（重启后逐项过一遍）  1. 书本图标右侧出现四角星按钮：细线空心、四角顶点小圆点、浅灰，与相邻按钮同尺寸，深色主题正常 2. 悬浮显示「优化并细化当前用户输入」 3. 权限下拉切 Read Only → 按钮置灰；切回恢复 4. 空输入点击 → Toast「请先输入内容再进行优化细化」 5. 有文本点击 → loading 旋转 → 全文覆盖（非追加）→ 光标在末尾可直接续写 6. 优化质量抽查：保留原意、逻辑通顺、无废话、语气一致、无解释性前后缀 7. 机器回复运行中按钮置灰；+新增/Read Only/书本图标/发送等原功能无回归 |
| 1712 | [zhangzhenwen1/dsh-task-effort](https://github.com/zhangzhenwen1/dsh-task-effort) | 0 | 2026-08-30 | 2026-08-30 | Auto-adjust model reasoning effort per task with DeepSeek peak-pricing-period capping: off/low/high/max classification, [effort=...] markers, error escalation, countdown notices |
| 1713 | [zhaozixi/dsh-attention](https://github.com/zhaozixi/dsh-attention) | 0 | 2026-08-28 | 2026-08-30 | DSH 跑任务时你通常只能盯着进度条。dsh-attention 把这段等待变成有产出的碎片时间 |
| 1714 | [zhchxiao123/dsh-devflow-plugins](https://github.com/zhchxiao123/dsh-devflow-plugins) | 0 | 2026-08-26 | 2026-08-30 | File-backed development workflow for DeepSeek Harness: durable cards, artifact and agent checks, human approvals, and a read-only web board. |
| 1715 | [zhengjy01/dsh-cloudflare-mcp](https://github.com/zhengjy01/dsh-cloudflare-mcp) | 0 | 2026-08-31 | 2026-08-31 | Cloudflare MCP connection for DeepSeek Harness |
| 1716 | [zhengjy01/dsh-qqbot-panel](https://github.com/zhengjy01/dsh-qqbot-panel) | 0 | 2026-08-31 | 2026-08-31 | Visual web settings panel for the official @tencent-connect/dsh-qqbot plugin: manage AppID/AppSecret, c2c & group access/allowlists, workspace picker, and scan-to-bind from the DSH web settings page |
| 1717 | [zhengjy01/dsh-vercel-mcp](https://github.com/zhengjy01/dsh-vercel-mcp) | 0 | 2026-08-30 | 2026-08-30 | Vercel MCP connection for DeepSeek Harness (DSH): official OAuth 2.0 flow (dynamic client registration + PKCE) against mcp.vercel.com, Vercel API tools under mcp__vercel__*, and a web settings panel |
| 1718 | [zhibailu/dsh-vsc](https://github.com/zhibailu/dsh-vsc) | 0 | 2026-08-23 | 2026-08-31 | Run DeepSeek Harness (DSH), a local AI agent, inside VS Code — native sidebar panel + editor bridge. A pure protocol client: no rewriting DSH, no second server |
| 1719 | [zhm20001/dsh-plugin-palette-board](https://github.com/zhm20001/dsh-plugin-palette-board) | 0 | 2026-08-31 | 2026-08-31 | 本项目为 DeepSeek Harness web 控制台带来一块 2D 调色盘应用板。唤出悬浮面板，即时搜索、分类过滤、全键盘导航，把散落在侧栏与浏览器里的插件页面收进一张可自定义的卡片网格。   |
| 1720 | [zhm20001/dsh-usage-board](https://github.com/zhm20001/dsh-usage-board) | 0 | 2026-08-27 | 2026-08-28 | dsh-usage-board 是专为 DSH (DeepSeek Harness) 设计的用量与成本可视化看板插件。  插件能实时捕获会话内的 Token 消耗、Step 耗时和异常指标，支持冷启动增量回溯历史全量会话，并按 Sub-agent DAG 调用关系进行树状归集与反向明细穿透。 |
| 1721 | [zhoujianbin/dsh-codex-continue](https://github.com/zhoujianbin/dsh-codex-continue) | 0 | 2026-08-29 | 2026-08-30 | DSH 插件：读取本机 Codex 项目与会话，一键在 DSH 里继续。Read local OpenAI Codex sessions and continue them in DeepSeek Harness. |
| 1722 | [zhubaohi/dsh-gpu-pulse](https://github.com/zhubaohi/dsh-gpu-pulse) | 0 | 2026-08-30 | 2026-08-30 | Floating GPU monitor (nvidia-smi) for the DSH Web UI — live per-GPU utilization, VRAM, temperature, power and fan, in the corner of the page. |
| 1723 | [ZhuYanTech/dsh-biomni](https://github.com/ZhuYanTech/dsh-biomni) | 0 | 2026-08-15 | 2026-08-31 | DeepSeek Harness biomni plugin |
| 1724 | [ZiFan1117/bazidiy](https://github.com/ZiFan1117/bazidiy) | 0 | 2026-08-26 | 2026-08-27 | 基于 DeepSeek Harness 的八字五行手串定制插件 |
| 1725 | [zisen123/dsh-reasoning-ruler](https://github.com/zisen123/dsh-reasoning-ruler) | 0 | 2026-08-30 | 2026-08-30 | Minimal reasoning-effort ruler for the DSH web composer: hairline + sliding marker, per-model memory, optimistic switching, streamlined model picker |
| 1726 | [ZK-Andy/dsh-frecency](https://github.com/ZK-Andy/dsh-frecency) | 0 | 2026-09-01 | 2026-09-02 | Resident-index + frecency file search for DeepSeek Harness — shadows the built-in grep/glob tools · DSH 常驻索引 + frecency 文件搜索，同名覆盖内置 grep/glob |
| 1727 | [zouxiaoyang/dsh-commandcode-usage](https://github.com/zouxiaoyang/dsh-commandcode-usage) | 0 | 2026-08-31 | 2026-08-31 | CommandCode usage & balance panel for DeepSeek Harness / DSH 的 CommandCode 用量与余额面板 |
| 1728 | [zpliao123/dsh-ark-quota](https://github.com/zpliao123/dsh-ark-quota) | 0 | 2026-08-27 | 2026-08-27 | Volcengine Ark Coding Plan / Agent Plan quota plugin for DeepSeek Harness (DSH) Web GUI: side float widget + settings page, persistent credentials, periodic auto-refresh, ark_coding_plan_usage model tool. |
| 1729 | [zptalk0221-cpu/dsh-remote-desktop](https://github.com/zptalk0221-cpu/dsh-remote-desktop) | 0 | 2026-08-26 | 2026-08-27 | 远程桌面移动化插件：为 DeepSeek Harness 提供手机横屏外壳与中文输入法 |
| 1730 | [zuohaisu/dsh-ai-soul](https://github.com/zuohaisu/dsh-ai-soul) | 0 | 2026-08-26 | 2026-09-01 | Persistent identity layer for DeepSeek Harness. The first reference implementation of AI Soul. |
| 1731 | [zuojinxin/dsh-provider-switch](https://github.com/zuojinxin/dsh-provider-switch) | 0 | 2026-08-28 | 2026-08-28 | Provider on/off switches, model search, and inline provider renaming for DeepSeek Harness. |
| 1732 | [zxheyi/dsh-work](https://github.com/zxheyi/dsh-work) | 0 | 2026-08-27 | 2026-08-27 | A plugin-native AI desktop for real work, built on DeepSeek Harness. |
| 1733 | [zzhi191/dsh-plugin-night-dog](https://github.com/zzhi191/dsh-plugin-night-dog) | 0 | 2026-08-29 | 2026-08-29 | A tan DeepSeek mascot dog named 夜官 that lives in the corner of the DSH web GUI: floats, reacts to the harness, adapts to the theme, and acts out a full repertoire (pant, stand, walk, tilt, yawn, bark, spin, whimper, lie down to sleep). Pure client plugin, installable from the DSH Community Market. |

## 从快照消失的已核准仓库 / Approved repositories missing from the snapshot

已核准但已不在当前快照中（删除或改名），核实后从 [data/approved.json](../approved.json) 移除或更新名称。

Approved but no longer present in the current snapshot (deleted or renamed) — after checking, remove them from [data/approved.json](../approved.json) or update the name.

- 0x5446/reins
- 1lyygit/dsh-launcher
- 240xu/tech-lead-skill
- ABccgh/dsh-agent-studio
- ABccgh/dsh-github-plugin-tools
- ABccgh/dsh-ima-plugin
- ABccgh/dsh-plugin-dev
- ABccgh/imakb
- ABccgh/ws-cleaner
- alaxrpg/dsh-adaptive-model-router
- alfonsoferrertorres-cyber/saare-suite
- Arslan-jh/deepseek-harness-usage
- Bacskat/dsh-claude-ui
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
- dat-lequoc/dsh-shots
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
- Gaq152/dsh-attention
- Gaq152/dsh-credits
- ggggggggggz/dsh-config
- GM-HZ/dsh-dag-workflow
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
- jiuge2467/DSH-WhaleDeck
- Jstn-1g/dsh-guarded-live-voice
- JUSTMONIKA2022/dsh-sandbox-escalation-fix
- KeS1Ke/dsh-exit
- kiligzzz/dsh-capability-manager
- krystal-cao/deepseek-harness-desktop
- krystal-cao/deepseek-harness-swift
- lamost423/dsh-trace-compare
- lhf6623/dsh-vibe
- liguobao/deepseek-harness-remote
- lmh-2026/dsh-periscope
- looput/dsn-finance-lab
- lovaxi/4d4y-browser
- lovstudio/dsh-plugin-creator-skill
- lovstudio/dsh-plugin-publisher-skill
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
- wezoo-wb/dsh-desktop-min
- WSL043/dsh-native-deepseek-balance
- WSL043/dsh-native-reasoning-slider
- WSL043/dsh-native-session-manager
- xiaoliang2/dsh-compact-after-task
- xie-tj/dsh-easy-exit
- xmutfyh/dsh-plugin-writing-guard
- XSakura666/ChronoAgent
- xuzhougeng/dsh-wisp-science-lab
- yhfgyyf/dsh-guardian-mode
- youridol/dsh-sess
- yustillrain/dsh-skill-browser
- Yvesgao/dsh-desktop-launcher
- Zh1rV/dsh-web-search-tavily
- zhaimingyou/aisync
- zhangyoufu-123/stylotrace
- zhongjie10086/dsh-adaptive-native-standard
