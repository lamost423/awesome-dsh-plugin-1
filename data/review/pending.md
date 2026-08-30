# 待审核仓库 / Pending review

> 新增到 `dsh-plugin` Topic 下、带有简介、尚未经维护者核实的仓库。本文件由 `scripts/update.mjs` 每日刷新，仅供审核使用，不是用户可见页面。
>
> Repositories newly added to the `dsh-plugin` topic that the maintainer has not verified yet. Refreshed daily by `scripts/update.mjs`; review-only, not a user-facing page.

- 生成时间 / Generated: **2026-08-30**
- 快照日期 / Snapshot date: **2026-08-30 (UTC)**
- 待审核 / Pending: **1035**
- 从快照消失的已核准仓库 / Approved repositories missing from the snapshot: **368**

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
| 1 | [chuspeeism/dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) | 2794 | 2026-07-24 | 2026-08-29 | 现代化可灵活嵌入的任务面板，支持 Codex、DeepSeek Harness |
| 2 | [AdamPlatin123/dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1432 | 2026-08-04 | 2026-08-28 | DSH Plugin Radar — 开源 DSH 插件生态雷达：自动发现 15900+ 候选、k8s 运行级实测 10000+、15 分钟快照管线；插件目录是其自动生成的 artifact |
| 3 | [Unclecheng-li/AI_Animation](https://github.com/Unclecheng-li/AI_Animation) | 1190 | 2026-04-11 | 2026-08-29 | 本项目整理了用于生成[炫酷 HTML 动画网页]的 AI Prompts，涵盖动画效果、3D 可视化、PPT 风格演示、UI 美化等多个类别。 |
| 4 | [platonai/Browser4](https://github.com/platonai/Browser4) | 1114 | 2018-03-12 | 2026-08-27 | Browser4 — an AI-native browser engine for autonomous agents, intelligent extraction, and large-scale web automation. |
| 5 | [wecode-ai/Wegent](https://github.com/wecode-ai/Wegent) | 747 | 2026-01-10 | 2026-08-30 | Plan, build, and deliver with an open-source, self-hostable AI workspace for coding, collaboration, and automation. |
| 6 | [myYangyunfan/dsh_desktop](https://github.com/myYangyunfan/dsh_desktop) | 610 | 2026-08-13 | 2026-08-30 | DeepSeek Harness (dsh) Windows desktop client - bundled Node.js + dsh CLI, one-click launch |
| 7 | [liguobao/ds-harness-remote](https://github.com/liguobao/ds-harness-remote) | 133 | 2026-08-14 | 2026-08-30 | 一个基于 DeepSeek Harness 插件机制构建的多端远程访问方案，通过安全、低延迟、端到端加密的 P2P 优先网络，支持从 PC、Android 和 Web 随时访问并操作远程 Harness。 (A multi-device remote access solution built on the DeepSeek Harness plugin system, enabling PC, Android, and Web clients to securely access and operate a remote Harness over a low-latency, end-to-end encrypted, P2P-first network.) |
| 8 | [theBigGavin/marketingdashboard](https://github.com/theBigGavin/marketingdashboard) | 126 | 2026-07-17 | 2026-08-30 | 面向金融与产业研究的一屏式实时行情大屏：A股/港股/美股指数、大宗商品、美债收益率、板块热点、主力资金流、7×24 快讯、产业链自选股、AI 大模型 Token 追踪。A real-time market research cockpit on a single screen: CN/HK/US indices, commodities, treasury yields, sector hotspots, capital flows, 7×24 news, industry-chain watchlists and AI token usage trends.  |
| 9 | [Jackywxsz/DSH-Creator](https://github.com/Jackywxsz/DSH-Creator) | 59 | 2026-08-25 | 2026-08-27 | Jacky Creator：面向内容创作者的 DeepSeek Harness 本地内容与运营工作台 |
| 10 | [lamost423/dsh-maze](https://github.com/lamost423/dsh-maze) | 59 | 2026-08-18 | 2026-08-27 | DeepSeek Harness 的执行迷宫——看 Agent 真实怎么干活：迷宫时间轴 · 数据轨道 · 确定性执行分析 · 多会话对比 \| The execution maze for DSH agents: maze timeline, per-step data tracks, deterministic execution analysis, multi-session comparison. Formerly dsh-trace-compare. |
| 11 | [HakureiMonika/dsh-sandbox-escalation-fix](https://github.com/HakureiMonika/dsh-sandbox-escalation-fix) | 35 | 2026-08-16 | 2026-08-28 | Session-aware sandbox escalation compatibility plugin for DeepSeek Harness/DSH第三方模型会话沙箱升级兼容插件 |
| 12 | [FrankHu-HK/mnemosyne](https://github.com/FrankHu-HK/mnemosyne) | 24 | 2026-08-10 | 2026-08-27 | Mnemosyne OS 7.0.0 — zero-dependency, local-first AI memory system (MCP / API / CLI / Python). MIT. |
| 13 | [extracurricular-ai/dsh-filesnap](https://github.com/extracurricular-ai/dsh-filesnap) | 19 | 2026-08-27 | 2026-08-27 | dsh-filesnap — 把对话和它改过的文件一起回退到某一轮之前,不需要 git 仓库. A blazing-fast rewind and redo plugin for DeepSeek Harness, powered by a 🦀 Rust core, tracking the conversion and the files it changed, no git required, low disk consumption |
| 14 | [chumingjun/dsh-harness-one](https://github.com/chumingjun/dsh-harness-one) | 17 | 2026-08-20 | 2026-08-27 | Visual AI workflow orchestrator for DeepSeek Harness (dsh): multi-agent DAGs, live execution, recovery, and Feishu integration. |
| 15 | [Ed-Marcavage/awesome-security-agent-harnesses](https://github.com/Ed-Marcavage/awesome-security-agent-harnesses) | 16 | 2026-08-03 | 2026-08-30 | AI agents for pentesting, code audit, fuzzing, vulnerability discovery, and reverse engineering — harnesses, sandboxes, security MCP servers, benchmarks, and evals. |
| 16 | [Suiwan/whale-purse](https://github.com/Suiwan/whale-purse) | 16 | 2026-08-14 | 2026-08-30 | A cute whale desktop pet for DeepSeek Harness that keeps an eye on your DeepSeek balance and session usage/cost. Drag her anywhere, click to open a live panel with real-time spend, peak/off-peak pricing, budget alerts, and history trends. |
| 17 | [NekroAI/nekro-nxt](https://github.com/NekroAI/nekro-nxt) | 15 | 2026-08-15 | 2026-08-27 | NekroNXT：基于 DeepSeek Harness（DSH）的多平台群聊智能体系统｜A DSH-powered multi-platform group-chat agent system |
| 18 | [ddtcorex/govard](https://github.com/ddtcorex/govard) | 13 | 2026-02-08 | 2026-08-28 | Go-based local development orchestrator for Magento, Laravel, Symfony, Next.js, WordPress, and more. Docker stacks, SSL, Xdebug, and a desktop dashboard. |
| 19 | [tinqiao-oss/clawtouch-mcp](https://github.com/tinqiao-oss/clawtouch-mcp) | 10 | 2026-06-01 | 2026-08-29 | ClawTouch MCP server — exposes a real USB-HID keyboard/mouse (Raspberry Pi Pico 2) as Model Context Protocol tools for any LLM agent. MIT. |
| 20 | [greenthree/ProbHub-skill](https://github.com/greenthree/ProbHub-skill) | 8 | 2026-05-25 | 2026-08-30 | 算法竞赛出题自动化skill（个人出题习惯），支持完善题面、构造数据、组卷用typ编译pdf和生成domjudge题目包 |
| 21 | [keman-ai/dsh-skin-market](https://github.com/keman-ai/dsh-skin-market) | 8 | 2026-08-18 | 2026-08-27 | Skin marketplace for DeepSeek Harness — search and install community skins from dsh.a2hmarket.ai right in the settings page |
| 22 | [LaoYueHanNi/dsh-token-usage](https://github.com/LaoYueHanNi/dsh-token-usage) | 8 | 2026-08-14 | 2026-08-27 | 贴近 DSH 原生设计风格的 token 用量统计插件：实时记录每次请求的用量与费用，在 Web UI 中提供趋势图表、按模型定价明细和供应商配额显示。 |
| 23 | [Ramenne/DeepSeek-Harness-Gov](https://github.com/Ramenne/DeepSeek-Harness-Gov) | 8 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 政务版：基于 deepseek-ai/deepseek-harness 的政务办事 WebUI 与红头公文插件 |
| 24 | [AngelosZou/graphlint](https://github.com/AngelosZou/graphlint) | 7 | 2026-07-01 | 2026-08-27 | Dead-code detection for AI-generated codebases: graphlint builds a dependency graph, finds code unreachable from any entry point to enable codebase cleanup and functional‑effectiveness understanding. |
| 25 | [fangqian616/consensus-pipeline](https://github.com/fangqian616/consensus-pipeline) | 7 | 2026-07-16 | 2026-08-30 | Multi-agent department framework for long-form complex tasks, fighting AI hallucination, validated on academic research. 共识管线：多智能体部门长线任务解决框架，对抗AI幻觉，以学术研究为验证场景。 |
| 26 | [imsai-sh/dsh-1024store](https://github.com/imsai-sh/dsh-1024store) | 7 | 2026-08-24 | 2026-08-27 | DeepSeek Harness plugin store, marketplace and hub — 11,000+ dsh plugins with search, rankings, install commands and a free public API. DeepSeek Harness 插件市场 / 插件商店：自动收集与格式校验，免费搜索 API。deepseek1024.com |
| 27 | [RiemannRe3/DSH-RolePlay](https://github.com/RiemannRe3/DSH-RolePlay) | 7 | 2026-08-25 | 2026-08-27 | DeepSeek Harness 的 Tavern 角色卡兼容与原生 Agent RolePlay 插件。 |
| 28 | [chen731215-dev/dsh-tavern-v2](https://github.com/chen731215-dev/dsh-tavern-v2) | 6 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Tavern Plugin - character card roleplay, worldbook management, preset switching, dark theme, memory summary, relationship graph, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 29 | [fb0sh/dsh-pentester](https://github.com/fb0sh/dsh-pentester) | 6 | 2026-08-19 | 2026-08-29 | 基于 DeepSeek Harness 的多 Agent PTES 渗透测试编排插件，支持自动化侦察、漏洞分析、验证与报告，使用 Docker/Kali 隔离工具箱 \| Multi-agent PTES penetration testing plugin for DeepSeek Harness with automated recon, vulnerability analysis, validation, reporting, and Docker/Kali toolbox |
| 30 | [liceses/dsh-workspace-tree](https://github.com/liceses/dsh-workspace-tree) | 6 | 2026-08-18 | 2026-08-30 | 把 DSH Web 左侧栏的「工作区」重做为文件系统树双模式。核心原则： 工作区 = 目录强绑定——会话的 cwd 就是它所在的目录，环境真正隔离。 |
| 31 | [awesome-deepseekharness/awesome-deepseek-harness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness) | 5 | 2026-08-15 | 2026-08-27 | Awesome DeepSeek Harness (dsh) — curated awesome list of plugins, tools, skills & resources. Everything is a plugin. |
| 32 | [jiazz197-cmyk/omd-dsh](https://github.com/jiazz197-cmyk/omd-dsh) | 5 | 2026-08-23 | 2026-08-29 | Multi-mode agent presets for DeepSeek Harness — per-mode model routing + tiered subagent delegation. |
| 33 | [keman-ai/dsh-skin-pack](https://github.com/keman-ai/dsh-skin-pack) | 5 | 2026-08-26 | 2026-08-27 | A full set of skins for DeepSeek Harness — one repository, each theme installable on its own |
| 34 | [LaoYueHanNi/dsh-git-worktree](https://github.com/LaoYueHanNi/dsh-git-worktree) | 5 | 2026-08-16 | 2026-08-30 | 在 Web 界面进行分支切换与 git worktree 隔离的 DSH 插件 |
| 35 | [ppy-web/dsh-plugin-xiaomi-mimo-tts](https://github.com/ppy-web/dsh-plugin-xiaomi-mimo-tts) | 5 | 2026-08-20 | 2026-08-28 | 给DSH接入免费的 Xiaomi MiMo TTS API，支持使用预置/自定义声音朗读正文 |
| 36 | [recoluan/recowork](https://github.com/recoluan/recowork) | 5 | 2026-07-06 | 2026-08-27 | Give your AI a workflow. |
| 37 | [rogerdigital/dsh-searxng](https://github.com/rogerdigital/dsh-searxng) | 5 | 2026-08-16 | 2026-08-29 | DeepSeek Harness (dsh) plugin that adds a SearXNG-backed web_search provider to the ctx.web seam — free, self-hosted, key-less search instead of paid Exa/Perplexity APIs. |
| 38 | [See-Sol-Lab/DeepSeekGUI](https://github.com/See-Sol-Lab/DeepSeekGUI) | 5 | 2026-08-17 | 2026-08-27 | A Windows desktop client for DeepSeek Harness. V1 wraps the official Web UI; v2 (independent workbench) in development. |
| 39 | [tta-lab/organon](https://github.com/tta-lab/organon) | 5 | 2026-03-18 | 2026-08-30 | Structure-aware tools for AI agents. Tree-sitter code editing, web page navigation, search. No daemon, no JSON, just stdin. |
| 40 | [WSL043/dsh-chat-manager](https://github.com/WSL043/dsh-chat-manager) | 5 | 2026-08-15 | 2026-08-27 | DeepSeek Harness 聊天管理器：搜索归档会话、恢复聊天并安全永久删除。 |
| 41 | [ai-eks/dsh-docking-layout](https://github.com/ai-eks/dsh-docking-layout) | 4 | 2026-08-21 | 2026-08-29 | Organize unlimited conversation tabs into editor-style, drag-to-split groups for DeepSeek Harness Web. |
| 42 | [cloveric/tarocub](https://github.com/cloveric/tarocub) | 4 | 2026-04-08 | 2026-08-29 | Feishu/Lark-first local AI agent gateway and native DeepSeek Harness plugin for Codex, Claude Code, Kimi Code, DeepSeek Harness, and Antigravity; Telegram optional. |
| 43 | [Drhushi/dsh-plugin-tav2](https://github.com/Drhushi/dsh-plugin-tav2) | 4 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 插件 —— 对话式游戏本地化：跟 AI 助手说说话，完成游戏翻译全流程。引擎适配器架构，首发支持 Ren'Py。 |
| 44 | [flymysql/dsh-memory](https://github.com/flymysql/dsh-memory) | 4 | 2026-08-14 | 2026-08-30 | DeepSeek Harness 跨会话记忆库：memory_remember/recall/forget 三个工具 + 系统提示注入，agent 持久化记忆 |
| 45 | [null119/dsh-mcp-manage](https://github.com/null119/dsh-mcp-manage) | 4 | 2026-08-17 | 2026-08-30 | DSH（DeepSeek Harness）Web GUI 插件：在设置页管理 MCP 服务器——列出已安装工具，添加/编辑/删除、启用/停用；组合配置提供的 MCP 同样可在运行时直接编辑、停用、移除并恢复，无需重启宿主。 |
| 46 | [ParticleLight/dsh-all-usage](https://github.com/ParticleLight/dsh-all-usage) | 4 | 2026-08-17 | 2026-08-29 | DeepSeek Harness 用量看板 / Usage dashboard: tokens, cache, model/provider/workspace analytics, DeepSeek balance, heatmap, and CSV export. |
| 47 | [pgmi-builds/better-dsh](https://github.com/pgmi-builds/better-dsh) | 4 | 2026-08-16 | 2026-08-28 | dsh RLM mode (Recursive Language Models), iPython REPL tool-calling interface, context-as-variables, in dsh Everything is a Plugin ecosystem. |
| 48 | [RexCue/dsh-wallpaper](https://github.com/RexCue/dsh-wallpaper) | 4 | 2026-08-14 | 2026-08-30 | Wallpaper skin for the DeepSeek Harness (dsh) web UI: image background with opacity, mask and blur controls. |
| 49 | [xianrui69/dsh-quick-phrases](https://github.com/xianrui69/dsh-quick-phrases) | 4 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: quick-phrase chip bar above the composer + /-triggered phrase menu |
| 50 | [yailPeralta/ast-mcp-server](https://github.com/yailPeralta/ast-mcp-server) | 4 | 2026-08-03 | 2026-08-29 | Correctness-oriented MCP server and batch CLI for compact structural reads and reviewed TypeScript/JavaScript edits. |
| 51 | [yu-wenchao/dsh-free-models-hub](https://github.com/yu-wenchao/dsh-free-models-hub) | 4 | 2026-08-26 | 2026-08-27 | 免费模型排行榜 · DeepSeek Harness 社区插件，在 DeepSeek Harness (DSH) Web UI 左侧边栏提供「免费模型榜」：分页浏览（每页 20 条、页码窗口、首页/末页）、 点击标题展开 API 调用地址 / 模型名称 / 【点击这里申请免费密钥key】按钮， 并支持一键配置到 设置 → 模型 → 自定义提供方 —— 用户只需自行粘贴免费 API Key |
| 52 | [Z-6354/dsh-version-autoupdate](https://github.com/Z-6354/dsh-version-autoupdate) | 4 | 2026-08-18 | 2026-08-28 | DSH version badge + one-click auto-update (dual-surface Cordis plugin) |
| 53 | [AnLifeX/dsh-credits](https://github.com/AnLifeX/dsh-credits) | 3 | 2026-08-17 | 2026-08-29 | DeepSeek Harness（dsh web）额度插件：跟随当前模型显示官方余额或 OpenCode Go 订阅用量，支持本会话估算、跨会话累计消耗与可视化设置。 |
| 54 | [chengdb/dsh-plugin-capability-panel](https://github.com/chengdb/dsh-plugin-capability-panel) | 3 | 2026-08-21 | 2026-08-27 | 在 Web GUI 里可视化管理项目的全部能力——Skills、MCP 服务器、快捷消息， 全部支持项目级 / 全局级双作用域，全部可以不离开浏览器完成安装、启停与分发 |
| 55 | [dushaobindoudou/dsh-freeroute](https://github.com/dushaobindoudou/dsh-freeroute) | 3 | 2026-08-21 | 2026-08-27 | dsh free token route |
| 56 | [Fakek0f3sT/dsh-mcp-diff](https://github.com/Fakek0f3sT/dsh-mcp-diff) | 3 | 2026-08-27 | 2026-08-27 | Uniform diff cards for every file mutation in DeepSeek Harness Web — MCP filesystem (edit_file/write_file) and built-in edit/write, collapsed by default, with per-line highlighting |
| 57 | [GM-HZ/agent-dag-workflow](https://github.com/GM-HZ/agent-dag-workflow) | 3 | 2026-08-23 | 2026-08-29 | Host-neutral durable DAG workflows for Agents: CLI-native access, fixed MCP gateway, on-demand Skills, triggers, replay, and visual Canvas. |
| 58 | [guoxiucai/dsh-code](https://github.com/guoxiucai/dsh-code) | 3 | 2026-08-16 | 2026-08-28 | pi tui  style code agent base on deepseek harness |
| 59 | [gwsbhqt/dsh-insight](https://github.com/gwsbhqt/dsh-insight) | 3 | 2026-08-25 | 2026-08-27 | 洞察 — read-only insight panel for a DeepSeek Harness profile: where every plugin, service, tool and model came from, which config layer inserted or disabled it, and what is running right now. |
| 60 | [jinxlux/xiao-theme-dsh-ui-plugin](https://github.com/jinxlux/xiao-theme-dsh-ui-plugin) | 3 | 2026-08-23 | 2026-08-29 | UI plugin for deepseek harness web |
| 61 | [lw-storm/dsh-plugin-masterprompt](https://github.com/lw-storm/dsh-plugin-masterprompt) | 3 | 2026-08-27 | 2026-08-28 | This plugin is used for custom persona configuration. It facilitates users in code development and customized‑role setup, and supports flexible persona adjustments for each conversation. |
| 62 | [mantonlove/dsh-prism-plugin](https://github.com/mantonlove/dsh-prism-plugin) | 3 | 2026-08-18 | 2026-08-27 | Prism · 棱镜 — a deeply customizable glassmorphism theme plugin for the DeepSeek Harness Web GUI |
| 63 | [QinpanWan/dsh-hiboard-push](https://github.com/QinpanWan/dsh-hiboard-push) | 3 | 2026-08-23 | 2026-08-27 | Push task-completion messages to the Huawei HarmonyOS assistant-today (负一屏) card feed from DeepSeek Harness — wire-compatible with the OpenClaw today-task skill. |
| 64 | [Shaky77/weiwen-law-dsh](https://github.com/Shaky77/weiwen-law-dsh) | 3 | 2026-08-19 | 2026-08-27 | 唯稳律 (Weiwen's Law) 白箱风控 DSH 插件 — DeepSeek Harness 因果约束中间件 |
| 65 | [SuCriss/dsh-leekbox](https://github.com/SuCriss/dsh-leekbox) | 3 | 2026-08-26 | 2026-08-27 | 韭菜盒子 LeekBox — A股看盘助手 · DeepSeek Harness (DSH) web 插件 |
| 66 | [UncleK/dsh-think-translate](https://github.com/UncleK/dsh-think-translate) | 3 | 2026-08-24 | 2026-08-27 | Thinking-chain UI translation for DeepSeek Harness: 8 target languages, local Ollama model primary with in-panel download, Google/Bing fallback |
| 67 | [vibe-any/dsh-plugin-save-token](https://github.com/vibe-any/dsh-plugin-save-token) | 3 | 2026-08-27 | 2026-08-27 | A DeepSeek Harness (dsh) dynamic plugin that cuts token cost without cutting model intelligence |
| 68 | [wkscc310/dsh-client-ui-cpa-quota](https://github.com/wkscc310/dsh-client-ui-cpa-quota) | 3 | 2026-08-17 | 2026-08-30 | Easily view your CLiProxyAPI quota in DeepSeek Harness. |
| 69 | [wycto/dsh-dock](https://github.com/wycto/dsh-dock) | 3 | 2026-08-21 | 2026-08-28 | dsh-dock · DeepSeek Harness 功能中枢：用一张管理面板统一注册、开关所有小功能（模型余额、Token 用量记录、任务动画等）。每个功能独立模块，支持开关与错误隔离，新功能即插即用。0.1.0 为基础框架，功能接入按 README 路线图迭代。 |
| 70 | [x102201/deepseek-harness-helper](https://github.com/x102201/deepseek-harness-helper) | 3 | 2026-08-25 | 2026-08-27 | 🖥️ 一台电脑无限多开 DeepSeek Harness · 🔀 每个实例=独立一套 dsh · 📐 可拖拽自定义分屏 · 📦 .dshpack 环境打包可卖 · 🪟🍎🐧 Win/macOS/Linux（x64 & ARM） |
| 71 | [xiaosurongjia/dsh-improved-inline-edit](https://github.com/xiaosurongjia/dsh-improved-inline-edit) | 3 | 2026-08-28 | 2026-08-29 |  当你的DSH正在工作时，你可以不用停止对话就可以再次提出要求 |
| 72 | [zh851233/docs-mode](https://github.com/zh851233/docs-mode) | 3 | 2026-08-25 | 2026-08-27 | You can use this plugin to complete the writing of technical documents, including development briefs, user manuals, reports/summary materials, and interface/API documentation, while reducing traces of AIGC. |
| 73 | [173787247/dsh-wsl-open](https://github.com/173787247/dsh-wsl-open) | 2 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: open WSL Linux paths from chat in Windows. |
| 74 | [452926826/dsh-at-skill](https://github.com/452926826/dsh-at-skill) | 2 | 2026-08-25 | 2026-08-27 | Invoke DeepSeek Harness skills with @name and composer suggestions |
| 75 | [9931666/dsh-plugin-roundtable](https://github.com/9931666/dsh-plugin-roundtable) | 2 | 2026-08-22 | 2026-08-29 | （roundtable V0.2.2）把一次 DeepSeek Harness 会话，从"你和 AI 一对一聊天"，升级成"你 + 主持人(DeepSeek) + 一圈专家 AI 开圆桌会 |
| 76 | [AnLifeX/dsh-attention](https://github.com/AnLifeX/dsh-attention) | 2 | 2026-08-20 | 2026-08-29 | dsh 提醒插件：别错过需要你的时刻 |
| 77 | [better-er/dsh-edit-diff](https://github.com/better-er/dsh-edit-diff) | 2 | 2026-08-28 | 2026-08-28 | dsh·去重复 diff 展示插件 |
| 78 | [bettermen/xiashuo](https://github.com/bettermen/xiashuo) | 2 | 2026-08-23 | 2026-08-30 | 虾说教材写作 · dsh-course-writer — AI course-authoring workspace plugin for DeepSeek Harness (DSH). 三栏式工作台 · 九阶段门禁 · 课程/章节/资料库/知识图谱 · 导出 TXT/Word · 分享协作。Three-pane workspace, nine-phase gated workflow, lorebook, export & share. |
| 79 | [BlueChonk/dsh-cli-anything](https://github.com/BlueChonk/dsh-cli-anything) | 2 | 2026-08-27 | 2026-08-27 | 将 CLI-Anything 集成到 DSH (DeepSeek Harness) 的插件方案。安装后通过自然语言对话即可浏览、安装、启动和管理 100+ CLI 工具。 |
| 80 | [d86e/dsh-doctor](https://github.com/d86e/dsh-doctor) | 2 | 2026-08-27 | 2026-08-27 | dsh-doctor: self-healing watchdog for the DeepSeek Harness web profile. Recovers from plugin-induced boot failures within 60s, runs an unbounded CLI doctor, captures every tool error, and watches all live sessions for stuck turns. |
| 81 | [delock/dsh-pr-board](https://github.com/delock/dsh-pr-board) | 2 | 2026-08-26 | 2026-08-27 | Maintainer PR review queue board for DeepSeek Harness: five-state tracking (waiting on me / waiting on author / ready to merge / merged / inbox), sidebar counters, fullscreen kanban, polling, and back-to-you transition toasts. |
| 82 | [EL4CTEO/roblox-devforum-mcp](https://github.com/EL4CTEO/roblox-devforum-mcp) | 2 | 2026-03-30 | 2026-08-30 | Give your AI coding agent the Roblox DevForum and official creator docs — check if a bug is already known, read the accepted answer, and verify APIs before writing Luau. |
| 83 | [everclear077/dsh-progressive-tools](https://github.com/everclear077/dsh-progressive-tools) | 2 | 2026-08-24 | 2026-08-27 | Progressive tool discovery for DeepSeek Harness — tiny stable surface, searchable catalog, real pipeline execution, context cache intact. |
| 84 | [FraYoshi/dsh-ui-models-invert-selection](https://github.com/FraYoshi/dsh-ui-models-invert-selection) | 2 | 2026-08-29 | 2026-08-29 | Invert selection in Deepseek Harness for when we are selecting models  |
| 85 | [fufengyuan/dsh-stool-plugin](https://github.com/fufengyuan/dsh-stool-plugin) | 2 | 2026-08-25 | 2026-08-27 | DSH 运维工具箱插件。将 stool 运维 CLI 的全部能力注册为 DSH 模型可调用的工具，无需手动操作即可让 Agent 自动执行服务器管理、日志搜索、数据库查询、CI/CD 部署等操作。 |
| 86 | [gameswu/dsh-human-coding](https://github.com/gameswu/dsh-human-coding) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 增加古法编程模式，让模型监督你写代码！ |
| 87 | [hi-fangj/dsh-models-radar](https://github.com/hi-fangj/dsh-models-radar) | 2 | 2026-08-26 | 2026-08-27 | Model capability radar plugin for the DeepSeek Harness Web GUI |
| 88 | [HiQ-AI/dingtalk-dsh-assistant](https://github.com/HiQ-AI/dingtalk-dsh-assistant) | 2 | 2026-08-25 | 2026-08-29 | 基于 DeepSeek Harness 的钉钉群聊常驻个人助理插件 |
| 89 | [Hou-DL/dsh-token-pulse](https://github.com/Hou-DL/dsh-token-pulse) | 2 | 2026-08-24 | 2026-08-28 | Local Token heatmap plugin for DSH Web — GitHub-style calendar views, per-hour/week/month/quarter/year, fully local, zero billing. |
| 90 | [HuaJi2077/empty-fort-strategy](https://github.com/HuaJi2077/empty-fort-strategy) | 2 | 2026-08-29 | 2026-08-29 | DSH插件，感受空城计的巧妙，消耗多余的Token。 |
| 91 | [huanghai-lab/dsh-custom-instructions](https://github.com/huanghai-lab/dsh-custom-instructions) | 2 | 2026-08-15 | 2026-08-28 | DSH Web 安全自定义指令管理器：编辑全局 AGENTS.md，支持模板、Markdown 预览、历史恢复、导入导出与并发保护。 |
| 92 | [huaxiren6/DSH-EmailReader](https://github.com/huaxiren6/DSH-EmailReader) | 2 | 2026-08-20 | 2026-08-27 | IMAP email reader for DeepSeek Harness: list, read, and search mail via imapflow (email_list / email_read / email_search). |
| 93 | [huaxiren6/DSH-SmsWebhook](https://github.com/huaxiren6/DSH-SmsWebhook) | 2 | 2026-08-20 | 2026-08-27 | SMS forwarding webhook for DeepSeek Harness: receive pushes from phone SMS Forwarder apps, store them, expose sms_recent / sms_search tools. |
| 94 | [iimaguest/phone-tunnel-pool](https://github.com/iimaguest/phone-tunnel-pool) | 2 | 2026-08-23 | 2026-08-28 | Refreshable Cloudflare quick-tunnel pool for the dsh web GUI — phone access with QR + embedded login |
| 95 | [imroc/dsh-project-prompt](https://github.com/imroc/dsh-project-prompt) | 2 | 2026-08-26 | 2026-08-27 | Private, per-project prompt rules for DeepSeek Harness — matched by git remote/repo/path, worktree-aware, never committed to the repo |
| 96 | [ipromise2021/dsh-omc-tui](https://github.com/ipromise2021/dsh-omc-tui) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness (DSH) 原生全功能终端交互界面 · Claude Code-styled Terminal TUI & CLI for DeepSeek Harness |
| 97 | [jing-hy/dsh-unified-market](https://github.com/jing-hy/dsh-unified-market) | 2 | 2026-08-21 | 2026-08-27 | Unified plugin market for DSH Desktop (EAC): curated catalog + GitHub dsh-plugin + npm registry three sources; install/update management and .dshpack feature packs. 统一插件市场（三源聚合，EAC 特化）。 |
| 98 | [jinsiyu/dsh-code-server-app](https://github.com/jinsiyu/dsh-code-server-app) | 2 | 2026-08-25 | 2026-08-27 | 将code-server（VSCode网页版）打包安装到dsh内的插件，快速实现专业的文件编辑。Package and install code-server (the web version of VSCode) as a plugin within dsh to quickly achieve professional file editing. |
| 99 | [jiuge2467/DSH-Desktop](https://github.com/jiuge2467/DSH-Desktop) | 2 | 2026-08-18 | 2026-08-28 | 🐬 专为小白与极客打造的 DeepSeek Harness 桌面全栈工作台：内置小鲸鱼姬桌宠、多源 MCP 调试沙箱、持久化终端与看板 \| The Geek & Cozy Desktop Client for DeepSeek Harness with Whale-chan Mascot, MCP Hub & Terminal. |
| 100 | [JochenYang/dsh-app](https://github.com/JochenYang/dsh-app) | 2 | 2026-08-20 | 2026-08-28 |   A community-maintained branded desktop client for  DeepSeek Harness, Windows / macOS / Linux |
| 101 | [Kilganon725/dsh-mic-dictation](https://github.com/Kilganon725/dsh-mic-dictation) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: mic dictation button next to the Full access control |
| 102 | [kiligzzz/dsh-skill-mcp-manager](https://github.com/kiligzzz/dsh-skill-mcp-manager) | 2 | 2026-08-21 | 2026-08-30 | Capability Manager for DeepSeek Harness: manage MCP servers and Skills from a Settings-page UI (dual-face dsh plugin) |
| 103 | [kober-basket/dsh-cachescope](https://github.com/kober-basket/dsh-cachescope) | 2 | 2026-08-26 | 2026-08-28 | Prompt-cache observability and logical-input diagnostics for DeepSeek Harness. |
| 104 | [leolee9086/zhihu-tools](https://github.com/leolee9086/zhihu-tools) | 2 | 2026-08-22 | 2026-08-27 | 知乎数据开放平台 DSH 静态双面插件:17工具+精美卡片+串行化限流。QQ群1017854502 https://qm.qq.com/q/RAHJuyhQQ |
| 105 | [maxmilian/dsh-grafana-query](https://github.com/maxmilian/dsh-grafana-query) | 2 | 2026-08-26 | 2026-08-27 | Read-only Grafana metrics and alert tools for DeepSeek Harness (PromQL via datasource proxy). |
| 106 | [maxmilian/dsh-odoo](https://github.com/maxmilian/dsh-odoo) | 2 | 2026-08-26 | 2026-08-27 | Read-only Odoo tools for DeepSeek Harness, with an opt-in restricted draft-create tool. |
| 107 | [maxmilian/dsh-sentry](https://github.com/maxmilian/dsh-sentry) | 2 | 2026-08-26 | 2026-08-27 | Read-only Sentry issue and event tools for DeepSeek Harness. |
| 108 | [meyaomiao/dsh-github-workbench](https://github.com/meyaomiao/dsh-github-workbench) | 2 | 2026-08-26 | 2026-08-27 | DSH 插件:在侧边栏使用 GitHub —— 仓库目录树 + Issues/PR/Actions 页签,支持建 Issue/PR、评论、合并、重跑 CI;better-sidebar 页签与独立面板双形态 |
| 109 | [meyaomiao/dsh-server-deck](https://github.com/meyaomiao/dsh-server-deck) | 2 | 2026-08-26 | 2026-08-28 | 服务器卡片仪表盘 for DeepSeek Harness — card dashboard (status/CPU/mem/disk) + one-click xterm terminal, better-sidebar tab or standalone drawer |
| 110 | [miuzel/dsh-subagent-ui](https://github.com/miuzel/dsh-subagent-ui) | 2 | 2026-08-26 | 2026-08-27 | Searchable workspace subagent manager for DeepSeek Harness Web |
| 111 | [mrRisega/dsh-remote](https://github.com/mrRisega/dsh-remote) | 2 | 2026-08-19 | 2026-08-27 | Remote control for DeepSeek Harness (dsh web) from any phone browser: tunnel-mode relay client with one-command install and self-hosting support |
| 112 | [ningbonb/dsh-client-ui-brand](https://github.com/ningbonb/dsh-client-ui-brand) | 2 | 2026-08-26 | 2026-08-27 | Custom product name and logo branding for DeepSeek Harness Web 自定义 DeepSeek Harness Web 端 logo 和产品名称 |
| 113 | [NOirBRight/dsh-llm-opencode-go](https://github.com/NOirBRight/dsh-llm-opencode-go) | 2 | 2026-08-26 | 2026-08-29 | OpenCode Go LLM provider plugin for DeepSeek Harness |
| 114 | [omdsh-dev/dsh-file-trace](https://github.com/omdsh-dev/dsh-file-trace) | 2 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 115 | [ph4310822/dsh-edex-jarvis-ui](https://github.com/ph4310822/dsh-edex-jarvis-ui) | 2 | 2026-08-25 | 2026-08-27 | DeepSeek Harness eDEX-UI shell plugin — JARVIS variant: electric cyan HUD with VITAL SIGNS / RT-MONITOR / RT-LOG left bar, POWER CORE / RADAR right bar, JARVIS header |
| 116 | [PianoPrince/dsh-workspace-mover](https://github.com/PianoPrince/dsh-workspace-mover) | 2 | 2026-08-26 | 2026-08-30 | 拖拽跨工作区真迁移 DSH 会话：批量移动、挂错归位、分组合并；步步备份回滚，零 token 消耗 / Move DSH sessions across workspaces by drag & drop — true migration, batch move, misfiled homing, group merge; backups + rollback, zero tokens. |
| 117 | [PolinniZhong/dsh-session-workbench](https://github.com/PolinniZhong/dsh-session-workbench) | 2 | 2026-08-21 | 2026-08-30 | Session Workbench for DeepSeek Harness: session-library full-text search + recall + conversation-view management (show/hide + reorder). 会话工作台：会话库（历史会话全文搜索与召回）+ 会话视图（标签栏显示/隐藏 + 拖拽排序）。 |
| 118 | [qingmomo233/dsh-thinking-language](https://github.com/qingmomo233/dsh-thinking-language) | 2 | 2026-08-16 | 2026-08-29 | 更改 deepseek harness 思考过程语言 |
| 119 | [QinpanWan/dsh-sky-skin](https://github.com/QinpanWan/dsh-sky-skin) | 2 | 2026-08-25 | 2026-08-27 | Sky: Children of the Light themed skin for DeepSeek Harness web UI - light children on a glowing star map, candlelight gold and starry night. 光遇·遇境主题皮肤。 |
| 120 | [SeverusZh/dsh-skills-mcp-group-manager](https://github.com/SeverusZh/dsh-skills-mcp-group-manager) | 2 | 2026-08-28 | 2026-08-28 | DeepSeek Harness Skills & MCPs 分组管理器 — 分组管理 Skills、过滤模型技能目录、独立开关 MCP 服务器、左侧面板一键管理 / Group skills, filter the model skill catalog, toggle MCP servers, left panel UI |
| 121 | [Shyboy0499/dsh-git-tools](https://github.com/Shyboy0499/dsh-git-tools) | 2 | 2026-08-26 | 2026-08-27 | Local git tools for DeepSeek Harness (dsh): git_status, git_diff, git_log, git_commit |
| 122 | [squirrel20/dsh-cron](https://github.com/squirrel20/dsh-cron) | 2 | 2026-08-26 | 2026-08-27 | Unattended scheduled jobs for the DeepSeek Harness (dsh): agent/command tasks on cron schedules |
| 123 | [STARDUSTLC666/dsh-cite](https://github.com/STARDUSTLC666/dsh-cite) | 2 | 2026-08-15 | 2026-08-27 | DeepSeek Harness 参考文献插件：cite_lookup/check/format/bibtex/health 五工具，DOI 精确查询、Crossref 题录检索、GB/T 7714/APA/MLA/Chicago 格式化、有界并发 DOI 校验；纯 Node 全平台。· Citation tools for DeepSeek Harness agents. |
| 124 | [statem-li/dsh-triad](https://github.com/statem-li/dsh-triad) | 2 | 2026-08-28 | 2026-08-28 | DSH 三合一扩展插件：用量工作台 · 技能管理 · 长期记忆引擎。零 DSH 源码改动，一句话安装。 |
| 125 | [Stylelinzzz/dsh-chat-history](https://github.com/Stylelinzzz/dsh-chat-history) | 2 | 2026-08-17 | 2026-08-30 | Chat history TOC for DeepSeek Harness: a History conversation view tab listing user messages with auto-paging and click-to-jump back into the chat. / DeepSeek Harness 会话目录插件：用户消息历史一键跳转。 |
| 126 | [summer-521/deepseek-harness-desktop](https://github.com/summer-521/deepseek-harness-desktop) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness 的非官方桌面封装：本地优先、沙箱隔离，内置 dsh 版本管理与插件管理，支持自动更新与任务完成桌面通知（macOS）。 |
| 127 | [theoneLee/deepseek-harness-sdk-go](https://github.com/theoneLee/deepseek-harness-sdk-go) | 2 | 2026-08-15 | 2026-08-27 | Go SDK for driving DeepSeek Harness |
| 128 | [vuldin/yapa](https://github.com/vuldin/yapa) | 2 | 2026-03-24 | 2026-08-27 | Yet Another Personal Assistant |
| 129 | [wanyexin1998/dsh-workbench](https://github.com/wanyexin1998/dsh-workbench) | 2 | 2026-08-26 | 2026-08-27 | Community-maintained source preview for two-Pane DeepSeek Harness Web workflows |
| 130 | [wishesl/dsh-launcher](https://github.com/wishesl/dsh-launcher) | 2 | 2026-08-28 | 2026-08-29 | Manage DSH plugins & runtime without launching it: plugin market, per-instance masking, version install. Wails v2 (Go + React).  DeepSeek Harness 桌面启动器：不启动 DSH 即可安全管理插件与本体——多实例/多版本一键启动、实时日志、npm 版本查询、插件市场（安装/卸载/开关/收藏/分享码）、实例级插件临时屏蔽。基于 Wails v2 (Go + React)。 |
| 131 | [WSL043/dsh-reasoning-slider](https://github.com/WSL043/dsh-reasoning-slider) | 2 | 2026-08-23 | 2026-08-27 | DeepSeek Harness 推理强度滑杆：按模型能力控制 reasoning effort，提供原生与 WebGL 模式。 |
| 132 | [x1shang/dsh-koin-lily-news](https://github.com/x1shang/dsh-koin-lily-news) | 2 | 2026-08-21 | 2026-08-27 | 菲奖得主强推的百合新闻订阅DSH插件 |
| 133 | [yaoshuo530/dsh-prompt-enhancer](https://github.com/yaoshuo530/dsh-prompt-enhancer) | 2 | 2026-08-28 | 2026-08-28 | A prompt-enhancement plugin for DeepSeek Harness: an ✨ Enhance composer button that rewrites prompts with first-principles thinking using session context, and asks clarifying questions when key info is missing. |
| 134 | [Yvesgao/dsh-shortcut-creator](https://github.com/Yvesgao/dsh-shortcut-creator) | 2 | 2026-08-15 | 2026-08-30 | DSH 启动器- 在 DSH 设置页一键创建 Windows 桌面快捷方式，自动打开浏览器、可固定任务栏。DSH plugin: one-click Windows desktop shortcut launcher from the Settings page (DeepSeek Harness or any local server) —Install: dsh plugin --profile web add github:Yvesgao/dsh-desktop-shortcut#main |
| 135 | [zhenghaoyang24/obsidian-plugin-deepshian](https://github.com/zhenghaoyang24/obsidian-plugin-deepshian) | 2 | 2026-08-27 | 2026-08-27 | Sidebar AI chat powered by the local DeepSeek Harness (dsh): streaming replies, tool calls, and real vault file edits. |
| 136 | [zhoulvyuan/dsh-plugin](https://github.com/zhoulvyuan/dsh-plugin) | 2 | 2026-08-26 | 2026-08-28 | deepseek-harness插件 |
| 137 | [0xrushmoon/dsh-freeroute](https://github.com/0xrushmoon/dsh-freeroute) | 1 | 2026-08-25 | 2026-08-27 | Free-tier model aggregation plugin for the DeepSeek Harness (dsh): transparent failover, multi-key rotation, settings panel |
| 138 | [166767/dsh-error-audit](https://github.com/166767/dsh-error-audit) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 实时 AI 自审插件：任何报错/警告第一时间连同时间、错误码、会话、用户原话、AI 动作与工作区写入专用日志目录，并主动通知 AI、内置 read_error_logs 工具随时读取。Real-time AI self-audit for DeepSeek Harness — captures every error/warning with timestamp, error code, session, user prompt, AI action and workspace into a dedicated log folder; instantly notifies the agent and ships a read_error_logs tool. |
| 139 | [173787247/dsh-tool-budget](https://github.com/173787247/dsh-tool-budget) | 1 | 2026-08-29 | 2026-08-29 | Hard-stop DeepSeek Harness tool use after a per-session call budget |
| 140 | [173787247/dsh-wsl-browser](https://github.com/173787247/dsh-wsl-browser) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: open http(s) URLs in the Windows default browser from WSL. |
| 141 | [173787247/dsh-wsl-clipboard](https://github.com/173787247/dsh-wsl-clipboard) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: read/write the Windows clipboard from WSL. |
| 142 | [173787247/dsh-wsl-cred](https://github.com/173787247/dsh-wsl-cred) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: safe Git credential hints for Windows GCM from WSL. |
| 143 | [173787247/dsh-wsl-distro](https://github.com/173787247/dsh-wsl-distro) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: current WSL distro facts and multi-distro warnings. |
| 144 | [173787247/dsh-wsl-github](https://github.com/173787247/dsh-wsl-github) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness: GitHub App status (open PRs + latest Actions) for WSL agents |
| 145 | [173787247/dsh-wsl-gpu](https://github.com/173787247/dsh-wsl-gpu) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: probe nvidia-smi / GPU visibility inside WSL. |
| 146 | [173787247/dsh-wsl-kit](https://github.com/173787247/dsh-wsl-kit) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness WSL kit (EN/ZH): docs + install.sh + cordis.patch for Windows browser + WSL agent plugins |
| 147 | [173787247/dsh-wsl-launch](https://github.com/173787247/dsh-wsl-launch) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: launch allowlisted Windows apps from WSL. |
| 148 | [173787247/dsh-wsl-notify](https://github.com/173787247/dsh-wsl-notify) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: Windows MessageBox notification from WSL. |
| 149 | [173787247/dsh-wsl-path](https://github.com/173787247/dsh-wsl-path) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: convert WSL Linux and Windows paths with /mnt/c caveats. |
| 150 | [173787247/dsh-wsl-port](https://github.com/173787247/dsh-wsl-port) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: diagnose WSL port listening and Windows localhost forwarding. |
| 151 | [240xu/verdict-engine](https://github.com/240xu/verdict-engine) | 1 | 2026-08-24 | 2026-08-27 | Verdict Engine — machine-checkable engineering governance: prose skill for any agent + dsh-themis DSH plugin (read-only tools, fail-closed, protocolJson negotiation). 纯文本规范 + 可校验运行时双载体。 |
| 152 | [33moren33/dsh-slice-bench](https://github.com/33moren33/dsh-slice-bench) | 1 | 2026-08-30 | 2026-08-30 | 把插件放进一台真起来的最小 DSH 机器，让 harness 自己说它站不站得住 · Runtime bench for DSH plugin version conflicts — the harness gives the verdict, not us |
| 153 | [452926826/dsh-ssh-logs](https://github.com/452926826/dsh-ssh-logs) | 1 | 2026-08-25 | 2026-08-27 | Read allowlisted remote logs over SSH from DeepSeek Harness conversations |
| 154 | [algerkong/dsh-image-preview](https://github.com/algerkong/dsh-image-preview) | 1 | 2026-08-27 | 2026-08-27 | Image preview for DSH (DeepSeek Harness) web sessions: read_image results render as a thumbnail, click for full size in the built-in lightbox. |
| 155 | [amphilagus/dsh-gamer](https://github.com/amphilagus/dsh-gamer) | 1 | 2026-08-20 | 2026-08-28 | DSH bundle + 游戏玩家 preset: play on a dsh-gaming-platform instance. |
| 156 | [Ansonfishing/dsh-ca-ref](https://github.com/Ansonfishing/dsh-ca-ref) | 1 | 2026-08-28 | 2026-08-28 | Clean Architecture reference library for DSH: 8 pinned reference repos with FTS5 search, assertion rules, and a review ledger for architecture reviews |
| 157 | [Ansonfishing/dsh-cap-profile](https://github.com/Ansonfishing/dsh-cap-profile) | 1 | 2026-08-28 | 2026-08-28 | Per-model capability profiling for DSH: turns local session history into tool-usage and error-rate dashboards with time-range filters |
| 158 | [arthur20150522/dsh-token-usage-cost](https://github.com/arthur20150522/dsh-token-usage-cost) | 1 | 2026-08-28 | 2026-08-28 | Shows per-turn and session token costs in DSH web conversations. |
| 159 | [Ary66101/dsh-desktop](https://github.com/Ary66101/dsh-desktop) | 1 | 2026-08-25 | 2026-08-27 | dsh的自制桌面端 |
| 160 | [Ary66101/dsh-instruction-bubble](https://github.com/Ary66101/dsh-instruction-bubble) | 1 | 2026-08-27 | 2026-08-27 | 你的上文语境小气泡 |
| 161 | [awnlight/talon-ui](https://github.com/awnlight/talon-ui) | 1 | 2026-08-28 | 2026-08-28 | A terminal UI for DeepSeek Harness (dsh) agents. |
| 162 | [better-er/dsh-cache-billing](https://github.com/better-er/dsh-cache-billing) | 1 | 2026-08-28 | 2026-08-28 | DSH 缓存账单插件：上下文圆环弹层里实时算账，峰谷自动计价，第三方中转照常记账 |
| 163 | [BHXiang/auto-pwa](https://github.com/BHXiang/auto-pwa) | 1 | 2026-08-19 | 2026-08-28 | AI驱动的分波分析自动化。 |
| 164 | [Binaryinject/dsh-review-checkout](https://github.com/Binaryinject/dsh-review-checkout) | 1 | 2026-08-26 | 2026-08-28 | dsh-review-checkout |
| 165 | [BlueChonk/dsh-balance-phoebe](https://github.com/BlueChonk/dsh-balance-phoebe) | 1 | 2026-08-28 | 2026-08-29 | 个人自用 鸣潮菲比查 longcat 剩余 token 挂件 - DSH 插件 |
| 166 | [bobjia/dsh-context-milvus](https://github.com/bobjia/dsh-context-milvus) | 1 | 2026-08-29 | 2026-08-29 | claude-context-milvus like plugin for Deepseek Harness (DSH)  |
| 167 | [Bobnemimimmi/dsh-always-status-bar](https://github.com/Bobnemimimmi/dsh-always-status-bar) | 1 | 2026-08-26 | 2026-08-27 | 始终显示消息下的 status bar，无需鼠标悬停 |
| 168 | [bruc3van/dsh-doctor](https://github.com/bruc3van/dsh-doctor) | 1 | 2026-08-29 | 2026-08-29 | 帮助 Agent 诊断和升级 DeepSeek Harness 插件，从 DSH 0.1.1 适配到 0.1.2：识别 API 变化、修改代码、处理语义迁移，并为重新发布做好准备。 |
| 169 | [caopu16/dsh-local-memory](https://github.com/caopu16/dsh-local-memory) | 1 | 2026-08-27 | 2026-08-27 | DSH（DeepSeek Harness）本地跨会话记忆插件：捕获每轮对话摘要、注入最近几天记忆，并提供 memory_search 工具按需检索全部历史记忆。 |
| 170 | [Carrick-K7/dsh-plugin-source](https://github.com/Carrick-K7/dsh-plugin-source) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: group the Settings plugin list by origin (official/community), show version, upstream repo link and local-dev marker. Read-only, zero network. |
| 171 | [ccll/dsh-activity-pane](https://github.com/ccll/dsh-activity-pane) | 1 | 2026-08-24 | 2026-08-29 | Activity session overview pane for DeepSeek Harness (DSH) web — running sessions, sub-agents, waiting-for-action reminders & recent history at a glance / DSH 活动会话总览窗格 |
| 172 | [Charlie-Wang-03/dsh-sightline](https://github.com/Charlie-Wang-03/dsh-sightline) | 1 | 2026-08-23 | 2026-08-27 | See the same repo through every agent's eyes — compare the effective instruction surfaces of DeepSeek Harness, Codex, and Claude Code. 查看同一仓库在 DeepSeek Harness、Codex 与 Claude Code 眼中的不同指令面。 |
| 173 | [chen731215-dev/dsh-muv-engine](https://github.com/chen731215-dev/dsh-muv-engine) | 1 | 2026-08-27 | 2026-08-27 | DSH Native MUV Engine - tavern companion: regex script execution, variable state tracking, iframe status bar rendering, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 174 | [chen731215-dev/dsh-muv-table](https://github.com/chen731215-dev/dsh-muv-table) | 1 | 2026-08-27 | 2026-08-27 | MUV Variable Table Editor - tavern companion plugin for DeepSeek Harness: structured table editing for UpdateVariable blocks, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 175 | [chendefine/dsh-sidebar-cdp-browser](https://github.com/chendefine/dsh-sidebar-cdp-browser) | 1 | 2026-08-19 | 2026-08-27 | deepseek harness live view chromium via cdp in sidebar tab |
| 176 | [cherrchen/dsh-theme-studio](https://github.com/cherrchen/dsh-theme-studio) | 1 | 2026-08-26 | 2026-08-27 | 可移植的 DSH/Cordis 主题插件：内置配色浏览、预览、应用与持久化；DeepSeek Harness Desktop 预装。 / Portable DSH/Cordis theme overlay plugin with builtin palettes, preview, apply, and persistence; pre-installed in DeepSeek Harness Desktop. |
| 177 | [chongyangdu2008-cyrus/dsh-subagent-inspector](https://github.com/chongyangdu2008-cyrus/dsh-subagent-inspector) | 1 | 2026-08-28 | 2026-08-28 | Read-only live subagent process inspector for DeepSeek Harness Web |
| 178 | [CJYLZS/dsh-commandcode-plan-autosync](https://github.com/CJYLZS/dsh-commandcode-plan-autosync) | 1 | 2026-08-28 | 2026-08-28 | auto sync commandcode coding plan models in dsh |
| 179 | [Cmjingahaha/dsh-dudulu](https://github.com/Cmjingahaha/dsh-dudulu) | 1 | 2026-08-27 | 2026-08-27 | 嘟一声 · DSH 任务完成提示音插件：Agent 回合完成时播放提示音，带设置面板（音量/试听/上传） |
| 180 | [CNSeniorious000/dsh-py-codeact](https://github.com/CNSeniorious000/dsh-py-codeact) | 1 | 2026-08-28 | 2026-08-28 | Python-based CodeAct for dsh with persistent state across cells, replacing Dynamic Workflows and code-mode |
| 181 | [CodermanYHZ/dsh-node-flow](https://github.com/CodermanYHZ/dsh-node-flow) | 1 | 2026-08-27 | 2026-08-27 | 节点式 DSH 工作流画布：编排子代理、代码、条件、循环与定时任务，支持模型路由与 AI 生成指南。 Node-mode DSH workflow canvas: orchestrate sub-agents, code, conditions, loops & scheduled tasks. |
| 182 | [conafun/dsh-music-plus](https://github.com/conafun/dsh-music-plus) | 1 | 2026-08-29 | 2026-08-29 | 基于 dsh-music-player 的修改版：移除在线QQ/酷狗/讲书/歌词，新增播客 |
| 183 | [crazy-L118/dsh-desktop-notify](https://github.com/crazy-L118/dsh-desktop-notify) | 1 | 2026-08-25 | 2026-08-27 | Desktop notification plugin for dsh: get a native OS toast when the AI finishes its reply. Toggle lives in dsh Settings → General. |
| 184 | [CSI-entitymorton/stavros-dsh-redteamer](https://github.com/CSI-entitymorton/stavros-dsh-redteamer) | 1 | 2026-08-29 | 2026-08-29 | Authorized-only AI red-team / pentest plugin for the DeepSeek Harness (DSH). Fail-closed scope guard: Stavros persona, 24 specialist subagents, 78 zero-dependency tools. |
| 185 | [czj-git/dsh-plugin-hub](https://github.com/czj-git/dsh-plugin-hub) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness tools for searching and ranking verified plugins from DSH Plugin Hub |
| 186 | [D-Robotics/dsh-plugin-rdk](https://github.com/D-Robotics/dsh-plugin-rdk) | 1 | 2026-08-14 | 2026-08-28 | D-Robotics RDK (地瓜机器人) integration for DeepSeek Harness — native RDK skill catalog, rdk_skills browser tool, and rdk_board_detect device detection |
| 187 | [D2Moqi/dsh-openwiki](https://github.com/D2Moqi/dsh-openwiki) | 1 | 2026-08-29 | 2026-08-29 | DSH 插件：把 openwiki 的代码库知识库能力搬进 DeepSeek Harness —— 一键生成 / 阅读 / 更新仓库 Wiki 与 Grounded Claims（溯源知识卡片），直接复用 DSH 已配置的模型，无需二次填 Key。 |
| 188 | [d3vmeh/dsh-fetch-timeouts](https://github.com/d3vmeh/dsh-fetch-timeouts) | 1 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: raise Node's HTTP timeouts process-wide so slow local models (Ollama, LM Studio) are not cut off at 5 minutes |
| 189 | [d3vmeh/dsh-llm-gate](https://github.com/d3vmeh/dsh-llm-gate) | 1 | 2026-08-29 | 2026-08-29 | Per-provider concurrency gate for DeepSeek Harness model requests |
| 190 | [DahliaVoid/dsh-temp-session](https://github.com/DahliaVoid/dsh-temp-session) | 1 | 2026-08-28 | 2026-08-28 | dsh工作区可选化，100%纯AI coding产物 |
| 191 | [daishengli/dsh-docker](https://github.com/daishengli/dsh-docker) | 1 | 2026-08-27 | 2026-08-28 | 使用 Docker 封装运行 deepseek-harness d的 Web 服务。容器内运行 dsh 和 Caddy，宿主机通过 3080 端口访问服务。 |
| 192 | [dat-lequoc/dsh-opinionated-subagent](https://github.com/dat-lequoc/dsh-opinionated-subagent) | 1 | 2026-08-27 | 2026-08-28 | A minimal, opinionated subagent for DeepSeek Harness: you choose which models a child may run on and at which reasoning effort, and a correction reaches a working child at its next step |
| 193 | [DDDFXYqiming/dsh-session-recap](https://github.com/DDDFXYqiming/dsh-session-recap) | 1 | 2026-08-28 | 2026-08-28 | Session recap plugin for DeepSeek Harness (Claude Code-style away summaries) |
| 194 | [ddtcorex/dsh-maestro-ci](https://github.com/ddtcorex/dsh-maestro-ci) | 1 | 2026-08-26 | 2026-08-28 | Reusable GitHub Actions workflows for the Maestro suite — Cordis / DSH |
| 195 | [ddtcorex/dsh-maestro-config-lib](https://github.com/ddtcorex/dsh-maestro-config-lib) | 1 | 2026-08-25 | 2026-08-28 | Maestro settings store library — atomic namespaced JSON store shared by dsh-maestro-* plugins (embedded dependency, no Cordis row) |
| 196 | [ddtcorex/dsh-maestro-dashboard](https://github.com/ddtcorex/dsh-maestro-dashboard) | 1 | 2026-08-28 | 2026-08-28 | Maestro Dashboard — unified Control Center (Overview/Plugins/Usage) DSH-native |
| 197 | [ddtcorex/dsh-maestro-devkit](https://github.com/ddtcorex/dsh-maestro-devkit) | 1 | 2026-08-27 | 2026-08-28 | General development toolkit for DeepSeek Harness — visual review, HMR, style inspector, Cordis/Govard/Skills dev (tunnel-aware) |
| 198 | [ddtcorex/dsh-maestro-diagram](https://github.com/ddtcorex/dsh-maestro-diagram) | 1 | 2026-08-27 | 2026-08-28 | DSH Maestro diagram studio — mermaid_verify + mermaid_drift |
| 199 | [ddtcorex/dsh-maestro-supervisor](https://github.com/ddtcorex/dsh-maestro-supervisor) | 1 | 2026-08-27 | 2026-08-28 | Supervisor daemon for DSH Web resilience — auto-detect crashes, rollback to LKG, report |
| 200 | [difimim/dsh-voice-input-npm](https://github.com/difimim/dsh-voice-input-npm) | 1 | 2026-08-30 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 201 | [domitor-syh/dsh-ui-skin-switcher](https://github.com/domitor-syh/dsh-ui-skin-switcher) | 1 | 2026-08-27 | 2026-08-28 | Model & reasoning-effort switcher plugin for DeepSeek Harness (DSH): composer seat with Off/Max effort slider. DSH 插件：模型与思考力度切换器。 |
| 202 | [doublemolu/dsh-balance-dock](https://github.com/doublemolu/dsh-balance-dock) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness balance dock: balance card, per-conversation spend/tokens, 50-yuan segmented progress bar, recharge button, position guard |
| 203 | [drscrewdriver/dsh-llm-openai-completions](https://github.com/drscrewdriver/dsh-llm-openai-completions) | 1 | 2026-08-29 | 2026-08-29 | dsh-llm-openai-completions |
| 204 | [EastMG/dsh-gacha-calendar](https://github.com/EastMG/dsh-gacha-calendar) | 1 | 2026-08-27 | 2026-08-30 | DeepSeek Harness 二游卡池/活动排期速查插件：侧边栏按钮 内置 11 款主流二游 可添加自定义游戏 |
| 205 | [Edge-Echo/dsh-netassist](https://github.com/Edge-Echo/dsh-netassist) | 1 | 2026-08-30 | 2026-08-30 | Network & proxy assistant for DeepSeek Harness (dsh): one-shot GitHub connectivity check, system proxy status, proxy port probing, full diag chain and hosts conflict scan. |
| 206 | [Edge-Echo/dsh-win-toolkit](https://github.com/Edge-Echo/dsh-win-toolkit) | 1 | 2026-08-30 | 2026-08-30 | Windows-native capability pack for DeepSeek Harness (dsh): clipboard, notifications, hosts file, network diagnostics — safe PowerShell-backed tools. |
| 207 | [elizax/dsh-http-proxy](https://github.com/elizax/dsh-http-proxy) | 1 | 2026-08-26 | 2026-08-27 | 支持设置LLM的代理地址 |
| 208 | [Elpsycoogroo/dsh-work-report](https://github.com/Elpsycoogroo/dsh-work-report) | 1 | 2026-08-28 | 2026-08-28 | Neural Ledger - turn DSH collaboration sessions into a visual work ledger: token analytics, smart insights, trend forecasting, and one-click daily/weekly/monthly Markdown reports. |
| 209 | [exoticknight/dsh-theme-eink-retro](https://github.com/exoticknight/dsh-theme-eink-retro) | 1 | 2026-08-26 | 2026-08-27 | A paper-and-ink client-side theme for DeepSeek Harness with Balanced and Immersive modes. |
| 210 | [ExplorerZYzhou/DSH-freeweb](https://github.com/ExplorerZYzhou/DSH-freeweb) | 1 | 2026-08-27 | 2026-08-27 | DSH 免费联网搜索插件（Parallel 后端，零依赖） |
| 211 | [f1yan9/dsh-balance-pie](https://github.com/f1yan9/dsh-balance-pie) | 1 | 2026-08-30 | 2026-08-30 | DSH 插件：可拖拽余额饼图 / 真实消耗 / 历史热力图 — balance pie with real spending & monthly heatmap for DeepSeek Harness. |
| 212 | [falling-ts/dsh-web-ding](https://github.com/falling-ts/dsh-web-ding) | 1 | 2026-08-27 | 2026-08-27 | Browser-only 'ding' on agent end; works on servers.浏览器专属"叮":回合结束时响起,服务器部署也生效 |
| 213 | [fan56/dsh-subagent-registry](https://github.com/fan56/dsh-subagent-registry) | 1 | 2026-08-16 | 2026-08-28 | dsh plugin: register ~/.dsh/agents/*.md as dsh-callable subagents |
| 214 | [FanetheDivine/dsh-plugin-om](https://github.com/FanetheDivine/dsh-plugin-om) | 1 | 2026-08-15 | 2026-08-27 | DSH插件，以Observational Memory方式管理上下文 |
| 215 | [fengb3/dsh-theme-aurum](https://github.com/fengb3/dsh-theme-aurum) | 1 | 2026-08-24 | 2026-08-28 | DSH 鎏金主题插件:金粉奢华皮肤,htm 恒等映射流水,原型驱动的逐节移植 |
| 216 | [focksor/dsh-plugin-mini-dashboard](https://github.com/focksor/dsh-plugin-mini-dashboard) | 1 | 2026-08-28 | 2026-08-28 | A session & token mini dashboard for DSH web. It renders just above the sidebar's "Settings" row and summarizes, in one small draggable float window, what your sessions are doing right now and what they have cost you today. |
| 217 | [focksor/dsh-plugin-thinking-size](https://github.com/focksor/dsh-plugin-thinking-size) | 1 | 2026-08-28 | 2026-08-28 | A live reasoning-token badge for DSH web. It appends a compact Think(128) / Think(5.2K) marker to the title of every "Think" disclosure row in the conversation — ticking in real time while the model is still thinking, and staying put on history messages afterwards. |
| 218 | [FranklinZaneDurant/agent-discipline](https://github.com/FranklinZaneDurant/agent-discipline) | 1 | 2026-08-27 | 2026-08-27 | 给 AI 编码 Agent 的仓库工作纪律插件（DeepSeek Harness bundle）：方法论提示段 + 工件脚手架（AGENTS.md/特性清单/验证门）+ 合规审计。 |
| 219 | [fu827707013/dsh-concurrency-guard](https://github.com/fu827707013/dsh-concurrency-guard) | 1 | 2026-08-26 | 2026-08-27 | DSH（DeepSeek Harness）并发请求监控与门闩插件。 |
| 220 | [fufengyuan/dsh-council](https://github.com/fufengyuan/dsh-council) | 1 | 2026-08-26 | 2026-08-27 | dsh-council — 高智议会（Council of High Intelligence）for DeepSeek Harness 在 dsh（DeepSeek Harness）里召集历史人物议会，对复杂问题进行多视角结构化辩论，最终由主席综合裁决。 |
| 221 | [g-yixuan/dsh-sidenote](https://github.com/g-yixuan/dsh-sidenote) | 1 | 2026-08-19 | 2026-08-28 | Codex-style side chat & selection annotations for DeepSeek Harness (DSH) web — fork the session into a persistent side panel; quote selections into context. Thin consumer of dsh-better-sidebar. |
| 222 | [georesearch-dsh/georesearch-dsh](https://github.com/georesearch-dsh/georesearch-dsh) | 1 | 2026-08-27 | 2026-08-28 | GeoResearch agent plugin for DeepSeek Harness |
| 223 | [Georgehaoren/DSH-WhaleConsole](https://github.com/Georgehaoren/DSH-WhaleConsole) | 1 | 2026-08-29 | 2026-08-29 | Unofficial macOS desktop companion and WebUI skin plugin for DeepSeek Harness. 面向 DeepSeek Harness 的非官方 macOS 桌面伴侣与 WebUI 换肤插件。 |
| 224 | [goldgish/dsh-agent-trace](https://github.com/goldgish/dsh-agent-trace) | 1 | 2026-08-26 | 2026-08-27 | Agent Trace — visualize an agent's reasoning, parallel tool calls, and results as an interactive DAG inside DeepSeek Harness. |
| 225 | [GuionAI/web](https://github.com/GuionAI/web) | 1 | 2026-08-22 | 2026-08-30 | A web research toolkit with multi-provider search and clean Markdown extraction from static and JavaScript-rendered pages, plus public code and library docs search—available via CLI and MCP. |
| 226 | [gulagala001/dsh-trisoul](https://github.com/gulagala001/dsh-trisoul) | 1 | 2026-08-27 | 2026-08-27 | TriSoul —— 三魂共识 Agent：三个灵魂盲写+匿名互评，三官（对齐/博识/实证）补偿生成，画布式上下文，记忆中枢。DeepSeek Harness 插件套件，一键装/独立端口/一键卸载 |
| 227 | [hackernotfound/dsh-tacit](https://github.com/hackernotfound/dsh-tacit) | 1 | 2026-08-27 | 2026-08-27 | Learns what you leave unsaid in your prompts and steers the DeepSeek Harness agent for you |
| 228 | [Haniubub/seo-toolkit](https://github.com/Haniubub/seo-toolkit) | 1 | 2026-08-29 | 2026-08-30 | Native local & technical SEO audit toolkit for DeepSeek Harness (DSH) — self-contained port of claude-seo v2.2.5. Weighted scoring, gated multi-agent fan-out, 24 sub-skills + 18 agents, schema.org, E-E-A-T, GBP, GEO/AI Overviews, Google APIs & extensions. No Claude Code required. |
| 229 | [hejielijob-commits/SemaRail](https://github.com/hejielijob-commits/SemaRail) | 1 | 2026-08-17 | 2026-08-30 | Governed semantic layer for AI agents, with a DeepSeek Harness plugin that turns Harness into a data agent. |
| 230 | [henrychenhao/dsh-skin-argentina](https://github.com/henrychenhao/dsh-skin-argentina) | 1 | 2026-08-27 | 2026-08-27 | 梅西 阿根廷皮肤 |
| 231 | [HenryPhoebe/dsh-plugin-easyppt](https://github.com/HenryPhoebe/dsh-plugin-easyppt) | 1 | 2026-08-27 | 2026-08-27 | easyppt是一个面向 DeepSeek Harness (DSH) 的演示文稿生成 dsh-plugin（npm 包 + Cordis bundle + 内置技能）。用户输入大纲（Markdown / JSON / 自然语言）与插图，即可基于 DSH 原生 Univer 工具链生成PPTX,HTML,JSON |
| 232 | [hgl011091/dsh-rss-monitor](https://github.com/hgl011091/dsh-rss-monitor) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 原生 RSS 订阅监控插件：多源订阅、关键词过滤、定时检查去重、新条目邮件通知（缩略图 HTML 模板），SMTP 密码走凭据库永不落盘，原生设置页四页签体验。 |
| 233 | [hhb1028/dsh-retry-boost](https://github.com/hhb1028/dsh-retry-boost) | 1 | 2026-08-27 | 2026-08-27 | 让 DeepSeek Harness 自动重试商汤 429/QUOTA 等瞬时网关故障直到任务完成——启动时给所有 llm-pi-ai provider 热注入加固版 retryPolicy。 |
| 234 | [hjj345/dsh-sm-context-piano](https://github.com/hjj345/dsh-sm-context-piano) | 1 | 2026-08-21 | 2026-08-29 | DeepSeek Harness Web GUI 的 Codex 风格对话导航器：帮助用户快速浏览、定位和切换对话，提升多任务、多会话场景下的工作效率。 \|  Codex-style conversation navigator for the DeepSeek Harness Web GUI. |
| 235 | [hjj345/dsh-sm-version-display](https://github.com/hjj345/dsh-sm-version-display) | 1 | 2026-08-28 | 2026-08-30 | 用于在侧边栏“设置”按钮上方显示已安装 dsh 版本的 DeepSeek Harness Web 插件。  \|  DeepSeek Harness Web plugin that displays the installed dsh version above the sidebar Settings button. |
| 236 | [HuanLinOTO/dsh-plugin-better-glob](https://github.com/HuanLinOTO/dsh-plugin-better-glob) | 1 | 2026-08-30 | 2026-08-30 | 以 per-agent 阴影顶替内置 glob：自动排除无底洞目录（node_modules 等），传 include 白名单才能搜入 \| Shadows the built-in glob per agent: auto-excludes bottomless directories (node_modules etc.), pass an include whitelist to search inside them |
| 237 | [ianho7/dsh-port-inspector](https://github.com/ianho7/dsh-port-inspector) | 1 | 2026-08-20 | 2026-08-30 | DeepSeek Harness 的 Windows Web 插件，可将本地 TCP 监听回溯至进程、会话与工具调用，保障编程助手安全处理端口冲突/A Windows DSH Web plugin for DeepSeek Harness that traces local TCP listeners back to processes, Sessions, and Tool Calls for safe Coding Agent port-conflict handling. |
| 238 | [iasiv5/skins](https://github.com/iasiv5/skins) | 1 | 2026-08-28 | 2026-08-28 | 换肤如换季，归真只一键 —— DeepSeek Harness Web 多皮肤切换器：明暗双态、中英双语、SHA 校验自动更新。Hot-swappable brand skins for DeepSeek Harness Web. |
| 239 | [Idreamxkl/dsh-conversation-flat](https://github.com/Idreamxkl/dsh-conversation-flat) | 1 | 2026-08-30 | 2026-08-30 | Document-flow conversation layout for DeepSeek Harness web GUI — full-width column, user message bars, sender label, full-width tables. 纯 CSS 的 dsh 对话区通栏布局插件 |
| 240 | [iimaguest/dsh-contradictions-indicator](https://github.com/iimaguest/dsh-contradictions-indicator) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin: 0-100 conversation coherence badge with parallel contradiction analysis |
| 241 | [jarvis959/galvanize-dsh](https://github.com/jarvis959/galvanize-dsh) | 1 | 2026-08-28 | 2026-08-28 | Triggers inside your DSH agent: wake a fresh DeepSeek Harness session when files, mail, webhooks, or git events happen. Native Cordis bundle, heartbeat-proved install. |
| 242 | [jarvisluk/dsh-projectless-session](https://github.com/jarvisluk/dsh-projectless-session) | 1 | 2026-08-18 | 2026-08-27 | Projectless sessions for DeepSeek Harness with isolated date-organized working directories |
| 243 | [JasonFreeLab/dsh-superpowers](https://github.com/JasonFreeLab/dsh-superpowers) | 1 | 2026-08-28 | 2026-08-28 | DSH (DeepSeek Harness) port of obra/superpowers — 14 native skills for multi-agent software development: brainstorming, planning, TDD, systematic debugging, and code review. |
| 244 | [jeffy-Peng/deepseek-harness-usage](https://github.com/jeffy-Peng/deepseek-harness-usage) | 1 | 2026-08-16 | 2026-08-28 | DeepSeek Harness 插件，显示每日消费与账户总余额。DeepSeek Harness plugin for account balance and evidence-bounded daily CNY consumption |
| 245 | [Jensen-Yao/dsh-model-palette](https://github.com/Jensen-Yao/dsh-model-palette) | 1 | 2026-08-26 | 2026-08-27 | Global provider-aware model command palette and optional OpenRouter media tools for DeepSeek Harness. |
| 246 | [jetheaven/dsh-code-reviewer](https://github.com/jetheaven/dsh-code-reviewer) | 1 | 2026-08-14 | 2026-08-27 | AI代码审查插件：bug检测/安全漏洞/性能/风格四维审查，行号定位+修复示例 |
| 247 | [jetheaven/dsh-content-rewriter](https://github.com/jetheaven/dsh-content-rewriter) | 1 | 2026-08-14 | 2026-08-27 | 一键内容改写：小红书/知乎/商务邮件/精简/扩写/Twitter 多风格 |
| 248 | [jetheaven/dsh-data-extractor](https://github.com/jetheaven/dsh-data-extractor) | 1 | 2026-08-14 | 2026-08-27 | 结构化数据提取：从非结构化文本提取字段，输出 JSON/CSV/表格 |
| 249 | [jetheaven/dsh-meeting-notes](https://github.com/jetheaven/dsh-meeting-notes) | 1 | 2026-08-14 | 2026-08-27 | 会议纪要智能生成：从转写文本提取决议/待办/负责人/截止时间/风险 |
| 250 | [jetheaven/dsh-prompt-optimizer](https://github.com/jetheaven/dsh-prompt-optimizer) | 1 | 2026-08-14 | 2026-08-27 | AI提示词优化器：诊断Prompt问题并输出结构化高质量优化版本 |
| 251 | [jetheaven/dsh-seo-writer](https://github.com/jetheaven/dsh-seo-writer) | 1 | 2026-08-14 | 2026-08-27 | SEO文章生成器：给定关键词和语言，生成搜索引擎友好的完整文章 |
| 252 | [jetheaven/dsh-text-diff](https://github.com/jetheaven/dsh-text-diff) | 1 | 2026-08-14 | 2026-08-27 | AI智能文本对比：找出两段文字的差异、语义变化和潜在风险点 |
| 253 | [jetheaven/dsh-translate-pro](https://github.com/jetheaven/dsh-translate-pro) | 1 | 2026-08-14 | 2026-08-27 | 专业翻译：术语一致、专业领域选择与语气调整，附带术语对照表 |
| 254 | [jiangliuhong/dsh-gpt-oauth](https://github.com/jiangliuhong/dsh-gpt-oauth) | 1 | 2026-08-26 | 2026-08-27 | openai models for login by chatgpt |
| 255 | [JianwuYang/dsh-ui-kanban](https://github.com/JianwuYang/dsh-ui-kanban) | 1 | 2026-08-27 | 2026-08-27 | 让 agent 直接干 Jira/GitLab 的活 · DSH 看板插件 \| A dsh plugin that turns Jira + GitLab into an agent-workable kanban board |
| 256 | [jianxx/dsh-cc](https://github.com/jianxx/dsh-cc) | 1 | 2026-08-15 | 2026-08-28 | Bring the Claude Code workflow to DeepSeek Harness - TUI, permissions, hooks, memory, skills, subagents, MCP, worktrees, and more. |
| 257 | [jing-hy/computer-user](https://github.com/jing-hy/computer-user) | 1 | 2026-08-21 | 2026-08-27 | DSH plugin: Codex-style computer use for Windows - read the screen, drive mouse & keyboard via SendInput; pairs with picturereader to close the look-act-verify loop. |
| 258 | [jypjypjypjyp/dsh-notifier](https://github.com/jypjypjypjyp/dsh-notifier) | 1 | 2026-08-27 | 2026-08-27 | 审批/完成/错误事件通知：浏览器 Notification + 系统原生 toast（Windows PowerShell WinRT / macOS osascript / Linux notify-send，均无需额外安装）；提示音可配、每条通知独立显示不互相替换、非安全上下文自动降级横幅 |
| 259 | [KannaKuron/dsh-better-workspace](https://github.com/KannaKuron/dsh-better-workspace) | 1 | 2026-08-30 | 2026-08-30 | DSH web plugin: a hierarchical workspace tree for the sidebar — titles containing / group into virtual folders; the add-workspace flow gains a parent-group popup |
| 260 | [keman-ai/dsh-opencode-zen](https://github.com/keman-ai/dsh-opencode-zen) | 1 | 2026-08-19 | 2026-08-27 | Bring OpenCode Zen's free models to DeepSeek Harness — zero config, no API key, catalog discovered live from upstream |
| 261 | [kenny2077/dsh-web-search-doubao](https://github.com/kenny2077/dsh-web-search-doubao) | 1 | 2026-08-29 | 2026-08-29 | Doubao Search provider for the DeepSeek Harness |
| 262 | [kenny2077/dsh-web-search-zai](https://github.com/kenny2077/dsh-web-search-zai) | 1 | 2026-08-28 | 2026-08-28 | One ZAI_API_KEY for both chat and search — plug-and-play Z.ai (GLM) web search for the DeepSeek Harness. |
| 263 | [KevinZhangNothing/dsh-task-graph](https://github.com/KevinZhangNothing/dsh-task-graph) | 1 | 2026-08-27 | 2026-08-27 | Task flow / execution graph plugin for DeepSeek Harness (DSH) — visualize a single task's full run: agents, tools, skills, subtasks, retries, live status. DSH 单任务执行流程图谱插件。 |
| 264 | [KhalilHsu/dsh-plugins](https://github.com/KhalilHsu/dsh-plugins) | 1 | 2026-08-17 | 2026-08-28 | Enhance DeepSeek Harness Web GUI with smart per-turn reasoning/tool folding and query navigation. |
| 265 | [kiligzzz/dsh-agent-dispatch](https://github.com/kiligzzz/dsh-agent-dispatch) | 1 | 2026-08-28 | 2026-08-28 | DSH 插件：预置专家 agent + 自动路由 + 小队编排。原生右 tab「Agent 调度」+ 悬浮活动球 +  触发器。 |
| 266 | [kirbylynx/dsh-hub](https://github.com/kirbylynx/dsh-hub) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Hub |
| 267 | [l-vM2k/dsh-ayaka-theme](https://github.com/l-vM2k/dsh-ayaka-theme) | 1 | 2026-08-28 | 2026-08-28 | deepseek harness plugins dsh-ayaka-theme |
| 268 | [LamplitIsles/kepos-imagegen](https://github.com/LamplitIsles/kepos-imagegen) | 1 | 2026-08-27 | 2026-08-30 | Image generation tools via kepos exposed codex endpoint |
| 269 | [lansi-ai/dsh-desktop](https://github.com/lansi-ai/dsh-desktop) | 1 | 2026-08-25 | 2026-08-27 | 把 DeepSeek Harness 做成一个真正的桌面应用：Electron 主进程内嵌 Cordis Host（与官方 Web 版同内核、零移植）， 渲染进程加载官方 Web UI 发行物（file:///自定义协议 + IPC 桥接，不开放 HTTP 端口）， 所有桌面原生能力（托盘、全局热键、系统通知、剪贴板、开机自启、协议唤起、多窗口）以 host 插件 形态注入运行时， 与官方「一切皆插件」的架构同构——不是给网页套壳，而是把桌面能力变成可装配、可卸载、可审查的插件树。  AI 驱动开发声明 |
| 270 | [lewes2/archpresent](https://github.com/lewes2/archpresent) | 1 | 2026-08-29 | 2026-08-29 | Agent skill: generate beautiful dark-themed architecture diagrams from your project/demo/idea. Interactive, verifiable, and editable. Delivered as self-contained HTML. |
| 271 | [lhh010/dsh-file-trace](https://github.com/lhh010/dsh-file-trace) | 1 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 272 | [LHKong7/dsh-browser-runtime](https://github.com/LHKong7/dsh-browser-runtime) | 1 | 2026-08-26 | 2026-08-27 | deepseek harness plugin browser runtime |
| 273 | [liiiubai/dsh-mcp-bridge](https://github.com/liiiubai/dsh-mcp-bridge) | 1 | 2026-08-28 | 2026-08-28 | Expose DeepSeek Harness tools as a standard MCP server (streamable HTTP) — drive dsh from Claude Code, Codex, or any MCP client |
| 274 | [LLYlab/DSHEssentialTools](https://github.com/LLYlab/DSHEssentialTools) | 1 | 2026-08-27 | 2026-08-28 | DSH 永久插件：LVAL 工程运行/代码查看/程序版本快照回退 + VTD 虚拟对话树（编辑/重试/分支、消息小版本）+ DET 管理器。A permanent DeepSeek Harness plugin: project run & code viewer, program snapshots, an in-session conversation tree (edit/retry/branches), message micro-versions and a feature manager. |
| 275 | [LoKiGGo/dsh-tools](https://github.com/LoKiGGo/dsh-tools) | 1 | 2026-08-16 | 2026-08-27 | dsh web通用工具箱插件，纯AI制作（包括仓库），零人工含量，可能不会维护，请谨慎使用。 |
| 276 | [LONGSASASASASA/dsh-issue2pr](https://github.com/LONGSASASASASA/dsh-issue2pr) | 1 | 2026-08-29 | 2026-08-30 | 从一条 Issue 到一份被合并的 PR，每一段都有自己的输入契约、失败信号、可回滚产物与可独立审查的 Artifact。 |
| 277 | [looput/dsh-finance-lab](https://github.com/looput/dsh-finance-lab) | 1 | 2026-08-18 | 2026-08-27 | DeepSeek Harness finance plugin: direct market HTTP APIs, portfolio settings, model tools |
| 278 | [Lsc-91-69/dsh-brain-compaction](https://github.com/Lsc-91-69/dsh-brain-compaction) | 1 | 2026-08-28 | 2026-08-28 | 人脑式上下文压缩逻辑，大幅减少长任务上下文占用以及token消耗 |
| 279 | [lumose0/dsh-file-reference-everything](https://github.com/lumose0/dsh-file-reference-everything) | 1 | 2026-08-27 | 2026-08-27 | Whole-disk @ file references for DeepSeek Harness — Everything-backed instant search with fuzzy/regex and a cross-platform fallback index |
| 280 | [Lzh3070/dsh-model-visibility](https://github.com/Lzh3070/dsh-model-visibility) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件：模型可见性管理——按渠道/模型隐藏或显示模型选择菜单里的条目 / Control which models appear in the DSH model selector |
| 281 | [m1khal3v/dsh-tool-codegraph](https://github.com/m1khal3v/dsh-tool-codegraph) | 1 | 2026-08-29 | 2026-08-30 | CodeGraph navigation tools for DeepSeek Harness |
| 282 | [maiziman/deepseek-harness-portable](https://github.com/maiziman/deepseek-harness-portable) | 1 | 2026-08-27 | 2026-08-27 | Community-built Windows desktop wrapper for official tagged DeepSeek Harness source — unzip and run; no Node.js, installer, or admin rights. |
| 283 | [mastergo-design/dsh-canvas](https://github.com/mastergo-design/dsh-canvas) | 1 | 2026-08-27 | 2026-08-27 | MasterGo Canvas MCP plugin for DeepSeek Harness |
| 284 | [maxwell-feng/dsh-tinyfish-search](https://github.com/maxwell-feng/dsh-tinyfish-search) | 1 | 2026-08-30 | 2026-08-30 | TinyFish-backed web search provider for DeepSeek Harness (ctx.web) — 将内置 web_search 接入 TinyFish Search API 的 DeepSeek Harness 插件 |
| 285 | [me93-ghb/dsh-matrix-think](https://github.com/me93-ghb/dsh-matrix-think) | 1 | 2026-08-27 | 2026-08-27 | Matrix rain for expanded thinking in DeepSeek Harness Web |
| 286 | [mengnanxyyyy/dsh-markdown-xyy](https://github.com/mengnanxyyyy/dsh-markdown-xyy) | 1 | 2026-08-29 | 2026-08-29 | dsh markdown 主题插件 |
| 287 | [MerlinShieh/AgentMemHub](https://github.com/MerlinShieh/AgentMemHub) | 1 | 2026-08-25 | 2026-08-27 | 统一提取多 Agent Harness 会话为全量事件流(含工具链/思维链/Shell/补丁) → SQLite 检索 → 桥接 MemOS 生成记忆 |
| 288 | [MichaelShii/dsh-plugin-teamflow](https://github.com/MichaelShii/dsh-plugin-teamflow) | 1 | 2026-08-17 | 2026-08-27 | dsh plugin teamflow |
| 289 | [Missher12/deepseek-harness-desktop](https://github.com/Missher12/deepseek-harness-desktop) | 1 | 2026-08-13 | 2026-08-29 | Unofficial Intel macOS desktop app for DeepSeek Harness |
| 290 | [mldhao/dsh-conversation-strip](https://github.com/mldhao/dsh-conversation-strip) | 1 | 2026-08-27 | 2026-08-27 | Codex-inspired vertical conversation-turn rail for the DeepSeek Harness web UI. |
| 291 | [moonlin1213/dsh-agent-sound-alert](https://github.com/moonlin1213/dsh-agent-sound-alert) | 1 | 2026-08-29 | 2026-08-29 | macOS sound alerts for DeepSeek Harness agent lifecycle events |
| 292 | [Movingtoleveltwo/dsh-revert](https://github.com/Movingtoleveltwo/dsh-revert) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 现代化对话回退与重试插件：纯 UI 图形交互、原地 Prompt 微调、支持工作区与外部文件双引擎安全恢复。 |
| 293 | [mtdx2001/think-zh](https://github.com/mtdx2001/think-zh) | 1 | 2026-08-29 | 2026-08-29 | AI reasoning real-time Chinese localization suite (DSH ready, OpenAI-compatible endpoint) |
| 294 | [MuAllen/dsh-gateway-wallet](https://github.com/MuAllen/dsh-gateway-wallet) | 1 | 2026-08-24 | 2026-08-27 | 读取当前 API key 在站点账本上的剩余额度和实扣，支持 Sub2API、New API 与 DeepSeek 官方，不是本地 token 估算。 |
| 295 | [mumuer1024/dsh-ui-liteglass](https://github.com/mumuer1024/dsh-ui-liteglass) | 1 | 2026-08-21 | 2026-08-27 | LiteGlass — a lightweight appearance skin for DeepSeek Harness Web UI: wallpaper, glass-like transparency, and accent color. Server-side settings, multi-device, leaves native light/dark mode alone. |
| 296 | [my-dsh/dsh-web-search-tavily](https://github.com/my-dsh/dsh-web-search-tavily) | 1 | 2026-08-30 | 2026-08-30 | Tavily web-search provider plugin for DeepSeek Harness (dsh) — registers into ctx.web so the model-facing web_search tool uses Tavily |
| 297 | [NexusAgentX/dsh-reasoning-effort](https://github.com/NexusAgentX/dsh-reasoning-effort) | 1 | 2026-08-15 | 2026-08-27 | Host-side dsh plugin that adds seven reasoning-effort levels to third-party llm-pi-ai models in the web composer. |
| 298 | [Niceck/dsh-hhxg-market](https://github.com/Niceck/dsh-hhxg-market) | 1 | 2026-08-27 | 2026-08-27 | 恢恢量化 hhxg.top A股量化数据插件 for DeepSeek Harness (dsh)：6 个免费工具 + 5 个 VIP 工具（MCP 桥接）· A-share quant data plugin |
| 299 | [NimuStudio/NimuQDock-dsh](https://github.com/NimuStudio/NimuQDock-dsh) | 1 | 2026-08-27 | 2026-08-27 | 把 DeepSeek Harness接入QQ的对接坞——带人格引擎的仿真群友：心情、精力、记忆，像真人一样潜水与参与。 |
| 300 | [niyongsheng/meww](https://github.com/niyongsheng/meww) | 1 | 2026-08-27 | 2026-08-27 | pokemon ai pet🐣电子宠物 |
| 301 | [njjpro/dsh-vault](https://github.com/njjpro/dsh-vault) | 1 | 2026-08-30 | 2026-08-30 | Persistent credential vault plugin for DeepSeek Harness (DSH) - manage API tokens, server logins, and site credentials in one settings panel. |
| 302 | [NOirBRight/dsh-llm-commandcode](https://github.com/NOirBRight/dsh-llm-commandcode) | 1 | 2026-08-27 | 2026-08-29 | Command Code Provider API LLM plugin for DeepSeek Harness |
| 303 | [NoxTyrannus/dsh-cipher](https://github.com/NoxTyrannus/dsh-cipher) | 1 | 2026-08-29 | 2026-08-29 | 把 cipher 的持续思考/三中台/四类记忆以 UNNI/LOOP 会话模式接入 DSH（dsh-plugin bundle） |
| 304 | [Nuomi9/dsh-fgo-chaldea](https://github.com/Nuomi9/dsh-fgo-chaldea) | 1 | 2026-08-15 | 2026-08-27 | FGO Chaldea-inspired skin pack for DeepSeek Harness Web UI: 5 themes, original generated backdrops, gold trim. |
| 305 | [Nzssm1/dsh-strategy-deployment-review](https://github.com/Nzssm1/dsh-strategy-deployment-review) | 1 | 2026-08-27 | 2026-08-27 | DSH agent preset for rigorous strategy live-deployment testing/evaluation. Retest. |
| 306 | [objectivex666/dsh-settings-search](https://github.com/objectivex666/dsh-settings-search) | 1 | 2026-08-25 | 2026-08-27 | A plugin that adds a search box to the DSH settings panel. |
| 307 | [openllmsh/dsh](https://github.com/openllmsh/dsh) | 1 | 2026-08-24 | 2026-08-27 | DeepSeek Harness (dsh) bundle: route the harness through OpenLLM (OpenAI-compatible) + register the OpenLLM MCP, with CLI/daemon onboarding. |
| 308 | [patrickluvsoj/dsh-llm-nous](https://github.com/patrickluvsoj/dsh-llm-nous) | 1 | 2026-08-21 | 2026-08-27 | Nous Portal LLM plugin bundle for DeepSeek Harness |
| 309 | [phantomSuying/dsh-module-driven-develop](https://github.com/phantomSuying/dsh-module-driven-develop) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin for module-driven development: decompose requirements into a module tree, generate each module with an independent agent, and fully regenerate from design on any change. |
| 310 | [pipipigu/dsh-workspace-tree](https://github.com/pipipigu/dsh-workspace-tree) | 1 | 2026-08-28 | 2026-08-28 | Virtual session folder grouping, drag & drop, and subproject manager for DeepSeek Harness (DSH). |
| 311 | [promisez322-prog/dsh-vox-input](https://github.com/promisez322-prog/dsh-vox-input) | 1 | 2026-08-30 | 2026-08-30 | Voice (speech-to-text) input for the DSH Web composer via Web Speech API — tap, speak, transcript fills the input box. Zero server, zero API keys. |
| 312 | [pwping/dsh-power-launch](https://github.com/pwping/dsh-power-launch) | 1 | 2026-08-29 | 2026-08-29 | DSH桌面启动器插件，双击桌面快捷方式启动dsh Web UI，不需要每次打开终端手动输入命令 |
| 313 | [Qian-Ning/prompt-skill-armory](https://github.com/Qian-Ning/prompt-skill-armory) | 1 | 2026-08-27 | 2026-08-30 | Managing prompts，, skills, MCP tools & wallpaper for DeepSeek Harness |
| 314 | [QinpanWan/dsh-doc-quick](https://github.com/QinpanWan/dsh-doc-quick) | 1 | 2026-08-25 | 2026-08-27 | Drag documents into the dsh web chat for direct local-file processing; a right sidebar lists outputs and file paths. 拖拽文档进 Web 对话框快速处理，右侧侧栏展示产出。 |
| 315 | [QinpanWan/dsh-harmonyos-market](https://github.com/QinpanWan/dsh-harmonyos-market) | 1 | 2026-08-24 | 2026-08-27 | HarmonyOS-exclusive plugin market for DeepSeek Harness — only plugins that actually run on HarmonyOS |
| 316 | [Qiongkura/dsh-interface-settings](https://github.com/Qiongkura/dsh-interface-settings) | 1 | 2026-08-16 | 2026-08-29 | DSH interface customization plugin: wallpaper / transparency / glass blur / splash screen一个 DeepSeek Harness 前端插件：把「壁纸 / 区域透明 / 输入框与轨迹毛玻璃 / 模糊程度 / 启动画面」做成一站式界面设置，作为独立插件项目上传、分享，装进 DSH 即可使用 |
| 317 | [qiufengcrl/dsh-ip-https](https://github.com/qiufengcrl/dsh-ip-https) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: remote settings + Let's Encrypt IP certificates |
| 318 | [qiyeren/dsh-eac-popup](https://github.com/qiyeren/dsh-eac-popup) | 1 | 2026-08-27 | 2026-08-27 | DSH plugin: ???? agent ??/?????,EAC ????(??????)+?????5?+?????? |
| 319 | [Raiyan007-gb/dsh-remote-tunnel-easy](https://github.com/Raiyan007-gb/dsh-remote-tunnel-easy) | 1 | 2026-08-28 | 2026-08-29 | DSH plugin bundle: scan a QR to open the deepseek-harness web UI on your phone inside the same session - cloudflared quick tunnel, no database, Windows/macOS/Linux |
| 320 | [ramen-ai-dev/dsh-ramen-guard](https://github.com/ramen-ai-dev/dsh-ramen-guard) | 1 | 2026-08-27 | 2026-08-27 | Fail-closed DeepSeek Harness guard enforcing ramen-ai Core IT policy before tool execution. |
| 321 | [Raphaelutumn/dsh-mood](https://github.com/Raphaelutumn/dsh-mood) | 1 | 2026-08-27 | 2026-08-27 | A tiny behavioral mood ring for your AI coding agent: a four-state session-header status light (GOOD/CONFUSED/FRUSTRATED/OVERWHELMED) for DeepSeek Harness |
| 322 | [RGarvel/dsh-channel-spec](https://github.com/RGarvel/dsh-channel-spec) | 1 | 2026-08-27 | 2026-08-27 | RFC: 按来源渠道对 DSH 会话分类展示（session header channel 字段 + GUI 渠道视图）— 源自 deepseek-harness discussion #3897 |
| 323 | [RGarvel/dsh-channel-view](https://github.com/RGarvel/dsh-channel-view) | 1 | 2026-08-27 | 2026-08-27 | DSH 渠道会话视图 spike：侧边栏 Channels tab 注入 + 会话投影数据链（RFC-0001, discussion #3897） |
| 324 | [rongxingda/dsh-prompt-enhance](https://github.com/rongxingda/dsh-prompt-enhance) | 1 | 2026-08-29 | 2026-08-29 | Prompt enhancement plugin for the DeepSeek Harness web GUI: one-click rewrite of the composer draft into a structured prompt, with preview, fill-back, and undo. |
| 325 | [runfali/dsh-prompt-injector](https://github.com/runfali/dsh-prompt-injector) | 1 | 2026-08-27 | 2026-08-27 | dsh 通用每轮上下文注入插件：设置页管理提示词清单，每轮对话把每条启用提示词以「上下文注入」提醒行注入模型上下文，让纪律规则（例如 图谱消费/wiki 先查/记忆召回）可靠生效。 |
| 326 | [SA1992X/dsh-ctrl-enter-submit](https://github.com/SA1992X/dsh-ctrl-enter-submit) | 1 | 2026-08-25 | 2026-08-27 | 轻松换行 |
| 327 | [sakthiveltofficial/dsh-shopify-plugins](https://github.com/sakthiveltofficial/dsh-shopify-plugins) | 1 | 2026-08-26 | 2026-08-27 | Shopify plugin for DeepSeek Harness: 213 model-facing shopify_* tools over the Shopify Admin REST + GraphQL APIs (products, orders, customers, inventory, fulfillments, discounts, content, webhooks, themes, billing, bulk operations) with Admin API access-token auth. |
| 328 | [Shaky77/KISS_Law-DSH](https://github.com/Shaky77/KISS_Law-DSH) | 1 | 2026-08-19 | 2026-08-27 | Weiwen's Law (KISS-Law) — a domain-agnostic causal-constraint middleware for DeepSeek Harness. A faithful, white-box presentation of how causal law actually runs. White-box audit, never prediction. Hard-gate the boundary; inner H decides freely. |
| 329 | [shaomingbo/dsh-subscription-search](https://github.com/shaomingbo/dsh-subscription-search) | 1 | 2026-08-19 | 2026-08-30 | ChatGPT/Grok subscription OAuth, model routes, and ChatGPT to Grok to Exa to DeepSeek web-search fallback for DeepSeek Harness |
| 330 | [ShinonomeAya/dsh-git-chain](https://github.com/ShinonomeAya/dsh-git-chain) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: Cursor-style Git commit-chain graph with SVG lanes, commit details, diff, filtering, and guarded branch switching. |
| 331 | [Shonean/deepseek-harness-vscode-desktop](https://github.com/Shonean/deepseek-harness-vscode-desktop) | 1 | 2026-08-27 | 2026-08-27 | Enhanced VS Code extension + Desktop app for DeepSeek Harness (DSH): inline diff, @mentions, selection context, approval UI, plan mode, global shortcut. Claude Code-grade experience. Unofficial community project. |
| 332 | [SleepEggTart/dsh-code-coverage](https://github.com/SleepEggTart/dsh-code-coverage) | 1 | 2026-08-26 | 2026-08-27 | 解析 DSH session 日志归因 AI 生成文件，叠加 c8 覆盖率，产出 AI vs 人工代码覆盖率对比、高危未测文件清单与信任分。 |
| 333 | [SleepEggTart/dsh-dev-wrapped](https://github.com/SleepEggTart/dsh-dev-wrapped) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (DSH) 开发者使用报告——类 Spotify Wrapped，统计与 AI 结对编程的行为，生成可分享报告卡片 |
| 334 | [softspark/dsh-codex](https://github.com/softspark/dsh-codex) | 1 | 2026-08-25 | 2026-08-27 | DeepSeek Harness provider for locally authenticated Codex app-server access through a ChatGPT subscription. |
| 335 | [starefinger/dsh-llm-qwen-local](https://github.com/starefinger/dsh-llm-qwen-local) | 1 | 2026-08-26 | 2026-08-27 | 面向 DeepSeek Harness(dsh)的 LLM 适配器插件:驱动由 OpenAI 兼容服务的本地部署 Qwen3.8-27B 模型。支持按模型多模态开关、完全可配置的推理档位、请求图像投影,以及中英双语 Web 设置页。 |
| 336 | [summer-521/deepseek-harness-swift](https://github.com/summer-521/deepseek-harness-swift) | 1 | 2026-08-25 | 2026-08-28 | 基于 AppKit、SwiftUI 与 WKWebView 的 DSH 原生 macOS 桌面壳，提供设置中心、DSH 版本管理、插件管理、通知和 Sparkle 应用更新。 |
| 337 | [Sunday2Mo/dsh-file-quote](https://github.com/Sunday2Mo/dsh-file-quote) | 1 | 2026-08-27 | 2026-08-27 | 基于 better-sidebar 的统一引用插件：划选文件/消息即可批注引用，引用块带文件路径与行区间、双端折叠、点击跳回原文 ｜ Unified-quoting plugin built on DSH-better-sidebar: select files or messages to annotate; quote blocks carry path & line range, collapse in chat and history, and jump back to the source on click. |
| 338 | [supersyh-sss/dsh-voice-assistant](https://github.com/supersyh-sss/dsh-voice-assistant) | 1 | 2026-08-29 | 2026-08-30 | Offline voice assistant for dsh web — wake word, speech dictation, voice edit commands & Chinese TTS. On-device sherpa-onnx WASM ASR, no Google dependency, works in China. |
| 339 | [svgop/dsh-rich-questions](https://github.com/svgop/dsh-rich-questions) | 1 | 2026-08-26 | 2026-08-29 | Rich branching survey system for DeepSeek Harness (DSH) Web GUI — ask_survey tool with branch graphs, delayed hover insights, Mermaid diagrams, quick mode, reroll/push/discuss actions |
| 340 | [sycamorestr/dsh-platform-account-manager-plugin](https://github.com/sycamorestr/dsh-platform-account-manager-plugin) | 1 | 2026-08-29 | 2026-08-29 | DSH platform account and persistent browser-session manager |
| 341 | [taoser258/dsh-client-ui-skin-qingxiao](https://github.com/taoser258/dsh-client-ui-skin-qingxiao) | 1 | 2026-08-29 | 2026-08-29 | 清宵 · 弦凝清霄 —— DeepSeek Harness (DSH) Web 界面美化皮肤：以《鸣潮》角色清宵为灵感的冰蓝·青碧·月白·玄夜调色板，含可换背景画卷、剑气流光粒子、磨砂玻璃面板与新会话迎宾页。A Qingxiao (Wuthering Waves) themed client UI skin for the DSH web GUI. |
| 342 | [TestTheBoy/dsh_plugin_file_attach](https://github.com/TestTheBoy/dsh_plugin_file_attach) | 1 | 2026-08-26 | 2026-08-27 | Add files to context |
| 343 | [tiger0012/dsh-we-wallpaper-sync](https://github.com/tiger0012/dsh-we-wallpaper-sync) | 1 | 2026-08-26 | 2026-08-27 | Reusable skill: browse/search/download Wallpaper Engine (Steam 431960) workshop wallpapers and wire them into the DSH skin center, bypassing the Steam HTTP block and region-mismatch sign-in block. |
| 344 | [Tkingxiao/dsh-novel-solo](https://github.com/Tkingxiao/dsh-novel-solo) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的「单核写作」插件：面向量化小模型做了充分的工具瘦身与输出加固，适合在本机用本地模型跑长篇小说流水线。 |
| 345 | [trrrrrryg/dsh-ssh-forge](https://github.com/trrrrrryg/dsh-ssh-forge) | 1 | 2026-08-24 | 2026-08-27 | DSH SSH Forge：为 DeepSeek Harness（DSH）提供 SSH 远程工作区能力：已核验的服务器身份、失败关闭的 Agent 执行路由、远端文件与命令操作；提供 Windows 离线一键安装包，无需 Node.js 或构建工具。 |
| 346 | [Tsqurt/dsh-plugin-studio](https://github.com/Tsqurt/dsh-plugin-studio) | 1 | 2026-08-27 | 2026-08-28 | 为了开发插件，开发了一个开发插件的插件。通过可视化的事件流、插件管理、工具管理、技能管理、预设管理，简化插件的开发流程，方便开发者理解插件的作用。 |
| 347 | [tyx6661234/dsh-community-listening](https://github.com/tyx6661234/dsh-community-listening) | 1 | 2026-08-26 | 2026-08-27 | 面向 DeepSeek Harness (DSH) 的社交评论研究插件 |
| 348 | [UNscientific-9/dsh-turnfold](https://github.com/UNscientific-9/dsh-turnfold) | 1 | 2026-08-27 | 2026-08-27 | DSH Web 轮次折叠插件：thinking/工具调用流式可见，turn 完成后自动收纳成一行摘要。 |
| 349 | [Urbanrook/agent-project-manager](https://github.com/Urbanrook/agent-project-manager) | 1 | 2026-08-28 | 2026-08-28 | A DeepSeek Harness plugin providing project workspace isolation: each project (task) maps to its own workspace and conversation, preventing rules, memory, and context from leaking across projects — so multiple projects can progress in parallel. |
| 350 | [v587d/dsh-custom-skin](https://github.com/v587d/dsh-custom-skin) | 1 | 2026-08-28 | 2026-08-28 | 自己的插件皮肤管理工具。 |
| 351 | [VioletScar-Hui/trcost-plugin](https://github.com/VioletScar-Hui/trcost-plugin) | 1 | 2026-08-28 | 2026-08-28 | 轨迹省钱优化器：DSH 会话轨迹 token 浪费分析 + waterfall 执行层强制拦截/截断。Trajectory cost optimizer with enforcement layer for DeepSeek Harness. |
| 352 | [wang-kaopu/dsh-cordis-devtools](https://github.com/wang-kaopu/dsh-cordis-devtools) | 1 | 2026-08-23 | 2026-08-27 | Give coding Agents runtime evidence for debugging and verifying DSH / Cordis plugins. 让 Coding Agent 获得用于调试和验证 DSH / Cordis 插件的运行时证据。 |
| 353 | [warment/deepseek-harness-locale-ru](https://github.com/warment/deepseek-harness-locale-ru) | 1 | 2026-08-30 | 2026-08-30 | Русский язык для DeepSeek Harness web UI — one-command install, 1061 строка, 100% покрытие |
| 354 | [Washington5533/guarftrain](https://github.com/Washington5533/guarftrain) | 1 | 2026-08-09 | 2026-08-27 | 🛡️ 一行命令，训练脚本零行改动，获得完整守护能力。GPU 监控 · 崩溃恢复 · OOM 自救 · Agent 决策 · MCP 35 工具 · Web Dashboard。 |
| 355 | [wenyixiaoqingnian/screenshot-review](https://github.com/wenyixiaoqingnian/screenshot-review) | 1 | 2026-08-29 | 2026-08-29 | dsh skill: 截图审阅——模型自己截图、自己看图、自己改代码，迭代优化前端效果 |
| 356 | [WesleyJay/dsh-weather](https://github.com/WesleyJay/dsh-weather) | 1 | 2026-08-27 | 2026-08-28 | 一个 DSH 天气查询插件，让 AI 智能体可以查询全球城市的实时天气和天气预报 |
| 357 | [wodongx123/dsh-qq-notify](https://github.com/wodongx123/dsh-qq-notify) | 1 | 2026-08-17 | 2026-08-27 | QQ notifications via local NapCat for DeepSeek Harness: qq_send / qq_status / qq_napcat / qq_deploy native tools + one-click deploy scripts. QQ???? |
| 358 | [wp-a/dsh-academic-paper-search](https://github.com/wp-a/dsh-academic-paper-search) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 的中文学术论文检索 Bundle：复用 Academic Paper Search MCP，支持多源检索去重、引用核验、引文图谱、MeSH、试验检索与审计导出。 |
| 359 | [WSL043/dsh-deepseek-dashboard](https://github.com/WSL043/dsh-deepseek-dashboard) | 1 | 2026-08-24 | 2026-08-27 | DeepSeek Harness 的 DeepSeek API 余额与本地用量面板：请求、Token、缓存和模型统计。 |
| 360 | [wszhoho/dsh-file-attachment](https://github.com/wszhoho/dsh-file-attachment) | 1 | 2026-08-28 | 2026-08-28 | 拖入 / 粘贴 / 工具栏上传按钮（↑，可多选、移动端支持拍照）为输入框附加文件：图片走既有草稿图片流程（不落盘）；文档全文落盘到会话工作区 .dsh-file-attachment/ 并插入 @绝对路径引用 |
| 361 | [wtksana/dsh-font-plugin](https://github.com/wtksana/dsh-font-plugin) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Font Plugin, DSH 字体插件 |
| 362 | [xiaochaZ/dsh-session-title-summary](https://github.com/xiaochaZ/dsh-session-title-summary) | 1 | 2026-08-25 | 2026-08-27 | DSH plugin: rolling session summary + current-task title (@xiaochaz) |
| 363 | [xiaoguomeiyitian/dsh-qr-share](https://github.com/xiaoguomeiyitian/dsh-qr-share) | 1 | 2026-08-29 | 2026-08-30 | DSH web plugin: a sidebar-footer QR-code button that lets a phone scan and re-issue the current browser's authenticated launch URL. |
| 364 | [xiaoshi7915/dsh-kb-manager](https://github.com/xiaoshi7915/dsh-kb-manager) | 1 | 2026-08-27 | 2026-08-27 | DSH local knowledge base plugin: multi-format import, smart chunking, vector index, hybrid search (BM25 + sqlite-vec + RRF) for agent long-term memory |
| 365 | [xiaozuishuai-eng/prompt_optimize_dsh](https://github.com/xiaozuishuai-eng/prompt_optimize_dsh) | 1 | 2026-08-30 | 2026-08-30 | DeepSeek Harness (DSH) 提示词优化器插件：一句口语化需求 → 结构化高质量提示词，结果自动填入会话输入框。复用 DSH 内置模型路由，零 API Key 管理。 |
| 366 | [Xichun123/dsh-relay-models](https://github.com/Xichun123/dsh-relay-models) | 1 | 2026-08-14 | 2026-08-29 | Mixed-protocol relay model discovery, metadata matching, and Web configuration for DeepSeek Harness |
| 367 | [xjailll/dsh-portfolio-publisher](https://github.com/xjailll/dsh-portfolio-publisher) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 插件：GitHub 求职仓库一键发布助手（LLM README + Web 面板 + 一键推送） |
| 368 | [xmnathan/dsh-skin-galactic-opera](https://github.com/xmnathan/dsh-skin-galactic-opera) | 1 | 2026-08-27 | 2026-08-27 | Unofficial cinematic space-opera dark skin bundle for the DSH Web GUI. |
| 369 | [XSakura666/dsh-plugin-ChronoAgent](https://github.com/XSakura666/dsh-plugin-ChronoAgent) | 1 | 2026-08-15 | 2026-08-27 | Local-first desktop app that schedules AI agent tasks like cron jobs — zero token cost until they run. Write a task, set a time, and it runs automatically with files, web, MCP tools, and multi-model support.      |
| 370 | [yakoylp/dsh-md-convert](https://github.com/yakoylp/dsh-md-convert) | 1 | 2026-08-28 | 2026-08-28 | Convert Office documents and PDFs (incl. scanned, via CPU-first routing OCR with lightweight models: PP-DocLayout-L layout, RapidOCR text, SLANet tables, FormulaNet formulas) to structurally-formatted Markdown. CLI + dsh agent tool (md_convert). |
| 371 | [Yang-wudi/dsh-video-gen](https://github.com/Yang-wudi/dsh-video-gen) | 1 | 2026-08-26 | 2026-08-29 | Bring text-to-video and image-to-video generation to DeepSeek Harness — DashScope Wanx, Volcengine/Doubao Seedance, Google Veo, OpenAI Sora & compatible relays. |
| 372 | [yangbobo2021/relay-dsh-plugin-manager](https://github.com/yangbobo2021/relay-dsh-plugin-manager) | 1 | 2026-08-26 | 2026-08-27 | A standalone plugin manager for DeepSeek Harness. |
| 373 | [Ycet/dsh-awesome-hud](https://github.com/Ycet/dsh-awesome-hud) | 1 | 2026-08-29 | 2026-08-30 | dsh侧边HUD面板，包含多个信息展示模块（可自定义是否展示），集成压缩上下文、查看git graph等功能。DSH side HUD panel, containing multiple information display modules (customizable whether to display), integrating features such as compressed context, viewing git graph, etc. |
| 374 | [YINGCHAO-98/dsh-private-plugins](https://github.com/YINGCHAO-98/dsh-private-plugins) | 1 | 2026-08-25 | 2026-08-27 | 在 DeepSeek Harness Web 设置中统一导入、启用、更新和管理本地及云端私有插件。 |
| 375 | [yj-liuzepeng/dsh-project-brain](https://github.com/yj-liuzepeng/dsh-project-brain) | 1 | 2026-08-30 | 2026-08-30 | Persistent project intelligence and memory plugin for DSH: architecture analysis, cross-session context, TODOs, and optional hybrid retrieval |
| 376 | [yongshuai0314/dsh-i-have-adhd](https://github.com/yongshuai0314/dsh-i-have-adhd) | 1 | 2026-08-26 | 2026-08-27 | ADHD-friendly output shaping for DeepSeek Harness: one system-prompt section with adhd_on/adhd_off/adhd_status tools, persisted across restarts. Inspired by ayghri/i-have-adhd (MIT). |
| 377 | [yuan-source-666/dsh-github-manager](https://github.com/yuan-source-666/dsh-github-manager) | 1 | 2026-08-27 | 2026-08-27 | GitHub 仓库 AI 自动管理通道插件 (DeepSeek Harness community bundle): 27 个工具（仓库/Issue/PR/分支/文件/标签/话题/Tags/Releases/搜索）+ Web 设置卡片 + dry-run 防护 + secret 令牌。 |
| 378 | [yuan-source-666/dsh-research-autoresearch](https://github.com/yuan-source-666/dsh-research-autoresearch) | 1 | 2026-08-27 | 2026-08-27 | AutoResearch 科研协议 DSH 全家桶插件：arXiv recall + LQS 评分 + 状态持久化 + 停滞红绿灯 + 五人格中位数评审 + 可视化总控台卡片。灵感：Deli Chen "From Draft to Strong-Accept: How a Self-Play Survey Hit 8.6"。 |
| 379 | [yuan-source-666/dsh-task-notifier](https://github.com/yuan-source-666/dsh-task-notifier) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness community plugin: OS notification when a turn, subagent, background job, goal, or workflow finishes. Localized wording, per-source switches, custom delivery command. npm: dsh-task-notifier |
| 380 | [yunniees/DSH-Plugin-Manager](https://github.com/yunniees/DSH-Plugin-Manager) | 1 | 2026-08-28 | 2026-08-28 | Visual plugin manager for DeepSeek Harness: AI auto-translation, AI one-click summaries, AI plugin search, one-click share & install of multiple plugins, bulk updates |
| 381 | [yx222yx/DSH-Feedback-Bridge](https://github.com/yx222yx/DSH-Feedback-Bridge) | 1 | 2026-08-29 | 2026-08-30 | 一个 DeepSeek Harness 插件，帮助用户将功能想法和错误反馈整理为清晰、注重隐私的 GitHub Discussions。A DeepSeek Harness plugin that helps users turn ideas and bug reports into clear, privacy-aware GitHub Discussions. |
| 382 | [yyyq0325-ai/dsh-webgate](https://github.com/yyyq0325-ai/dsh-webgate) | 1 | 2026-08-22 | 2026-08-27 | 为 DeepSeek Harness 的 Web GUI 加一道账号密码门：每次打开 DSH Web 都必须先登录；登录令牌有效期 12 小时；令牌过期被登出时，后台正在运行的任务完全不受影响，重新登录后一切还在。 |
| 383 | [yztdtf/dsh-worktable-pet](https://github.com/yztdtf/dsh-worktable-pet) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness ??????????(Dynamic Cordis Plugin) |
| 384 | [Zara-Siwei/dsh-float](https://github.com/Zara-Siwei/dsh-float) | 1 | 2026-08-26 | 2026-08-27 | Floating minimal-mode DeepSeek Harness (dsh) plugin: a transparent terminal TUI over dsh web in a borderless Electron window. |
| 385 | [zhangyqjiaoshou-oss/dsh-model-sync](https://github.com/zhangyqjiaoshou-oss/dsh-model-sync) | 1 | 2026-08-29 | 2026-08-29 | One-click / auto model sync for DeepSeek Harness providers |
| 386 | [Zhanxueyou/deepseek-balance](https://github.com/Zhanxueyou/deepseek-balance) | 1 | 2026-08-30 | 2026-08-30 | 零依赖 Python CLI 查询 DeepSeek API 余额，低余额自动提醒并发送 macOS 通知；附带 DSH 侧边栏插件，实时展示余额、今日/本月用量与缓存命中率。 |
| 387 | [Zhanxueyou/dsh-plugin-manager](https://github.com/Zhanxueyou/dsh-plugin-manager) | 1 | 2026-08-30 | 2026-08-30 | DSH Web 客户端插件管理器侧边栏面板：全量插件清单（描述/状态/来源/版本/分类）、启停热重载、删除本地自定义插件，并可浏览、搜索、一键安装 GitHub topic:dsh-plugin 远程插件。 |
| 388 | [zhaoxuejie/dsh-daily-digest](https://github.com/zhaoxuejie/dsh-daily-digest) | 1 | 2026-08-27 | 2026-08-27 | DSH 每日工作摘要插件：自动记录任务/会话/错误，一键生成日报/周报 Markdown，Web 悬浮摘要卡 |
| 389 | [zhaoxuejie/dsh-plugin-learning-path](https://github.com/zhaoxuejie/dsh-plugin-learning-path) | 1 | 2026-08-21 | 2026-08-27 | DeepSeek Harness 插件开发学习教程：15 节课程 + 4 个实战项目 + 发布课，交互式单页应用，纯 HTML/CSS/JS 零构建 |
| 390 | [Zhiyi-Zhao/dsh-notion-skill](https://github.com/Zhiyi-Zhao/dsh-notion-skill) | 1 | 2026-08-27 | 2026-08-27 | DSH (DeepSeek Harness) skill: read/write Notion workspaces via the official REST API |
| 391 | [Zhiyi-Zhao/file-brief](https://github.com/Zhiyi-Zhao/file-brief) | 1 | 2026-07-30 | 2026-08-27 | Task-local, privacy-preserving file catalogs for reusable Codex input-file understanding. |
| 392 | [zhongjie10086/dsh-adaptive-native](https://github.com/zhongjie10086/dsh-adaptive-native) | 1 | 2026-08-16 | 2026-08-30 | Windows-native Adaptive preset for DeepSeek Harness |
| 393 | [zhoupengyun572-cell/dsh-hana-research](https://github.com/zhoupengyun572-cell/dsh-hana-research) | 1 | 2026-08-28 | 2026-08-28 | A local literature review, PDF annotation, evidence synthesis, and research notes workbench for DeepSeek Harness. |
| 394 | [zhuzichen362/dsh-call-shrink](https://github.com/zhuzichen362/dsh-call-shrink) | 1 | 2026-08-29 | 2026-08-29 | dsh |
| 395 | [zjh02249/dsh-desktop-operator](https://github.com/zjh02249/dsh-desktop-operator) | 1 | 2026-08-27 | 2026-08-27 | DSH Desktop Operator: safe Windows Computer Use, desktop automation, UI Automation, and MCP tools for DeepSeek Harness |
| 396 | [zw11591-sketch/dsh-pet-panel](https://github.com/zw11591-sketch/dsh-pet-panel) | 1 | 2026-08-28 | 2026-08-28 | A desktop pet plus a conversation overview panel for the DeepSeek Harness Web UI — self-contained client plugin (no host service) |
| 397 | [zzy-12345678/dsh-file-convert](https://github.com/zzy-12345678/dsh-file-convert) | 1 | 2026-08-29 | 2026-08-30 | Local-first file conversion for DeepSeek Harness — images, PDF, data, audio/video & office docs. 7 tools, 26 conversions, no API keys, no uploads. |
| 398 | [ZZZjf13960/dsh-onfail](https://github.com/ZZZjf13960/dsh-onfail) | 1 | 2026-08-28 | 2026-08-28 | DSH plugin: poll GitHub Actions, surface failed checks as cards, open a fix session with log context. |
| 399 | [123twtd/dsh-plugin-manager](https://github.com/123twtd/dsh-plugin-manager) | 0 | 2026-08-29 | 2026-08-29 | Independent DSH plugin inventory and transactional Profile manager. |
| 400 | [1Ecc/dsh-lenovo-toolkit](https://github.com/1Ecc/dsh-lenovo-toolkit) | 0 | 2026-08-28 | 2026-08-28 | 联想专业工具集 · DeepSeek Harness 插件。电池健康检测（macOS/Windows）：容量、循环次数、双口径健康度、SVG 衰减趋势图与系统官方电池报告。Lenovo professional toolkit for DeepSeek Harness. |
| 401 | [2877905731/dsh-think-autoexpand](https://github.com/2877905731/dsh-think-autoexpand) | 0 | 2026-08-27 | 2026-08-27 | dsh-think-autoexpand：让 DeepSeek Harness 里的 Think 思考行始终可见，并在流式输出时自动展开，实时查看 Agent 完整推理过程；保留工具卡折叠体验。 |
| 402 | [2DogsLee/dsh_whalebuddy](https://github.com/2DogsLee/dsh_whalebuddy) | 0 | 2026-08-29 | 2026-08-29 | whalebuddy - DeepSeek Harness desktop pet (Windows): a DSH bundle plugin + Tauri shell. A porthole whale reflects your agent live state, with autostart & skin settings. |
| 403 | [452926826/dsh-feishu-bot](https://github.com/452926826/dsh-feishu-bot) | 0 | 2026-08-25 | 2026-08-27 | Connect a Feishu bot to DeepSeek Harness projects and conversations |
| 404 | [618527/dsh-install-guard](https://github.com/618527/dsh-install-guard) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件安装前兼容性预检守卫：检查 Node/engines、@deepseek-ai peer 版本与 dsh 清单，可选隔离试启动。 |
| 405 | [6jeffr3y/dsh-burpsuite-mcp](https://github.com/6jeffr3y/dsh-burpsuite-mcp) | 0 | 2026-08-30 | 2026-08-30 | Native Burp Suite MCP tools and live settings for DeepSeek Harness |
| 406 | [6jeffr3y/dsh-session-manager](https://github.com/6jeffr3y/dsh-session-manager) | 0 | 2026-08-30 | 2026-08-30 | Session archive, tagging, relationship graph and safe deletion for DeepSeek Harness Web |
| 407 | [988hj7tczd-oss/harness-github](https://github.com/988hj7tczd-oss/harness-github) | 0 | 2026-08-23 | 2026-08-27 | DeepSeek Harness GitHub plugin: review PRs, triage issues, debug Actions CI, handle incoming GitHub events (webhooks + polling) via dsh-native tools. |
| 408 | [a1303845406/dsh-comfy-video-studio](https://github.com/a1303845406/dsh-comfy-video-studio) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的 ComfyUI MiniMax H3 视频工作台 |
| 409 | [a1303845406/dsh-sakura-theme](https://github.com/a1303845406/dsh-sakura-theme) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的晴樱与夜樱主题插件 |
| 410 | [aalvsz/dsh-hermes-bridge](https://github.com/aalvsz/dsh-hermes-bridge) | 0 | 2026-08-27 | 2026-08-27 | Literal Hermes Agent → DeepSeek Harness bridge: shared memory, skills, live tools, MCP, and full-agent delegation. |
| 411 | [abbccdd/dsh-localtts](https://github.com/abbccdd/dsh-localtts) | 0 | 2026-08-28 | 2026-08-29 | Local IndexTTS 2.5 and GPT-SoVITS speech synthesis and playback for DeepSeek Harness. |
| 412 | [ABccgh/dsh-desktop-dev](https://github.com/ABccgh/dsh-desktop-dev) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness agent preset: Windows full-stack desktop development team |
| 413 | [adoreQ/deepseek-balance](https://github.com/adoreQ/deepseek-balance) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness查看余额插件 |
| 414 | [Aetheri-AI/dsh-plugins](https://github.com/Aetheri-AI/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | Community plugins for DeepSeek Harness (dsh) |
| 415 | [aiko-dsh-plugins/dsh-bid-studio](https://github.com/aiko-dsh-plugins/dsh-bid-studio) | 0 | 2026-08-29 | 2026-08-29 | Installable Bid Studio workbench for DeepSeek Harness |
| 416 | [aiko-dsh-plugins/dsh-ontology-kernel](https://github.com/aiko-dsh-plugins/dsh-ontology-kernel) | 0 | 2026-08-29 | 2026-08-29 | Installable Ontology Kernel bundle for DeepSeek Harness |
| 417 | [ailiasdesu/dsh-session-manager](https://github.com/ailiasdesu/dsh-session-manager) | 0 | 2026-08-28 | 2026-08-28 | DSH session migration plugin: drag-and-drop sessions between workspaces in the Web UI settings panel (auto backup/rollback, official workspaceRegistry sync) |
| 418 | [aiyacharley/dsh-pubmed](https://github.com/aiyacharley/dsh-pubmed) | 0 | 2026-08-27 | 2026-08-27 | 把 pubmed-mcp-server 的核心能力 移植成 DSH 原生模型工具：搜索、文章元数据、全文、引用格式化、MeSH、ID 转换等 11 个工具， 直接对接 NCBI E-utilities 与 Europe PMC REST，无需额外的 MCP 客户端配置。 |
| 419 | [AKUSH99/dsh-balance-chip](https://github.com/AKUSH99/dsh-balance-chip) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek API balance in the DSH sidebar footer and bottom-right pill - live status dot plus amount, 60s refresh, API key stays in the local credential store |
| 420 | [alaxrpg/dsh-chatgpt-pip](https://github.com/alaxrpg/dsh-chatgpt-pip) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：ChatGPT 画中画小窗 + 把 ChatGPT 定稿计划回流到新 DSH 对话执行 |
| 421 | [alaxrpg/dsh-subagent-route-badges](https://github.com/alaxrpg/dsh-subagent-route-badges) | 0 | 2026-08-27 | 2026-08-27 | Display subagent provider, model, and reasoning effort badges in DeepSeek Harness |
| 422 | [alaxrpg/dsh-vision-bridge](https://github.com/alaxrpg/dsh-vision-bridge) | 0 | 2026-08-25 | 2026-08-27 | DSH 插件：为纯文本模型提供视觉能力，支持任意 OpenAI 兼容多模态 API |
| 423 | [Albertlsy588/dsh-shipgate](https://github.com/Albertlsy588/dsh-shipgate) | 0 | 2026-08-28 | 2026-08-28 | Local-first DSH pre-merge delivery receipt generator |
| 424 | [AlgoVaultLabs/dsh-algovault](https://github.com/AlgoVaultLabs/dsh-algovault) | 0 | 2026-08-30 | 2026-08-30 | Preconfigured DeepSeek Harness bundle for the AlgoVault MCP server — composite trade calls, market regime and cross-venue funding arbitrage as mcp__algovault__* tools. |
| 425 | [alin-ever/dsh-plugin-autoqueue](https://github.com/alin-ever/dsh-plugin-autoqueue) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 无人值守任务队列插件：丢 .md 进收件箱 → AI 自动执行 → 产出报告 |
| 426 | [alpacachen/dsh-automation](https://github.com/alpacachen/dsh-automation) | 0 | 2026-08-30 | 2026-08-30 | Schedule and manage one-time and recurring Agent tasks in DeepSeek Harness |
| 427 | [Amoss-1/routine-taskboard](https://github.com/Amoss-1/routine-taskboard) | 0 | 2026-08-27 | 2026-08-28 | Self-contained routine board plugin for DeepSeek Harness (DSH): scheduled job placards with scripts, IO artifacts, health lamps. MIT. |
| 428 | [AnakinWu/DSH-plugin](https://github.com/AnakinWu/DSH-plugin) | 0 | 2026-08-30 | 2026-08-30 | Anakin‘s dsh-plugins |
| 429 | [andrepontesmelo/dsh-model-router](https://github.com/andrepontesmelo/dsh-model-router) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: virtual model routes with failover, exponential backoff, sleep windows |
| 430 | [andrepontesmelo/dsh-suite](https://github.com/andrepontesmelo/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | The DSH productivity suite: plugins + agent skills for the DeepSeek Harness, installable in one command. |
| 431 | [andrepontesmelo/moving-target](https://github.com/andrepontesmelo/moving-target) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: cold-start context — distills your first prompts into one goal paragraph injected into every new session |
| 432 | [AndyWipe13/dsh-session-management](https://github.com/AndyWipe13/dsh-session-management) | 0 | 2026-08-30 | 2026-08-30 | A plugin for managing sessions generated by DeepSeek Harness, allowing users to freely delete legacy sessions and supporting session import from other third-party Agents (Claude Code, Codex). |
| 433 | [Anna-la/dsh-simplify](https://github.com/Anna-la/dsh-simplify) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 界面简化插件：清理模式下右键移除页面元素，设置页中可原样恢复。 |
| 434 | [Anna-la/dsh-submodel-change](https://github.com/Anna-la/dsh-submodel-change) | 0 | 2026-08-27 | 2026-08-29 | 可以选择子 agent 调用的模型。 |
| 435 | [Anna-la/dsh-token-stat](https://github.com/Anna-la/dsh-token-stat) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness token 用量统计插件: 按模型/日期区分, 设置页看板, 数据目录在线更改 |
| 436 | [AnonyJcy/dsh-plugin-j-space](https://github.com/AnonyJcy/dsh-plugin-j-space) | 0 | 2026-08-23 | 2026-08-27 | J-Space Cognition Suite V3.7 原生 DeepSeek Harness 智能体预设与独立 Cordis 插件，提供深层推理路由、工作区状态外化账本（.jspace）与全模型解耦的认知工作空间 |
| 437 | [AnonyJcy/dsh-plugin-mobile-touch](https://github.com/AnonyJcy/dsh-plugin-mobile-touch) | 0 | 2026-08-27 | 2026-08-28 | Mobile & iPad touch optimization plugin for DeepSeek Harness Web GUI |
| 438 | [Ansonfishing/dsh-model-manager](https://github.com/Ansonfishing/dsh-model-manager) | 0 | 2026-08-28 | 2026-08-28 | Manage local LLM inference servers in DSH: GPU registry, parameter profiles, VRAM validation, and tok/s benchmarks for llama.cpp, SGLang, and vLLM |
| 439 | [Anyway-one/dsh-balance](https://github.com/Anyway-one/dsh-balance) | 0 | 2026-08-26 | 2026-08-27 | 为 DeepSeek Harness 提供持久化的余额与用量显示插件，让您随时掌握资源消耗情况，无需离开工作区。 |
| 440 | [Army1900/dsh-e2e-dev-sdd](https://github.com/Army1900/dsh-e2e-dev-sdd) | 0 | 2026-08-26 | 2026-08-27 | dsh插件，用于驱动定制的e2e开发 |
| 441 | [asdasdsdsdasdasdasd/dsh-computer-use](https://github.com/asdasdsdsdasdasdasd/dsh-computer-use) | 0 | 2026-08-25 | 2026-08-29 | Linux X11 computer-use for DeepSeek Harness: screenshot, mouse, keyboard via a zero-dependency Python XTest helper — no Node native modules, no accessibility framework. |
| 442 | [AstralFoundry/dsh-workspace](https://github.com/AstralFoundry/dsh-workspace) | 0 | 2026-08-27 | 2026-08-27 | A lightweight IDE and Git workspace plugin for DeepSeek Harness |
| 443 | [auggie246/dsh-mattpocock-skills](https://github.com/auggie246/dsh-mattpocock-skills) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to install Mattpocock skills. |
| 444 | [auggie246/dsh-output-styles](https://github.com/auggie246/dsh-output-styles) | 0 | 2026-08-28 | 2026-08-28 | Enable output styles in Deepseek Harness settings! |
| 445 | [auggie246/dsh-sidebar](https://github.com/auggie246/dsh-sidebar) | 0 | 2026-08-27 | 2026-08-28 | Sidebar and panels for full developer interaction! |
| 446 | [auggie246/dsh-synthetic-web-search](https://github.com/auggie246/dsh-synthetic-web-search) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to use synthetic.new web search instead of built-in Deepseek web search |
| 447 | [avdergh/chroma-cut](https://github.com/avdergh/chroma-cut) | 0 | 2026-08-28 | 2026-08-28 | Preserve anti-aliased outlines while cutting chroma-backed game assets. CLI + MCP + Codex plugin. |
| 448 | [awol2005ex3/dsh-md-table-export](https://github.com/awol2005ex3/dsh-md-table-export) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（`dsh`）插件：把对话内容里的 **Markdown 表格** 一键导出为 **Excel（`.xlsx`）**。 |
| 449 | [awol2005ex3/dsh-role-manager](https://github.com/awol2005ex3/dsh-role-manager) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（dsh）角色管理插件。为每个"角色"预设一份初始系统提示词，在 Web 界面中切换当前角色，从而让模型以不同的身份 / 设定开始对话。 |
| 450 | [ayumedaze/dsh-git](https://github.com/ayumedaze/dsh-git) | 0 | 2026-08-29 | 2026-08-29 | dsh-plugin |
| 451 | [baiyang123/dsh-audit-missing](https://github.com/baiyang123/dsh-audit-missing) | 0 | 2026-08-27 | 2026-08-28 | 对照开发计划等文档，当AI开发完一个迭代之后扫描是否有漏开发的功能（真的好用） |
| 452 | [BaoBao1996121/dsh-restart-ui](https://github.com/BaoBao1996121/dsh-restart-ui) | 0 | 2026-08-28 | 2026-08-28 | One-click cross-platform restart button for DeepSeek Harness Web UI |
| 453 | [BaronCyrus/dsh-kimi-subscription](https://github.com/BaronCyrus/dsh-kimi-subscription) | 0 | 2026-08-28 | 2026-08-28 | Use a Kimi Code subscription in DeepSeek Harness with OAuth, quota display, and composer usage |
| 454 | [BarrierFly/apx-watchdog](https://github.com/BarrierFly/apx-watchdog) | 0 | 2026-08-26 | 2026-08-27 | 牛来写的东西 |
| 455 | [Barry-Liu-001/dsh_ark_plan_usage](https://github.com/Barry-Liu-001/dsh_ark_plan_usage) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 侧边栏插件：实时展示火山方舟 Agent Plan 用量（5h/周/月），数据来自本机 arkcli |
| 456 | [Barry-Liu-001/dsh_chat_index](https://github.com/Barry-Liu-001/dsh_chat_index) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 对话索引插件：在对话区右边缘显示一列小圆点，每个点代表一条用户发送的消息。圆点等间距、紧凑、纵向居中排列（消息过多放不下时间距自动压缩以适应高度）；当前阅读位置的点高亮为品牌色。 |
| 457 | [bbboy31/dsh-terminal-tabs](https://github.com/bbboy31/dsh-terminal-tabs) | 0 | 2026-08-26 | 2026-08-27 | Terminals view tab for DeepSeek Harness web UI — live background job count, streaming output, one-click kill |
| 458 | [benz-ai-x/dsh-session-graph](https://github.com/benz-ai-x/dsh-session-graph) | 0 | 2026-08-28 | 2026-08-30 | Visual session graph for DeepSeek Harness — browse, arrange, branch, merge, and summarize AI agent sessions on an interactive canvas. |
| 459 | [berserk0501/dsh-soundscape](https://github.com/berserk0501/dsh-soundscape) | 0 | 2026-08-26 | 2026-08-27 | DSH 本机思考与工具音效插件，支持 MediaPlayer、WAV/MP3、自定义映射和设置面板 |
| 460 | [Bigesila-B/dsh-media-forge](https://github.com/Bigesila-B/dsh-media-forge) | 0 | 2026-08-26 | 2026-08-27 | DSH Media Forge plugin: agent + skills workflow for media-generation APIs, with a sidebar skill panel (zh/en docs) |
| 461 | [BISTU-guheihei/DSH-SessionManager](https://github.com/BISTU-guheihei/DSH-SessionManager) | 0 | 2026-08-26 | 2026-08-27 | DSH 会话管理工具：可视化/命令行查看与删除历史聊天记录，自动清理缓存残留 |
| 462 | [bitterSmilezzz/dsh-asr-voice](https://github.com/bitterSmilezzz/dsh-asr-voice) | 0 | 2026-08-25 | 2026-08-27 | 开口即成文 · Speak-to-prompt for DeepSeek Harness：云端 ASR 语音识别 + 提示词优化 + 填入草稿/自动发送，跨平台 macOS / Windows。 |
| 463 | [bjzkhy/dsh-token-ledger-pro](https://github.com/bjzkhy/dsh-token-ledger-pro) | 0 | 2026-08-30 | 2026-08-30 | DSH cost panel: meters every request from session events, prices it against a built-in catalog of 136 models across 16 providers, and shows model, balance, session/today/month spend and a monthly budget bar next to the composer. |
| 464 | [bleakbelladonnals/dsh-artifact-harbor](https://github.com/bleakbelladonnals/dsh-artifact-harbor) | 0 | 2026-08-27 | 2026-08-27 | Artifact Harbor — secure, session-aware artifact previews for DeepSeek Harness Web |
| 465 | [bleakbelladonnals/dsh-echo](https://github.com/bleakbelladonnals/dsh-echo) | 0 | 2026-08-27 | 2026-08-27 | Record MCP once. Replay it safely inside DeepSeek Harness. |
| 466 | [bleamayaka/dsh-file-beam](https://github.com/bleamayaka/dsh-file-beam) | 0 | 2026-08-27 | 2026-08-27 | dsh-file-beam - DSH plugin: drag files into the web composer, resolve real absolute paths, hidden path injection for the agent (no copy, no path in composer). |
| 467 | [bLueriVerLHR/dsh-better-webui](https://github.com/bLueriVerLHR/dsh-better-webui) | 0 | 2026-08-20 | 2026-08-27 | Minimal improvement if possible. |
| 468 | [bo961386926/dolphin-pet-plugin](https://github.com/bo961386926/dolphin-pet-plugin) | 0 | 2026-08-26 | 2026-08-27 | Cute desktop pet for DeepSeek Harness - custom name, upload your own pet image, or generate one with AI. DSH 桌面宠物插件 |
| 469 | [bosinHU/dsh-skill-editor](https://github.com/bosinHU/dsh-skill-editor) | 0 | 2026-08-29 | 2026-08-30 | Edit skills directly in DSH web settings |
| 470 | [Britneycode/dsh-distillery](https://github.com/Britneycode/dsh-distillery) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：本地蒸馏器——扫历史会话挖「用户纠错 → 改对」片段，脱敏后蒸馏成微调 JSONL / SKILL.md 技能草稿 / AGENTS.md 规则补丁，带人工审核队列 |
| 471 | [Britneycode/dsh-live-room](https://github.com/Britneycode/dsh-live-room) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：把会话变成免登录、只读、可分享的实时直播间（SSE 观看页 + 弹幕 + agent 工具） |
| 472 | [Bronier/dsh-web-search-so360](https://github.com/Bronier/dsh-web-search-so360) | 0 | 2026-08-27 | 2026-08-27 | Keyless web search provider for DeepSeek Harness backed by 360 Search (so.com). |
| 473 | [buchylx/create-dsh-content-plugin](https://github.com/buchylx/create-dsh-content-plugin) | 0 | 2026-08-26 | 2026-08-27 | Zero-dependency CLI that scaffolds a content-automation DSH plugin (Dev.to/GitHub/Bluesky/Mastodon). Like create-vite, for DSH. |
| 474 | [bycall/dsh-code-collector](https://github.com/bycall/dsh-code-collector) | 0 | 2026-08-27 | 2026-08-27 | Session code collector for DeepSeek Harness: gather every code block the model produced in the current session, grouped by language, with copy / download-all / jump-to-turn. |
| 475 | [ByxHuster/DSH-Paper-Highlighting-Agent](https://github.com/ByxHuster/DSH-Paper-Highlighting-Agent) | 0 | 2026-08-27 | 2026-08-27 | An interactive and customized paper highlighting tool built upon Deepseek Harness (DSH), still under development. |
| 476 | [c0nfident/github-slideshow](https://github.com/c0nfident/github-slideshow) | 0 | 2020-07-07 | 2026-08-30 | A robot powered training repository :robot: |
| 477 | [CagierAsh123/dsh-obsidian-agent-wiki](https://github.com/CagierAsh123/dsh-obsidian-agent-wiki) | 0 | 2026-08-26 | 2026-08-27 | Searchable SQLite-indexed Obsidian memory for DeepSeek Harness |
| 478 | [Calvin451970353/dsh-vmic](https://github.com/Calvin451970353/dsh-vmic) | 0 | 2026-08-25 | 2026-08-27 | Voice input plugin for DeepSeek Harness: mic button, 16kHz WAV recording, ASR via Xiaomi MiMo / Volcengine Doubao (live), optional LLM polish. |
| 479 | [CanaryJing/dsh-big-fat-whale-maid-adaptive](https://github.com/CanaryJing/dsh-big-fat-whale-maid-adaptive) | 0 | 2026-08-23 | 2026-08-27 | 大肥鱼女仆长智能体，用风神与明神插件vibe而来，解决wsl与windows互通问题 |
| 480 | [Castem114/dsh-visioncraft](https://github.com/Castem114/dsh-visioncraft) | 0 | 2026-08-26 | 2026-08-27 | 为 DeepSeek Harness（DSH）Web 量身打造的双插件扩展，为纯文本模型补齐"视觉"短板 |
| 481 | [cayan0x/dsh-fold-context](https://github.com/cayan0x/dsh-fold-context) | 0 | 2026-08-28 | 2026-08-28 | Auto-fold context/system messages in DSH — collapse think blocks, tool calls, and tool results into grouped expandable bars. |
| 482 | [ch3vr0n5/dsh-docker-services](https://github.com/ch3vr0n5/dsh-docker-services) | 0 | 2026-08-26 | 2026-08-27 | Portable DeepSeek Harness plugin for securely monitoring and operating Docker services |
| 483 | [changyinliangbaikai/dsh-b2us-schedule](https://github.com/changyinliangbaikai/dsh-b2us-schedule) | 0 | 2026-08-29 | 2026-08-30 | dsh定时任务插件，支持延迟、固定间隔、cron表达式，支持执行shell命令，支持发起Agent会话 |
| 484 | [Che-Year/dsh-pet-lulu](https://github.com/Che-Year/dsh-pet-lulu) | 0 | 2026-08-26 | 2026-08-27 | A cute terminal and web pet plugin for DeepSeek Harness (dsh), using assets from lulu and capybara projects. |
| 485 | [Cheeserackery/deepseek-time](https://github.com/Cheeserackery/deepseek-time) | 0 | 2026-08-18 | 2026-08-28 | 一款Agent插件，能够实时直观显示DeepSeek当前收费时段状态。DeepSeek pricing-period status indicator with Hermes, DSH, and Codex adapters. |
| 486 | [chen70456-lang/dsh-tmwebdriver](https://github.com/chen70456-lang/dsh-tmwebdriver) | 0 | 2026-08-30 | 2026-08-30 | One tool, infinite reach: arbitrary JS in your real logged-in browser. Unlike fixed-action plugins, browser_execute_js does anything DevTools can — read, click, type, fill, navigate, screenshot, CDP. Plus list_tabs/snapshot/type. Zero-setup, self-healing. |
| 487 | [chendefine/dsh-sidebar-onlyoffice](https://github.com/chendefine/dsh-sidebar-onlyoffice) | 0 | 2026-08-24 | 2026-08-27 | DSH web plugin: open and edit .docx/.xlsx/.pptx in the better-sidebar editor through a self-hosted ONLYOFFICE Document Server (JWT-signed config, atomic save-back, live refresh on AI edits) |
| 488 | [chendefine/dsh-sidebar-vscode](https://github.com/chendefine/dsh-sidebar-vscode) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: a better-sidebar tab embedding the VS Code web workbench at the session workspace; editor selections and explorer files land as atomic reference chips |
| 489 | [chenyangcun/dsh-command-palette](https://github.com/chenyangcun/dsh-command-palette) | 0 | 2026-08-30 | 2026-08-30 | A keyboard-first command palette for standard DeepSeek Harness |
| 490 | [chenyangcun/dsh-fixed-new-session-model](https://github.com/chenyangcun/dsh-fixed-new-session-model) | 0 | 2026-08-30 | 2026-08-30 | 为 DSH 固定新会话的默认 Agent 预设与模型，支持全局默认设置和工作区独立配置。 |
| 491 | [chocobo77/dsh-infinite-context](https://github.com/chocobo77/dsh-infinite-context) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: multi-tier memory management, semantic retrieval, structured memory, and model-context awareness for infinite context. |
| 492 | [chouyulanxia114514/dsh-uisketch](https://github.com/chouyulanxia114514/dsh-uisketch) | 0 | 2026-08-28 | 2026-08-28 | UI Sketch to AI 画板编辑器 × DSH 插件：侧栏开关 + 全屏 iframe 浮层，开箱即用 |
| 493 | [CHristianREEVEE/dsh-xiuxian-world](https://github.com/CHristianREEVEE/dsh-xiuxian-world) | 0 | 2026-08-28 | 2026-08-28 | 云仙大世界 — a living xiuxian world for DeepSeek Harness agents: enter, cultivate, and export a self-contained HTML replay of your journey |
| 494 | [cloveric/deepseek-harness-web-search-plugin](https://github.com/cloveric/deepseek-harness-web-search-plugin) | 0 | 2026-08-29 | 2026-08-29 | Source-traceable Brave + Tavily live web search and URL extraction for DeepSeek Harness. Native DSH plugin; TaroCub optional. |
| 495 | [ColdCGH/dsh-desktop-shell](https://github.com/ColdCGH/dsh-desktop-shell) | 0 | 2026-08-24 | 2026-08-29 | dsh desktop shell plugin |
| 496 | [Cooberped/dsh-evidence](https://github.com/Cooberped/dsh-evidence) | 0 | 2026-08-28 | 2026-08-28 | Turn local files into versioned evidence in DeepSeek Harness: composer upload, private local retrieval, and coordinate-exact PDF/DOCX/XLSX/PPTX reads. |
| 497 | [coolgech/dsh-siyuan](https://github.com/coolgech/dsh-siyuan) | 0 | 2026-08-27 | 2026-08-27 | A plugin for deepseek harnes that operates on the notes of Siyuan. |
| 498 | [CoolTea001/dsh-cool-theme](https://github.com/CoolTea001/dsh-cool-theme) | 0 | 2026-08-30 | 2026-08-30 | A plugin for changing themes for DSH, with a number of popular default themes built in. |
| 499 | [cslht11/dsh-provider-config](https://github.com/cslht11/dsh-provider-config) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) LLM 供应商配置模板与限流重试机制最佳实践（SenseNova 脱敏版）。Provider config templates + retry-policy best practices for DSH, sanitized. |
| 500 | [CyberFox-lab/dsh-rss](https://github.com/CyberFox-lab/dsh-rss) | 0 | 2026-08-30 | 2026-08-30 | RSS/Atom reader and Agent tools plugin for DeepSeek Harness |
| 501 | [cyjyyd/dsh-llm-xai-oauth](https://github.com/cyjyyd/dsh-llm-xai-oauth) | 0 | 2026-08-27 | 2026-08-27 | Native SuperGrok / X Premium OAuth provider for DeepSeek Harness. Reuses local grok-bridge tokens; no xAI API key. |
| 502 | [d3vmeh/dsh-context-budget](https://github.com/d3vmeh/dsh-context-budget) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: keep a local model's context at a size your GPU handles well (measured prefill speed, hard ceiling, early compaction) |
| 503 | [daveycodez/dsh-llm-agent-bridge](https://github.com/daveycodez/dsh-llm-agent-bridge) | 0 | 2026-08-26 | 2026-08-27 | Claude as a selectable LLM provider in DeepSeek Harness, via Anthropic's official Claude Agent SDK. Works in any DSH mode. |
| 504 | [david0702/dsh-cost](https://github.com/david0702/dsh-cost) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) 对话底部费用显示插件：按每笔请求时间+模型分批计费，分时段明细，模型归属，读图金额，余额。 |
| 505 | [Dayi-Z/gitcompass](https://github.com/Dayi-Z/gitcompass) | 0 | 2026-08-28 | 2026-08-29 | GitHub-connected visual git panel for DeepSeek Harness - branch switcher, file-level approval cards, PR/issue workspace |
| 506 | [DeepseekHarnessPlugins/Notification](https://github.com/DeepseekHarnessPlugins/Notification) | 0 | 2026-08-26 | 2026-08-27 | DeepseekHarnessPlugin |
| 507 | [demacia1314/dsh-remote-deliver](https://github.com/demacia1314/dsh-remote-deliver) | 0 | 2026-08-27 | 2026-08-27 | 🚀 告别繁琐 SCP！远程部署 DSH 一键下载修改后的文件与图片预览交付插件 |
| 508 | [Demigod-cyber/dsh-angelina-theme](https://github.com/Demigod-cyber/dsh-angelina-theme) | 0 | 2026-08-26 | 2026-08-27 | DSH主题插件——直到大地变成一颗酸橙（Angelina 浅蓝主题） |
| 509 | [dengyier/openworkproof-dsh-plugin](https://github.com/dengyier/openworkproof-dsh-plugin) | 0 | 2026-08-30 | 2026-08-30 | Community DeepSeek Harness plugin for verifiable AI agent authorization, execution evidence, and offline delivery verification |
| 510 | [dennisrongo/dsh-plugins](https://github.com/dennisrongo/dsh-plugins) | 0 | 2026-08-23 | 2026-08-27 | Dennis Rongo's plugin collection for DeepSeek Harness (dsh)  |
| 511 | [DepressionL/fortune-assistant](https://github.com/DepressionL/fortune-assistant) | 0 | 2026-08-28 | 2026-08-30 | dsh算命插件 |
| 512 | [dfhxxc666/dsh-llm-mimo](https://github.com/dfhxxc666/dsh-llm-mimo) | 0 | 2026-08-27 | 2026-08-27 | Xiaomi MiMo v2.5 adapter for DeepSeek Harness — fixed fork (sanitize tool args, dsh-llm 0.1.1-rc.2, prepareCall, keepalive) |
| 513 | [difimim/dsh-voice-input](https://github.com/difimim/dsh-voice-input) | 0 | 2026-08-29 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 514 | [dingminhua/dsh-connect-trae](https://github.com/dingminhua/dsh-connect-trae) | 0 | 2026-08-28 | 2026-08-28 | Connect locally signed-in Trae models to DeepSeek Harness with a read-only credits overview. |
| 515 | [dingminhua/dsh-connect-workbuddy](https://github.com/dingminhua/dsh-connect-workbuddy) | 0 | 2026-08-28 | 2026-08-30 | Connect locally signed-in WorkBuddy models to DeepSeek Harness with a read-only credits overview and model management. |
| 516 | [dingyi580/dsh-plugin-gemini-theme](https://github.com/dingyi580/dsh-plugin-gemini-theme) | 0 | 2026-08-29 | 2026-08-30 | A Gemini-styled skin for the DeepSeek Harness web client |
| 517 | [DobyChao/dsh-workspace-enhancement](https://github.com/DobyChao/dsh-workspace-enhancement) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness plugin: local and remote (SSH) workspaces in one place. Remote execution uses a single SSH connection (multi-hop jumps allowed); bash, files, PTY, and LSP share that link. |
| 518 | [doer1296/dsh-plugin-voice](https://github.com/doer1296/dsh-plugin-voice) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 语音插件：火山 seed-tts 云端 TTS（自动回退 SAPI/Huihui 离线）+ 桌面通知 + 场景化 WAV 提示音 + 提问自动呼叫。DSH 原生集成，零 Python 依赖，Windows 原生。 |
| 519 | [dongsheng123132/dsh-break-glass-settlement-proof](https://github.com/dongsheng123132/dsh-break-glass-settlement-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed DSH proof for break-glass session settlement evidence |
| 520 | [dongsheng123132/dsh-change-window-proof](https://github.com/dongsheng123132/dsh-change-window-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed DSH proof for change-window settlement evidence |
| 521 | [dongsheng123132/dsh-credential-retirement-proof](https://github.com/dongsheng123132/dsh-credential-retirement-proof) | 0 | 2026-08-26 | 2026-08-27 | Evidence-only DSH plugin for credential retirement settlement |
| 522 | [dongsheng123132/dsh-duty-separation-proof](https://github.com/dongsheng123132/dsh-duty-separation-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed duty-separation evidence for supplied DSH workflow receipts |
| 523 | [dongsheng123132/dsh-license-obligation-proof](https://github.com/dongsheng123132/dsh-license-obligation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for license obligation delivery closure |
| 524 | [dongsheng123132/dsh-vulnerability-remediation-proof](https://github.com/dongsheng123132/dsh-vulnerability-remediation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for vulnerability remediation closure |
| 525 | [donoteatme/dsh-local-link](https://github.com/donoteatme/dsh-local-link) | 0 | 2026-08-27 | 2026-08-28 | Lightweight DeepSeek Harness plugin for paired LAN access: scan a QR code and continue the current DSH Web session from any phone, tablet, or computer. |
| 526 | [DoshinJiu/dsh-ui-boost](https://github.com/DoshinJiu/dsh-ui-boost) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness界面调色插件/RGB滑块调色 |
| 527 | [dsh-plugins/dsh-plugin-market](https://github.com/dsh-plugins/dsh-plugin-market) | 0 | 2026-08-26 | 2026-08-27 | A structured plugin marketplace for DeepSeek Harness — each plugin described as JSON, auto-aggregated into a single plugins.json for the dsh-plugins.github.io site. DeepSeek Harness 结构化插件市场 —— 每个插件以 JSON 描述，自动聚合为单一 plugins.json 供 dsh-plugins.github.io 站点消费。 |
| 528 | [dusbin/dsh-attention](https://github.com/dusbin/dsh-attention) | 0 | 2026-08-30 | 2026-08-30 | 任务完成后进行提醒，发完任务就可以去喝杯咖啡了，完成了会叫你的 |
| 529 | [dusbin/dsh-multi-tenant](https://github.com/dusbin/dsh-multi-tenant) | 0 | 2026-08-29 | 2026-08-29 | dsh 支持多租户插件 |
| 530 | [dusbin/voice-plugin](https://github.com/dusbin/voice-plugin) | 0 | 2026-08-27 | 2026-08-27 | Dsh(deepseek harness)语音输入插件 Ps: 朗读功能目前还不是很棒。 |
| 531 | [dxsdyhm/dsh-adb-logcat](https://github.com/dxsdyhm/dsh-adb-logcat) | 0 | 2026-08-26 | 2026-08-27 | Android Studio-style ADB logcat viewer for the DSH Web GUI |
| 532 | [dy395769511-star/dsh-pdf-to-word](https://github.com/dy395769511-star/dsh-pdf-to-word) | 0 | 2026-08-29 | 2026-08-29 | PDF to Word conversion plugin for DeepSeek Harness (dsh): PyMuPDF/PaddleOCR pipeline + LLM visual style verification |
| 533 | [EasyTZ/dsh-git](https://github.com/EasyTZ/dsh-git) | 0 | 2026-08-27 | 2026-08-27 | Git panel plugin for DeepSeek Harness (dsh) — visual staging, commits, push and branch switching in the sidebar |
| 534 | [EasyTZ/dsh-reveal-explorer](https://github.com/EasyTZ/dsh-reveal-explorer) | 0 | 2026-08-27 | 2026-08-27 | Reveal-in-file-manager plugin for DeepSeek Harness (dsh) — open the current workspace in your system file manager |
| 535 | [EasyTZ/dsh-terminal-panel](https://github.com/EasyTZ/dsh-terminal-panel) | 0 | 2026-08-27 | 2026-08-27 | Terminal panel plugin for DeepSeek Harness (dsh) — run commands in the current workspace with streaming output |
| 536 | [EasyTZ/dsh-ui-balance](https://github.com/EasyTZ/dsh-ui-balance) | 0 | 2026-08-27 | 2026-08-27 | Balance display plugin for DeepSeek Harness (dsh) — show your DeepSeek API balance under each reply |
| 537 | [eehcx/dsh-gentle-engram](https://github.com/eehcx/dsh-gentle-engram) | 0 | 2026-08-26 | 2026-08-27 | DSH adapter for Engram — persistent memory bridge built with Cordis. |
| 538 | [EmptyCollin/dsh-peak-valley-queue](https://github.com/EmptyCollin/dsh-peak-valley-queue) | 0 | 2026-08-27 | 2026-08-27 | Peak/valley pricing task queue for DeepSeek Harness |
| 539 | [evlon/deepseek-harness-launcher](https://github.com/evlon/deepseek-harness-launcher) | 0 | 2026-08-28 | 2026-08-29 | 托盘常驻的 DeepSeek Harness 安装 / 启动器（Tauri 2 无窗口应用，仅系统托盘 + 原生通知 + 日志文件） |
| 540 | [evlon/dsh-codebuddy-models](https://github.com/evlon/dsh-codebuddy-models) | 0 | 2026-08-26 | 2026-08-29 | 把本机已登录的 CodeBuddy / WorkBuddy（腾讯代码助手） 订阅作为 dsh（DeepSeek Harness） 的原生 provider 接入，启用后 CodeBuddy 模型会直接出现在 dsh 的模型选择器中，可像其它模型一样被 agent 调用。 |
| 541 | [evlon/dsh-matrix-agent](https://github.com/evlon/dsh-matrix-agent) | 0 | 2026-08-27 | 2026-08-29 | DeepSeek Harness（dsh）的 Matrix agent 桥接插件：把 Matrix 房间桥接到 harness agent 会话，每个房间一个会话，支持在聊天里远程监控、审批和追加指令；多分身架构 + 媒体/富文本/回复/编辑信息完整处理。 |
| 542 | [Exception-H/dsh-gpt56-ptc](https://github.com/Exception-H/dsh-gpt56-ptc) | 0 | 2026-08-30 | 2026-08-30 | Native DSH Bundle: user-owned pure PTC / Code Mode preset for GPT-5.6 with plain-language answers and bounded execution. |
| 543 | [FADE-4869/dsh-gacha-viz](https://github.com/FADE-4869/dsh-gacha-viz) | 0 | 2026-08-26 | 2026-08-27 | Genshin Impact gacha history visualizer and pity probability calculator for DeepSeek Harness (DSH plugin) |
| 544 | [fan56/dsh-ask-router](https://github.com/fan56/dsh-ask-router) | 0 | 2026-08-25 | 2026-08-29 | dsh plugin: multi-surface ask-user routing, first answer wins |
| 545 | [fan56/dsh-dcp](https://github.com/fan56/dsh-dcp) | 0 | 2026-08-17 | 2026-08-28 | dsh plugin: deterministic context compression backend — zero LLM calls, reproducible compression |
| 546 | [fan56/dsh-feishu](https://github.com/fan56/dsh-feishu) | 0 | 2026-08-23 | 2026-08-27 | dsh plugin: drive an existing dsh session from Feishu/Lark — outbound-only bot, /resume picker, run status card |
| 547 | [fan56/dsh-mcp-adapter](https://github.com/fan56/dsh-mcp-adapter) | 0 | 2026-08-26 | 2026-08-29 | dsh plugin: fold mcp__* tool schemas into two meta-tools via prompt-side shim to save tokens |
| 548 | [fan56/dsh-model-sync](https://github.com/fan56/dsh-model-sync) | 0 | 2026-08-28 | 2026-08-29 | A dsh (DeepSeek Harness) Cordis plugin that keeps llm-pi-ai provider routes' model catalog in sync with the pi.dev gateway — written through the official settings seam, zero patches to dsh internals. |
| 549 | [fan56/dsh-web-search-anysearch](https://github.com/fan56/dsh-web-search-anysearch) | 0 | 2026-08-26 | 2026-08-29 | AnySearch web search provider plugin for DeepSeek Harness (dsh) — zero-config, out-of-the-box |
| 550 | [fan56/dsh-web-search-tavily](https://github.com/fan56/dsh-web-search-tavily) | 0 | 2026-08-25 | 2026-08-29 | Tavily web search provider plugin for DeepSeek Harness (dsh) |
| 551 | [fantasyce/dsh-typelens](https://github.com/fantasyce/dsh-typelens) | 0 | 2026-08-27 | 2026-08-28 | Automatic bounded type context and edit diagnostics for DeepSeek Harness |
| 552 | [Fast-Editor/lynkr-dsh-plugin](https://github.com/Fast-Editor/lynkr-dsh-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness (dsh) plugin: registers Lynkr as a custom OpenAI-compatible provider |
| 553 | [faye0526/dsh-backup-btn](https://github.com/faye0526/dsh-backup-btn) | 0 | 2026-08-26 | 2026-08-27 | DSH 一键备份按钮 - 浮动按钮备份 DSH 数据到 GitHub Gist |
| 554 | [FeatureAgents/AgentsGitFlowController](https://github.com/FeatureAgents/AgentsGitFlowController) | 0 | 2026-08-17 | 2026-08-28 | Agents Client Level Git Flow Controller |
| 555 | [felix-lj-ct/dsh-mcp-live-status](https://github.com/felix-lj-ct/dsh-mcp-live-status) | 0 | 2026-08-28 | 2026-08-28 | Live MCP server status in the DeepSeek Harness conversation composer — see which MCP servers are actually connected before you hit send. |
| 556 | [fentz26/dsh-goodjob](https://github.com/fentz26/dsh-goodjob) | 0 | 2026-08-26 | 2026-08-27 | Multi-agent operations workspace for DeepSeek Harness. |
| 557 | [fentz26/dsh-next](https://github.com/fentz26/dsh-next) | 0 | 2026-08-26 | 2026-08-27 | Performance-oriented backend/runtime modernization layer for DeepSeek Harness. |
| 558 | [firestige/wsr-dsh](https://github.com/firestige/wsr-dsh) | 0 | 2026-08-29 | 2026-08-29 | WSR integrations for DeepSeek Harness: Execution, Studio, and suite bundles. |
| 559 | [firestige/wsr-execution](https://github.com/firestige/wsr-execution) | 0 | 2026-08-17 | 2026-08-30 | Host-neutral execution boundary for workflow-self-recursive: resolves one exact Workflow Package, binds an immutable Delivery Manifest, coordinates the Delivery, emits bounded OTLP observations. Install via dsh plugin add wsr-dsh-intake · 与宿主无关的 Agent 工作流执行边界：解析并校验确定的工作流包，绑定不可变交付清单，协调交付并发出有界观测。 |
| 560 | [FishBottle7/opencode2dsh](https://github.com/FishBottle7/opencode2dsh) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin — free OpenCode Zen models for DeepSeek Harness (DSH). Free LLM API, no API key needed. 在 DSH 中使用 OpenCode Zen 免费模型，无需 API key |
| 561 | [fishfromsky/dsh-march7th-skin](https://github.com/fishfromsky/dsh-march7th-skin) | 0 | 2026-08-20 | 2026-08-27 | 崩坏星穹铁道三月七主题的deepseek harness皮肤插件 |
| 562 | [Flan246/dsh-latex-guard](https://github.com/Flan246/dsh-latex-guard) | 0 | 2026-08-26 | 2026-08-27 | LaTeX compile check and BibTeX lint/fill/audit tools for DeepSeek Harness and any agent. dsh plugin + CLI + SKILL.md. |
| 563 | [Flan246/dsh-lit-search](https://github.com/Flan246/dsh-lit-search) | 0 | 2026-08-26 | 2026-08-27 | Academic literature search, citation and BibTeX tools for DeepSeek Harness and any agent (Crossref + OpenAlex). dsh plugin + CLI + SKILL.md. |
| 564 | [flashyiyi/dsh-envelope-highlight](https://github.com/flashyiyi/dsh-envelope-highlight) | 0 | 2026-08-28 | 2026-08-28 | Restore syntax highlighting of read/write tool envelopes inside run_code (PTC / Code Mode) result cards |
| 565 | [flyingfishzxf/dsh-dsbal](https://github.com/flyingfishzxf/dsh-dsbal) | 0 | 2026-08-18 | 2026-08-27 | A simple DeepSeek API balance display plugin for dsh(deepseek-harness) |
| 566 | [force-push/dsh-llm-fallback](https://github.com/force-push/dsh-llm-fallback) | 0 | 2026-08-27 | 2026-08-27 | Self-healing cross-provider model fallback plugin for the DeepSeek Harness (DSH) — retries exhausted, re-bind the session to the next healthy model. |
| 567 | [founder987/dsh-dev-ui](https://github.com/founder987/dsh-dev-ui) | 0 | 2026-08-25 | 2026-08-27 | 适合编码研发的UI界面 |
| 568 | [Francesco502/dsh-quota](https://github.com/Francesco502/dsh-quota) | 0 | 2026-08-26 | 2026-08-27 | AI Quota and Token Usage Monitor for DeepSeek Harness (Codex, Cursor, Antigravity, OpenCode-Go) |
| 569 | [Frank-NF/dsh-drop-md](https://github.com/Frank-NF/dsh-drop-md) | 0 | 2026-08-30 | 2026-08-30 | Drag-and-drop markdown enhancer for DeepSeek Harness (DSH): inline small files, @-reference large ones, one-click SKILL.md install |
| 570 | [freedomkk-qfeng/dsh-oidc](https://github.com/freedomkk-qfeng/dsh-oidc) | 0 | 2026-08-30 | 2026-08-30 | Enterprise OIDC, secure API-key binding, declarative branding, and OpenAI-compatible model integration for DeepSeek Harness. |
| 571 | [FriendsHL/dsh-agent-evolution](https://github.com/FriendsHL/dsh-agent-evolution) | 0 | 2026-08-26 | 2026-08-27 | Preset-composed Agent experiments and evolution primitives for DeepSeek Harness |
| 572 | [GavinQiEr/dsh-cmdwatch](https://github.com/GavinQiEr/dsh-cmdwatch) | 0 | 2026-08-30 | 2026-08-30 | Real-time command monitor for DeepSeek Harness (DSH). Watch foreground/background command output in the Web UI without pausing the conversation. 命令窗：实时显示 DSH 命令与执行输出。 |
| 573 | [geeklei/dsh-plugins](https://github.com/geeklei/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | 一个面向 DeepSeek Harness (dsh)的插件库 |
| 574 | [geekyfoxlab/dsh-subagents](https://github.com/geekyfoxlab/dsh-subagents) | 0 | 2026-08-26 | 2026-08-27 | Focused child-agent delegation (scout, researcher, worker, reviewer, oracle, delegate) and multi-agent workflows (council, parallel review, review loop) for DeepSeek Harness. |
| 575 | [ghbhiee/dsh-plugin-tui](https://github.com/ghbhiee/dsh-plugin-tui) | 0 | 2026-08-28 | 2026-08-28 | Claude Code-style terminal UI plugin for DeepSeek Harness (dsh): streaming REPL, collapsed thinking, interactive session/model pickers, history replay, approval modes, bottom status bar |
| 576 | [Ghost011118/dsh-plugin-governor-extension](https://github.com/Ghost011118/dsh-plugin-governor-extension) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin governance: installable runtime tool policy plus companion boot admission, supervised restart, and rollback. |
| 577 | [Ghost011118/dsh-plugin-marketplace](https://github.com/Ghost011118/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Built-in plugin discovery, local requirement matching, optional GitHub stars, and one-click installation for DeepSeek Harness. |
| 578 | [GitNoHup/macaron-theme](https://github.com/GitNoHup/macaron-theme) | 0 | 2026-08-26 | 2026-08-27 | 🍬 马卡龙毛玻璃主题（Macaron Glassmorphism Theme）— DeepSeek Harness 动态主题插件：四套马卡龙配色、145° 双色渐变、毛玻璃卡片；日间上色 / 夜间自动清除并记忆恢复。 |
| 579 | [Glazyonyt/dsh-lowtide](https://github.com/Glazyonyt/dsh-lowtide) | 0 | 2026-08-28 | 2026-08-28 | Queue AI tasks during off-peak hours to cut costs and automate runs with dsh-lowtide for DeepSeek Harness. |
| 580 | [GoldenZqqq/dsh-model-collapse](https://github.com/GoldenZqqq/dsh-model-collapse) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin: collapse the model picker by provider, with a pinned quick bar (expand-all / collapse-all / focus-current / filter / reset). |
| 581 | [goldgish/dsh-gamepad-approval](https://github.com/goldgish/dsh-gamepad-approval) | 0 | 2026-08-30 | 2026-08-30 | Xbox 手柄硬件审批插件 for DeepSeek Harness (dsh) — Agent 高危工具调用需物理按键确认，A 批准 / B 驳回 |
| 582 | [GooDAnDReaDY/dsh-messenger-gateway](https://github.com/GooDAnDReaDY/dsh-messenger-gateway) | 0 | 2026-08-26 | 2026-08-27 | Telegram messenger bridge for DeepSeek Harness: sessions, steer, homes, and TTS voice notes |
| 583 | [Gorilla-Kevv/scnu-thesis-formatter](https://github.com/Gorilla-Kevv/scnu-thesis-formatter) | 0 | 2026-08-30 | 2026-08-30 | 华南师范大学本科毕业论文格式改写 + matplotlib 数据可视化（DeepSeek Harness 技能） |
| 584 | [GreenLv/dsh-completion-guard](https://github.com/GreenLv/dsh-completion-guard) | 0 | 2026-08-26 | 2026-08-29 | Task-contract and completion-certification layer for DeepSeek Harness |
| 585 | [guangxiangwu6-cmd/dsh-llm-failover](https://github.com/guangxiangwu6-cmd/dsh-llm-failover) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness model auto-failover plugin: retry threshold -> mark unavailable -> seamless switch to next healthy model -> cooldown auto-recover. 18-model pool, 19/19 tests, boot-safe. |
| 586 | [guazixiong/dsh-coding-mode-preset](https://github.com/guazixiong/dsh-coding-mode-preset) | 0 | 2026-08-30 | 2026-08-30 | 为本地 DeepSeek Harness（`@deepseek-ai/dsh`）追加一个**编码模式** Agent Preset：门禁式工程交付流水线，包含三条独立流程——**需求开发**、**Bug 修复**、**功能迭代**。每个阶段的产物由全新上下文的"空白子代理"独立专家评审，通过后须经用户确认才进入下一阶段；最终以用户验收作为任务完结条件。 |
| 587 | [GuoxinShan/dsh-yzj](https://github.com/GuoxinShan/dsh-yzj) | 0 | 2026-08-14 | 2026-08-27 | 云之家 (Yunzhijia) plugin bundle for DeepSeek Harness: yzj-cli bridge, 41 model-facing tools, floating workspace panel with drag/@ reference chips |
| 588 | [gychen-NJU/dsh-overleaf](https://github.com/gychen-NJU/dsh-overleaf) | 0 | 2026-08-27 | 2026-08-29 | Embedded Overleaf workbench tab for DeepSeek Harness Web: same-origin reverse proxy, direct-CDP login, selection quoting, caret insertion, LaTeX assist panel |
| 589 | [Hanmingh/dsh-desktop](https://github.com/Hanmingh/dsh-desktop) | 0 | 2026-08-27 | 2026-08-27 | Desktop Plugin for Deepseek Harness |
| 590 | [haohaiHuang/Design-Agent](https://github.com/haohaiHuang/Design-Agent) | 0 | 2026-08-27 | 2026-08-27 | DSH 设计 Agent 完整可复现包：design-references 路由技能（DSH 适配）+ design-router 确定性工具插件 + my-agent 预设 |
| 591 | [haoranwang0921/dsh-bid-desk](https://github.com/haoranwang0921/dsh-bid-desk) | 0 | 2026-08-28 | 2026-08-30 | DSH 投标合规工作台是一个 DSH 插件 MVP，服务于投标文件编制过程。它将招标来源证据、要求记录、人工复核决定和生成报告关联起来，帮助具备相应资质或经验的人员在提交前核查缺口。 |
| 592 | [haoyu-qi/dsh-zentao](https://github.com/haoyu-qi/dsh-zentao) | 0 | 2026-08-15 | 2026-08-27 | 面向 DeepSeek Harness 的 AVCON Web 界面定制与个人禅道 CLI 工作中心 |
| 593 | [haozheou/dsh-exam-expert](https://github.com/haozheou/dsh-exam-expert) | 0 | 2026-08-30 | 2026-08-30 | 出题专家 · Exam Expert plugin for DeepSeek Harness: 把出题流程固化成值守流水线（角色+目录→通读→勾选表单→六分身流水线→看板交付） \| Turn the exam-paper workflow into an agent-supervised pipeline: wizard dialog, prefilled checklist form, six-role dual-kanban production |
| 594 | [harness-home/harness-ai-plugins](https://github.com/harness-home/harness-ai-plugins) | 0 | 2026-08-26 | 2026-08-27 | Community plugin catalog for Harness AI: a scanner over the public npm registry, and the snapshot it publishes. |
| 595 | [Harzva/dsh-restart-autoresume](https://github.com/Harzva/dsh-restart-autoresume) | 0 | 2026-08-29 | 2026-08-29 | Safe DSH restart coordination and durable top-level session autoresume |
| 596 | [haythamat/dsh-client-ui-rtl](https://github.com/haythamat/dsh-client-ui-rtl) | 0 | 2026-08-27 | 2026-08-27 | Right-to-left text direction for the DeepSeek Harness Web client |
| 597 | [hedging8563/tokenlab-deepseek-harness-provider](https://github.com/hedging8563/tokenlab-deepseek-harness-provider) | 0 | 2026-08-27 | 2026-08-27 | TokenLab native-protocol model provider, multimodal tools, and async tasks for DeepSeek Harness |
| 598 | [hehetoshang/dsh-talebook-plugin](https://github.com/hehetoshang/dsh-talebook-plugin) | 0 | 2026-08-27 | 2026-08-30 | DeepSeek Harness plugin for safely operating Talebook |
| 599 | [helibeiqi/dsh-cdp-metadata](https://github.com/helibeiqi/dsh-cdp-metadata) | 0 | 2026-08-23 | 2026-08-28 | Capability Description Protocol (CDP) v0.1 — read-only AI-readable capability metadata layer for DSH Cordis plugins. |
| 600 | [helibeiqi/dsh-cn-disclosure](https://github.com/helibeiqi/dsh-cn-disclosure) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 公告/年报 结构化抽取 MCP server (dsh-plugin) |
| 601 | [helibeiqi/dsh-context-aware-search](https://github.com/helibeiqi/dsh-context-aware-search) | 0 | 2026-08-19 | 2026-08-28 | Context-aware web search plugin for DeepSeek Harness (dsh): rewrites queries with session context, reranks + credibility-tags results, one-click source summarization across multiple backends. Fully decoupled from @deepseek-ai private packages for public CI. |
| 602 | [helibeiqi/dsh-dcs-engine](https://github.com/helibeiqi/dsh-dcs-engine) | 0 | 2026-08-24 | 2026-08-28 | Dynamic Capability Synthesis Engine — DSH protocol stack credit engine |
| 603 | [helibeiqi/dsh-docx-mcp](https://github.com/helibeiqi/dsh-docx-mcp) | 0 | 2026-08-28 | 2026-08-28 | Zero-dependency MCP stdio server that generates real .docx files from a JSON spec — Chinese office-automation vertical for DeepSeek Harness. |
| 604 | [helibeiqi/dsh-hr-payroll-mcp](https://github.com/helibeiqi/dsh-hr-payroll-mcp) | 0 | 2026-08-29 | 2026-08-29 | 通用 HR 算薪 MCP 服务：本地化法定社保/公积金/个税计算 + 通用表头适配 + 企业配置 + 安全绩效公式（PII 不出机） |
| 605 | [helibeiqi/dsh-industry-graph-mcp](https://github.com/helibeiqi/dsh-industry-graph-mcp) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 产业链/申万行业/概念板块 知识图谱 MCP server (dsh-plugin) |
| 606 | [helibeiqi/dsh-memory-projection](https://github.com/helibeiqi/dsh-memory-projection) | 0 | 2026-08-20 | 2026-08-28 | Hot-pluggable memory-projection scheduling framework for DeepSeek Harness (dsh): pure-function projection strategies + a runtime invariant guard, built on the cordis plugin kernel. |
| 607 | [helibeiqi/dsh-quant-factor-pipeline](https://github.com/helibeiqi/dsh-quant-factor-pipeline) | 0 | 2026-08-28 | 2026-08-28 | Quant factor research pipeline as a dsh user-layer MCP server (CGO disposal-effect factor, RankIC, Newey-West t, regime-aware) |
| 608 | [hellofuture2068/dsh-simple-view](https://github.com/hellofuture2068/dsh-simple-view) | 0 | 2026-08-26 | 2026-08-27 | Declutter DeepSeek Harness chat: hide agent execution-log rows, tighten spacing & fonts, bubble messages, and set a "reply concisely" system-prompt instruction. |
| 609 | [hellogit2021/avoid-ai-writing-cn](https://github.com/hellogit2021/avoid-ai-writing-cn) | 0 | 2026-08-29 | 2026-08-29 | 知乎"去AI味写作技巧"社区免费提供：中文写作去 AI 味插件（AI-isms / AI writing / humanize）。说"去掉AI味"即重写，说"写的不错"自动学习新 AI 词。安装：dsh plugin --profile web add github:hellogit2021/avoid-ai-writing-cn |
| 610 | [helloworld1631/dsh-volcengine-usage](https://github.com/helloworld1631/dsh-volcengine-usage) | 0 | 2026-08-27 | 2026-08-27 | Draggable Volcengine Coding Plan usage monitor for DeepSeek Harness Web. |
| 611 | [hfyydd/dsh-cua](https://github.com/hfyydd/dsh-cua) | 0 | 2026-08-28 | 2026-08-28 | Computer Use for DeepSeek Harness, backed by the cua-driver daemon (trycua): UIA element-level targeting, background-first input delivery, deterministic verification. |
| 612 | [hhb1028/dsh-client-ui-timeline](https://github.com/hhb1028/dsh-client-ui-timeline) | 0 | 2026-08-30 | 2026-08-30 | DSH Web GUI 会话问题导航条：聊天区左缘一问一杠，随滚动高亮当前问题、悬停显示问答预览气泡、点击把该问平滑滚到视口顶（未渲染的更早历史自动翻页加载），无需改动 dsh 本体源码 |
| 613 | [HiSeax/dsh-agent-outputs-reader](https://github.com/HiSeax/dsh-agent-outputs-reader) | 0 | 2026-08-29 | 2026-08-30 | Overlay reader for agent output files: Markdown/GFM rendering, in-panel PDF, DOCX/XLSX/PPTX text preview, reply-end file chips. Pure JS, zero deps. |
| 614 | [HiSeax/dsh-better-model-setting](https://github.com/HiSeax/dsh-better-model-setting) | 0 | 2026-08-23 | 2026-08-29 | DSH plugin: replaces official Models settings page with provider management, per-model reasoning effort, retry overrides, drag reorder, add official DeepSeek, credential status |
| 615 | [hmlyx/dsh-memory](https://github.com/hmlyx/dsh-memory) | 0 | 2026-08-29 | 2026-08-29 | 简单的插件，让你的每个 AI 记录经验和记忆 |
| 616 | [hmlyx/dsh-notify](https://github.com/hmlyx/dsh-notify) | 0 | 2026-08-29 | 2026-08-29 | 在输入框右边加了一个泡泡窗口，你可以接入插件或者告诉 AI 什么时候使用它。 |
| 617 | [honoriomelo/dsh-model-picker-search](https://github.com/honoriomelo/dsh-model-picker-search) | 0 | 2026-08-29 | 2026-08-29 | DSH Web GUI plugin: adds a live search field inside the model picker menu of the composer, plus the Effort (reasoning) selector. Drop-in replacement for the native model seat, sharing the same per-session ModelDirectory so /model popup, the effort selector, and the /model command stay consistent. |
| 618 | [horizon105457/tsstream](https://github.com/horizon105457/tsstream) | 0 | 2026-08-26 | 2026-08-27 | 🌊 Agent-native time-series streaming for DeepSeek Harness (DSH plugin) — terminal/serial byte streams → indexed, queryable, event-driven timeline. 19 tools · 9 operators · 🧪 experimental |
| 619 | [Hoshino-Yumetsuki/as-compatible-copilot](https://github.com/Hoshino-Yumetsuki/as-compatible-copilot) | 0 | 2026-08-01 | 2026-08-29 | A VSCode extension to use Openai/Anthropic/Gemini API Providers in GitHub Copilot Chat |
| 620 | [hu669293657/dsh-turn-tools](https://github.com/hu669293657/dsh-turn-tools) | 0 | 2026-08-29 | 2026-08-29 | DSH web plugin: per-turn deliverable buttons (open with the OS default app) and a turn-navigator dot rail for jumping between conversation turns. |
| 621 | [huangDouP/dsh-client-ui-notifications](https://github.com/huangDouP/dsh-client-ui-notifications) | 0 | 2026-08-29 | 2026-08-29 | DSH Web notifications: browser notifications, tab title flash, favicon badge, and native Windows toasts with a bilingual (zh/en) settings page. |
| 622 | [HuanLinOTO/dsh-plugin-copilot](https://github.com/HuanLinOTO/dsh-plugin-copilot) | 0 | 2026-08-28 | 2026-08-28 | Copilot 引导层插件：WebUI 设置卡片一键 GitHub 授权 + 自动激活模型路由并收窄模型列表（复用 dsh-llm-pi-ai 内置 device-flow） \| Copilot onboarding plugin: one-click GitHub auth from the WebUI settings card, auto-activating the model route and narrowing the model list (reuses dsh-llm-pi-ai's builtin device flow) |
| 623 | [HuanLinOTO/dsh-plugin-tools-manager](https://github.com/HuanLinOTO/dsh-plugin-tools-manager) | 0 | 2026-08-14 | 2026-08-28 | DSH 工具管理器：查看/启停宿主已注册工具 \| DSH tools manager: inspect and toggle host-registered tools |
| 624 | [HuanyuTan777/dsh-tool-pdf](https://github.com/HuanyuTan777/dsh-tool-pdf) | 0 | 2026-08-28 | 2026-08-28 | DSH PDF reader plugin (pdf_info / pdf_extract / pdf_render) |
| 625 | [huaxiren6/DSH-QrPairing](https://github.com/huaxiren6/DSH-QrPairing) | 0 | 2026-08-19 | 2026-08-27 | Floating phone-pairing QR button for the DSH WebUI. Companion UI for dsh-remote-link. |
| 626 | [HULILI-com/dsh-namecheck](https://github.com/HULILI-com/dsh-namecheck) | 0 | 2026-08-26 | 2026-08-27 | dsh plugin for checking domain availability and trademark screening of candidate product names |
| 627 | [hunbs-1/dsh-codepect](https://github.com/hunbs-1/dsh-codepect) | 0 | 2026-08-29 | 2026-08-30 | dsh-codepect is a DSH plugin generating OpenAPI 3.0 from TS/JS. Features: visual docs, versioning, change detection, mock & auto-rescan. Zero-dep, offline, ensures code-doc sync for backend API delivery. dsh-codepect是DSH插件，扫描TS/JS生成OpenAPI3.0文档。支持可视化、多版本、变更检测、Mock及自动重扫。零依赖离线可用，确保代码文档一致，助后端交付API契约。 |
| 628 | [hunterxxn/deep-flow](https://github.com/hunterxxn/deep-flow) | 0 | 2026-08-14 | 2026-08-29 | deepseek-harness tui |
| 629 | [huyang2024/dsh-openai-api](https://github.com/huyang2024/dsh-openai-api) | 0 | 2026-08-27 | 2026-08-27 | OpenAI-compatible HTTP surface for DeepSeek Harness (dsh): POST /v1/chat/completions, POST /v1/responses, GET /v1/models over the harness webServer + llm runtime |
| 630 | [icyaaaww/dsh-tui-secret-guard](https://github.com/icyaaaww/dsh-tui-secret-guard) | 0 | 2026-08-26 | 2026-08-27 | Blocks high-confidence secrets before dsh-TUI sends them to a model, compliant with dsh ecosystem manifest v0.15. |
| 631 | [iguanren/Taishan-Vision](https://github.com/iguanren/Taishan-Vision) | 0 | 2026-08-29 | 2026-08-29 | 让 DeepSeek Harness 纯文本模型也能识图：默认推荐智谱 GLM-4.6V-FLASH和 GLM-4.1V-FLASH 免费视觉模型 |
| 632 | [ihorleleka/Local-Rag-Wiki](https://github.com/ihorleleka/Local-Rag-Wiki) | 0 | 2026-06-03 | 2026-08-27 | A per-repository, Docker-hosted MCP knowledge service that gives coding agents a governed Markdown "wiki" with semantic retrieval. The promise — a local RAG wiki that accumulates durable project knowledge across agentic sessions. |
| 633 | [IKEASven69/dsh-opencli](https://github.com/IKEASven69/dsh-opencli) | 0 | 2026-08-30 | 2026-08-30 | 让 DeepSeek Harness (dsh) 会办事:登录态真实浏览器 + 170+ 站点适配器 + write 审批门 |
| 634 | [imkingjh999/dsh-adaptive-effort](https://github.com/imkingjh999/dsh-adaptive-effort) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: auto reasoning_effort (low/high/max) per turn via MiniMax complexity scorer + token ledger + per-reply metadata label |
| 635 | [iTrimut/GitHub-Road](https://github.com/iTrimut/GitHub-Road) | 0 | 2026-08-28 | 2026-08-28 | Github-Road: 大陆稳定访问 GitHub 官网的网络路径修复技能（hosts 直连 + 动态 IP 择优 + 30 分钟自动自愈，免代理、零费用）——非 agent 专属，任意智能体可用，也可纯手动运行。A network-path fix skill (not agent-specific) for reliable github.com access from mainland China. |
| 636 | [jaaty/dsh-gsd-bundle](https://github.com/jaaty/dsh-gsd-bundle) | 0 | 2026-08-23 | 2026-08-30 | A DeepSeek Harness bundle reimplementing opengsd-core (Git Ship Done) as host-plane Cordis plugins, replacing the default agent-loop behaviour with the GSD phase loop. |
| 637 | [JackyYangxx/dsh-plugins](https://github.com/JackyYangxx/dsh-plugins) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness (DSH) plugin workspace — home of lbx-agent-team, a multi-agent development team plugin (captain-led planner/checker/dever/tester with pipeline hard gates, git worktrees and a live web panel) |
| 638 | [jasonguide/dsh-skills-hub](https://github.com/jasonguide/dsh-skills-hub) | 0 | 2026-08-28 | 2026-08-29 | 一个多 Agent 平台的 Skills 统一管理插件（DeepSeek Harness 插件），可以在DSH中统一管理codex、claude code、PI、OpenCode、Hermes、Openclaw等平台的Skills技能 |
| 639 | [Jensen-Yao/dsh-deepexcel](https://github.com/Jensen-Yao/dsh-deepexcel) | 0 | 2026-08-27 | 2026-08-28 | Deepcel 工作簿 · DeepSeek Harness (dsh) 皮肤中心 v2 皮肤：Excel 风格工作簿，单元格化消息、工作表网格、工作簿标签。Small-tailqwq/dsh-deepcel 的 v2 完整移植。 |
| 640 | [Jiachi5533/dsh-remote-gateway](https://github.com/Jiachi5533/dsh-remote-gateway) | 0 | 2026-08-28 | 2026-08-28 | Source-filtered remote gateway for DeepSeek Harness behind an authenticated reverse proxy |
| 641 | [jiang12345-code/dsh-openrouter-free](https://github.com/jiang12345-code/dsh-openrouter-free) | 0 | 2026-08-27 | 2026-08-27 | OpenRouter 免费模型面板 for DeepSeek Harness — 分级星标 · 一键切换 · 任务续跑友好 |
| 642 | [jiang12345-code/dsh-self-restart](https://github.com/jiang12345-code/dsh-self-restart) | 0 | 2026-08-29 | 2026-08-29 | DSH self-restart plugin (Windows): reliable elevated restart via schtasks, transparent front-end recovery, auto-detect and resume in-progress sessions across reboots, business gate prevents wake self-excitation loops. |
| 643 | [jiangchuangege/anime-pet-widget](https://github.com/jiangchuangege/anime-pet-widget) | 0 | 2024-01-19 | 2026-08-27 | jenkins测试 |
| 644 | [JiayiXie-jpg/dsh-desktop-pet](https://github.com/JiayiXie-jpg/dsh-desktop-pet) | 0 | 2026-08-26 | 2026-08-27 | 一只住在 DSH 网页里的养成系桌宠：随编码活动升级进化、语音打气，还能用 AI 生成专属的透明动画形象。 |
| 645 | [jimmyzhang219/dsh-plan-and-execute](https://github.com/jimmyzhang219/dsh-plan-and-execute) | 0 | 2026-08-30 | 2026-08-30 | dsh插件plan-and-execute |
| 646 | [jingyunstudio/jingyun-dsh](https://github.com/jingyunstudio/jingyun-dsh) | 0 | 2026-08-27 | 2026-08-29 | 基于 Jingyun Studio + DeepSeek Harness (DSH) 打造的一站式 AI 商业化桌面客户端 |
| 647 | [jingzhonghui/dsh-mcp-manager](https://github.com/jingzhonghui/dsh-mcp-manager) | 0 | 2026-08-30 | 2026-08-30 | DSH dynamic Cordis plugin: visually manage MCP servers (stdio) from the settings sidebar, and expose their tools to the agent as mcp__<server>__<tool>. |
| 648 | [jinwendijv/dsh-applauncher](https://github.com/jinwendijv/dsh-applauncher) | 0 | 2026-08-27 | 2026-08-27 | DSH 的应用启动器插件：自动扫描本机已安装的电脑应用，在侧边栏“设置”图标上方提供一键启动，像 Windows 开始菜单一样，扫描添加后可以点击启动应用 |
| 649 | [jn18755/dsh-skill-nannan](https://github.com/jn18755/dsh-skill-nannan) | 0 | 2026-08-27 | 2026-08-27 | DSH 插件：基于《地狱磨砺》(Hell Grind) 方法论的 AI 视频提示词规范（29 条规则，已去除压力测试阶段） |
| 650 | [jo32/dsh-strudel-studio](https://github.com/jo32/dsh-strudel-studio) | 0 | 2026-08-29 | 2026-08-30 | A professional song-level Strudel visual sequencer with structured AI arrangement for DeepDeck. |
| 651 | [jo32/dsh-video-sherlock](https://github.com/jo32/dsh-video-sherlock) | 0 | 2026-08-26 | 2026-08-27 | A local-first, evidence-backed video investigation app for DeepDeck. |
| 652 | [joao-paulo-santos/dsh-bouncing-squares-example](https://github.com/joao-paulo-santos/dsh-bouncing-squares-example) | 0 | 2026-08-26 | 2026-08-27 | Example plugin for dsh-granular-settings: three bouncing squares, one per settings scope (session, workspace, global). Switch sessions and workspaces to watch each scope behave differently |
| 653 | [joao-paulo-santos/dsh-diff-view](https://github.com/joao-paulo-santos/dsh-diff-view) | 0 | 2026-08-29 | 2026-08-29 | Diff view: a reusable two-text diff viewer for DSH client plugins — line LCS, word highlights, split/unified views, true line numbers across context collapse. |
| 654 | [joao-paulo-santos/dsh-granular-prompt](https://github.com/joao-paulo-santos/dsh-granular-prompt) | 0 | 2026-08-27 | 2026-08-27 | Prompt composition manager for DSH: live census of every system-prompt section with suppress and replace, custom system prompts, and a persona library with a picker right in the chat composer |
| 655 | [joao-paulo-santos/dsh-granular-settings](https://github.com/joao-paulo-santos/dsh-granular-settings) | 0 | 2026-08-26 | 2026-08-27 | Granular settings platform: one Granular Settings page (Workspace/Session/Plugin tabs) where other DSH plugins register scoped, namespaced controls (session, workspace, global). Nine control types, doorbell-only push via dsh-event-relay |
| 656 | [joao-paulo-santos/dsh-md-view](https://github.com/joao-paulo-santos/dsh-md-view) | 0 | 2026-08-29 | 2026-08-29 | Markdown view: a safe markdown-to-React renderer for DSH client plugins — GitHub-subset markdown, shared stylesheet, no HTML injection. |
| 657 | [joao-paulo-santos/dsh-scratchpad](https://github.com/joao-paulo-santos/dsh-scratchpad) | 0 | 2026-08-28 | 2026-08-28 | Scratch pad: one shared floating text surface in the middle of the screen, opened by other plugins through the client service scratchpad. |
| 658 | [joao-paulo-santos/dsh-wo-github](https://github.com/joao-paulo-santos/dsh-wo-github) | 0 | 2026-08-29 | 2026-08-29 | Workspace Overview GitHub tab: About card, README rendered as markdown, and the default-branch commit history with per-file patches. |
| 659 | [joao-paulo-santos/dsh-workspace-history](https://github.com/joao-paulo-santos/dsh-workspace-history) | 0 | 2026-08-28 | 2026-08-28 | Workspace history: journals every compaction summary to the workspace and adds a History subtab to the Workspace Overview tab for reading it back. |
| 660 | [joao-paulo-santos/dsh-workspace-overview](https://github.com/joao-paulo-santos/dsh-workspace-overview) | 0 | 2026-08-28 | 2026-08-28 | Workspace overview: a Workspace Overview tab beside Chat with a subtab facade for other plugins, and a GitHub pill in the session header when the workspace has a github.com repository. |
| 661 | [JochenYang/dsh-remote](https://github.com/JochenYang/dsh-remote) | 0 | 2026-08-29 | 2026-08-29 | Operate DeepSeek Harness from your phone: self-hosted relay + desktop plugin tunnel with a mobile-adapted web UI. MIT |
| 662 | [JoeeLiu/dsh-super-subscriptions](https://github.com/JoeeLiu/dsh-super-subscriptions) | 0 | 2026-08-28 | 2026-08-28 | Unified subscription providers, model routing, quota UI, and media tools for DeepSeek Harness |
| 663 | [JoeyLearnsToCode/dsh-workspace-native-open](https://github.com/JoeyLearnsToCode/dsh-workspace-native-open) | 0 | 2026-08-28 | 2026-08-28 | dsh plugin for native open workspace / 用于本地打开工作区目录的 dsh 插件 |
| 664 | [johnvictorio/dsh-custom-prompt](https://github.com/johnvictorio/dsh-custom-prompt) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin that injects an editable section into the global system prompt, with a Settings page |
| 665 | [joshryandavis/dsh-catalog-refresh](https://github.com/joshryandavis/dsh-catalog-refresh) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically rebuild model catalogues for OpenRouter, OpenCode, Fireworks, etc |
| 666 | [joshryandavis/dsh-goal-restart](https://github.com/joshryandavis/dsh-goal-restart) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically restart goals on harness restart |
| 667 | [jsoncode/dsh-model-list](https://github.com/jsoncode/dsh-model-list) | 0 | 2026-08-27 | 2026-08-28 | OpenRouter free-models browser & one-click model config for DeepSeek Harness (DSH) — newest-first, local search, platform tabs. DSH 免费模型浏览器：按最新排序、本地搜索、一键添加到模型列表 |
| 668 | [Jstn-1g/dsh-live-voice](https://github.com/Jstn-1g/dsh-live-voice) | 0 | 2026-08-25 | 2026-08-28 | DSH Live Voice preview: consent-bound voice add-on for DeepSeek Harness with exact-Session isolation and one bounded manual audio turn. |
| 669 | [junwei529/work-charter-dsh](https://github.com/junwei529/work-charter-dsh) | 0 | 2026-08-28 | 2026-08-30 | DSH-native Work Charter policy plugin backed by session-coordinator-dsh |
| 670 | [jwilson411/dsh-arxiv](https://github.com/jwilson411/dsh-arxiv) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: tiny read-only arXiv search + abstract fetch (Atom API, no PDF ingest) |
| 671 | [jwilson411/dsh-kokoro](https://github.com/jwilson411/dsh-kokoro) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: HTTP TTS client for jwilson411/kokoro-tts-api. No weights. |
| 672 | [jwilson411/dsh-llamacpp](https://github.com/jwilson411/dsh-llamacpp) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness LLM adapter for a local llama.cpp OpenAI-compatible server. |
| 673 | [jwilson411/dsh-modelprint](https://github.com/jwilson411/dsh-modelprint) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: fingerprint provider, model id, sampling, tool schemas, and system-prompt prefix; pin the card and fail structured on drift. |
| 674 | [jwilson411/dsh-otel](https://github.com/jwilson411/dsh-otel) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: emit OpenTelemetry spans from a session log (turn / step / tool execute). Export only. |
| 675 | [jwilson411/dsh-plugin-kit](https://github.com/jwilson411/dsh-plugin-kit) | 0 | 2026-08-29 | 2026-08-29 | A minimal, tested template for DeepSeek Harness plugins. |
| 676 | [kaixinguo360/dsh-bsk-ws-bridge](https://github.com/kaixinguo360/dsh-bsk-ws-bridge) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness BrowserSkill 桥接插件：把本机 bsk daemon 的 WebSocket 经浏览器信道暴露给远程 BrowserSkill 扩展。配套的修改版 BrowserSkill 扩展：https://github.com/kaixinguo360/BrowserSkill-DSH-Remote |
| 677 | [kaka-crypto/dsh-disk-guard](https://github.com/kaka-crypto/dsh-disk-guard) | 0 | 2026-08-28 | 2026-08-28 | Disk guard for DeepSeek Harness: redirect downloads/artifacts/caches/temp off the C: drive, inject a path-discipline prompt into every session, disk_guard tool for status/cleanup. |
| 678 | [KarthusLorin/dsh-subagent-grok](https://github.com/KarthusLorin/dsh-subagent-grok) | 0 | 2026-08-29 | 2026-08-29 | One-shot Grok CLI subagent provider for DeepSeek Harness |
| 679 | [Kehao/dsh-client-ui-weather](https://github.com/Kehao/dsh-client-ui-weather) | 0 | 2026-08-30 | 2026-08-30 | Deepseek harness 天气插件 |
| 680 | [KeS1Ke/dsh-start-and-exit](https://github.com/KeS1Ke/dsh-start-and-exit) | 0 | 2026-08-24 | 2026-08-27 | dsh-start&exit: safe start, exit, and restart controls for the DeepSeek Harness Web profile, plus a loopback-only Windows foreground launcher. |
| 681 | [KimFischer99/DeepSeek-Harness-Desktop](https://github.com/KimFischer99/DeepSeek-Harness-Desktop) | 0 | 2026-08-15 | 2026-08-27 | 一个轻量的 macOS 桌面应用壳，Rust 编写，承载 DeepSeek Harness WebUI，一键启停 |
| 682 | [kittimzhe/dsh-plugin-authoring-guide](https://github.com/kittimzhe/dsh-plugin-authoring-guide) | 0 | 2026-08-29 | 2026-08-29 | Hands-on guide to building a DeepSeek Harness plugin (EN/ZH) — real code & pitfalls from dsh-session-export and dsh-session-recall |
| 683 | [kivensteven8-eng/dsh-file-download](https://github.com/kivensteven8-eng/dsh-file-download) | 0 | 2026-08-27 | 2026-08-27 | DSH 插件：把会话工作区文件变成浏览器直接下载的 HTTP 通道 —— 为 iPad 等局域网/域名设备设计。 |
| 684 | [KL3jd/handwritten-ocr](https://github.com/KL3jd/handwritten-ocr) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin for local OCR: handwritten Chinese + math → Markdown with LaTeX. GPU / CPU backends. |
| 685 | [knownothing114/dsh-notify](https://github.com/knownothing114/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | A dsh plugin that raises a desktop notification whenever dsh needs your attention. |
| 686 | [kobenfang/BigTimer](https://github.com/kobenfang/BigTimer) | 0 | 2026-08-29 | 2026-08-29 | 🕐 BigTimer · 定时任务+消息推送管家 — Scheduled tasks & message push manager for DeepSeek Harness (dsh) |
| 687 | [Kogisune/dsh-skin-koi-pond](https://github.com/Kogisune/dsh-skin-koi-pond) | 0 | 2026-08-20 | 2026-08-28 | 🎏 锦鲤池塘 · Koi Pond theme for DeepSeek Harness (DSH) WebUI — 动画锦鲤 + 部件拆分 CSS |
| 688 | [konanzheng/dsh-timeline](https://github.com/konanzheng/dsh-timeline) | 0 | 2026-08-26 | 2026-08-27 | show timeline for deepseek harness |
| 689 | [ktao732084-arch/dsh-vibegap](https://github.com/ktao732084-arch/dsh-vibegap) | 0 | 2026-08-27 | 2026-08-27 | Vocabulary flashcards inside the dsh web UI - appear while your agent runs, retreat when it finishes. A VibeGap plugin. |
| 690 | [ktao732084-arch/vibegap](https://github.com/ktao732084-arch/vibegap) | 0 | 2026-08-26 | 2026-08-27 | Mini-window for the gaps in vibe coding: vocabulary flashcards (and more panels) that auto-appear while your AI coding agent runs |
| 691 | [LamplitIsles/dsh-companion](https://github.com/LamplitIsles/dsh-companion) | 0 | 2026-08-30 | 2026-08-30 | dsh as companion ai frontend in Svelte |
| 692 | [LamplitIsles/kepos-tts](https://github.com/LamplitIsles/kepos-tts) | 0 | 2026-08-29 | 2026-08-30 | Qwen/Volcengine TTS for dsh |
| 693 | [Lanzgale/dsh-listener](https://github.com/Lanzgale/dsh-listener) | 0 | 2026-08-30 | 2026-08-30 | 安全版本地语音输入插件 for DeepSeek Harness:同源宿主代理 + 127.0.0.1 + token,SenseVoice-Small INT8 ONNX 本地转写,音频不出网。 |
| 694 | [lasdrder0705/dsh-chat-zone-std](https://github.com/lasdrder0705/dsh-chat-zone-std) | 0 | 2026-08-26 | 2026-08-27 | dsh-std Community v0.15 chat zone: ~/dsh_CHAT/<date>/chatN as Tools and Commands. Install adapter-dsh first. |
| 695 | [lasdrder0705/dsh-pro-vision-std](https://github.com/lasdrder0705/dsh-pro-vision-std) | 0 | 2026-08-26 | 2026-08-27 | dsh-std Community v0.15 ModelProvider: V4-Pro with Flash-Vision captions. Install adapter-dsh first. |
| 696 | [lastplayer82/dsh-sticky-notes](https://github.com/lastplayer82/dsh-sticky-notes) | 0 | 2026-08-27 | 2026-08-27 | 灵感便签 (Sticky Notes) plugin for the dsh web GUI: jot ideas while the agent thinks — without interrupting it. Queue-channel sends/forwards, auto-persist (localStorage + host file), export TXT/JSON/MD, bilingual zh/en. DeepSeek Harness plugin · @lastplayer82/dsh-sticky-notes |
| 697 | [Leo3-7/dsh-obsidian-inbox](https://github.com/Leo3-7/dsh-obsidian-inbox) | 0 | 2026-08-28 | 2026-08-28 | DSH skill: ingest the conclusions/mistakes/projects from conversations into an Obsidian vault via a 7-step workflow with two-level validation. 把对话结论/错题/项目按七步流程整理进 Obsidian 的 DeepSeek Harness 技能。 |
| 698 | [LeoChen98/dsh-worktable-notebook-to-ppt](https://github.com/LeoChen98/dsh-worktable-notebook-to-ppt) | 0 | 2026-08-26 | 2026-08-27 | 基于 dsh-worktable 工作台搭建的「课本到 PPT」自动化工作流插件——在 DeepSeek Harness 中一键将 Jupyter Notebook 转化为专业可编辑的演示文稿（.pptx），让知识沉淀与分享更高效。 |
| 699 | [LeonSone/dsh-question-rail](https://github.com/LeonSone/dsh-question-rail) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: 模仿 deepseek 网页版界面右侧的问题条 — 右缘一条竖向问题栏，列出当前会话每一轮的用户提问，点击平滑滚动定位。DeepSeek Harness right-edge question rail. |
| 700 | [lgquan/dsh-voco](https://github.com/lgquan/dsh-voco) | 0 | 2026-08-27 | 2026-08-27 | Persistent voice conversations for DSH with cloud speech recognition, Edge TTS, and background Agent delegation. |
| 701 | [lhf6623/dsh-thrum](https://github.com/lhf6623/dsh-thrum) | 0 | 2026-08-16 | 2026-08-29 | DeepSeek Harness 输入氛围插件：为输入过程增添氛围。 |
| 702 | [liangminhua/agent-notes-toolkit](https://github.com/liangminhua/agent-notes-toolkit) | 0 | 2026-08-30 | 2026-08-30 | Agent Notes mechanism as a portable toolkit: verification gates, scaffolding CLI, and the AN dsh preset/bundle |
| 703 | [liangsheng999/dsh-client-ui-connection-status](https://github.com/liangsheng999/dsh-client-ui-connection-status) | 0 | 2026-08-26 | 2026-08-27 | DSH Web client plugin: a corner pill showing live connection state for the DeepSeek Harness Web UI. npm: dsh-client-ui-connection-status |
| 704 | [liangsheng999/dsh-dream](https://github.com/liangsheng999/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH host plugin: scheduled background 'dream' (memory consolidation) passes for DeepSeek Harness. npm: dsh-dream |
| 705 | [liangxiaobing520/dsh-local-vector-memory](https://github.com/liangxiaobing520/dsh-local-vector-memory) | 0 | 2026-08-29 | 2026-08-29 | Fully local vector memory plugin for DeepSeek Harness: local embeddings, SQLite storage, automatic recall injection, dedup with conflict detection, soft-delete recycle bin, online backup. |
| 706 | [LianPing-cyber/dsh-browser-full-access](https://github.com/LianPing-cyber/dsh-browser-full-access) | 0 | 2026-08-29 | 2026-08-29 | Full-access background-tab fork of dsh-browser for DeepSeek Harness (DSH). Based on dsh-browser, MCP, and browser-use. |
| 707 | [liceses/dsh-hmm-wait](https://github.com/liceses/dsh-hmm-wait) | 0 | 2026-08-22 | 2026-08-27 | 化口水为乐趣，把大肥鱼流的口水变成游戏连击！ |
| 708 | [Lichtspur/deepseek-style-theme](https://github.com/Lichtspur/deepseek-style-theme) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek official-home style theme for the dsh web GUI: fluid particle background, glass sidebar, glass composer, frosted header, running-subagent progress panel, DSTT time-based mode, and DeepSeek brand link |
| 709 | [lijian-ui/dsh-file-manager](https://github.com/lijian-ui/dsh-file-manager) | 0 | 2026-08-18 | 2026-08-27 | 为 DeepSeek Harness 桌面端（dsh web）开发的插件：聊天区右侧的 Explorer 文件面板 + Preview 预览面板（FileManager 风格，Apache-2.0 参考实现非抄录），以及输入框 @ 引用项目文件（树形多选弹窗 + 输入框内胶囊 + 行号） |
| 710 | [lijian-ui/dsh-schedule-view](https://github.com/lijian-ui/dsh-schedule-view) | 0 | 2026-08-24 | 2026-08-27 | A cron-based scheduled task plugin for DeepSeek Harness (dsh) desktop: create / edit / delete / fire-now tasks from the settings panel, with cross-session agent follow-up and multi-level notifications. Zero LLM tools — purely human-driven scheduling. |
| 711 | [lijian-ui/dsh-skill-manage](https://github.com/lijian-ui/dsh-skill-manage) | 0 | 2026-08-22 | 2026-08-27 | A skill management plugin for DeepSeek Harness (dsh) desktop: list / enable / disable / delete / add skills, filling the gap in dsh's official skill toggle control. |
| 712 | [lijian-ui/dsh-term](https://github.com/lijian-ui/dsh-term) | 0 | 2026-08-19 | 2026-08-27 | Panel-style local terminal for the DSH web GUI. |
| 713 | [lijian-ui/dsh-vision-toggle](https://github.com/lijian-ui/dsh-vision-toggle) | 0 | 2026-08-28 | 2026-08-28 | dsh-vision-toggle 是一个为 DeepSeek Harness (dsh) 提供「支持图片」开关的插件，让你在设置页按模型一键启用/禁用图片输入 |
| 714 | [limlnx523/dsh-plus-plus](https://github.com/limlnx523/dsh-plus-plus) | 0 | 2026-08-27 | 2026-08-28 | DSH++ — a local-first control plane for DeepSeek Harness. Plugin security auditing and workflow regression testing. |
| 715 | [Lion-Li-git/dsh-external-links](https://github.com/Lion-Li-git/dsh-external-links) | 0 | 2026-08-30 | 2026-08-30 | DSH desktop (Deepseek Harness EAC) plugin: open http/https/mailto/tel/file links in the default browser/app, bypassing the broken shell.open-external bridge |
| 716 | [lisongxuan/ds-hentai](https://github.com/lisongxuan/ds-hentai) | 0 | 2026-08-25 | 2026-08-28 | ExHentai-inspired UI for DeepSeek Harness. ExHentai风格DeepSeek Harness皮肤。 ds hentai / deepseek hentai |
| 717 | [liujia-io/dsh-image-picker](https://github.com/liujia-io/dsh-image-picker) | 0 | 2026-08-26 | 2026-08-27 | Paperclip image-picker button for the DeepSeek Harness web composer - pick reference images via the system file dialog and feed them into the official attachment pipeline. |
| 718 | [Liujie-harsh/heart-health-dsh-suite](https://github.com/Liujie-harsh/heart-health-dsh-suite) | 0 | 2026-08-28 | 2026-08-28 | 适配心脏健康场景的 DeepSeek Harness 插件套件：在「心衰辅助诊断算法服务（heart-algo MCP）」之上， 为 DSH 会话提供一组受控的领域包装工具、驻留临床指导与原始工具隐藏策略。 |
| 719 | [liuwenji007/dsh-trust-check](https://github.com/liuwenji007/dsh-trust-check) | 0 | 2026-08-27 | 2026-08-27 | Static capability disclosure for DeepSeek Harness plugins — evidence-backed, zero-token, no safety claims. |
| 720 | [ljc6413/pkg-dev](https://github.com/ljc6413/pkg-dev) | 0 | 2026-08-29 | 2026-08-30 | YiHe 编程认知内核 for DeepSeek Harness：27 领域包 + 55 RFB 经验库 + 工程工具链 + 商业/安全/进化体系（会进化的编程助手） |
| 721 | [LJH-snow/dsh-tool-kubernetes](https://github.com/LJH-snow/dsh-tool-kubernetes) | 0 | 2026-08-27 | 2026-08-27 | Kubernetes tools for DeepSeek Harness: cluster, namespace, workload, pod, log, rollout, and manifest operations |
| 722 | [LJH-snow/dsh-tool-monitoring](https://github.com/LJH-snow/dsh-tool-monitoring) | 0 | 2026-08-28 | 2026-08-28 | Prometheus and Alertmanager tool plugin for DeepSeek Harness |
| 723 | [LJH-snow/dsh-tool-slack](https://github.com/LJH-snow/dsh-tool-slack) | 0 | 2026-08-30 | 2026-08-30 | Slack tools for DeepSeek Harness |
| 724 | [ljlj7149-cloud/dsh-cognitio](https://github.com/ljlj7149-cloud/dsh-cognitio) | 0 | 2026-08-26 | 2026-08-27 | 纠错驱动的认知架构插件（DeepSeek Harness）：分层记忆 + 哨兵自动提醒 + 纠错进化 + 审批仲裁。让 AI 记得你的规矩，换模型换预设都有效；所有自动沉淀，你批准才生效。 |
| 725 | [lkdxzhxi/dsh-glass-ui-theme](https://github.com/lkdxzhxi/dsh-glass-ui-theme) | 0 | 2026-08-29 | 2026-08-29 | 为 DeepSeek Harness 打造的液态玻璃主题插件：磨砂玻璃、可调色调、动态壁纸，让 DSH 界面焕然一新 |
| 726 | [lnetrit-alt/dsh-system-control](https://github.com/lnetrit-alt/dsh-system-control) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: sidebar-embedded DeepSeek balance readout with a black minimalist full-shutdown button. |
| 727 | [loiasdi/dsh-prompthub-ecosystem](https://github.com/loiasdi/dsh-prompthub-ecosystem) | 0 | 2026-08-26 | 2026-08-27 | PromptHub Ecosystem for DeepSeek Harness (DSH): bilingual Plugin and Skill catalog with GitHub and local tarball installation. |
| 728 | [lokih1028/dsh-prompt-optimizer](https://github.com/lokih1028/dsh-prompt-optimizer) | 0 | 2026-08-29 | 2026-08-29 | One-click prompt enhancement and structuring plugin for DeepSeek Harness (DSH) |
| 729 | [Lorvaste/DSH-Project-Initialization](https://github.com/Lorvaste/DSH-Project-Initialization) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：项目初始化插件，通过结构化的整理编排，需求与要素确认，无论是项目刚起步还是准备维护，都有一个好的开始. |
| 730 | [lovstudio/dsh-llm-config](https://github.com/lovstudio/dsh-llm-config) | 0 | 2026-08-29 | 2026-08-29 | Reusable LLM configuration profile library exposed to browser consumers as a Remote (DeepSeek Harness plugin) |
| 731 | [lovstudio/dsh-plugin-marketplace](https://github.com/lovstudio/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Local-first DeepSeek Harness plugin marketplace with GitHub and dshfind providers |
| 732 | [loyalchiiina/dsh-font-enhancer](https://github.com/loyalchiiina/dsh-font-enhancer) | 0 | 2026-08-27 | 2026-08-27 | DIY 你的 DSH 界面：按区域自定义字体/字号/颜色 \| DIY your DSH UI fonts & colors |
| 733 | [Luawig/dsh-cloudflare-access](https://github.com/Luawig/dsh-cloudflare-access) | 0 | 2026-08-27 | 2026-08-27 | Cloudflare Access JWT verification and remote privileged authorization for DeepSeek Harness |
| 734 | [Lubaoshuai/dsh-notify](https://github.com/Lubaoshuai/dsh-notify) | 0 | 2026-08-30 | 2026-08-30 | Push notifications for DeepSeek Harness: agent-callable notify_send tool + external delivery for schedule reminders (Telegram/Slack/Discord/飞书/钉钉/Bark/ntfy/webhook). DSH plugin. |
| 735 | [luckzhangfengbo/dsh-web-theme](https://github.com/luckzhangfengbo/dsh-web-theme) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness 背景主题插件 |
| 736 | [LUMOGRESS/dsh-skill-navigator](https://github.com/LUMOGRESS/dsh-skill-navigator) | 0 | 2026-08-29 | 2026-08-29 | DSH skill quick-picker and manager: one-click quick-pick (categories/search/context recommendations) + management (categories/updates/expert packs/market/panel settings). DSH 技能速查+管理插件。 |
| 737 | [Lunatic029/dsh-clash-proxy](https://github.com/Lunatic029/dsh-clash-proxy) | 0 | 2026-08-27 | 2026-08-27 | Route DeepSeek Harness's outbound network through Clash — LLM, web search/fetch and shell commands all use your local Clash proxy. |
| 738 | [luoghong/dsh-session-recorder](https://github.com/luoghong/dsh-session-recorder) | 0 | 2026-08-29 | 2026-08-30 | 记录和deek Harness对话记录为md格式 |
| 739 | [luomeii/dsh-review-squad](https://github.com/luomeii/dsh-review-squad) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 并行多角色代码评审插件：/review 派出安全/正确性/测试/风格四名只读评审员子代理（可各自指定模型与思考强度），汇总为结构化报告。 |
| 740 | [lussey820/dsh-essentials-bundle](https://github.com/lussey820/dsh-essentials-bundle) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) Web UI all-in-one essentials pack — a bundled collection, not a single-feature plugin: chat wallpaper / token usage stats / session manager / per-turn undo with artifact rollback / built-in file explorer & editor. Zero-dependency, inject-only, never overrides core. |
| 741 | [luxueliu/luxueliu-agent-discipline-skills](https://github.com/luxueliu/luxueliu-agent-discipline-skills) | 0 | 2026-08-25 | 2026-08-27 | AI 不缺聪明，缺纪律！交付前自检（没从磁盘回读不算完成）/跑偏纠偏（一句「你偏了」就停）/系统化调试（同一个修复猜三次不收敛时用）/多 agent 接力（防旧状态盖掉新写入）——4 个单文件技能零依赖，每条都来自真实翻车事故，DeepSeek Harness / Claude Code / Codex 通用 |
| 742 | [luxueliu/luxueliu-intel-scout](https://github.com/luxueliu/luxueliu-intel-scout) | 0 | 2026-08-25 | 2026-08-27 | 每天自动巡 RSS：AI 简报 + 脑神经/意识简报，关键词过滤后压成速览+详情。DSH 插件；脚本仍是 Python / 计划任务。 |
| 743 | [lyaoliu/dsh-reasoning-effort-slider](https://github.com/lyaoliu/dsh-reasoning-effort-slider) | 0 | 2026-08-29 | 2026-08-29 | DSH Desktop reasoning effort slider plugin - 7-level effort control with whale-mom skin |
| 744 | [lylarcher/dsh-model-capabilities](https://github.com/lylarcher/dsh-model-capabilities) | 0 | 2026-08-29 | 2026-08-29 | 一个DSH插件，为自定义模型配置输入类型(input)、推理模式（reasoningEfforts） |
| 745 | [lyuwen/dsh-as-service](https://github.com/lyuwen/dsh-as-service) | 0 | 2026-08-26 | 2026-08-27 | Running DSH as a service on the background |
| 746 | [lyuwen/dsh-steer-button](https://github.com/lyuwen/dsh-steer-button) | 0 | 2026-08-26 | 2026-08-27 | Queue, Steer, and Backlog for DSH. More diverse way to interact with the agent while it's running. |
| 747 | [lyuwen/dsh-thinking-summary](https://github.com/lyuwen/dsh-thinking-summary) | 0 | 2026-08-27 | 2026-08-27 | Readable thinking display for DeepSeek Harness |
| 748 | [lyuwen/dsh-tui](https://github.com/lyuwen/dsh-tui) | 0 | 2026-08-28 | 2026-08-28 | [WIP] TUI for DeepSeeh-Harness |
| 749 | [Lzh3070/dsh-search-hub](https://github.com/Lzh3070/dsh-search-hub) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 联网搜索多入口管理插件：DeepSeek 官方 / GLM（智谱）/ Kimi 多搜索模型共存，置顶一个web_search生效，设置页一键切换免重启 |
| 750 | [LZMW/dsh-memory](https://github.com/LZMW/dsh-memory) | 0 | 2026-08-24 | 2026-08-28 | Persistent long-term memory plugin for DeepSeek Harness (dsh): single memory tool, markdown storage, auto session summary, curator governance, user-profile injection. |
| 751 | [lzxcs/archive-vault-pro](https://github.com/lzxcs/archive-vault-pro) | 0 | 2026-08-26 | 2026-08-27 | 归档会话库：查看所有工作区的已归档会话、只读回看内容、右键取消归档（不影响官方逻辑）。 |
| 752 | [lzxcs/btw-pro](https://github.com/lzxcs/btw-pro) | 0 | 2026-08-26 | 2026-08-27 | /btw 旁路问答：不打断当前会话（含流式输出中），基于当前上下文回答一个问题；答案以「旁答」命令结果行显示在主会话里，不进入主模型上下文。 |
| 753 | [lzxcs/chat-width-pro](https://github.com/lzxcs/chat-width-pro) | 0 | 2026-08-26 | 2026-08-27 | 对话页面宽度设置：把固定的内容宽度暴露到设置页，默认 748px（应用当前宽度）。 |
| 754 | [lzxcs/dsh-enter-swap](https://github.com/lzxcs/dsh-enter-swap) | 0 | 2026-08-26 | 2026-08-27 | Swap the web UI composer shortcuts: Ctrl/Meta+Enter inserts a newline, Shift+Enter sends. |
| 755 | [lzxcs/dsh-tray-notify](https://github.com/lzxcs/dsh-tray-notify) | 0 | 2026-08-26 | 2026-08-27 | DSH → 托盘通知：agent 停顿 / 提问 / 计划审批 / 授权时调用 notify-sender.py 弹窗（--source dsh，托盘按蓝色主题区分于 Claude Code）。纯 node 侧插件。 |
| 756 | [lzxcs/edit-diff-pro](https://github.com/lzxcs/edit-diff-pro) | 0 | 2026-08-26 | 2026-08-27 | Claude Code 风格的 edit/write diff 卡片：±3 行上下文、绝对行号、可配置默认展开（默认折叠）。 |
| 757 | [lzxcs/file-diff-pro](https://github.com/lzxcs/file-diff-pro) | 0 | 2026-08-26 | 2026-08-27 | 产物文件点击弹窗查看本轮 diff（代码类文件）；非代码文件维持桌面打开。 |
| 758 | [lzxcs/lag-trace-pro](https://github.com/lzxcs/lag-trace-pro) | 0 | 2026-08-26 | 2026-08-27 | DSH web UI performance recorder: auto-captures page jank (long animation frames, long tasks, frame freezes) with context snapshots, stored under ~/.dsh/perf/ |
| 759 | [lzxcs/paste-file-path-pro](https://github.com/lzxcs/paste-file-path-pro) | 0 | 2026-08-26 | 2026-08-27 | Pasting non-image files into the web composer inserts their paths as @file references (host-side clipboard reading). |
| 760 | [makajo/dsh-gemini-m3e-theme](https://github.com/makajo/dsh-gemini-m3e-theme) | 0 | 2026-08-29 | 2026-08-30 | Gemini-style Material 3 Expressive theme for DeepSeek Harness Web (persistent client bundle) |
| 761 | [mapan0424/deepseek-harness-channels](https://github.com/mapan0424/deepseek-harness-channels) | 0 | 2026-08-28 | 2026-08-28 | Community channel plugins for DeepSeek Harness: core, visual config, and Feishu channel. |
| 762 | [MarceloSenai/dsh-plugin-kie-ai](https://github.com/MarceloSenai/dsh-plugin-kie-ai) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: image and video generation over the KIE AI API |
| 763 | [MaRi23333/dsh-serverchan-watchdog](https://github.com/MaRi23333/dsh-serverchan-watchdog) | 0 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 的 Server酱推送插件：审批、计划评审或问答超时未处理时，发送微信/Server酱³ App 提醒。第三方非官方项目。 |
| 764 | [masknull/dsh-workspace-default-path](https://github.com/masknull/dsh-workspace-default-path) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：添加工作区时记住上次使用的目录，下次打开浏览对话框直接定位（预填+自动记忆，官方流程不动）。DSH plugin: remember the last used workspace directory for Add workspace - prefill + auto-memory over the official flow. |
| 765 | [Mason-1011/dsh-schematic](https://github.com/Mason-1011/dsh-schematic) | 0 | 2026-08-25 | 2026-08-30 | Live plugin-topology viewer for DeepSeek Harness — the wiring diagram of mounted plugins, their runtime activity, and a composer-side star map. Pure observer. |
| 766 | [MauricioPerera/kdd-gates](https://github.com/MauricioPerera/kdd-gates) | 0 | 2026-08-27 | 2026-08-27 | KDD methodology gates as DeepSeek Harness (dsh) plugin tools |
| 767 | [me9rez/dsh-pwsh-style](https://github.com/me9rez/dsh-pwsh-style) | 0 | 2026-08-28 | 2026-08-28 | 修改 DSH 会话回复中 pwsh(PowerShell) 工具卡片的主题、字体与可读性增强。Restyle pwsh tool-call cards in DSH: themes, system fonts, copy & expand, workdir display. |
| 768 | [Mengshang-spec/dsh-third-party-api-balance-wallet](https://github.com/Mengshang-spec/dsh-third-party-api-balance-wallet) | 0 | 2026-08-27 | 2026-08-27 | 第三方 API 接入 DSH 查询余额插件 |
| 769 | [meyaomiao/dsh-files-native](https://github.com/meyaomiao/dsh-files-native) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件：接近原生质感的附件上传（拖入/粘贴/回形针，图片与文件混排） |
| 770 | [MichaelGong/dsh-session-hover-preview](https://github.com/MichaelGong/dsh-session-hover-preview) | 0 | 2026-08-27 | 2026-08-27 | Codex-style user-message navigation for DeepSeek Harness conversations |
| 771 | [Mide69/dsh-boot-doctor](https://github.com/Mide69/dsh-boot-doctor) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: console log sink and stuck-plugin warnings |
| 772 | [mingzhong15/dsh-cursor-passthrough](https://github.com/mingzhong15/dsh-cursor-passthrough) | 0 | 2026-08-27 | 2026-08-27 | Add a Cursor passthrough group to the DSH chat model picker. |
| 773 | [Missher12/dsh-project-ops](https://github.com/Missher12/dsh-project-ops) | 0 | 2026-08-27 | 2026-08-27 | Scoped project task discovery and execution receipts for DeepSeek Harness |
| 774 | [ml020/dsh-workbuddy](https://github.com/ml020/dsh-workbuddy) | 0 | 2026-08-28 | 2026-08-28 | Wordless-styled WorkBuddy hero for DSH: replaces the blank-session brand mark and workspace picker while keeping the native composer. |
| 775 | [Momojie-S/dsh-archive-retention](https://github.com/Momojie-S/dsh-archive-retention) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件: 归档会话定期清理 —— 物理归档堆与页面归档会话超保留期(页面可配天/小时,cron 调度)自动物理删除 |
| 776 | [Moonshile/moonshile-dsh-plugins](https://github.com/Moonshile/moonshile-dsh-plugins) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) plugins — dsh-workspace-sort: re-sorts sidebar workspaces by last activity once per day. One-command npm bundle install. |
| 777 | [moonwellxh/DSH-Launcher](https://github.com/moonwellxh/DSH-Launcher) | 0 | 2026-08-27 | 2026-08-30 | DSH 魔偶助手（DSH一键启动托盘）(DeepSeek Harness launcher / tray) |
| 778 | [morphlinglan/dsh-leopard-gecko](https://github.com/morphlinglan/dsh-leopard-gecko) | 0 | 2026-08-28 | 2026-08-28 | 豹纹守宫旅行桌宠小插件：一只会自己出门旅行、寄回明信片、带回特产的守宫。庭院三叶草随时间生长，收割后可在商店购买便当与护身符。 |
| 779 | [mtdx2001/dsh-think-translate](https://github.com/mtdx2001/dsh-think-translate) | 0 | 2026-08-29 | 2026-08-29 | Display-layer translation for the DeepSeek Harness Web UI: thinking chain, task cards and answers in 8 languages - pure display layer, originals untouched, local-first with failover. |
| 780 | [my-dsh/dsh-session-attention](https://github.com/my-dsh/dsh-session-attention) | 0 | 2026-08-28 | 2026-08-28 | Session attention overlay plugin for DeepSeek Harness: character dance animation while any session awaits user action |
| 781 | [my-dsh/dsh-token-usage-dashboard](https://github.com/my-dsh/dsh-token-usage-dashboard) | 0 | 2026-08-28 | 2026-08-28 | Cross-session token usage dashboard plugin for DeepSeek Harness: SQLite-backed capture + browser dashboard panel |
| 782 | [mycodesite/dsh-rules](https://github.com/mycodesite/dsh-rules) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (dsh) 插件：全局+项目两级 Markdown 规则注入（RuleBase） |
| 783 | [mykeura/dsh-minimalist-themes](https://github.com/mykeura/dsh-minimalist-themes) | 0 | 2026-08-26 | 2026-08-27 | 18 minimalist color themes for DeepSeek Harness. Pick one with a single click — it's just another plugin. |
| 784 | [N9-Developer-Empowerment/DSH-Vibeify](https://github.com/N9-Developer-Empowerment/DSH-Vibeify) | 0 | 2026-08-26 | 2026-08-29 | Turn AI work into a living local magazine for DeepSeek Harness. DeepSeek, ChatGPT, or both. |
| 785 | [Nath-Vikky/dsh-codekin](https://github.com/Nath-Vikky/dsh-codekin) | 0 | 2026-08-24 | 2026-08-28 | Codekin: a creature-collection and match-three RPG for DeepSeek Harness Web. |
| 786 | [navid-kianfar/dsh-memory](https://github.com/navid-kianfar/dsh-memory) | 0 | 2026-08-26 | 2026-08-27 | Persistent, searchable, per-project memory for the DeepSeek Harness: decisions, rules, and session context in a queryable DuckDB file, with the rule set injected into every model request — plus a full management UI in the Web Client. |
| 787 | [navid-kianfar/dsh-worktree](https://github.com/navid-kianfar/dsh-worktree) | 0 | 2026-08-26 | 2026-08-27 | Git worktrees and branches for the DeepSeek Harness Web Client: a session-header chip that switches branches, creates worktrees, and opens them as harness workspaces. |
| 788 | [NecromanAlbert/dsh-i-have-adhd](https://github.com/NecromanAlbert/dsh-i-have-adhd) | 0 | 2026-08-26 | 2026-08-27 | Always-on ADHD-friendly output for every DeepSeek Harness session. Host systemPrompt, not a skill catalog item. |
| 789 | [NecromanAlbert/dsh-self-restart](https://github.com/NecromanAlbert/dsh-self-restart) | 0 | 2026-08-26 | 2026-08-27 | Any DSH session can request a Desktop restart, then the same persisted session is resumed and followup'd with its mission. |
| 790 | [NexusAgentX/dsh-advisor](https://github.com/NexusAgentX/dsh-advisor) | 0 | 2026-08-23 | 2026-08-27 | dsh plugin bundle porting the rpiv advisor subsystem: an on-demand zero-parameter advisor() tool that forwards the full session to a separately-configured reviewer model. |
| 791 | [nicecx/dsh-reset-handoff](https://github.com/nicecx/dsh-reset-handoff) | 0 | 2026-08-30 | 2026-08-30 | DSH never restarts itself: host plugin that hands reset requests to an external ops agent (e.g. Hermes) via a versioned JSON protocol — preflight → gate → restart → health-check → recover → deliver back |
| 792 | [nickkkkkk123123/dsh-resume-on-restart](https://github.com/nickkkkkk123123/dsh-resume-on-restart) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：重启后自动唤醒 agent 并投递信息性消息，agent 自主决定是否恢复工作 |
| 793 | [nickkkkkk123123/dsh-whale-girl](https://github.com/nickkkkkk123123/dsh-whale-girl) | 0 | 2026-08-27 | 2026-08-27 | 鲸鱼娘·灵动挂件 — 会卖萌、会记账、会弹跳的 DSH 桌面挂件插件（余额/用量/上下文/峰谷/右键菜单/拖动甩抛） |
| 794 | [niushuanan/dsh-adaptive-update](https://github.com/niushuanan/dsh-adaptive-update) | 0 | 2026-08-26 | 2026-08-27 | Check upstream manually or every six hours, use a narrowly scoped agent for compatibility work, and switch atomically with rollback. |
| 795 | [niushuanan/dsh-chat-migration](https://github.com/niushuanan/dsh-chat-migration) | 0 | 2026-08-29 | 2026-08-29 | Native DeepSeek chat migration and workspace-free chat mode for DeepSeek Harness |
| 796 | [niushuanan/dsh-image-vision](https://github.com/niushuanan/dsh-image-vision) | 0 | 2026-08-26 | 2026-08-27 | Let vision-capable models read native attachments while giving text-only models an image tool that supports follow-up questions. |
| 797 | [niushuanan/dsh-model-usage](https://github.com/niushuanan/dsh-model-usage) | 0 | 2026-08-26 | 2026-08-27 | Inspect model quotas, periods, and refresh state by provider in Settings, with data loaded only when the user opens the page. |
| 798 | [niushuanan/dsh-multi-window](https://github.com/niushuanan/dsh-multi-window) | 0 | 2026-08-26 | 2026-08-27 | Open multiple independent conversations side by side, each with isolated navigation, drafts, and runtime state. |
| 799 | [niushuanan/dsh-parallel-worktree](https://github.com/niushuanan/dsh-parallel-worktree) | 0 | 2026-08-26 | 2026-08-27 | Move parallel tasks into isolated Git worktrees, inspect conflicts, and merge the results safely into the current branch. |
| 800 | [niushuanan/dsh-pure-chat](https://github.com/niushuanan/dsh-pure-chat) | 0 | 2026-08-26 | 2026-08-27 | Start a chat immediately without a workspace, work mode, or execution permissions while keeping image and text-file uploads. |
| 801 | [niushuanan/dsh-selection-memory](https://github.com/niushuanan/dsh-selection-memory) | 0 | 2026-08-26 | 2026-08-27 | Quote, discuss, or remember selected conversation text, then maintain durable context in separate editable user and AI memories. |
| 802 | [niushuanan/dsh-skill-manager](https://github.com/niushuanan/dsh-skill-manager) | 0 | 2026-08-26 | 2026-08-27 | Browse installed Skills, their files, and content in Settings, then adaptively import from a file, folder, ZIP, or GitHub with AI. |
| 803 | [niushuanan/dsh-teamwork](https://github.com/niushuanan/dsh-teamwork) | 0 | 2026-08-26 | 2026-08-27 | Run collaborating agents and external experts concurrently under one coordinating agent, then bring every result back into the current task. |
| 804 | [niushuanan/dsh-token-overview](https://github.com/niushuanan/dsh-token-overview) | 0 | 2026-08-26 | 2026-08-27 | See tokens, cache usage, calls, active periods, and estimated cost across AI clients on the whole computer. |
| 805 | [niushuanan/dsh-whale-girl](https://github.com/niushuanan/dsh-whale-girl) | 0 | 2026-08-26 | 2026-08-27 | Add a native cross-page companion whose presence, shortcuts, and feedback follow the current DSH session state. |
| 806 | [Noemm/dsh-web-search-glm](https://github.com/Noemm/dsh-web-search-glm) | 0 | 2026-08-28 | 2026-08-28 | Zhipu GLM search provider for the DeepSeek Harness (dsh) web seam — native web_search via the Anthropic-compatible API |
| 807 | [NOirBRight/dsh-mobile-pairing](https://github.com/NOirBRight/dsh-mobile-pairing) | 0 | 2026-08-21 | 2026-08-29 | DSH Mobile Remote pairing plugin |
| 808 | [NOirBRight/dsh-model-switch](https://github.com/NOirBRight/dsh-model-switch) | 0 | 2026-08-19 | 2026-08-29 | Model purposes spec and tickets for DeepSeek Harness |
| 809 | [NOirBRight/dsh-plugins](https://github.com/NOirBRight/dsh-plugins) | 0 | 2026-08-29 | 2026-08-30 | Independent catalog of DSH plugins and mobile companion published by NOirBRight |
| 810 | [Nth-5620/dsh-crystal-viewer](https://github.com/Nth-5620/dsh-crystal-viewer) | 0 | 2026-08-29 | 2026-08-30 | A crystal-structure visualization window for DeepSeek Harness: 3D structure + Q-peak viewer and parameter panel, opened as a dsh-better-sidebar tab. |
| 811 | [NyaaCaster/dsh-yuque-kb](https://github.com/NyaaCaster/dsh-yuque-kb) | 0 | 2026-08-24 | 2026-08-28 | dsh web插件，语雀文档知识库化在dsh中调用 |
| 812 | [oh-summy/dsh-remote-control](https://github.com/oh-summy/dsh-remote-control) | 0 | 2026-08-30 | 2026-08-30 | Secure remote access for DeepSeek Harness (DSH): Cloudflare Tunnel + password gate + Feishu notifications. macOS first, Linux first-class. |
| 813 | [Olina1Ye/internal-skill-workshop-plugin](https://github.com/Olina1Ye/internal-skill-workshop-plugin) | 0 | 2026-08-27 | 2026-08-27 | A read-only DeepSeek Harness Web plugin for browsing a configured Skill Base catalog. |
| 814 | [Oliver0804/dsh-openrouter-monitor](https://github.com/Oliver0804/dsh-openrouter-monitor) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: OpenRouter account balance, per-key spend, alert thresholds and trend charts under the composer. |
| 815 | [Oliver0804/dsh-peak-pricing](https://github.com/Oliver0804/dsh-peak-pricing) | 0 | 2026-08-17 | 2026-08-27 | DSH plugin: DeepSeek peak/off-peak pricing, flat rates for other providers like z-ai/glm-5.3-flash, live per-session cost estimate and a hover cache-hit trend chart. |
| 816 | [Olympianz/dsh-deploy-master](https://github.com/Olympianz/dsh-deploy-master) | 0 | 2026-08-30 | 2026-08-30 | A DSH deploy-assistant plugin: GitHub publish + Linear sync + npm publish + community announcement. |
| 817 | [Olympianz/dsh-heatmap](https://github.com/Olympianz/dsh-heatmap) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 页面埋点与热力图分析插件：科学埋点采集、本地热力图与统计、CLI/HTTP 接口、上传授权。 |
| 818 | [onclaw-dev/dsh-ima-copilot](https://github.com/onclaw-dev/dsh-ima-copilot) | 0 | 2026-08-30 | 2026-08-30 | 腾讯 IMA 是一个非常好的知识库应用，但是他们提供的skill版本针对公开知识库的检索方式只提供了基于文件标题的关键字检索，好一阵无语。为了补足在harness的这种知识库检索能力，基于tencent-ima-copilot-mcp迭代了对应的dsh版本。 |
| 819 | [opdsh/unity-plugin](https://github.com/opdsh/unity-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: control the Unity Editor through the unity CLI |
| 820 | [Oscar-Williams/dsh-deepcanary](https://github.com/Oscar-Williams/dsh-deepcanary) | 0 | 2026-08-29 | 2026-08-30 | Local attention supervision for DeepSeek Harness: evidence-first signals, quiet notifications, and an actionable inbox. |
| 821 | [oThTJx/dsh-always-apply](https://github.com/oThTJx/dsh-always-apply) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: injects alwaysApply-marked skill bodies into sessions before the first model request — no skill tool load needed. |
| 822 | [oThTJx/dsh-superpowers](https://github.com/oThTJx/dsh-superpowers) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: obra/superpowers skill library adapted to dsh tooling, plus a session-start bootstrap — brainstorming, systematic debugging, TDD, planning and more. |
| 823 | [pacoyi/dsh-memory-lite](https://github.com/pacoyi/dsh-memory-lite) | 0 | 2026-08-28 | 2026-08-28 | Lightweight cross-session memory plugin for DeepSeek Harness |
| 824 | [PaidaxingTuT/dsh-code-runner](https://github.com/PaidaxingTuT/dsh-code-runner) | 0 | 2026-08-29 | 2026-08-29 | 在 DSH-better-sidebar 中一键运行侧边栏代码文件，让代码可以在dsh终端中运行 |
| 825 | [Parker-xia/dsh-research-refs](https://github.com/Parker-xia/dsh-research-refs) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: tidy messy pasted citations into uniformly formatted references (refs_parse / refs_verify / refs_dedup / refs_format + research-refs skill) |
| 826 | [pauloapoloni/dsh-pr-checks](https://github.com/pauloapoloni/dsh-pr-checks) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: status and progress of GitHub Actions checks for open PRs, in the sidebar footer. |
| 827 | [peikuo/dayreel](https://github.com/peikuo/dayreel) | 0 | 2026-08-30 | 2026-08-30 | Dayreel — a DeepSeek Harness (dsh) community plugin: turn your day of work sessions into a designed daily report + a narrated summary video. |
| 828 | [peiyucn/dsh-sparrow](https://github.com/peiyucn/dsh-sparrow) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness Web 插件小合集（dsh-chat-fim / dsh-vision-access / dsh-archive-session） |
| 829 | [perinchiang/dsh-memory-dashboard](https://github.com/perinchiang/dsh-memory-dashboard) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness embedded read-only viewer for TencentDB Agent Memory's four-layer local memory |
| 830 | [PerryLink/dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) | 0 | 2026-08-29 | 2026-08-30 | Community certification spec and registry for DeepSeek Harness plugins: five machine-checkable dimensions, A-D grades, and a security veto. |
| 831 | [PerryLink/dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) | 0 | 2026-08-26 | 2026-08-27 | Shared zero-runtime-dependency toolkit for PerryLink DSH plugins: a pluggable Provider registry seam, fail-closed approval and adaptive session-event gates, mechanical verify scripts, shared sanitize/pricing/judge modules, and a new-plugin skeleton. |
| 832 | [PerryLink/dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | 0 | 2026-08-26 | 2026-08-27 | Zero-dependency static portal rendering the @perrylink DeepSeek Harness plugin ecosystem as grouped cards: one page, no build step, no runtime framework. |
| 833 | [PerryLink/perrylink](https://github.com/PerryLink/perrylink) | 0 | 2026-08-16 | 2026-08-30 | DeepSeek Harness ecosystem: 33 plugins - second-model approval, permission rules, memory, MCP panel, supply-chain security & certification |
| 834 | [ping1999/dsh-minimap](https://github.com/ping1999/dsh-minimap) | 0 | 2026-08-29 | 2026-08-29 | VS Code-style minimap (text thumbnail + draggable viewport) overlay for the dsh web GUI's side file viewer |
| 835 | [pipipigu/dsh-ssh-control](https://github.com/pipipigu/dsh-ssh-control) | 0 | 2026-08-28 | 2026-08-28 | Unified, non-intrusive SSH control center for DeepSeek Harness (DSH) |
| 836 | [pixellover1433/dsh-plugin-dev-skills](https://github.com/pixellover1433/dsh-plugin-dev-skills) | 0 | 2026-08-30 | 2026-08-30 | This set of skills allows your agent to create plugins for Deepseek Harness. |
| 837 | [PlusQi/dsh-plugins](https://github.com/PlusQi/dsh-plugins) | 0 | 2026-08-28 | 2026-08-27 | 个人 DeepSeek Harness (DSH) 插件集 |
| 838 | [PolinniZhong/dsh-skill-trace](https://github.com/PolinniZhong/dsh-skill-trace) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Skill 追踪：看清 Agent 实际加载的 Skill，把运行过程变成可复看、可学习的本地收据。 |
| 839 | [Proton1917/dsh-harness-plugin](https://github.com/Proton1917/dsh-harness-plugin) | 0 | 2026-08-17 | 2026-08-28 | Independent TypeScript plugins for DeepSeek Harness: live stats, Web UI customization, and a medical Fable mode |
| 840 | [publieople/dsh-omniroute-models](https://github.com/publieople/dsh-omniroute-models) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: searchable/filterable model manager for OmniRoute (or any OpenAI-compatible gateway) — provider directory, modality discovery, multi-select enable. |
| 841 | [QChengW/dsh-conversation-shortcuts](https://github.com/QChengW/dsh-conversation-shortcuts) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin for conversation keyboard shortcuts |
| 842 | [qgx1992/dsh-model-select-style](https://github.com/qgx1992/dsh-model-select-style) | 0 | 2026-08-27 | 2026-08-27 | DSH web 插件：把输入框模型选择控件替换为两个独立按钮（供应商 + 模型两级联动，支持推理等级调节） |
| 843 | [qgx1992/dsh-notify](https://github.com/qgx1992/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | DSH 通知显示层插件：全局 toast 栈，订阅桌面壳 __dshExo 桥事件，点击经官方 sessions runtime 程序化激活会话；无壳时降级订阅 sessions store 自绘。可插拔通知显示层的 web 侧。 |
| 844 | [qipenglin/dsh-plugin-manager](https://github.com/qipenglin/dsh-plugin-manager) | 0 | 2026-08-28 | 2026-08-29 | Profile plugin manager for DeepSeek Harness |
| 845 | [qipenglin/dsh-theme-spectrum](https://github.com/qipenglin/dsh-theme-spectrum) | 0 | 2026-08-28 | 2026-08-29 | Light and dark theme presets for DeepSeek Harness Web |
| 846 | [qipenglin/dsh-web-access](https://github.com/qipenglin/dsh-web-access) | 0 | 2026-08-27 | 2026-08-27 | Optional Web access authentication plugin for DeepSeek Harness |
| 847 | [qt-11564/dsh-git-seam](https://github.com/qt-11564/dsh-git-seam) | 0 | 2026-08-29 | 2026-08-29 | Structured git tools for DeepSeek Harness: diff-before-commit gate + deterministic porcelain parsing (Chinese/UTF-8 paths, Windows) |
| 848 | [QuanQQQ/dsh-plugin-dev-manager](https://github.com/QuanQQQ/dsh-plugin-dev-manager) | 0 | 2026-08-24 | 2026-08-27 | Stable control plane for isolated DeepSeek Harness plugin development |
| 849 | [QWE13-ART/dsh-skill-folder](https://github.com/QWE13-ART/dsh-skill-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH skill catalog prompt surface: static KV-cache-stable catalog + BM25/bge-m3 hybrid skill_search + autoRoute hints. v0.3.0. npm: dsh-skill-folder |
| 850 | [QWE13-ART/dsh-tool-folder](https://github.com/QWE13-ART/dsh-tool-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH tool surface per request + ChainGuard firewall (high-risk block + exfil-chain detection + anti-obfuscation) + BM25/bge-m3 hybrid tools_search. Shrinks schema tokens 80-90% while keeping selection accuracy. v0.2.0 adds a semantic retrieval leg (local Ollama bge-m3, RRF hybrid) and ChainGuard obfuscation detection. npm: dsh-tool-folder |
| 851 | [RaberShef/dsh-pin-session](https://github.com/RaberShef/dsh-pin-session) | 0 | 2026-08-26 | 2026-08-27 | Pin DSH sessions to the top of the sidebar and mark them unread for later. |
| 852 | [raktim-mondol/dsh-researchcraft](https://github.com/raktim-mondol/dsh-researchcraft) | 0 | 2026-08-28 | 2026-08-28 | ResearchCraft as a DeepSeek Harness (DSH) profile plugin: research persona, scientific skills catalogue, living lab notebook, and specialist subagents. |
| 853 | [randomix777/dsh-plugin-subscriptions](https://github.com/randomix777/dsh-plugin-subscriptions) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: OAuth sign-in for Claude, Codex, Grok, Antigravity, OpenRouter, Agnes AI — expose subscription LLMs as DeepSeek Harness providers |
| 854 | [Ranz-Feng/dsh-web-import](https://github.com/Ranz-Feng/dsh-web-import) | 0 | 2026-08-26 | 2026-08-27 | Import DeepSeek Web (chat.deepseek.com) chat history into DeepSeek Harness as resumable, workspace-grouped sessions with original titles preserved. |
| 855 | [renat3u/dsh-upgrade-skill](https://github.com/renat3u/dsh-upgrade-skill) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件升级适配skill |
| 856 | [renchengxiang/dsh-web-search-tavily](https://github.com/renchengxiang/dsh-web-search-tavily) | 0 | 2026-08-28 | 2026-08-28 | Tavily-backed web search provider for DeepSeek Harness, with Settings → Plugins configuration UI |
| 857 | [Reseezhang/vizcb-codeblock-visualizer](https://github.com/Reseezhang/vizcb-codeblock-visualizer) | 0 | 2026-08-28 | 2026-08-29 | DeepSeek Harness 可视化插件：svg/html/mermaid 代码块渲染为图表卡片（宿主端 mermaid、深色主题配色、节点文字自适应、灯箱、保存导出） |
| 858 | [rm-Vstar/web-search-tinyfish](https://github.com/rm-Vstar/web-search-tinyfish) | 0 | 2026-08-28 | 2026-08-28 | A TinyFish web searching plugin for Deepseek Harness |
| 859 | [robbin810130/dsh-vault-plugin](https://github.com/robbin810130/dsh-vault-plugin) | 0 | 2026-08-24 | 2026-08-27 | DSH 保险箱插件：项目与对话的前台隐私锁 |
| 860 | [rogerdigital/dsh-vet](https://github.com/rogerdigital/dsh-vet) | 0 | 2026-08-29 | 2026-08-29 | Security vetting for DeepSeek Harness (DSH) plugins: permission & supply-chain audits before install, graded via the open dsh-vet/v1 report standard. |
| 861 | [Rudyy898/dsh-drag-path](https://github.com/Rudyy898/dsh-drag-path) | 0 | 2026-08-27 | 2026-08-27 | dsh-plugin |
| 862 | [Ruixinhua/dsh-universe-api](https://github.com/Ruixinhua/dsh-universe-api) | 0 | 2026-08-27 | 2026-08-27 | Offline, deterministic public API discovery for DeepSeek Harness and DSH Desktop. |
| 863 | [ruiyukirin/dsh-douyin-oem-touliu-report](https://github.com/ruiyukirin/dsh-douyin-oem-touliu-report) | 0 | 2026-08-28 | 2026-08-28 | 抖音本地推 OEM 投流日报/周报自动化插件 - Douyin OEM ad daily/weekly report automation plugin for DeepSeek Harness (Author: Kirin) |
| 864 | [runcat-tommy/dsh-plugin-runcat-inventory](https://github.com/runcat-tommy/dsh-plugin-runcat-inventory) | 0 | 2026-08-26 | 2026-08-28 | 逃咪-插件总览（Runcat Plugin Overview）—— 更好用的 DSH 插件列表：表格视图、状态过滤、启用/停用开关（热生效）、配置查看与复制、中英双语界面。 |
| 865 | [runcat-tommy/dsh-theme-manager](https://github.com/runcat-tommy/dsh-theme-manager) | 0 | 2026-08-28 | 2026-08-28 | Two-level theme manager for DeepSeek Harness Web: pick a culture/scene or a national flag first, then a concrete style. 40 built-in styles (ink wash, ukiyo-e, Suzhou garden, cyberpunk, 20 flags & more). |
| 866 | [runcat-tommy/dsh-view-manager](https://github.com/runcat-tommy/dsh-view-manager) | 0 | 2026-08-27 | 2026-08-28 | Manage DeepSeek Harness Web GUI view tabs (Chat/Trajectory): enable, hide, reorder & rename with zh/en locale. |
| 867 | [RyanShen3/dsh-toutiao-reader](https://github.com/RyanShen3/dsh-toutiao-reader) | 0 | 2026-08-29 | 2026-08-29 | 读网页/头条文章全文的 DSH 插件：webfetch 工具 + toutiao-reader 经验技能 |
| 868 | [Rycbartbad/dsh-key-manager](https://github.com/Rycbartbad/dsh-key-manager) | 0 | 2026-08-29 | 2026-08-29 | Multiple API keys per provider for DeepSeek Harness: pools with notes, one-click switching that really takes effect |
| 869 | [Ryu6Zero/dsh-hindsight](https://github.com/Ryu6Zero/dsh-hindsight) | 0 | 2026-08-25 | 2026-08-27 | 🧠 Cross-session memory for DeepSeek Harness backed by Hindsight. Self-contained dsh-plugin: /hindsight commands + hindsight_recall/remember/status/list/forget agent tools. Lightweight, no dsh-mnemon, no orchestrator. |
| 870 | [sANDzER0/dsh-hippocampus](https://github.com/sANDzER0/dsh-hippocampus) | 0 | 2026-08-26 | 2026-08-27 | Cross-session project memory for DeepSeek Harness — capture / consolidate / recall, keyword + optional local-Ollama semantic search. Inspired by magic-context. |
| 871 | [saqie803/ponytail](https://github.com/saqie803/ponytail) | 0 | 2026-08-29 | 2026-08-29 | Ship production-ready code with one line of AI-generated output, built for 20 agents and zero ceremony. |
| 872 | [sdoygb/geometry-knowledge](https://github.com/sdoygb/geometry-knowledge) | 0 | 2026-08-26 | 2026-08-27 | 几何论（共扼谱几何 CSG）知识库插件 for DeepSeek Harness: 纯离线 BM25 检索，零运行时依赖 |
| 873 | [seewhydee/dsh-emacs-bridge](https://github.com/seewhydee/dsh-emacs-bridge) | 0 | 2026-08-23 | 2026-08-27 | Deepseek Harness to Emacs bridge |
| 874 | [seiriosPlus/miaoda_for_deepseek_harness](https://github.com/seiriosPlus/miaoda_for_deepseek_harness) | 0 | 2026-08-26 | 2026-08-29 | miaoda_for_deepseek harness |
| 875 | [SeverusZh/dsh-ollama-usage](https://github.com/SeverusZh/dsh-ollama-usage) | 0 | 2026-08-27 | 2026-08-27 | Ollama Cloud 用量余量可视化 DeepSeek Harness 插件:5h 会话/周用量双横条 + 设置页面板,Key 与快照持久化,自动刷新,登录引导。Ollama Cloud usage & quota visualization plugin for DeepSeek Harness. |
| 876 | [ShadowQuill/DialogueContextBridge](https://github.com/ShadowQuill/DialogueContextBridge) | 0 | 2026-08-26 | 2026-08-27 | 对话上下文桥接 — 为大语言模型(LLM)/AI 智能体的对话做跨会话上下文桥接的 DSH 插件：把一次对话的共识打包成可移植快照，一键引入新对话（三层快照 / SQLite+FTS5 / AES-256-GCM） |
| 877 | [shaneconner/canon](https://github.com/shaneconner/canon) | 0 | 2026-08-10 | 2026-08-30 | Canonical project memory for the Pi coding agent: one governing article per asset, an append-only journal, capsule surfacing. A project wiki with a spine. |
| 878 | [ShanHaiFish/dsh-theme-brick](https://github.com/ShanHaiFish/dsh-theme-brick) | 0 | 2026-08-30 | 2026-08-30 | DSH 主题插件（Brick/砌砖）：纯 token 覆盖层，暖石膏与火烧黏土、灰缝线条、一砖一色，零全局 CSS；Settings → General 开关可随时关闭还原。A restrained token-only theme for DeepSeek Harness web — plaster & fired-clay, one accent, no global CSS, with an on/off switch. |
| 879 | [shaomingbo/dsh-open-in-editor](https://github.com/shaomingbo/dsh-open-in-editor) | 0 | 2026-08-26 | 2026-08-27 | Open DSH Web produced files in a configurable local macOS IDE |
| 880 | [shaomingbo/dsh-subscription-antigravity](https://github.com/shaomingbo/dsh-subscription-antigravity) | 0 | 2026-08-29 | 2026-08-29 | Google Antigravity subscription reuse for DeepSeek Harness: browser PKCE sign-in, loopback OpenAI-compatible proxy to Cloud Code Assist, Gemini/Claude/GPT-OSS model routes. |
| 881 | [shaomingbo/dsh-token-usage](https://github.com/shaomingbo/dsh-token-usage) | 0 | 2026-08-30 | 2026-08-30 | Accounts, subscription allowance observations, and local usage ledger for DeepSeek Harness |
| 882 | [shengmk/godsh](https://github.com/shengmk/godsh) | 0 | 2026-08-28 | 2026-08-28 | godsh - GUI launcher for DeepSeek Harness (dsh): manage profiles, plugins, kernels, and dsh versions |
| 883 | [shengyvself/narrative-prompt-polish](https://github.com/shengyvself/narrative-prompt-polish) | 0 | 2026-08-28 | 2026-08-30 | DSH 插件：主输入框 ✨ 一键把草稿润色成清晰、可执行的提示词，经 better-sidebar 侧栏对话多轮打磨后回填。A DSH plugin: ✨ one-click draft polish into agent-ready prompts, multi-turn side-chat via better-sidebar (>=0.16.1). |
| 884 | [ShenXuAkaEkstasis/dsh-ai-shopping-assistant](https://github.com/ShenXuAkaEkstasis/dsh-ai-shopping-assistant) | 0 | 2026-08-28 | 2026-08-28 | AI Shopping Assistant plugin for DeepSeek Harness (DSH), with product comparison, price analysis, merchant/review evidence and source-quality checks. |
| 885 | [shimingming520/dsh-audiogen](https://github.com/shimingming520/dsh-audiogen) | 0 | 2026-08-28 | 2026-08-29 | AI audio generation plugin for the DeepSeek Harness web GUI: multi-vendor TTS, music, sound effects and voice design with a sidebar panel, model comparison, resource library and Agent tools. |
| 886 | [shuaweng/DSH_xieshujing](https://github.com/shuaweng/DSH_xieshujing) | 0 | 2026-08-30 | 2026-08-30 | 写书鲸：面向 DeepSeek Harness 的原生 AI 小说创作工作台插件 |
| 887 | [SHUJILAI/dsh-model-auto-hot-switch](https://github.com/SHUJILAI/dsh-model-auto-hot-switch) | 0 | 2026-08-28 | 2026-08-28 | Automatic per-task model hot-switching for DeepSeek Harness (dsh): image-aware tasks route to the vision model automatically, every other task keeps your default model. Zero extra tokens, no context disturbance. |
| 888 | [shxtmaker/dsh-usage-monitor](https://github.com/shxtmaker/dsh-usage-monitor) | 0 | 2026-08-26 | 2026-08-28 | DSH 用量监控插件：供应商周期限额显示（DeepSeek/OpenCode/Command Code）+ 自动探测 DSH 已添加供应商并自动填入 API Key |
| 889 | [sijie-ni-0214/dsh-subagent-error-details](https://github.com/sijie-ni-0214/dsh-subagent-error-details) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: deliver the real failure reason (e.g. RATE_LIMIT 429) to the parent agent when a background subagent fails |
| 890 | [SiriusWJ/dsh-mihome](https://github.com/SiriusWJ/dsh-mihome) | 0 | 2026-08-30 | 2026-08-30 | Mi Home (米家) control for DeepSeek Harness agents — list homes/devices, read props, control devices behind a human approval gate. |
| 891 | [SJCLZ/MixlabLz-dsh-skills](https://github.com/SJCLZ/MixlabLz-dsh-skills) | 0 | 2026-08-27 | 2026-08-27 | MixlabLz's collection of DSH (DeepSeek Harness) skills and plugins |
| 892 | [SMOKTEA/dsh-chartlab](https://github.com/SMOKTEA/dsh-chartlab) | 0 | 2026-08-26 | 2026-08-28 | Let the agent turn your data into an interactive chart.  \|  一句话：让 Agent 帮你把数据变成一张可交互的图表。 |
| 893 | [Snow-ea/dsh-token-optimizer](https://github.com/Snow-ea/dsh-token-optimizer) | 0 | 2026-08-30 | 2026-08-30 | Deterministic, recoverable tool-result compression and cache-aware compaction for DeepSeek Harness. |
| 894 | [soberbiak/amazon-sucareer](https://github.com/soberbiak/amazon-sucareer) | 0 | 2026-08-28 | 2026-08-30 | 基于真实证据，把亚马逊运营经历酥成招聘方看得懂、面试讲得透的职业定位、简历与求职表达。拒绝硬编 KPI，争取人生大结果。 |
| 895 | [softspark/dsh-orchestrator](https://github.com/softspark/dsh-orchestrator) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness bundle for one-shot Claude Code and GitHub Copilot Gemini delegation through native subscription logins. |
| 896 | [soulYANG/dsh-baogongtou](https://github.com/soulYANG/dsh-baogongtou) | 0 | 2026-08-26 | 2026-08-27 | 包工头：DeepSeek Harness 工作 agent 皮肤。能力还是 dsh，嘴和按钮是包工头。 |
| 897 | [STARDUSTLC666/dsh-dream](https://github.com/STARDUSTLC666/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH 做梦插件：会话回放（梦原料）→ 反思 → 梦境日记（记忆巩固）→ 高频教训幂等桥接 AGENTS.md。多帧 zstd 会话读取、默认隐私脱敏、零运行时依赖。Dream plugin for DeepSeek Harness: session replay, reflection, dream journal, memory bridge. |
| 898 | [STARDUSTLC666/dsh-suite](https://github.com/STARDUSTLC666/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | STARDUSTLC 插件全家桶：一条命令装入 18 个 DSH 插件（办公流/媒体工坊/DevOps/做梦）。The STARDUSTLC plugin suite: 18 DSH plugins, one command. |
| 899 | [starsinc1708/dsh-tool-council](https://github.com/starsinc1708/dsh-tool-council) | 0 | 2026-08-26 | 2026-08-27 | Map-reduce council of subagents for the DeepSeek Harness: one task fans out to independent members, their findings are deduplicated, verified by a separate panel, and reduced to a quorum report |
| 900 | [stayhpjinng/dsh-provider-proxy](https://github.com/stayhpjinng/dsh-provider-proxy) | 0 | 2026-08-29 | 2026-08-29 | Provider-scoped HTTP/HTTPS forward proxy plugin for DeepSeek Harness |
| 901 | [steven-ngle/dsh-elden](https://github.com/steven-ngle/dsh-elden) | 0 | 2026-08-30 | 2026-08-30 | Elden Ring style event overlays for the DeepSeek Harness web UI |
| 902 | [substitute525/dsh-tool-monitor](https://github.com/substitute525/dsh-tool-monitor) | 0 | 2026-08-28 | 2026-08-28 | 一个 dsh-plugin：后台监听文件或命令输出，输出到达时唤醒所属会话，并在 Web 会话头部提供实时监听的列表与输出查看面板。MIT License。 |
| 903 | [Suguyun/dsh-bili-miniplay](https://github.com/Suguyun/dsh-bili-miniplay) | 0 | 2026-08-28 | 2026-08-28 | 跨平台 fork of dsh-bili-widget：DSH B站悬浮看片小窗（Node 原生 fetch，macOS/Linux/Windows 通用） |
| 904 | [sunyuhuirong/fsviewer](https://github.com/sunyuhuirong/fsviewer) | 0 | 2026-08-29 | 2026-08-30 | Codex-style right-edge workspace for DeepSeek dsh web: file tree + preview, embedded browser, and side chat |
| 905 | [sunzhyang1616-ui/dsh-ssh-terminal](https://github.com/sunzhyang1616-ui/dsh-ssh-terminal) | 0 | 2026-08-29 | 2026-08-29 | 在 DSH 侧边栏（dsh-better-sidebar）连接远程主机的 SSH 终端：逐步查看 agent 命令与输出，内置 ssh_connect / ssh_exec 等工具，记录本机持久化。 |
| 906 | [superkonka/dsh-poor-mode](https://github.com/superkonka/dsh-poor-mode) | 0 | 2026-08-27 | 2026-08-27 | 穷鬼模式 Poor Mode — 供应商感知的分时省钱 DSH agent preset：复杂任务可选「立即执行」或「闲时执行」（DeepSeek 峰谷半价；其他平台可自定义规则） |
| 907 | [SuperstructureJH/dsh-workbuddy-ppt](https://github.com/SuperstructureJH/dsh-workbuddy-ppt) | 0 | 2026-08-26 | 2026-08-27 | Editable PPTX generation for DSH with bundled authoring skills and deterministic PPTD validation |
| 908 | [suyukun/dsh-plugin-publish](https://github.com/suyukun/dsh-plugin-publish) | 0 | 2026-08-26 | 2026-08-27 | Ship your skills, grow your influence — a model-agnostic publishing protocol for AI agent skills: preflight checks, GitHub repo, index PRs, marketplace submissions, promo copy. 把 agent 技能标准化发布到 GitHub 的流程协议。 |
| 909 | [suyukun/dsh-tech-selection](https://github.com/suyukun/dsh-tech-selection) | 0 | 2026-08-26 | 2026-08-27 | Stop letting your AI guess — a research protocol for tech decisions that any AI agent (DSH/Claude/Cursor/Codex) can follow: quantified requirements, T1-T6 source tiers, quality gates, traceable verdicts. 模型无关的技术选型调研协议。 |
| 910 | [svgop/dsh-generative-ideas](https://github.com/svgop/dsh-generative-ideas) | 0 | 2026-08-26 | 2026-08-29 | Roadmap ideation for DeepSeek Harness — generate and compare distinct roadmap options via headless agent runs, pick one, export as goal.md |
| 911 | [svgop/dsh-rich-context](https://github.com/svgop/dsh-rich-context) | 0 | 2026-08-26 | 2026-08-29 | Agent instruction manager for DSH — edit and template the AGENTS.md files the harness actually reads (global + per-workspace) |
| 912 | [svgop/dsh-rich-tracking](https://github.com/svgop/dsh-rich-tracking) | 0 | 2026-08-26 | 2026-08-29 | Percent-progress scoreboard for DeepSeek Harness — evidence-bound rows, git-captured checkpoints, pursue/align/dismiss operator whip |
| 913 | [syfun/dsh-dogpet](https://github.com/syfun/dsh-dogpet) | 0 | 2026-08-27 | 2026-08-27 | 🐕 中华田园犬桌面宠物 - DSH Desktop Pet |
| 914 | [syncended/deepseek-harness-messenger](https://github.com/syncended/deepseek-harness-messenger) | 0 | 2026-08-25 | 2026-08-29 | Messenger bridge plugin for DeepSeek Harness, starting with Telegram |
| 915 | [syncended/deepseek-harness-usage](https://github.com/syncended/deepseek-harness-usage) | 0 | 2026-08-26 | 2026-08-27 | Token usage, model cost analytics, trends, and activity heatmaps for DeepSeek Harness |
| 916 | [szymonsheng2045/dsh-carbonclub](https://github.com/szymonsheng2045/dsh-carbonclub) | 0 | 2026-08-28 | 2026-08-28 | A zero-model-cost human waiting room for DeepSeek Harness |
| 917 | [Tangweiwei227/dsh-asc](https://github.com/Tangweiwei227/dsh-asc) | 0 | 2026-08-29 | 2026-08-29 | App Store Connect CLI (asc) as a native tool for DeepSeek Harness — structured argv, JSON output, no-shell execution. |
| 918 | [taod8205-spec/model-switcher-dsh](https://github.com/taod8205-spec/model-switcher-dsh) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 模型与推理强度一键切换插件，支持胶囊滑杆、档位吸附和极高态视觉。 |
| 919 | [TelosmaYLX/dsh-session-notify](https://github.com/TelosmaYLX/dsh-session-notify) | 0 | 2026-08-28 | 2026-08-28 | 当dsh任务完成/阻塞/提问等情况时，自动推送windows消息，支持自定义文案和图片，以及显示会话用时、消耗token、速度tps等指标。Automatically push Windows notifications upon completion of a dsh task, supporting custom text and images, as well as displaying metrics including session duration, token consumption, and TPS speed. |
| 920 | [tianhanly/dsh-official-port-nav](https://github.com/tianhanly/dsh-official-port-nav) | 0 | 2026-08-29 | 2026-08-30 | Perfectly replicate DeepSeek's official right-side chat navigation in Harness |
| 921 | [tianhanly/dsh-warm-reminder](https://github.com/tianhanly/dsh-warm-reminder) | 0 | 2026-08-29 | 2026-08-29 | 智能温馨提醒插件，检测使用时长自动提示喝水、护眼、休息，支持深夜关怀与节假日祝福。基于DSH/Cordis框架开发。 |
| 922 | [tianyuegithub/dsh-pactflow](https://github.com/tianyuegithub/dsh-pactflow) | 0 | 2026-08-30 | 2026-08-30 | DSH PactFlow（零脉模式）外部 Profile Bundle |
| 923 | [Tinnikx/dsh-desktop](https://github.com/Tinnikx/dsh-desktop) | 0 | 2026-08-20 | 2026-08-29 | DeepSeek Harness 的 Linux Electron 桌面客户端，由claude opus生成, 打包后开箱即用, 已更新至0.1.1-rc.2, 插件安装方式与web端一致, 支持"插件市场"插件, 可以安装插件市场后在插件市场中搜索并安装插件, 也可以通过正常命令 ./bin/dsh plugin --profile web add xxxx, download in the Release Page. |
| 924 | [TnzGit/dsh-live-perf-gauges](https://github.com/TnzGit/dsh-live-perf-gauges) | 0 | 2026-08-27 | 2026-08-27 | Real-time Decode tok/s, TTFT and Prefill throughput dashboard for DeepSeek Harness. |
| 925 | [Traveritas/petween](https://github.com/Traveritas/petween) | 0 | 2026-08-21 | 2026-08-29 | Agent pet plugin for DeepSeek Harness (dsh): a few pose images in, expressive comic-style motion out — WAAPI timeline engine, custom animation editor, pose presets, and extension services for companion plugins |
| 926 | [Traveritas/petween-physics](https://github.com/Traveritas/petween-physics) | 0 | 2026-08-25 | 2026-08-29 | Throw-physics companion plugin for Petween (drag-fling, wall bounce, ground slide), consuming the petween extension services |
| 927 | [trueRISCOacnt/maa-dsh-skill](https://github.com/trueRISCOacnt/maa-dsh-skill) | 0 | 2026-08-28 | 2026-08-30 | 基于 MaaAssistantArknights (MAA) 官方命令行工具 maa-cli 构建的 DeepSeek Harness Skill：让 DeepSeek Harness 直接驱动 MaaCore，自动化完成《明日方舟》日常任务。 |
| 928 | [tumi-huakai/dsh-plugin-meow-speech](https://github.com/tumi-huakai/dsh-plugin-meow-speech) | 0 | 2026-08-28 | 2026-08-28 | 喵语定制：DSH 消息正文显示层文本替换插件（仅界面显示，不改动真实对话内容） |
| 929 | [TussalZeus18028/dsh-conflict-checker](https://github.com/TussalZeus18028/dsh-conflict-checker) | 0 | 2026-08-26 | 2026-08-27 | Detect DeepSeek Harness plugin conflicts and internal issues; manage plugins (enable/disable/uninstall) from a settings page. |
| 930 | [tuzkier/valley-liang](https://github.com/tuzkier/valley-liang) | 0 | 2026-08-28 | 2026-08-28 | 梁文谷：替换 DeepSeek Harness Web 品牌标识，并按北京时间高峰时段切换图片。 |
| 931 | [UnforgetMemory/um-dsh-websearch](https://github.com/UnforgetMemory/um-dsh-websearch) | 0 | 2026-08-27 | 2026-08-27 | Exa (exa.ai) web search provider plugin for DeepSeek Harness (DSH): dynamic enabled switch, credentials-service key resolution, bilingual settings card. |
| 932 | [unknowbug/dsh-thinking-loop-guard](https://github.com/unknowbug/dsh-thinking-loop-guard) | 0 | 2026-08-27 | 2026-08-27 | Detect & break thinking-chain loops in DSH agents at the turn boundary (no proxy). Ported from ollama-loop-guard. |
| 933 | [UnKnownFish125/dsh-livetaskboard](https://github.com/UnKnownFish125/dsh-livetaskboard) | 0 | 2026-08-26 | 2026-08-27 | 派生动态任务看板插件：独立任务状态机、存储、看板 UI、外援（sol + 保底子代理）；从 dsh-deepmemory 派生。 |
| 934 | [uppercrusteve/dsh-plugin-split-and-solve](https://github.com/uppercrusteve/dsh-plugin-split-and-solve) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: split batch / multi-subproblem research tasks into small questions and solve them with sub-agents |
| 935 | [vb2250158/dsh-plugins](https://github.com/vb2250158/dsh-plugins) | 0 | 2026-08-27 | 2026-08-27 | Open-source DeepSeek Harness plugin bundle with portable multi-computer synchronization |
| 936 | [Viktirr/dsh-llm-lmstudio](https://github.com/Viktirr/dsh-llm-lmstudio) | 0 | 2026-08-28 | 2026-08-29 | LM Studio (OpenAI-compatible local server) adapter plugin for DeepSeek Harness |
| 937 | [Viviana-Luna/dsh-window](https://github.com/Viviana-Luna/dsh-window) | 0 | 2026-08-24 | 2026-08-28 | macOS 薄桌面客户端，为本机 DSH 提供 Liquid Glass UI。 |
| 938 | [w2327644822-png/dsh-usage-analytics](https://github.com/w2327644822-png/dsh-usage-analytics) | 0 | 2026-08-26 | 2026-08-27 | Personal usage analytics & activity dashboard for the DeepSeek Harness (dsh) web GUI: token totals, contribution heatmap, model share, insights. Local-only, metadata only. |
| 939 | [wantosure/dsh-plugin-browser-memory](https://github.com/wantosure/dsh-plugin-browser-memory) | 0 | 2026-08-26 | 2026-08-27 | Local-first DeepSeek Harness plugin for searching Chrome, Edge, and Brave bookmarks, history, and downloads. |
| 940 | [wenyixiaoqingnian/ds-mobile-skin](https://github.com/wenyixiaoqingnian/ds-mobile-skin) | 0 | 2026-08-30 | 2026-08-30 | Mobile DeepSeek-app look for DSH Web GUI + dsh-token-viewer billing patch |
| 941 | [wf-ping/dsh-message-injector](https://github.com/wf-ping/dsh-message-injector) | 0 | 2026-08-30 | 2026-08-30 | dsh（DeepSeek Harness）插件：预设消息注入内容组合，每条消息自动注入 —— auto-inject preset content into every message |
| 942 | [whutzefengxie-ops/dsh-shadow-mind](https://github.com/whutzefengxie-ops/dsh-shadow-mind) | 0 | 2026-08-24 | 2026-08-28 | Independent Shadow agent orchestration plugin for DeepSeek Harness |
| 943 | [Wickaninnish/dsh-skill-manager](https://github.com/Wickaninnish/dsh-skill-manager) | 0 | 2026-08-22 | 2026-08-27 | DeepSeek Harness 技能运维插件：自动发现、审计、去重和优化技能，构建安全可控的维护闭环。 |
| 944 | [Wilson-Lai-Ab/dsh-idea-style](https://github.com/Wilson-Lai-Ab/dsh-idea-style) | 0 | 2026-08-21 | 2026-08-27 | DSH plugin |
| 945 | [windrover/dsh-long-term-memory](https://github.com/windrover/dsh-long-term-memory) | 0 | 2026-08-25 | 2026-08-27 | Layered deterministic long-term memory for DeepSeek Harness: CJK-aware BM25 recall, JSONL storage, per-assembly context injection, write guards and threat scanning. |
| 946 | [winghv/dsh-acp-activity](https://github.com/winghv/dsh-acp-activity) | 0 | 2026-08-30 | 2026-08-30 | Community ACP automation server for DeepSeek Harness with committed tool-activity frames (tool_call/tool_call_update) — dsh-plugin |
| 947 | [WinnieJQ/dsh-conversation-cost](https://github.com/WinnieJQ/dsh-conversation-cost) | 0 | 2026-08-28 | 2026-08-28 | Per-conversation DeepSeek API cost badge for DeepSeek Harness (dsh): zero-dependency sessionCost projection with peak/off-peak pricing and a live hover-card badge in the web conversation header. |
| 948 | [Wisdoverse/dsh-inline-media-viewer-plugin](https://github.com/Wisdoverse/dsh-inline-media-viewer-plugin) | 0 | 2026-08-26 | 2026-08-28 | Inline image, video, and audio previews for DeepSeek Harness Web, with workspace-safe local files, direct web media, and an optional ComfyUI proxy. |
| 949 | [Wisdoverse/dsh-skills-manager-plugin](https://github.com/Wisdoverse/dsh-skills-manager-plugin) | 0 | 2026-08-28 | 2026-08-28 | Skill manager for DeepSeek Harness: proactive skill activation with trigger hooks, GitHub source sync, and a Settings management UI. |
| 950 | [Witchwarren2344/dsh-mnemosyne-memory](https://github.com/Witchwarren2344/dsh-mnemosyne-memory) | 0 | 2026-08-29 | 2026-08-29 | Provide long-term memory, vector semantic search, and LLM reflection for DeepSeek Harness (DSH) with this free, MIT-licensed plugin. |
| 951 | [wjf1/dsh-commandcode](https://github.com/wjf1/dsh-commandcode) | 0 | 2026-08-30 | 2026-08-30 | DSH-Desktop LLM provider plugin for Command Code with model catalog sync, request retry, multi-credential support, and a settings UI. |
| 952 | [WJNCT55555/dsh-crt-theme](https://github.com/WJNCT55555/dsh-crt-theme) | 0 | 2026-08-26 | 2026-08-27 | Dual-palette CRT terminal theme for DeepSeek Harness Web |
| 953 | [Wlain/kling-ai-deepseek-plugin](https://github.com/Wlain/kling-ai-deepseek-plugin) | 0 | 2026-08-26 | 2026-08-27 | Kling AI remote MCP plugin for DeepSeek Harness |
| 954 | [wly8691-jpg/dsh-office-com](https://github.com/wly8691-jpg/dsh-office-com) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: COM-driven real Office automation (VBA/pivot/recalc/layout) |
| 955 | [wodongx123/dsh-language-control](https://github.com/wodongx123/dsh-language-control) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: force agent chain-of-thought to stay in Chinese — 让 Agent 的思考过程也自动使用中文 |
| 956 | [WolffyCode/deepseek-harness-plugin](https://github.com/WolffyCode/deepseek-harness-plugin) | 0 | 2026-08-25 | 2026-08-29 | Multi-engine Claude CLI and Codex CLI integration for DeepSeek Harness |
| 957 | [WooLeo1995/dsh-llm-ai](https://github.com/WooLeo1995/dsh-llm-ai) | 0 | 2026-08-27 | 2026-08-27 | 替换 llm-pi-ai 模型配置，主要处理 dsh-llm-pi-ai 厂商和模型更新不及时的问题 |
| 958 | [wr-web/dsh-context-tree](https://github.com/wr-web/dsh-context-tree) | 0 | 2026-08-26 | 2026-08-27 | Reusable trajectory-tree context, exact-turn forks, and bounded cross-session recall for DeepSeek Harness |
| 959 | [WSL043/dsh-dictation](https://github.com/WSL043/dsh-dictation) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 语音输入：本地多语言识别与 Codex Desktop 听写，只写入可编辑草稿。 |
| 960 | [WSL043/dsh-image-viewer](https://github.com/WSL043/dsh-image-viewer) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 图片查看器：缩放、平移、原图下载、图库与区域标注。 |
| 961 | [wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback](https://github.com/wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback) | 0 | 2026-08-25 | 2026-08-27 | DSH plugin that converts read_image PNG/WebP attachments to JPEG for LM Studio compatibility. |
| 962 | [wxjgit/permission-popup](https://github.com/wxjgit/permission-popup) | 0 | 2026-08-27 | 2026-08-27 | 当前会话或后台会话正在等待权限审批时，插件会在页面角落显示审批卡片，让你无需切回原会话就能选择“允许一次”或“拒绝”。 |
| 963 | [xain/ui-beep](https://github.com/xain/ui-beep) | 0 | 2026-08-26 | 2026-08-27 | **dsh-beep** — an agent-heartbeat sonification plugin for the DeepSeek Harness Web surface. |
| 964 | [xarleyn/dsh-doc-impact](https://github.com/xarleyn/dsh-doc-impact) | 0 | 2026-08-28 | 2026-08-28 | Documentation impact enforcement for DeepSeek Harness — keep docs in sync by linking code changes to affected documentation. |
| 965 | [xarleyn/dsh-session-scope](https://github.com/xarleyn/dsh-session-scope) | 0 | 2026-08-28 | 2026-08-28 | Per-session workspace scoping for DeepSeek Harness — expose only selected directories to agents with focused and isolated enforcement. |
| 966 | [xarleyn/dsh-sleev](https://github.com/xarleyn/dsh-sleev) | 0 | 2026-08-26 | 2026-08-27 | Sleev integration for DeepSeek Harness with route-aware LLM telemetry and context-optimization observability |
| 967 | [xchannel1987/dsh-mobile-xc](https://github.com/xchannel1987/dsh-mobile-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH Web mobile UI adaptation plugin with overlay drawer, safe-area support, and canary version detection |
| 968 | [xchannel1987/dsh-power-xc](https://github.com/xchannel1987/dsh-power-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH power control plugin with restart/shutdown menu and Windows-style overlay animation |
| 969 | [xchannel1987/dsh-reverse-proxy-xc](https://github.com/xchannel1987/dsh-reverse-proxy-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH LAN reverse proxy plugin for accessing Web GUI from mobile devices |
| 970 | [xchannel1987/dsh-session-xc](https://github.com/xchannel1987/dsh-session-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH session enhancement plugin with session count display, archive management, and cross-workspace move |
| 971 | [xchannel1987/dsh-token-usage-xc](https://github.com/xchannel1987/dsh-token-usage-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH token usage statistics plugin with daily/7-day trends and cache hit rate |
| 972 | [xfqz86/dsh-usage-stats](https://github.com/xfqz86/dsh-usage-stats) | 0 | 2026-08-23 | 2026-08-27 | DSH Web 插件：侧边栏中的 Token 使用统计 |
| 973 | [XianmingLF/xmlf-plugin-manager](https://github.com/XianmingLF/xmlf-plugin-manager) | 0 | 2026-08-21 | 2026-08-28 | 管理当前第三方已安装插件的信息 比较简单的版本 可按照自己的需求修改 |
| 974 | [xiaoso456/dsh-tool-plus](https://github.com/xiaoso456/dsh-tool-plus) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 基础工具增强：持久 bash、结构化 read、多模式 edit、原子 write、双引擎 grep/glob、图像直读，一个插件全覆盖 |
| 975 | [XiaoWind/dsh-btw](https://github.com/XiaoWind/dsh-btw) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: a /btw slash command to add notes without interrupting the agent |
| 976 | [XiaoWind/dsh-vault](https://github.com/XiaoWind/dsh-vault) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness plugin: portable workspace vault for DSH conversations and logs |
| 977 | [xiaoxiao44443/dfy-dsh-plugins](https://github.com/xiaoxiao44443/dfy-dsh-plugins) | 0 | 2026-08-17 | 2026-08-28 | Personal plugins for DeepSeek Harness |
| 978 | [xiaoxingyuemiao/dsh-bg-plugin](https://github.com/xiaoxingyuemiao/dsh-bg-plugin) | 0 | 2026-08-27 | 2026-08-27 | DSH 自定义背景插件：为 DSH Web GUI 应用远程/本地图片背景，支持清晰度、压暗、模糊调节，设置面板保持默认外观。 |
| 979 | [xiyi123465/dsh-usage-calendar](https://github.com/xiyi123465/dsh-usage-calendar) | 0 | 2026-08-25 | 2026-08-27 | DeepSeekAPI余额查询插件 |
| 980 | [xiyunSacire/dsh-skill-manager](https://github.com/xiyunSacire/dsh-skill-manager) | 0 | 2026-08-28 | 2026-08-28 |  The dsh-skill-manager is a deep-integration Web UI plugin designed to provide developers and advanced users with direct visibility and control over the true, persistent "skill memory" of DeepSeek Harness (DSH). |
| 981 | [xlin20021/dsh-mcp-hub](https://github.com/xlin20021/dsh-mcp-hub) | 0 | 2026-08-29 | 2026-08-29 | dsh-mcp-hub |
| 982 | [xlin20021/dsh-stock-chart](https://github.com/xlin20021/dsh-stock-chart) | 0 | 2026-08-29 | 2026-08-29 | dsh-stock-chart |
| 983 | [xobexo/dsh-smart-scenario-router](https://github.com/xobexo/dsh-smart-scenario-router) | 0 | 2026-08-27 | 2026-08-27 | 国产模型优先，按任务类型自动切换模型，支持可视化配置面板 |
| 984 | [xswt442-cmd/dsh-treekeeper](https://github.com/xswt442-cmd/dsh-treekeeper) | 0 | 2026-08-27 | 2026-08-27 | 对账 DSH 任务账本与 OS 进程树，定位归属、检测泄漏并安全治理｜Reconcile DSH task ledgers with OS process trees for attribution, leak detection, and safe governance. |
| 985 | [xyingsoft/dsh-chat](https://github.com/xyingsoft/dsh-chat) | 0 | 2026-08-29 | 2026-08-29 | dsh-chat 设计文档：面向自建团队、受管团队与企业组织的 DSH Web 协作平台 |
| 986 | [Xylocarpro/dsh-plugin-recycle-bin](https://github.com/Xylocarpro/dsh-plugin-recycle-bin) | 0 | 2026-08-29 | 2026-08-30 | 强制 DSH 删除走回收站、禁用 del/rm/Remove-Item，回收站或硬盘满时停手询问用户。 |
| 987 | [Ya-MiC/zhanzhen](https://github.com/Ya-MiC/zhanzhen) | 0 | 2026-08-24 | 2026-08-27 | 湛箴 — 中小企业审计风险平台 v1 框架（FastAPI + Vue3，规则引擎本地运行，证据哈希链） |
| 988 | [yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix](https://github.com/yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix) | 0 | 2026-08-27 | 2026-08-27 | 修复 sandbox_permissions 和 justification 字段在 pwsh/bash/fs/dsh-sandbox 中的 no-op 升级报错。当会话已是 danger-full-access 模式时，模型携带空 justification 或重申同一模式被拒的问题。 |
| 989 | [yangdongzhen590/dsh-knj-obsidian](https://github.com/yangdongzhen590/dsh-knj-obsidian) | 0 | 2026-08-28 | 2026-08-28 | DSH ??? Obsidian:AI agent ?????????????UI ?????(v1-v7) |
| 990 | [yangzhe1991/dsh-project-session-store](https://github.com/yangzhe1991/dsh-project-session-store) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: store each project's session logs inside the project directory (.dsh/sessions/) \| DSH 插件:把每个项目的会话日志保存在项目目录(.dsh/sessions/)下,不再集中到 ~/.dsh/sessions |
| 991 | [yanqd0/dsh-covtrim](https://github.com/yanqd0/dsh-covtrim) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: one-shot test coverage flow — run tests with coverage, compress with covtrim, return compact TSV to the agent |
| 992 | [yanqd0/dsh-mint](https://github.com/yanqd0/dsh-mint) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: mint issue tracking integration — session context injection, event reminders, plan binding, mint_query tool, and a session tab |
| 993 | [yaodongH/dsh-vscode-bridge](https://github.com/yaodongH/dsh-vscode-bridge) | 0 | 2026-08-30 | 2026-08-30 | DSH web 插件：在 DeepSeek Harness 中心区嵌入固定版本 code-server（VS Code Web），跟随当前工作空间，支持自定义端口/路径与热切换。 |
| 994 | [yaotongsb/dsh-phosphor](https://github.com/yaotongsb/dsh-phosphor) | 0 | 2026-08-29 | 2026-08-29 | A full-screen, Matrix-styled TUI frontend for DeepSeek Harness — built with React + Ink as a Cordis bundle plugin |
| 995 | [yhbd-top/dsh-plugin-top](https://github.com/yhbd-top/dsh-plugin-top) | 0 | 2026-08-29 | 2026-08-29 | yhbd.top 插件雷达 for DeepSeek Harness：侧边栏大面板浏览 3900+ 插件目录（搜索 / 22 分类 / 站点同款五榜单 / 榜单联动分类），安装引导语一键写入会话输入框；进程内同源反代，零配置；附带 Agent 可调用的搜索与榜单工具。 |
| 996 | [yhPrime/dsh-github-installer](https://github.com/yhPrime/dsh-github-installer) | 0 | 2026-08-29 | 2026-08-29 | GitHub 仓库一键安装插件：粘贴任意 GitHub 插件仓库网址即可安装（标准 dsh plugin add github:… 协议，同 dsh-market）。Install any DeepSeek Harness plugin from a GitHub repo URL. |
| 997 | [Yidien/dsh-host-router](https://github.com/Yidien/dsh-host-router) | 0 | 2026-08-29 | 2026-08-29 | dsh 外挂式网络路由插件:按域名勾选走本地代理(Clash 等),其余直连;内置嗅探,设置页勾选即生效。 |
| 998 | [yonglun/deepseek-harness-themes](https://github.com/yonglun/deepseek-harness-themes) | 0 | 2026-08-27 | 2026-08-28 | 74 non-invasive DeepSeek Harness themes generated from awesome-design-md |
| 999 | [yongshuai0314/dsh-turnsnap](https://github.com/yongshuai0314/dsh-turnsnap) | 0 | 2026-08-27 | 2026-08-27 | Zero-config per-turn git checkpoints for DeepSeek Harness: every completed agent turn in a git workspace becomes one tagged [turnsnap] commit |
| 1000 | [yoshino-xiao7/dsh-codex](https://github.com/yoshino-xiao7/dsh-codex) | 0 | 2026-08-28 | 2026-08-29 | 社区维护的 DeepSeek Harness Codex 插件：OAuth、模型、图片与流式恢复；非官方 / Community Codex plugin for DSH: OAuth, models, images, stream recovery; unofficial. |
| 1001 | [youridol/dsh-plugin](https://github.com/youridol/dsh-plugin) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件收录总库：收录遵循 Cordis 框架、经官方 profile 机制挂载的 DSH 插件。收录插件自动同步上游，自研插件可手动维护。 |
| 1002 | [YUANMINGXUE/dsh-search](https://github.com/YUANMINGXUE/dsh-search) | 0 | 2026-08-26 | 2026-08-27 | Local-browser web search & page fetch plugin for DeepSeek Harness (dsh): browser_search / browser_fetch over Chrome DevTools Protocol, no API key. |
| 1003 | [YUEYUEXYS/dsh-think-ultra](https://github.com/YUEYUEXYS/dsh-think-ultra) | 0 | 2026-08-30 | 2026-08-30 | Reasoning layer for the official DeepSeek Harness: every request stays on native max effort, with isolated Flash/Vision/Pro depth controls, stability axes and reasoning toolboxes built above it. Delivered build only; commercial use open, reverse/modify/extract closed. |
| 1004 | [yunxiiQwQ/drool-whale-pet-for-dsh](https://github.com/yunxiiQwQ/drool-whale-pet-for-dsh) | 0 | 2026-08-27 | 2026-08-27 | 适用于dsh的pet插件 |
| 1005 | [Yur0918/dsh-user-addons](https://github.com/Yur0918/dsh-user-addons) | 0 | 2026-08-28 | 2026-08-28 | Community DSH web plugin for file uploads, archived-session management, image capability detection, and model/token usage insights. |
| 1006 | [Yurzi/dsh-web-fetch-enhanced](https://github.com/Yurzi/dsh-web-fetch-enhanced) | 0 | 2026-08-28 | 2026-08-28 | Configurable non-public address allowlists for DeepSeek Harness web_fetch |
| 1007 | [Yurzi/dsh-web-search-enhanced](https://github.com/Yurzi/dsh-web-search-enhanced) | 0 | 2026-08-29 | 2026-08-29 | Multi-protocol web_search provider for DeepSeek Harness |
| 1008 | [yustillrain/dsh-plugin-tool-repository](https://github.com/yustillrain/dsh-plugin-tool-repository) | 0 | 2026-08-26 | 2026-08-27 | DSH 插件仓库 第三方插件 让你可视化管理已安装的 skill/插件 对skill/插件功能进行介绍和分类  |
| 1009 | [yx-yinhe/dsh-message-navigator](https://github.com/yx-yinhe/dsh-message-navigator) | 0 | 2026-08-27 | 2026-08-27 | ChatGPT-style message navigator for DeepSeek Harness conversations with hover previews and smooth jump navigation. |
| 1010 | [Yyyyyylor/dsh-asuka-school-theme](https://github.com/Yyyyyylor/dsh-asuka-school-theme) | 0 | 2026-08-25 | 2026-08-27 | Theme-Asuka — An unofficial Asuka-inspired theme plugin for DeepSeek Harness Web UI, featuring time-of-day wallpapers, adaptive palette transitions, and restrained EVA-02 visual details. |
| 1011 | [z7ping/narratica](https://github.com/z7ping/narratica) | 0 | 2026-08-28 | 2026-08-28 | AI 原生故事创作与媒体生产工作区｜AI-native storytelling workspace for novels, screenplays, and media production. |
| 1012 | [zdjmrq/dsh-chat-mode](https://github.com/zdjmrq/dsh-chat-mode) | 0 | 2026-08-26 | 2026-08-27 | DSH 插件：为 DeepSeek Harness 增加「对话」纯聊天模式（ChatGPT 式）——侧边栏新会话模式切换（DSH/对话）、对话会话仅提问+搜索工具、专属 \/chat 聊天工作区 |
| 1013 | [zengweicheng666/dsh-svn-tools](https://github.com/zengweicheng666/dsh-svn-tools) | 0 | 2026-08-29 | 2026-08-29 | SVN (Subversion) tools + sidebar UI for DeepSeek Harness: 33 agent tools with UTF-8 Chinese commit logs, plus an SVN panel in dsh-better-sidebar. |
| 1014 | [zenvertao/dsh-inline-comments](https://github.com/zenvertao/dsh-inline-comments) | 0 | 2026-08-26 | 2026-08-27 | 选中即批注，刷新亦留存 —— DSH 行内批注插件 |
| 1015 | [Zessi-C/biofigure-self-evolve](https://github.com/Zessi-C/biofigure-self-evolve) | 0 | 2026-08-29 | 2026-08-30 | Self-evolving bioinformatics figure library skill: learn plots from papers/PDFs/WeChat articles/screenshots into reusable recipes (R/Python), imitate them when plotting. 自进化的生信 figure 学习库与复用引擎 |
| 1016 | [zhang-jiazhi/dsh-prompt-optimizer](https://github.com/zhang-jiazhi/dsh-prompt-optimizer) | 0 | 2026-08-30 | 2026-08-30 | 将原作者 linshenkx 的 prompt-optimizer 移植到 DeepSeek Harness 的第三方插件（非官方） |
| 1017 | [zhangguiping-xydt/dsh-session-lab](https://github.com/zhangguiping-xydt/dsh-session-lab) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness session teaching, evidence capsules, and controlled trajectory comparison |
| 1018 | [zhangkkkai/dsh-spec-panel](https://github.com/zhangkkkai/dsh-spec-panel) | 0 | 2026-08-28 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 SDD（规范驱动开发，Spec-Driven Development）配套插件：在侧边栏提供一个 Spec 工作台，围绕 OpenSpec 的标准目录结构，让「先写规范 → 再实现 → 再验证」的流程一目了然、可操作。 |
| 1019 | [zhangkkkai/dsh-todo-panel](https://github.com/zhangkkkai/dsh-todo-panel) | 0 | 2026-08-27 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 TODO 任务清单侧边栏插件：卡片式布局、优先级颜色标记、中文界面、按会话持久化。 |
| 1020 | [zhangliang0115/ai-plugin](https://github.com/zhangliang0115/ai-plugin) | 0 | 2026-08-29 | 2026-08-29 | One command to install any AI agent skill/plugin into every agent — Claude Code, DeepSeek Harness (dsh), Codex, Gemini CLI, Copilot, Cursor. Zero-dependency CLI + cross-agent marketplace. |
| 1021 | [zhangzhenwen1/dsh-task-effort](https://github.com/zhangzhenwen1/dsh-task-effort) | 0 | 2026-08-30 | 2026-08-30 | Auto-adjust model reasoning effort per task with DeepSeek peak-pricing-period capping: off/low/high/max classification, [effort=...] markers, error escalation, countdown notices |
| 1022 | [zhaozixi/dsh-attention](https://github.com/zhaozixi/dsh-attention) | 0 | 2026-08-28 | 2026-08-30 | DSH 跑任务时你通常只能盯着进度条。dsh-attention 把这段等待变成有产出的碎片时间 |
| 1023 | [zhchxiao123/dsh-devflow-plugins](https://github.com/zhchxiao123/dsh-devflow-plugins) | 0 | 2026-08-26 | 2026-08-30 | File-backed development workflow for DeepSeek Harness: durable cards, artifact and agent checks, human approvals, and a read-only web board. |
| 1024 | [zhengjy01/dsh-vercel-mcp](https://github.com/zhengjy01/dsh-vercel-mcp) | 0 | 2026-08-30 | 2026-08-30 | Vercel MCP connection for DeepSeek Harness (DSH): official OAuth 2.0 flow (dynamic client registration + PKCE) against mcp.vercel.com, Vercel API tools under mcp__vercel__*, and a web settings panel |
| 1025 | [zhm20001/dsh-usage-board](https://github.com/zhm20001/dsh-usage-board) | 0 | 2026-08-27 | 2026-08-28 | dsh-usage-board 是专为 DSH (DeepSeek Harness) 设计的用量与成本可视化看板插件。  插件能实时捕获会话内的 Token 消耗、Step 耗时和异常指标，支持冷启动增量回溯历史全量会话，并按 Sub-agent DAG 调用关系进行树状归集与反向明细穿透。 |
| 1026 | [zhoujianbin/dsh-codex-continue](https://github.com/zhoujianbin/dsh-codex-continue) | 0 | 2026-08-29 | 2026-08-30 | DSH 插件：读取本机 Codex 项目与会话，一键在 DSH 里继续。Read local OpenAI Codex sessions and continue them in DeepSeek Harness. |
| 1027 | [zhubaohi/dsh-gpu-pulse](https://github.com/zhubaohi/dsh-gpu-pulse) | 0 | 2026-08-30 | 2026-08-30 | Floating GPU monitor (nvidia-smi) for the DSH Web UI — live per-GPU utilization, VRAM, temperature, power and fan, in the corner of the page. |
| 1028 | [ZiFan1117/bazidiy](https://github.com/ZiFan1117/bazidiy) | 0 | 2026-08-26 | 2026-08-27 | 基于 DeepSeek Harness 的八字五行手串定制插件 |
| 1029 | [zisen123/dsh-reasoning-ruler](https://github.com/zisen123/dsh-reasoning-ruler) | 0 | 2026-08-30 | 2026-08-30 | Minimal reasoning-effort ruler for the DSH web composer: hairline + sliding marker, per-model memory, optimistic switching, streamlined model picker |
| 1030 | [Zleap-AI/dsh-sag](https://github.com/Zleap-AI/dsh-sag) | 0 | 2026-08-29 | 2026-08-29 | 面向 DeepSeek Harness 的 SAG 本地个人知识库插件，支持知识检索、原文读取、文件上传、文本写入与文档管理。 |
| 1031 | [zpliao123/dsh-ark-quota](https://github.com/zpliao123/dsh-ark-quota) | 0 | 2026-08-27 | 2026-08-27 | Volcengine Ark Coding Plan / Agent Plan quota plugin for DeepSeek Harness (DSH) Web GUI: side float widget + settings page, persistent credentials, periodic auto-refresh, ark_coding_plan_usage model tool. |
| 1032 | [zptalk0221-cpu/dsh-remote-desktop](https://github.com/zptalk0221-cpu/dsh-remote-desktop) | 0 | 2026-08-26 | 2026-08-27 | 远程桌面移动化插件：为 DeepSeek Harness 提供手机横屏外壳与中文输入法 |
| 1033 | [zuojinxin/dsh-provider-switch](https://github.com/zuojinxin/dsh-provider-switch) | 0 | 2026-08-28 | 2026-08-28 | Provider on/off switches, model search, and inline provider renaming for DeepSeek Harness. |
| 1034 | [zxheyi/dsh-work](https://github.com/zxheyi/dsh-work) | 0 | 2026-08-27 | 2026-08-27 | A plugin-native AI desktop for real work, built on DeepSeek Harness. |
| 1035 | [zzhi191/dsh-plugin-night-dog](https://github.com/zzhi191/dsh-plugin-night-dog) | 0 | 2026-08-29 | 2026-08-29 | A tan DeepSeek mascot dog named 夜官 that lives in the corner of the DSH web GUI: floats, reacts to the harness, adapts to the theme, and acts out a full repertoire (pant, stand, walk, tilt, yawn, bark, spin, whimper, lie down to sleep). Pure client plugin, installable from the DSH Community Market. |

## 从快照消失的已核准仓库 / Approved repositories missing from the snapshot

已核准但已不在当前快照中（删除或改名），核实后从 [data/approved.json](../approved.json) 移除或更新名称。

Approved but no longer present in the current snapshot (deleted or renamed) — after checking, remove them from [data/approved.json](../approved.json) or update the name.

- 240xu/tech-lead-skill
- ABccgh/dsh-agent-studio
- ABccgh/dsh-github-plugin-tools
- ABccgh/dsh-ima-plugin
- ABccgh/dsh-plugin-dev
- ABccgh/imakb
- ABccgh/ws-cleaner
- alfonsoferrertorres-cyber/saare-suite
- Arslan-jh/deepseek-harness-usage
- Bacskat/dsh-claude-ui
- bettermen/dsh-course-writer
- bitterSmilezzz/dsh-ui-tweaks
- BlackDawnNova/dsh-web-open
- blueWhalei/dsh-verify-gate
- CharlesAQ/dsh-fgo-chaldea
- Cheerwhy/dsh-chat-anchors
- chendefine/dsh-better-sidebar-onlyoffice
- chendefine/dsh-cdp-live-view
- chinaRXQ/dsh-wallpaper
- chumingjun/harness-one
- cking000bigdemon/dsh-acp-interactive
- cking000bigdemon/dsh-toolbelt
- coder-wu/dsh-finance-data
- coeasy/oh-my-dsh
- collapsey/xiaokui-pet
- dat-lequoc/dsh-shots
- ddtcorex/dsh-maestro-harness
- dHR-P/dsh-anchored-wsl
- dolcejust-spec/dsh-event-watch
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
- Entity-Him/dsh-doc-quick
- Entity-Him/dsh-harmonyos-market
- Entity-Him/dsh-hiboard-push
- Entity-Him/dsh-sky-skin
- fff122/dsh-agent-arcade
- fff122/dsh-prompt-presets
- fff122/dsh-research-notes
- fff122/dsh-task-checklist
- firestige/execution-system
- g-yixuan/dsh-sidechat
- Gaq152/dsh-attention
- Gaq152/dsh-credits
- ggggggggggz/dsh-config
- GM-HZ/dsh-dag-workflow
- hawkongz/doubao-vision-dsh
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
- lovstudio/dsh-plugin-creator-skill
- lovstudio/dsh-plugin-publisher-skill
- morlay/session-persistence-rdb
- mrgaoang/dsh-remote
- mrlfarano/dsh-tailscale-surface
- mrpulor-gh/nuphus-mcp
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
- statem-li/dsh-better-markdown
- statem-li/dsh-browser
- statem-li/dsh-image-gallery
- statem-li/dsh-reasoning-effort
- statem-li/dsh-tool-summary
- statem-li/dsh-usage-skill
- statem-li/dsh-vision-helper
- statem-li/dsh-zh-thinking
- tinchak0207/dsh-emu-workbench
- trrrrrryg/dsh-remote-workspace
- udsy19/dsh-toolcall-stream-repair
- vikasranax/dsh-plugin-cats
- WSL043/dsh-native-deepseek-balance
- WSL043/dsh-native-reasoning-slider
- WSL043/dsh-native-session-manager
- xiaoliang2/dsh-compact-after-task
- xiaoliang2/enterprise-compliance
- XSakura666/ChronoAgent
- youridol/dsh-sess
- yustillrain/dsh-skill-browser
- Yvesgao/dsh-desktop-launcher
- Zh1rV/dsh-web-search-tavily
- zhaimingyou/aisync
- zhangyoufu-123/stylotrace
- zhongjie10086/dsh-adaptive-native-standard
