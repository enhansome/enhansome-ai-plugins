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
  Discover extensions for Codex, ChatGPT, Claude Code, Gemini CLI, Grok, Kimi, DeepSeek Harness, Cursor, OpenCode, and other compatible AI assistants from one community-maintained catalog.
</p>

<p align="center">
  Listings may target one assistant, several assistants, or open standards such as Agent Skills and MCP. Check each project for its supported clients and installation instructions.
</p>

<br>

## Contents

* [Start Here](#start-here)
* [Official Plugins](#official-plugins)
* [Community Plugins](#community-plugins)
  * [Grok Plugins](#grok-plugins)
  * [Kimi Plugins](#kimi-plugins)
  * [DeepSeek Harness Plugins](#deepseek-harness-plugins)
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

1. **Validate with [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 510 | 🐛 43 | 🌐 Python | 📅 2026-08-31** — recommended local preflight
2. **Add the [HOL scanner GitHub Action](https://github.com/hashgraph-online/ai-plugin-scanner-action) ⭐ 4 | 🐛 1 | 📅 2026-08-31** — recommended for security, optional for listing
3. Choose the clients and open formats you support
4. Build the plugin, skill, MCP server, app, or agent tool
5. Ship or submit with confidence

### Quick preflight

```bash
pipx run plugin-scanner lint .
pipx run plugin-scanner verify .
```

### Scanner CI (recommended for security)

Scanner CI is optional for listing. HOL still scans listed projects independently. We recommend including it so MCP servers, skills, plugins, and other agent extensions stay continuously checked — that is how this catalog stays safer for everyone who installs from it. Projects that maintain scanner CI receive the full trust score; projects without it remain eligible and receive a 10% trust-score reduction.

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

* [Claude Code Skills](https://github.com/alirezarezvani/claude-skills) ⭐ 25,309 | 🐛 10 | 🌐 Python | 📅 2026-08-30 - 223 production-ready skills, 23 agents, and 298 Python tools across 9 domains — engineering, marketing, product, compliance, and more.
* [Generative Media Skills](https://github.com/SamurAIGPT/Generative-Media-Skills) ⭐ 4,196 | 🐛 3 | 🌐 Shell | 📅 2026-08-27 - 13 skills for image, video, and audio generation using 100+ models - FLUX, Midjourney v7, Veo3, Kling 3.0, Suno, and HunyuanVideo via muapi.ai.
* [Claude Octopus](https://github.com/nyldn/claude-octopus) ⭐ 4,024 | 🐛 12 | 🌐 Shell | 📅 2026-08-31 - Multi-LLM orchestration dispatching to 8 providers (Codex, Gemini, Copilot, Qwen, Perplexity, OpenRouter, Ollama, OpenCode) with Double Diamond workflows, adversarial review, and safety gates.
* [AI Video Transcriber](https://github.com/wendy7756/AI-Video-Transcriber) ⭐ 3,241 | 🐛 10 | 🌐 Python | 📅 2026-08-23 - Transcribe and summarize videos, podcasts, and local media via a Codex plugin, Claude Code skill, and MCP server.
* [MegaLinter](https://github.com/oxsecurity/megalinter) ⭐ 2,573 | 🐛 41 | 🌐 Dockerfile | 📅 2026-08-31 - Set up, run and fix MegaLinter on any repository, covering 100+ linters and formatters for 69+ languages and 23+ formats, in CI or locally, with per-linter fix guides for the agent.
* [Better Harness](https://github.com/QoderAI/better-harness) ⭐ 2,073 | 🐛 7 | 🌐 JavaScript | 📅 2026-08-31 - Evidence-backed workflow analysis for coding agents that turns project and session signals into prioritized, verifiable improvements across supported hosts.
* [Brooks Lint](https://github.com/hyhmrright/brooks-lint) ⭐ 1,439 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-31 - AI code reviews grounded in six classic engineering books — decay risk diagnostics with book citations, severity labels, and four analysis modes (PR review, architecture audit, tech debt, test quality).
* [Antigravity Workspace Template](https://github.com/study8677/antigravity-workspace-template) ⭐ 1,321 | 🐛 3 | 🌐 Python | 📅 2026-08-28 - Multi-agent codebase knowledge graph generator with context-aware planning and automatic scope management — turns codebases into coherent agent workspaces.
* [Aegis](https://github.com/GanyuanRan/Aegis) ⭐ 1,155 | 🐛 3 | 🌐 Python | 📅 2026-08-31 - An agentic skills framework & software development methodology that works: planning, TDD, debugging, and collaboration workflows.
* [spec-superflow](https://github.com/MageByte-Zero/spec-superflow) ⭐ 780 | 🐛 7 | 🌐 JavaScript | 📅 2026-08-29 - Spec-first workflow with nine skills, user-controlled Quick / Hotfix / Tweak / Full paths, auditable recovery commands, hardened delta-spec sync, and guarded review gates.
* [Boss](https://github.com/echoVic/boss-skill) ⭐ 552 | 🐛 14 | 🌐 TypeScript | 📅 2026-08-30 - BMAD pipeline plugin that orchestrates a full requirements-to-deploy workflow across nine specialist agents with an auditable runtime DAG and quality gates, for Claude Code, Codex, OpenClaw, and Antigravity.
* [token-optimizer](https://github.com/ooples/token-optimizer-mcp) ⭐ 502 | 🐛 5 | 🌐 JavaScript | 📅 2026-08-31 - Spend less context and keep the conclusions across 16 coding clients including Claude Code, Codex, Gemini CLI, Cursor, and Copilot — diff-only re-reads, paths-only search, out-of-context stashing, and a local ledger that measures each tool's actual return.
* [Codex Multi Auth](https://github.com/ndycode/codex-multi-auth) ⭐ 467 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-31 - Multi-account OAuth manager for the official Codex CLI with switching, health checks, and recovery tools.
* [AgentOps](https://github.com/boshu2/agentops) ⭐ 432 | 🐛 1 | 🌐 Shell | 📅 2026-08-28 - DevOps layer for coding agents with flow, feedback, and memory that compounds between sessions.
* [Audio Plugin Coder](https://github.com/Noizefield/audio-plugin-coder) ⭐ 313 | 🐛 0 | 🌐 C++ | 📅 2026-08-25 - Agent-agnostic JUCE workflow for building VST3/AU plugins from idea through design, implementation, test, and installer packaging.
* [Reviewable HTML Workbench](https://github.com/u-ichi/reviewable-html-workbench) ⭐ 294 | 🐛 3 | 🌐 Python | 📅 2026-08-09 - Generate reviewable HTML documents, serve previews, collect inline review comments, and feed review outcomes back into agent workflows.
* [Ditto](https://github.com/ohad6k/ditto) ⭐ 280 | 🐛 21 | 🌐 Python | 📅 2026-08-24 - Mines selected evidence from local coding-agent sessions into private work, design, and writing profiles for Codex, Claude Code, and GitHub Copilot.
* [OpenCode Orchestrator](https://github.com/agnusdei1207/opencode-orchestrator) ⭐ 232 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-24 - Multi-agent mission control for OpenCode with Commander, Planner, Worker, and Reviewer workflows.
* [Claude Code for Codex](https://github.com/sendbird/cc-plugin-codex) ⭐ 183 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-31 - Reverse of OpenAI's official Claude-hosted plugin: use Claude Code from Codex for reviews, rescue tasks, tracked background jobs, and hook-powered review gates.
* [agent-talk](https://github.com/xhluca/agent-talk) ⭐ 178 | 🐛 2 | 🌐 Python | 📅 2026-08-24 - Skills-based plugin built on the retalk CLI that gives coding agents end-to-end encrypted messaging with other agents, including agents run by other people, across Claude Code, Codex, Antigravity, pi, opencode, and GitHub Copilot CLI.
* [claude-remember](https://github.com/Digital-Process-Tools/claude-remember) ⭐ 163 | 🐛 10 | 🌐 Python | 📅 2026-08-29 - Persistent memory for Claude Code with identity, context, and continuity carried across sessions.
* [Suede Creator Skills](https://github.com/JasonColapietro/suede-creator-skills) ⭐ 129 | 🐛 6 | 🌐 JavaScript | 📅 2026-08-31 - An open-source Agent Skills pack for Claude Code and Codex covering multi-agent workflows, code review, design, copy, SEO, app shipping, creator-rights workflows, and local read-only MCP discovery.
* [Krypton](https://github.com/jturntdev/krypton) ⭐ 128 | 🐛 2 | 🌐 Shell | 📅 2026-07-24 - Goal-based planning and proof gate for Codex and Claude Code that turns requests into ownership, cutover, review-gate, and acceptance-evidence plans.
* [Superloopy](https://github.com/beefiker/superloopy) ⭐ 108 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-25 - Evidence-gated Codex loop harness with specialist skills, including near-pixel authorized website cloning backed by screenshots, assets, build output, and visual QA.
* [trace-mcp](https://github.com/nikolai-vysotskyi/trace-mcp) ⭐ 102 | 🐛 7 | 🌐 TypeScript | 📅 2026-08-31 - Precomputed code-intelligence graph served over MCP — symbol search, call graphs, change impact, and test mapping as structured answers instead of whole-file reads.
* [Coordinate Agents](https://github.com/hogancv/coordinate-agents) ⭐ 101 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-31 - Plugin-first multi-agent coordination tool with a local-first, recoverable Agent Bus and human-gated planning, implementation, review, and release workflows.
* [2718lab DevKit](https://github.com/2718labs/2718lab-devkit) ⭐ 99 | 🐛 2 | 🌐 Python | 📅 2026-08-31 - Codex-first local MCP server and skill bundle for deterministic project intelligence, durable workflow orchestration, and reusable engineering tools.
* [Sealos](https://github.com/labring/sealos-skills) ⭐ 78 | 🐛 6 | 🌐 Python | 📅 2026-08-14 - Deploy apps to Sealos Cloud from Codex with readiness checks, Dockerfile generation, Compose conversion, image builds, and rollout updates.
* [Globalping](https://github.com/jsdelivr/globalping-mcp-server) ⭐ 63 | 🐛 4 | 🌐 TypeScript | 📅 2026-08-31 - Access thousands of probes around the world to run network tests such as ping, traceroute, http, dns and mtr.
* [claude-image-gen](https://github.com/guinacio/claude-image-gen) ⭐ 60 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-22 - AI-powered image generation using Google Gemini or OpenAI (gpt-image-2), integrated with Claude Code via Skills or Claude.ai via MCP.
* [skillsaw](https://github.com/stbenjam/skillsaw) ⭐ 59 | 🐛 6 | 🌐 Python | 📅 2026-08-31 - A configurable linter for agent skills, plugins, and AI coding assistant context.
* [Archcore](https://github.com/archcore-ai/plugin) ⭐ 53 | 🐛 15 | 🌐 Shell | 📅 2026-08-17 - Gives coding agents the architecture, rules, and prior decisions of the repo via skills, hooks, and MCP — so new changes land where the project says they belong across Claude Code, Cursor, and Codex CLI.
* [pstack for Codex](https://github.com/Aqua-123/pstack-for-codex) ⭐ 53 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-31 - Codex-native engineering workflows derived from pstack, with 45 explicit skills and 23 Poteto Mode playbooks.
* [Honcho](https://github.com/plastic-labs/codex-honcho) ⭐ 51 | 🐛 9 | 🌐 TypeScript | 📅 2026-07-16 - Persistent cross-session memory for Codex powered by Honcho — lifecycle hooks capture each session and inject relevant context back at session start, so Codex remembers your preferences, projects, and decisions across restarts.
* [mcp-local-memory](https://github.com/Beledarian/mcp-local-memory) ⭐ 51 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-26 - A lightweight, powerful local memory server for AI agents supporting text, entities, relations, and time-based recall.
* [Session Orchestrator](https://github.com/Kanevry/session-orchestrator) ⭐ 49 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-28 - Session orchestration for Claude Code, Codex, and Cursor IDE — structured planning, wave-based execution, VCS integration (GitLab + GitHub), quality gates, and clean session close-out with issue tracking.
* [Rootly MCP Server](https://github.com/rootlyhq/rootly-mcp-server) ⭐ 45 | 🐛 8 | 🌐 Python | 📅 2026-08-31 - Manage and resolve production incidents from MCP-compatible AI assistants through dynamically generated, access-controlled Rootly API tools.
* [Docflow](https://github.com/MedAdemBHA/docflow) ⭐ 41 | 🐛 0 | 🌐 Shell | 📅 2026-08-15 - Lightweight documentation memory for AI coding agents that scaffolds a 7-category docs tree, runs readiness checks, validates docs before finishing, and keeps a monthly changelog across Claude Code and Codex.
* [memi](https://github.com/sarveshsea/memi) ⭐ 40 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-08 - Interface understanding and design-system memory for Codex, Claude Code, Cursor, and MCP agents with UI audits, Tailwind token extraction, shadcn registry workflows, and a bundled Codex plugin.
* [Waggle](https://github.com/Abhigyan-Shekhar/Waggle-mcp) ⭐ 39 | 🐛 210 | 🌐 Python | 📅 2026-08-31 - Persistent graph-backed conversational memory for Codex that recalls project decisions, constraints, preferences, and outcomes across sessions.
* [Codebase Recon](https://github.com/yujiachen-y/codebase-recon-skill) ⭐ 36 | 🐛 0 | 📅 2026-04-26 - Analyze git history to understand a codebase before reading any code — auto-scales by repo size and cross-references hotspots with bug magnets to surface high-risk files, bus factor, and team momentum.
* [iris-agentic-dev](https://github.com/intersystems-community/iris-agentic-dev) ⭐ 35 | 🐛 6 | 🌐 Rust | 📅 2026-08-30 - MCP server giving AI assistants live access to InterSystems IRIS — execute ObjectScript, query globals, inspect productions, run tests, search code, and manage skills.
* [Labtasker](https://github.com/luocfprime/labtasker) ⭐ 34 | 🐛 1 | 🌐 Python | 📅 2026-08-28 - Queue and run independent ML inference, evaluation, and experiment tasks across long-lived Python or command workers with a Claude Code plugin and cross-agent skill.
* [Open Dynamic Workflows](https://github.com/Suraj1235/open-dynamic-workflows) ⭐ 33 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-09 - Local-first MIT dynamic multi-agent workflows for Codex, OpenCode, Antigravity, Cursor, and VS Code with a daemon, MCP bridge, Codex skills, OpenCode plugin, and bring-your-own-model support.
* [Velith](https://github.com/epicsagas/Velith) ⭐ 33 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-09 - AI-native publishing system with a 6-phase pipeline from ideation to EPUB/PDF across 8 genres.
* [Dely](https://github.com/hieuphung97/dely) ⭐ 32 | 🐛 2 | 🌐 Shell | 📅 2026-08-31 - Multi-harness control protocol that turns requests into approved design contracts, orchestrating isolated worker sessions for sequential implementation and independent code reviews under Orca supervision for Claude Code, Codex, Cursor, Antigravity, and other AI coding agents.
* [AI-Native SDLC](https://github.com/bashebr/ai-native-sdlc) ⭐ 31 | 🐛 0 | 🌐 Python | 📅 2026-08-29 - Reusable skill and plugin bundle implementing the AI-native SDLC workflow: plan, design, build, test, deploy, and maintain with human approval gates.
* [Designer Skill](https://github.com/Pythoughts-labs/designer-skill) ⭐ 29 | 🐛 12 | 🌐 JavaScript | 📅 2026-08-30 - Plug-and-play MCP that gives your agent UI superpowers. One install: design skill + MCP server, zero config.
* [Hera Agent Unity](https://github.com/NotNull92/hera-agent-unity) ⭐ 28 | 🐛 0 | 🌐 C# | 📅 2026-08-19 - Controls and verifies a live Unity Editor through a low-token CLI, with scene, asset, Inspector, Play Mode, test, screenshot, and runtime C# workflows for Codex and other coding agents.
* [harness-eval](https://github.com/redhat-community-ai-tools/harness-eval) ⭐ 27 | 🐛 4 | 🌐 Python | 📅 2026-08-27 - Linter tool (static analysis rules) and LLM reviewer for AI agent harness files that runs quality and security health checks, catching cross-component security chains, redundancy, and config drift, and vets individual skills before install, across Claude Code, Cursor, Codex, Copilot, Gemini, and OpenCode.
* [Knowl](https://github.com/dat999zx/knowl) ⭐ 27 | 🐛 6 | 🌐 TypeScript | 📅 2026-08-31 - Local-first project memory over MCP for Claude Code, Codex, Cursor and eight other hosts: a SQLite store that retires facts when they change, shares knowledge across linked repos, and retrieves it by hybrid search.
* [Vibe Prospecting](https://github.com/explorium-ai/vibeprospecting-plugin) ⭐ 27 | 🐛 3 | 🌐 Shell | 📅 2026-08-20 - Live B2B company and contact intelligence for building lead lists, researching prospects, enriching contacts, and personalizing outreach.
* [HOTL Plugin](https://github.com/yimwoo/hotl-plugin) ⭐ 26 | 🐛 0 | 🌐 Shell | 📅 2026-07-06 - Human-on-the-Loop AI coding workflow plugin for Codex, Claude Code, and Cline with structured planning, review, and verification guardrails.
* [Agent Guard](https://github.com/JeongJaeSoon/agent-guard) ⭐ 25 | 🐛 4 | 🌐 Shell | 📅 2026-08-31 - Real-time secret-leak guardrails for AI coding agents (Claude Code, Codex), Git hooks, and CI.
* [AgentPack](https://github.com/vishal2612200/agentpack) ⭐ 25 | 🐛 19 | 🌐 Python | 📅 2026-08-29 - Ranks repo context for Codex with likely files, skill recommendations, agent rules, commands, warnings, and compact task-focused packs before editing.
* [Stark](https://github.com/f0d010c/stark) ⭐ 25 | 🐛 0 | 🌐 Python | 📅 2026-07-26 - UI/UX design plugin for AI coding agents with product-flow routing, platform-native interface guidance, asset planning, and shipped-reference analysis before code.
* [VibePortrait](https://github.com/dadwadw233/VibePortrait) ⭐ 25 | 🐛 0 | 🌐 HTML | 📅 2026-04-08 - Developer personality portrait generator — analyzes AI conversation history to produce MBTI type (16 color themes), capability radar, developer rating, 3-dimension famous match, and a persona skill that lets any AI "think like you".
* [Quality Engineering Skills](https://github.com/RBraga01/Quality-Engineering-Skills) ⭐ 24 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-28 - 22 structured quality engineering skills for automotive and manufacturing: ISO 9001, IATF 16949, AIAG-VDA FMEA, VDA 6.3, PPAP, APQP, SPC, MSA.
* [Web Search MCP](https://github.com/sydasif/web-search-mcp) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-08-31 - Comprehensive FastMCP server giving LLMs real-time web access across search engines (DuckDuckGo, Exa), social platforms (Reddit, Hacker News, GitHub, X, LinkedIn), and academic tools (arXiv, Wikipedia), with SSRF-protected URL fetching.
* [Frappe Agent](https://github.com/Dkm0315/frappe-agent) ⭐ 23 | 🐛 2 | 📅 2026-08-30 - Frappe and ERPNext coding, customization, bench, and review intelligence for Codex.
* [RAG Reviewer](https://github.com/mimfort/rag_for_git) ⭐ 21 | 🐛 2 | 🌐 Python | 📅 2026-08-31 - Agentic PR review: hybrid RAG + code graph via MCP, review skills for Codex.
* [Supergraph](https://github.com/datit309/supergraph) ⭐ 21 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Engineering workflow system for AI coding agents that enforces planning, TDD, verification, review, and architecture-aware decisions with local codebase graph intelligence across Claude Code, Codex CLI, Antigravity, and OpenCode,..
* [Espresso](https://github.com/mirkobozzetto/espresso) ⭐ 19 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-08 - Full token-saving stack in one plugin - output compression, global rules, RTK hook, Caveman ultra, GitNexus config. Detects existing setup, installs only what's missing. Works on Claude Code and Codex.
* [SOTA Engineering Skills](https://github.com/martinholovsky/SOTA-skills) ⭐ 18 | 🐛 0 | 🌐 Python | 📅 2026-08-29 - Router-mapped library of 40 domain and language skills with BUILD and AUDIT modes, loading only the rules a task needs and ending every rules file in an audit checklist.
* [VASTlint](https://github.com/aleksUIX/vastlint) ⭐ 18 | 🐛 2 | 🌐 Rust | 📅 2026-08-31 - Validate VAST, VMAP, and DAAST ad tags against IAB Tech Lab specs via Gemini CLI, Claude Code, and a hosted MCP server.
* [Epic Harness](https://github.com/epicsagas/epic-harness) ⭐ 17 | 🐛 3 | 🌐 Rust | 📅 2026-08-31 - Auto-trigger quality skills + self-evolving agent harness — orbit (spec-to-ship), evolve (skill mutation), team (multi-agent), TDD, check, ship, simplify, debug, perf, secure.
* [Rel.AI MCP](https://github.com/Kyne0328/rel-ai-mcp) ⭐ 17 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-30 - Brings Codex-style coding workflows to ChatGPT Web, connecting it to local development workspaces through MCP while using ChatGPT Web quota instead of Codex quota.
* [aide](https://github.com/jmylchreest/aide) ⭐ 16 | 🐛 0 | 🌐 Go | 📅 2026-08-31 - Persistent memory, code intelligence, and multi-agent orchestration for Claude Code, OpenCode, and Codex CLI via skills, hooks, and an MCP server.
* [claude-supertool](https://github.com/Digital-Process-Tools/claude-supertool) ⭐ 16 | 🐛 113 | 🌐 Python | 📅 2026-08-29 - Batches file, git and tracker operations into one round-trip, collapsing many reads, greps and globs into a single call for fewer output tokens and less wall time.
* [coffee-paladin](https://github.com/pawelkwaczynski/coffee-paladin) ⭐ 16 | 🐛 1 | 🌐 Python | 📅 2026-08-29 - Thermal guard for Apple Silicon: pauses hot jobs before the Mac throttles and gates Claude Code, Codex and Gemini CLI before heavy commands.
* [ejentum-mcp](https://github.com/ejentum/ejentum-mcp) ⭐ 16 | 🐛 1 | 🌐 JavaScript | 📅 2026-06-11 - MCP server exposing reasoning, code, anti-deception, and memory harness tools for Codex.
* [Alcove](https://github.com/epicsagas/alcove) ⭐ 15 | 🐛 0 | 🌐 Rust | 📅 2026-08-19 - Local-first MCP server for private project docs with hybrid BM25+vector search, tree-sitter code indexing, and automated linting for team-wide documentation standards.
* [MeMesh](https://github.com/PCIRCLE-AI/memesh) ⭐ 15 | 🐛 47 | 🌐 TypeScript | 📅 2026-08-31 - Local SQLite memory shared by Claude Code, Codex, Gemini, Cursor, and other MCP clients, captured automatically by hooks from real work and injected at the moment the agent acts.
* [UIZZE](https://github.com/uizze/uizze) ⭐ 15 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-29 - STOP UI SLOP. Gives Codex 800,000+ real web and iOS screens, a product-specific design contract, and a hard finish gate before generic UI ships; connect it at <https://uizze.com>.
* [BGS Modding Superpowers](https://github.com/BB-84C/bgs-modding-superpowers) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2026-08-24 - Agentic Bethesda Game Studio modpack curation toolkit with MCP-driven xEdit conflict audit, MO2 control plane, BA2/BSA and Papyrus tooling, and skills for setup, dev-log, and release-changelog workflows.
* [Codex Reviewer](https://github.com/schuettc/codex-reviewer) ⭐ 14 | 🐛 0 | 📅 2026-05-05 - Second-pass review of Claude-driven plans and implementations.
* [Project Autopilot](https://github.com/AlexMi64/codex-project-autopilot) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2026-04-09 - Turn an idea into a structured project workflow with planning, execution, verification, and handoff.
* [trigger-tree](https://github.com/Hedde/trigger_tree) ⭐ 14 | 🐛 3 | 🌐 Python | 📅 2026-08-31 - Local documentation telemetry for Claude Code and Codex: see which docs your agent actually reads, gate discoverability in CI, and measure instruction adherence.
* [A Team](https://github.com/RBraga01/a-team) ⭐ 13 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-09 - Universal multi-agent infrastructure with 25 specialist agents, 16 enforced workflow skills, and a lead orchestrator for Claude Code, Codex CLI, Cursor, and OpenCode.
* [MARGINAL](https://github.com/SignalLayerLabs/Marginal) ⭐ 13 | 🐛 25 | 🌐 Python | 📅 2026-08-27 - Local-first runtime governor for AI coding agents that detects proven no-progress repetition, records decision evidence, starts in Shadow Mode, and earns narrow enforcement only after repository-local evidence.
* [NeatContext](https://github.com/XTSoftwareLabs/neatcontext-plugins) ⭐ 13 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-23 - Saves the durable knowledge from Claude Code, Codex, GitHub Copilot, Kimi Code, and pi conversations as structured, reusable contexts you can reconnect in later sessions or share with your team.
* [Staff Engineer Mode](https://github.com/sirmarkz/staff-engineer-mode) ⭐ 13 | 🐛 1 | 🌐 Python | 📅 2026-08-01 - Routes engineering design, delivery, reliability, security, operations, and maintenance prompts to focused staff-level specialist guidance for AI coding agents.
* [Codex Agenteam](https://github.com/yimwoo/codex-agenteam) ⭐ 12 | 🐛 0 | 🌐 Python | 📅 2026-07-06 - Specialist AI agents (researcher, PM, architect, developer, QA, reviewer) orchestrated as a configurable team pipeline.
* [SEO Skills AI](https://github.com/seoskillsai/seo-skills-ai) ⭐ 12 | 🐛 3 | 🌐 Python | 📅 2026-08-27 - Universal SEO skill suite and technical audit engine for Claude Code, Cursor, Codex, and other agents, with first-party Python adapters and HOL plugin-scanner CI.
* [Tool Advisor](https://github.com/dragon1086/claude-skills) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-04-23 - Read-only meta-skill that scans your MCP servers, skills, plugins, and CLI tools, then suggests up to three ranked approaches (Methodical / Fast / Deep) with a copy-paste Quick Action table.
* [Writer's Loop](https://github.com/xxsang/writers-loop) ⭐ 12 | 🐛 0 | 🌐 JavaScript | 📅 2026-05-09 - Structured AI writing workflow for planning, critique, revision, translation, style distillation, and opt-in local preference learning.
* [Agentic Ship](https://github.com/moasq/agentic-ship) ⭐ 11 | 🐛 9 | 🌐 JavaScript | 📅 2026-08-29 - Cross-host product-development toolkit for Claude Code, Codex, Cursor, Hermes, and OpenClaw with shared rules, specialist roles, service connections, and machine-checked UI, backend, security, and launch gates.
* [Claude Code Harness](https://github.com/dadwadw233/claude-code-harness) ⭐ 11 | 🐛 0 | 📅 2026-04-05 - Harness blueprint skill for turning vague agent ideas into concrete designs for request assembly, control loops, memory, permissions, recovery, and extension planes.
* [Claude Watchdog](https://github.com/Temikus/claude-watchdog) ⭐ 11 | 🐛 1 | 🌐 Shell | 📅 2026-08-30 - Stop hook that runs a critical post-mortem on every Claude Code session, cross-checking what was asked against the actual git diff for missed goals, wasted detours, and unverified claims.
* [Development Skills](https://github.com/reidemeister94/development-skills) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2026-07-24 - Three-tier triage (PASS\_THROUGH / LIGHT / FULL 4-phase) development workflow for Codex and Claude Code with language auto-detection (Python, Java, TypeScript, Swift, frontend) and a staff-reviewer subagent for fresh-eyes review on every change.
* [Hera Agent Godot](https://github.com/NotNull92/hera-agent-godot) ⭐ 11 | 🐛 0 | 🌐 Go | 📅 2026-07-29 - Drives a live Godot 4.x editor through the low-token Hera CLI — scene, node, and signal edits, play control, and runtime QA with verifiable compact JSON output, with the companion addon published on the official Godot Asset Store.
* [Casefile](https://github.com/x4cc3/casefile) ⚠️ Archived - Persistent security case tracking for bug bounties, CTFs, and security audits.
* [Clean Room](https://github.com/whit3rabbit/clean-room-skill) ⭐ 10 | 🐛 5 | 🌐 JavaScript | 📅 2026-08-26 - Spec-first clean-room workflow for authorized source analysis, behavioral specs, role separation, and verification without replacement code.
* [FlexViz](https://github.com/flex-analytics/flexviz) ⭐ 10 | 🐛 5 | 🌐 Python | 📅 2026-08-31 - Interactive cross-filter dashboards for large datasets with a Claude Code skill for agent-driven data exploration.
* [LoreConvo](https://github.com/labyrinth-analytics/loreconvo) ⭐ 10 | 🐛 1 | 🌐 Python | 📅 2026-08-28 - Persistent session memory MCP server for Claude — auto-saves and recalls conversation context, decisions, and artifacts across Claude Code, chat, and other surfaces with full-text search.
* [Spec-Driven Development](https://github.com/Habib0x0/spec-driven-plugin) ⭐ 10 | 🐛 0 | 🌐 Shell | 📅 2026-05-18 - Three-phase Requirements → Design → Tasks workflow for Claude Code and Codex — EARS notation acceptance criteria, autonomous execution loop, cross-spec dependencies, and post-implementation acceptance testing.
* [Agent Harness Skills](https://github.com/yfge/agent-harness-skills) ⭐ 9 | 🐛 2 | 🌐 Python | 📅 2026-07-14 - Designs agent-ready repository harnesses with entrypoints, validation surfaces, runtime evidence, delivery records, and atomic commit guidance.
* [Praxis](https://github.com/ouonet/praxis) ⭐ 9 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-31 - Intent-driven workflow skills for coding agents: describe what done looks like, not the steps. Triage-first design keeps token costs low across design, TDD, debug, review, and release.
* [debt-ops](https://github.com/bcanfield/agentic-tech-debt) ⭐ 8 | 🐛 13 | 🌐 Python | 📅 2026-08-31 - Catches AI-introduced tech debt at write-time: hooks log every deferral to a registry in your repo and a review skill ranks paydown by file churn.
* [Universal Design Principles](https://github.com/HDeibler/universal-design-principles) ⭐ 8 | 🐛 1 | 🌐 Markdown | 📅 2026-05-03 - Cross-agent UX and product-design marketplace with a root Codex collection plugin, five focused plugin bundles, and 137 Agent Skills for design review, accessibility, layout, interaction, cognition, and product polish.
* [BABOK Analyst](https://github.com/GSkuza/BABOK_ANALYST) ⭐ 7 | 🐛 10 | 🌐 JavaScript | 📅 2026-08-27 - BABOK v3 business analysis agent with 16 MCP tools, a 9-stage pipeline, and human-in-the-loop approval gates.
* [Cover My Repo](https://github.com/sjh9714/cover-my-repo) ⭐ 7 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-23 - Designs three checked GitHub social preview cards with Codex or Cursor, then renders them locally with Chrome.
* [Tartiner Labs](https://github.com/tartinerlabs/skills) ⭐ 7 | 🐛 5 | 🌐 Go | 📅 2026-08-23 - Agent skills for git workflows, GitHub automation, security audits, code refactoring, and project tooling.
* [Wingman](https://github.com/lsshym/wingman.ai) ⭐ 7 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-25 - Cross-platform AI coding-agent plugin for repo-local project memory, data-contract checks, and project-map discovery before agents edit code.
* [Zagrosi Forge](https://github.com/zagrosi-code/zagrosi-forge) ⭐ 7 | 🐛 2 | 🌐 Python | 📅 2026-08-28 - Decompose broad project briefs into researched plans and implement sectioned work with TDD, quality gates, and traceability.
* [Embedded Workbench](https://github.com/AmethystLuna/embedded-workbench) ⭐ 6 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-31 - Embedded C/C++ firmware development toolbox — 7 skills (FreeRTOS, Keil MDK, ARMCLANG, HardFault triage, state machines, LVGL) plus workflow gates and 4 agents for Claude Code, Codex, Cursor, Kimi, OpenCode, and ZCode.
* [Agent Workflow System](https://github.com/1139030773-cmd/agent-workflow-system) ⭐ 5 | 🐛 0 | 🌐 PowerShell | 📅 2026-06-12 - 一套中文AI工作流系统：7个协作技能 + 行为规范宪法 + 会话恢复机制，模糊目标→可执行任务，全生命周期引导。Codex & Claude Code 双平台，新手友好。
* [ArmorCodex](https://github.com/armoriq/armorCodex) ⭐ 5 | 🐛 25 | 🌐 JavaScript | 📅 2026-08-25 - Intent-based security for Codex with MCP plan registration, policy gating, CSRG cryptographic proofs, and audit logging on `bash` and `apply_patch`.
* [Codex rg Guard](https://github.com/Rycen7822/codex-rg-guard) ⭐ 5 | 🐛 0 | 🌐 Rust | 📅 2026-05-09 - Budgeted `rg`/`grep` replacement for Codex that narrows broad searches before they waste model context.
* [Dev Skills](https://github.com/Jason-chen-coder/dev-skills) ⭐ 5 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-12 - Team workflow skills for specs, plans, TDD, debugging, verification, review, branch finishing, and design context.
* [LLM Transpile](https://github.com/epicsagas/llm-transpile) ⭐ 5 | 🐛 5 | 🌐 HTML | 📅 2026-07-24 - Auto-compress .md, .html, and .txt files via PostToolUse hook, cutting context usage by up to 40% with zero workflow change.
* [Maestro](https://github.com/mbanderas/maestro) ⭐ 5 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-27 - Opt-in local multi-CLI fusion engine and orchestration doctrine that fans a prompt across model CLIs, then judges and synthesizes one grounded answer.
* [MCP Migration Check](https://github.com/AlpayC/mcp-migration-check) ⭐ 5 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-31 - Deterministic MCP 2026-07-28 migration checker with an agent skill, CLI, GitHub Action, and hosted web probe powered by one rule engine.
* [Simple Man](https://github.com/Maksim-Burtsev/simple-man) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2026-08-22 - High-compression communication mode for Codex agents that removes filler while preserving search, validation, and implementation effort.
* [VillageSQL Skills](https://github.com/villagesql/villagesql-skills) ⭐ 5 | 🐛 1 | 📅 2026-08-29 - Skills for VillageSQL including building extensions from scratch and porting PostgreSQL extensions to VillageSQL.
* [Agentizer](https://github.com/Humiris/wwa-transform) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2026-05-05 - Turn any website into an AI-powered agentfront with split-pane
* [HOL Guard Plugin](https://github.com/hashgraph-online/hol-guard-plugin) ⭐ 4 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-26 - AI antivirus workflow for Codex, Claude Code, Cursor, Gemini, OpenCode, MCP servers, skills, and plugin release checks with local approvals and receipts.
* [LoreDocs](https://github.com/labyrinth-analytics/loredocs) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-08-31 - Knowledge vault MCP server for Claude — organizes durable project docs, specs, and guides with FTS5 search, tagging, and cross-project context loading.
* [Superpipelines](https://github.com/gustavo-meilus/superpipelines) ⭐ 4 | 🐛 13 | 🌐 JavaScript | 📅 2026-07-15 - Design and run write/review-isolated multi-agent AI pipelines across Codex, Claude Code, OpenCode, Cursor, Windsurf, and Cline.
* [tailtest](https://github.com/avansaber/tailtest-codex) ⭐ 4 | 🐛 9 | 🌐 Python | 📅 2026-06-13 - Hook-powered test generation -- detects files changed during an agent turn and instructs Codex to write and run tests automatically. Zero config, 8 languages.
* [Codex How To](https://github.com/Phelan164/codex-howto) ⭐ 3 | 🐛 3 | 🌐 Python | 📅 2026-08-31 - Engineering-first Codex curriculum and plugin with 9 skills, measured token-efficiency experiments, bounded orchestration, testing, review, and living knowledge maintenance.
* [Codex Process Jobs](https://github.com/joelfarthing/codex-process-jobs) ⭐ 3 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-26 - Run long local builds, tests, benchmarks, and inference jobs as durable detached processes with tracked status, bounded results, and completion delivery across Codex surfaces.
* [Context Guard](https://github.com/GreenLv/codex-context-guard) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-08-31 - Preserves authoritative requirements and verification evidence across long-running Codex tasks and context compaction.
* [LinkedIn Animated Infographics](https://github.com/imMamdouhaboammar/linkedin-animated-infographics) ⭐ 3 | 🐛 1 | 🌐 Python | 📅 2026-08-31 - Evidence-safe animated infographic generator with multi-agent design pipeline for LinkedIn.
* [Logic Probe](https://github.com/AmethystLuna/logicprobe) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-31 - Design-document & plan claim verification — checks every verifiable claim against the codebase, escalates behavioral claims to executable-model verification (7 structural checks + 7 adversarial probes), and compares before/after models for refactoring regression detection.
* [AgiFlow](https://github.com/AgiFlow/ai-plugin) ⭐ 2 | 🐛 0 | 📅 2026-07-10 - Project management workflows for AI coding agents with planning, grooming, task execution, review, and AgiFlow MCP integration.
* [AIBoarding](https://github.com/gustavo-meilus/aiboarding) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Generate, maintain, compress, and audit standard AI-agent onboarding files with AGENTS.md, CLAUDE.md, drift tracking, and lifecycle hooks.
* [Anchor](https://github.com/biefan/anchor) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-05-22 - Engineering discipline pack for Claude Code & Codex CLI with task-scope locking, anti-drift braking, condition-based codex review, project-CLAUDE.md pitfall writeback, and PreToolUse hooks that block irreversible bash patterns.
* [Codex Skin Pack Installer](https://github.com/ChannelerH/codex-skin-packs) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-08-25 - Codex plugin and Skill that stages verified desktop skin packs from GitHub releases, validates files, and keeps restore guidance visible.
* [Codex Usage and Resets](https://github.com/joelfarthing/codex-usage-and-resets) ⭐ 2 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-26 - Turns Codex usage into planning facts with linear pace, projected exhaustion, banked-reset expirations, and conservative unexpected-reset detection.
* [falsegreen-skill](https://github.com/vinicq/falsegreen-skill) ⭐ 2 | 🐛 5 | 🌐 JavaScript | 📅 2026-08-31 - Finds tests that stay green when the code they cover is broken, applying six ordered judgments over Python, TypeScript, JavaScript, and Robot Framework suites in Codex CLI and Claude Code.
* [GCF Proxy](https://github.com/blackwell-systems/gcf-codex-plugin) ⭐ 2 | 🐛 2 | 📅 2026-08-29 - Save 71% on MCP tool call tokens by wrapping any server with GCF encoding, with session stats hook and setup skill.
* [GrayMatter](https://github.com/ValkyrLabs/GrayMatter) ⭐ 2 | 🐛 1 | 🌐 Shell | 📅 2026-08-27 - Durable memory and shared graph state for Codex and OpenClaw agents, with live ValkyrAI schema awareness.
* [River Review](https://github.com/s977043/river-review) ⭐ 2 | 🐛 19 | 🌐 JavaScript | 📅 2026-08-31 - Versioned Skill Registry of code-review skills driven by a perspective-based review agent (code, security, performance, architecture, testing, adversarial) that verifies findings against the diff.
* [site-risk-check](https://github.com/kobimantzur/agent-skills) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-08-27 - Zero-dependency skill that scans a live URL for the conditions behind accessibility and privacy demand letters — trackers firing before consent, missing policies, and machine-checkable WCAG gaps — mapped to the jurisdictions the site actually sells to.
* [Team Skills Platform](https://github.com/Colin4k1024/tsp) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-19 - Role-based team delivery framework — Tech Lead-orchestrated 8-role system with 195+ skills, 27 specialist agents, 80+ commands, hooks, and ECC harness for Claude Code, Codex, and OpenCode.
* [Agentry Observability](https://github.com/fr33dr4g0n/agentry-public) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-07-13 - Agent-native product analytics, error logging, and deploy attribution for coding agents through one HTTP API.
* [Antigravity Context Meter](https://github.com/Dunphil692/antigravity-context-meter) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-26 - Real-time 1:1 Cursor-style context meter & zero-loss session migration for Google Antigravity (Desktop HUD & IDE Extension).
* [Bring Your AI Migration Auditor](https://github.com/unitedideas/bringyour-mcp) ⭐ 1 | 🐛 0 | 📅 2026-05-25 - Read-only Codex plugin for auditing Claude Code to Codex migrations before Codex edits code. Checks AGENTS.md/CLAUDE.md scope, hooks, MCP config, skills, secret references, and validation notes.
* [claude-jit-context](https://github.com/Digital-Process-Tools/claude-jit-context) ⭐ 1 | 🐛 3 | 🌐 Shell | 📅 2026-08-26 - Project knowledge that loads only when it is needed, matched against the prompt, the file being touched, or the tool being run instead of sitting in context all session.
* [dev-harness-kit](https://github.com/sh-ai-x/dev-harness-kit) ⭐ 1 | 🐛 2 | 🌐 Python | 📅 2026-08-31 - Enforced development workflow skills for Codex and Claude Code covering planning, TDD, debugging, review, security, CI, and release.
* [kgai](https://github.com/kgaidev/kgai) ⭐ 1 | 🐛 0 | 🌐 Go | 📅 2026-08-29 - Shared decision memory for AI dev teams, an immutable local log of the decisions behind your code, synced over an S3 bucket you own.
* [LVTD Skills](https://github.com/LVTD-LLC/skills) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-07-28 - Reusable Agent Skills for Codex, Claude Code, and compatible clients, covering Django, Rust, Cookiecutter, SEO, traction, product marketing, and nonfiction publishing workflows.
* [MailAgent](https://github.com/Alex0nder/MailAgent) ⚠️ Archived - Temporary inboxes for Codex — OTP, magic links, signup QA, simulate-first autotests (23 MCP tools).
* [Mermail Skills](https://github.com/Nudgen-Marketing/mermail-skills) ⭐ 1 | 🐛 84 | 🌐 JavaScript | 📅 2026-08-27 - Official Mermail Agent Skills and Codex plugin that connect AI assistants to hosted Mermail MCP for inbox, scheduling, GTM, support, and x402 wallet workflows.
* [Registry Broker](https://github.com/hashgraph-online/registry-broker-codex-plugin) ⭐ 1 | 🐛 17 | 🌐 TypeScript | 📅 2026-08-24 - Delegate tasks to specialist AI agents via the HOL Registry, plan, find, summon, and recover sessions.
* [RoadmapSmith](https://github.com/PapiScholz/roadmapsmith) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-30 - Evidence-backed ROADMAP.md workflows for AI coding agents with validation, sync, and roadmap generation across any tech stack.
* [Runtype Skills](https://github.com/runtypelabs/skills) ⭐ 1 | 🐛 7 | 🌐 JavaScript | 📅 2026-08-27 - Supercharge your coding agent for AI product development — build, deploy, and operate agents, flows, tools, and surfaces on Runtype's managed edge runtime.
* [skill-sync-publisher](https://github.com/liuyewang/skill-sync-publisher) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-28 - Safely synchronize this Codex skill across public agent-skill registries.
* [Spellbook Skills](https://github.com/yyykf/spellbook-skills) ⭐ 1 | 🐛 3 | 🌐 Python | 📅 2026-08-29 - Practical Claude Code and Codex skills for worktrees, PR/MR automation, review cleanup, YApi lookup, and Java DDD guidance.
* [Tandem Workflow Architect](https://github.com/frumu-ai/tandem-codex-plugin) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-05-21 - Plan Tandem workflows in Codex, then validate, preview, and run them through the governed Tandem engine.
* [Unforgit](https://github.com/MiguelMedeiros/unforgit-codex-plugin) ⭐ 1 | 🐛 1 | 📅 2026-08-28 - Git-backed repository memory for Codex and other coding agents via MCP, with durable local knowledge for decisions, conventions, gotchas, and playbooks.
* [Unity Agent Workflows](https://github.com/AUN-PN/unity-agent-workflows) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-05-19 - Codex plugin and skill for Unity 2D agents that enforces "No proof, no edit" workflows with runtime-owner proof, Teach structure maps, and validation gates.
* [Workflow Kit](https://github.com/Le-Xuan-Thang/workflow-kit) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-06-02 - Full product lifecycle plugin for Claude Code, Codex CLI, and OpenCode: define Vision/Mission/Core → generate workplan → execute with mandatory cross-provider reviewer agents → synthesize deliverables → maintain, with parallel task execution, crash recovery, and AgentOps metrics.
* [Agency Continuity Audit](https://github.com/revertcreations/agency-continuity-audit) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-08-26 - Read-only audit that distinguishes durable agent goals, state, corrections, restart evidence, authority boundaries, scheduler claims, and commercial proof from self-reported health.
* [Agent Deck](https://github.com/not-so-fat/agent-deck) ⭐ 0 | 🐛 4 | 🌐 TypeScript | 📅 2026-08-30 - One MCP for context management: bind self-improving playbooks, MCP tools, and API keys to the session.
* [Claude Code Codex Plugin](https://github.com/davidq888/claude-code-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-26 - Security-focused Codex plugin that connects to the local Claude Code CLI through MCP with login, status checks, safe-mode prompts, and no credential storage.
* [CodeTruss](https://github.com/DeliriumPulse/codetruss-plugins) ⭐ 0 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-12 - Local-first acceptance gate that checks coding-agent scope, sensitive surfaces, deterministic analyzers, and repository verification from immutable Git snapshots, then writes signed receipts before the PR.
* [Codex TUI Proof](https://github.com/bnc4vk/codex-tui-proof) ⭐ 0 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-01 - Visually validate real local terminal UIs in Codex's in-app browser with screenshots and session evidence.
* [Contexo](https://github.com/maheedhar132/Contexo) ⭐ 0 | 🐛 8 | 🌐 TypeScript | 📅 2026-08-25 - Portable AI context and cost control across every AI coding harness.
* [Delx Recovery](https://github.com/davidmosiah/delx-plugins) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-15 - Free recovery and continuity plugin for AI agents: resume prior sessions, capture state, process failures into a recovery plan, and remember across sessions through a hosted MCP server (works in Codex, Claude Code, Cursor, and VS Code).
* [metabrain](https://github.com/ariaxhan/metabrain) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-26 - MCP server for agent memory: SQLite, zero dependencies, tools learn/recall/verdict/hypotheses/start\_brief/stats/capture\_error, patterns graduating to hypotheses then preferences; `pip install "metabrain[mcp]"` then `metabrain-mcp --db PATH`.
* [Ontoly](https://github.com/0xsarwagya/ontoly-codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-07-21 - Deterministic Software Graph workflows for Codex: architecture review, dependency analysis, request tracing, configuration analysis, and impact analysis.
* [Personal Data Protection](https://github.com/AltByteSG/personal-data-protection-skill) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-05-17 - Engineer-facing personal-data-protection compliance reference — Singapore PDPA, Thailand PDPA, Indonesia UU PDP, Malaysia PDPA (Act 709 + 2024 Amendments), Philippines DPA — organised by where in the stack each obligation lands, with checklists, breach-response runbook, and a developer-view divergence table across all five.
* [Tree Ring Memory](https://github.com/TerminallyLazy/tree-ring-memory-codex-plugin) ⭐ 0 | 🐛 1 | 🌐 Shell | 📅 2026-08-26 - Local-first memory lifecycle guidance for Codex agents with recall, evidence-backed lessons, privacy-safe memory capture, audit, consolidation, and explicit forgetting.
* [Changelog Forge](./plugins/mturac/changelog-forge) - Conventional commits → CHANGELOG section + semver bump.
* [Codex Full-Stack Workflow](https://github.com/kevin592/codex-full-stack-workflow) - Turns rough product requests into staged, reviewable full-stack delivery with persistent requirements, change control, visual evidence, and completion gates.
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

* [ego-browser](https://github.com/citrolabs/ego-lite) ⭐ 14,486 | 🐛 145 | 🌐 JavaScript | 📅 2026-08-31 - Browser automation for AI agents through ego lite, a Chromium browser where agents navigate pages, fill forms, capture screenshots, and extract data in isolated task spaces that reuse the user's existing logins.
* [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-AI-Toolkit) ⭐ 1,087 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-31 - Backend for AI coding agents on Tencent CloudBase — database, auth, and functions via Plugin, Skills & MCP.
* [KiCad Happy](https://github.com/aklofas/kicad-happy) ⭐ 1,054 | 🐛 5 | 🌐 Python | 📅 2026-08-20 - KiCad EDA skills for schematic analysis, PCB layout review, component sourcing, BOM management, and manufacturing preparation.
* [Digital Marketing Pro](https://github.com/indranilbanerjee/digital-marketing-pro) ⭐ 779 | 🐛 0 | 🌐 Python | 📅 2026-08-17 - Open-source AI marketing plugin for agencies — 154 skills, 25 specialist agents, 12-Part Strategy Flow, AEO/GEO, GSC AI Performance Report, Google Ads API v24, EU AI Act Article 50 / C2PA compliance.
* [Education Agent Skills](https://github.com/GarethManning/education-agent-skills) ⭐ 709 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-28 - 131 evidence-based education skills for curriculum design, lesson planning, and assessment, with transparent evidence ratings and MCP server.
* [LinkedIn Skills](https://github.com/sergebulaev/linkedin-skills) ⭐ 629 | 🐛 0 | 🌐 Python | 📅 2026-08-30 - Codex-ready LinkedIn marketing bundle with a native .codex-plugin manifest and 10 skills: post writing with 16 tested hook formulas, AI-tell humanizer, pre-publish audit, comment and reply drafting, hook extraction, content planning, profile optimization, engager analytics, and thread monitoring; also works in Claude Code.
* [ru-text](https://github.com/talkstream/ru-text) ⭐ 222 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Russian text quality — \~1,044 rules for typography, info-style, editorial, UX writing, and business correspondence.
* [Taisly Agent Kit](https://github.com/taisly/agent) ⭐ 220 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-06 - Publish short-form videos to TikTok, Instagram Reels, YouTube Shorts, X, and Facebook from Codex with the Taisly MCP server and bundled social media posting skill.
* [Telnyx](https://github.com/team-telnyx/ai) ⭐ 213 | 🐛 16 | 🌐 TypeScript | 📅 2026-08-31 - Telnyx toolkit for AI agents bundling Claude Code, Cursor, Gemini CLI, and OpenCode plugins, an agent toolkit for OpenAI/LangChain/CrewAI/Vercel AI SDK, a hosted MCP server, and a one-command CLI for messaging, voice, numbers, and account management.
* [Bitbucket CLI](https://github.com/avivsinai/bitbucket-cli) ⭐ 197 | 🐛 4 | 🌐 Go | 📅 2026-08-31 - Manage Bitbucket repos, PRs, branches, issues, webhooks, and pipelines for Data Center and Cloud.
* [Codex Usage Tracker](https://github.com/douglasmonsky/codex-usage-tracker) ⭐ 193 | 🐛 10 | 🌐 Python | 📅 2026-08-20 - Track aggregate Codex token usage from local session logs with MCP tools for summaries, session detail, CSV export, and dashboard generation.
* [X Twitter Scraper](https://github.com/Xquik-dev/x-twitter-scraper) ⭐ 192 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-27 - X/Twitter data, monitored workflows, HMAC webhooks, and MCP access through the Xquik REST API with confirmation-gated write guidance.
* [OC ChatGPT Multi Auth](https://github.com/ndycode/oc-chatgpt-multi-auth) ⭐ 181 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-31 - Codex setup skill and OpenCode plugin for ChatGPT Plus/Pro OAuth, GPT-5/Codex presets, and multi-account failover.
* [Miro](https://github.com/miroapp/miro-ai) ⭐ 151 | 🐛 14 | 🌐 TypeScript | 📅 2026-08-26 - Official Miro MCP server and agent integrations for Claude Code, Codex, Gemini CLI, Cursor, and other AI tools — read and write Miro boards, create diagrams, extract context from boards, and generate code from designs.
* [Hostinger API MCP](https://github.com/hostinger/api-mcp-server) ⭐ 149 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-28 - Manage Hostinger VPS, domains, DNS, hosting, and billing through MCP tools backed by the official Hostinger API.
* [unslop](https://github.com/MohamedAbdallah-14/unslop) ⭐ 121 | 🐛 1 | 🌐 Python | 📅 2026-08-31 - Strip AI writing patterns from text output — removes filler phrases, hedging language, and generic constructs to produce cleaner written content. Install: `npm install -g unslop`.
* [Langfuse Observability](https://github.com/avivsinai/langfuse-mcp) ⭐ 105 | 🐛 1 | 🌐 Python | 📅 2026-08-26 - Query traces, debug exceptions, analyze sessions, and manage prompts via MCP tools.
* [Agent Message Queue](https://github.com/avivsinai/agent-message-queue) ⭐ 85 | 🐛 5 | 🌐 Go | 📅 2026-08-31 - File-based inter-agent messaging with co-op mode, cross-project federation, and orchestrator integrations.
* [Call-E](https://github.com/CALLE-AI/call-e-integrations) ⭐ 85 | 🐛 10 | 🌐 JavaScript | 📅 2026-08-27 - Plan, run, and inspect Call-E phone call workflows from Codex through the calle CLI.
* [Jenkins CLI](https://github.com/avivsinai/jenkins-cli) ⭐ 82 | 🐛 3 | 🌐 Go | 📅 2026-08-31 - GitHub CLI-style interface for Jenkins controllers with jobs, pipelines, runs, logs, artifacts, credentials, and nodes.
* [Cortex](https://github.com/cdeust/Cortex) ⭐ 71 | 🐛 17 | 🌐 Python | 📅 2026-08-30 - Persistent thermodynamic memory and cognitive-profiling MCP server for Claude Code, Codex, and Gemini CLI — heat/decay dynamics, predictive-coding write gates, knowledge graph, and intent-aware recall across sessions.
* [Azure Cosmos DB Agent Kit](https://github.com/AzureCosmosDB/cosmosdb-agent-kit) ⭐ 53 | 🐛 24 | 🌐 Python | 📅 2026-08-24 - Azure Cosmos DB best-practice skills and MCP tooling for Codex, Claude Code, Cursor, Gemini CLI, Grok Build, Kimi Code, GitHub Copilot, and other Agent Skills-compatible assistants.
* [Nimble](https://github.com/Nimbleway/agent-skills) ⭐ 53 | 🐛 4 | 🌐 Python | 📅 2026-08-26 - Web Search Agents that search, browse, extract, and reason across live pages and return cited, schema-enforced results, with self-learning retrieval that improves accuracy and lowers cost per task on repeat work, plus Search and Extract skills for fast raw web data in Claude Code, Codex, Cursor, and Grok Build.
* [ScrapeGraph AI](https://github.com/ScrapeGraphAI/just-scrape) ⭐ 52 | 🐛 4 | 🌐 TypeScript | 📅 2026-08-24 - AI-powered web scraping CLI to search, scrape, extract structured JSON, crawl, and monitor web pages via the ScrapeGraph AI API.
* [X (Twitter) Skills](https://github.com/sergebulaev/x-skills) ⭐ 50 | 🐛 1 | 🌐 Python | 📅 2026-08-30 - Codex-ready X (Twitter) marketing bundle with a native .codex-plugin manifest: tweet and thread writing with corpus-validated hook formulas (validated against \~450 top tweets), AI-tell humanizer, hook extraction, reply drafting, content planning, and audience insights; also works in Claude Code.
* [AnyCap](https://github.com/anycap-ai/anycap) ⭐ 42 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-25 - Multimodal media generation, analysis, live web research, file sharing, and page publishing through one CLI, Agent Skill, and local MCP server.
* [PANews Agent Toolkit](https://github.com/panewslab/skills) ⭐ 42 | 🐛 0 | 🌐 JavaScript | 📅 2026-04-16 - Crypto and blockchain news discovery, authenticated creator publishing workflows, and page-to-Markdown reading.
* [Pronounce](https://github.com/anzy-renlab-ai/pronounce) ⭐ 39 | 🐛 1 | 🌐 Shell | 📅 2026-08-27 - Pronounce developer jargon out loud: an MCP server (lookup/search) and skill backed by a 1,721-entry sourced dictionary with IPA, audio, and cited pronunciations for kubectl, nginx, YAML, JWT, and more.
* [Kachilu Browser](https://github.com/kachilu-inc/kachilu-browser) ⭐ 38 | 🐛 0 | 🌐 JavaScript | 📅 2026-05-12 - Anti-bot-aware browser automation for AI agents with MCP tools, CAPTCHA-aware workflows, and WSL2 Windows browser support.
* [Talivia Agent Kit](https://github.com/talivia-group/agent) ⭐ 35 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-02 - Install and verify revenue-first website analytics from Codex, connect payment attribution, and identify which traffic sources and customer journeys become revenue.
* [Flow Studio Power Automate](https://github.com/ninihen1/power-automate-mcp-skills) ⭐ 31 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-27 - Debug, build, and operate Power Automate flows via FlowStudio MCP with action-level inputs and outputs.
* [Hermes Tweet](https://github.com/Xquik-dev/hermes-tweet) ⭐ 31 | 🐛 3 | 🌐 Python | 📅 2026-08-25 - Hermes Agent X/Twitter plugin for read-first social research, monitoring, and approval-gated actions through Xquik.
* [MorningAI](https://github.com/octo-patch/MorningAI) ⭐ 29 | 🐛 2 | 🌐 Python | 📅 2026-05-16 - AI news tracking skill that monitors 80+ entities across 6 sources (Reddit, HN, GitHub, Hugging Face, arXiv, X) and generates scored daily reports with infographics and message digests.
* [Kreuzberg](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Local document extraction for 91+ formats with skills for CLI usage, OCR, table extraction, output formats, and a local MCP server.
* [Kreuzberg Cloud](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Managed document extraction for Codex with API-key setup, presigned uploads, job tracking, webhook workflows, and usage guidance.
* [Kreuzcrawl](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Web crawling and scraping for Codex with skills for single-page scraping, site crawls, URL mapping, and headless browser fallback.
* [Codex Obsidian](https://github.com/greg-asher/codex-obsidian) ⭐ 25 | 🐛 1 | 📅 2026-04-22 - Local Obsidian note and vault workflows through the official desktop `obsidian` CLI.
* [Skill-Atlas](https://github.com/danielLublinsky/Skill-Atlas) ⭐ 23 | 🐛 1 | 🌐 Python | 📅 2026-08-16 - A third tier for Claude Code skills — dormant, zero tokens, still findable. Search a graph of your collection instead of preloading it.
* [Zero Slop](https://github.com/manavmishra/ZeroSlop) ⭐ 23 | 🐛 4 | 🌐 Python | 📅 2026-08-31 - Say no to AI slop: a human-in-the-loop learning agentic workflow skill that scores text 0-100 for AI slop and rewrites it tastefully, with a standard-library Python scorer that has zero dependencies and runs offline.
* [Yandex Direct](https://github.com/nebelov/yandex-direct-for-all) ⭐ 21 | 🐛 1 | 🌐 Python | 📅 2026-07-17 - GitHub-ready Codex plugin bundle for Yandex Direct, Wordstat, Metrika, and Roistat.
* [prompt-to-asset](https://github.com/MohamedAbdallah-14/prompt-to-asset) ⭐ 18 | 🐛 15 | 🌐 TypeScript | 📅 2026-08-12 - Route image-generation prompts to 30+ models (DALL-E, Stable Diffusion, Flux, Midjourney, and more) through a single MCP interface. Install: `npm install -g prompt-to-asset`.
* [Kindle Highlights](https://github.com/l3a0/claude-plugins) ⭐ 17 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-30 - Claude Code skill that exports a book's Kindle highlights to verbatim, location-cited Markdown, recovering the ones Amazon's export limit truncates or hides (macOS).
* [claude-math](https://github.com/vladimirrott/claude-math) ⭐ 16 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-18 - Emit mathematics as copy- and search-safe inline Unicode (∑, ≤, ℝ, x², matrices, set-builder) instead of LaTeX so equations stay legible in the Codex TUI, terminals, and Claude Code.
* [Cargo Skills](https://github.com/getcargohq/cargo-skills) ⭐ 15 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-29 - GTM engineering for coding agents — 17 skills over the Cargo CLI for lead sourcing, contact enrichment and email verification, lead scoring, CRM sync, buying-signal monitoring, and workspace-as-code.
* [Thermal-Fluid Research Workflow](https://github.com/hanhuark/mechanical-engineering-research-skill) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2026-08-29 - Thermal-fluid mechanical engineering research workflow for literature review, technical writing, data analysis, presentations, proposals, coding, and AI/ML tools.
* [Codex Mem](https://github.com/2kDarki/codex-mem) ⭐ 12 | 🐛 0 | 🌐 TypeScript | 📅 2026-03-23 - Automatically capture, compress, and inject session context back into future Codex sessions.
* [Data Product Builder for dbt](https://github.com/entropy-data/dataproduct-builder-dbt) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-05-28 - Full data-product lifecycle on dbt for Entropy Data: scaffold, audit, and integrate projects with ODCS, ODPS, OpenLineage, and GitHub Actions.
* [Context Pack](https://github.com/Rothschildiuk/context-pack) ⭐ 10 | 🐛 0 | 🌐 Rust | 📅 2026-03-19 - Generate compact first-pass repository briefings for coding agents before deeper exploration.
* [Val Town](https://github.com/val-town/plugins) ⭐ 10 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-29 - Build and deploy serverless TypeScript on Val Town from Codex — hosted MCP server plus skills for HTTP vals, cron, SQLite, email, OAuth, and React UI.
* [Codex SEO](https://github.com/BestLemoon/codex-seo) ⭐ 9 | 🐛 8 | 🌐 Python | 📅 2026-07-03 - Full-stack SEO audits, Google API workflows, backlinks analysis, reporting, and optional MCP extensions for Codex.
* [sitemd](https://github.com/sitemd-cc/sitemd) ⭐ 9 | 🐛 2 | 🌐 HTML | 📅 2026-06-25 - Build websites from Markdown via MCP — 22 tools for creating pages, generating content, validating, running SEO audits, configuring settings, and deploying static sites to Cloudflare Pages.
* [WakeWire](https://github.com/glenncalleja/wakewire) ⭐ 9 | 🐛 6 | 🌐 TypeScript | 📅 2026-08-31 - Push events from GitHub, Gmail, Slack, and any signed webhook (Linear, Sentry, ClickUp) straight into your Codex threads as new turns — event-driven triggers instead of polling, with HMAC verification, deduplication, and a durable delivery queue.
* [SysKnife](https://github.com/lacs-project/sysknife) ⭐ 8 | 🐛 34 | 🌐 Rust | 📅 2026-08-28 - Linux sysadmin co-pilot as an MCP server for Codex: plain-language requests become typed, risk-classified actions that a privileged daemon runs only after out-of-band terminal approval, with an Ed25519-signed audit chain and automatic rollback.
* [Codex Be Serious](https://github.com/lulucatdev/codex-be-serious) ⭐ 7 | 🐛 0 | 🌐 Shell | 📅 2026-06-01 - Enforce formal, textbook-grade written register across all agent output.
* [Rust Reverse Engineering](https://github.com/jingjing2222/rust-reverse-engineering-skill) ⭐ 7 | 🐛 0 | 🌐 Shell | 📅 2026-04-18 - Reverse engineer Rust binaries and libraries: triage targets, demangle symbols, recover crate namespaces, and map panic, unwind, async, and FFI paths.
* [Apple Productivity](https://github.com/matk0shub/apple-productivity-mcp) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-03-27 - Local Apple Calendar and Reminders tooling for macOS with Codex plugin adapters.
* [Dodo Payments](https://github.com/dodopayments/dodo-agent-plugin) ⭐ 6 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-31 - Payments integration for checkouts, subscriptions, and billing with live API and documentation MCP servers with browser OAuth.
* [Unified AI System](https://github.com/happy520ai/unified-ai-system) ⭐ 6 | 🐛 15 | 🌐 JavaScript | 📅 2026-08-29 - Self-hosted AI gateway for Codex with provider-free prompt enhancement, nine governed MCP tools, and a credential-free Docker path.
* [Upwork Autopilot](https://github.com/klajdikkolaj/upwork-autopilot) ⭐ 6 | 🐛 4 | 🌐 JavaScript | 📅 2026-07-03 - Controlled Upwork job search, qualification, and proposal submission sessions through a dedicated Chrome profile.
* [AutoCAD Tianzheng Tools](https://github.com/summer521521/AutoCAD_Tianzheng_plugin) ⭐ 5 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to AutoCAD and Tianzheng HVAC through a local MCP server for DWG-aware HVAC drawing inspection and workflow automation.
* [Chrome DevTools](https://github.com/win4r/chrome-devtools-codex-plugin) ⭐ 5 | 🐛 0 | 📅 2026-03-27 - One-click Codex plugin wrapper for chrome-devtools-mcp.
* [PapersFlow](https://github.com/papersflow-ai/papersflow-codex-plugin) ⭐ 4 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-29 - Paper discovery, citation verification, graph exploration, and DeepScan analysis.
* [Read Image](https://github.com/ZXY1240/read-image) ⭐ 4 | 🐛 6 | 🌐 Python | 📅 2026-08-17 - Read local images, videos, web pages, and Windows screenshots through Doubao, GLM, or Qwen-compatible vision APIs.
* [Remotion Plugin](https://github.com/tim-osterhus/codex-remotion-plugin) ⭐ 4 | 🐛 0 | 📅 2026-04-03 - Build parameterized Remotion videos in Codex with the official Remotion docs MCP, composition scaffolding, and a data-driven launch-video workflow.
* [Synta MCP](https://github.com/Synta-ai/n8n-mcp-codex-plugin-synta) ⭐ 4 | 🐛 0 | 📅 2026-04-03 - Build, edit, validate, and self-heal n8n workflows with Synta MCP tools and Codex-ready workflow guidance.
* [Task Scheduler](https://github.com/6Delta9/task-scheduler-codex-plugin) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-04-03 - OpenAI Codex plugin and local MCP server for turning task lists into realistic schedules with blocked dates, capacity overrides, overflow tracking, and markdown planning output.
* [Agent Vision](https://github.com/zfifteen/agent-vision) ⭐ 3 | 🐛 0 | 🌐 Shell | 📅 2026-07-14 - macOS-only local camera plugin for explicit snapshots, streaming controls, and file-backed image input.
* [Antigravity 2.0](https://github.com/comprono/antigravity-2-codex-plugin) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-07 - Local Codex bridge for Antigravity desktop with setup checks, model limit summaries, DevTools UI automation, and safe project/chat handoff.
* [AxonFlow](https://github.com/getaxonflow/axonflow-codex-plugin) ⭐ 3 | 🐛 0 | 🌐 Shell | 📅 2026-08-30 - Runtime governance for Codex with policy enforcement on terminal commands, advisory checks for non-terminal tools via skills, PII/secret detection, and compliance-grade audit trails. Self-hosted via Docker.
* [Feishu to Codex](https://github.com/zlsbksdxl/codex-lark) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-10 - Connect Codex to Feishu/Lark workflows for Docs, Messenger, Drive, Sheets, Base, Calendar, Tasks, Meetings, Mail, approvals, and more through the official Lark CLI.
* [Zotero Research Tools](https://github.com/summer521521/Zotero_Research_plugin) ⭐ 3 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to Zotero Desktop for local-library search, citation export, collection and tag inspection, and research workflow support.
* [Agentgram](https://github.com/jerryfane/agentgram) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-07-28 - Send explicit Telegram messages from Codex and local AI agents through a Telegram bot token and chat id.
* [Cadence Code](https://github.com/michael-L-i/cadence-code) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-08-28 - Fully local voice conversations for Claude Code, Codex, Cursor, and Antigravity on Apple Silicon, with selectable MLX speech and transcription models.
* [Canvas Apps Plugin Codex](https://github.com/Ratnam-Mishra/canvas-apps-plugin-codex) ⭐ 2 | 🐛 1 | 📅 2026-05-03 - Build and edit Microsoft Power Apps Canvas Apps using natural language and Canvas Authoring MCP server.
* [Maestro: Costguard](https://github.com/mbanderas/costguard) ⭐ 2 | 🐛 5 | 🌐 TypeScript | 📅 2026-08-13 - Cost auditor for Codex that flags CI/cron and cloud-spend waste via read-only provider checks, then previews and applies surgical CI workflow fixes locally without writing to provider accounts or pushing git.
* [OrgX](https://github.com/useorgx/orgx-codex-plugin) ⭐ 2 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-29 - MCP access and initiative-aware skills for organizational workflows.
* [Shots](https://github.com/hitSlop/shots) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-08-25 - Agent-native App Store screenshot, app icon, ASO, and localization workflows through the hosted Shots MCP server.
* [AgentGuards](https://github.com/alelaguard/agentguards-plugins) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-30 - LLM security guardrails for Codex with enforcing hooks and MCP tools: jailbreak and prompt-injection detection, web-content scanning, data-exfiltration blocking, and destructive-command authorization.
* [agentmailkit](https://github.com/ariaxhan/agentmailkit) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-28 - MCP server for scheduled LLM-written email digests from RSS, web and local sources: tools list\_jobs/run\_job/preview\_job/list\_plugins, local-first, run\_job dry-run by default; `pip install "agentmailkit[mcp]"` then `agentmailkit mcp`.
* [Computer Usage Summary](https://github.com/liuyewang/computer-usage-summary-skill) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-03 - Privacy-first, local ActivityWatch reports for app time, AFK time, projects, billable work, and redacted timelines across macOS, Windows, and Linux.
* [CONTAM Tools](https://github.com/summer521521/CONTAM_plugin) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-01 - Runs and inspects CONTAM airflow projects through a local MCP server with project guards, diagnostics, simulation helpers, and bridge workflows.
* [Exa Web Search](https://github.com/zlsbksdxl/codex-exa) ⭐ 1 | 🐛 2 | 🌐 Shell | 📅 2026-08-26 - Search and fetch current web sources in Codex through the official Exa MCP server with browser OAuth.
* [MATLAB Simulink Tools](https://github.com/summer521521/MATLAB_Simulink_plugin) ⭐ 1 | 🐛 0 | 🌐 MATLAB | 📅 2026-07-01 - Connects Codex to MATLAB and Simulink through a local MCP server for model inspection, script execution, and engineering workflow automation.
* [Nullcost](https://github.com/johnvouros/nullcost-plugin) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-12 - Catalog-backed free-tier, free-trial, and cheap developer-tool recommendations for Codex through bundled skills and MCP tools.
* [Ophis](https://github.com/ophis-fi/skills) ⭐ 1 | 🐛 2 | 📅 2026-08-24 - Onchain token swaps for Codex via the hosted Ophis MCP server, MEV-protected and gasless, built on CoW Protocol.
* [Aient](https://github.com/aient-ai/aient-codex-plugin) ⭐ 0 | 🐛 0 | 📅 2026-06-02 - AI operations plugin for Codex that connects production telemetry, problem lifecycle context, and remediation workflows through Aient's MCP server.
* [CarsXE](https://github.com/carsxe/carsxe-codex-plugin) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-27 - Decode VINs, license plates, market value, vehicle history, recalls, liens, OBD codes, and more via the CarsXE API.
* [Coolify](https://github.com/Sevi-py/coolify-codex-plugin) ⭐ 0 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-28 - Control Coolify Cloud and self-hosted Coolify instances through API-aware workflow skills and local tools.
* [Droplinked](https://github.com/droplinked/droplinked-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-05 - Verified-inventory agentic commerce over a hosted MCP server, with merchant and product discovery, agent-initiated checkout, and onchain brand, credit-risk, and repayment attestations.
* [GH Project](https://github.com/zfifteen/gh-project-plugin) ⭐ 0 | 🐛 0 | 🌐 HTML | 📅 2026-05-15 - Create GitHub repositories from Codex with inferred defaults, native menus, explicit confirmation, and deterministic local cloning.
* [Lacuna Music](https://github.com/JOYLINK-LTD/lacuna-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-31 - Generate original instrumental music and vocal songs from Codex through the Lacuna MCP server.
* [Launch Fast](https://github.com/BlockchainHB/launchfast_codex_plugin) ⭐ 0 | 🐛 0 | 📅 2026-08-20 - Official Launch Fast plugin adapter for rapid SaaS deployment.
* [Mobazha](https://github.com/mobazha/mobazha-skills) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-05-03 - Decentralized e-commerce skills — deploy self-hosted stores, import products from Shopify/Amazon, configure custom domains and Telegram bots, set up Tor privacy, and manage your store via MCP.
* [OpenProject Codex](https://github.com/varaprasadreddy9676/openproject-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-16 - OpenProject integration for Codex with project, team, work package, bulk workflow, boards, wiki, meeting, attachment, and reporting support.
* [plori](https://github.com/plori-ai/codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-30 - Create and drive plori cloud agents (each an AI agent on its own cloud computer) over plori's remote MCP server, with OAuth auto-discovery.
* [site-spec](https://github.com/ariaxhan/site-spec) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-27 - MCP server for website audit and auto-fix: 40 checks across SEO, accessibility, privacy, structured data and AI searchability, tools audit\_site/fix\_issue/compile\_spec/list\_checks; `npx -y site-spec-mcp`.
* [SolidWorks GPT Plugin](https://github.com/Erfouni/solidworks-GPT-plugin) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-08-24 - Knowledge-backed SolidWorks design and validation workflows for Codex with standards lookup, CAD evidence gates, and consent-based session learning.
* [Storyflo](https://github.com/droplinked/storyflo-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-03 - Agentic newsroom over a hosted MCP server with narrated briefings, a news-versus-prediction-market Divergence Index, and a searchable declassified archive.
* [Token Harbor](https://github.com/NickHOI/Token-Harbor) ⭐ 0 | 🐛 6 | 🌐 JavaScript | 📅 2026-08-26 - Turn Codex token usage into Sail Power for a local-first fishing, fleet, and harbor-building companion game.
* [TokRepo Search](https://github.com/henu-wang/tokrepo-codex-plugin) ⭐ 0 | 🐛 0 | 📅 2026-04-02 - Search and install AI assets from TokRepo with a bundled skill and MCP server for Codex.
* [VidSeeds.ai](https://github.com/CarrotGamesStudios/vidseeds-mcp) ⭐ 0 | 🐛 0 | 📅 2026-07-20 - Hosted MCP connector for pre-upload video SEO, metadata optimization, AI thumbnails, and multi-platform publishing with workflow skills for Codex agents.
* [Mantis](./plugins/deonmenezes/mantishack) - Autonomous bug bounty hunter for authorized engagements — 7-phase FSM (RECON → AUTH → HUNT → CHAIN → VERIFY → GRADE → REPORT), parallel hunter sub-agents, cryptographic scope enforcement, and BLAKE3/Ed25519 Merkle event logs.
* [PDF Monster](https://github.com/jbaehova/pdf-monster) - Analyzes PDFs as extracted text, OCR text, rendered page images, and embedded figures for coding agents.
* [SEO Dungeon](https://github.com/avalonreset/seo-dungeon) - Gamified local SEO audits that turn website issues into 16-bit dungeon battles for Codex, Claude, and Gemini CLI workflows.

### Grok Plugins

xAI Grok Build plugins can bundle skills, commands, agents, hooks, MCP servers,
and language-server configuration. A native plugin may include
`.grok-plugin/plugin.json`; install a repository with `grok plugin install
owner/repo --trust`. Add verified community plugins here in alphabetical order.
See the [official xAI plugin marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 201 | 🐛 271 | 🌐 Python | 📅 2026-08-31
and [Grok plugin guide](https://github.com/xai-org/grok-build/blob/main/crates/codegen/xai-grok-pager/docs/user-guide/09-plugins.md) ⭐ 26,288 | 🐛 0 | 🌐 Rust | 📅 2026-08-31
before submitting.

* [Grok Imagine Cinematic Studio](https://github.com/FineComputer14451/Grok-Imagine-Cinematic-Studio) ⭐ 25 | 🐛 3 | 🌐 Python | 📅 2026-08-31 - Independent multi-agent cinematic production suite (25 Role-Card agents, 64 skills, Production Bible workflow, Character DNA locking, native Grok Imagine Video 1.5 support) for Grok Build.

### Kimi Plugins

Kimi Code plugins package skills, agents, and MCP servers for the Kimi runtime.
Depending on the plugin version, a repository can expose `kimi.plugin.json` or
`.kimi-plugin/plugin.json`; install a GitHub repository with Kimi Code's
`/plugins install https://github.com/owner/repo` command. Add verified community
plugins here in alphabetical order. See the [official Kimi plugin documentation](https://github.com/MoonshotAI/kimi-code/blob/main/docs/en/customization/plugins.md) ⭐ 7,180 | 🐛 1,252 | 🌐 TypeScript | 📅 2026-08-31
before submitting.

* [deja](https://github.com/vshulcz/deja-vu) ⭐ 744 | 🐛 55 | 🌐 Go | 📅 2026-08-31 - Recalls the sessions the other coding agents on the machine already wrote to disk, including work from before it was installed, through MCP tools, a `/deja:recall` command and recall on every prompt.

### DeepSeek Harness Plugins

DeepSeek Harness (DSH) plugins are Cordis modules or npm packages that expose a
`dsh.bundle` manifest and can be installed with `dsh plugin add`. Add verified
community plugins here in alphabetical order. See the [official DeepSeek Harness
plugin tutorial](https://github.com/deepseek-ai/deepseek-harness/blob/master/docs/cordis-tutorial/01-first-plugin.md) ⭐ 206,305 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-31
and the [`dsh-plugin` community topic](https://github.com/topics/dsh-plugin) before
submitting a repository.

* [dsh-deja](https://github.com/vshulcz/deja-vu) ⭐ 744 | 🐛 55 | 🌐 Go | 📅 2026-08-31 - Brings the session history of nineteen other coding agents into DeepSeek Harness: recall, session digest and per-file history tools over a local index, plus optional automatic recall.
* [Engramory](https://github.com/tinqiao-oss/engramory) ⭐ 179 | 🐛 1 | 🌐 Python | 📅 2026-08-31 - Curated, file-based long-term memory for DSH agents — plain markdown notes in one store shared across hosts, with the index size cap enforced as a monotonic `ctx.tools.guard()` refusal rather than a reminder. Install: `dsh plugin --profile <name> add dsh-engramory`.
* [dsh-config-manager](https://github.com/xiajiajun516/dsh-config-manager) ⭐ 58 | 🐛 6 | 🌐 TypeScript | 📅 2026-08-30 - Backup, restore, export, import, migrate and sync your complete DeepSeek Harness (DSH) configuration — settings, model providers, plugins, MCP servers, skills, agent presets and workspaces — and restore your whole environment on a new machine with one click.

## Formats & Development

AI extensions use several overlapping formats. Agent Skills provide reusable instructions, MCP servers expose tools and data, DeepSeek Harness loads Cordis modules/npm packages, and client-specific plugin manifests package those capabilities for installation. Grok Build and Kimi Code each have native plugin manifests and runtime installers. Prefer open formats where practical, then add client adapters for the assistants you support.

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

### DeepSeek Harness Plugin Anatomy

DeepSeek Harness plugins export a Cordis `apply` function. Installable packages
declare a `dsh.bundle` entry in `package.json`; they do not need a
`.codex-plugin/plugin.json` file.

```ts
import type { Context } from '@deepseek-ai/cordis'

export const name = 'my-plugin'

export function apply(ctx: Context) {
  // Register services, tools, or UI contributions with ctx.
}
```

Install a published package or GitHub package through the DSH profile manager:

```bash
dsh plugin add <npm-package-or-github-spec>
```

### Grok Plugin Anatomy

Grok Build plugins can group skills, commands, agents, hooks, MCP servers, and
LSP configuration. A repository can describe the bundle with an optional
`.grok-plugin/plugin.json` manifest and can publish it through a Grok
marketplace catalog.

```text
my-plugin/
├── .grok-plugin/
│   └── plugin.json          # Optional native manifest
├── skills/                  # Optional Agent Skills
├── commands/                # Optional slash commands
├── agents/                  # Optional subagents
└── .mcp.json                # Optional MCP servers
```

Install a GitHub repository with:

```bash
grok plugin install owner/repo --trust
```

### Kimi Plugin Anatomy

Kimi Code plugins can expose skills, agents, and MCP servers. Current Kimi Code
plugins use `kimi.plugin.json`; earlier plugin bundles may use
`.kimi-plugin/plugin.json` or `plugin.json`. Follow the repository's manifest
and installation instructions.

```text
my-plugin/
├── kimi.plugin.json         # Current Kimi Code manifest
├── skills/                  # Optional skills
├── agents/                  # Optional agents
└── mcpServers/              # Optional MCP server definitions
```

Install a GitHub repository from Kimi Code with:

```text
/plugins install https://github.com/owner/repo
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

After scaffolding with `$plugin-creator`, use [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 510 | 🐛 43 | 🌐 Python | 📅 2026-08-31 as your quality gate before publishing, review, or distribution.

For skill/plugin authoring workflows, [Codex SkillForge](https://github.com/f0d010c/skillforge) ⭐ 0 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-23 provides an ESLint-style CLI and GitHub Action for scaffolding, linting, smoke-testing, and packaging Codex skills/plugins before publishing.

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

* [Awesome DeepSeek Harness Plugins](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) ⭐ 13,884 | 🐛 347 | 🌐 Python | 📅 2026-08-31 - Community-maintained DSH plugin list and discovery reference.
* [Kimi Code](https://github.com/MoonshotAI/kimi-code) ⭐ 7,180 | 🐛 1,252 | 🌐 TypeScript | 📅 2026-08-31 - Official Kimi Code runtime and plugin documentation.
* [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) ⭐ 869 | 🐛 26 | 🌐 Python | 📅 2026-08-31 - Codex-focused catalog that inspired this cross-platform list.
* [xAI Grok Plugin Marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 201 | 🐛 271 | 🌐 Python | 📅 2026-08-31 - Official Grok Build plugin marketplace and catalog format.
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

Every plugin in this list is automatically ingested by the [HOL Plugin Registry](https://hol.org/registry/plugins), which runs each through the [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 510 | 🐛 43 | 🌐 Python | 📅 2026-08-31 to produce a trust score and security analysis.

A snapshot of scored installable plugins (plus modeled Guard runtime fixtures and public advisories) is published on Hugging Face as [HOL Plugin Security](https://huggingface.co/datasets/HashgraphOnline/hol-plugin-security). Scan ≠ safety guarantee. Catalog plugin count is not the Registry Broker agent catalog. HOL publishes it; not independent validation.

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

1. Fork this repo and add a single line to the appropriate section in `README.md` (alphabetical order)
2. Submit a PR with the plugin repo URL. Scanner CI in the source repository is optional for listing and recommended for security.

**You do not need to copy plugin files into this repo.** A generator fetches your bundle from your source repo and regenerates catalog files automatically.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-31._
