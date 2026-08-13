# Awesome ai plugins with stars

<p align="center">
  <br>
  <img width="80" src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="Awesome">
  <br>
</p>

<h1 align="center">Awesome AI Plugins</h1>

<p align="center">A curated, cross-platform list of plugins, skills, MCP servers, apps, and agent tools for AI assistants.</p>

<p align="center">
  <a href="https://hol.org/registry/plugins">
    <img src="assets/awesome-ai-plugins-hol.png" alt="Awesome AI Plugins by HOL" width="960" height="540">
  </a>
</p>

<p align="center">
  <a href="#contributing"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
  <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License"></a>
  <a href="https://hol.org/registry/plugins"><img src="https://img.shields.io/badge/Browse-Registry-green" alt="Browse Registry"></a>
  <a href="https://github.com/sponsors/hashgraph-online"><img src="https://img.shields.io/badge/Sponsor%20HOL-GitHub%20Sponsors-ea4aaa" alt="Sponsor HOL on GitHub"></a>
</p>

<p align="center">
  Discover extensions for Codex, ChatGPT, Claude Code, Gemini CLI, Cursor, OpenCode, and other compatible AI assistants from one community-maintained catalog.
</p>

<p align="center">
  Listings may target one assistant, several assistants, or open standards such as Agent Skills and MCP. Check each project for its supported clients and installation instructions.
</p>

<br>

## Contents

* [Start Here](#start-here)
* [Official Plugins](#official-plugins)
* [Community Plugins](#community-plugins)
* [Formats & Development](#formats--development)
* [Guides & Articles](#guides--articles)
* [Related Projects](#related-projects)
* [Claim Your Plugin](#claim-your-plugin)
* [Plugin Trust Scores](#plugin-trust-scores)
* [Plugin Quality](#plugin-quality)
* [Contributing](#contributing)

***

## Start Here

New extension workflow:

1. **Validate with [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 433 | 🐛 29 | 🌐 Python | 📅 2026-08-13** — **Required: score ≥ 80, no high/critical findings**
2. **Gate PRs with the [HOL scanner GitHub Action](https://github.com/hashgraph-online/ai-plugin-scanner-action) ⭐ 3 | 🐛 1 | 📅 2026-08-10** — **Required for listing**
3. Choose the clients and open formats you support
4. Build the plugin, skill, MCP server, app, or agent tool
5. Ship or submit with confidence

### Quick preflight

```bash
pipx run plugin-scanner lint .
pipx run plugin-scanner verify .
```

### Scanner Requirements (Mandatory for This List)

All plugins submitted to **Awesome AI Plugins** must pass the HOL AI Plugin Scanner:

| Requirement  | Threshold                                      |
| ------------ | ---------------------------------------------- |
| **Score**    | ≥ 80 / 130                                     |
| **Severity** | No critical or high findings                   |
| **CI**       | Scanner must run in your repo's GitHub Actions |

See the full guide: [`SCANNER_GUIDE.md`](./SCANNER_GUIDE.md)\
See contributing requirements: [`CONTRIBUTING.md`](./CONTRIBUTING.md)

The README is the human-readable cross-platform catalog. Machine-readable compatibility exports are available in `plugins.json` and `.agents/plugins/marketplace.json` for registry and automation consumers.

### Browse the catalog

Browse the sections below or use the searchable [HOL Plugin Registry](https://hol.org/registry/plugins). Installation varies by client and project, so follow the linked project's setup guide.

This repository is a discovery catalog, not a universal installer. Follow each linked project's instructions for the clients and formats it supports.

## Official Plugins

<details>
<summary>Curated by OpenAI — available in the built-in Codex Plugin Directory</summary>

* Box - Access and manage files.
* Cloudflare - Manage Workers, Pages, DNS, and infrastructure.
* Figma - Inspect designs, extract specs, and document components.
* GitHub - Review changes, manage issues, and interact with repositories.
* Gmail - Read, search, and compose emails.
* Google Drive - Edit and manage files in Google Drive.
* Hugging Face - Browse models, datasets, and spaces.
* Linear - Create and manage issues, projects, and workflows.
* Notion - Create and edit pages, databases, and content.
* Sentry - Monitor errors, triage issues, and track performance.
* Slack - Send messages, search channels, manage conversations.
* Vercel - Deploy, preview, and manage Vercel projects.

</details>

## Community Plugins

Third-party plugins built by the community. [PRs welcome](#contributing)!

### Development & Workflow

<!-- pinned -->

* [Claude Code Skills](https://github.com/alirezarezvani/claude-skills) ⭐ 24,376 | 🐛 26 | 🌐 Python | 📅 2026-08-09 - 223 production-ready skills, 23 agents, and 298 Python tools across 9 domains — engineering, marketing, product, compliance, and more.
* [Generative Media Skills](https://github.com/SamurAIGPT/Generative-Media-Skills) ⭐ 4,044 | 🐛 4 | 🌐 Shell | 📅 2026-08-08 - 13 skills for image, video, and audio generation using 100+ models - FLUX, Midjourney v7, Veo3, Kling 3.0, Suno, and HunyuanVideo via muapi.ai.
* [Claude Octopus](https://github.com/nyldn/claude-octopus) ⭐ 3,961 | 🐛 11 | 🌐 Shell | 📅 2026-08-13 - Multi-LLM orchestration dispatching to 8 providers (Codex, Gemini, Copilot, Qwen, Perplexity, OpenRouter, Ollama, OpenCode) with Double Diamond workflows, adversarial review, and safety gates.
* [Antigravity Workspace Template](https://github.com/study8677/antigravity-workspace-template) ⭐ 1,307 | 🐛 2 | 🌐 Python | 📅 2026-08-13 - Multi-agent codebase knowledge graph generator with context-aware planning and automatic scope management — turns codebases into coherent agent workspaces.
* [Brooks Lint](https://github.com/hyhmrright/brooks-lint) ⭐ 1,300 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-04 - AI code reviews grounded in six classic engineering books — decay risk diagnostics with book citations, severity labels, and four analysis modes (PR review, architecture audit, tech debt, test quality).
* [Aegis](https://github.com/GanyuanRan/Aegis) ⭐ 992 | 🐛 0 | 🌐 Python | 📅 2026-08-13 - An agentic skills framework & software development methodology that works: planning, TDD, debugging, and collaboration workflows.
* [spec-superflow](https://github.com/MageByte-Zero/spec-superflow) ⭐ 738 | 🐛 6 | 🌐 JavaScript | 📅 2026-08-10 - Spec-first workflow with nine skills, user-controlled Quick / Hotfix / Tweak / Full paths, auditable recovery commands, hardened delta-spec sync, and guarded review gates.
* [Boss](https://github.com/echoVic/boss-skill) ⭐ 552 | 🐛 13 | 🌐 TypeScript | 📅 2026-08-09 - BMAD pipeline plugin that orchestrates a full requirements-to-deploy workflow across nine specialist agents with an auditable runtime DAG and quality gates, for Claude Code, Codex, OpenClaw, and Antigravity.
* [token-optimizer](https://github.com/ooples/token-optimizer-mcp) ⭐ 480 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-12 - Cut token usage 60-90% with caching, compression, and smart file tools — diff-only re-reads, paths-only search, out-of-context stashing, and a per-tool savings report for Codex and Claude Code.
* [Codex Multi Auth](https://github.com/ndycode/codex-multi-auth) ⭐ 441 | 🐛 9 | 🌐 TypeScript | 📅 2026-08-13 - Multi-account OAuth manager for the official Codex CLI with switching, health checks, and recovery tools.
* [AgentOps](https://github.com/boshu2/agentops) ⭐ 420 | 🐛 3 | 🌐 Go | 📅 2026-08-12 - DevOps layer for coding agents with flow, feedback, and memory that compounds between sessions.
* [Reviewable HTML Workbench](https://github.com/u-ichi/reviewable-html-workbench) ⭐ 281 | 🐛 2 | 🌐 Python | 📅 2026-08-09 - Generate reviewable HTML documents, serve previews, collect inline review comments, and feed review outcomes back into agent workflows.
* [Ditto](https://github.com/ohad6k/ditto) ⭐ 220 | 🐛 21 | 🌐 Python | 📅 2026-08-04 - Mines selected evidence from local coding-agent sessions into private work, design, and writing profiles for Codex, Claude Code, and GitHub Copilot.
* [Claude Code for Codex](https://github.com/sendbird/cc-plugin-codex) ⭐ 167 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-10 - Reverse of OpenAI's official Claude-hosted plugin: use Claude Code from Codex for reviews, rescue tasks, tracked background jobs, and hook-powered review gates.
* [Krypton](https://github.com/jturntdev/krypton) ⭐ 128 | 🐛 2 | 🌐 Shell | 📅 2026-07-24 - Goal-based planning and proof gate for Codex and Claude Code that turns requests into ownership, cutover, review-gate, and acceptance-evidence plans.
* [Superloopy](https://github.com/beefiker/superloopy) ⭐ 106 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-11 - Evidence-gated Codex loop harness with specialist skills, including near-pixel authorized website cloning backed by screenshots, assets, build output, and visual QA.
* [Sealos](https://github.com/labring/sealos-skills) ⭐ 69 | 🐛 6 | 🌐 Python | 📅 2026-08-12 - Deploy apps to Sealos Cloud from Codex with readiness checks, Dockerfile generation, Compose conversion, image builds, and rollout updates.
* [Archcore](https://github.com/archcore-ai/plugin) ⭐ 52 | 🐛 15 | 🌐 Shell | 📅 2026-08-11 - Gives coding agents the architecture, rules, and prior decisions of the repo via skills, hooks, and MCP — so new changes land where the project says they belong across Claude Code, Cursor, and Codex CLI.
* [Honcho](https://github.com/plastic-labs/codex-honcho) ⭐ 47 | 🐛 7 | 🌐 TypeScript | 📅 2026-07-16 - Persistent cross-session memory for Codex powered by Honcho — lifecycle hooks capture each session and inject relevant context back at session start, so Codex remembers your preferences, projects, and decisions across restarts.
* [Session Orchestrator](https://github.com/Kanevry/session-orchestrator) ⭐ 45 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-09 - Session orchestration for Claude Code, Codex, and Cursor IDE — structured planning, wave-based execution, VCS integration (GitLab + GitHub), quality gates, and clean session close-out with issue tracking.
* [memi](https://github.com/sarveshsea/memi) ⭐ 39 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-08 - Interface understanding and design-system memory for Codex, Claude Code, Cursor, and MCP agents with UI audits, Tailwind token extraction, shadcn registry workflows, and a bundled Codex plugin.
* [Docflow](https://github.com/MedAdemBHA/docflow) ⭐ 37 | 🐛 0 | 🌐 Shell | 📅 2026-08-12 - Lightweight documentation memory for AI coding agents that scaffolds a 7-category docs tree, runs readiness checks, validates docs before finishing, and keeps a monthly changelog across Claude Code and Codex.
* [Waggle](https://github.com/Abhigyan-Shekhar/Waggle-mcp) ⭐ 35 | 🐛 223 | 🌐 Python | 📅 2026-08-12 - Persistent graph-backed conversational memory for Codex that recalls project decisions, constraints, preferences, and outcomes across sessions.
* [Codebase Recon](https://github.com/yujiachen-y/codebase-recon-skill) ⭐ 31 | 🐛 0 | 📅 2026-04-26 - Analyze git history to understand a codebase before reading any code — auto-scales by repo size and cross-references hotspots with bug magnets to surface high-risk files, bus factor, and team momentum.
* [Velith](https://github.com/epicsagas/Velith) ⭐ 30 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-09 - AI-native publishing system with a 6-phase pipeline from ideation to EPUB/PDF across 8 genres.
* [Designer Skill](https://github.com/Pythoughts-labs/designer-skill) ⭐ 27 | 🐛 8 | 🌐 JavaScript | 📅 2026-08-02 - Plug-and-play MCP that gives your agent UI superpowers. One install: design skill + MCP server, zero config.
* [Open Dynamic Workflows](https://github.com/Suraj1235/open-dynamic-workflows) ⭐ 26 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-09 - Local-first MIT dynamic multi-agent workflows for Codex, OpenCode, Antigravity, Cursor, and VS Code with a daemon, MCP bridge, Codex skills, OpenCode plugin, and bring-your-own-model support.
* [Hera Agent Unity](https://github.com/NotNull92/hera-agent-unity) ⭐ 25 | 🐛 0 | 🌐 C# | 📅 2026-08-13 - Controls and verifies a live Unity Editor through a low-token CLI, with scene, asset, Inspector, Play Mode, test, screenshot, and runtime C# workflows for Codex and other coding agents.
* [HOTL Plugin](https://github.com/yimwoo/hotl-plugin) ⭐ 25 | 🐛 0 | 🌐 Shell | 📅 2026-07-06 - Human-on-the-Loop AI coding workflow plugin for Codex, Claude Code, and Cline with structured planning, review, and verification guardrails.
* [VibePortrait](https://github.com/dadwadw233/VibePortrait) ⭐ 25 | 🐛 0 | 🌐 HTML | 📅 2026-04-08 - Developer personality portrait generator — analyzes AI conversation history to produce MBTI type (16 color themes), capability radar, developer rating, 3-dimension famous match, and a persona skill that lets any AI "think like you".
* [Stark](https://github.com/f0d010c/stark) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-07-26 - UI/UX design plugin for AI coding agents with product-flow routing, platform-native interface guidance, asset planning, and shipped-reference analysis before code.
* [AgentPack](https://github.com/vishal2612200/agentpack) ⭐ 23 | 🐛 17 | 🌐 Python | 📅 2026-08-13 - Ranks repo context for Codex with likely files, skill recommendations, agent rules, commands, warnings, and compact task-focused packs before editing.
* [Agent Guard](https://github.com/JeongJaeSoon/agent-guard) ⭐ 19 | 🐛 10 | 🌐 Shell | 📅 2026-08-12 - Real-time secret-leak guardrails for AI coding agents (Claude Code, Codex), Git hooks, and CI.
* [Frappe Agent](https://github.com/Dkm0315/frappe-agent) ⭐ 19 | 🐛 2 | 📅 2026-07-26 - Frappe and ERPNext coding, customization, bench, and review intelligence for Codex.
* [Quality Engineering Skills](https://github.com/RBraga01/Quality-Engineering-Skills) ⭐ 19 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-10 - 22 structured quality engineering skills for automotive and manufacturing: ISO 9001, IATF 16949, AIAG-VDA FMEA, VDA 6.3, PPAP, APQP, SPC, MSA.
* [RAG Reviewer](https://github.com/mimfort/rag_for_git) ⭐ 19 | 🐛 0 | 🌐 Python | 📅 2026-08-13 - Agentic PR review: hybrid RAG + code graph via MCP, review skills for Codex.
* [Espresso](https://github.com/mirkobozzetto/espresso) ⭐ 17 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-08 - Full token-saving stack in one plugin - output compression, global rules, RTK hook, Caveman ultra, GitNexus config. Detects existing setup, installs only what's missing. Works on Claude Code and Codex.
* [Alcove](https://github.com/epicsagas/alcove) ⭐ 15 | 🐛 3 | 🌐 Rust | 📅 2026-08-13 - Local-first MCP server for private project docs with hybrid BM25+vector search, tree-sitter code indexing, and automated linting for team-wide documentation standards.
* [Epic Harness](https://github.com/epicsagas/epic-harness) ⭐ 15 | 🐛 8 | 🌐 Rust | 📅 2026-07-23 - Auto-trigger quality skills + self-evolving agent harness — orbit (spec-to-ship), evolve (skill mutation), team (multi-agent), TDD, check, ship, simplify, debug, perf, secure.
* [Codex Reviewer](https://github.com/schuettc/codex-reviewer) ⭐ 14 | 🐛 0 | 📅 2026-05-05 - Second-pass review of Claude-driven plans and implementations.
* [ejentum-mcp](https://github.com/ejentum/ejentum-mcp) ⭐ 14 | 🐛 1 | 🌐 JavaScript | 📅 2026-06-11 - MCP server exposing reasoning, code, anti-deception, and memory harness tools for Codex.
* [Project Autopilot](https://github.com/AlexMi64/codex-project-autopilot) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2026-04-09 - Turn an idea into a structured project workflow with planning, execution, verification, and handoff.
* [A Team](https://github.com/RBraga01/a-team) ⭐ 13 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-09 - Universal multi-agent infrastructure with 25 specialist agents, 16 enforced workflow skills, and a lead orchestrator for Claude Code, Codex CLI, Cursor, and OpenCode.
* [Staff Engineer Mode](https://github.com/sirmarkz/staff-engineer-mode) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2026-08-01 - Routes engineering design, delivery, reliability, security, operations, and maintenance prompts to focused staff-level specialist guidance for AI coding agents.
* [Tool Advisor](https://github.com/dragon1086/claude-skills) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-04-23 - Read-only meta-skill that scans your MCP servers, skills, plugins, and CLI tools, then suggests up to three ranked approaches (Methodical / Fast / Deep) with a copy-paste Quick Action table.
* [BGS Modding Superpowers](https://github.com/BB-84C/bgs-modding-superpowers) ⭐ 11 | 🐛 2 | 🌐 Python | 📅 2026-08-12 - Agentic Bethesda Game Studio modpack curation toolkit with MCP-driven xEdit conflict audit, MO2 control plane, BA2/BSA and Papyrus tooling, and skills for setup, dev-log, and release-changelog workflows.
* [Claude Code Harness](https://github.com/dadwadw233/claude-code-harness) ⭐ 11 | 🐛 0 | 📅 2026-04-05 - Harness blueprint skill for turning vague agent ideas into concrete designs for request assembly, control loops, memory, permissions, recovery, and extension planes.
* [Development Skills](https://github.com/reidemeister94/development-skills) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2026-07-24 - Three-tier triage (PASS\_THROUGH / LIGHT / FULL 4-phase) development workflow for Codex and Claude Code with language auto-detection (Python, Java, TypeScript, Swift, frontend) and a staff-reviewer subagent for fresh-eyes review on every change.
* [Hera Agent Godot](https://github.com/NotNull92/hera-agent-godot) ⭐ 11 | 🐛 0 | 🌐 Go | 📅 2026-07-29 - Drives a live Godot 4.x editor through the low-token Hera CLI — scene, node, and signal edits, play control, and runtime QA with verifiable compact JSON output, with the companion addon published on the official Godot Asset Store.
* [Writer's Loop](https://github.com/xxsang/writers-loop) ⭐ 11 | 🐛 0 | 🌐 JavaScript | 📅 2026-05-09 - Structured AI writing workflow for planning, critique, revision, translation, style distillation, and opt-in local preference learning.
* [Casefile](https://github.com/x4cc3/casefile) ⚠️ Archived - Persistent security case tracking for bug bounties, CTFs, and security audits.
* [Codex Agenteam](https://github.com/yimwoo/codex-agenteam) ⭐ 10 | 🐛 0 | 🌐 Python | 📅 2026-07-06 - Specialist AI agents (researcher, PM, architect, developer, QA, reviewer) orchestrated as a configurable team pipeline.
* [Spec-Driven Development](https://github.com/Habib0x0/spec-driven-plugin) ⭐ 10 | 🐛 0 | 🌐 Shell | 📅 2026-05-18 - Three-phase Requirements → Design → Tasks workflow for Claude Code and Codex — EARS notation acceptance criteria, autonomous execution loop, cross-spec dependencies, and post-implementation acceptance testing.
* [Clean Room](https://github.com/whit3rabbit/clean-room-skill) ⭐ 9 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-04 - Spec-first clean-room workflow for authorized source analysis, behavioral specs, role separation, and verification without replacement code.
* [Agent Harness Skills](https://github.com/yfge/agent-harness-skills) ⭐ 8 | 🐛 2 | 🌐 Python | 📅 2026-07-14 - Designs agent-ready repository harnesses with entrypoints, validation surfaces, runtime evidence, delivery records, and atomic commit guidance.
* [debt-ops](https://github.com/bcanfield/agentic-tech-debt) ⭐ 8 | 🐛 13 | 🌐 Python | 📅 2026-08-10 - Catches AI-introduced tech debt at write-time: hooks log every deferral to a registry in your repo and a review skill ranks paydown by file churn.
* [Praxis](https://github.com/ouonet/praxis) ⭐ 7 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-05 - Intent-driven workflow skills for coding agents: describe what done looks like, not the steps. Triage-first design keeps token costs low across design, TDD, debug, review, and release.
* [Tartiner Labs](https://github.com/tartinerlabs/skills) ⭐ 7 | 🐛 8 | 🌐 Go | 📅 2026-08-12 - Agent skills for git workflows, GitHub automation, security audits, code refactoring, and project tooling.
* [Wingman](https://github.com/lsshym/wingman.ai) ⭐ 7 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-21 - Cross-platform AI coding-agent plugin for repo-local project memory, data-contract checks, and project-map discovery before agents edit code.
* [BABOK Analyst](https://github.com/GSkuza/BABOK_ANALYST) ⭐ 6 | 🐛 9 | 🌐 JavaScript | 📅 2026-08-13 - BABOK v3 business analysis agent with 16 MCP tools, a 9-stage pipeline, and human-in-the-loop approval gates.
* [Universal Design Principles](https://github.com/HDeibler/universal-design-principles) ⭐ 6 | 🐛 1 | 🌐 Markdown | 📅 2026-05-03 - Cross-agent UX and product-design marketplace with a root Codex collection plugin, five focused plugin bundles, and 137 Agent Skills for design review, accessibility, layout, interaction, cognition, and product polish.
* [Zagrosi Forge](https://github.com/zagrosi-code/zagrosi-forge) ⭐ 6 | 🐛 1 | 🌐 Python | 📅 2026-08-13 - Decompose broad project briefs into researched plans and implement sectioned work with TDD, quality gates, and traceability.
* [Dev Skills](https://github.com/Jason-chen-coder/dev-skills) ⭐ 5 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-12 - Team workflow skills for specs, plans, TDD, debugging, verification, review, branch finishing, and design context.
* [LLM Transpile](https://github.com/epicsagas/llm-transpile) ⭐ 5 | 🐛 5 | 🌐 HTML | 📅 2026-07-24 - Auto-compress .md, .html, and .txt files via PostToolUse hook, cutting context usage by up to 40% with zero workflow change.
* [VillageSQL Skills](https://github.com/villagesql/villagesql-skills) ⭐ 5 | 🐛 1 | 📅 2026-08-11 - Skills for VillageSQL including building extensions from scratch and porting PostgreSQL extensions to VillageSQL.
* [Agent Workflow System](https://github.com/1139030773-cmd/agent-workflow-system) ⭐ 4 | 🐛 0 | 🌐 PowerShell | 📅 2026-06-12 - 一套中文AI工作流系统：7个协作技能 + 行为规范宪法 + 会话恢复机制，模糊目标→可执行任务，全生命周期引导。Codex & Claude Code 双平台，新手友好。
* [Agentizer](https://github.com/Humiris/wwa-transform) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2026-05-05 - Turn any website into an AI-powered agentfront with split-pane
* [Codex rg Guard](https://github.com/Rycen7822/codex-rg-guard) ⭐ 4 | 🐛 0 | 🌐 Rust | 📅 2026-05-09 - Budgeted `rg`/`grep` replacement for Codex that narrows broad searches before they waste model context.
* [Superpipelines](https://github.com/gustavo-meilus/superpipelines) ⭐ 4 | 🐛 13 | 🌐 JavaScript | 📅 2026-07-15 - Design and run write/review-isolated multi-agent AI pipelines across Codex, Claude Code, OpenCode, Cursor, Windsurf, and Cline.
* [tailtest](https://github.com/avansaber/tailtest-codex) ⭐ 4 | 🐛 9 | 🌐 Python | 📅 2026-06-13 - Hook-powered test generation -- detects files changed during an agent turn and instructs Codex to write and run tests automatically. Zero config, 8 languages.
* [HOL Guard Plugin](https://github.com/hashgraph-online/hol-guard-plugin) ⭐ 3 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-13 - AI antivirus workflow for Codex, Claude Code, Cursor, Gemini, OpenCode, MCP servers, skills, and plugin release checks with local approvals and receipts.
* [Maestro](https://github.com/mbanderas/maestro) ⭐ 3 | 🐛 3 | 🌐 JavaScript | 📅 2026-07-27 - Opt-in local multi-CLI fusion engine and orchestration doctrine that fans a prompt across model CLIs, then judges and synthesizes one grounded answer.
* [AgiFlow](https://github.com/AgiFlow/ai-plugin) ⭐ 2 | 🐛 0 | 📅 2026-07-10 - Project management workflows for AI coding agents with planning, grooming, task execution, review, and AgiFlow MCP integration.
* [AIBoarding](https://github.com/gustavo-meilus/aiboarding) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-07-15 - Generate, maintain, compress, and audit standard AI-agent onboarding files with AGENTS.md, CLAUDE.md, drift tracking, and lifecycle hooks.
* [Anchor](https://github.com/biefan/anchor) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-05-22 - Engineering discipline pack for Claude Code & Codex CLI with task-scope locking, anti-drift braking, condition-based codex review, project-CLAUDE.md pitfall writeback, and PreToolUse hooks that block irreversible bash patterns.
* [ArmorCodex](https://github.com/armoriq/armorCodex) ⭐ 2 | 🐛 24 | 🌐 JavaScript | 📅 2026-08-11 - Intent-based security for Codex with MCP plan registration, policy gating, CSRG cryptographic proofs, and audit logging on `bash` and `apply_patch`.
* [Codex How To](https://github.com/Phelan164/codex-howto) ⭐ 2 | 🐛 3 | 🌐 Python | 📅 2026-08-11 - Engineering-first Codex curriculum and plugin with 9 skills, measured token-efficiency experiments, bounded orchestration, testing, review, and living knowledge maintenance.
* [Codex Skin Pack Installer](https://github.com/ChannelerH/codex-skin-packs) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-07-24 - Codex plugin and Skill that stages verified desktop skin packs from GitHub releases, validates files, and keeps restore guidance visible.
* [falsegreen-skill](https://github.com/vinicq/falsegreen-skill) ⭐ 2 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-11 - Finds tests that stay green when the code they cover is broken, applying six ordered judgments over Python, TypeScript, JavaScript, and Robot Framework suites in Codex CLI and Claude Code.
* [GrayMatter](https://github.com/ValkyrLabs/GrayMatter) ⭐ 2 | 🐛 1 | 🌐 Shell | 📅 2026-08-06 - Durable memory and shared graph state for Codex and OpenClaw agents, with live ValkyrAI schema awareness.
* [River Review](https://github.com/s977043/river-review) ⭐ 2 | 🐛 18 | 🌐 JavaScript | 📅 2026-08-13 - Versioned Skill Registry of code-review skills driven by a perspective-based review agent (code, security, performance, architecture, testing, adversarial) that verifies findings against the diff.
* [Simple Man](https://github.com/Maksim-Burtsev/simple-man) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-08-01 - High-compression communication mode for Codex agents that removes filler while preserving search, validation, and implementation effort.
* [Team Skills Platform](https://github.com/Colin4k1024/tsp) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-07 - Role-based team delivery framework — Tech Lead-orchestrated 8-role system with 195+ skills, 27 specialist agents, 80+ commands, hooks, and ECC harness for Claude Code, Codex, and OpenCode.
* [Agentry Observability](https://github.com/fr33dr4g0n/agentry-public) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-07-13 - Agent-native product analytics, error logging, and deploy attribution for coding agents through one HTTP API.
* [Bring Your AI Migration Auditor](https://github.com/unitedideas/bringyour-mcp) ⭐ 1 | 🐛 0 | 📅 2026-05-25 - Read-only Codex plugin for auditing Claude Code to Codex migrations before Codex edits code. Checks AGENTS.md/CLAUDE.md scope, hooks, MCP config, skills, secret references, and validation notes.
* [Codex Full-Stack Workflow](https://github.com/kevin592/codex-full-stack-workflow) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-08 - Turns rough product requests into staged, reviewable full-stack delivery with persistent requirements, change control, visual evidence, and completion gates.
* [Codex Process Jobs](https://github.com/joelfarthing/codex-process-jobs) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-09 - Run long local builds, tests, benchmarks, and inference jobs as durable detached processes with tracked status, bounded results, and completion delivery across Codex surfaces.
* [Codex Usage and Resets](https://github.com/joelfarthing/codex-usage-and-resets) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-31 - Turns Codex usage into planning facts with linear pace, projected exhaustion, banked-reset expirations, and conservative unexpected-reset detection.
* [Context Guard](https://github.com/GreenLv/codex-context-guard) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-12 - Preserves authoritative requirements and verification evidence across long-running Codex tasks and context compaction.
* [dev-harness-kit](https://github.com/sh-ai-x/dev-harness-kit) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-13 - Enforced development workflow skills for Codex and Claude Code covering planning, TDD, debugging, review, security, CI, and release.
* [GCF Proxy](https://github.com/blackwell-systems/gcf-codex-plugin) ⭐ 1 | 🐛 2 | 📅 2026-07-25 - Save 71% on MCP tool call tokens by wrapping any server with GCF encoding, with session stats hook and setup skill.
* [LVTD Skills](https://github.com/LVTD-LLC/skills) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-07-28 - Reusable Agent Skills for Codex, Claude Code, and compatible clients, covering Django, Rust, Cookiecutter, SEO, traction, product marketing, and nonfiction publishing workflows.
* [MailAgent](https://github.com/Alex0nder/MailAgent) ⚠️ Archived - Temporary inboxes for Codex — OTP, magic links, signup QA, simulate-first autotests (23 MCP tools).
* [Registry Broker](https://github.com/hashgraph-online/registry-broker-codex-plugin) ⭐ 1 | 🐛 17 | 🌐 TypeScript | 📅 2026-07-20 - Delegate tasks to specialist AI agents via the HOL Registry, plan, find, summon, and recover sessions.
* [RoadmapSmith](https://github.com/PapiScholz/roadmapsmith) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-25 - Evidence-backed ROADMAP.md workflows for AI coding agents with validation, sync, and roadmap generation across any tech stack.
* [Runtype Skills](https://github.com/runtypelabs/skills) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-13 - Supercharge your coding agent for AI product development — build, deploy, and operate agents, flows, tools, and surfaces on Runtype's managed edge runtime.
* [Spellbook Skills](https://github.com/yyykf/spellbook-skills) ⭐ 1 | 🐛 3 | 🌐 Python | 📅 2026-07-25 - Practical Claude Code and Codex skills for worktrees, PR/MR automation, review cleanup, YApi lookup, and Java DDD guidance.
* [Tandem Workflow Architect](https://github.com/frumu-ai/tandem-codex-plugin) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-05-21 - Plan Tandem workflows in Codex, then validate, preview, and run them through the governed Tandem engine.
* [UIZZE](https://github.com/uizze/uizze) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-09 - STOP UI SLOP. Gives Codex 800,000+ real web and iOS screens, a product-specific design contract, and a hard finish gate before generic UI ships; connect it at <https://uizze.com>.
* [Unforgit](https://github.com/MiguelMedeiros/unforgit-codex-plugin) ⭐ 1 | 🐛 2 | 📅 2026-07-24 - Git-backed repository memory for Codex and other coding agents via MCP, with durable local knowledge for decisions, conventions, gotchas, and playbooks.
* [Agency Continuity Audit](https://github.com/revertcreations/agency-continuity-audit) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-08-05 - Read-only audit that distinguishes durable agent goals, state, corrections, restart evidence, authority boundaries, scheduler claims, and commercial proof from self-reported health.
* [Agent Deck](https://github.com/not-so-fat/agent-deck) ⭐ 0 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-13 - One MCP for context management: bind self-improving playbooks, MCP tools, and API keys to the session.
* [Claude Code Codex Plugin](https://github.com/davidq888/claude-code-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-22 - Security-focused Codex plugin that connects to the local Claude Code CLI through MCP with login, status checks, safe-mode prompts, and no credential storage.
* [CodeTruss](https://github.com/DeliriumPulse/codetruss-plugins) ⭐ 0 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-12 - Local-first acceptance gate that checks coding-agent scope, sensitive surfaces, deterministic analyzers, and repository verification from immutable Git snapshots, then writes signed receipts before the PR.
* [Codex TUI Proof](https://github.com/bnc4vk/codex-tui-proof) ⭐ 0 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-01 - Visually validate real local terminal UIs in Codex's in-app browser with screenshots and session evidence.
* [Ontoly](https://github.com/0xsarwagya/ontoly-codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-07-21 - Deterministic Software Graph workflows for Codex: architecture review, dependency analysis, request tracing, configuration analysis, and impact analysis.
* [Personal Data Protection](https://github.com/AltByteSG/personal-data-protection-skill) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-05-17 - Engineer-facing personal-data-protection compliance reference — Singapore PDPA, Thailand PDPA, Indonesia UU PDP, Malaysia PDPA (Act 709 + 2024 Amendments), Philippines DPA — organised by where in the stack each obligation lands, with checklists, breach-response runbook, and a developer-view divergence table across all five.
* [skill-sync-publisher](https://github.com/liuyewang/skill-sync-publisher) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-28 - Safely synchronize this Codex skill across public agent-skill registries.
* [Tree Ring Memory](https://github.com/TerminallyLazy/tree-ring-memory-codex-plugin) ⭐ 0 | 🐛 2 | 🌐 Shell | 📅 2026-07-23 - Local-first memory lifecycle guidance for Codex agents with recall, evidence-backed lessons, privacy-safe memory capture, audit, consolidation, and explicit forgetting.
* [Unity Agent Workflows](https://github.com/AUN-PN/unity-agent-workflows) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-05-19 - Codex plugin and skill for Unity 2D agents that enforces "No proof, no edit" workflows with runtime-owner proof, Teach structure maps, and validation gates.
* [Workflow Kit](https://github.com/Le-Xuan-Thang/workflow-kit) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-06-02 - Full product lifecycle plugin for Claude Code, Codex CLI, and OpenCode: define Vision/Mission/Core → generate workplan → execute with mandatory cross-provider reviewer agents → synthesize deliverables → maintain, with parallel task execution, crash recovery, and AgentOps metrics.
* [Changelog Forge](./plugins/mturac/changelog-forge) - Conventional commits → CHANGELOG section + semver bump.
* [Commit Narrator](./plugins/mturac/commit-narrator) - Generate semantic commit message from staged diff, including the *why*.
* [Deps Doctor](./plugins/mturac/deps-doctor) - Multi-ecosystem dependency audit (npm, pip, cargo, go) in one report.
* [Env Lint](./plugins/mturac/env-lint) - `.env` vs `.env.example` key parity — never prints values.
* [Flaky Detector](./plugins/mturac/flaky-detector) - Run a test command N times, report per-test flakiness %.
* [PR Storyteller](./plugins/mturac/pr-storyteller) - PR title + body + test plan from commits and diff vs base branch.
* [Secret Guard](./plugins/mturac/secret-guard) - Pre-commit secret scanner using pattern and entropy detection.
* [Standup Generator](./plugins/mturac/standup-gen) - Daily standup notes from git activity across repos.
* [Test Gap](./plugins/mturac/test-gap) - Find lines in your diff lacking test coverage (Cobertura, lcov, coverage.json).
* [TODO Harvest](./plugins/mturac/todo-harvest) - TODO/FIXME/HACK scan with `git blame` author + age.

### Tools & Integrations

* [KiCad Happy](https://github.com/aklofas/kicad-happy) ⭐ 952 | 🐛 6 | 🌐 Python | 📅 2026-08-01 - KiCad EDA skills for schematic analysis, PCB layout review, component sourcing, BOM management, and manufacturing preparation.
* [Digital Marketing Pro](https://github.com/indranilbanerjee/digital-marketing-pro) ⭐ 734 | 🐛 1 | 🌐 Python | 📅 2026-08-12 - Open-source AI marketing plugin for agencies — 154 skills, 25 specialist agents, 12-Part Strategy Flow, AEO/GEO, GSC AI Performance Report, Google Ads API v24, EU AI Act Article 50 / C2PA compliance.
* [Education Agent Skills](https://github.com/GarethManning/education-agent-skills) ⭐ 611 | 🐛 8 | 🌐 TypeScript | 📅 2026-08-10 - 131 evidence-based education skills for curriculum design, lesson planning, and assessment, with transparent evidence ratings and MCP server.
* [LinkedIn Skills](https://github.com/sergebulaev/linkedin-skills) ⭐ 546 | 🐛 0 | 🌐 Python | 📅 2026-08-09 - Codex-ready LinkedIn marketing bundle with a native .codex-plugin manifest and 10 skills: post writing with 16 tested hook formulas, AI-tell humanizer, pre-publish audit, comment and reply drafting, hook extraction, content planning, profile optimization, engager analytics, and thread monitoring; also works in Claude Code.
* [Taisly Agent Kit](https://github.com/taisly/agent) ⭐ 255 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-06 - Publish short-form videos to TikTok, Instagram Reels, YouTube Shorts, X, and Facebook from Codex with the Taisly MCP server and bundled social media posting skill.
* [ru-text](https://github.com/talkstream/ru-text) ⭐ 195 | 🐛 0 | 🌐 Shell | 📅 2026-08-12 - Russian text quality — \~1,044 rules for typography, info-style, editorial, UX writing, and business correspondence.
* [Codex Usage Tracker](https://github.com/douglasmonsky/codex-usage-tracker) ⭐ 191 | 🐛 10 | 🌐 Python | 📅 2026-08-12 - Track aggregate Codex token usage from local session logs with MCP tools for summaries, session detail, CSV export, and dashboard generation.
* [Bitbucket CLI](https://github.com/avivsinai/bitbucket-cli) ⭐ 184 | 🐛 0 | 🌐 Go | 📅 2026-08-12 - Manage Bitbucket repos, PRs, branches, issues, webhooks, and pipelines for Data Center and Cloud.
* [X Twitter Scraper](https://github.com/Xquik-dev/x-twitter-scraper) ⭐ 178 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-13 - X/Twitter data, monitored workflows, HMAC webhooks, and MCP access through the Xquik REST API with confirmation-gated write guidance.
* [OC ChatGPT Multi Auth](https://github.com/ndycode/oc-chatgpt-multi-auth) ⭐ 170 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-11 - Codex setup skill and OpenCode plugin for ChatGPT Plus/Pro OAuth, GPT-5/Codex presets, and multi-account failover.
* [Langfuse Observability](https://github.com/avivsinai/langfuse-mcp) ⭐ 104 | 🐛 2 | 🌐 Python | 📅 2026-08-09 - Query traces, debug exceptions, analyze sessions, and manage prompts via MCP tools.
* [unslop](https://github.com/MohamedAbdallah-14/unslop) ⭐ 94 | 🐛 3 | 🌐 Python | 📅 2026-06-29 - Strip AI writing patterns from text output — removes filler phrases, hedging language, and generic constructs to produce cleaner written content. Install: `npm install -g unslop`.
* [Agent Message Queue](https://github.com/avivsinai/agent-message-queue) ⭐ 81 | 🐛 1 | 🌐 Go | 📅 2026-08-13 - File-based inter-agent messaging with co-op mode, cross-project federation, and orchestrator integrations.
* [Jenkins CLI](https://github.com/avivsinai/jenkins-cli) ⭐ 81 | 🐛 1 | 🌐 Go | 📅 2026-08-11 - GitHub CLI-style interface for Jenkins controllers with jobs, pipelines, runs, logs, artifacts, credentials, and nodes.
* [Call-E](https://github.com/CALLE-AI/call-e-integrations) ⭐ 74 | 🐛 6 | 🌐 JavaScript | 📅 2026-08-11 - Plan, run, and inspect Call-E phone call workflows from Codex through the calle CLI.
* [Talivia Agent Kit](https://github.com/talivia-group/agent) ⭐ 61 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-02 - Install and verify revenue-first website analytics from Codex, connect payment attribution, and identify which traffic sources and customer journeys become revenue.
* [ScrapeGraph AI](https://github.com/ScrapeGraphAI/just-scrape) ⭐ 46 | 🐛 4 | 🌐 TypeScript | 📅 2026-07-27 - AI-powered web scraping CLI to search, scrape, extract structured JSON, crawl, and monitor web pages via the ScrapeGraph AI API.
* [X (Twitter) Skills](https://github.com/sergebulaev/x-skills) ⭐ 44 | 🐛 0 | 🌐 Python | 📅 2026-08-09 - Codex-ready X (Twitter) marketing bundle with a native .codex-plugin manifest: tweet and thread writing with corpus-validated hook formulas (validated against \~450 top tweets), AI-tell humanizer, hook extraction, reply drafting, content planning, and audience insights; also works in Claude Code.
* [PANews Agent Toolkit](https://github.com/panewslab/skills) ⭐ 42 | 🐛 0 | 🌐 JavaScript | 📅 2026-04-16 - Crypto and blockchain news discovery, authenticated creator publishing workflows, and page-to-Markdown reading.
* [Kachilu Browser](https://github.com/kachilu-inc/kachilu-browser) ⭐ 38 | 🐛 0 | 🌐 JavaScript | 📅 2026-05-12 - Anti-bot-aware browser automation for AI agents with MCP tools, CAPTCHA-aware workflows, and WSL2 Windows browser support.
* [Pronounce](https://github.com/anzy-renlab-ai/pronounce) ⭐ 33 | 🐛 1 | 🌐 Shell | 📅 2026-07-28 - Pronounce developer jargon out loud: an MCP server (lookup/search) and skill backed by a 1,721-entry sourced dictionary with IPA, audio, and cited pronunciations for kubectl, nginx, YAML, JWT, and more.
* [Flow Studio Power Automate](https://github.com/ninihen1/power-automate-mcp-skills) ⭐ 28 | 🐛 2 | 🌐 JavaScript | 📅 2026-05-10 - Debug, build, and operate Power Automate flows via FlowStudio MCP with action-level inputs and outputs.
* [MorningAI](https://github.com/octo-patch/MorningAI) ⭐ 28 | 🐛 1 | 🌐 Python | 📅 2026-05-16 - AI news tracking skill that monitors 80+ entities across 6 sources (Reddit, HN, GitHub, Hugging Face, arXiv, X) and generates scored daily reports with infographics and message digests.
* [Hermes Tweet](https://github.com/Xquik-dev/hermes-tweet) ⭐ 26 | 🐛 1 | 🌐 Python | 📅 2026-08-13 - Hermes Agent X/Twitter plugin for read-first social research, monitoring, and approval-gated actions through Xquik.
* [Kreuzberg](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Local document extraction for 91+ formats with skills for CLI usage, OCR, table extraction, output formats, and a local MCP server.
* [Kreuzberg Cloud](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Managed document extraction for Codex with API-key setup, presigned uploads, job tracking, webhook workflows, and usage guidance.
* [Kreuzcrawl](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Web crawling and scraping for Codex with skills for single-page scraping, site crawls, URL mapping, and headless browser fallback.
* [Codex Obsidian](https://github.com/greg-asher/codex-obsidian) ⭐ 24 | 🐛 1 | 📅 2026-04-22 - Local Obsidian note and vault workflows through the official desktop `obsidian` CLI.
* [Yandex Direct](https://github.com/nebelov/yandex-direct-for-all) ⭐ 20 | 🐛 1 | 🌐 Python | 📅 2026-07-17 - GitHub-ready Codex plugin bundle for Yandex Direct, Wordstat, Metrika, and Roistat.
* [prompt-to-asset](https://github.com/MohamedAbdallah-14/prompt-to-asset) ⭐ 17 | 🐛 14 | 🌐 TypeScript | 📅 2026-08-12 - Route image-generation prompts to 30+ models (DALL-E, Stable Diffusion, Flux, Midjourney, and more) through a single MCP interface. Install: `npm install -g prompt-to-asset`.
* [Thermal-Fluid Research Workflow](https://github.com/hanhuark/mechanical-engineering-research-skill) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2026-08-12 - Thermal-fluid mechanical engineering research workflow for literature review, technical writing, data analysis, presentations, proposals, coding, and AI/ML tools.
* [claude-math](https://github.com/vladimirrott/claude-math) ⭐ 13 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-12 - Emit mathematics as copy- and search-safe inline Unicode (∑, ≤, ℝ, x², matrices, set-builder) instead of LaTeX so equations stay legible in the Codex TUI, terminals, and Claude Code.
* [Data Product Builder for dbt](https://github.com/entropy-data/dataproduct-builder-dbt) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-05-28 - Full data-product lifecycle on dbt for Entropy Data: scaffold, audit, and integrate projects with ODCS, ODPS, OpenLineage, and GitHub Actions.
* [Codex Mem](https://github.com/2kDarki/codex-mem) ⭐ 10 | 🐛 0 | 🌐 TypeScript | 📅 2026-03-23 - Automatically capture, compress, and inject session context back into future Codex sessions.
* [Context Pack](https://github.com/Rothschildiuk/context-pack) ⭐ 10 | 🐛 0 | 🌐 Rust | 📅 2026-03-19 - Generate compact first-pass repository briefings for coding agents before deeper exploration.
* [sitemd](https://github.com/sitemd-cc/sitemd) ⭐ 9 | 🐛 2 | 🌐 HTML | 📅 2026-06-25 - Build websites from Markdown via MCP — 22 tools for creating pages, generating content, validating, running SEO audits, configuring settings, and deploying static sites to Cloudflare Pages.
* [Val Town](https://github.com/val-town/plugins) ⭐ 9 | 🐛 6 | 🌐 JavaScript | 📅 2026-08-12 - Build and deploy serverless TypeScript on Val Town from Codex — hosted MCP server plus skills for HTTP vals, cron, SQLite, email, OAuth, and React UI.
* [WakeWire](https://github.com/glenncalleja/wakewire) ⭐ 9 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-03 - Push events from GitHub, Gmail, Slack, and any signed webhook (Linear, Sentry, ClickUp) straight into your Codex threads as new turns — event-driven triggers instead of polling, with HMAC verification, deduplication, and a durable delivery queue.
* [Codex Be Serious](https://github.com/lulucatdev/codex-be-serious) ⭐ 7 | 🐛 0 | 🌐 Shell | 📅 2026-06-01 - Enforce formal, textbook-grade written register across all agent output.
* [Codex SEO](https://github.com/BestLemoon/codex-seo) ⭐ 7 | 🐛 8 | 🌐 Python | 📅 2026-07-03 - Full-stack SEO audits, Google API workflows, backlinks analysis, reporting, and optional MCP extensions for Codex.
* [Rust Reverse Engineering](https://github.com/jingjing2222/rust-reverse-engineering-skill) ⭐ 6 | 🐛 0 | 🌐 Shell | 📅 2026-04-18 - Reverse engineer Rust binaries and libraries: triage targets, demangle symbols, recover crate namespaces, and map panic, unwind, async, and FFI paths.
* [Upwork Autopilot](https://github.com/klajdikkolaj/upwork-autopilot) ⭐ 6 | 🐛 4 | 🌐 JavaScript | 📅 2026-07-03 - Controlled Upwork job search, qualification, and proposal submission sessions through a dedicated Chrome profile.
* [Apple Productivity](https://github.com/matk0shub/apple-productivity-mcp) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2026-03-27 - Local Apple Calendar and Reminders tooling for macOS with Codex plugin adapters.
* [AutoCAD Tianzheng Tools](https://github.com/summer521521/AutoCAD_Tianzheng_plugin) ⭐ 5 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to AutoCAD and Tianzheng HVAC through a local MCP server for DWG-aware HVAC drawing inspection and workflow automation.
* [Dodo Payments](https://github.com/dodopayments/dodo-agent-plugin) ⭐ 5 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-10 - Payments integration for checkouts, subscriptions, and billing with live API and documentation MCP servers with browser OAuth.
* [SysKnife](https://github.com/lacs-project/sysknife) ⭐ 5 | 🐛 3 | 🌐 Rust | 📅 2026-08-13 - Linux sysadmin co-pilot as an MCP server for Codex: plain-language requests become typed, risk-classified actions that a privileged daemon runs only after out-of-band terminal approval, with an Ed25519-signed audit chain and automatic rollback.
* [Chrome DevTools](https://github.com/win4r/chrome-devtools-codex-plugin) ⭐ 4 | 🐛 0 | 📅 2026-03-27 - One-click Codex plugin wrapper for chrome-devtools-mcp.
* [PapersFlow](https://github.com/papersflow-ai/papersflow-codex-plugin) ⭐ 4 | 🐛 3 | 🌐 JavaScript | 📅 2026-07-04 - Paper discovery, citation verification, graph exploration, and DeepScan analysis.
* [Remotion Plugin](https://github.com/tim-osterhus/codex-remotion-plugin) ⭐ 4 | 🐛 0 | 📅 2026-04-03 - Build parameterized Remotion videos in Codex with the official Remotion docs MCP, composition scaffolding, and a data-driven launch-video workflow.
* [Synta MCP](https://github.com/Synta-ai/n8n-mcp-codex-plugin-synta) ⭐ 4 | 🐛 0 | 📅 2026-04-03 - Build, edit, validate, and self-heal n8n workflows with Synta MCP tools and Codex-ready workflow guidance.
* [Task Scheduler](https://github.com/6Delta9/task-scheduler-codex-plugin) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-04-03 - OpenAI Codex plugin and local MCP server for turning task lists into realistic schedules with blocked dates, capacity overrides, overflow tracking, and markdown planning output.
* [Unified AI System](https://github.com/happy520ai/unified-ai-system) ⭐ 4 | 🐛 7 | 🌐 JavaScript | 📅 2026-08-13 - Self-hosted AI gateway for Codex with provider-free prompt enhancement, nine governed MCP tools, and a credential-free Docker path.
* [Agent Vision](https://github.com/zfifteen/agent-vision) ⭐ 3 | 🐛 0 | 🌐 Shell | 📅 2026-07-14 - macOS-only local camera plugin for explicit snapshots, streaming controls, and file-backed image input.
* [Antigravity 2.0](https://github.com/comprono/antigravity-2-codex-plugin) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-07 - Local Codex bridge for Antigravity desktop with setup checks, model limit summaries, DevTools UI automation, and safe project/chat handoff.
* [AxonFlow](https://github.com/getaxonflow/axonflow-codex-plugin) ⭐ 2 | 🐛 3 | 🌐 Shell | 📅 2026-08-03 - Runtime governance for Codex with policy enforcement on terminal commands, advisory checks for non-terminal tools via skills, PII/secret detection, and compliance-grade audit trails. Self-hosted via Docker.
* [Canvas Apps Plugin Codex](https://github.com/Ratnam-Mishra/canvas-apps-plugin-codex) ⭐ 2 | 🐛 1 | 📅 2026-05-03 - Build and edit Microsoft Power Apps Canvas Apps using natural language and Canvas Authoring MCP server.
* [Feishu to Codex](https://github.com/zlsbksdxl/codex-lark) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-10 - Connect Codex to Feishu/Lark workflows for Docs, Messenger, Drive, Sheets, Base, Calendar, Tasks, Meetings, Mail, approvals, and more through the official Lark CLI.
* [OrgX](https://github.com/useorgx/orgx-codex-plugin) ⭐ 2 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-05 - MCP access and initiative-aware skills for organizational workflows.
* [Read Image](https://github.com/ZXY1240/read-image) ⭐ 2 | 🐛 5 | 🌐 Python | 📅 2026-08-10 - Read local images, videos, web pages, and Windows screenshots through Doubao, GLM, or Qwen-compatible vision APIs.
* [Shots](https://github.com/hitSlop/shots) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-08-10 - Agent-native App Store screenshot, app icon, ASO, and localization workflows through the hosted Shots MCP server.
* [Zotero Research Tools](https://github.com/summer521521/Zotero_Research_plugin) ⭐ 2 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to Zotero Desktop for local-library search, citation export, collection and tag inspection, and research workflow support.
* [Agentgram](https://github.com/jerryfane/agentgram) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-07-28 - Send explicit Telegram messages from Codex and local AI agents through a Telegram bot token and chat id.
* [AgentGuards](https://github.com/alelaguard/agentguards-plugins) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-13 - LLM security guardrails for Codex with enforcing hooks and MCP tools: jailbreak and prompt-injection detection, web-content scanning, data-exfiltration blocking, and destructive-command authorization.
* [CONTAM Tools](https://github.com/summer521521/CONTAM_plugin) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-01 - Runs and inspects CONTAM airflow projects through a local MCP server with project guards, diagnostics, simulation helpers, and bridge workflows.
* [Exa Web Search](https://github.com/zlsbksdxl/codex-exa) ⭐ 1 | 🐛 1 | 🌐 Shell | 📅 2026-07-22 - Search and fetch current web sources in Codex through the official Exa MCP server with browser OAuth.
* [Maestro: Costguard](https://github.com/mbanderas/costguard) ⭐ 1 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-13 - Cost auditor for Codex that flags CI/cron and cloud-spend waste via read-only provider checks, then previews and applies surgical CI workflow fixes locally without writing to provider accounts or pushing git.
* [MATLAB Simulink Tools](https://github.com/summer521521/MATLAB_Simulink_plugin) ⭐ 1 | 🐛 0 | 🌐 MATLAB | 📅 2026-07-01 - Connects Codex to MATLAB and Simulink through a local MCP server for model inspection, script execution, and engineering workflow automation.
* [Nullcost](https://github.com/johnvouros/nullcost-plugin) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-12 - Catalog-backed free-tier, free-trial, and cheap developer-tool recommendations for Codex through bundled skills and MCP tools.
* [Ophis](https://github.com/ophis-fi/skills) ⭐ 1 | 🐛 2 | 📅 2026-07-24 - Onchain token swaps for Codex via the hosted Ophis MCP server, MEV-protected and gasless, built on CoW Protocol.
* [Aient](https://github.com/aient-ai/aient-codex-plugin) ⭐ 0 | 🐛 0 | 📅 2026-06-02 - AI operations plugin for Codex that connects production telemetry, problem lifecycle context, and remediation workflows through Aient's MCP server.
* [CarsXE](https://github.com/carsxe/carsxe-codex-plugin) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-23 - Decode VINs, license plates, market value, vehicle history, recalls, liens, OBD codes, and more via the CarsXE API.
* [Computer Usage Summary](https://github.com/liuyewang/computer-usage-summary-skill) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-03 - Privacy-first, local ActivityWatch reports for app time, AFK time, projects, billable work, and redacted timelines across macOS, Windows, and Linux.
* [Coolify](https://github.com/Sevi-py/coolify-codex-plugin) ⭐ 0 | 🐛 3 | 🌐 JavaScript | 📅 2026-07-24 - Control Coolify Cloud and self-hosted Coolify instances through API-aware workflow skills and local tools.
* [Droplinked](https://github.com/droplinked/droplinked-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-05 - Verified-inventory agentic commerce over a hosted MCP server, with merchant and product discovery, agent-initiated checkout, and onchain brand, credit-risk, and repayment attestations.
* [GH Project](https://github.com/zfifteen/gh-project-plugin) ⭐ 0 | 🐛 0 | 🌐 HTML | 📅 2026-05-15 - Create GitHub repositories from Codex with inferred defaults, native menus, explicit confirmation, and deterministic local cloning.
* [Lacuna Music](https://github.com/JOYLINK-LTD/lacuna-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-09 - Generate original instrumental music and vocal songs from Codex through the Lacuna MCP server.
* [Launch Fast](https://github.com/BlockchainHB/launchfast_codex_plugin) ⭐ 0 | 🐛 0 | 📅 2026-03-27 - Official Launch Fast plugin adapter for rapid SaaS deployment.
* [Mobazha](https://github.com/mobazha/mobazha-skills) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-05-03 - Decentralized e-commerce skills — deploy self-hosted stores, import products from Shopify/Amazon, configure custom domains and Telegram bots, set up Tor privacy, and manage your store via MCP.
* [OpenProject Codex](https://github.com/varaprasadreddy9676/openproject-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-16 - OpenProject integration for Codex with project, team, work package, bulk workflow, boards, wiki, meeting, attachment, and reporting support.
* [plori](https://github.com/plori-ai/codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-11 - Create and drive plori cloud agents (each an AI agent on its own cloud computer) over plori's remote MCP server, with OAuth auto-discovery.
* [SolidWorks GPT Plugin](https://github.com/Erfouni/solidworks-GPT-plugin) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-08-02 - Knowledge-backed SolidWorks design and validation workflows for Codex with standards lookup, CAD evidence gates, and consent-based session learning.
* [Storyflo](https://github.com/droplinked/storyflo-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-03 - Agentic newsroom over a hosted MCP server with narrated briefings, a news-versus-prediction-market Divergence Index, and a searchable declassified archive.
* [Token Harbor](https://github.com/NickHOI/Token-Harbor) ⭐ 0 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-12 - Turn Codex token usage into Sail Power for a local-first fishing, fleet, and harbor-building companion game.
* [TokRepo Search](https://github.com/henu-wang/tokrepo-codex-plugin) ⭐ 0 | 🐛 0 | 📅 2026-04-02 - Search and install AI assets from TokRepo with a bundled skill and MCP server for Codex.
* [VidSeeds.ai](https://github.com/CarrotGamesStudios/vidseeds-mcp) ⭐ 0 | 🐛 0 | 📅 2026-07-20 - Hosted MCP connector for pre-upload video SEO, metadata optimization, AI thumbnails, and multi-platform publishing with workflow skills for Codex agents.
* [Mantis](./plugins/deonmenezes/mantishack) - Autonomous bug bounty hunter for authorized engagements — 7-phase FSM (RECON → AUTH → HUNT → CHAIN → VERIFY → GRADE → REPORT), parallel hunter sub-agents, cryptographic scope enforcement, and BLAKE3/Ed25519 Merkle event logs.
* [PDF Monster](https://github.com/jbaehova/pdf-monster) - Analyzes PDFs as extracted text, OCR text, rendered page images, and embedded figures for coding agents.
* [SEO Dungeon](https://github.com/avalonreset/seo-dungeon) - Gamified local SEO audits that turn website issues into 16-bit dungeon battles for Codex, Claude, and Gemini CLI workflows.

## Formats & Development

AI extensions use several overlapping formats. Agent Skills provide reusable instructions, MCP servers expose tools and data, and client-specific plugin manifests package those capabilities for installation. Prefer open formats where practical, then add client adapters for the assistants you support.

### Getting Started

* [Official Docs: Agent Skills](https://developers.openai.com/codex/skills) - The skill authoring format.
* [Official Docs: Build Plugins](https://developers.openai.com/codex/plugins/build) - Author and package plugins.
* [Plugin Structure](https://developers.openai.com/codex/plugins/build#create-a-plugin-manually) - `.codex-plugin/plugin.json` manifest format.

### Codex-Compatible Plugin Anatomy

```
my-plugin/
├── .codex-plugin/
│   └── plugin.json          # Required: name, version, description, skills path
├── skills/
│   └── my-skill/
│       ├── SKILL.md          # Required: skill instructions + metadata
│       ├── scripts/          # Optional: executable scripts
│       └── references/       # Optional: docs and templates
├── apps/                     # Optional: app integrations
└── mcp.json                  # Optional: MCP server configuration
```

### Codex Plugin Creator

Use the built-in skill to scaffold a new plugin:

```
$plugin-creator
```

### Publishing

Distribution varies by client. Most projects publish from a GitHub repository; compatible Codex bundles can also use local marketplaces (`~/.agents/plugins/marketplace.json`) or repo marketplaces (`$REPO_ROOT/.agents/plugins/marketplace.json`). Follow each target client's current packaging and installation documentation.

For this curated list, the README is the editorial source of truth. Generated JSON files provide compatibility exports for registry and automation consumers; they are not a promise that every entry can be installed directly from this repository.

## Validate Before You Ship

After scaffolding with `$plugin-creator`, use [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 433 | 🐛 29 | 🌐 Python | 📅 2026-08-13 as your quality gate before publishing, review, or distribution.

For skill/plugin authoring workflows, [Codex SkillForge](https://github.com/f0d010c/skillforge) ⭐ 0 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-09 provides an ESLint-style CLI and GitHub Action for scaffolding, linting, smoke-testing, and packaging Codex skills/plugins before publishing.

### Local Preflight

```bash
pipx run plugin-scanner lint .
pipx run plugin-scanner verify .
```

### PR Gate (GitHub Actions)

```yaml
- uses: hashgraph-online/ai-plugin-scanner-action@v1
  with:
    plugin_dir: "."
    fail_on_severity: high
```

### Submission Preflight

Use scanner outputs as evidence for maintainers/reviewers:

* Structural lint results
* Publish-readiness verification output
* SARIF/findings for CI and code scanning

The score is best used as a quick trust signal and triage summary (not the only readiness signal).

## Guides & Articles

* [Codex Plugins, Visually Explained](https://adithyan.io/blog/codex-plugins-visual-explainer) - Visual walkthrough by @adithyan.
* [Codex Plugins: Slack, Figma, Google Drive](https://arstechnica.com/ai/2026/03/openai-brings-plugins-to-codex-closing-some-of-the-gap-with-claude-code/) - Ars Technica feature deep dive.
* [Codex v0.117.0 Plugin Walkthrough](https://reddit.com/r/codex/) - Reddit explainer.
* [OpenAI's Codex Gets Plugins](https://thenewstack.io/openais-codex-gets-plugins/) - The New Stack ecosystem overview.

## Related Projects

* [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) ⭐ 800 | 🐛 19 | 🌐 Python | 📅 2026-08-10 - Codex-focused catalog that inspired this cross-platform list.
* [HOL Plugin Registry](https://hol.org/registry/plugins) - Browse plugins with scanner-backed security analysis and trust scores.

## Claim Your Plugin

Verify ownership of your plugin on the [HOL Plugin Registry](https://hol.org/registry/plugins) to display a verified badge on your listing.

### How to claim

1. Go to [hol.org/guard/plugins](https://hol.org/guard/plugins) and sign in with GitHub
2. Find your plugin in the list and click **Verify Ownership**
3. Authorize the read-only GitHub connection (view your profile, email, and public org membership — no write access)
4. Once verified, your plugin listing will display a **Verified** badge

That's it. The verification confirms you are the repository owner or an organization admin. Plugins owned by organizations may require additional review.

> **Note:** You only need to verify once per plugin. If your verification needs to be reset, contact support at `support@hol.org`.

## Plugin Trust Scores

Every plugin in this list is automatically ingested by the [HOL Plugin Registry](https://hol.org/registry/plugins), which runs each through the [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 433 | 🐛 29 | 🌐 Python | 📅 2026-08-13 to produce a trust score and security analysis.

Each plugin gets a detailed breakdown across six factors:

* **Installability** - Can the plugin be installed and run without errors?
* **Maintenance** - Is the repo actively maintained with clear documentation?
* **MCP Posture** - How securely are MCP servers configured?
* **Plugin Security** - Does the manifest follow security best practices?
* **Provenance** - Can the publisher's identity be verified?
* **Publisher Quality** - Does the publisher have a track record of quality releases?

You can embed a trust badge in your plugin's README:

```
[![Plugin Name on HOL Registry (Trust Score)](https://img.shields.io/endpoint?url=https%3A%2F%2Fhol.org%2Fapi%2Fregistry%2Fbadges%2Fplugin%3Fslug%3DOWNER%252FREPO%26metric%3Dtrust%26style%3Dfor-the-badge%26label%3DPlugin+Name)](https://hol.org/registry/plugins/OWNER%2FREPO)
```

Replace `OWNER%2FREPO` with your plugin's GitHub owner and repo name (URL-encoded slash). Metrics available: `trust`, `security`. Styles: `flat`, `flat-square`, `plastic`, `for-the-badge`, `social`.

### HOL Guard Protection Badge

Show that your plugin repo is protected by [HOL Guard](https://hol.org/guard):

```
[![HOL Guard](https://img.shields.io/endpoint?url=https%3A%2F%2Fhol.org%2Fapi%2Fregistry%2Fbadges%2Fguard%2FOWNER%2FREPO%3Fstyle%3Dflat-square)](https://hol.org/guard)
```

The badge checks your repo for HOL Guard adoption (config files, CI workflows, dependencies) and displays `Protected` (green) or `Unprotected` (grey). To get the badge:

1. Install HOL Guard: `pipx install hol-guard && hol-guard init`
2. Or add the scanner to CI: `uses: hashgraph-online/ai-plugin-scanner-action@v1`
3. Add the badge markdown to your README (replace `OWNER%2FREPO`)

## Plugin Quality

If you received a scanner report on your repo, check the [Scanner Guide](SCANNER_GUIDE.md) for setup instructions, common fixes, and CI setup.

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

To add a plugin:

1. Set up the HOL Plugin Scanner in your plugin repo (see [CONTRIBUTING.md](CONTRIBUTING.md))
2. Fork this repo and add a single line to the appropriate section in `README.md` (alphabetical order)
3. Submit a PR with your scanner score and plugin repo URL

**You do not need to copy plugin files into this repo.** A generator fetches your bundle from your source repo and regenerates catalog files automatically.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-13._
