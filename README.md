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

1. **Validate with [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 756 | 🐛 139 | 🌐 Python | 📅 2026-10-04** — recommended local preflight
2. **Add the [HOL scanner GitHub Action](https://github.com/hashgraph-online/ai-plugin-scanner-action) ⭐ 6 | 🐛 1 | 📅 2026-10-04** — recommended for security, optional for listing
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

* [mblode/agent-skills](https://github.com/mblode/agent-skills) ⭐ 141 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Nobody ships AI slop on purpose. These skills make sure you don't. UI audits, typography, docs, PR review, and releases.

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

* [Ponytail](https://github.com/DietrichGebert/ponytail) ⭐ 154,479 | 🐛 228 | 🌐 JavaScript | 📅 2026-10-03 - Guides coding agents toward minimal working solutions through YAGNI, existing code, standard libraries, and native platform features.
* [Claude Code Skills](https://github.com/alirezarezvani/claude-skills) ⭐ 27,572 | 🐛 27 | 🌐 Python | 📅 2026-08-30 - 223 production-ready skills, 23 agents, and 298 Python tools across 9 domains — engineering, marketing, product, compliance, and more.
* [Planning with Files](https://github.com/OthmanAdi/planning-with-files) ⭐ 27,277 | 🐛 10 | 🌐 Shell | 📅 2026-10-01 - Persistent file-based planning for Claude Code, Codex, and other AI coding agents, preserving task plans, findings, and progress across context loss, crashes, and compaction.
* [Screenpipe MCP](https://github.com/screenpipe/screenpipe) ⭐ 21,812 | 🐛 36 | 🌐 Rust | 📅 2026-10-04 - Gives agents searchable screen-text and audio history through MCP and a local API; source-available under the Screenpipe Commercial License, with configured cloud features able to send context off-device.
* [Browser Harness](https://github.com/browser-use/browser-harness) ⭐ 18,280 | 🐛 423 | 🌐 Python | 📅 2026-09-27 - MCP server and agent skill that connect an AI agent to a real browser through one editable CDP WebSocket.
* [Generative Media Skills](https://github.com/SamurAIGPT/Generative-Media-Skills) ⭐ 5,399 | 🐛 2 | 🌐 Python | 📅 2026-10-03 - 13 skills for image, video, and audio generation using 100+ models - FLUX, Midjourney v7, Veo3, Kling 3.0, Suno, and HunyuanVideo via muapi.ai.
* [avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) ⭐ 4,847 | 🐛 23 | 🌐 JavaScript | 📅 2026-10-04 - Portable agent skill for auditing and rewriting AI-patterned prose, with an optional local MCP detector that calls no model and sends no text to a network service.
* [Claude Octopus](https://github.com/nyldn/claude-octopus) ⭐ 4,147 | 🐛 6 | 🌐 Shell | 📅 2026-10-03 - Multi-LLM orchestration dispatching to 8 providers (Codex, Gemini, Copilot, Qwen, Perplexity, OpenRouter, Ollama, OpenCode) with Double Diamond workflows, adversarial review, and safety gates.
* [AI Video Transcriber](https://github.com/wendy7756/AI-Video-Transcriber) ⭐ 3,322 | 🐛 10 | 🌐 Python | 📅 2026-09-15 - Transcribe and summarize videos, podcasts, and local media via a Codex plugin, Claude Code skill, and MCP server.
* [zui](https://github.com/easysoft/zui) ⭐ 2,766 | 🐛 45 | 🌐 TypeScript | 📅 2026-10-04 - Codex skills that integrate the ZUI 3 web UI framework into existing projects and generate standalone ZUI-powered pages from plain briefs.
* [MegaLinter](https://github.com/oxsecurity/megalinter) ⭐ 2,610 | 🐛 65 | 🌐 Dockerfile | 📅 2026-10-04 - Set up, run and fix MegaLinter on any repository, covering 100+ linters and formatters for 69+ languages and 23+ formats, in CI or locally, with per-linter fix guides for the agent.
* [Better Harness](https://github.com/QoderAI/better-harness) ⭐ 2,360 | 🐛 15 | 🌐 JavaScript | 📅 2026-09-28 - Evidence-backed workflow analysis for coding agents that turns project and session signals into prioritized, verifiable improvements across supported hosts.
* [traceway](https://github.com/tracewayapp/traceway) ⭐ 1,596 | 🐛 30 | 🌐 Go | 📅 2026-10-04 - Agent skills that instrument repositories with Traceway OpenTelemetry monitoring and query production exceptions, logs, endpoints, and metrics.
* [mcp-server-kubernetes](https://github.com/Flux159/mcp-server-kubernetes) ⭐ 1,593 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-02 - MCP server for managing Kubernetes clusters via kubectl with tools for get, describe, apply, delete, logs, exec, port-forward, scaling, rollouts, Helm chart operations, and context switching.
* [agmsg](https://github.com/fujibee/agmsg) ⭐ 1,539 | 🐛 338 | 🌐 Shell | 📅 2026-10-04 - Cross-vendor messaging for CLI coding agents (Claude Code, Codex, Gemini CLI, Grok): sessions join a team by name and hand work to each other through a shared local SQLite file, with durable history and ext-tool members that let a program such as Slack or Jev join like any agent.
* [Brooks Lint](https://github.com/hyhmrright/brooks-lint) ⭐ 1,503 | 🐛 0 | 🌐 HTML | 📅 2026-09-28 - AI code reviews grounded in six classic engineering books — decay risk diagnostics with book citations, severity labels, and four analysis modes (PR review, architecture audit, tech debt, test quality).
* [pm-claude-skills](https://github.com/mohitagw15856/pm-claude-skills) ⭐ 1,421 | 🐛 3 | 🌐 HTML | 📅 2026-10-04 - Open-source library of 1174 plain-markdown agent skills for Claude Code, Codex, Gemini, and Cursor, covering professional and life tasks with built-in quality checks and anti-patterns.
* [Antigravity Workspace Template](https://github.com/study8677/antigravity-workspace-template) ⭐ 1,325 | 🐛 6 | 🌐 Python | 📅 2026-09-09 - Multi-agent codebase knowledge graph generator with context-aware planning and automatic scope management — turns codebases into coherent agent workspaces.
* [Aegis](https://github.com/GanyuanRan/Aegis) ⭐ 1,319 | 🐛 4 | 🌐 Python | 📅 2026-10-03 - An agentic skills framework & software development methodology that works: planning, TDD, debugging, and collaboration workflows.
* [Awesome-Journal-Skills](https://github.com/brycewang-stanford/Awesome-Journal-Skills) ⭐ 1,208 | 🐛 2 | 🌐 Stata | 📅 2026-09-27 - Claude Code plugin marketplace (also usable as Codex skills) of 300 journal- and conference-specific packs covering topic fit, house style, submission rules, and reviewer response for 744 venues across economics, social science, natural science, medicine, and computer science.
* [StyleSeed](https://github.com/bitjaru/styleseed) ⭐ 967 | 🐛 10 | 🌐 JavaScript | 📅 2026-10-01 - Compiles your project's design decisions into a lock file, then enforces them on Claude Code, Codex, and Cursor output with code and rendered-pixel gates so screens stay consistent across sessions.
* [spec-superflow](https://github.com/MageByte-Zero/spec-superflow) ⭐ 837 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-01 - Spec-first workflow with nine skills, user-controlled Quick / Hotfix / Tweak / Full paths, auditable recovery commands, hardened delta-spec sync, and guarded review gates.
* [claude-council](https://github.com/hex/claude-council) ⭐ 827 | 🐛 1 | 🌐 Shell | 📅 2026-10-01 - Claude Code plugin that asks Gemini, OpenAI, Grok, Perplexity, Kimi, OpenRouter models, the Codex, Cursor, Grok and Kimi CLIs and a local ollama model the same question in parallel and lines the answers up with a synthesis of where they agree and differ.
* [Boss](https://github.com/echoVic/boss-skill) ⭐ 563 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-04 - BMAD pipeline plugin that orchestrates a full requirements-to-deploy workflow across nine specialist agents with an auditable runtime DAG and quality gates, for Claude Code, Codex, OpenClaw, and Antigravity.
* [token-optimizer](https://github.com/ooples/token-optimizer-mcp) ⭐ 538 | 🐛 17 | 🌐 JavaScript | 📅 2026-10-04 - Spend less context and keep the conclusions across 16 coding clients including Claude Code, Codex, Gemini CLI, Cursor, and Copilot — diff-only re-reads, paths-only search, out-of-context stashing, and a local ledger that measures each tool's actual return.
* [OpenCode Power Pack](https://github.com/waybarrios/opencode-power-pack) ⭐ 531 | 🐛 3 | 🌐 Python | 📅 2026-09-30 - Fifty-four portable development and security workflows for Codex, Claude Code, OpenCode, and Pi, with opt-in native sandbox profiles for safer command execution.
* [Codex Multi Auth](https://github.com/ndycode/codex-multi-auth) ⭐ 529 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-03 - Multi-account OAuth manager for the official Codex CLI with switching, health checks, and recovery tools.
* [MisakaNet](https://github.com/Ikalus1988/MisakaNet) ⭐ 521 | 🐛 169 | 🌐 Python | 📅 2026-10-04 - Git-backed failure-memory for AI coding agents with 290 indexed lessons, MCP server with 5 tools (search, get\_lesson, submit\_usage, submit\_intake, usage\_status), and DeepSeekHarness adapter.
* [de-anthropocentric-research-engine](https://github.com/yogsoth-ai/de-anthropocentric-research-engine) ⭐ 504 | 🐛 1 | 📅 2026-09-29 - Collection of 900+ markdown research skills that let Claude Code autonomously survey literature, find gaps, form hypotheses, and design experiments.
* [Jev MCP](https://github.com/jkudish/jev-mcp) ⭐ 492 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Fast, sub-cent typed judgments for agents, such as verifying claims against evidence, screening content for prompt injection before it enters context, and ranking candidates by meaning, each with probabilities and confidence in milliseconds.
* [AgentOps](https://github.com/boshu2/agentops) ⭐ 447 | 🐛 1 | 🌐 Go | 📅 2026-10-04 - DevOps layer for coding agents with flow, feedback, and memory that compounds between sessions.
* [Skillstore](https://github.com/aiskillstore/marketplace) ⭐ 430 | 🐛 11 | 🌐 Python | 📅 2026-10-04 - Security-audited Agent Skills marketplace with one-command installation for Claude Code and Codex via the skillstore CLI.
* [dryforge](https://github.com/prekuter/dryforge) ⭐ 396 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Intent to implementation: ready, then go.
* [AgentBridge](https://github.com/raysonmeng/agent-bridge) ⭐ 370 | 🐛 49 | 🌐 TypeScript | 📅 2026-10-03 - Local bidirectional bridge that keeps Claude Code and Codex live as peers in one session, with mid-turn injection and quota-window handoff.
* [genie](https://github.com/automagik-dev/genie) ⭐ 345 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-04 - Agent skills and CLI that interview a wish into a plan, dispatch parallel subagents, and review results against acceptance criteria.
* [AREX-Skill](https://github.com/VectorSpaceLab/AREX-Skill) ⭐ 328 | 🐛 1 | 🌐 Python | 📅 2026-09-03 - A library of 5,000+ verified, executable skills distilled from ML repositories for coding and research agents.
* [Audio Plugin Coder](https://github.com/Noizefield/audio-plugin-coder) ⭐ 327 | 🐛 0 | 🌐 HTML | 📅 2026-10-04 - Agent-agnostic JUCE workflow for building VST3/AU plugins from idea through design, implementation, test, and installer packaging.
* [Jev Browser](https://github.com/jkudish/jev-browser) ⭐ 307 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-02 - Fast, very cheap browser use for agents: Jev picks every action, code owns the loop, and you get the final page, an auditable step trace, console errors, and a screenshot; MCP server, CLI, or library.
* [Reviewable HTML Workbench](https://github.com/u-ichi/reviewable-html-workbench) ⭐ 298 | 🐛 4 | 🌐 Python | 📅 2026-09-10 - Generate reviewable HTML documents, serve previews, collect inline review comments, and feed review outcomes back into agent workflows.
* [Emulo](https://github.com/ohad6k/emulo) ⭐ 293 | 🐛 16 | 🌐 HTML | 📅 2026-10-02 - Mines selected evidence from local coding-agent sessions into private work, design, and writing profiles for Codex, Claude Code, and GitHub Copilot.
* [Spellbook](https://github.com/majiayu000/spellbook) ⭐ 287 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Cross-runtime library of 108 agent skills installable into Claude Code and Codex via one command.
* [DataMagic](https://github.com/HKUSTDial/DataMagic) ⭐ 282 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-02 - A skill that teaches coding agents to plan and render narrated animated data videos from tabular data using DVSpec.
* [OpenCode Orchestrator](https://github.com/agnusdei1207/opencode-orchestrator) ⭐ 264 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-04 - Multi-agent mission control for OpenCode with Commander, Planner, Worker, and Reviewer workflows.
* [Knowledge Manager](https://github.com/treylom/knowledge-manager) ⭐ 244 | 🐛 0 | 🌐 Python | 📅 2026-09-28 - Extracts and organizes content from web pages, files, Notion, and images into an Obsidian knowledge vault with GraphRAG-backed search, exporting to Notion, Markdown, and PDF.
* [Claude Code for Codex](https://github.com/sendbird/cc-plugin-codex) ⭐ 218 | 🐛 15 | 🌐 JavaScript | 📅 2026-09-28 - Reverse of OpenAI's official Claude-hosted plugin: use Claude Code from Codex for reviews, rescue tasks, tracked background jobs, and hook-powered review gates.
* [Oh My Design](https://github.com/3x-haust/oh-my-design) ⭐ 198 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-29 - Evidence-backed design workflow for Claude Code and Codex with reference research, multi-agent reviews, visual QA, and anti-slop guardrails.
* [lattice](https://github.com/techygarg/lattice) ⭐ 197 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-07 - Composable AI skills framework that infuses clean code, clean architecture, domain-driven design, secure coding, and proper testing into the workflow by default, with scenario-driven guides for getting started, customization, and team use.
* [ab-method](https://github.com/ayoubben18/ab-method) ⭐ 192 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-01 - A skill and workflow plugin for Claude Code and Codex that grills problems into plans and drives test-driven missions with critic reviews.
* [claude-remember](https://github.com/Digital-Process-Tools/claude-remember) ⭐ 192 | 🐛 20 | 🌐 Python | 📅 2026-10-04 - Persistent memory for Claude Code with identity, context, and continuity carried across sessions.
* [agent-talk](https://github.com/xhluca/agent-talk) ⭐ 189 | 🐛 2 | 🌐 Python | 📅 2026-09-10 - Skills-based plugin built on the retalk CLI that gives coding agents end-to-end encrypted messaging with other agents, including agents run by other people, across Claude Code, Codex, Antigravity, pi, opencode, and GitHub Copilot CLI.
* [trace-mcp](https://github.com/nikolai-vysotskyi/trace-mcp) ⭐ 185 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-04 - Precomputed code-intelligence graph served over MCP — symbol search, call graphs, change impact, and test mapping as structured answers instead of whole-file reads.
* [keep-the-why](https://github.com/oliver-zehentleitner/keep-the-why) ⭐ 177 | 🐛 1 | 🌐 Python | 📅 2026-10-04 - Preserves the reasoning behind a codebase as project memory — decisions, rejected alternatives, workarounds, incident learnings, constraints.
* [codex-profiles](https://github.com/Ducksss/codex-profiles) ⭐ 175 | 🐛 2 | 🌐 Shell | 📅 2026-10-03 - Switch Codex CLI and Desktop accounts with isolated `CODEX_HOME` profile directories instead of copying token files.
* [opencode-models-discovery](https://github.com/yuhp/opencode-models-discovery) ⭐ 167 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-02 - OpenCode plugin that dynamically discovers models from OpenAI-compatible providers and injects them into provider config with filtering and metadata enrichment.
* [claude-dnd-skill](https://github.com/neuralinitiative/claude-dnd-skill) ⭐ 164 | 🐛 4 | 🌐 Python | 📅 2026-09-16 - Unofficial D\&D 5e Dungeon Master for Claude Code with persistent campaigns, full 5e rules mechanics, and an optional cinematic display companion for a TV.
* [opencode-synced](https://github.com/iHildy/opencode-synced) ⭐ 157 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-23 - OpenCode plugin that syncs global configuration and skills across machines via Git, with optional sessions and secrets for private repositories.
* [ContextPilot](https://github.com/EfficientContext/ContextPilot) ⭐ 139 | 🐛 15 | 🌐 Python | 📅 2026-10-02 - Context optimization engine that reorders and deduplicates context blocks to raise cache hits, shipping as plugins for OpenClaw and Hermes.
* [Krypton](https://github.com/jturntdev/krypton) ⭐ 132 | 🐛 2 | 🌐 Shell | 📅 2026-07-24 - Goal-based planning and proof gate for Codex and Claude Code that turns requests into ownership, cutover, review-gate, and acceptance-evidence plans.
* [humanizer-ru](https://github.com/Vladimir-Human/humanizer-ru) ⭐ 126 | 🐛 3 | 🌐 Python | 📅 2026-10-02 - Deterministic offline diagnostics and safe cleanup of chat-interface copy-paste artifacts in Russian text and Markdown, shipped as an Agent Skill, MCP server, CLI, GitHub Action, and browser demo, with no authorship verdicts.
* [Suede Creator Skills](https://github.com/JasonColapietro/suede-creator-skills) ⭐ 126 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-04 - An open-source Agent Skills pack for Claude Code and Codex covering multi-agent workflows, code review, design, copy, SEO, app shipping, creator-rights workflows, and local read-only MCP discovery.
* [Knowl](https://github.com/dat999zx/knowl) ⭐ 124 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-30 - Local-first project memory over MCP for Claude Code, Codex, Cursor and eight other hosts: a SQLite store that retires facts when they change, shares knowledge across linked repos, and retrieves it by hybrid search.
* [Janus](https://github.com/RamitVishwakarma/Janus) ⭐ 123 | 🐛 3 | 🌐 Swift | 📅 2026-09-28 - macOS menu bar app that saves each Claude Code account's session so switching between accounts is one click, and reclaims disk space by measuring developer caches and moving them to the Trash.
* [jevmem](https://github.com/Avinash-jetwani/jevmem) ⭐ 117 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-04 - Plugin and MCP server that automatically saves project decisions, rules and dead ends to a JEVMEM.md file and recalls them in later sessions.
* [orchflows](https://github.com/DanMcInerney/orchflows) ⭐ 117 | 🐛 1 | 🌐 Python | 📅 2026-10-04 - Use 2 simple skills to build complex, composable workflows for task-specific jobs.
* [dsh-whale-musume](https://github.com/Sutera-Diffusus/dsh-whale-musume) ⭐ 112 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-04 - Whale-girl desktop pet for the DSH Web UI with pat-to-raise growth, work-state poses, 494 dialogue lines, 30 achievements and a built-in settings panel; local-first, zero telemetry.
* [Superloopy](https://github.com/beefiker/superloopy) ⭐ 111 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-30 - Evidence-gated Codex loop harness with specialist skills, including near-pixel authorized website cloning backed by screenshots, assets, build output, and visual QA.
* [2718lab DevKit](https://github.com/2718labs/2718lab-devkit) ⭐ 99 | 🐛 3 | 🌐 Python | 📅 2026-10-04 - Codex-first local MCP server and skill bundle for deterministic project intelligence, durable workflow orchestration, and reusable engineering tools.
* [Coordinate Agents](https://github.com/hogancv/coordinate-agents) ⭐ 99 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-03 - Plugin-first multi-agent coordination tool with a local-first, recoverable Agent Bus and human-gated planning, implementation, review, and release workflows.
* [otelyssey](https://github.com/using-system/otelyssey) ⭐ 99 | 🐛 3 | 🌐 Python | 📅 2026-10-04 - Marketplace of OpenTelemetry agent plugins (instrumentation, Collector, backends, observability) for Claude Code, Copilot CLI, Codex, Grok Build and more, run by the repository itself: submit a plugin.json URL, it validates, reviews, lists and follows releases.
* [sci-brain](https://github.com/QuantumBFS/sci-brain) ⭐ 98 | 🐛 5 | 🌐 Python | 📅 2026-09-25 - Research skills plugin for Claude Code, Codex, OpenCode, and pi that surveys literature into a citable knowledge base, brainstorms research ideas, and drafts papers and slides.
* [FlowBoard](https://github.com/rasimme/FlowBoard) ⭐ 96 | 🐛 5 | 🌐 JavaScript | 📅 2026-09-25 - Local-first project workspace and task-coordination plugin for OpenClaw and external coding agents, with lazy-loaded context and a shared Kanban board.
* [opencode-see-image](https://github.com/alfaoz/opencode-see-image) ⭐ 90 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-27 - OpenCode plugin that gives non-vision models image and screenshot understanding by routing attachments to a vision-capable model.
* [forgecat-agent-profiles](https://github.com/nota-america/forgecat-agent-profiles) ⭐ 89 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-23 - Catalog of 191 cross-platform agent profiles installable via the ForgeCat CLI into Claude Code, Cursor, Codex, OpenClaw, and Hermes Agent.
* [Codex Attachment Manager](https://github.com/chipfighter/codex-attachment-manager) ⭐ 88 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-29 - Codex plugin that lets users pick which past images are resent to the model, replacing unchecked ones with placeholders to shrink requests.
* [Vibe Prospecting](https://github.com/explorium-ai/vibeprospecting-plugin) ⭐ 88 | 🐛 4 | 🌐 Shell | 📅 2026-10-04 - Live B2B company and contact intelligence for building lead lists, researching prospects, enriching contacts, and personalizing outreach.
* [Dely](https://github.com/hieuphung97/dely) ⭐ 86 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - Multi-harness control protocol that turns requests into approved design contracts, orchestrating isolated worker sessions for sequential implementation and independent code reviews under Orca supervision for Claude Code, Codex, Cursor, Antigravity, and other AI coding agents.
* [Gangsta Agents](https://github.com/kucherenko/gangsta) ⭐ 85 | 🐛 1 | 🌐 Shell | 📅 2026-08-14 - Agent skills providing a spec-driven development pipeline with reconnaissance, adversarial debate, TDD execution, and verification phases for Claude Code, Codex, Cursor, OpenCode, and Gemini CLI.
* [MCP Video Analyzer](https://github.com/guimatheus92/mcp-video-analyzer) ⭐ 85 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-04 - Gives agents video input: transcript, key frames, OCR text, metadata, and an annotated timeline from Loom, YouTube, Instagram, TikTok, direct URLs, or a local file, over MCP, a one-shot CLI, or the /video skill.
* [BanyanCode](https://github.com/EkagraAgarwal/BanyanCode) ⭐ 82 | 🐛 10 | 🌐 TypeScript | 📅 2026-10-04 - Terminal coding agent with parallel subagents, cross-session memory, Tree-sitter code graph, and free web research.
* [opencode-litellm](https://github.com/yuseferi/opencode-litellm) ⭐ 82 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-30 - OpenCode plugin that auto-detects a LiteLLM proxy and dynamically registers its models in the OpenCode picker.
* [pstack for Codex](https://github.com/Aqua-123/pstack-for-codex) ⭐ 81 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-02 - Codex-native engineering workflows derived from pstack, with 45 explicit skills and 23 Poteto Mode playbooks.
* [opencode-skills-collection](https://github.com/FrancoStino/opencode-skills-collection) ⭐ 80 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - OpenCode plugin that bundles 1595+ skills and auto-syncs them locally, loading each on demand via pointer files.
* [Sealos](https://github.com/labring/sealos-skills) ⭐ 80 | 🐛 8 | 🌐 Python | 📅 2026-09-28 - Deploy apps to Sealos Cloud from Codex with readiness checks, Dockerfile generation, Compose conversion, image builds, and rollout updates.
* [taskflow](https://github.com/heggria/taskflow) ⭐ 76 | 🐛 19 | 🌐 TypeScript | 📅 2026-10-03 - Declarative, verifiable DAG orchestration for Grok Build subagents — fan-out, gates, loops, tournaments, approvals, and resumable runs via MCP tools, with intermediate transcripts kept out of context.
* [AI-Native SDLC](https://github.com/bashebr/ai-native-sdlc) ⭐ 73 | 🐛 0 | 🌐 Python | 📅 2026-09-11 - Reusable skill and plugin bundle implementing the AI-native SDLC workflow: plan, design, build, test, deploy, and maintain with human approval gates.
* [claude-image-gen](https://github.com/guinacio/claude-image-gen) ⭐ 71 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-08 - AI-powered image generation using Google Gemini or OpenAI (gpt-image-2), integrated with Claude Code via Skills or Claude.ai via MCP.
* [Mycelium](https://github.com/arjunrajlaboratory/mycelium) ⭐ 69 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Gives Claude Code and Codex analytical repositories durable memory for decisions, findings, provenance, reusable conventions, and analysis workflows.
* [skillsaw](https://github.com/stbenjam/skillsaw) ⭐ 68 | 🐛 3 | 🌐 Python | 📅 2026-10-02 - A configurable linter for agent skills, plugins, and AI coding assistant context.
* [Craft](https://github.com/drobins25/craft) ⭐ 67 | 🐛 1 | 🌐 Shell | 📅 2026-10-03 - A Claude Code plugin that acts as an intelligent harness for your development workflow: your codebase is read-only by default, every change passes through a Write Gate as planned and approved work, and craft tracks your project's history, design tokens, and decisions locally so Claude learns your taste and architectural preferences over time.
* [Archcore](https://github.com/archcore-ai/archcore) ⭐ 66 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-04 - Spec-driven development and context engineering for Claude Code, Cursor, Codex, and GitHub Copilot — backed by project context in Git.
* [session-handoff](https://github.com/yuzushi-dev/session-handoff) ⭐ 66 | 🐛 1 | 🌐 Python | 📅 2026-10-02 - Create handoffs and migrate sessions between Claude Code and Codex.
* [Globalping](https://github.com/jsdelivr/globalping-mcp-server) ⭐ 64 | 🐛 10 | 🌐 TypeScript | 📅 2026-09-04 - Access thousands of probes around the world to run network tests such as ping, traceroute, http, dns and mtr.
* [silica](https://github.com/kiycoh/silica-harness) ⭐ 64 | 🐛 0 | 🌐 Python | 📅 2026-09-17 - Serves an Obsidian vault as the agent's memory over MCP: semantic and literal recall, gated note writing, and hooks that open each session already knowing its vault.
* [YYLO](https://github.com/yylo-dev/yylo) ⭐ 63 | 🐛 11 | 🌐 Python | 📅 2026-10-03 - Command-line orchestrator for coding agents that creates a dedicated branch/worktree per task, delegates to Pi and Codex subagents, and enforces typed task, validation, merge, and release-readiness boundaries with receipt-backed repository changes.
* [mstar-harness](https://github.com/btspoony/mstar-harness) ⭐ 62 | 🐛 16 | 🌐 TypeScript | 📅 2026-10-04 - Multi-agent code harness plugin that routes work through PM, dev, QC, and QA roles with deterministic workflow gates enforced by a TypeScript engine, installable across dsh, omp, OpenCode, Cursor, Kimi Code, ZCode, and Codex.
* [Blender Agent Studio](https://github.com/ifBars/blender-agent-studio) ⭐ 61 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-04 - Codex plugin with specialist skills and a local MCP server for building, inspecting, validating, and rendering Blender scenes, plus browser handoffs for Mixamo motion and Pixabay sound effects.
* [Festival](https://github.com/Obedience-Corp/festival) ⭐ 58 | 🐛 4 | 🌐 Shell | 📅 2026-10-03 - Planning and persistent context tools that let coding agents execute multi-phase goals across sessions using files and Git.
* [FlexViz](https://github.com/flex-analytics/flexviz) ⭐ 58 | 🐛 50 | 🌐 Python | 📅 2026-10-04 - Interactive cross-filter dashboards for large datasets with a Claude Code skill for agent-driven data exploration.
* [mcp-local-memory](https://github.com/Beledarian/mcp-local-memory) ⭐ 56 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-14 - A lightweight, powerful local memory server for AI agents supporting text, entities, relations, and time-based recall.
* [WorkFlowX](https://github.com/TreeX-X/WorkFlowX) ⭐ 54 | 🐛 1 | 🌐 HTML | 📅 2026-09-27 - Multi-agent orchestration plugin for Claude Code and Codex that structures planning, coding, and independent evaluation of development tasks.
* [Session Orchestrator](https://github.com/Kanevry/session-orchestrator) ⭐ 53 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-03 - Session orchestration for Claude Code, Codex, and Cursor IDE — structured planning, wave-based execution, VCS integration (GitLab + GitHub), quality gates, and clean session close-out with issue tracking.
* [Honcho](https://github.com/plastic-labs/codex-honcho) ⭐ 52 | 🐛 16 | 🌐 TypeScript | 📅 2026-09-01 - Persistent cross-session memory for Codex powered by Honcho — lifecycle hooks capture each session and inject relevant context back at session start, so Codex remembers your preferences, projects, and decisions across restarts.
* [Knowledge Loom](https://github.com/magickaichen/knowledge-loom) ⭐ 52 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-30 - Agent-neutral skills for initializing, auditing, using, and maintaining governed local Markdown knowledge vaults across Agent Skills-compatible runtimes.
* [web-ai-agent-skills](https://github.com/webmaxru/web-ai-agent-skills) ⭐ 52 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-29 - Agent skills that guide coding agents through integrating browser Web AI APIs: Prompt API, Translator, Language Detector, Proofreader, WebMCP, and WebNN.
* [OpenSea Skills](https://github.com/ProjectOpenSea/opensea-skill) ⭐ 51 | 🐛 0 | 🌐 Shell | 📅 2026-09-30 - Five Agent Skills for OpenSea data, Seaport trading, ERC20 swaps, wallet signing, and ERC-8257 tool development.
* [kitbash](https://github.com/Open-Dev-Society/kitbash) ⭐ 50 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-27 - Breaks an idea into components and classifies each one as BORROW, KITBASH, or WRITE, checking every repo it names against the live GitHub API so invented ones never reach you; ships as a skill, plugin, and MCP server.
* [memi](https://github.com/sarveshsea/memi) ⭐ 47 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-29 - Interface understanding and design-system memory for Codex, Claude Code, Cursor, and MCP agents with UI audits, Tailwind token extraction, shadcn registry workflows, and a bundled Codex plugin.
* [Open PR](https://github.com/TOMOSIA-VIETNAM/open-pr) ⭐ 46 | 🐛 4 | 🌐 Python | 📅 2026-10-04 - AI code review that lands on the pull request itself across GitHub, GitLab, and Bitbucket, learning each repo's conventions to post one review, one fix commit, and in-thread replies from Claude Code, Cursor, Codex, Gemini CLI, or Antigravity.
* [Designer Skill](https://github.com/PyModel/designer-skill) ⭐ 45 | 🐛 6 | 🌐 JavaScript | 📅 2026-09-30 - Plug-and-play MCP that gives your coding agent UI superpowers: design references, intent routing and a static anti-slop gate, no API key.
* [jev-use](https://github.com/shitianfang/jev-use) ⭐ 45 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-22 - Hands the agent steps that need no text output to Jev's judgment model across Claude Code, Codex, and Pi, returning everything it should not decide to the LLM under a typed escalation contract.
* [Jevbridge](https://github.com/tacticocc/Jevbridge) ⭐ 45 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-21 - OSS ACP/MCP adapter that bridges TypeSafe Jev with any LLM, putting computer use and typed decisions alongside Codex, Claude, Grok, and OpenCode without replacing those hosts.
* [Rootly MCP Server](https://github.com/rootlyhq/rootly-mcp-server) ⭐ 45 | 🐛 9 | 🌐 Python | 📅 2026-10-02 - Manage and resolve production incidents from MCP-compatible AI assistants through dynamically generated, access-controlled Rootly API tools.
* [Waggle](https://github.com/Abhigyan-Shekhar/Waggle-mcp) ⭐ 44 | 🐛 207 | 🌐 Python | 📅 2026-10-02 - Persistent graph-backed conversational memory for Codex that recalls project decisions, constraints, preferences, and outcomes across sessions.
* [Groundwork](https://github.com/etr/groundwork) ⭐ 43 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-15 - Comprehensive skills library for Claude Code and Codex that structures discovery, planning, design, TDD, debugging, validation, collaboration, and shipping.
* [Docflow](https://github.com/MedAdemBHA/docflow) ⭐ 42 | 🐛 0 | 🌐 Shell | 📅 2026-08-15 - Lightweight documentation memory for AI coding agents that scaffolds a 7-category docs tree, runs readiness checks, validates docs before finishing, and keeps a monthly changelog across Claude Code and Codex.
* [Codebase Recon](https://github.com/yujiachen-y/codebase-recon-skill) ⭐ 41 | 🐛 0 | 📅 2026-04-26 - Analyze git history to understand a codebase before reading any code — auto-scales by repo size and cross-references hotspots with bug magnets to surface high-risk files, bus factor, and team momentum.
* [iris-agentic-dev](https://github.com/intersystems-community/iris-agentic-dev) ⭐ 41 | 🐛 10 | 🌐 Rust | 📅 2026-10-01 - MCP server giving AI assistants live access to InterSystems IRIS — execute ObjectScript, query globals, inspect productions, run tests, search code, and manage skills.
* [Open Dynamic Workflows](https://github.com/Suraj1235/open-dynamic-workflows) ⭐ 41 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-09 - Local-first MIT dynamic multi-agent workflows for Codex, OpenCode, Antigravity, Cursor, and VS Code with a daemon, MCP bridge, Codex skills, OpenCode plugin, and bring-your-own-model support.
* [Click](https://github.com/grapefruit0205/click) ⭐ 40 | 🐛 6 | 🌐 Python | 📅 2026-10-02 - Record revision-aware evidence for normal Codex work and optionally bind higher-risk execution to one human-readable approval contract.
* [opencode-openai-compact](https://github.com/partment/opencode-openai-compact) ⭐ 40 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-04 - OpenCode plugin that uses OpenAI Responses API native compaction v2 and stores checkpoints in SQLite.
* [JevScout](https://github.com/hqman/JevScout) ⭐ 39 | 🐛 1 | 🌐 Python | 📅 2026-09-18 - Autonomous job hunt orchestrator powered by TypeSafe Jev and Chrome DevTools Protocol to discover and evaluate AI engineering roles.
* [Labtasker](https://github.com/luocfprime/labtasker) ⭐ 38 | 🐛 1 | 🌐 Python | 📅 2026-10-02 - Queue and run independent ML inference, evaluation, and experiment tasks across long-lived Python or command workers with a Claude Code plugin and cross-agent skill.
* [Quality Engineering Skills](https://github.com/RBraga01/Quality-Engineering-Skills) ⭐ 38 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-02 - 22 structured quality engineering skills for automotive and manufacturing: ISO 9001, IATF 16949, AIAG-VDA FMEA, VDA 6.3, PPAP, APQP, SPC, MSA.
* [UIZZE](https://github.com/uizze/uizze) ⭐ 38 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-03 - Free MIT anti-ui-slop Skill with a product-specific design contract, required UI states, and a hard finish gate; full UIZZE adds live reference search, validation, and audits across 800,000+ real web and iOS screens through its authenticated MCP server at <https://uizze.com/mcp>.
* [Velith](https://github.com/epicsagas/Velith) ⭐ 37 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-30 - AI-native publishing system with a 6-phase pipeline from ideation to EPUB/PDF across 8 genres.
* [super-token-saver](https://github.com/ww-w-ai/super-token-saver) ⭐ 34 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-30 - Cuts Claude Code and Codex token spend with prompt-cache expiry warnings, zero-cost session restore after compaction, and per-model usage and cost reports.
* [Jump Skills](https://github.com/fabricioctelles/jump-skills) ⭐ 32 | 🐛 1 | 🌐 Shell | 📅 2026-10-04 - Meta-skills that route requests to specialized skills across Claude Code, Codex, Cursor, OpenCode, and other agent hosts.
* [Agent Guard](https://github.com/JeongJaeSoon/agent-guard) ⭐ 31 | 🐛 3 | 🌐 Shell | 📅 2026-10-04 - Real-time secret-leak guardrails for AI coding agents (Claude Code, Codex), Git hooks, and CI.
* [BioNexus](https://github.com/HERRY423/BioNexus) ⭐ 31 | 🐛 12 | 🌐 Python | 📅 2026-09-25 - Warrant-first scientific reliability layer for AI bioinformatics that audits analytical assumptions, calibrates evidence strength, caps unsupported claims, and verifies execution provenance.
* [harness-eval](https://github.com/redhat-community-ai-tools/harness-eval) ⭐ 31 | 🐛 4 | 🌐 Python | 📅 2026-10-04 - Linter tool (static analysis rules) and LLM reviewer for AI agent harness files that runs quality and security health checks, catching cross-component security chains, redundancy, and config drift, and vets individual skills before install, across Claude Code, Cursor, Codex, Copilot, Gemini, and OpenCode.
* [Harness Kit](https://github.com/romabeckman/harness-kit) ⭐ 30 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-30 - Agentic development harness for orchestrating specification, implementation, review, and telemetry across multiple AI coding assistants.
* [Agent Context OS](https://github.com/conorbronsdon/agent-context-os) ⭐ 29 | 🐛 7 | 🌐 Python | 📅 2026-09-30 - Portable Git-backed context and session workflow layer with first-class Claude Code, Codex, and OpenClaw support plus experimental adapters for Hermes, Cursor, and Devin.
* [Hera Agent Unity](https://github.com/NotNull92/hera-agent-unity) ⭐ 29 | 🐛 1 | 🌐 C# | 📅 2026-08-19 - Controls and verifies a live Unity Editor through a low-token CLI, with scene, asset, Inspector, Play Mode, test, screenshot, and runtime C# workflows for Codex and other coding agents.
* [Stark](https://github.com/f0d010c/stark) ⭐ 29 | 🐛 3 | 🌐 Python | 📅 2026-07-26 - UI/UX design plugin for AI coding agents with product-flow routing, platform-native interface guidance, asset planning, and shipped-reference analysis before code.
* [NixKits](https://github.com/Kihara777/NixKits) ⭐ 28 | 🐛 0 | 🌐 Nix | 📅 2026-10-04 - Declarative Nix flake collection that keeps coding-agent packages and NixOS modules updated and reproducible, with maintenance skills covering upstream version checks, NixOS CLI usage, config recovery, and multilingual project docs.
* [geml](https://github.com/geml-spec/geml) ⭐ 27 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-04 - An agent-native markup language featuring deterministic block-level editing and built-in validation to ensure documents never drift or break during AI operations.
* [HOTL Plugin](https://github.com/yimwoo/hotl-plugin) ⭐ 27 | 🐛 1 | 🌐 Shell | 📅 2026-07-06 - Human-on-the-Loop AI coding workflow plugin for Codex, Claude Code, and Cline with structured planning, review, and verification guardrails.
* [ThumbGate](https://github.com/IgorGanapolsky/ThumbGate) ⭐ 27 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-02 - Pre-action infrastructure firewall for AI coding agents: feedback becomes lessons and prevention rules enforced by PreToolUse hooks across Claude Code, Codex, Gemini, and MCP.
* [VibePortrait](https://github.com/dadwadw233/VibePortrait) ⭐ 27 | 🐛 2 | 🌐 HTML | 📅 2026-04-08 - Developer personality portrait generator — analyzes AI conversation history to produce MBTI type (16 color themes), capability radar, developer rating, 3-dimension famous match, and a persona skill that lets any AI "think like you".
* [claude-supertool](https://github.com/Digital-Process-Tools/claude-supertool) ⭐ 26 | 🐛 20 | 🌐 Python | 📅 2026-10-04 - Batches file, git and tracker operations into one round-trip, collapsing many reads, greps and globs into a single call for fewer output tokens and less wall time.
* [Pixel](https://github.com/Pixel-CLI/pixel) ⭐ 26 | 🐛 38 | 🌐 Rust | 📅 2026-10-04 - Local, deterministic code index that Claude Code, Codex, Pi, OpenCode and other coding agents query for signatures, callers, impact and Git history instead of reading whole files.
* [Rider Skills](https://github.com/JetBrains/rider-skills) ⭐ 26 | 🐛 0 | 📅 2026-10-02 - Official JetBrains Rider agent skills that let AI coding agents use the IDE's semantic code understanding, refactoring, debugger, and test tooling in .NET and Unreal Engine projects.
* [AgentPack](https://github.com/vishal2612200/agentpack) ⭐ 25 | 🐛 19 | 🌐 Python | 📅 2026-09-27 - Ranks repo context for Codex with likely files, skill recommendations, agent rules, commands, warnings, and compact task-focused packs before editing.
* [harmonyos-skills](https://github.com/liasica/harmonyos-skills) ⭐ 25 | 🐛 0 | 🌐 Python | 📅 2026-10-03 - Offline mirror of 16,800+ HarmonyOS NEXT official docs packaged as a Codex / Claude Code skill and MCP server, so AI coding assistants answer ArkTS / ArkUI / API questions with cited sources.
* [Frappe Agent](https://github.com/Dkm0315/frappe-agent) ⭐ 24 | 🐛 3 | 📅 2026-10-04 - Frappe and ERPNext coding, customization, bench, and review intelligence for Codex.
* [i-hate-editing](https://github.com/ranahaani/i-hate-editing) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Claude Code skill that turns raw talking-head footage into a finished cut with local whisper.cpp + ffmpeg (model never watches the pixels).
* [Rel.AI MCP](https://github.com/Kyne0328/rel-ai-mcp) ⭐ 24 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-04 - Brings Codex-style coding workflows to ChatGPT Web, connecting it to local development workspaces through MCP while using ChatGPT Web quota instead of Codex quota.
* [Vanguard Frontier Agentic](https://github.com/VincentChuWaiChow/vanguard-frontier-agentic) ⭐ 24 | 🐛 0 | 🌐 Rust | 📅 2026-09-30 - Multi-harness marketplace of skills, specialist agents, rules, and MCP references for guarded cloud, platform, compliance, and business workflows.
* [Web Search MCP](https://github.com/sydasif/web-search-mcp) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Comprehensive FastMCP server giving LLMs real-time web access across search engines (DuckDuckGo, Exa), social platforms (Reddit, Hacker News, GitHub, X, LinkedIn), and academic tools (arXiv, Wikipedia), with SSRF-protected URL fetching.
* [agentic-readiness-assessment](https://github.com/exadel-inc/agentic-readiness-assessment) ⭐ 23 | 🐛 4 | 🌐 Python | 📅 2026-09-28 - Agent skill that audits a repository for AI coding agent readiness and produces an evidence-based scorecard with prioritized fixes.
* [Espresso](https://github.com/mirkobozzetto/espresso) ⭐ 23 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-06 - Full token-saving stack in one plugin - output compression, global rules, RTK hook, Caveman ultra, GitNexus config. Detects existing setup, installs only what's missing. Works on Claude Code and Codex.
* [Agnostic-AI](https://github.com/ucsandman/Agnostic-AI) ⭐ 22 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Capture your Claude Code or Codex harness once (rules, hooks, skills, subagents, commands and MCP servers) and apply it identically to Gemini CLI, Cursor, Antigravity and 16 more clients.
* [gemini-for-kubernetes-development](https://github.com/gke-labs/gemini-for-kubernetes-development) ⭐ 22 | 🐛 93 | 🌐 Go | 📅 2026-10-04 - Gemini CLI extension that automates Kubernetes development tasks: declarative validation authoring, PR review, and SIG API Machinery issue triage.
* [go-ultimate](https://github.com/Djarvur/go-ultimate) ⭐ 22 | 🐛 1 | 🌐 Go | 📅 2026-10-04 - Opinionated Go skill that routes any Go task (CLI, library, backend service, MCP server, AI agent) to the right architecture, conventions, and review checklist across Claude Code, Codex, Cursor, Grok Build, Copilot CLI, and OpenCode.
* [SOTA Engineering Skills](https://github.com/martinholovsky/SOTA-skills) ⭐ 22 | 🐛 1 | 🌐 Python | 📅 2026-10-03 - Router-mapped library of 40 domain and language skills with BUILD and AUDIT modes, loading only the rules a task needs and ending every rules file in an audit checklist.
* [Supergraph](https://github.com/datit309/supergraph) ⭐ 22 | 🐛 0 | 🌐 Shell | 📅 2026-09-29 - Engineering workflow system for AI coding agents that enforces planning, TDD, verification, review, and architecture-aware decisions with local codebase graph intelligence across Claude Code, Codex CLI, Antigravity, and OpenCode,..
* [A Team](https://github.com/RBraga01/a-team) ⭐ 21 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-09 - Universal multi-agent infrastructure with 25 specialist agents, 16 enforced workflow skills, and a lead orchestrator for Claude Code, Codex CLI, Cursor, and OpenCode.
* [mcp-zuul](https://github.com/imatza-rh/mcp-zuul) ⭐ 21 | 🐛 1 | 🌐 Python | 📅 2026-10-03 - MCP server for Zuul CI with 48 tools for build analysis, failure diagnosis, log search, flaky job detection, pipeline status, and live console streaming.
* [RAG Reviewer](https://github.com/mimfort/rag_for_git) ⭐ 21 | 🐛 4 | 🌐 Python | 📅 2026-10-04 - Agentic PR review: hybrid RAG + code graph via MCP, review skills for Codex.
* [agent-kit](https://github.com/agent-kit-startup/agent-kit) ⭐ 20 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-04 - Extension pack of slash commands, skills, rules, and hooks adding plan-driven, confirmation-gated coding and staging-to-prod git workflows to Cursor and Claude Code.
* [synthesis-skills](https://github.com/synthesisengineering/synthesis-skills) ⭐ 20 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Engineering workflow skills (planning, review, rituals, fleet co-op) for Claude Code, Codex, and Muse, shipped through a gated cross-client release train.
* [vibekit](https://github.com/rizukirr/vibekit) ⭐ 20 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-03 - Evidence-based guardrail pipeline for vibe coding: brainstorm, plan, one fresh agent per task, verify, across Claude Code, Codex, opencode, and Antigravity.
* [coffee-paladin](https://github.com/pawelkwaczynski/coffee-paladin) ⭐ 19 | 🐛 1 | 🌐 Python | 📅 2026-09-18 - Thermal guard for Apple Silicon: pauses hot jobs before the Mac throttles and gates Claude Code, Codex and Gemini CLI before heavy commands.
* [Epic Harness](https://github.com/epicsagas/epic-harness) ⭐ 19 | 🐛 2 | 🌐 Rust | 📅 2026-10-02 - Auto-trigger quality skills + self-evolving agent harness — orbit (spec-to-ship), evolve (skill mutation), team (multi-agent), TDD, check, ship, simplify, debug, perf, secure.
* [aide](https://github.com/jmylchreest/aide) ⭐ 18 | 🐛 2 | 🌐 Go | 📅 2026-09-28 - Persistent memory, code intelligence, and multi-agent orchestration for Claude Code, OpenCode, and Codex CLI via skills, hooks, and an MCP server.
* [CommitLore](https://github.com/MongLong0214/commitlore) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - Keeps constraints, rejected alternatives, and warnings in Git trailers and serves them back to the agent before it edits a file.
* [hiai-opencode](https://github.com/HiAi-gg/hiai-opencode) ⭐ 18 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-15 - OpenCode plugin adding a multi-agent team with 10 specialist agents, execution gates, LSP tools, browser automation, and memory search.
* [ictfax-mcp](https://github.com/ictinnovations/ictfax-mcp) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for ICTFax. List and track fax transmissions, with opt-in tools to upload documents and send faxes.
* [SEO Skills AI](https://github.com/seoskillsai/seo-skills-ai) ⭐ 18 | 🐛 3 | 🌐 Python | 📅 2026-10-01 - Universal SEO skill suite and technical audit engine for Claude Code, Cursor, Codex, and other agents, with first-party Python adapters and HOL plugin-scanner CI.
* [TermaGITchi](https://github.com/TevvvB/termagitchi) ⭐ 18 | 🐛 3 | 🌐 Go | 📅 2026-09-18 - Stable per-worktree identity for parallel Claude Code, Codex, and tmux sessions; mood reads repository hygiene, not what the agent is doing.
* [VASTlint](https://github.com/aleksUIX/vastlint) ⭐ 18 | 🐛 2 | 🌐 Rust | 📅 2026-10-04 - Validate VAST, VMAP, and DAAST ad tags against IAB Tech Lab specs via Gemini CLI, Claude Code, and a hosted MCP server.
* [BGS Modding Superpowers](https://github.com/BB-84C/bgs-modding-superpowers) ⭐ 17 | 🐛 2 | 🌐 Python | 📅 2026-10-01 - Agentic Bethesda Game Studio modpack curation toolkit with MCP-driven xEdit conflict audit, MO2 control plane, BA2/BSA and Papyrus tooling, and skills for setup, dev-log, and release-changelog workflows.
* [MARGINAL](https://github.com/SignalLayerLabs/Marginal) ⭐ 17 | 🐛 16 | 🌐 Python | 📅 2026-10-01 - Local-first runtime governor for AI coding agents that detects proven no-progress repetition, records decision evidence, starts in Shadow Mode, and earns narrow enforcement only after repository-local evidence.
* [Neo](https://github.com/Parslee-ai/neo) ⭐ 17 | 🐛 4 | 🌐 Python | 📅 2026-10-04 - Code reasoning plugin for Claude Code and Codex that runs multi-agent analysis over relevant repository files and keeps a local semantic memory, promoting a lesson only after its suggestions are verified as accepted in git.
* [pbx-mcp](https://github.com/ictinnovations/pbx-mcp) ⭐ 17 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-02 - MCP server for Asterisk (AMI) and FreeSWITCH (ESL). Inspect channels, SIP registrations, trunks, and dialplan on a live PBX.
* [Blender Developer Tools](https://github.com/TMHSDigital/Blender-Developer-Tools) ⭐ 16 | 🐛 4 | 🌐 Python | 📅 2026-10-04 - 16 skills, 9 rules, snippets, templates, and smoke-tested examples for Blender Python add-on and scripting work with correct 4.5 LTS and 5.2 LTS APIs, installable as a Claude Code plugin and usable from Cursor.
* [ejentum-mcp](https://github.com/ejentum/ejentum-mcp) ⭐ 16 | 🐛 2 | 🌐 JavaScript | 📅 2026-06-11 - MCP server exposing reasoning, code, anti-deception, and memory harness tools for Codex.
* [ictcontact-mcp](https://github.com/ictinnovations/ictcontact-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTContact contact center. Monitor outbound campaigns, with opt-in tools to start and stop them.
* [ictdialer-mcp](https://github.com/ictinnovations/ictdialer-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTDialer cloud auto-dialer. Monitor outbound campaigns, with opt-in start and stop controls.
* [ictexam-mcp](https://github.com/ictinnovations/ictexam-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for reading exams, gradebooks, and item analysis, with opt-in tools for AI question-paper parsing and exam publishing.
* [ictpbx-mcp](https://github.com/ictinnovations/ictpbx-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - Read-only MCP server for ICTPBX. Inspect extensions, DID numbers, SIP trunks, tenants, and live PBX statistics.
* [Jev Studio](https://github.com/utk2103/jev-studio) ⭐ 16 | 🐛 1 | 🌐 Python | 📅 2026-10-04 - One-stop kit for playing with TypeSafe's Jev: MCP tools for Choice/Noul/Score, ready-made prompt libraries, and slash commands for every cookbook.
* [jevyoumean](https://github.com/syumai/jevyoumean) ⭐ 16 | 🐛 1 | 🌐 Go | 📅 2026-09-23 - CLI wrapper that uses TypeSafe's Jev to give semantic "Did you mean?" suggestions for mistyped subcommands, matching by intent rather than edit distance (e.g. `git record` → `git commit`).
* [MeMesh](https://github.com/PCIRCLE-AI/memesh) ⭐ 16 | 🐛 96 | 🌐 TypeScript | 📅 2026-10-04 - Local SQLite memory shared by Claude Code, Codex, Gemini, Cursor, and other MCP clients, captured automatically by hooks from real work and injected at the moment the agent acts.
* [Alcove](https://github.com/epicsagas/alcove) ⭐ 15 | 🐛 0 | 🌐 Rust | 📅 2026-09-20 - Local-first MCP server for private project docs with hybrid BM25+vector search, tree-sitter code indexing, and automated linting for team-wide documentation standards.
* [jev-harness](https://github.com/AntonioCoppe/jev-harness) ⭐ 15 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-25 - Decision harness for TypeSafe Jev (confidence gates, shadow mode, recipes, eval CLI)
* [Project Autopilot](https://github.com/AlexMi64/codex-project-autopilot) ⭐ 15 | 🐛 2 | 🌐 Python | 📅 2026-04-09 - Turn an idea into a structured project workflow with planning, execution, verification, and handoff.
* [trigger-tree](https://github.com/Hedde/trigger_tree) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2026-10-01 - Local documentation telemetry for Claude Code and Codex: see which docs your agent actually reads, gate discoverability in CI, and measure instruction adherence.
* [Codex Agenteam](https://github.com/yimwoo/codex-agenteam) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-07-06 - Specialist AI agents (researcher, PM, architect, developer, QA, reviewer) orchestrated as a configurable team pipeline.
* [Codex Reviewer](https://github.com/schuettc/codex-reviewer) ⭐ 14 | 🐛 4 | 📅 2026-05-05 - Second-pass review of Claude-driven plans and implementations.
* [opencode-nexus](https://github.com/mohammad154/opencode-nexus) ⭐ 14 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-30 - OpenCode plugin with a fixed three-agent execution workflow, conditional planning advice, fresh impact analysis, deterministic verification, and durable run state.
* [Staff Engineer Mode](https://github.com/sirmarkz/staff-engineer-mode) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-08-01 - Routes engineering design, delivery, reliability, security, operations, and maintenance prompts to focused staff-level specialist guidance for AI coding agents.
* [Super Jev](https://github.com/Kevthetech143/super-jev) ⭐ 14 | 🐛 15 | 🌐 Python | 📅 2026-10-04 - One judge between your agent and your data: finds the right skill and file, checks claims, gates actions, and remembers only the answers you approve.
* [WebLatexMCP](https://github.com/elias-ramzi/WebLatexMCP) ⭐ 14 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-02 - MCP server plus bundled skills for editing, compiling, and committing LaTeX in git-hosted projects like Overleaf.
* [xcode-mods](https://github.com/artemnovichkov/xcode-mods) ⭐ 14 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-02 - Claude Code plugin that brings Xcode build, run, tests, console and SwiftUI previews into live panes over the headless Xcode MCP server.
* [Check and Fix Accessibility](https://github.com/Neha/check-fix-accessibility) ⭐ 13 | 🐛 1 | 🌐 Python | 📅 2026-10-01 - Agent skill that audits and fixes front-end accessibility to WCAG 2.2 A/AA, covering semantics, keyboard navigation, ARIA, forms, contrast, and screen readers for web and native mobile across Cursor, Claude Code, Codex, Kiro, and Antigravity.
* [Embedded Workbench](https://github.com/AmethystLuna/embedded-workbench) ⭐ 13 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - Embedded C/C++ firmware development toolbox — 7 skills (FreeRTOS, Keil MDK, ARMCLANG, HardFault triage, state machines, LVGL) plus workflow gates and 4 agents for Claude Code, Codex, Cursor, Kimi, OpenCode, and ZCode.
* [Kernel](https://github.com/ariaxhan/kernel-claude) ⭐ 13 | 🐛 9 | 🌐 Python | 📅 2026-10-02 - Claude Code plugin marketplace and Codex plugin: hooks that block destructive commands, spawn guards on subagent contracts, agentdb memory with recall-before-act, blind verifiers, deterministic review; install with `/plugin marketplace add ariaxhan/kernel-claude`.
* [NeatContext](https://github.com/XTSoftwareLabs/neatcontext-plugins) ⭐ 13 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-23 - Saves the durable knowledge from Claude Code, Codex, GitHub Copilot, Kimi Code, and pi conversations as structured, reusable contexts you can reconnect in later sessions or share with your team.
* [opencode-9router](https://github.com/vheins/opencode-9router) ⭐ 13 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-25 - OpenCode plugin that registers 9Router as a provider with automatic model discovery and caching.
* [opencode-plugin-peers](https://github.com/jkrandom-sudo/opencode-plugin-peers) ⭐ 13 | 🐛 7 | 🌐 JavaScript | 📅 2026-09-29 - OpenCode plugin for cross-session messaging: independent instances on the same machine discover each other and exchange plain-text messages.
* [Writer's Loop](https://github.com/xxsang/writers-loop) ⭐ 13 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-21 - Structured AI writing workflow for planning, critique, revision, translation, style distillation, and opt-in local preference learning.
* [chat-history](https://github.com/ay-bh/chat-history) ⭐ 12 | 🐛 1 | 🌐 Rust | 📅 2026-09-25 - Claude Code/Codex/Cursor history search + export.
* [Claude Code Harness](https://github.com/dadwadw233/claude-code-harness) ⭐ 12 | 🐛 1 | 📅 2026-04-05 - Harness blueprint skill for turning vague agent ideas into concrete designs for request assembly, control loops, memory, permissions, recovery, and extension planes.
* [Claude Watchdog](https://github.com/Temikus/claude-watchdog) ⭐ 12 | 🐛 4 | 🌐 Shell | 📅 2026-10-04 - Stop hook that runs a critical post-mortem on every Claude Code session, cross-checking what was asked against the actual git diff for missed goals, wasted detours, and unverified claims.
* [Codex How To](https://github.com/Phelan164/codex-howto) ⭐ 12 | 🐛 5 | 🌐 Python | 📅 2026-10-02 - Engineering-first Codex curriculum and plugin with 9 skills, measured token-efficiency experiments, bounded orchestration, testing, review, and living knowledge maintenance.
* [Development Skills](https://github.com/reidemeister94/development-skills) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2026-09-20 - Three-tier triage (PASS\_THROUGH / LIGHT / FULL 4-phase) development workflow for Codex and Claude Code with language auto-detection (Python, Java, TypeScript, Swift, frontend) and a staff-reviewer subagent for fresh-eyes review on every change.
* [Hera Agent Godot](https://github.com/NotNull92/hera-agent-godot) ⭐ 12 | 🐛 0 | 🌐 Go | 📅 2026-09-15 - Drives a live Godot 4.x editor through the low-token Hera CLI — scene, node, and signal edits, play control, and runtime QA with verifiable compact JSON output, with the companion addon published on the official Godot Asset Store.
* [React Native Developer Skills](https://github.com/Neha/rn-developer-skills) ⭐ 12 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-29 - Vendor-neutral React Native skill collection covering spec authoring, architecture, performance, security, testing, and code review for Codex, Claude, and Cursor.
* [Tool Advisor](https://github.com/dragon1086/claude-skills) ⭐ 12 | 🐛 2 | 🌐 Shell | 📅 2026-04-23 - Read-only meta-skill that scans your MCP servers, skills, plugins, and CLI tools, then suggests up to three ranked approaches (Methodical / Fast / Deep) with a copy-paste Quick Action table.
* [Agentic Ship](https://github.com/moasq/agentic-ship) ⭐ 11 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - Cross-host product-development toolkit for Claude Code, Codex, Cursor, Hermes, and OpenClaw with shared rules, specialist roles, service connections, and machine-checked UI, backend, security, and launch gates.
* [Game Development Studio](https://github.com/theisegoria/game-development-studio) ⭐ 11 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-04 - CLI, skills, and MCP server for game asset production, vendoring, visual debugging, and performance analysis.
* [i-m-senior-developer](https://github.com/spumer/i-m-senior-developer) ⭐ 11 | 🐛 16 | 🌐 Python | 📅 2026-09-01 - A collection of Claude Code plugins covering TDD, code clarity, planning, review roles, and context upkeep.
* [opencode-plugin-loop](https://github.com/jkrandom-sudo/opencode-plugin-loop) ⭐ 11 | 🐛 6 | 🌐 JavaScript | 📅 2026-09-29 - OpenCode plugin adding a /loop command that runs prompts on fixed, adaptive, or one-shot schedules per session.
* [Praxis](https://github.com/ouonet/praxis) ⭐ 11 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-01 - Intent-driven workflow skills for coding agents: describe what done looks like, not the steps. Triage-first design keeps token costs low across design, TDD, debug, review, and release.
* [Salesforce Compound Engineering](https://github.com/divingsbysangam/salesforce-compound-engineering-plugin) ⭐ 11 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-02 - Salesforce-focused compound engineering plugin for Claude Code, Cursor, Codex, and other AI coding tools, with skills-first workflows, parallel persona dispatch, and Apex/LWC/Flow coverage.
* [Simple Man](https://github.com/Maksim-Burtsev/simple-man) ⭐ 11 | 🐛 2 | 🌐 Python | 📅 2026-10-01 - High-compression communication mode for Codex agents that removes filler while preserving search, validation, and implementation effort.
* [Agent Harness Skills](https://github.com/yfge/agent-harness-skills) ⭐ 10 | 🐛 4 | 🌐 Python | 📅 2026-07-14 - Designs agent-ready repository harnesses with entrypoints, validation surfaces, runtime evidence, delivery records, and atomic commit guidance.
* [BABOK Analyst](https://github.com/GSkuza/BABOK_ANALYST) ⭐ 10 | 🐛 13 | 🌐 JavaScript | 📅 2026-10-01 - BABOK v3 business analysis agent with 16 MCP tools, a 9-stage pipeline, and human-in-the-loop approval gates.
* [Casefile](https://github.com/x4cc3/casefile) ⚠️ Archived - Persistent security case tracking for bug bounties, CTFs, and security audits.
* [Clean Room](https://github.com/whit3rabbit/clean-room-skill) ⭐ 10 | 🐛 7 | 🌐 JavaScript | 📅 2026-09-30 - Spec-first clean-room workflow for authorized source analysis, behavioral specs, role separation, and verification without replacement code.
* [LoreConvo](https://github.com/labyrinth-analytics/loreconvo) ⭐ 10 | 🐛 0 | 🌐 Python | 📅 2026-10-03 - Persistent session memory MCP server for Claude — auto-saves and recalls conversation context, decisions, and artifacts across Claude Code, chat, and other surfaces with full-text search.
* [skills](https://github.com/pwguler/skills) ⭐ 10 | 🐛 0 | 🌐 Shell | 📅 2026-10-01 - Agent skills against the debt coding agents leave behind: unsettled plans, untested code, and claims nobody checked.
* [Spec-Driven Development](https://github.com/Habib0x0/spec-driven-plugin) ⭐ 10 | 🐛 0 | 🌐 Shell | 📅 2026-05-18 - Three-phase Requirements → Design → Tasks workflow for Claude Code and Codex — EARS notation acceptance criteria, autonomous execution loop, cross-spec dependencies, and post-implementation acceptance testing.
* [Stvena](https://github.com/nccapo/stvena) ⭐ 10 | 🐛 0 | 🌐 Go | 📅 2026-09-29 - Terminal workspace for running Codex or Claude Code beside live diffs, full-file review, checks, staging, and precise code feedback.
* [oddyssey](https://github.com/using-system/oddyssey) ⭐ 9 | 🐛 7 | 🌐 Python | 📅 2026-10-02 - Observability-Driven Development for coding agents: instrument an application or an AI agent with OpenTelemetry (gen\_ai semantic conventions: model, agent, tool and MCP spans, token and latency metrics), observe a run through its metrics, traces, logs and profiles on a local Grafana stack or a remote backend, benchmark it with k6, and verify that a fix landed.
* [Shadowclone](https://github.com/theonly1me/shadowclone) ⭐ 9 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-04 - Turns the engineering preferences you keep repeating into reusable skills and instructions for Claude Code, Codex, Cursor, and Antigravity.
* [Universal Design Principles](https://github.com/HDeibler/universal-design-principles) ⭐ 9 | 🐛 3 | 🌐 Markdown | 📅 2026-05-03 - Cross-agent UX and product-design marketplace with a root Codex collection plugin, five focused plugin bundles, and 137 Agent Skills for design review, accessibility, layout, interaction, cognition, and product polish.
* [debt-ops](https://github.com/bcanfield/agentic-tech-debt) ⭐ 8 | 🐛 14 | 🌐 Python | 📅 2026-10-04 - Catches AI-introduced tech debt at write-time: hooks log every deferral to a registry in your repo and a review skill ranks paydown by file churn.
* [GitCortex](https://github.com/bharath03-a/GitCortex) ⭐ 8 | 🐛 8 | 🌐 Rust | 📅 2026-10-03 - Branch-aware knowledge graph of a Git repo that incrementally re-indexes via tree-sitter and exposes it to AI coding assistants over MCP.
* [Professor](https://github.com/rezzminator/professor) ⭐ 8 | 🐛 1 | 🌐 Go | 📅 2026-10-03 - LLM-harness fleet framework for Claude Code, Codex, and OpenCode with a Go fleet CLI/TUI, cross-chat messaging, and a discipline layer of agents, commands, and hooks compiled across all three runtimes.
* [Tartiner Labs](https://github.com/tartinerlabs/skills) ⭐ 8 | 🐛 8 | 🌐 Go | 📅 2026-10-02 - Agent skills for git workflows, GitHub automation, security audits, code refactoring, and project tooling.
* [Demo GIF](https://github.com/conorbronsdon/demo-gif-skill) ⭐ 7 | 🐛 0 | 📅 2026-09-24 - Agent Skill that scripts, renders, optimizes, and embeds reproducible demo GIFs for CLI, TUI, web, and library projects using VHS or Playwright plus ffmpeg.
* [grip](https://github.com/guilyx/grip) ⭐ 7 | 🐛 0 | 🌐 Python | 📅 2026-09-28 - Git hook that quizzes you on your own diff before commit or push, with a Claude Code plugin plus Codex and Gemini CLI support.
* [LinkedIn Animated Infographics](https://github.com/imMamdouhaboammar/linkedin-animated-infographics) ⭐ 7 | 🐛 50 | 🌐 Python | 📅 2026-09-28 - Evidence-safe animated infographic generator with multi-agent design pipeline for LinkedIn.
* [opencode-weave](https://github.com/weave-io/weave) ⭐ 7 | 🐛 51 | 🌐 TypeScript | 📅 2026-10-03 - OpenCode plugin providing multi-agent orchestration with specialized agents, category task dispatch, and background sub-agent execution.
* [Orka](https://github.com/ugorur/orka) ⭐ 7 | 🐛 0 | 🌐 Shell | 📅 2026-09-29 - Orchestrates headless coding-agent CLIs (Codex, Grok, Claude Code, Cursor, Gemini, OpenCode, Copilot) as a team in isolated git worktrees, with cross-model review, QA and a scored run ledger.
* [Windrunner](https://github.com/shzlw/windrunner) ⭐ 7 | 🐛 0 | 🌐 Java | 📅 2026-09-15 - Self-hosted project workspace with Spring AI, MCP, CLI, and multi-provider AI integrations.
* [Wingman](https://github.com/lsshym/wingman.ai) ⭐ 7 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-29 - Cross-platform AI coding-agent plugin for repo-local project memory, data-contract checks, and project-map discovery before agents edit code.
* [Zagrosi Forge](https://github.com/zagrosi-code/zagrosi-forge) ⭐ 7 | 🐛 0 | 🌐 Python | 📅 2026-10-03 - Decompose broad project briefs into researched plans and implement sectioned work with TDD, quality gates, and traceability.
* [ArmorCodex](https://github.com/armoriq/armorCodex) ⭐ 6 | 🐛 44 | 🌐 JavaScript | 📅 2026-10-04 - Intent-based security for Codex with MCP plan registration, policy gating, CSRG cryptographic proofs, and audit logging on `bash` and `apply_patch`.
* [BioSymphony Structure Factory](https://github.com/BioSymphony/structure-factory) ⭐ 6 | 🐛 1 | 🌐 Python | 📅 2026-10-01 - Turn structural biology questions into agent-ready campaigns for protein design, structure prediction, and model comparison, with reproducible workflows and verifiable results.
* [Contorium](https://github.com/ContoriumLabs/contorium) ⭐ 6 | 🐛 1 | 🌐 TypeScript | 📅 2026-07-27 - Runtime continuity layer for AI coding agents, providing persistent workspace state, Git-aware sessions, and MCP-based context retrieval across tools and agent runs.
* [Cover My Repo](https://github.com/sjh9714/cover-my-repo) ⭐ 6 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-23 - Designs three checked GitHub social preview cards with Codex or Cursor, then renders them locally with Chrome.
* [Dev Skills](https://github.com/Jason-chen-coder/dev-skills) ⭐ 6 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-06 - Team workflow skills for specs, plans, TDD, debugging, verification, review, branch finishing, and design context.
* [LLM Transpile](https://github.com/epicsagas/llm-transpile) ⭐ 6 | 🐛 6 | 🌐 HTML | 📅 2026-09-20 - Auto-compress .md, .html, and .txt files via PostToolUse hook, cutting context usage by up to 40% with zero workflow change.
* [Munim](https://github.com/vishalsg42/munim) ⭐ 6 | 🐛 5 | 🌐 Python | 📅 2026-10-01 - Multi-account MCP server that holds a separate OAuth session per client across 11 providers, forwards each provider's own tools with that client's credentials, and refuses any call that would send one client's credential to another host.
* [SlopBar](https://github.com/thelioo/slopbar) ⭐ 6 | 🐛 5 | 🌐 Rust | 📅 2026-09-28 - Windows taskbar widget that shows Claude Code and Codex plan usage, limit resets and alerts, and switches accounts before one runs out.
* [Agent Workflow System](https://github.com/1139030773-cmd/agent-workflow-system) ⭐ 5 | 🐛 1 | 🌐 PowerShell | 📅 2026-06-12 - 一套中文AI工作流系统：7个协作技能 + 行为规范宪法 + 会话恢复机制，模糊目标→可执行任务，全生命周期引导。Codex & Claude Code 双平台，新手友好。
* [Codex rg Guard](https://github.com/Rycen7822/codex-rg-guard) ⭐ 5 | 🐛 3 | 🌐 Rust | 📅 2026-05-09 - Budgeted `rg`/`grep` replacement for Codex that narrows broad searches before they waste model context.
* [Codex Subagent Playbook](https://github.com/shinpr/codex-subagent-playbook) ⭐ 5 | 🐛 0 | 📅 2026-10-01 - Routes subagent work using model and reasoning-effort defaults tuned through measured comparisons and daily Codex use: stronger models handle judgment-heavy research and review, lower-cost models execute well-specified plans, and Codex uses longer waits to avoid frequent polling, intervenes on stalls, and verifies results.
* [Context Guard](https://github.com/GreenLv/codex-context-guard) ⭐ 5 | 🐛 1 | 🌐 Python | 📅 2026-10-04 - Preserves authoritative requirements and verification evidence across long-running Codex tasks and context compaction.
* [Logic Probe](https://github.com/AmethystLuna/logicprobe) ⭐ 5 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - Design-document & plan claim verification — checks every verifiable claim against the codebase, escalates behavioral claims to executable-model verification, compares before/after models for regression detection, and mines concurrency risk claims.
* [Maestro](https://github.com/mbanderas/maestro) ⭐ 5 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-01 - Opt-in local multi-CLI fusion engine and orchestration doctrine that fans a prompt across model CLIs, then judges and synthesizes one grounded answer.
* [MCP Migration Check](https://github.com/AlpayC/mcp-migration-check) ⭐ 5 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-04 - Deterministic MCP 2026-07-28 migration checker with an agent skill, CLI, GitHub Action, and hosted web probe powered by one rule engine.
* [md-prompt](https://github.com/nogu66/md-prompt) ⭐ 5 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - Claude Code plugin that paints Markdown onto the prompt box as you type, turning fenced code into syntax-highlighted cards without changing the text you send.
* [Mental CLI](https://github.com/afaraha8403/mental) ⭐ 5 | 🐛 51 | 🌐 JavaScript | 📅 2026-09-22 - Local-first CLI that keeps where you left off and what’s still open across agent sessions so you can pick up without reconstructing from memory.
* [Pixeltable](https://github.com/pixeltable/pixeltable-skill) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Declarative multimodal AI data engine for tables, computed columns, embedding search, agents, and FastAPI services.
* [telepathy](https://github.com/Winterrks/telepathy) ⭐ 5 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-26 - Lets coding-agent sessions on one machine (Claude Code, Codex, OpenCode, Gemini CLI, Copilot CLI, Cursor, Grok, Devin, Antigravity, Kimi Code, Qwen Code, Kilo Code) find and message each other through the same three MCP tools, starting a turn in an idle session where the agent allows it, with no network calls or telemetry.
* [VillageSQL Skills](https://github.com/villagesql/villagesql-skills) ⭐ 5 | 🐛 0 | 📅 2026-10-01 - Skills for VillageSQL including building extensions from scratch and porting PostgreSQL extensions to VillageSQL.
* [Agentizer](https://github.com/Humiris/wwa-transform) ⭐ 4 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-05 - Turn any website into an AI-powered agentfront with split-pane
* [AgiFlow](https://github.com/AgiFlow/ai-plugin) ⭐ 4 | 🐛 1 | 📅 2026-07-10 - Project management workflows for AI coding agents with planning, grooming, task execution, review, and AgiFlow MCP integration.
* [Codex Process Jobs](https://github.com/joelfarthing/codex-process-jobs) ⭐ 4 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-01 - Run long local builds, tests, benchmarks, and inference jobs as durable detached processes with tracked status, bounded results, and completion delivery across Codex surfaces.
* [Codex × Grok Bot Task Bridge](https://github.com/aipmer/codex-grok-task-bridge) ⭐ 4 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-03 - MCP task bridge for queued, read-only research between Codex and Grok Bot, with fenced leases, idempotency, scoped OAuth, evidence-based results, and optional Codex-side continuation.
* [Context Optimizer](https://github.com/evermeer/context-optimizer) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-25 - Keep your coding agent's context small. When a session gets compacted, Context Optimizer reranks the relevant parts, drops duplicates, and compresses the rest with a local ML pipeline (LLMLingua-2 + Sentence Transformers)
* [LoreDocs](https://github.com/labyrinth-analytics/loredocs) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-09-25 - Knowledge vault MCP server for Claude — organizes durable project docs, specs, and guides with FTS5 search, tagging, and cross-project context loading.
* [mermaid-for-claude](https://github.com/lucaswx2/mermaid-for-claude) ⭐ 4 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-30 - Renders Mermaid blocks from Claude Code replies as ASCII/Unicode diagrams inside the terminal, fully local with no browser.
* [Superpipelines](https://github.com/gustavo-meilus/superpipelines) ⭐ 4 | 🐛 16 | 🌐 JavaScript | 📅 2026-07-15 - Design and run write/review-isolated multi-agent AI pipelines across Codex, Claude Code, OpenCode, Cursor, Windsurf, and Cline.
* [tailtest](https://github.com/avansaber/tailtest-codex) ⭐ 4 | 🐛 10 | 🌐 Python | 📅 2026-06-13 - Hook-powered test generation -- detects files changed during an agent turn and instructs Codex to write and run tests automatically. Zero config, 8 languages.
* [Alloy](https://github.com/tlangridge/Alloy) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Orchestrates Codex, Claude, Grok, and Antigravity CLIs using existing subscriptions, with Jev task routing, read-only review panels, and managed worktree execution with independent review.
* [Anchor](https://github.com/biefan/anchor) ⭐ 3 | 🐛 2 | 🌐 Shell | 📅 2026-05-22 - Engineering discipline pack for Claude Code & Codex CLI with task-scope locking, anti-drift braking, condition-based codex review, project-CLAUDE.md pitfall writeback, and PreToolUse hooks that block irreversible bash patterns.
* [Camouflage](https://github.com/sinameraji/camouflage) ⭐ 3 | 🐛 0 | 🌐 Rust | 📅 2026-10-03 - Terminal UI for coding-agent harnesses that turns NDJSON events (Node SDK included) into a Claude Code-style inline transcript with pickers, forms, and permission prompts, using no CPU while idle.
* [claude-jit-context](https://github.com/Digital-Process-Tools/claude-jit-context) ⭐ 3 | 🐛 5 | 🌐 Shell | 📅 2026-10-04 - Project knowledge that loads only when it is needed, matched against the prompt, the file being touched, or the tool being run instead of sitting in context all session.
* [HOL Guard Plugin](https://github.com/hashgraph-online/hol-guard-plugin) ⭐ 3 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-03 - AI antivirus workflow for Codex, Claude Code, Cursor, Gemini, OpenCode, MCP servers, skills, and plugin release checks with local approvals and receipts.
* [jev-preflight](https://github.com/muse0509/jev-preflight) ⭐ 3 | 🐛 0 | 🌐 Go | 📅 2026-09-20 - Claude Code plugin that uses TypeSafe's Jev to assess code-change risk and request at most one additional investigation before a turn completes.
* [JevPromptCoach](https://github.com/CrowdLinker/JevPromptCoach) ⭐ 3 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-02 - Claude Code plugin that scores how well you prompt a coding agent and tracks whether your habits improve over time, running on TypeSafe's Jev model with no added latency on the prompt path.
* [kgai](https://github.com/kgaidev/kgai) ⭐ 3 | 🐛 1 | 🌐 Go | 📅 2026-10-04 - Shared decision memory for AI dev teams — share the decisions and knowledge behind your code across Claude Code, Codex CLI and Gemini CLI as an immutable local log, synced over an S3 bucket you own.
* [Pika](https://github.com/ayushjainr/pikamux) ⭐ 3 | 🐛 0 | 🌐 Rust | 📅 2026-10-04 - Enables Codex, Claude Code, and OpenCode agents to discover peers with relevant experience and consult them through private side conversations while their original work continues.
* [Repo Audit](https://github.com/conorbronsdon/repo-audit) ⭐ 3 | 🐛 0 | 📅 2026-09-24 - Agent Skill that checks whether a repository's README matches its code and whether stated rules are actually enforced, with an opt-in open-source launch workflow.
* [River Review](https://github.com/s977043/river-review) ⭐ 3 | 🐛 50 | 🌐 JavaScript | 📅 2026-10-04 - Versioned Skill Registry of code-review skills driven by a perspective-based review agent (code, security, performance, architecture, testing, adversarial) that verifies findings against the diff.
* [squidward](https://github.com/keshavbiswa/squidward) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-30 - Claude Code plugin that does the work correctly but delivers every sentence sarcastically, with mild, rowdy, and savage levels and a one-line roast code review.
* [Team Skills Platform](https://github.com/Colin4k1024/tsp) ⭐ 3 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-19 - Role-based team delivery framework — Tech Lead-orchestrated 8-role system with 195+ skills, 27 specialist agents, 80+ commands, hooks, and ECC harness for Claude Code, Codex, and OpenCode.
* [Agentry Observability](https://github.com/fr33dr4g0n/agentry-public) ⭐ 2 | 🐛 2 | 🌐 TypeScript | 📅 2026-07-13 - Agent-native product analytics, error logging, and deploy attribution for coding agents through one HTTP API.
* [AgentWiki](https://github.com/tidusvn05/agentwiki) ⭐ 2 | 🐛 0 | 🌐 Rust | 📅 2026-09-27 - Rust CLI that generates C4-style architecture docs for any repository using already-authenticated agent CLIs (Claude Code, Codex, Devin) as the LLM backend.
* [AIBoarding](https://github.com/gustavo-meilus/aiboarding) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Generate, maintain, compress, and audit standard AI-agent onboarding files with AGENTS.md, CLAUDE.md, drift tracking, and lifecycle hooks.
* [Codex Skin Pack Installer](https://github.com/ChannelerH/codex-skin-packs) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-09-29 - Codex plugin and skill that stages verified desktop skin packs from GitHub releases, validates files, and keeps restore guidance visible.
* [Codex Usage and Resets](https://github.com/joelfarthing/codex-usage-and-resets) ⭐ 2 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-29 - Turns Codex usage into planning facts with linear pace, projected exhaustion, banked-reset expirations, and conservative unexpected-reset detection.
* [crews](https://github.com/mdalexandre/crews) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-03 - Claude Code plugin that plans subagents before they run: each role gets a fixed model and effort, roles run in waves with blind checks, and a hook blocks subagents that were not planned.
* [dsh-product-subagent-console](https://github.com/Jokasa7/dsh-product-subagent-console) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-29 - Designs multi-Agent plans, observes real child-session trees, compares approved tasks with runtime attempts, and prepares evidence-backed recovery inside DeepSeek Harness conversations.
* [Easy-MCP](https://github.com/Mark007-R/Easy-MCP) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Turns plain Python functions into secure MCP servers, with ready-made read-only GitHub and Postgres servers installable in one command.
* [falsegreen-skill](https://github.com/vinicq/falsegreen-skill) ⭐ 2 | 🐛 5 | 🌐 JavaScript | 📅 2026-09-28 - Finds tests that stay green when the code they cover is broken, applying six ordered judgments over Python, TypeScript, JavaScript, and Robot Framework suites in Codex CLI and Claude Code.
* [GCF Proxy](https://github.com/blackwell-systems/gcf-codex-plugin) ⭐ 2 | 🐛 3 | 📅 2026-09-23 - Save 71% on MCP tool call tokens by wrapping any server with GCF encoding, with session stats hook and setup skill.
* [GrayMatter](https://github.com/ValkyrLabs/GrayMatter) ⭐ 2 | 🐛 2 | 🌐 Shell | 📅 2026-10-03 - Durable memory and shared graph state for Codex and OpenClaw agents, with live ValkyrAI schema awareness.
* [Hey Jarvis](https://github.com/dijiclick/hey-jarvis) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-10-01 - macOS voice assistant with an on-device wake word that runs quick Mac actions instantly and hands real work (code, browser, apps, email) to Claude Code through the Agent SDK.
* [jevcheck](https://github.com/sathariels/jevcheck) ⭐ 2 | 🐛 3 | 🌐 Python | 📅 2026-09-30 - Model-upgrade contract CLI for TypeSafe Jev (fixture eval, record/compare, CI-friendly exits); `pip install jevcheck`.
* [local-memory-mcp](https://github.com/vheins/local-memory-mcp) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - A lightweight MCP server that gives AI agents persistent memory with semantic search, backed by SQLite.
* [Mermail Skills](https://github.com/Nudgen-Marketing/mermail-skills) ⭐ 2 | 🐛 345 | 🌐 JavaScript | 📅 2026-10-01 - Official Mermail Agent Skills and Codex plugin that connect AI assistants to hosted Mermail MCP for inbox, scheduling, GTM, support, and x402 wallet workflows.
* [site-risk-check](https://github.com/kobimantzur/agent-skills) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-10-01 - Zero-dependency skill that scans a live URL for the conditions behind accessibility and privacy demand letters — trackers firing before consent, missing policies, and machine-checkable WCAG gaps — mapped to the jurisdictions the site actually sells to.
* [ssot-check](https://github.com/conorbronsdon/ssot-check) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-09-24 - Agent Skill and dependency-free Python CLI that discovers repeated facts in documentation and checks declared copies against canonical values.
* [What's Agent Doing](https://github.com/tzafrir/whats-agent-doing) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-04 - Claude Code mod that says in plain English what each step is for, with a timer, plus a live row per background agent.
* [Agent Deck](https://github.com/not-so-fat/agent-deck) ⭐ 1 | 🐛 12 | 🌐 TypeScript | 📅 2026-10-04 - One MCP for context management: bind self-improving playbooks, MCP tools, and API keys to the session.
* [Agent Guild](https://github.com/AgentTanuki/agent-guild-plugin) ⭐ 1 | 🐛 1 | 📅 2026-09-27 - Vet autonomous agents before delegating work or money, verify portable passports, use escrow, and record signed outcomes across Claude Code, Codex, MCP, A2A, and OpenClaw.
* [Antigravity Context Meter](https://github.com/Dunphil692/antigravity-context-meter) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-26 - Real-time 1:1 Cursor-style context meter & zero-loss session migration for Google Antigravity (Desktop HUD & IDE Extension).
* [BPMN Mapper](https://github.com/rwspatin/bpmn-skill) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Claude Code plugin that reconstructs an application's business flows from its source code as validated BPMN 2.0, with style lint, incremental updates and XML export for bpmn.io and Camunda.
* [Bring Your AI Migration Auditor](https://github.com/unitedideas/bringyour-mcp) ⭐ 1 | 🐛 2 | 📅 2026-05-25 - Read-only Codex plugin for auditing Claude Code to Codex migrations before Codex edits code. Checks AGENTS.md/CLAUDE.md scope, hooks, MCP config, skills, secret references, and validation notes.
* [bury-bench](https://github.com/Onur45500/bury-bench) ⭐ 1 | 🐛 7 | 🌐 Python | 📅 2026-09-10 - Deterministic zero-LLM-judge CLI that scores coding-agent replies for answer-burial and builds a Markdown leaderboard.
* [Claude Code Codex Plugin](https://github.com/davidq888/claude-code-codex-plugin) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-30 - Security-focused Codex plugin that connects to the local Claude Code CLI through MCP with login, status checks, safe-mode prompts, and no credential storage.
* [Codex TUI Proof](https://github.com/bnc4vk/codex-tui-proof) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-01 - Visually validate real local terminal UIs in Codex's in-app browser with screenshots and session evidence.
* [Compact Jev](https://github.com/edoproch/compact-jev) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-02 - Claude Code command that uses Jev to remove stale tool calls and results from long conversations while keeping user and assistant text verbatim.
* [Consensus](https://github.com/seanheiney/consensus) ⭐ 1 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-29 - Sends a hard question to a panel of frontier models (Claude, GPT, Gemini, Grok) that answer independently, critique each other adversarially, and return one answer the panel signed off on with its confidence and unresolved disagreements, via a CLI, MCP server, or skill pack that runs on your existing subscriptions with every panelist in a no-tools clean room.
* [Contexo](https://github.com/maheedhar132/Contexo) ⭐ 1 | 🐛 8 | 🌐 TypeScript | 📅 2026-09-29 - Portable AI context and cost control across every AI coding harness.
* [crayon](https://github.com/jonpojonpo/cc-crayon) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-02 - Claude Code plugin that redraws replies with themed Markdown and inline color tags Claude writes itself, across six switchable themes.
* [Deskbar](https://github.com/0NE-C0DEMAN/deskbar) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - Claude Code mod that adds a row of widgets above the prompt: context usage, Gmail, calendar, tasks across sessions, notes with reminders, a music deck, and a billable-hours timer.
* [dev-harness-kit](https://github.com/sh-ai-x/dev-harness-kit) ⭐ 1 | 🐛 15 | 🌐 Python | 📅 2026-10-02 - Enforced development workflow skills for Codex and Claude Code covering planning, TDD, debugging, review, security, CI, and release.
* [honeycomb](https://github.com/sediment-ai/honeycomb) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-09-27 - Buzz agent fleet as code, with each agent defined in YAML, deployed to Kubernetes, and routed to models through a LiteLLM gateway.
* [ictcrm-mcp](https://github.com/ictinnovations/ictcrm-mcp) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTCRM contact database. Read contact groups, with opt-in tools to create contacts and add them to campaigns.
* [idea-diamond](https://github.com/luckysharda/idea-diamond) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-09-17 - A Claude Code plugin for startup idea validation with predefined decision criteria, parallel research, skeptical review, and a human decision gate.
* [lumberroom-claude-code](https://github.com/lumberroom/lumberroom-claude-code) ⭐ 1 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-04 - Claude Code mod that replaces Claude Code's built-in memory with lumberroom shared memory, on lumberroom.cloud or a self-hosted engine, with session digests, optional per-prompt recall, automatic fact extraction, and token accounting in the status line.
* [LVTD Skills](https://github.com/LVTD-LLC/skills) ⚠️ Archived - Reusable Agent Skills for Codex, Claude Code, and compatible clients, covering Django, Rust, Cookiecutter, SEO, traction, product marketing, and nonfiction publishing workflows.
* [MailAgent](https://github.com/Alex0nder/MailAgent) ⚠️ Archived - Temporary inboxes for Codex — OTP, magic links, signup QA, simulate-first autotests (23 MCP tools).
* [Ontoly](https://github.com/0xsarwagya/ontoly-codex-plugin) ⭐ 1 | 🐛 2 | 📅 2026-07-21 - Deterministic Software Graph workflows for Codex: architecture review, dependency analysis, request tracing, configuration analysis, and impact analysis.
* [Personal Data Protection](https://github.com/AltByteSG/personal-data-protection-skill) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-09-17 - Engineer-facing personal-data-protection compliance reference — Singapore PDPA, Thailand PDPA, Indonesia UU PDP, Malaysia PDPA (Act 709 + 2024 Amendments), Philippines DPA — organised by where in the stack each obligation lands, with checklists, breach-response runbook, and a developer-view divergence table across all five.
* [Promptiff](https://github.com/BrantonLiu/promptiff) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-02 - Compares AI responses against original user prompts to surface possible omissions and unsourced additions; local CLI and Skill with a comparison canvas.
* [Redfox Agent Plugins](https://github.com/redfox-data/redfox-agent-plugins) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-09-22 - Ten cross-platform agent skills (video download, transcripts, image gen, trend search) installable on Claude Code, Codex, Cursor, and Gemini CLI from a single repo.
* [Registry Broker](https://github.com/hashgraph-online/registry-broker-codex-plugin) ⭐ 1 | 🐛 18 | 🌐 TypeScript | 📅 2026-08-24 - Delegate tasks to specialist AI agents via the HOL Registry, plan, find, summon, and recover sessions.
* [remembrandt](https://github.com/rishibanota/remembrandt) ⭐ 1 | 🐛 3 | 🌐 Python | 📅 2026-10-03 - Persistent memory for Claude Code, Cursor, and Codex coding agents that preserves decisions, gotchas, and changelogs across sessions.
* [RoadmapSmith](https://github.com/PapiScholz/roadmapsmith) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-27 - Evidence-backed ROADMAP.md workflows for AI coding agents with validation, sync, and roadmap generation across any tech stack.
* [RowTrail](https://github.com/adam2go/rowtrail) ⭐ 1 | 🐛 0 | 🌐 Rust | 📅 2026-09-29 - Local CLI and MCP server for agents to explore CSV/Parquet with bounded responses, versioned results, and reusable analysis handoffs.
* [Runtype Skills](https://github.com/runtypelabs/skills) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-03 - Supercharge your coding agent for AI product development — build, deploy, and operate agents, flows, tools, and surfaces on Runtype's managed edge runtime.
* [skill-sync-publisher](https://github.com/liuyewang/skill-sync-publisher) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-28 - Safely synchronize this Codex skill across public agent-skill registries.
* [Spellbook Skills](https://github.com/yyykf/spellbook-skills) ⭐ 1 | 🐛 3 | 🌐 Python | 📅 2026-10-03 - Practical Claude Code and Codex skills for worktrees, PR/MR automation, review cleanup, YApi lookup, and Java DDD guidance.
* [STE-Pro Max](https://github.com/shyamsridhar123/STE-Pro-Max) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Simplified Technical English-inspired writing, interactive visual explanations, and evidence-linked storytelling for Claude Code, Codex, and GitHub Copilot CLI.
* [Tandem Workflow Architect](https://github.com/frumu-ai/tandem-codex-plugin) ⭐ 1 | 🐛 2 | 🌐 TypeScript | 📅 2026-05-21 - Plan Tandem workflows in Codex, then validate, preview, and run them through the governed Tandem engine.
* [Unforgit](https://github.com/MiguelMedeiros/unforgit-codex-plugin) ⭐ 1 | 🐛 1 | 📅 2026-10-02 - Git-backed repository memory for Codex and other coding agents via MCP, with durable local knowledge for decisions, conventions, gotchas, and playbooks.
* [Unity Agent Workflows](https://github.com/AUN-PN/unity-agent-workflows) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-02 - Codex plugin and skill for Unity 2D agents that enforces "No proof, no edit" workflows with runtime-owner proof, Teach structure maps, and validation gates.
* [Workflow Kit](https://github.com/Le-Xuan-Thang/workflow-kit) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-06-02 - Full product lifecycle plugin for Claude Code, Codex CLI, and OpenCode: define Vision/Mission/Core → generate workplan → execute with mandatory cross-provider reviewer agents → synthesize deliverables → maintain, with parallel task execution, crash recovery, and AgentOps metrics.
* [Agency Continuity Audit](https://github.com/revertcreations/agency-continuity-audit) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-09-30 - Read-only audit that distinguishes durable agent goals, state, corrections, restart evidence, authority boundaries, scheduler claims, and commercial proof from self-reported health.
* [Azzle](https://github.com/azzle-lab/azzle) ⭐ 0 | 🐛 22 | 🌐 HTML | 📅 2026-10-02 - Base-native task coordination and settlement for AI agents, exposed through a hosted MCP server and TypeScript agent SDK.
* [Cloudish](https://github.com/cloudishai/skills) ⭐ 0 | 🐛 0 | 📅 2026-10-03 - Deploy a Dockerfile, source folder, or container image to Cloudish from Claude Code or Codex and report the live URL, with persistent volumes and an agent-created, credit-capped API key.
* [CodeTruss](https://github.com/DeliriumPulse/codetruss-plugins) ⭐ 0 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-12 - Local-first acceptance gate that checks coding-agent scope, sensitive surfaces, deterministic analyzers, and repository verification from immutable Git snapshots, then writes signed receipts before the PR.
* [Codex Token Watch](https://github.com/premk134/codex-token-watch) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-30 - Read-only macOS CLI that turns local Codex Desktop task logs into per-turn token, prompt-cache, cache-miss, duration, and API-cost analysis.
* [Delx Recovery](https://github.com/davidmosiah/delx-plugins) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-27 - Free recovery and continuity plugin for AI agents: resume prior sessions, capture state, process failures into a recovery plan, and remember across sessions through a hosted MCP server (works in Codex, Claude Code, Cursor, and VS Code).
* [Encore Lite](https://github.com/keegan-dotcom/encore-lite) ⭐ 0 | 🐛 0 | 📅 2026-07-24 - Free end-of-week surprise builder for Claude Code and Codex - the night before your weekly usage cap resets, it reads your recent work and builds one bonus deliverable, delivered as a reveal with an optional weekly scheduled run.
* [FinBridge](https://github.com/Jakechj/finbridge-mcp) ⭐ 0 | 🐛 0 | 📅 2026-10-04 - Remote MCP server for Korean and US market data with filings, screeners, insider activity, and portfolio backtests.
* [ga4-gsc-clarity-mcp-server](https://github.com/rakoo04/ga4-gsc-clarity-mcp-server) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - Read-only MCP server for Google Analytics 4, Google Search Console, and Microsoft Clarity with named OAuth/token connections reusable across any project.
* [Grafana Dashboards-as-Code](https://github.com/jburgess/mcp-grafana) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-27 - Typed Grafana dashboard and panel builders, structural linting, semantic dashboard diff, and scaffold/audit/review recipes exposed over MCP.
* [harness-scope](https://github.com/shimo4228/harness-scope) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-04 - Claude Code mod that turns global skills, agents, rules files and tools on or off per repo through named profiles kept in \~/.claude, with no network or model calls.
* [Jev Go](https://github.com/nandansrikrishna/jev-go) ⭐ 0 | 🐛 0 | 🌐 Go | 📅 2026-09-19 - Standalone Go CLI and MCP server for TypeSafe's Jev model, with typed single and batch evaluation, JSONL pipelines, and resume support.
* [limitwise](https://github.com/aarsht7/limitwise) ⭐ 0 | 🐛 4 | 🌐 Rust | 📅 2026-09-30 - Schedule and automate Codex work while respecting rolling and weekly usage limits in percentage or in tokens. Let your PC work while you sleep.
* [loose-ends](https://github.com/fernandomoraes/loose-ends) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - Keeps a live checklist above the Claude Code prompt of the topics, open questions and tasks a conversation raised, updated by a small model after each turn and drawn with function hooks.
* [mcp-md-reader](https://github.com/JoseEstevez520/mcp-md-reader) ⭐ 0 | 🐛 7 | 🌐 JavaScript | 📅 2026-09-27 - MCP server that helps AI agents find Markdown structure and read only the relevant section, metadata, or vault links.
* [metabrain](https://github.com/ariaxhan/metabrain) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-26 - MCP server for agent memory: SQLite, zero dependencies, tools learn/recall/verdict/hypotheses/start\_brief/stats/capture\_error, patterns graduating to hypotheses then preferences; `pip install "metabrain[mcp]"` then `metabrain-mcp --db PATH`.
* [Metis](https://github.com/gkrtjd99/Metis) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-03 - Repository-level engineering orchestrator that delegates bounded discovery, planning, implementation, review, and verification to fresh subagents, isolates mutable tasks in Git worktrees with declared path ownership, and requires evidence-gated completion.
* [Nibbl](https://github.com/nuromirzak/nibbl) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-02 - Tamagotchi-style pixel pet for Claude Code that lives in a band above the prompt via function hooks and reacts to tool calls, passing checks, and commits.
* [omp-rewrite](https://github.com/zPeppOz/omp-rewrite) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-29 - Oh My Pi (omp) extension that adds a /rewrite command, which asks clarifying questions about a rough draft prompt in a side turn and puts a thorough rewrite in the composer.
* [opencode-toolrouter](https://github.com/Nsilswal/opencode-toolrouter) ⭐ 0 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-30 - OpenCode plugin that uses TypeSafe's Jev to send the model only the MCP tools each request needs, cutting tool-schema tokens per model call by about 92% in a 296-tool benchmark.
* [Orchestrate Task Force](https://github.com/alexpsz/orchestrate-task-force) ⭐ 0 | 🐛 0 | 📅 2026-09-29 - Task orchestration skill for Codex Desktop, Claude Code, and Google Antigravity, with visible task ownership, scoped parallel work, and integrated review.
* [OutcomeLoop](https://github.com/tinyopsstudio/outcomeloop-build-week) ⭐ 0 | 🐛 5 | 🌐 JavaScript | 📅 2026-07-17 - Outcome-verified Codex runner and plugin that resumes one GPT-5.6 session until an external verifier passes, then seals the evidence in an Ed25519-signed receipt.
* [PageSpeed Optimizer](https://github.com/alexlivre/pagespeed-optimizer-alexlivre) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-24 - Optimizes web applications for 100/100 PageSpeed Insights, Core Web Vitals, and Generative Engine Optimization (GEO).
* [pi-codex-web-search](https://github.com/devinat1/pi-codex-web-search) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - A Pi extension that searches the web through the authenticated Codex CLI.
* [slopless](https://github.com/0xGondarxyz/slopless) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - Claude Code plugin that checks social media drafts against 92 AI writing patterns and blocks the post until they are fixed.
* [smt-mcp-server-poc](https://github.com/ab-ten/smt-mcp-server-poc) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-19 - Read-only local workspace MCP server PoC for ChatGPT via OpenAI Secure MCP Tunnel, with path/mount containment and `.mcpignore` exposure controls.
* [Task Lantern](https://github.com/paranjaymundra/task-lantern) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-28 - Offline dashboard that collects progress published by Claude Code and Codex threads across projects into one local HTML workspace, showing the current step, decisions needed, blockers, and recent files.
* [TaskDock](https://github.com/m1nga/taskdock) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-19 - Resume agent tasks from current deliverables and decisions, with portable folders, link repair, and reversible file organization.
* [tmux-agentic-plugin](https://github.com/Abstrucked/tmux-agentic-plugin) ⭐ 0 | 🐛 3 | 🌐 Shell | 📅 2026-10-01 - tmux status-bar strip and picker showing which Claude Code, Codex and OpenCode agents are working, blocked or ready, including on other machines over ssh and Tailscale, with desktop notifications.
* [Tree Ring Memory](https://github.com/TerminallyLazy/tree-ring-memory-codex-plugin) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-09-30 - Local-first memory lifecycle guidance for Codex agents with recall, evidence-backed lessons, privacy-safe memory capture, audit, consolidation, and explicit forgetting.
* [Usage Monitor](https://github.com/Errr0rr404/usage-monitor) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-03 - Floating desktop meter that shows remaining Grok, MiniMax, Codex, Claude, Cursor, Copilot, and Gemini usage and keeps each session on this computer.
* [Changelog Forge](./plugins/mturac/changelog-forge) - Conventional commits → CHANGELOG section + semver bump.
* [Codex Full-Stack Workflow](https://github.com/kevin592/codex-full-stack-workflow) - Turns rough product requests into staged, reviewable full-stack delivery with persistent requirements, change control, visual evidence, and completion gates.
* [Commit Narrator](./plugins/mturac/commit-narrator) - Generate semantic commit message from staged diff, including the *why*.
* [Deps Doctor](./plugins/mturac/deps-doctor) - Multi-ecosystem dependency audit (npm, pip, cargo, go) in one report.
* [Env Lint](./plugins/mturac/env-lint) - `.env` vs `.env.example` key parity — never prints values.
* [Flaky Detector](./plugins/mturac/flaky-detector) - Run a test command N times, report per-test flakiness %.
* [PR Storyteller](./plugins/mturac/pr-storyteller) - PR title + body + test plan from commits and diff vs base branch.
* [SearchLink Lite](https://github.com/GlobalMatchHub/searchlink-lite) - Local read-only MCP server for Google Search Console: site performance and query breakdowns, low-CTR and rank 8-20 opportunities, URL inspection, sitemaps, on-page checks and Google ranking update history.
* [Secret Guard](./plugins/mturac/secret-guard) - Pre-commit secret scanner using pattern and entropy detection.
* [Standup Generator](./plugins/mturac/standup-gen) - Daily standup notes from git activity across repos.
* [Test Gap](./plugins/mturac/test-gap) - Find lines in your diff lacking test coverage (Cobertura, lcov, coverage.json).
* [TODO Harvest](./plugins/mturac/todo-harvest) - TODO/FIXME/HACK scan with `git blame` author + age.

### Tools & Integrations

* [ego-browser](https://github.com/citrolabs/ego-lite) ⭐ 16,824 | 🐛 180 | 🌐 JavaScript | 📅 2026-09-23 - Browser automation for AI agents through ego lite, a Chromium browser where agents navigate pages, fill forms, capture screenshots, and extract data in isolated task spaces that reuse the user's existing logins.

* [LinkedIn Skills](https://github.com/sergebulaev/linkedin-skills) ⭐ 4,088 | 🐛 4 | 🌐 Python | 📅 2026-10-03 - Codex-ready LinkedIn marketing bundle with a native .codex-plugin manifest and 11 skills: post writing with 20 tested hook formulas, AI-tell humanizer, pre-publish audit, comment and reply drafting, hook extraction, content planning, profile optimization, engager analytics, and thread monitoring; also works in Claude Code.

* [LetsFG](https://github.com/LetsFG/LetsFG) ⭐ 2,109 | 🐛 6 | 🌐 Python | 📅 2026-10-04 - Flight and hotel search and booking for AI agents across hundreds of airlines and the major booking sites, via a remote MCP server (Claude, ChatGPT, Cursor, Windsurf), CLI, Python/JS SDKs, and an Agent Skill, with free search after a one-time card connection and real airline PNRs on flight bookings.

* [edgeone-makers-tools](https://github.com/TencentEdgeOne/edgeone-makers-tools) ⭐ 1,861 | 🐛 8 | 🌐 JavaScript | 📅 2026-09-23 - Agent skill for EdgeOne Makers, a one-stop deployment platform where developers rapidly deploy full-stack projects, cloud functions, and AI agents and instantly get a live URL, covering the full path from development to launch.

* [Logo Design Skill](https://github.com/kaankiziltug/logo-design-skill) ⭐ 1,817 | 🐛 0 | 🌐 HTML | 📅 2026-09-30 - Agent Skill for Claude Code, Codex, Gemini CLI, and other agents that runs a full logo workflow, from brief and category research to three tested SVG concepts and a concept checkpoint, then builds favicons, app icons, and presentation boards, backed by a 1,400+ logo reference library.

* [claude-fuer-deutsches-recht](https://github.com/Klotzkette/claude-fuer-deutsches-recht) ⭐ 1,655 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Experimental German-law skill collection with installable plugins, drafting workflows, legal source checks, and practice case files.

* [yomiyasu](https://github.com/nanaism/yomiyasu) ⭐ 1,371 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Agent Skill for rewriting unnatural, AI-generated Japanese into human-readable, high-information-density text while strictly preserving the original meaning.

* [KiCad Happy](https://github.com/aklofas/kicad-happy) ⭐ 1,330 | 🐛 5 | 🌐 Python | 📅 2026-09-13 - KiCad EDA skills for schematic analysis, PCB layout review, component sourcing, BOM management, and manufacturing preparation.

* [DeepPaperNote](https://github.com/917Dhj/DeepPaperNote) ⭐ 1,151 | 🐛 5 | 🌐 Python | 📅 2026-10-04 - Agent skill that deep-reads a single paper and generates structured Obsidian research notes with figures, results, and limitations.

* [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-AI-Toolkit) ⭐ 1,130 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-04 - Backend for AI coding agents on Tencent CloudBase — database, auth, and functions via Plugin, Skills & MCP.

* [Agent QA](https://github.com/vostride/agent-qa) ⭐ 898 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-03 - MCP server and Agent Skills for authoring, running, and triaging natural-language web and mobile tests with reusable execution memory.

* [Digital Marketing Pro](https://github.com/indranilbanerjee/digital-marketing-pro) ⭐ 849 | 🐛 2 | 🌐 Python | 📅 2026-10-04 - Open-source AI marketing plugin for agencies — 154 skills, 25 specialist agents, 12-Part Strategy Flow, AEO/GEO, GSC AI Performance Report, Google Ads API v24, EU AI Act Article 50 / C2PA compliance.

* [Education Agent Skills](https://github.com/GarethManning/education-agent-skills) ⭐ 821 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-28 - 131 evidence-based education skills for curriculum design, lesson planning, and assessment, with transparent evidence ratings and MCP server.

* [GodotPrompter](https://github.com/jame581/GodotPrompter) ⭐ 783 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-04 - Collection of 55 Godot 4.x domain skills and agents that AI coding agents load on demand for GDScript and C# development.

* [Watermelon UI](https://github.com/WatermelonCorp/watermelon-platform) ⭐ 609 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-04 - MCP server exposing 850+ source-backed React components, blocks, dashboards, and templates through search, retrieval, category, and page-composition tools.

* [humanizer-ru](https://github.com/ilyautov/humanizer-ru) ⭐ 408 | 🐛 4 | 🌐 Python | 📅 2026-10-02 - Agent skill for Claude Code, Codex, Cursor and Gemini that rewrites Russian text to remove 64 AI-generation markers (bureaucratese, calques, ChatGPT fingerprints), with a corpus-calibrated scanner, audit mode and author-voice calibration.

* [Backlot](https://github.com/brekkylab/backlot) ⭐ 360 | 🐛 117 | 🌐 Python | 📅 2026-10-04 - Local emulator for Slack, Gmail, Google Drive, GitHub, Jira, Notion, S3 and other enterprise SaaS APIs, reproducing their response shapes, pagination, auth and per-document ACLs over a corpus you supply, so agents and RAG pipelines can be tested with no vendor account; `backlot mcp` serves every source as MCP tools.

* [mcpsnoop](https://github.com/kerlenton/mcpsnoop) ⭐ 359 | 🐛 0 | 🌐 Go | 📅 2026-10-04 - Wireshark for MCP, a transparent proxy that shows the real traffic between your AI client and MCP servers, fails CI on it and exports it as OpenTelemetry spans.

* [Busabase](https://github.com/busabase/busabase) ⭐ 326 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-28 - Open-source database and workspace for AI agents to manage typed tables, fields, views, records, docs, files, and search with a Streamable HTTP MCP server and human-in-the-loop ChangeRequests.

* [opencode-visual-cache](https://github.com/Hotakus/opencode-visual-cache) ⭐ 304 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-30 - OpenCode TUI plugin that displays real-time token cache hit rate, token usage, cost savings, and provider balance in a sidebar.

* [affine-mcp-server](https://github.com/DAWNCR0W/affine-mcp-server) ⭐ 296 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - MCP server exposing AFFiNE workspaces, documents, and databases to AI clients over stdio or HTTP.

* [QVeris Agent Toolkit](https://github.com/QVerisAI/qveris-agent-toolkit) ⭐ 262 | 🐛 7 | 🌐 JavaScript | 📅 2026-10-04 - Cross-client toolkit that brings professional data and tools to AI assistants, products, and workflows: find services, review supported scope, call them, and audit usage.

* [ru-text](https://github.com/talkstream/ru-text) ⭐ 247 | 🐛 3 | 🌐 Shell | 📅 2026-10-03 - Russian text quality — \~1,044 rules for typography, info-style, editorial, UX writing, and business correspondence.

* [Bitbucket CLI](https://github.com/avivsinai/bitbucket-cli) ⭐ 229 | 🐛 9 | 🌐 Go | 📅 2026-10-04 - Manage Bitbucket repos, PRs, branches, issues, webhooks, and pipelines for Data Center and Cloud.

* [Telnyx](https://github.com/team-telnyx/ai) ⭐ 220 | 🐛 24 | 🌐 TypeScript | 📅 2026-10-01 - Telnyx toolkit for AI agents bundling Claude Code, Cursor, Gemini CLI, and OpenCode plugins, an agent toolkit for OpenAI/LangChain/CrewAI/Vercel AI SDK, a hosted MCP server, and a one-command CLI for messaging, voice, numbers, and account management.

* [Taisly Agent Kit](https://github.com/taisly/agent) ⭐ 216 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-03 - Publish short-form videos to TikTok, Instagram Reels, YouTube Shorts, X, and Facebook from Codex with the Taisly MCP server and bundled social media posting skill.

* [X Twitter Scraper](https://github.com/Xquik-dev/x-twitter-scraper) ⭐ 210 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-04 - X/Twitter data, monitored workflows, HMAC webhooks, and MCP access through the Xquik REST API with confirmation-gated write guidance.

* [Codex Usage Tracker](https://github.com/douglasmonsky/codex-usage-tracker) ⭐ 196 | 🐛 13 | 🌐 Python | 📅 2026-08-20 - Track aggregate Codex token usage from local session logs with MCP tools for summaries, session detail, CSV export, and dashboard generation.

* [OC ChatGPT Multi Auth](https://github.com/ndycode/oc-chatgpt-multi-auth) ⭐ 195 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-02 - Codex setup skill and OpenCode plugin for ChatGPT Plus/Pro OAuth, GPT-5/Codex presets, and multi-account failover.

* [tlgr](https://github.com/tlgrcli/tlgr) ⭐ 188 | 🐛 5 | 🌐 Python | 📅 2026-10-03 - Claude Code plugin and Agent Skill for operating a personal Telegram account through the tlgr CLI over MTProto, with JSON output and webhook event push.

* [Commercial Legal PL](https://github.com/apiotrowski-afk/commercial-legal-pl) ⭐ 176 | 🐛 1 | 🌐 Python | 📅 2026-09-23 - Drafts and reviews contracts under Polish law (B2B IT, IP, settlements) with a clause library, doctrinal knowledge base, and § / ust. / pkt cross-reference consistency checks.

* [search1api-mcp](https://github.com/superagents-lab/search1api-mcp) ⭐ 173 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-29 - MCP server providing web search, news, page crawling, sitemaps, and trending topics via Search1API.

* [opencode-visualiser](https://github.com/psinetron/opencode-visualiser) ⭐ 169 | 🐛 3 | 🌐 HTML | 📅 2026-10-02 - OpenCode plugin that renders live agent sessions as an animated pixel-art office with per-agent characters.

* [AgentCall](https://github.com/pattern-ai-labs/agentcall) ⭐ 164 | 🐛 2 | 🌐 Python | 📅 2026-09-15 - Lets Claude Code, Codex, Cursor, Gemini CLI, and 30+ other agents join Google Meet, Zoom, or Microsoft Teams as a speaking, listening, presenting participant with text-to-speech, live transcripts, screenshare, and an avatar camera feed.

* [Miro](https://github.com/miroapp/miro-ai) ⭐ 159 | 🐛 17 | 🌐 TypeScript | 📅 2026-09-17 - Official Miro MCP server and agent integrations for Claude Code, Codex, Gemini CLI, Cursor, and other AI tools — read and write Miro boards, create diagrams, extract context from boards, and generate code from designs.

* [Hostinger API MCP](https://github.com/hostinger/api-mcp-server) ⭐ 157 | 🐛 11 | 🌐 TypeScript | 📅 2026-10-01 - Manage Hostinger VPS, domains, DNS, hosting, and billing through MCP tools backed by the official Hostinger API.

* [unslop](https://github.com/MohamedAbdallah-14/unslop) ⭐ 153 | 🐛 4 | 🌐 Python | 📅 2026-09-28 - Strip AI writing patterns from text output — removes filler phrases, hedging language, and generic constructs to produce cleaner written content. Install: `npm install -g unslop`.

* [Jev Social](https://github.com/socai-io/jev-social) ⭐ 145 | 🐛 13 | 🌐 JavaScript | 📅 2026-10-01 - Agent skill that runs read-only Instagram, TikTok, and LinkedIn research via browser automation and returns source-linked evidence reports.

* [Zero Slop](https://github.com/manavmishra/ZeroSlop) ⭐ 131 | 🐛 5 | 🌐 Python | 📅 2026-10-04 - Say no to AI slop: a human-in-the-loop learning agentic workflow skill that scores text 0-100 for AI slop and rewrites it tastefully, with a standard-library Python scorer that has zero dependencies and runs offline.

* [DocsMint](https://github.com/HiAi-gg/docsmint) ⭐ 118 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-28 - Cloud or self-hosted knowledge workspace with MCP tools for hybrid search, GraphRAG, and document management.

* [X (Twitter) Skills](https://github.com/sergebulaev/x-skills) ⭐ 117 | 🐛 1 | 🌐 Python | 📅 2026-10-03 - Codex-ready X (Twitter) marketing bundle with a native .codex-plugin manifest: tweet and thread writing with corpus-validated hook formulas (validated against \~450 top tweets), AI-tell humanizer, hook extraction, reply drafting, content planning, and audience insights; also works in Claude Code.

* [Langfuse Observability](https://github.com/avivsinai/langfuse-mcp) ⭐ 113 | 🐛 1 | 🌐 Python | 📅 2026-09-25 - Query traces, debug exceptions, analyze sessions, and manage prompts via MCP tools.

* [opencode-cmd-provider](https://github.com/rashidrazak/opencode-cmd-provider) ⭐ 112 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-04 - OpenCode plugin that registers Command Code as a provider so you can run its models and plans inside OpenCode, with a sidebar showing tier, allowances, and deal rates.

* [im-ai-copyeditor](https://github.com/Turtle-Hwan/im-ai-copyeditor) ⭐ 100 | 🐛 0 | 🌐 Python | 📅 2026-09-08 - Korean copyediting skill for coding agents that fixes spelling, translation-style phrasing, AI tone, and style sentence by sentence.

* [whatsapp-claude-plugin](https://github.com/Rich627/whatsapp-claude-plugin) ⭐ 100 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - Claude Code channel plugin and stdio MCP server that connects WhatsApp as a linked device for messaging, voice transcription, and remote tool approval.

* [GDS Agent](https://github.com/neo4j-contrib/gds-agent) ⭐ 98 | 🐛 0 | 🌐 Python | 📅 2026-09-21 - Graph data scientist as an MCP server and skill: project Neo4j graphs and run GDS algorithms for centrality, community, path finding, similarity, embeddings, and ML pipelines.

* [Call-E](https://github.com/CALLE-AI/call-e-integrations) ⭐ 96 | 🐛 29 | 🌐 JavaScript | 📅 2026-09-23 - Plan, run, and inspect Call-E phone call workflows from Codex through the calle CLI.

* [Jenkins CLI](https://github.com/avivsinai/jenkins-cli) ⭐ 91 | 🐛 4 | 🌐 Go | 📅 2026-09-29 - GitHub CLI-style interface for Jenkins controllers with jobs, pipelines, runs, logs, artifacts, credentials, and nodes.

* [Agent Message Queue](https://github.com/avivsinai/agent-message-queue) ⭐ 87 | 🐛 6 | 🌐 Go | 📅 2026-10-04 - File-based inter-agent messaging with co-op mode, cross-project federation, and orchestrator integrations.

* [You.com Agent Skills](https://github.com/youdotcom-oss/agent-skills) ⭐ 83 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-02 - Cross-platform You.com skill and plugin bundle that gives coding agents current web search, URL content extraction, cited research, finance research, and integration discovery, plus MCP server configs.

* [Network-AI](https://github.com/Jovancoding/Network-AI) ⭐ 78 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-29 - TypeScript multi-agent orchestrator shipped as a Claude Code plugin, Gemini CLI extension, and MCP server that adds an atomic shared blackboard, per-agent token budgets, permission gating, and audit trails across 32 agent frameworks.

* [Kesha Voice Kit](https://github.com/drakulavich/kesha-voice-kit) ⭐ 76 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-04 - Local speech-to-text and text-to-speech CLI with an MCP server; it transcribes 25 languages and speaks 9, and every model runs on the machine itself rather than in a cloud service.

* [VMware-AIops](https://github.com/vmware-skills/VMware-AIops) ⭐ 74 | 🐛 2 | 🌐 Python | 📅 2026-09-20 - Skill and MCP server with 60 tools for VMware vCenter and ESXi VM lifecycle, OVA/template deployment, snapshots, guest operations and cluster management, where every destructive tool previews what it would change and acts only on an explicit confirm.

* [Cortex](https://github.com/cdeust/Cortex) ⭐ 73 | 🐛 7 | 🌐 Python | 📅 2026-10-03 - Persistent thermodynamic memory and cognitive-profiling MCP server for Claude Code, Codex, and Gemini CLI — heat/decay dynamics, predictive-coding write gates, knowledge graph, and intent-aware recall across sessions.

* [mcp-music-studio](https://github.com/linxule/mcp-music-studio) ⭐ 73 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-04 - MCP server for AI music creation: scored ABC notation composition and Strudel live coding, with sheet music rendering, harmony analysis, and MIDI/WAV export.

* [ScrapeGraph AI](https://github.com/ScrapeGraphAI/just-scrape) ⭐ 67 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-21 - AI-powered web scraping CLI to search, scrape, extract structured JSON, crawl, and monitor web pages via the ScrapeGraph AI API.

* [TikTok Skills](https://github.com/sergebulaev/tiktok-skills) ⭐ 62 | 🐛 1 | 🌐 Python | 📅 2026-10-03 - Codex-ready TikTok marketing bundle with a native .codex-plugin manifest and 8 skills: 3-second hook scripting (spoken line plus on-screen text), caption and hashtag writing under the 2,200-char API limit, trend mapping, profile optimization, AI-tell humanizer, and comment drafting; publishes through Publora with approval before anything goes live; also works in Claude Code.

* [Azure Cosmos DB Agent Kit](https://github.com/AzureCosmosDB/cosmosdb-agent-kit) ⭐ 57 | 🐛 28 | 🌐 Python | 📅 2026-10-03 - Azure Cosmos DB best-practice skills and MCP tooling for Codex, Claude Code, Cursor, Gemini CLI, Grok Build, Kimi Code, GitHub Copilot, and other Agent Skills-compatible assistants.

* [Nimble](https://github.com/Nimbleway/agent-skills) ⭐ 57 | 🐛 7 | 🌐 Python | 📅 2026-10-04 - Web Search Agents that search, browse, extract, and reason across live pages and return cited, schema-enforced results, with self-learning retrieval that improves accuracy and lowers cost per task on repeat work, plus Search and Extract skills for fast raw web data in Claude Code, Codex, Cursor, and Grok Build.

* [Arize Skills](https://github.com/Arize-ai/arize-skills) ⭐ 56 | 🐛 37 | 🌐 Python | 📅 2026-10-02 - A collection of agent skills for adding Arize observability and managing tracing, datasets, experiments, and prompt workflows via the Arize ax CLI.

* [OpenAI-Compatible Images](https://github.com/Syh1906/openai-compatible-imagegen) ⭐ 55 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-13 - Generate, edit, and batch-process images through OpenAI-compatible APIs using a standalone skill or a Codex App plugin with a canvas for annotating edit requests.

* [RunAPI MCP Server](https://github.com/runapi-ai/mcp) ⭐ 55 | 🐛 10 | 🌐 TypeScript | 📅 2026-09-30 - MCP server for AI image generation, AI video generation, AI music creation, text-to-speech, prompt search, and model discovery.

* [Sando](https://github.com/yuzushi-dev/sando) ⭐ 54 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-03 - Plugin for Claude Code and Codex that caps oversized tool output, salvages key lines, stores full artifacts, and redacts secrets.

* [Threads Analytics](https://github.com/ridemountainpig/threads-analytics) ⭐ 52 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-04 - Self-hosted Threads analytics dashboard with an OAuth-protected, read-only MCP server for querying synced posts, performance metrics, and follower history.

* [immich-photo-manager](https://github.com/drolosoft/immich-photo-manager) ⭐ 50 | 🐛 0 | 🌐 Python | 📅 2026-10-03 - MCP server and Claude Code plugin for self-hosted Immich photo libraries: CLIP and OCR search, geographic album curation, duplicate detection, people and faces, metadata repair, video frames and PDF photobooks, 94 tools and 13 skills tested live on Immich 2.x and 3.x, also via uvx or Docker.

* [KGLite](https://github.com/kkollsga/kglite) ⭐ 50 | 🐛 1 | 🌐 Rust | 📅 2026-10-04 - Turn datasets large and small into knowledge graphs for AI agent memory, knowledge retrieval, and connected-data analysis, with a high-performance local graph database and a ready-to-use MCP interface.

* [kunglao-agent](https://github.com/amd2g2zz/kunglao-agent) ⭐ 49 | 🐛 59 | 🌐 Python | 📅 2026-10-04 - Reverse-engineering expert agent for binaries, firmware, protocols, and web/JS: MCP servers registered by kunglao-init (ghidra, sequential-thinking, x64dbg, ...), see the MCP supply table under Internals.

* [PANews Agent Toolkit](https://github.com/panewslab/skills) ⭐ 45 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-22 - Crypto and blockchain news discovery, authenticated creator publishing workflows, and page-to-Markdown reading.

* [AnyCap](https://github.com/anycap-ai/anycap) ⭐ 43 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-30 - Multimodal media generation, analysis, live web research, file sharing, and page publishing through one CLI, Agent Skill, and local MCP server.

* [Agent402](https://github.com/MikeyPetrillo/Agent402) ⭐ 41 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-04 - Open-source MCP server and x402 seller: 500+ tools for web search, rendering, PDFs, OCR, market and SEC data, paid per call in USDC or free via proof-of-work, no account or API key.

* [Pronounce](https://github.com/anzy-renlab-ai/pronounce) ⭐ 41 | 🐛 4 | 🌐 Python | 📅 2026-09-01 - Pronounce developer jargon out loud: an MCP server (lookup/search) and skill backed by a 1,721-entry sourced dictionary with IPA, audio, and cited pronunciations for kubectl, nginx, YAML, JWT, and more.

* [Substack MCP](https://github.com/conorbronsdon/substack-mcp) ⭐ 40 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-04 - Safe Substack creator operations across publications: rich drafts, Notes, analytics, and consented subscribers; long-form posts stay draft-only, while Notes publish immediately.

* [claude-dev-suite](https://github.com/claude-dev-suite/claude-dev-suite) ⭐ 39 | 🐛 26 | 🌐 TypeScript | 📅 2026-10-03 - Detects a project's stack and installs the matching agents, framework skills and MCP servers into it, writing each assistant's own config format for Claude Code, Copilot, Cursor, Gemini CLI, Codex CLI, Cline and Kimi Code.

* [Kachilu Browser](https://github.com/kachilu-inc/kachilu-browser) ⭐ 38 | 🐛 3 | 🌐 JavaScript | 📅 2026-05-12 - Anti-bot-aware browser automation for AI agents with MCP tools, CAPTCHA-aware workflows, and WSL2 Windows browser support.

* [Hermes Tweet](https://github.com/Xquik-dev/hermes-tweet) ⭐ 36 | 🐛 2 | 🌐 Python | 📅 2026-09-29 - Hermes Agent X/Twitter plugin for read-first social research, monitoring, and approval-gated actions through Xquik.

* [aginxbrowser](https://github.com/yinnho/aginxbrowser) ⭐ 35 | 🐛 7 | 🌐 Rust | 📅 2026-10-03 - Rust MCP server and HTTP service that lets agents fetch JS-rendered or protected pages as clean markdown, meta-search 14 engines, screenshot, and run persistent logged-in sessions — each session exposes a live view URL so a human can watch and take over with the mouse.

* [PixelLab Pip](https://github.com/Shilo/pixellab-pip) ⭐ 35 | 🐛 1 | 🌐 Python | 📅 2026-10-04 - An unofficial, agent-agnostic Agent Skill for creating, editing, and animating pixel-art assets from plain-language requests, routing each task to PixelLab MCP tools, API endpoints, or editor workflows.

* [Flow Studio Power Automate](https://github.com/ninihen1/power-automate-mcp-skills) ⭐ 34 | 🐛 7 | 🌐 JavaScript | 📅 2026-09-04 - Debug, build, and operate Power Automate flows via FlowStudio MCP with action-level inputs and outputs.

* [Talivia Agent Kit](https://github.com/talivia-group/agent) ⭐ 34 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-01 - Install and verify revenue-first website analytics from Codex, connect payment attribution, and identify which traffic sources and customer journeys become revenue.

* [MorningAI](https://github.com/octo-patch/MorningAI) ⭐ 33 | 🐛 5 | 🌐 Python | 📅 2026-05-16 - AI news tracking skill that monitors 80+ entities across 6 sources (Reddit, HN, GitHub, Hugging Face, arXiv, X) and generates scored daily reports with infographics and message digests.

* [Miro MCP Server](https://github.com/olgasafonova/miro-mcp-server) ⭐ 28 | 🐛 1 | 🌐 Go | 📅 2026-10-02 - Self-hosted single-binary Go MCP server exposing 110 tools for Miro boards, covering stickies, shapes, connectors, frames, mindmaps, flowcharts, tags, and bulk operations, with an essentials profile that trims the preload to 14 tools for smaller context budgets.

* [opencode-cache-hit](https://github.com/zhumengzhu/opencode-cache-hit) ⭐ 28 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-25 - OpenCode sidebar plugin showing prompt cache hit rate, token usage, and cost with sub-agent session rollup.

* [Codex Obsidian](https://github.com/greg-asher/codex-obsidian) ⭐ 27 | 🐛 3 | 📅 2026-04-22 - Local Obsidian note and vault workflows through the official desktop `obsidian` CLI.

* [opencode-agy-auth](https://github.com/anthonyhaussman/opencode-agy-auth) ⭐ 27 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-03 - OpenCode plugin providing OAuth 2.0 authentication, model fetching, and quota tracking for the Antigravity CLI.

* [Kreuzberg](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Local document extraction for 91+ formats with skills for CLI usage, OCR, table extraction, output formats, and a local MCP server.

* [Kreuzberg Cloud](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Managed document extraction for Codex with API-key setup, presigned uploads, job tracking, webhook workflows, and usage guidance.

* [Kreuzcrawl](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Web crawling and scraping for Codex with skills for single-page scraping, site crawls, URL mapping, and headless browser fallback.

* [dotpals](https://github.com/Rikinshah787/dotpals) ⭐ 25 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-04 - Desktop pal and notch that shows what AI coding agents did in plain words, with live diffs, approvals, and flags for .env changes, force-pushes, and two agents editing the same file across Claude Code, Codex, Cursor, Gemini CLI, and OpenCode.

* [agentic-seo](https://github.com/dalroot/agentic-seo) ⭐ 23 | 🐛 7 | 🌐 Python | 📅 2026-09-29 - SEO skill collection for AI coding assistants with 16 sub-skills, 10 specialist agents, and 89 evidence-collection scripts.

* [framewright](https://github.com/smwbev/framewright) ⭐ 23 | 🐛 0 | 🌐 HTML | 📅 2026-09-26 - Agent skill for Claude Code, Codex and Gemini CLI that turns a brief into a short video from code: one self-contained HTML file with deterministic frames, 16 visual styles, rendered by headless Chrome and ffmpeg with a synthesized soundtrack and no footage.

* [Skill-Atlas](https://github.com/danielLublinsky/Skill-Atlas) ⭐ 23 | 🐛 0 | 🌐 Python | 📅 2026-08-16 - A third tier for Claude Code skills — dormant, zero tokens, still findable. Search a graph of your collection instead of preloading it.

* [Mimi Seed](https://github.com/jeonghwanko/mimi-seed-sdk) ⭐ 22 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-03 - App launch ops for Claude Code and Codex: a local MCP server and CLI that drive Google Play, App Store Connect, Firebase, AdMob, and more from local credentials.

* [BoondManager MCP Server](https://github.com/fauguste/boondmanager-mcp-server) ⭐ 21 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-02 - MCP server for the BoondManager staffing ERP/CRM exposing 182 tools, 12 prompts and 22 resources over candidates, resources, opportunities, projects, invoices and expense reports, with stdio and OAuth-protected HTTP transports.

* [Yandex Direct](https://github.com/nebelov/yandex-direct-for-all) ⭐ 21 | 🐛 2 | 🌐 Python | 📅 2026-07-17 - GitHub-ready Codex plugin bundle for Yandex Direct, Wordstat, Metrika, and Roistat.

* [claude-math](https://github.com/vladimirrott/claude-math) ⭐ 20 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-18 - Emit mathematics as copy- and search-safe inline Unicode (∑, ≤, ℝ, x², matrices, set-builder) instead of LaTeX so equations stay legible in the Codex TUI, terminals, and Claude Code.

* [prompt-to-asset](https://github.com/MohamedAbdallah-14/prompt-to-asset) ⭐ 20 | 🐛 20 | 🌐 TypeScript | 📅 2026-09-29 - Route image-generation prompts to 30+ models (DALL-E, Stable Diffusion, Flux, Midjourney, and more) through a single MCP interface. Install: `npm install -g prompt-to-asset`.

* [Cargo Skills](https://github.com/getcargohq/cargo-skills) ⭐ 19 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-03 - GTM engineering for coding agents — 17 skills over the Cargo CLI for lead sourcing, contact enrichment and email verification, lead scoring, CRM sync, buying-signal monitoring, and workspace-as-code.

* [Kindle Highlights](https://github.com/l3a0/claude-plugins) ⭐ 19 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Claude Code skill that exports a book's Kindle highlights to verbatim, location-cited Markdown, recovering the ones Amazon's export limit truncates or hides (macOS).

* [Thermal-Fluid Research Workflow](https://github.com/hanhuark/mechanical-engineering-research-skill) ⭐ 19 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Thermal-fluid mechanical engineering research workflow for literature review, technical writing, data analysis, presentations, proposals, coding, and AI/ML tools.

* [clawock](https://github.com/KCNyu/clawock) ⭐ 17 | 🐛 14 | 🌐 Python | 📅 2026-10-04 - A reusable investment decision-workflow extension that adds evidence-gated, code-settled trading decisions to external agents like Claude Code and OpenClaw.

* [unic](https://github.com/DevopsArtFactory/unic) ⭐ 17 | 🐛 1 | 🌐 Go | 📅 2026-09-29 - Local MCP server exposing read-only AWS inspection tools to AI agents, including capability discovery, Backup vault listing, and context sync previews.

* [SysKnife](https://github.com/lacs-project/sysknife) ⭐ 15 | 🐛 48 | 🌐 Rust | 📅 2026-10-04 - Linux sysadmin co-pilot as an MCP server for Codex: plain-language requests become typed, risk-classified actions that a privileged daemon runs only after out-of-band terminal approval, with an Ed25519-signed audit chain and automatic rollback.

* [Codex Mem](https://github.com/2kDarki/codex-mem) ⭐ 13 | 🐛 3 | 🌐 TypeScript | 📅 2026-03-23 - Automatically capture, compress, and inject session context back into future Codex sessions.

* [Data Product Builder for dbt](https://github.com/entropy-data/dataproduct-builder-dbt) ⭐ 13 | 🐛 2 | 🌐 Shell | 📅 2026-05-28 - Full data-product lifecycle on dbt for Entropy Data: scaffold, audit, and integrate projects with ODCS, ODPS, OpenLineage, and GitHub Actions.

* [Context Pack](https://github.com/Rothschildiuk/context-pack) ⭐ 12 | 🐛 2 | 🌐 Rust | 📅 2026-09-27 - Generate compact first-pass repository briefings for coding agents before deeper exploration.

* [Scholar Feed](https://github.com/YGao2005/scholar-feed-mcp) ⭐ 12 | 🐛 7 | 🌐 TypeScript | 📅 2026-09-29 - MCP server over 600k+ CS/AI/ML papers: rank by citations or forecast rising impact, trace 23.2M citation edges, and pull full text and BibTeX; `npx -y scholar-feed-mcp`.

* [Clera](https://github.com/getclera/mcp) ⭐ 10 | 🐛 0 | 📅 2026-09-21 - Hosted hiring MCP server plus Claude Code, Cursor and Gemini CLI plugins: search 210,000+ vetted startup candidates, review Clera's picks and request intros over OAuth.

* [lemo-mod](https://github.com/lemomo-ai/lemo-mod) ⭐ 10 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-04 - Claude Code plugin bundle: 21 styles for the terminal and desktop app, plus 16 mods (a panel, usage band, message numbers, speech, session recaps and more), with only looks on at install.

* [Val Town](https://github.com/val-town/plugins) ⭐ 10 | 🐛 10 | 🌐 JavaScript | 📅 2026-09-24 - Build and deploy serverless TypeScript on Val Town from Codex — hosted MCP server plus skills for HTTP vals, cron, SQLite, email, OAuth, and React UI.

* [WakeWire](https://github.com/glenncalleja/wakewire) ⭐ 10 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-28 - Push events from GitHub, Gmail, Slack, and any signed webhook (Linear, Sentry, ClickUp) straight into your Codex threads as new turns — event-driven triggers instead of polling, with HMAC verification, deduplication, and a durable delivery queue.

* [ai-memory-skill](https://github.com/syedair/ai-memory-skill) ⭐ 9 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Persistent memory skill for Claude Code and Kiro that auto-loads markdown context and runs a consolidation pass (`npx ai-memory-skill`).

* [Codex SEO](https://github.com/BestLemoon/codex-seo) ⭐ 9 | 🐛 11 | 🌐 Python | 📅 2026-07-03 - Full-stack SEO audits, Google API workflows, backlinks analysis, reporting, and optional MCP extensions for Codex.

* [Rust Reverse Engineering](https://github.com/jingjing2222/rust-reverse-engineering-skill) ⭐ 9 | 🐛 3 | 🌐 Shell | 📅 2026-04-18 - Reverse engineer Rust binaries and libraries: triage targets, demangle symbols, recover crate namespaces, and map panic, unwind, async, and FFI paths.

* [sitemd](https://github.com/sitemd-cc/sitemd) ⚠️ Archived - Build websites from Markdown via MCP — 22 tools for creating pages, generating content, validating, running SEO audits, configuring settings, and deploying static sites to Cloudflare Pages.

* [Unified AI System](https://github.com/happy520ai/unified-ai-system) ⭐ 8 | 🐛 47 | 🌐 JavaScript | 📅 2026-10-04 - Self-hosted AI gateway for Codex with provider-free prompt enhancement, governed MCP tools, and a credential-free Docker path.

* [Apple Productivity](https://github.com/matk0shub/apple-productivity-mcp) ⭐ 7 | 🐛 4 | 🌐 Python | 📅 2026-03-27 - Local Apple Calendar and Reminders tooling for macOS with Codex plugin adapters.

* [Codex Be Serious](https://github.com/lulucatdev/codex-be-serious) ⭐ 7 | 🐛 3 | 🌐 Shell | 📅 2026-06-01 - Enforce formal, textbook-grade written register across all agent output.

* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 7 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-29 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.

* [pi-recall](https://github.com/pratikgajjar/recall) ⭐ 7 | 🐛 0 | 🌐 Go | 📅 2026-10-02 - pi extension that lets an agent search your past AI chat history across Cursor, Claude Code, Codex, and pi, backed by a local SQLite FTS5 index.

* [Upwork Autopilot](https://github.com/klajdikkolaj/upwork-autopilot) ⭐ 7 | 🐛 8 | 🌐 JavaScript | 📅 2026-07-03 - Controlled Upwork job search, qualification, and proposal submission sessions through a dedicated Chrome profile.

* [Dodo Payments](https://github.com/dodopayments/dodo-agent-plugin) ⭐ 6 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-28 - Payments integration for checkouts, subscriptions, and billing with live API and documentation MCP servers with browser OAuth.

* [Ethora](https://github.com/dappros/ethora-mcp-server) ⭐ 6 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-03 - MCP server for the Ethora chat and messaging platform: create and manage apps, chat rooms and users, broadcast messages, and deploy AI agents and RAG chatbots.

* [Antigravity 2.0](https://github.com/comprono/antigravity-2-codex-plugin) ⭐ 5 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-07 - Local Codex bridge for Antigravity desktop with setup checks, model limit summaries, DevTools UI automation, and safe project/chat handoff.

* [AutoCAD Tianzheng Tools](https://github.com/summer521521/AutoCAD_Tianzheng_plugin) ⭐ 5 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to AutoCAD and Tianzheng HVAC through a local MCP server for DWG-aware HVAC drawing inspection and workflow automation.

* [AgentGuards](https://github.com/alelaguard/agentguards-plugins) ⭐ 4 | 🐛 2 | 🌐 Python | 📅 2026-10-03 - LLM security guardrails for Codex with enforcing hooks and MCP tools: jailbreak and prompt-injection detection, web-content scanning, data-exfiltration blocking, and destructive-command authorization.

* [Chrome DevTools](https://github.com/win4r/chrome-devtools-codex-plugin) ⭐ 4 | 🐛 4 | 📅 2026-03-27 - One-click Codex plugin wrapper for chrome-devtools-mcp.

* [Cordon](https://github.com/ilyautov/cordon) ⭐ 4 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-01 - Deterministic trust boundary between untrusted content and agent actions for Claude Code, Gemini CLI, MCP hosts and LangChain that strips the hidden layer, keeps provenance of every piece of data, issues an intent certificate and gates calls against it with no model call anywhere on the hot path, covered by 998 tests over 18 pinned attack vectors.

* [Feishu to Codex](https://github.com/zlsbksdxl/codex-lark) ⭐ 4 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-10 - Connect Codex to Feishu/Lark workflows for Docs, Messenger, Drive, Sheets, Base, Calendar, Tasks, Meetings, Mail, approvals, and more through the official Lark CLI.

* [motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) ⭐ 4 | 🐛 0 | 🌐 HTML | 📅 2026-09-29 - Claude Code skill that turns a short brief into a looping kinetic-typography launch video, written as one self-contained HTML file and rendered locally to MP4 with motion blur and a seamless loop.

* [PapersFlow](https://github.com/papersflow-ai/papersflow-codex-plugin) ⭐ 4 | 🐛 5 | 🌐 JavaScript | 📅 2026-08-29 - Paper discovery, citation verification, graph exploration, and DeepScan analysis.

* [Read Image](https://github.com/ZXY1240/read-image) ⭐ 4 | 🐛 6 | 🌐 Python | 📅 2026-09-28 - Read local images, videos, web pages, and Windows screenshots through Doubao, GLM, or Qwen-compatible vision APIs.

* [Remotion Plugin](https://github.com/tim-osterhus/codex-remotion-plugin) ⭐ 4 | 🐛 2 | 📅 2026-04-03 - Build parameterized Remotion videos in Codex with the official Remotion docs MCP, composition scaffolding, and a data-driven launch-video workflow.

* [Synta MCP](https://github.com/Synta-ai/n8n-mcp-codex-plugin-synta) ⭐ 4 | 🐛 1 | 📅 2026-04-03 - Build, edit, validate, and self-heal n8n workflows with Synta MCP tools and Codex-ready workflow guidance.

* [Task Scheduler](https://github.com/6Delta9/task-scheduler-codex-plugin) ⭐ 4 | 🐛 2 | 🌐 Python | 📅 2026-04-03 - OpenAI Codex plugin and local MCP server for turning task lists into realistic schedules with blocked dates, capacity overrides, overflow tracking, and markdown planning output.

* [Zotero Research Tools](https://github.com/summer521521/Zotero_Research_plugin) ⭐ 4 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to Zotero Desktop for local-library search, citation export, collection and tag inspection, and research workflow support.

* [Agent Vision](https://github.com/zfifteen/agent-vision) ⭐ 3 | 🐛 2 | 🌐 Shell | 📅 2026-07-14 - macOS-only local camera plugin for explicit snapshots, streaming controls, and file-backed image input.

* [Agentgram](https://github.com/jerryfane/agentgram) ⭐ 3 | 🐛 3 | 🌐 Python | 📅 2026-07-28 - Send Telegram messages, files, and forwarded inbox imports from Codex and local AI agents through a Telegram bot token and chat id.

* [AxonFlow](https://github.com/getaxonflow/axonflow-codex-plugin) ⭐ 3 | 🐛 8 | 🌐 Shell | 📅 2026-09-25 - Runtime governance for Codex with policy enforcement on terminal commands, advisory checks for non-terminal tools via skills, PII/secret detection, and compliance-grade audit trails. Self-hosted via Docker.

* [Court Rules](https://github.com/foklepoint/court-rules-mcp) ⭐ 3 | 🐛 0 | 📅 2026-09-30 - Hosted MCP server (<https://mcp.courtrules.app/mcp>) for U.S. federal court rules, judge standing orders, court holidays, and filing checks, with a source citation on every rule.

* [SCVD General Store](https://github.com/seancrecord/scvd-general-store-repo) ⭐ 3 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-02 - Skills and hosted MCP for x402 endpoint preflight, signed receipt verification, and evidence-backed agentic commerce workflows.

* [SolidWorks GPT Plugin](https://github.com/Erfouni/solidworks-GPT-plugin) ⭐ 3 | 🐛 2 | 🌐 Python | 📅 2026-10-03 - Knowledge-backed SolidWorks design and validation workflows for Codex with standards lookup, CAD evidence gates, and consent-based session learning.

* [Whiteboard Video](https://github.com/Matteoikarieth96/whiteboard-video-skill) ⭐ 3 | 🐛 0 | 🌐 HTML | 📅 2026-09-28 - Claude Code skill that turns any topic into a hand-drawn whiteboard explainer video: it interviews you, writes a fact-checked script, offers voice samples (macOS, ElevenLabs, OpenAI or your own recordings), then draws, voices and renders an MP4 locally.

* [AI Command Center](https://github.com/Hredo/ai-command-center) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-01 - Local-first Windows, macOS and Linux command center for Claude Code, Codex, OpenCode, Aider, Gemini CLI, Ollama and 8,000+ API models, with live cost and token analytics (even for Claude Code sessions in other terminals), a side-by-side Arena, real terminals and git per project.

* [Cadence Code](https://github.com/michael-L-i/cadence-code) ⭐ 2 | 🐛 5 | 🌐 Python | 📅 2026-10-02 - Fully local voice conversations for Claude Code, Codex, Cursor, and Antigravity on Apple Silicon, with selectable MLX speech and transcription models.

* [Canvas Apps Plugin Codex](https://github.com/Ratnam-Mishra/canvas-apps-plugin-codex) ⭐ 2 | 🐛 4 | 📅 2026-05-03 - Build and edit Microsoft Power Apps Canvas Apps using natural language and Canvas Authoring MCP server.

* [Command Code Usage](https://github.com/Jovan1666/commandcode-usage) ⭐ 2 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-01 - Shows Command Code plan quota (5-hour, weekly and monthly windows with reset times) inside Claude Code, Codex, ZCode, Grok Build, opencode, pi and DeepSeek Harness, read from local session data so checking your quota costs no quota.

* [DataForge](https://github.com/ianktoo/data-forge) ⭐ 2 | 🐛 11 | 🌐 Python | 📅 2026-09-29 - Turns any website into a quality-scored LLM fine-tuning dataset in JSONL, Parquet or on the Hugging Face Hub, with a CLI and a `dataforge mcp` server exposing tools to scrape, explore, validate, run and inspect a dataset build.

* [Deadbolt](https://github.com/seanebones-lang/deadbolt) ⭐ 2 | 🐛 3 | 🌐 Rust | 📅 2026-10-01 - Local admission gate for software agents with short-lived leases, tool policy, one-shot approval, and operator revocation through Rust, HTTP, and stdio MCP integrations.

* [Maestro: Costguard](https://github.com/mbanderas/costguard) ⭐ 2 | 🐛 7 | 🌐 TypeScript | 📅 2026-09-17 - Cost auditor for Codex that flags CI/cron and cloud-spend waste via read-only provider checks, then previews and applies surgical CI workflow fixes locally without writing to provider accounts or pushing git.

* [MATLAB Simulink Tools](https://github.com/summer521521/MATLAB_Simulink_plugin) ⭐ 2 | 🐛 0 | 🌐 MATLAB | 📅 2026-07-01 - Connects Codex to MATLAB and Simulink through a local MCP server for model inspection, script execution, and engineering workflow automation.

* [OrgX](https://github.com/useorgx/orgx-codex-plugin) ⭐ 2 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-02 - MCP access and initiative-aware skills for organizational workflows.

* [SEO Dungeon](https://github.com/avalonreset/seo-dungeon) ⭐ 2 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - Gamified local SEO audits that turn website issues into 16-bit dungeon battles for Codex, Claude, and Gemini CLI workflows.

* [Sessionbus](https://github.com/antst/sessionbus-peers) ⭐ 2 | 🐛 1 | 🌐 Go | 📅 2026-09-30 - Connects independently started Claude Code, Codex, Grok, Qwen, OpenCode and Kilo sessions and custom tools through an open bus protocol for live messaging and optional managed sessions across products and hosts, while keeping native harnesses.

* [Shots](https://github.com/hitSlop/shots) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-09-29 - Agent-native App Store screenshot, app icon, ASO, and localization workflows through the hosted Shots MCP server.

* [SpringBrand](https://github.com/springbrand-lab/springbrand-agent-setup) ⭐ 2 | 🐛 21 | 🌐 Python | 📅 2026-10-02 - Hosted go-to-market MCP server with setup guides for Claude Code, Codex, Cursor and other agents: social listening across X, TikTok, Instagram, YouTube, Reddit and Xiaohongshu, website traffic and SEO research, company, contact and creator discovery, and copy, image, video and voiceover generation over OAuth, billed per call.

* [agentmailkit](https://github.com/ariaxhan/agentmailkit) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-28 - MCP server for scheduled LLM-written email digests from RSS, web and local sources: tools list\_jobs/run\_job/preview\_job/list\_plugins, local-first, run\_job dry-run by default; `pip install "agentmailkit[mcp]"` then `agentmailkit mcp`.

* [Bilinc](https://github.com/atakanelik34/Bilinc) ⭐ 1 | 🐛 2 | 🌐 Python | 📅 2026-09-30 - Persistent memory for AI agents over MCP: commit, recall, revise, snapshot and roll back agent state with provenance, shared across Claude Code, Claude Desktop and other MCP clients.

* [Chorale](https://github.com/hxy9243/chorale) ⭐ 1 | 🐛 18 | 🌐 TypeScript | 📅 2026-10-04 - An LLM-assisted music sheet analysis and composition local MCP server and a web UI for inspect, annotate, compose, and interactively editing ABC notations for music.

* [Computer Usage Summary](https://github.com/liuyewang/computer-usage-summary-skill) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-03 - Privacy-first, local ActivityWatch reports for app time, AFK time, projects, billable work, and redacted timelines across macOS, Windows, and Linux.

* [CONTAM Tools](https://github.com/summer521521/CONTAM_plugin) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-01 - Runs and inspects CONTAM airflow projects through a local MCP server with project guards, diagnostics, simulation helpers, and bridge workflows.

* [Coolify](https://github.com/Sevi-py/coolify-codex-plugin) ⭐ 1 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-02 - Control Coolify Cloud and self-hosted Coolify instances through API-aware workflow skills and local tools.

* [Exa Web Search](https://github.com/zlsbksdxl/codex-exa) ⭐ 1 | 🐛 2 | 🌐 Shell | 📅 2026-09-30 - Search and fetch current web sources in Codex through the official Exa MCP server with browser OAuth.

* [Hotpath](https://github.com/mourad-baazi/hotpath) ⭐ 1 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-01 - Records an agent's MCP tool calls once and compiles them into a deterministic, editable workflow that drops failed calls, uses AI only at judgment steps, and self-heals when data changes shape.

* [Hyreflow](https://github.com/automindz-solutions/hyreflow-plugins) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-09-23 - Recruitment automation plugin for Codex, Claude Code, Cowork and Cursor with Agent Skills and a remote OAuth MCP server: source, enrich, qualify and sequence candidates, then push them to your ATS on metered credits.

* [nsfw-ai-skill](https://github.com/Spicy-API/nsfw-ai-skill) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-02 - Agent Skill and Claude Code plugin for adult (18+) image, image-to-video and image-edit generation through the SpicyAPI API, with cost quotes before every run and adults-only / consent rules.

* [Nullcost](https://github.com/johnvouros/nullcost-plugin) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-12 - Catalog-backed free-tier, free-trial, and cheap developer-tool recommendations for Codex through bundled skills and MCP tools.

* [opencode-stay-awake](https://github.com/AuroraAeon/opencode-stay-awake) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-23 - OpenCode plugin that holds a system sleep inhibitor while a session is running, using caffeinate on macOS and systemd-inhibit on Linux, and releases it as soon as the work finishes.

* [Ophis](https://github.com/ophis-fi/skills) ⭐ 1 | 🐛 3 | 📅 2026-09-21 - Onchain token swaps for Codex via the hosted Ophis MCP server, MEV-protected and gasless, built on CoW Protocol.

* [Reduck Agents](https://github.com/reduck-ai/agents) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-08-06 - Claude Code plugin marketplace and agent skills that discover, run, and create browser automation scripts through the Reduck MCP in your own logged-in Chrome, with reference agents for GEO audits and SaaS invoice retrieval.

* [site-spec](https://github.com/ariaxhan/site-spec) ⭐ 1 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-02 - MCP server for website audit and auto-fix: 40 checks across SEO, accessibility, privacy, structured data and AI searchability, tools audit\_site/fix\_issue/compile\_spec/list\_checks; `npx -y site-spec-mcp`.

* [ThoughtProof MCP](https://github.com/ThoughtProof/thoughtproof-mcp) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-28 - Local MCP pre-action verification for agents: mandate + proposed action → ALLOW/BLOCK/UNCERTAIN; execute only on ALLOW.

* [YYLO Skills](https://github.com/yylo-dev/yylo-skills) ⭐ 1 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-03 - Reusable agent skills maintained by YYLO: the canonical, independently versioned source for the ledger-tasks, wiki, workflow, artifact, benchmark, understand-project, plan-ledger-tasks and ralph-loop skills used by YYLO CLI and YYLO Ledger.

* [AgentDocStore](https://github.com/koushikginjupally/agentdocstore) ⭐ 0 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-03 - Self-hostable, offline-first versioned document store with a web UI, REST API, and a 16-tool stdio MCP server that catches secrets before they are saved.

* [agentic-finance-graph-mcp](https://github.com/AgenticFinanceGraph/agentic-finance-graph-mcp) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Read-only MCP server and CLI for Agentic Finance Graph, the independent ledger of machine money: which AI agents on Base actually pay, what they really spend, ranks, detections and metric history, free with no API key.

* [Aient](https://github.com/aient-ai/aient-codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-06-02 - AI operations plugin for Codex that connects production telemetry, problem lifecycle context, and remediation workflows through Aient's MCP server.

* [Anywhere](https://github.com/raph559/anywhere) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Self-hosted web app to start, open and stop Claude Code Remote Control sessions on your own Linux, WSL and Windows machines from your phone: pick a device, pick a folder, tap Start.

* [CarsXE](https://github.com/carsxe/carsxe-codex-plugin) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-01 - Decode VINs, license plates, market value, vehicle history, recalls, liens, OBD codes, and more via the CarsXE API.

* [cguard](https://github.com/simon-init/cguard) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-01 - A Claude Code plugin hook that keeps secrets, stray docs and destructive commands out of agent sessions.

* [Clayform](https://github.com/sezginkipel/clayform) ⭐ 0 | 🐛 4 | 🌐 TypeScript | 📅 2026-09-29 - MCP server that lets agents build 3D models from a semantic scene document, look at them through a software renderer, check them with measuring critics, rig and animate them, and export glTF, with no Blender or GPU.

* [Codex Reset](https://github.com/suvadadepolo-blip/codex-reset-mcp) ⭐ 0 | 🐛 0 | 📅 2026-09-24 - Hosted read-only MCP tools for when Codex usage limits reset: 24/48h reset forecast, verified reset record with sources, and outage-vs-limit service status.

* [CoreSpeed](https://github.com/corespeed-io/cs) ⭐ 0 | 🐛 1 | 📅 2026-09-29 - One MCP endpoint with browser sign-in that gives any agent (Claude Code, Codex, Cursor and more) your apps, your team's shared memory and built-in tools for media, web search and social data, with spend caps and an activity log; this plugin adds it to Claude Code and Codex with skills for the cs CLI.

* [Droplinked](https://github.com/droplinked/droplinked-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-05 - Verified-inventory agentic commerce over a hosted MCP server, with merchant and product discovery, agent-initiated checkout, and onchain brand, credit-risk, and repayment attestations.

* [flacli](https://github.com/h-3303/flacli) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-09-21 - CLI, MCP servers and Claude Code plugin that take named albums or a playlist (TIDAL, Deezer, YouTube Music, export files), match them against the local library via MusicBrainz, fetch the missing tracks through the user's own Nicotine+ (Soulseek) client, then file, tag and tidy the library; successor to claude-music.

* [GH Project](https://github.com/zfifteen/gh-project-plugin) ⭐ 0 | 🐛 2 | 🌐 HTML | 📅 2026-05-15 - Create GitHub repositories from Codex with inferred defaults, native menus, explicit confirmation, and deterministic local cloning.

* [GPT-6 Astra Outbound System](https://github.com/heypastel/pastel-outbound-system) ⭐ 0 | 🐛 1 | 📅 2026-10-01 - Codex plugin with 20 outbound skills and 12 agents that catch LinkedIn buying signals, qualify and rank leads, write human-sounding messages and posts, run sequences, and handle replies through the Pastel MCP, with every send approved first.

* [Grabbit](https://github.com/BrainGridAI/grabbit-mcp) ⭐ 0 | 🐛 0 | 📅 2026-09-29 - Hosted screenshot MCP for agents that grabs any URL as a hosted image with no local Chromium.

* [GSC Quick Wins](https://github.com/iniyan/gsc-quick-wins) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-09-29 - Agent Skill that reads a Google Search Console export, finds keywords stuck in positions 4–20, and writes the exact title, meta, H2, FAQ and internal-link fixes, with a zero-dependency Python scorer.

* [HodlJuice](https://github.com/nmorton13/hodljuice-cli) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-04 - Claude Code plugin and `hj` CLI for searching and playing 30,000+ Bitcoin podcast episodes, with a status-line player, /pint and /brew commands, and a hosted MCP server.

* [HProxy MCP](https://github.com/hproxy-com/hproxy-mcp) ⭐ 0 | 🐛 0 | 📅 2026-10-02 - Hosted MCP server, Claude Code plugin and Gemini CLI extension exposing proxy\_list, proxy\_check and ip\_lookup over a keyless, continuously verified free proxy pool, with nothing to install.

* [Lacuna Music](https://github.com/JOYLINK-LTD/lacuna-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-31 - Generate original instrumental music and vocal songs from Codex through the Lacuna MCP server.

* [Launch Fast](https://github.com/BlockchainHB/launchfast_codex_plugin) ⭐ 0 | 🐛 3 | 📅 2026-08-20 - Official Launch Fast plugin adapter for rapid SaaS deployment.

* [mcp-dialect-fix](https://github.com/Salman-Labs/mcp-dialect-fix) ⭐ 0 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-02 - npx stdio proxy that rewrites MCP tool schemas from JSON Schema draft-07 to 2020-12 for Claude Desktop and Cowork, plus an SDK transport wrapper and a CI check.

* [Mnemoverse Memory](https://github.com/mnemoverse/claude-plugin) ⭐ 0 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-02 - Claude Code plugin for hosted AI agent memory over MCP that learns from outcomes: tell it a recalled memory helped or misled and it re-ranks what comes back next, with shared rooms for multi-agent work and browser OAuth sign-in instead of an API key.

* [Mobazha](https://github.com/mobazha/mobazha-skills) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-05-03 - Decentralized e-commerce skills — deploy self-hosted stores, import products from Shopify/Amazon, configure custom domains and Telegram bots, set up Tor privacy, and manage your store via MCP.

* [okaypic-video-skill](https://github.com/okaypic/okaypic-video-skill) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-03 - Claude Code skill and Python toolchain that turns a script into a finished episode through the okaypic.com video API: character reference sheets, batch MiniMax H3 rendering with generated voices, a local timeline editor with English and Chinese captions, and a one-command final cut.

* [OpenProject Codex](https://github.com/varaprasadreddy9676/openproject-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-16 - OpenProject integration for Codex with project, team, work package, bulk workflow, boards, wiki, meeting, attachment, and reporting support.

* [Overleaf LaTeX](https://github.com/MarcoDotIO/overleaf-latex) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-30 - Local MCP/Codex plugin for creating and editing Overleaf projects.

* [ParlayAPI](https://github.com/JacobiusMakes/parlay-api-mcp) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-10-02 - Python MCP server for sports odds, player props, public event discovery, and account usage; account data tools require your own API key and allowances.

* [phone-sms](https://github.com/h-3303/phone-sms) ⭐ 0 | 🐛 0 | 🌐 CSS | 📅 2026-10-02 - MCP server and Claude Code plugin that reads and sends SMS through the user's own Android phone over KDE Connect on the local network, with no cloud relay, sending only after the user approves recipient and text.

* [pi-visor](https://github.com/laveesingh/awesome-pi-extensions) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-02 - Pi extension that collapses every tool call to two lines and each agent run into a bounded two-layer frame you expand by click or Ctrl+O, with a live turn bar and one-line thinking summaries. Install: `pi install npm:pi-visor`.

* [Plancast](https://github.com/sarthakdabhi/plancast) ⭐ 0 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-04 - Local-first macOS CLI that helps developers and researchers turn Markdown, text, PDFs, and public articles into two-host audio briefings.

* [plori](https://github.com/plori-ai/codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-10-01 - Create and drive plori cloud agents (each an AI agent on its own cloud computer) over plori's remote MCP server, with OAuth auto-discovery.

* [Portway](https://github.com/rath/portway) ⭐ 0 | 🐛 0 | 🌐 Rust | 📅 2026-10-04 - A local HTTP proxy for Claude Code, Codex, and OpenAI-compatible endpoints on vLLM or SGLang that sends each turn as a zstd delta against the previous one: about 1 KiB, not the whole context.

* [Ratchet](https://github.com/baisethomas/Ratchet) ⭐ 0 | 🐛 1 | 🌐 Shell | 📅 2026-10-01 - Verification playbook and Claude Code plugin for coding agents at any capability tier: a model-agnostic AGENTS.md contract, a destructive-command guard, a stop gate that runs your checks before "done", and skills that reproduce a bug and prove its regression test can fail; the same skills load in Codex from `.agents/skills/`.

* [Serply Agent Skills](https://github.com/serply-inc/skills) ⭐ 0 | 🐛 2 | 📅 2026-09-28 - Agent Skill and Claude Code plugin that teaches coding agents to pull live Google Search, Scholar, News, Maps, Jobs, Bing, Amazon and Reddit results and scrape URLs to markdown through the Serply API or its hosted MCP server.

* [Storyflo](https://github.com/droplinked/storyflo-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-09-12 - Agentic newsroom over a hosted MCP server with narrated briefings, a news-versus-prediction-market Divergence Index, and a searchable declassified archive.

* [TokRepo Search](https://github.com/henu-wang/tokrepo-codex-plugin) ⭐ 0 | 🐛 4 | 📅 2026-04-02 - Search and install AI assets from TokRepo with a bundled skill and MCP server for Codex.

* [VidSeeds.ai](https://github.com/CarrotGamesStudios/vidseeds-mcp) ⭐ 0 | 🐛 2 | 📅 2026-07-20 - Hosted MCP connector for pre-upload video SEO, metadata optimization, AI thumbnails, and multi-platform publishing with workflow skills for Codex agents.

* [VoiceMoat Skills](https://github.com/prateeks367/voicemoat-skills) ⭐ 0 | 🐛 0 | 📅 2026-10-04 - 26 Agent Skills for LinkedIn and Twitter/X posts that draft in your own voice, audit a post before you publish, fix weak openings, draft comments and replies, read your numbers and plan the week, for Claude Code, Codex and any client that reads SKILL.md.

* [aw1-breaker](https://github.com/MvikManners/aw1-circuit-breaker) - Deterministic out-of-band execution circuit breaker and AST safety proxy for autonomous AI agent tool calls.

* [Mantis](./plugins/deonmenezes/mantishack) - Autonomous bug bounty hunter for authorized engagements — 7-phase FSM (RECON → AUTH → HUNT → CHAIN → VERIFY → GRADE → REPORT), parallel hunter sub-agents, cryptographic scope enforcement, and BLAKE3/Ed25519 Merkle event logs.

* [PDF Monster](https://github.com/jbaehova/pdf-monster) - Analyzes PDFs as extracted text, OCR text, rendered page images, and embedded figures for coding agents.

* [Token Harbor](https://github.com/NickHOI/Token-Harbor) - Turn Codex token usage into Sail Power for a local-first fishing, fleet, and harbor-building companion game.

### Grok Plugins

xAI Grok Build plugins can bundle skills, commands, agents, hooks, MCP servers,
and language-server configuration. A native plugin may include
`.grok-plugin/plugin.json`; install a repository with `grok plugin install
owner/repo --trust`. Add verified community plugins here in alphabetical order.
See the [official xAI plugin marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 276 | 🐛 747 | 🌐 Python | 📅 2026-10-04
and [Grok plugin guide](https://github.com/xai-org/grok-build/blob/main/crates/codegen/xai-grok-pager/docs/user-guide/09-plugins.md) ⭐ 27,218 | 🐛 0 | 🌐 Rust | 📅 2026-09-29
before submitting.

* [hypergrok-trading-desk](https://github.com/galleonlabs/hypergrok-trading-desk) ⭐ 78 | 🐛 1 | 🌐 Python | 📅 2026-10-02 - Seven-agent Hyperliquid trading desk roles and skills for Grok Bot that research, size, execute and review trades with user approval.
* [Grok Imagine Cinematic Studio](https://github.com/FineComputer14451/Grok-Imagine-Cinematic-Studio) ⭐ 31 | 🐛 4 | 🌐 Python | 📅 2026-10-03 - Independent multi-agent cinematic production suite (25 Role-Card agents, 64 skills, Production Bible workflow, Character DNA locking, native Grok Imagine Video 1.5 support) for Grok Build.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 7 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-29 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.
* [BlindOracle](https://github.com/craigmbrown/blindoracle-plugin) ⭐ 0 | 🐛 4 | 📅 2026-10-03 - Joins a Grok Bot or Grok Build agent to the BlindOracle agent marketplace with a free ERC-8004 passport, role-scoped MCP tools, counterparty-risk controls for buying or selling A2A, and two $0.01 settlement proofs anyone can verify.

### Kimi Plugins

Kimi Code plugins package skills, agents, and MCP servers for the Kimi runtime.
Depending on the plugin version, a repository can expose `kimi.plugin.json` or
`.kimi-plugin/plugin.json`; install a GitHub repository with Kimi Code's
`/plugins install https://github.com/owner/repo` command. Add verified community
plugins here in alphabetical order. See the [official Kimi plugin documentation](https://github.com/MoonshotAI/kimi-code/blob/main/docs/en/customization/plugins.md) ⭐ 7,771 | 🐛 1,529 | 🌐 TypeScript | 📅 2026-10-02
before submitting.

* [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-AI-Toolkit) ⭐ 1,130 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-04 - Backend for AI coding agents on Tencent CloudBase — database, auth, and functions via Plugin, Skills & MCP.
* [deja](https://github.com/vshulcz/deja-vu) ⭐ 1,129 | 🐛 30 | 🌐 Go | 📅 2026-10-04 - Recalls the sessions the other coding agents on the machine already wrote to disk, including work from before it was installed, through MCP tools, a `/deja:recall` command and recall on every prompt.
* [GoodMemory](https://github.com/hjqcan/GoodMemory) ⭐ 18 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-03 - Local-first, auditable cross-session project memory for Kimi Code with scoped recall, traceable provenance, and approval-gated writes.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 7 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-29 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.

### DeepSeek Harness Plugins

DeepSeek Harness (DSH) plugins are Cordis modules or npm packages that expose a
`dsh.bundle` manifest and can be installed with `dsh plugin add`. Add verified
community plugins here in alphabetical order. See the [official DeepSeek Harness
plugin tutorial](https://github.com/deepseek-ai/deepseek-harness/blob/master/docs/cordis-tutorial/01-first-plugin.md) ⭐ 243,301 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03
and the [`dsh-plugin` community topic](https://github.com/topics/dsh-plugin) before
submitting a repository.

* [dsh-deja](https://github.com/vshulcz/deja-vu) ⭐ 1,129 | 🐛 30 | 🌐 Go | 📅 2026-10-04 - Brings the session history of nineteen other coding agents into DeepSeek Harness: recall, session digest and per-file history tools over a local index, plus optional automatic recall.
* [dsh-vision-router](https://github.com/ysr666/dsh-vision-router) ⭐ 1,126 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-04 - Gives text-only DeepSeek Harness agents image understanding through a built-in no-key vision chain plus fourteen tools for Q\&A, grounding, OCR, crop, screenshots and pixel diff.
* [humanizer-ru](https://github.com/ilyautov/humanizer-ru) ⭐ 408 | 🐛 4 | 🌐 Python | 📅 2026-10-02 - Text-only `dsh.bundle` that mounts the humanizer-ru Agent Skill into DeepSeek Harness: rewrites Russian text to remove 64 markers of AI generation, with a corpus-calibrated scanner and audit mode; install with `dsh plugin --profile web add humanizer-ru` (npm) or `github:ilyautov/humanizer-ru`.
* [Engramory](https://github.com/tinqiao-oss/engramory) ⭐ 192 | 🐛 1 | 🌐 Python | 📅 2026-09-24 - Curated, file-based long-term memory for DSH agents — plain markdown notes in one store shared across hosts, with the index size cap enforced as a monotonic `ctx.tools.guard()` refusal rather than a reminder. Install: `dsh plugin --profile <name> add dsh-engramory`.
* [dsh-blender-plugin](https://github.com/sixtysevenlf/dsh-blender-plugin) ⭐ 157 | 🐛 1 | 🌐 Python | 📅 2026-09-30 - DSH plugin that lets an AI model drive Blender over a direct TCP channel: viewport frames, custom-angle renders, Python execution, headless offload, and a judgment/acceptance layer (`blender_rt_plan`, 28 families / 183 ops).
* [dsh-config-manager](https://github.com/xiajiajun516/dsh-config-manager) ⭐ 151 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-04 - Backup, restore, export, import, migrate and sync your complete DeepSeek Harness (DSH) configuration — settings, model providers, plugins, MCP servers, skills, agent presets and workspaces — and restore your whole environment on a new machine with one click.
* [dsh-opencode-palette](https://github.com/FeatherHunter/dsh-opencode-palette) ⭐ 42 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-03 - Multi-theme engine for DSH Web with full support for all 38 opencode themes.
* [Vibe-Mathematics](https://github.com/ChongCyrus/Vibe-Mathematics) ⭐ 34 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-04 - Plugin bundle installing four multi-agent math problem-solving and cross-verification agent presets into DeepSeek Harness.
* [dsh-plugin-hub](https://github.com/wingsky-1/dsh-plugin-hub) ⭐ 23 | 🐛 15 | 🌐 TypeScript | 📅 2026-10-03 - Plugin collection for the DeepSeek Harness web GUI: task notifications, provider usage tracking, MCP management, and LAN access.
* [dsh-prompt](https://github.com/FeatherHunter/dsh-prompt) ⭐ 21 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-02 - Prompt toolbox for DeepSeek Harness: preset and custom prompt templates with one-click insert into the conversation.
* [dsh-im-companion](https://github.com/FeatherHunter/dsh-im-companion) ⭐ 18 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-02 - Workspace presence companion for dsh-im: see which workspaces have an assistant on duty and whether they are online.
* [dsh-api-balance](https://github.com/Kihara777/dsh-api-balance) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - API usage-balance panel for DeepSeek Harness: adds a 「Usage / Balance」 tab to the webui usage ring showing the account balance and today / this-month / 30-day cost with charts, acquiring the platform token automatically from local browser sessions.

### ZCode Plugins & Localization

ZCode (Z.ai) ships its desktop UI with en-US/zh-CN dictionaries compiled into
`app.asar`; community packs add further locales on top of an installed app.
Add verified community localization packs and plugins here in alphabetical order.

* **[zcode-ru](https://github.com/warment/zcode-ru) ⭐ 2 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-26** — Russian (ru-RU) localization pack for the ZCode desktop app (3.10.1): 5,018 UI strings (100% of the renderer corpus), third language in the selector with English fallback, one-command installer with backup/restore. MIT.

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

After scaffolding with `$plugin-creator`, use [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 756 | 🐛 139 | 🌐 Python | 📅 2026-10-04 as your quality gate before publishing, review, or distribution.

For skill/plugin authoring workflows, [Codex SkillForge](https://github.com/f0d010c/skillforge) ⭐ 0 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-27 provides an ESLint-style CLI and GitHub Action for scaffolding, linting, smoke-testing, and packaging Codex skills/plugins before publishing.

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
* [HostDeFi](https://hostdefi.com) — free token-safety scanner grading tokens A+–F from on-chain checks (mint/freeze authority, liquidity, holder concentration) across Solana + 7 EVM chains. Keyless REST API, hosted MCP, x402 endpoints.
* [OpenAI's Codex Gets Plugins](https://thenewstack.io/openais-codex-gets-plugins/) - The New Stack ecosystem overview.

## Related Projects

* [Awesome DeepSeek Harness Plugins](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) ⭐ 17,754 | 🐛 610 | 🌐 JavaScript | 📅 2026-10-01 - Community-maintained DSH plugin list and discovery reference.
* [Kimi Code](https://github.com/MoonshotAI/kimi-code) ⭐ 7,771 | 🐛 1,529 | 🌐 TypeScript | 📅 2026-10-02 - Official Kimi Code runtime and plugin documentation.
* [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) ⭐ 1,197 | 🐛 21 | 🌐 JavaScript | 📅 2026-10-04 - Codex-focused catalog that inspired this cross-platform list.
* [xAI Grok Plugin Marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 276 | 🐛 747 | 🌐 Python | 📅 2026-10-04 - Official Grok Build plugin marketplace and catalog format.
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

Every plugin in this list is automatically ingested by the [HOL Plugin Registry](https://hol.org/registry/plugins), which runs each through the [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 756 | 🐛 139 | 🌐 Python | 📅 2026-10-04 to produce a trust score and security analysis.

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

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-10-04._
