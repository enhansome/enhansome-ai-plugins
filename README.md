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

1. **Validate with [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 605 | 🐛 67 | 🌐 Python | 📅 2026-09-14** — recommended local preflight
2. **Add the [HOL scanner GitHub Action](https://github.com/hashgraph-online/ai-plugin-scanner-action) ⭐ 5 | 🐛 1 | 📅 2026-09-14** — recommended for security, optional for listing
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

* [mblode/agent-skills](https://github.com/mblode/agent-skills) ⭐ 113 | 🐛 0 | 🌐 Python | 📅 2026-09-13 - Nobody ships AI slop on purpose. These skills make sure you don't. UI audits, typography, docs, PR review, and releases.

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

* [Planning with Files](https://github.com/OthmanAdi/planning-with-files) ⭐ 26,884 | 🐛 8 | 🌐 Shell | 📅 2026-09-14 - Persistent file-based planning for Claude Code, Codex, and other AI coding agents, preserving task plans, findings, and progress across context loss, crashes, and compaction.
* [Claude Code Skills](https://github.com/alirezarezvani/claude-skills) ⭐ 25,949 | 🐛 17 | 🌐 Python | 📅 2026-08-30 - 223 production-ready skills, 23 agents, and 298 Python tools across 9 domains — engineering, marketing, product, compliance, and more.
* [Browser Harness](https://github.com/browser-use/browser-harness) ⭐ 17,533 | 🐛 341 | 🌐 Python | 📅 2026-09-12 - MCP server and agent skill that connect an AI agent to a real browser through one editable CDP WebSocket.
* [avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) ⭐ 4,378 | 🐛 60 | 🌐 JavaScript | 📅 2026-09-14 - Portable agent skill for auditing and rewriting AI-patterned prose, with an optional local MCP detector that calls no model and sends no text to a network service.
* [Generative Media Skills](https://github.com/SamurAIGPT/Generative-Media-Skills) ⭐ 4,272 | 🐛 4 | 🌐 Shell | 📅 2026-09-08 - 13 skills for image, video, and audio generation using 100+ models - FLUX, Midjourney v7, Veo3, Kling 3.0, Suno, and HunyuanVideo via muapi.ai.
* [Claude Octopus](https://github.com/nyldn/claude-octopus) ⭐ 4,071 | 🐛 4 | 🌐 Shell | 📅 2026-09-12 - Multi-LLM orchestration dispatching to 8 providers (Codex, Gemini, Copilot, Qwen, Perplexity, OpenRouter, Ollama, OpenCode) with Double Diamond workflows, adversarial review, and safety gates.
* [AI Video Transcriber](https://github.com/wendy7756/AI-Video-Transcriber) ⭐ 3,278 | 🐛 9 | 🌐 Python | 📅 2026-08-23 - Transcribe and summarize videos, podcasts, and local media via a Codex plugin, Claude Code skill, and MCP server.
* [MegaLinter](https://github.com/oxsecurity/megalinter) ⭐ 2,586 | 🐛 37 | 🌐 Dockerfile | 📅 2026-09-13 - Set up, run and fix MegaLinter on any repository, covering 100+ linters and formatters for 69+ languages and 23+ formats, in CI or locally, with per-linter fix guides for the agent.
* [Better Harness](https://github.com/QoderAI/better-harness) ⭐ 2,271 | 🐛 15 | 🌐 JavaScript | 📅 2026-09-14 - Evidence-backed workflow analysis for coding agents that turns project and session signals into prioritized, verifiable improvements across supported hosts.
* [mcp-server-kubernetes](https://github.com/Flux159/mcp-server-kubernetes) ⭐ 1,579 | 🐛 9 | 🌐 TypeScript | 📅 2026-09-14 - MCP server for managing Kubernetes clusters via kubectl with tools for get, describe, apply, delete, logs, exec, port-forward, scaling, rollouts, Helm chart operations, and context switching.
* [Brooks Lint](https://github.com/hyhmrright/brooks-lint) ⭐ 1,474 | 🐛 2 | 🌐 HTML | 📅 2026-09-14 - AI code reviews grounded in six classic engineering books — decay risk diagnostics with book citations, severity labels, and four analysis modes (PR review, architecture audit, tech debt, test quality).
* [Antigravity Workspace Template](https://github.com/study8677/antigravity-workspace-template) ⭐ 1,326 | 🐛 5 | 🌐 Python | 📅 2026-09-09 - Multi-agent codebase knowledge graph generator with context-aware planning and automatic scope management — turns codebases into coherent agent workspaces.
* [Aegis](https://github.com/GanyuanRan/Aegis) ⭐ 1,185 | 🐛 4 | 🌐 Python | 📅 2026-09-14 - An agentic skills framework & software development methodology that works: planning, TDD, debugging, and collaboration workflows.
* [spec-superflow](https://github.com/MageByte-Zero/spec-superflow) ⭐ 798 | 🐛 8 | 🌐 JavaScript | 📅 2026-09-02 - Spec-first workflow with nine skills, user-controlled Quick / Hotfix / Tweak / Full paths, auditable recovery commands, hardened delta-spec sync, and guarded review gates.
* [claude-council](https://github.com/hex/claude-council) ⭐ 745 | 🐛 1 | 🌐 Shell | 📅 2026-09-13 - Claude Code plugin that asks Gemini, OpenAI, Grok, Perplexity, Kimi, OpenRouter models, the Codex, Cursor, Grok and Kimi CLIs and a local ollama model the same question in parallel and lines the answers up with a synthesis of where they agree and differ.
* [Boss](https://github.com/echoVic/boss-skill) ⭐ 556 | 🐛 14 | 🌐 TypeScript | 📅 2026-09-13 - BMAD pipeline plugin that orchestrates a full requirements-to-deploy workflow across nine specialist agents with an auditable runtime DAG and quality gates, for Claude Code, Codex, OpenClaw, and Antigravity.
* [token-optimizer](https://github.com/ooples/token-optimizer-mcp) ⭐ 525 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-14 - Spend less context and keep the conclusions across 16 coding clients including Claude Code, Codex, Gemini CLI, Cursor, and Copilot — diff-only re-reads, paths-only search, out-of-context stashing, and a local ledger that measures each tool's actual return.
* [OpenCode Power Pack](https://github.com/waybarrios/opencode-power-pack) ⭐ 505 | 🐛 2 | 🌐 Python | 📅 2026-09-14 - Fifty-four portable development and security workflows for Codex, Claude Code, OpenCode, and Pi, with opt-in native sandbox profiles for safer command execution.
* [Codex Multi Auth](https://github.com/ndycode/codex-multi-auth) ⭐ 495 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-08 - Multi-account OAuth manager for the official Codex CLI with switching, health checks, and recovery tools.
* [MisakaNet](https://github.com/Ikalus1988/MisakaNet) ⭐ 491 | 🐛 43 | 🌐 Python | 📅 2026-09-14 - Git-backed failure-memory for AI coding agents with 290 indexed lessons, MCP server with 5 tools (search, get\_lesson, submit\_usage, submit\_intake, usage\_status), and DeepSeekHarness adapter.
* [AgentOps](https://github.com/boshu2/agentops) ⭐ 436 | 🐛 2 | 🌐 Go | 📅 2026-09-14 - DevOps layer for coding agents with flow, feedback, and memory that compounds between sessions.
* [AgentBridge](https://github.com/raysonmeng/agent-bridge) ⭐ 342 | 🐛 45 | 🌐 TypeScript | 📅 2026-09-13 - Local bidirectional bridge that keeps Claude Code and Codex live as peers in one session, with mid-turn injection and quota-window handoff.
* [Audio Plugin Coder](https://github.com/Noizefield/audio-plugin-coder) ⭐ 318 | 🐛 0 | 🌐 HTML | 📅 2026-09-14 - Agent-agnostic JUCE workflow for building VST3/AU plugins from idea through design, implementation, test, and installer packaging.
* [Reviewable HTML Workbench](https://github.com/u-ichi/reviewable-html-workbench) ⭐ 297 | 🐛 4 | 🌐 Python | 📅 2026-09-10 - Generate reviewable HTML documents, serve previews, collect inline review comments, and feed review outcomes back into agent workflows.
* [Ditto](https://github.com/ohad6k/ditto) ⭐ 290 | 🐛 22 | 🌐 Python | 📅 2026-08-24 - Mines selected evidence from local coding-agent sessions into private work, design, and writing profiles for Codex, Claude Code, and GitHub Copilot.
* [OpenCode Orchestrator](https://github.com/agnusdei1207/opencode-orchestrator) ⭐ 247 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-14 - Multi-agent mission control for OpenCode with Commander, Planner, Worker, and Reviewer workflows.
* [Knowledge Manager](https://github.com/treylom/knowledge-manager) ⭐ 238 | 🐛 1 | 🌐 Python | 📅 2026-09-10 - Extracts and organizes content from web pages, files, Notion, and images into an Obsidian knowledge vault with GraphRAG-backed search, exporting to Notion, Markdown, and PDF.
* [Claude Code for Codex](https://github.com/sendbird/cc-plugin-codex) ⭐ 206 | 🐛 11 | 🌐 JavaScript | 📅 2026-09-14 - Reverse of OpenAI's official Claude-hosted plugin: use Claude Code from Codex for reviews, rescue tasks, tracked background jobs, and hook-powered review gates.
* [lattice](https://github.com/techygarg/lattice) ⭐ 189 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-07 - Composable AI skills framework that infuses clean code, clean architecture, domain-driven design, secure coding, and proper testing into the workflow by default, with scenario-driven guides for getting started, customization, and team use.
* [Oh My Design](https://github.com/3x-haust/oh-my-design) ⭐ 187 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-13 - Evidence-backed design workflow for Claude Code and Codex with reference research, multi-agent reviews, visual QA, and anti-slop guardrails.
* [agent-talk](https://github.com/xhluca/agent-talk) ⭐ 184 | 🐛 1 | 🌐 Python | 📅 2026-09-10 - Skills-based plugin built on the retalk CLI that gives coding agents end-to-end encrypted messaging with other agents, including agents run by other people, across Claude Code, Codex, Antigravity, pi, opencode, and GitHub Copilot CLI.
* [trace-mcp](https://github.com/nikolai-vysotskyi/trace-mcp) ⭐ 175 | 🐛 13 | 🌐 TypeScript | 📅 2026-09-14 - Precomputed code-intelligence graph served over MCP — symbol search, call graphs, change impact, and test mapping as structured answers instead of whole-file reads.
* [claude-remember](https://github.com/Digital-Process-Tools/claude-remember) ⭐ 169 | 🐛 9 | 🌐 Python | 📅 2026-09-14 - Persistent memory for Claude Code with identity, context, and continuity carried across sessions.
* [keep-the-why](https://github.com/oliver-zehentleitner/keep-the-why) ⭐ 158 | 🐛 3 | 🌐 Python | 📅 2026-09-14 - Preserves the reasoning behind a codebase as project memory — decisions, rejected alternatives, workarounds, incident learnings, constraints.
* [codex-profiles](https://github.com/Ducksss/codex-profiles) ⭐ 146 | 🐛 1 | 🌐 Shell | 📅 2026-09-13 - Switch Codex CLI and Desktop accounts with isolated `CODEX_HOME` profile directories instead of copying token files.
* [Suede Creator Skills](https://github.com/JasonColapietro/suede-creator-skills) ⭐ 135 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-13 - An open-source Agent Skills pack for Claude Code and Codex covering multi-agent workflows, code review, design, copy, SEO, app shipping, creator-rights workflows, and local read-only MCP discovery.
* [Krypton](https://github.com/jturntdev/krypton) ⭐ 132 | 🐛 2 | 🌐 Shell | 📅 2026-07-24 - Goal-based planning and proof gate for Codex and Claude Code that turns requests into ownership, cutover, review-gate, and acceptance-evidence plans.
* [humanizer-ru](https://github.com/Vladimir-Human/humanizer-ru) ⭐ 124 | 🐛 1 | 🌐 Python | 📅 2026-09-14 - Deterministic offline diagnostics and safe cleanup of chat-interface copy-paste artifacts in Russian text and Markdown, shipped as an Agent Skill, MCP server, CLI, GitHub Action, and browser demo, with no authorship verdicts.
* [Superloopy](https://github.com/beefiker/superloopy) ⭐ 107 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-14 - Evidence-gated Codex loop harness with specialist skills, including near-pixel authorized website cloning backed by screenshots, assets, build output, and visual QA.
* [2718lab DevKit](https://github.com/2718labs/2718lab-devkit) ⭐ 102 | 🐛 2 | 🌐 Python | 📅 2026-09-06 - Codex-first local MCP server and skill bundle for deterministic project intelligence, durable workflow orchestration, and reusable engineering tools.
* [Coordinate Agents](https://github.com/hogancv/coordinate-agents) ⭐ 102 | 🐛 8 | 🌐 JavaScript | 📅 2026-09-14 - Plugin-first multi-agent coordination tool with a local-first, recoverable Agent Bus and human-gated planning, implementation, review, and release workflows.
* [sci-brain](https://github.com/QuantumBFS/sci-brain) ⭐ 95 | 🐛 6 | 🌐 Python | 📅 2026-09-14 - Research skills plugin for Claude Code, Codex, OpenCode, and pi that surveys literature into a citable knowledge base, brainstorms research ideas, and drafts papers and slides.
* [Sealos](https://github.com/labring/sealos-skills) ⭐ 79 | 🐛 8 | 🌐 Python | 📅 2026-08-14 - Deploy apps to Sealos Cloud from Codex with readiness checks, Dockerfile generation, Compose conversion, image builds, and rollout updates.
* [opencode-skills-collection](https://github.com/FrancoStino/opencode-skills-collection) ⭐ 76 | 🐛 0 | 🌐 Python | 📅 2026-09-14 - OpenCode plugin that bundles 1595+ skills and auto-syncs them locally, loading each on demand via pointer files.
* [Knowl](https://github.com/dat999zx/knowl) ⭐ 74 | 🐛 8 | 🌐 TypeScript | 📅 2026-09-14 - Local-first project memory over MCP for Claude Code, Codex, Cursor and eight other hosts: a SQLite store that retires facts when they change, shares knowledge across linked repos, and retrieves it by hybrid search.
* [taskflow](https://github.com/heggria/taskflow) ⭐ 71 | 🐛 16 | 🌐 TypeScript | 📅 2026-09-11 - Declarative, verifiable DAG orchestration for Grok Build subagents — fan-out, gates, loops, tournaments, approvals, and resumable runs via MCP tools, with intermediate transcripts kept out of context.
* [Mycelium](https://github.com/arjunrajlaboratory/mycelium) ⭐ 67 | 🐛 1 | 🌐 Python | 📅 2026-09-03 - Gives Claude Code and Codex analytical repositories durable memory for decisions, findings, provenance, reusable conventions, and analysis workflows.
* [pstack for Codex](https://github.com/Aqua-123/pstack-for-codex) ⭐ 66 | 🐛 4 | 🌐 TypeScript | 📅 2026-09-11 - Codex-native engineering workflows derived from pstack, with 45 explicit skills and 23 Poteto Mode playbooks.
* [skillsaw](https://github.com/stbenjam/skillsaw) ⭐ 66 | 🐛 5 | 🌐 Python | 📅 2026-09-12 - A configurable linter for agent skills, plugins, and AI coding assistant context.
* [claude-image-gen](https://github.com/guinacio/claude-image-gen) ⭐ 64 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-08 - AI-powered image generation using Google Gemini or OpenAI (gpt-image-2), integrated with Claude Code via Skills or Claude.ai via MCP.
* [dsh-whale-musume](https://github.com/Sutera-Diffusus/dsh-whale-musume) ⭐ 63 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-14 - Whale-girl desktop pet for the DSH Web UI with pat-to-raise growth, work-state poses, 494 dialogue lines, 30 achievements and a built-in settings panel; local-first, zero telemetry.
* [Globalping](https://github.com/jsdelivr/globalping-mcp-server) ⭐ 63 | 🐛 10 | 🌐 TypeScript | 📅 2026-09-04 - Access thousands of probes around the world to run network tests such as ping, traceroute, http, dns and mtr.
* [Craft](https://github.com/drobins25/craft) ⭐ 62 | 🐛 1 | 🌐 Shell | 📅 2026-09-08 - A Claude Code plugin that acts as an intelligent harness for your development workflow: your codebase is read-only by default, every change passes through a Write Gate as planned and approved work, and craft tracks your project's history, design tokens, and decisions locally so Claude learns your taste and architectural preferences over time.
* [MCP Video Analyzer](https://github.com/guimatheus92/mcp-video-analyzer) ⭐ 61 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-13 - Gives agents video input: transcript, key frames, OCR text, metadata, and an annotated timeline from Loom, YouTube, Instagram, TikTok, direct URLs, or a local file, over MCP, a one-shot CLI, or the /video skill.
* [mstar-harness](https://github.com/btspoony/mstar-harness) ⭐ 59 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-14 - Multi-agent code harness plugin that routes work through PM, dev, QC, and QA roles with deterministic workflow gates enforced by a TypeScript engine, installable across dsh, omp, OpenCode, Cursor, Kimi Code, ZCode, and Codex.
* [silica](https://github.com/kiycoh/silica-harness) ⭐ 59 | 🐛 0 | 🌐 Python | 📅 2026-09-11 - Serves an Obsidian vault as the agent's memory over MCP: semantic and literal recall, gated note writing, and hooks that open each session already knowing its vault.
* [Dely](https://github.com/hieuphung97/dely) ⭐ 58 | 🐛 2 | 🌐 Shell | 📅 2026-09-14 - Multi-harness control protocol that turns requests into approved design contracts, orchestrating isolated worker sessions for sequential implementation and independent code reviews under Orca supervision for Claude Code, Codex, Cursor, Antigravity, and other AI coding agents.
* [mcp-local-memory](https://github.com/Beledarian/mcp-local-memory) ⭐ 56 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-26 - A lightweight, powerful local memory server for AI agents supporting text, entities, relations, and time-based recall.
* [Archcore](https://github.com/archcore-ai/plugin) ⭐ 55 | 🐛 16 | 🌐 Shell | 📅 2026-09-12 - Gives coding agents the architecture, rules, and prior decisions of the repo via skills, hooks, and MCP — so new changes land where the project says they belong across Claude Code, Cursor, and Codex CLI.
* [Honcho](https://github.com/plastic-labs/codex-honcho) ⭐ 51 | 🐛 11 | 🌐 TypeScript | 📅 2026-09-01 - Persistent cross-session memory for Codex powered by Honcho — lifecycle hooks capture each session and inject relevant context back at session start, so Codex remembers your preferences, projects, and decisions across restarts.
* [Session Orchestrator](https://github.com/Kanevry/session-orchestrator) ⭐ 51 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-13 - Session orchestration for Claude Code, Codex, and Cursor IDE — structured planning, wave-based execution, VCS integration (GitLab + GitHub), quality gates, and clean session close-out with issue tracking.
* [AI-Native SDLC](https://github.com/bashebr/ai-native-sdlc) ⭐ 49 | 🐛 0 | 🌐 Python | 📅 2026-09-11 - Reusable skill and plugin bundle implementing the AI-native SDLC workflow: plan, design, build, test, deploy, and maintain with human approval gates.
* [Rootly MCP Server](https://github.com/rootlyhq/rootly-mcp-server) ⭐ 45 | 🐛 5 | 🌐 Python | 📅 2026-09-14 - Manage and resolve production incidents from MCP-compatible AI assistants through dynamically generated, access-controlled Rootly API tools.
* [Knowledge Loom](https://github.com/magickaichen/knowledge-loom) ⭐ 43 | 🐛 5 | 🌐 JavaScript | 📅 2026-09-11 - Agent-neutral skills for initializing, auditing, using, and maintaining governed local Markdown knowledge vaults across Agent Skills-compatible runtimes.
* [memi](https://github.com/sarveshsea/memi) ⭐ 43 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-08 - Interface understanding and design-system memory for Codex, Claude Code, Cursor, and MCP agents with UI audits, Tailwind token extraction, shadcn registry workflows, and a bundled Codex plugin.
* [Docflow](https://github.com/MedAdemBHA/docflow) ⭐ 42 | 🐛 1 | 🌐 Shell | 📅 2026-08-15 - Lightweight documentation memory for AI coding agents that scaffolds a 7-category docs tree, runs readiness checks, validates docs before finishing, and keeps a monthly changelog across Claude Code and Codex.
* [Groundwork](https://github.com/etr/groundwork) ⭐ 42 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-12 - Comprehensive skills library for Claude Code and Codex that structures discovery, planning, design, TDD, debugging, validation, collaboration, and shipping.
* [Open PR](https://github.com/TOMOSIA-VIETNAM/open-pr) ⭐ 42 | 🐛 5 | 🌐 Python | 📅 2026-09-12 - AI code review that lands on the pull request itself across GitHub, GitLab, and Bitbucket, learning each repo's conventions to post one review, one fix commit, and in-thread replies from Claude Code, Cursor, Codex, Gemini CLI, or Antigravity.
* [Click](https://github.com/grapefruit0205/click) ⭐ 41 | 🐛 2 | 🌐 Python | 📅 2026-09-13 - Record revision-aware evidence for normal Codex work and optionally bind higher-risk execution to one human-readable approval contract.
* [Waggle](https://github.com/Abhigyan-Shekhar/Waggle-mcp) ⭐ 40 | 🐛 217 | 🌐 Python | 📅 2026-09-11 - Persistent graph-backed conversational memory for Codex that recalls project decisions, constraints, preferences, and outcomes across sessions.
* [iris-agentic-dev](https://github.com/intersystems-community/iris-agentic-dev) ⭐ 38 | 🐛 8 | 🌐 Rust | 📅 2026-09-14 - MCP server giving AI assistants live access to InterSystems IRIS — execute ObjectScript, query globals, inspect productions, run tests, search code, and manage skills.
* [Codebase Recon](https://github.com/yujiachen-y/codebase-recon-skill) ⭐ 37 | 🐛 2 | 📅 2026-04-26 - Analyze git history to understand a codebase before reading any code — auto-scales by repo size and cross-references hotspots with bug magnets to surface high-risk files, bus factor, and team momentum.
* [Open Dynamic Workflows](https://github.com/Suraj1235/open-dynamic-workflows) ⭐ 36 | 🐛 0 | 🌐 JavaScript | 📅 2026-07-09 - Local-first MIT dynamic multi-agent workflows for Codex, OpenCode, Antigravity, Cursor, and VS Code with a daemon, MCP bridge, Codex skills, OpenCode plugin, and bring-your-own-model support.
* [Labtasker](https://github.com/luocfprime/labtasker) ⭐ 35 | 🐛 0 | 🌐 Python | 📅 2026-09-13 - Queue and run independent ML inference, evaluation, and experiment tasks across long-lived Python or command workers with a Claude Code plugin and cross-agent skill.
* [Velith](https://github.com/epicsagas/Velith) ⭐ 35 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-12 - AI-native publishing system with a 6-phase pipeline from ideation to EPUB/PDF across 8 genres.
* [super-token-saver](https://github.com/ww-w-ai/super-token-saver) ⭐ 31 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-07 - Cuts Claude Code and Codex token spend with prompt-cache expiry warnings, zero-cost session restore after compaction, and per-model usage and cost reports.
* [BioNexus](https://github.com/HERRY423/BioNexus) ⭐ 30 | 🐛 11 | 🌐 Python | 📅 2026-09-14 - Warrant-first scientific reliability layer for AI bioinformatics that audits analytical assumptions, calibrates evidence strength, caps unsupported claims, and verifies execution provenance.
* [Designer Skill](https://github.com/Pythoughts-labs/designer-skill) ⭐ 30 | 🐛 18 | 🌐 JavaScript | 📅 2026-09-13 - Plug-and-play MCP that gives your agent UI superpowers. One install: design skill + MCP server, zero config.
* [harness-eval](https://github.com/redhat-community-ai-tools/harness-eval) ⭐ 29 | 🐛 5 | 🌐 Python | 📅 2026-09-14 - Linter tool (static analysis rules) and LLM reviewer for AI agent harness files that runs quality and security health checks, catching cross-component security chains, redundancy, and config drift, and vets individual skills before install, across Claude Code, Cursor, Codex, Copilot, Gemini, and OpenCode.
* [Jump Skills](https://github.com/fabricioctelles/jump-skills) ⭐ 29 | 🐛 0 | 🌐 Shell | 📅 2026-09-10 - Meta-skills that route requests to specialized skills across Claude Code, Codex, Cursor, OpenCode, and other agent hosts.
* [Quality Engineering Skills](https://github.com/RBraga01/Quality-Engineering-Skills) ⭐ 29 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-11 - 22 structured quality engineering skills for automotive and manufacturing: ISO 9001, IATF 16949, AIAG-VDA FMEA, VDA 6.3, PPAP, APQP, SPC, MSA.
* [Stark](https://github.com/f0d010c/stark) ⭐ 29 | 🐛 3 | 🌐 Python | 📅 2026-07-26 - UI/UX design plugin for AI coding agents with product-flow routing, platform-native interface guidance, asset planning, and shipped-reference analysis before code.
* [Vibe Prospecting](https://github.com/explorium-ai/vibeprospecting-plugin) ⭐ 29 | 🐛 3 | 🌐 Shell | 📅 2026-09-08 - Live B2B company and contact intelligence for building lead lists, researching prospects, enriching contacts, and personalizing outreach.
* [Hera Agent Unity](https://github.com/NotNull92/hera-agent-unity) ⭐ 28 | 🐛 0 | 🌐 C# | 📅 2026-08-19 - Controls and verifies a live Unity Editor through a low-token CLI, with scene, asset, Inspector, Play Mode, test, screenshot, and runtime C# workflows for Codex and other coding agents.
* [Agent Guard](https://github.com/JeongJaeSoon/agent-guard) ⭐ 27 | 🐛 2 | 🌐 Shell | 📅 2026-09-14 - Real-time secret-leak guardrails for AI coding agents (Claude Code, Codex), Git hooks, and CI.
* [HOTL Plugin](https://github.com/yimwoo/hotl-plugin) ⭐ 27 | 🐛 1 | 🌐 Shell | 📅 2026-07-06 - Human-on-the-Loop AI coding workflow plugin for Codex, Claude Code, and Cline with structured planning, review, and verification guardrails.
* [geml](https://github.com/geml-spec/geml) ⭐ 26 | 🐛 0 | 🌐 HTML | 📅 2026-09-14 - An agent-native markup language featuring deterministic block-level editing and built-in validation to ensure documents never drift or break during AI operations.
* [ThumbGate](https://github.com/IgorGanapolsky/ThumbGate) ⭐ 26 | 🐛 22 | 🌐 JavaScript | 📅 2026-09-14 - Pre-action infrastructure firewall for AI coding agents: feedback becomes lessons and prevention rules enforced by PreToolUse hooks across Claude Code, Codex, Gemini, and MCP.
* [AgentPack](https://github.com/vishal2612200/agentpack) ⭐ 25 | 🐛 20 | 🌐 Python | 📅 2026-09-14 - Ranks repo context for Codex with likely files, skill recommendations, agent rules, commands, warnings, and compact task-focused packs before editing.
* [claude-supertool](https://github.com/Digital-Process-Tools/claude-supertool) ⭐ 25 | 🐛 27 | 🌐 Python | 📅 2026-09-12 - Batches file, git and tracker operations into one round-trip, collapsing many reads, greps and globs into a single call for fewer output tokens and less wall time.
* [VibePortrait](https://github.com/dadwadw233/VibePortrait) ⭐ 25 | 🐛 2 | 🌐 HTML | 📅 2026-04-08 - Developer personality portrait generator — analyzes AI conversation history to produce MBTI type (16 color themes), capability radar, developer rating, 3-dimension famous match, and a persona skill that lets any AI "think like you".
* [Agent Context OS](https://github.com/conorbronsdon/agent-context-os) ⭐ 24 | 🐛 12 | 🌐 Python | 📅 2026-09-11 - Portable Git-backed context and session workflow layer with first-class Claude Code, Codex, and OpenClaw support plus experimental adapters for Hermes, Cursor, and Devin.
* [Frappe Agent](https://github.com/Dkm0315/frappe-agent) ⭐ 24 | 🐛 3 | 📅 2026-09-13 - Frappe and ERPNext coding, customization, bench, and review intelligence for Codex.
* [Web Search MCP](https://github.com/sydasif/web-search-mcp) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-09-04 - Comprehensive FastMCP server giving LLMs real-time web access across search engines (DuckDuckGo, Exa), social platforms (Reddit, Hacker News, GitHub, X, LinkedIn), and academic tools (arXiv, Wikipedia), with SSRF-protected URL fetching.
* [SOTA Engineering Skills](https://github.com/martinholovsky/SOTA-skills) ⭐ 23 | 🐛 0 | 🌐 Python | 📅 2026-09-14 - Router-mapped library of 40 domain and language skills with BUILD and AUDIT modes, loading only the rules a task needs and ending every rules file in an audit checklist.
* [Vanguard Frontier Agentic](https://github.com/VincentChuWaiChow/vanguard-frontier-agentic) ⭐ 23 | 🐛 3 | 🌐 Rust | 📅 2026-09-14 - Multi-harness marketplace of skills, specialist agents, rules, and MCP references for guarded cloud, platform, compliance, and business workflows.
* [Espresso](https://github.com/mirkobozzetto/espresso) ⭐ 22 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-06 - Full token-saving stack in one plugin - output compression, global rules, RTK hook, Caveman ultra, GitNexus config. Detects existing setup, installs only what's missing. Works on Claude Code and Codex.
* [go-ultimate](https://github.com/Djarvur/go-ultimate) ⭐ 22 | 🐛 2 | 🌐 Go | 📅 2026-09-13 - Opinionated Go skill that routes any Go task (CLI, library, backend service, MCP server, AI agent) to the right architecture, conventions, and review checklist across Claude Code, Codex, Cursor, Grok Build, Copilot CLI, and OpenCode.
* [Supergraph](https://github.com/datit309/supergraph) ⭐ 22 | 🐛 0 | 🌐 Shell | 📅 2026-09-05 - Engineering workflow system for AI coding agents that enforces planning, TDD, verification, review, and architecture-aware decisions with local codebase graph intelligence across Claude Code, Codex CLI, Antigravity, and OpenCode,..
* [mcp-zuul](https://github.com/imatza-rh/mcp-zuul) ⭐ 21 | 🐛 0 | 🌐 Python | 📅 2026-09-14 - MCP server for Zuul CI with 48 tools for build analysis, failure diagnosis, log search, flaky job detection, pipeline status, and live console streaming.
* [RAG Reviewer](https://github.com/mimfort/rag_for_git) ⭐ 21 | 🐛 4 | 🌐 Python | 📅 2026-09-13 - Agentic PR review: hybrid RAG + code graph via MCP, review skills for Codex.
* [UIZZE](https://github.com/uizze/uizze) ⭐ 20 | 🐛 5 | 🌐 JavaScript | 📅 2026-09-11 - Free MIT anti-ui-slop Skill with a product-specific design contract, required UI states, and a hard finish gate; full UIZZE adds live reference search, validation, and audits across 800,000+ real web and iOS screens through its authenticated MCP server at <https://uizze.com/mcp>.
* [Epic Harness](https://github.com/epicsagas/epic-harness) ⭐ 19 | 🐛 6 | 🌐 Rust | 📅 2026-09-11 - Auto-trigger quality skills + self-evolving agent harness — orbit (spec-to-ship), evolve (skill mutation), team (multi-agent), TDD, check, ship, simplify, debug, perf, secure.
* [harmonyos-skills](https://github.com/liasica/harmonyos-skills) ⭐ 19 | 🐛 0 | 🌐 Python | 📅 2026-09-13 - Offline mirror of 16,800+ HarmonyOS NEXT official docs packaged as a Codex / Claude Code skill and MCP server, so AI coding assistants answer ArkTS / ArkUI / API questions with cited sources.
* [Rel.AI MCP](https://github.com/Kyne0328/rel-ai-mcp) ⭐ 19 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-14 - Brings Codex-style coding workflows to ChatGPT Web, connecting it to local development workspaces through MCP while using ChatGPT Web quota instead of Codex quota.
* [vibekit](https://github.com/rizukirr/vibekit) ⭐ 19 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-13 - Evidence-based guardrail pipeline for vibe coding: brainstorm, plan, one fresh agent per task, verify, across Claude Code, Codex, opencode, and Antigravity.
* [coffee-paladin](https://github.com/pawelkwaczynski/coffee-paladin) ⭐ 18 | 🐛 1 | 🌐 Python | 📅 2026-08-29 - Thermal guard for Apple Silicon: pauses hot jobs before the Mac throttles and gates Claude Code, Codex and Gemini CLI before heavy commands.
* [FlexViz](https://github.com/flex-analytics/flexviz) ⭐ 18 | 🐛 21 | 🌐 Python | 📅 2026-09-14 - Interactive cross-filter dashboards for large datasets with a Claude Code skill for agent-driven data exploration.
* [ictfax-mcp](https://github.com/ictinnovations/ictfax-mcp) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for ICTFax. List and track fax transmissions, with opt-in tools to upload documents and send faxes.
* [VASTlint](https://github.com/aleksUIX/vastlint) ⭐ 18 | 🐛 7 | 🌐 Rust | 📅 2026-09-14 - Validate VAST, VMAP, and DAAST ad tags against IAB Tech Lab specs via Gemini CLI, Claude Code, and a hosted MCP server.
* [aide](https://github.com/jmylchreest/aide) ⭐ 17 | 🐛 4 | 🌐 Go | 📅 2026-09-14 - Persistent memory, code intelligence, and multi-agent orchestration for Claude Code, OpenCode, and Codex CLI via skills, hooks, and an MCP server.
* [CommitLore](https://github.com/MongLong0214/commitlore) ⭐ 17 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-14 - Keeps constraints, rejected alternatives, and warnings in Git trailers and serves them back to the agent before it edits a file.
* [A Team](https://github.com/RBraga01/a-team) ⭐ 16 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-09 - Universal multi-agent infrastructure with 25 specialist agents, 16 enforced workflow skills, and a lead orchestrator for Claude Code, Codex CLI, Cursor, and OpenCode.
* [BGS Modding Superpowers](https://github.com/BB-84C/bgs-modding-superpowers) ⭐ 16 | 🐛 2 | 🌐 Python | 📅 2026-09-12 - Agentic Bethesda Game Studio modpack curation toolkit with MCP-driven xEdit conflict audit, MO2 control plane, BA2/BSA and Papyrus tooling, and skills for setup, dev-log, and release-changelog workflows.
* [ejentum-mcp](https://github.com/ejentum/ejentum-mcp) ⭐ 16 | 🐛 2 | 🌐 JavaScript | 📅 2026-06-11 - MCP server exposing reasoning, code, anti-deception, and memory harness tools for Codex.
* [ictcontact-mcp](https://github.com/ictinnovations/ictcontact-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTContact contact center. Monitor outbound campaigns, with opt-in tools to start and stop them.
* [ictdialer-mcp](https://github.com/ictinnovations/ictdialer-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTDialer cloud auto-dialer. Monitor outbound campaigns, with opt-in start and stop controls.
* [ictexam-mcp](https://github.com/ictinnovations/ictexam-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for reading exams, gradebooks, and item analysis, with opt-in tools for AI question-paper parsing and exam publishing.
* [ictpbx-mcp](https://github.com/ictinnovations/ictpbx-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - Read-only MCP server for ICTPBX. Inspect extensions, DID numbers, SIP trunks, tenants, and live PBX statistics.
* [pbx-mcp](https://github.com/ictinnovations/pbx-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-02 - MCP server for Asterisk (AMI) and FreeSWITCH (ESL). Inspect channels, SIP registrations, trunks, and dialplan on a live PBX.
* [SEO Skills AI](https://github.com/seoskillsai/seo-skills-ai) ⭐ 16 | 🐛 3 | 🌐 Python | 📅 2026-09-10 - Universal SEO skill suite and technical audit engine for Claude Code, Cursor, Codex, and other agents, with first-party Python adapters and HOL plugin-scanner CI.
* [Alcove](https://github.com/epicsagas/alcove) ⭐ 15 | 🐛 1 | 🌐 Rust | 📅 2026-09-11 - Local-first MCP server for private project docs with hybrid BM25+vector search, tree-sitter code indexing, and automated linting for team-wide documentation standards.
* [MARGINAL](https://github.com/SignalLayerLabs/Marginal) ⭐ 15 | 🐛 18 | 🌐 Python | 📅 2026-09-11 - Local-first runtime governor for AI coding agents that detects proven no-progress repetition, records decision evidence, starts in Shadow Mode, and earns narrow enforcement only after repository-local evidence.
* [MeMesh](https://github.com/PCIRCLE-AI/memesh) ⭐ 15 | 🐛 30 | 🌐 TypeScript | 📅 2026-09-14 - Local SQLite memory shared by Claude Code, Codex, Gemini, Cursor, and other MCP clients, captured automatically by hooks from real work and injected at the moment the agent acts.
* [TermaGITchi](https://github.com/TevvvB/termagitchi) ⭐ 15 | 🐛 2 | 🌐 Go | 📅 2026-09-09 - Stable per-worktree identity for parallel Claude Code, Codex, and tmux sessions; mood reads repository hygiene, not what the agent is doing.
* [Codex Reviewer](https://github.com/schuettc/codex-reviewer) ⭐ 14 | 🐛 4 | 📅 2026-05-05 - Second-pass review of Claude-driven plans and implementations.
* [Project Autopilot](https://github.com/AlexMi64/codex-project-autopilot) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-04-09 - Turn an idea into a structured project workflow with planning, execution, verification, and handoff.
* [Staff Engineer Mode](https://github.com/sirmarkz/staff-engineer-mode) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-08-01 - Routes engineering design, delivery, reliability, security, operations, and maintenance prompts to focused staff-level specialist guidance for AI coding agents.
* [trigger-tree](https://github.com/Hedde/trigger_tree) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2026-09-14 - Local documentation telemetry for Claude Code and Codex: see which docs your agent actually reads, gate discoverability in CI, and measure instruction adherence.
* [Codex Agenteam](https://github.com/yimwoo/codex-agenteam) ⭐ 13 | 🐛 2 | 🌐 Python | 📅 2026-07-06 - Specialist AI agents (researcher, PM, architect, developer, QA, reviewer) orchestrated as a configurable team pipeline.
* [Kernel](https://github.com/ariaxhan/kernel-claude) ⭐ 13 | 🐛 9 | 🌐 Python | 📅 2026-09-14 - Claude Code plugin marketplace and Codex plugin: hooks that block destructive commands, spawn guards on subagent contracts, agentdb memory with recall-before-act, blind verifiers, deterministic review; install with `/plugin marketplace add ariaxhan/kernel-claude`.
* [NeatContext](https://github.com/XTSoftwareLabs/neatcontext-plugins) ⭐ 13 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-23 - Saves the durable knowledge from Claude Code, Codex, GitHub Copilot, Kimi Code, and pi conversations as structured, reusable contexts you can reconnect in later sessions or share with your team.
* [Claude Watchdog](https://github.com/Temikus/claude-watchdog) ⭐ 12 | 🐛 1 | 🌐 Shell | 📅 2026-09-07 - Stop hook that runs a critical post-mortem on every Claude Code session, cross-checking what was asked against the actual git diff for missed goals, wasted detours, and unverified claims.
* [Hera Agent Godot](https://github.com/NotNull92/hera-agent-godot) ⭐ 12 | 🐛 0 | 🌐 Go | 📅 2026-09-14 - Drives a live Godot 4.x editor through the low-token Hera CLI — scene, node, and signal edits, play control, and runtime QA with verifiable compact JSON output, with the companion addon published on the official Godot Asset Store.
* [i-hate-editing](https://github.com/ranahaani/i-hate-editing) ⭐ 12 | 🐛 0 | 🌐 Python | 📅 2026-09-12 - Claude Code skill that turns raw talking-head footage into a finished cut with local whisper.cpp + ffmpeg (model never watches the pixels).
* [Tool Advisor](https://github.com/dragon1086/claude-skills) ⭐ 12 | 🐛 2 | 🌐 Shell | 📅 2026-04-23 - Read-only meta-skill that scans your MCP servers, skills, plugins, and CLI tools, then suggests up to three ranked approaches (Methodical / Fast / Deep) with a copy-paste Quick Action table.
* [Writer's Loop](https://github.com/xxsang/writers-loop) ⭐ 12 | 🐛 2 | 🌐 JavaScript | 📅 2026-05-09 - Structured AI writing workflow for planning, critique, revision, translation, style distillation, and opt-in local preference learning.
* [Agentic Ship](https://github.com/moasq/agentic-ship) ⭐ 11 | 🐛 12 | 🌐 JavaScript | 📅 2026-09-11 - Cross-host product-development toolkit for Claude Code, Codex, Cursor, Hermes, and OpenClaw with shared rules, specialist roles, service connections, and machine-checked UI, backend, security, and launch gates.
* [Claude Code Harness](https://github.com/dadwadw233/claude-code-harness) ⭐ 11 | 🐛 1 | 📅 2026-04-05 - Harness blueprint skill for turning vague agent ideas into concrete designs for request assembly, control loops, memory, permissions, recovery, and extension planes.
* [Development Skills](https://github.com/reidemeister94/development-skills) ⭐ 11 | 🐛 1 | 🌐 Python | 📅 2026-07-24 - Three-tier triage (PASS\_THROUGH / LIGHT / FULL 4-phase) development workflow for Codex and Claude Code with language auto-detection (Python, Java, TypeScript, Swift, frontend) and a staff-reviewer subagent for fresh-eyes review on every change.
* [Spec-Driven Development](https://github.com/Habib0x0/spec-driven-plugin) ⭐ 11 | 🐛 1 | 🌐 Shell | 📅 2026-05-18 - Three-phase Requirements → Design → Tasks workflow for Claude Code and Codex — EARS notation acceptance criteria, autonomous execution loop, cross-spec dependencies, and post-implementation acceptance testing.
* [Agent Harness Skills](https://github.com/yfge/agent-harness-skills) ⭐ 10 | 🐛 4 | 🌐 Python | 📅 2026-07-14 - Designs agent-ready repository harnesses with entrypoints, validation surfaces, runtime evidence, delivery records, and atomic commit guidance.
* [Casefile](https://github.com/x4cc3/casefile) ⚠️ Archived - Persistent security case tracking for bug bounties, CTFs, and security audits.
* [Clean Room](https://github.com/whit3rabbit/clean-room-skill) ⭐ 10 | 🐛 7 | 🌐 JavaScript | 📅 2026-09-09 - Spec-first clean-room workflow for authorized source analysis, behavioral specs, role separation, and verification without replacement code.
* [Embedded Workbench](https://github.com/AmethystLuna/embedded-workbench) ⭐ 10 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-12 - Embedded C/C++ firmware development toolbox — 7 skills (FreeRTOS, Keil MDK, ARMCLANG, HardFault triage, state machines, LVGL) plus workflow gates and 4 agents for Claude Code, Codex, Cursor, Kimi, OpenCode, and ZCode.
* [LoreConvo](https://github.com/labyrinth-analytics/loreconvo) ⭐ 10 | 🐛 0 | 🌐 Python | 📅 2026-09-05 - Persistent session memory MCP server for Claude — auto-saves and recalls conversation context, decisions, and artifacts across Claude Code, chat, and other surfaces with full-text search.
* [Praxis](https://github.com/ouonet/praxis) ⭐ 10 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-01 - Intent-driven workflow skills for coding agents: describe what done looks like, not the steps. Triage-first design keeps token costs low across design, TDD, debug, review, and release.
* [Salesforce Compound Engineering](https://github.com/divingsbysangam/salesforce-compound-engineering-plugin) ⭐ 10 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-14 - Salesforce-focused compound engineering plugin for Claude Code, Cursor, Codex, and other AI coding tools, with skills-first workflows, parallel persona dispatch, and Apex/LWC/Flow coverage.
* [Stvena](https://github.com/nccapo/stvena) ⭐ 10 | 🐛 0 | 🌐 Go | 📅 2026-09-11 - Terminal workspace for running Codex or Claude Code beside live diffs, full-file review, checks, staging, and precise code feedback.
* [BABOK Analyst](https://github.com/GSkuza/BABOK_ANALYST) ⭐ 8 | 🐛 13 | 🌐 JavaScript | 📅 2026-09-10 - BABOK v3 business analysis agent with 16 MCP tools, a 9-stage pipeline, and human-in-the-loop approval gates.
* [debt-ops](https://github.com/bcanfield/agentic-tech-debt) ⭐ 8 | 🐛 14 | 🌐 Python | 📅 2026-09-14 - Catches AI-introduced tech debt at write-time: hooks log every deferral to a registry in your repo and a review skill ranks paydown by file churn.
* [Simple Man](https://github.com/Maksim-Burtsev/simple-man) ⭐ 8 | 🐛 1 | 🌐 Python | 📅 2026-09-01 - High-compression communication mode for Codex agents that removes filler while preserving search, validation, and implementation effort.
* [Tartiner Labs](https://github.com/tartinerlabs/skills) ⭐ 8 | 🐛 7 | 🌐 Go | 📅 2026-08-23 - Agent skills for git workflows, GitHub automation, security audits, code refactoring, and project tooling.
* [Universal Design Principles](https://github.com/HDeibler/universal-design-principles) ⭐ 8 | 🐛 3 | 🌐 Markdown | 📅 2026-05-03 - Cross-agent UX and product-design marketplace with a root Codex collection plugin, five focused plugin bundles, and 137 Agent Skills for design review, accessibility, layout, interaction, cognition, and product polish.
* [Cover My Repo](https://github.com/sjh9714/cover-my-repo) ⭐ 7 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-23 - Designs three checked GitHub social preview cards with Codex or Cursor, then renders them locally with Chrome.
* [Demo GIF](https://github.com/conorbronsdon/demo-gif-skill) ⭐ 7 | 🐛 0 | 📅 2026-09-07 - Agent Skill that scripts, renders, optimizes, and embeds reproducible demo GIFs for CLI, TUI, web, and library projects using VHS or Playwright plus ffmpeg.
* [Windrunner](https://github.com/shzlw/windrunner) ⭐ 7 | 🐛 0 | 🌐 Java | 📅 2026-09-14 - Self-hosted project workspace with Spring AI, MCP, CLI, and multi-provider AI integrations.
* [Wingman](https://github.com/lsshym/wingman.ai) ⭐ 7 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-08 - Cross-platform AI coding-agent plugin for repo-local project memory, data-contract checks, and project-map discovery before agents edit code.
* [Zagrosi Forge](https://github.com/zagrosi-code/zagrosi-forge) ⭐ 7 | 🐛 1 | 🌐 Python | 📅 2026-09-05 - Decompose broad project briefs into researched plans and implement sectioned work with TDD, quality gates, and traceability.
* [Contorium](https://github.com/ContoriumLabs/contorium) ⭐ 6 | 🐛 1 | 🌐 TypeScript | 📅 2026-07-27 - Runtime continuity layer for AI coding agents, providing persistent workspace state, Git-aware sessions, and MCP-based context retrieval across tools and agent runs.
* [Agent Workflow System](https://github.com/1139030773-cmd/agent-workflow-system) ⭐ 5 | 🐛 1 | 🌐 PowerShell | 📅 2026-06-12 - 一套中文AI工作流系统：7个协作技能 + 行为规范宪法 + 会话恢复机制，模糊目标→可执行任务，全生命周期引导。Codex & Claude Code 双平台，新手友好。
* [ArmorCodex](https://github.com/armoriq/armorCodex) ⭐ 5 | 🐛 28 | 🌐 JavaScript | 📅 2026-09-08 - Intent-based security for Codex with MCP plan registration, policy gating, CSRG cryptographic proofs, and audit logging on `bash` and `apply_patch`.
* [Codex How To](https://github.com/Phelan164/codex-howto) ⭐ 5 | 🐛 5 | 🌐 Python | 📅 2026-09-14 - Engineering-first Codex curriculum and plugin with 9 skills, measured token-efficiency experiments, bounded orchestration, testing, review, and living knowledge maintenance.
* [Codex rg Guard](https://github.com/Rycen7822/codex-rg-guard) ⭐ 5 | 🐛 3 | 🌐 Rust | 📅 2026-05-09 - Budgeted `rg`/`grep` replacement for Codex that narrows broad searches before they waste model context.
* [Dev Skills](https://github.com/Jason-chen-coder/dev-skills) ⭐ 5 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-06 - Team workflow skills for specs, plans, TDD, debugging, verification, review, branch finishing, and design context.
* [LLM Transpile](https://github.com/epicsagas/llm-transpile) ⭐ 5 | 🐛 6 | 🌐 HTML | 📅 2026-09-11 - Auto-compress .md, .html, and .txt files via PostToolUse hook, cutting context usage by up to 40% with zero workflow change.
* [Logic Probe](https://github.com/AmethystLuna/logicprobe) ⭐ 5 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-11 - Design-document & plan claim verification — checks every verifiable claim against the codebase, escalates behavioral claims to executable-model verification, compares before/after models for regression detection, and mines concurrency risk claims.
* [Maestro](https://github.com/mbanderas/maestro) ⭐ 5 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-10 - Opt-in local multi-CLI fusion engine and orchestration doctrine that fans a prompt across model CLIs, then judges and synthesizes one grounded answer.
* [MCP Migration Check](https://github.com/AlpayC/mcp-migration-check) ⭐ 5 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-14 - Deterministic MCP 2026-07-28 migration checker with an agent skill, CLI, GitHub Action, and hosted web probe powered by one rule engine.
* [VillageSQL Skills](https://github.com/villagesql/villagesql-skills) ⭐ 5 | 🐛 1 | 📅 2026-09-14 - Skills for VillageSQL including building extensions from scratch and porting PostgreSQL extensions to VillageSQL.
* [Agentizer](https://github.com/Humiris/wwa-transform) ⭐ 4 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-05 - Turn any website into an AI-powered agentfront with split-pane
* [LinkedIn Animated Infographics](https://github.com/imMamdouhaboammar/linkedin-animated-infographics) ⭐ 4 | 🐛 41 | 🌐 Python | 📅 2026-08-31 - Evidence-safe animated infographic generator with multi-agent design pipeline for LinkedIn.
* [LoreDocs](https://github.com/labyrinth-analytics/loredocs) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-09-08 - Knowledge vault MCP server for Claude — organizes durable project docs, specs, and guides with FTS5 search, tagging, and cross-project context loading.
* [Superpipelines](https://github.com/gustavo-meilus/superpipelines) ⭐ 4 | 🐛 15 | 🌐 JavaScript | 📅 2026-07-15 - Design and run write/review-isolated multi-agent AI pipelines across Codex, Claude Code, OpenCode, Cursor, Windsurf, and Cline.
* [tailtest](https://github.com/avansaber/tailtest-codex) ⭐ 4 | 🐛 10 | 🌐 Python | 📅 2026-06-13 - Hook-powered test generation -- detects files changed during an agent turn and instructs Codex to write and run tests automatically. Zero config, 8 languages.
* [AgiFlow](https://github.com/AgiFlow/ai-plugin) ⭐ 3 | 🐛 1 | 📅 2026-07-10 - Project management workflows for AI coding agents with planning, grooming, task execution, review, and AgiFlow MCP integration.
* [Codex Process Jobs](https://github.com/joelfarthing/codex-process-jobs) ⭐ 3 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-08 - Run long local builds, tests, benchmarks, and inference jobs as durable detached processes with tracked status, bounded results, and completion delivery across Codex surfaces.
* [Context Guard](https://github.com/GreenLv/codex-context-guard) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-09-14 - Preserves authoritative requirements and verification evidence across long-running Codex tasks and context compaction.
* [Context Optimizer](https://github.com/evermeer/context-optimizer) ⭐ 3 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-14 - Keep your coding agent's context small. When a session gets compacted, Context Optimizer reranks the relevant parts, drops duplicates, and compresses the rest with a local ML pipeline (LLMLingua-2 + Sentence Transformers)
* [HOL Guard Plugin](https://github.com/hashgraph-online/hol-guard-plugin) ⭐ 3 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-13 - AI antivirus workflow for Codex, Claude Code, Cursor, Gemini, OpenCode, MCP servers, skills, and plugin release checks with local approvals and receipts.
* [Repo Audit](https://github.com/conorbronsdon/repo-audit) ⭐ 3 | 🐛 0 | 📅 2026-09-07 - Agent Skill that checks whether a repository's README matches its code and whether stated rules are actually enforced, with an opt-in open-source launch workflow.
* [River Review](https://github.com/s977043/river-review) ⭐ 3 | 🐛 25 | 🌐 JavaScript | 📅 2026-09-14 - Versioned Skill Registry of code-review skills driven by a perspective-based review agent (code, security, performance, architecture, testing, adversarial) that verifies findings against the diff.
* [Team Skills Platform](https://github.com/Colin4k1024/tsp) ⭐ 3 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-19 - Role-based team delivery framework — Tech Lead-orchestrated 8-role system with 195+ skills, 27 specialist agents, 80+ commands, hooks, and ECC harness for Claude Code, Codex, and OpenCode.
* [AIBoarding](https://github.com/gustavo-meilus/aiboarding) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Generate, maintain, compress, and audit standard AI-agent onboarding files with AGENTS.md, CLAUDE.md, drift tracking, and lifecycle hooks.
* [Anchor](https://github.com/biefan/anchor) ⭐ 2 | 🐛 2 | 🌐 Shell | 📅 2026-05-22 - Engineering discipline pack for Claude Code & Codex CLI with task-scope locking, anti-drift braking, condition-based codex review, project-CLAUDE.md pitfall writeback, and PreToolUse hooks that block irreversible bash patterns.
* [claude-jit-context](https://github.com/Digital-Process-Tools/claude-jit-context) ⭐ 2 | 🐛 2 | 🌐 Shell | 📅 2026-09-11 - Project knowledge that loads only when it is needed, matched against the prompt, the file being touched, or the tool being run instead of sitting in context all session.
* [Codex Skin Pack Installer](https://github.com/ChannelerH/codex-skin-packs) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-09-08 - Codex plugin and skill that stages verified desktop skin packs from GitHub releases, validates files, and keeps restore guidance visible.
* [Codex Usage and Resets](https://github.com/joelfarthing/codex-usage-and-resets) ⭐ 2 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-08 - Turns Codex usage into planning facts with linear pace, projected exhaustion, banked-reset expirations, and conservative unexpected-reset detection.
* [falsegreen-skill](https://github.com/vinicq/falsegreen-skill) ⭐ 2 | 🐛 5 | 🌐 JavaScript | 📅 2026-09-14 - Finds tests that stay green when the code they cover is broken, applying six ordered judgments over Python, TypeScript, JavaScript, and Robot Framework suites in Codex CLI and Claude Code.
* [GCF Proxy](https://github.com/blackwell-systems/gcf-codex-plugin) ⭐ 2 | 🐛 3 | 📅 2026-09-05 - Save 71% on MCP tool call tokens by wrapping any server with GCF encoding, with session stats hook and setup skill.
* [GrayMatter](https://github.com/ValkyrLabs/GrayMatter) ⭐ 2 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-09 - Durable memory and shared graph state for Codex and OpenClaw agents, with live ValkyrAI schema awareness.
* [kgai](https://github.com/kgaidev/kgai) ⭐ 2 | 🐛 0 | 🌐 Go | 📅 2026-09-14 - Shared decision memory for AI dev teams, an immutable local log of the decisions behind your code, synced over an S3 bucket you own.
* [site-risk-check](https://github.com/kobimantzur/agent-skills) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-09-10 - Zero-dependency skill that scans a live URL for the conditions behind accessibility and privacy demand letters — trackers firing before consent, missing policies, and machine-checkable WCAG gaps — mapped to the jurisdictions the site actually sells to.
* [ssot-check](https://github.com/conorbronsdon/ssot-check) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-09-10 - Agent Skill and dependency-free Python CLI that discovers repeated facts in documentation and checks declared copies against canonical values.
* [Agentry Observability](https://github.com/fr33dr4g0n/agentry-public) ⭐ 1 | 🐛 2 | 🌐 TypeScript | 📅 2026-07-13 - Agent-native product analytics, error logging, and deploy attribution for coding agents through one HTTP API.
* [Antigravity Context Meter](https://github.com/Dunphil692/antigravity-context-meter) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-26 - Real-time 1:1 Cursor-style context meter & zero-loss session migration for Google Antigravity (Desktop HUD & IDE Extension).
* [Bring Your AI Migration Auditor](https://github.com/unitedideas/bringyour-mcp) ⭐ 1 | 🐛 2 | 📅 2026-05-25 - Read-only Codex plugin for auditing Claude Code to Codex migrations before Codex edits code. Checks AGENTS.md/CLAUDE.md scope, hooks, MCP config, skills, secret references, and validation notes.
* [bury-bench](https://github.com/Onur45500/bury-bench) ⭐ 1 | 🐛 7 | 🌐 Python | 📅 2026-09-10 - Deterministic zero-LLM-judge CLI that scores coding-agent replies for answer-burial and builds a Markdown leaderboard.
* [Codex TUI Proof](https://github.com/bnc4vk/codex-tui-proof) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-01 - Visually validate real local terminal UIs in Codex's in-app browser with screenshots and session evidence.
* [dev-harness-kit](https://github.com/sh-ai-x/dev-harness-kit) ⭐ 1 | 🐛 22 | 🌐 Python | 📅 2026-09-14 - Enforced development workflow skills for Codex and Claude Code covering planning, TDD, debugging, review, security, CI, and release.
* [dsh-product-subagent-console](https://github.com/Jokasa7/dsh-product-subagent-console) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-29 - Designs multi-Agent plans, observes real child-session trees, compares approved tasks with runtime attempts, and prepares evidence-backed recovery inside DeepSeek Harness conversations.
* [ictcrm-mcp](https://github.com/ictinnovations/ictcrm-mcp) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTCRM contact database. Read contact groups, with opt-in tools to create contacts and add them to campaigns.
* [LVTD Skills](https://github.com/LVTD-LLC/skills) ⚠️ Archived - Reusable Agent Skills for Codex, Claude Code, and compatible clients, covering Django, Rust, Cookiecutter, SEO, traction, product marketing, and nonfiction publishing workflows.
* [MailAgent](https://github.com/Alex0nder/MailAgent) ⚠️ Archived - Temporary inboxes for Codex — OTP, magic links, signup QA, simulate-first autotests (23 MCP tools).
* [Mermail Skills](https://github.com/Nudgen-Marketing/mermail-skills) ⭐ 1 | 🐛 198 | 🌐 JavaScript | 📅 2026-09-10 - Official Mermail Agent Skills and Codex plugin that connect AI assistants to hosted Mermail MCP for inbox, scheduling, GTM, support, and x402 wallet workflows.
* [Personal Data Protection](https://github.com/AltByteSG/personal-data-protection-skill) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-05-17 - Engineer-facing personal-data-protection compliance reference — Singapore PDPA, Thailand PDPA, Indonesia UU PDP, Malaysia PDPA (Act 709 + 2024 Amendments), Philippines DPA — organised by where in the stack each obligation lands, with checklists, breach-response runbook, and a developer-view divergence table across all five.
* [Registry Broker](https://github.com/hashgraph-online/registry-broker-codex-plugin) ⭐ 1 | 🐛 18 | 🌐 TypeScript | 📅 2026-08-24 - Delegate tasks to specialist AI agents via the HOL Registry, plan, find, summon, and recover sessions.
* [RoadmapSmith](https://github.com/PapiScholz/roadmapsmith) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-13 - Evidence-backed ROADMAP.md workflows for AI coding agents with validation, sync, and roadmap generation across any tech stack.
* [Runtype Skills](https://github.com/runtypelabs/skills) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-14 - Supercharge your coding agent for AI product development — build, deploy, and operate agents, flows, tools, and surfaces on Runtype's managed edge runtime.
* [skill-sync-publisher](https://github.com/liuyewang/skill-sync-publisher) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-28 - Safely synchronize this Codex skill across public agent-skill registries.
* [Spellbook Skills](https://github.com/yyykf/spellbook-skills) ⭐ 1 | 🐛 3 | 🌐 Python | 📅 2026-09-12 - Practical Claude Code and Codex skills for worktrees, PR/MR automation, review cleanup, YApi lookup, and Java DDD guidance.
* [Tandem Workflow Architect](https://github.com/frumu-ai/tandem-codex-plugin) ⭐ 1 | 🐛 2 | 🌐 TypeScript | 📅 2026-05-21 - Plan Tandem workflows in Codex, then validate, preview, and run them through the governed Tandem engine.
* [Unforgit](https://github.com/MiguelMedeiros/unforgit-codex-plugin) ⭐ 1 | 🐛 1 | 📅 2026-09-11 - Git-backed repository memory for Codex and other coding agents via MCP, with durable local knowledge for decisions, conventions, gotchas, and playbooks.
* [Unity Agent Workflows](https://github.com/AUN-PN/unity-agent-workflows) ⭐ 1 | 🐛 1 | 🌐 Shell | 📅 2026-05-19 - Codex plugin and skill for Unity 2D agents that enforces "No proof, no edit" workflows with runtime-owner proof, Teach structure maps, and validation gates.
* [Workflow Kit](https://github.com/Le-Xuan-Thang/workflow-kit) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-06-02 - Full product lifecycle plugin for Claude Code, Codex CLI, and OpenCode: define Vision/Mission/Core → generate workplan → execute with mandatory cross-provider reviewer agents → synthesize deliverables → maintain, with parallel task execution, crash recovery, and AgentOps metrics.
* [Agency Continuity Audit](https://github.com/revertcreations/agency-continuity-audit) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-09-09 - Read-only audit that distinguishes durable agent goals, state, corrections, restart evidence, authority boundaries, scheduler claims, and commercial proof from self-reported health.
* [Agent Deck](https://github.com/not-so-fat/agent-deck) ⭐ 0 | 🐛 12 | 🌐 TypeScript | 📅 2026-09-14 - One MCP for context management: bind self-improving playbooks, MCP tools, and API keys to the session.
* [Agent Guild](https://github.com/AgentTanuki/agent-guild-plugin) ⭐ 0 | 🐛 1 | 📅 2026-09-13 - Vet autonomous agents before delegating work or money, verify portable passports, use escrow, and record signed outcomes across Claude Code, Codex, MCP, A2A, and OpenClaw.
* [Claude Code Codex Plugin](https://github.com/davidq888/claude-code-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-09 - Security-focused Codex plugin that connects to the local Claude Code CLI through MCP with login, status checks, safe-mode prompts, and no credential storage.
* [CodeTruss](https://github.com/DeliriumPulse/codetruss-plugins) ⭐ 0 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-12 - Local-first acceptance gate that checks coding-agent scope, sensitive surfaces, deterministic analyzers, and repository verification from immutable Git snapshots, then writes signed receipts before the PR.
* [Contexo](https://github.com/maheedhar132/Contexo) ⭐ 0 | 🐛 8 | 🌐 TypeScript | 📅 2026-09-08 - Portable AI context and cost control across every AI coding harness.
* [Delx Recovery](https://github.com/davidmosiah/delx-plugins) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-15 - Free recovery and continuity plugin for AI agents: resume prior sessions, capture state, process failures into a recovery plan, and remember across sessions through a hosted MCP server (works in Codex, Claude Code, Cursor, and VS Code).
* [Encore Lite](https://github.com/keegan-dotcom/encore-lite) ⭐ 0 | 🐛 0 | 📅 2026-07-24 - Free end-of-week surprise builder for Claude Code and Codex - the night before your weekly usage cap resets, it reads your recent work and builds one bonus deliverable, delivered as a reveal with an optional weekly scheduled run.
* [FinBridge](https://github.com/Jakechj/finbridge-mcp) ⭐ 0 | 🐛 0 | 📅 2026-09-09 - Remote MCP server for Korean and US market data with filings, screeners, insider activity, and portfolio backtests.
* [Grafana Dashboards-as-Code](https://github.com/jburgess/mcp-grafana) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-27 - Typed Grafana dashboard and panel builders, structural linting, semantic dashboard diff, and scaffold/audit/review recipes exposed over MCP.
* [mcp-md-reader](https://github.com/JoseEstevez520/mcp-md-reader) ⭐ 0 | 🐛 6 | 🌐 JavaScript | 📅 2026-09-13 - MCP server that helps AI agents find Markdown structure and read only the relevant section, metadata, or vault links.
* [metabrain](https://github.com/ariaxhan/metabrain) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-26 - MCP server for agent memory: SQLite, zero dependencies, tools learn/recall/verdict/hypotheses/start\_brief/stats/capture\_error, patterns graduating to hypotheses then preferences; `pip install "metabrain[mcp]"` then `metabrain-mcp --db PATH`.
* [Metis](https://github.com/gkrtjd99/Metis) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-12 - Repository-level engineering orchestrator that delegates bounded discovery, planning, implementation, review, and verification to fresh subagents, isolates mutable tasks in Git worktrees with declared path ownership, and requires evidence-gated completion.
* [Ontoly](https://github.com/0xsarwagya/ontoly-codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-07-21 - Deterministic Software Graph workflows for Codex: architecture review, dependency analysis, request tracing, configuration analysis, and impact analysis.
* [TaskDock](https://github.com/m1nga/taskdock) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-13 - Resume agent tasks from current deliverables and decisions, with portable folders, link repair, and reversible file organization.
* [Tree Ring Memory](https://github.com/TerminallyLazy/tree-ring-memory-codex-plugin) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-09-09 - Local-first memory lifecycle guidance for Codex agents with recall, evidence-backed lessons, privacy-safe memory capture, audit, consolidation, and explicit forgetting.
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

* [ego-browser](https://github.com/citrolabs/ego-lite) ⭐ 15,886 | 🐛 169 | 🌐 JavaScript | 📅 2026-09-11 - Browser automation for AI agents through ego lite, a Chromium browser where agents navigate pages, fill forms, capture screenshots, and extract data in isolated task spaces that reuse the user's existing logins.
* [LinkedIn Skills](https://github.com/sergebulaev/linkedin-skills) ⭐ 2,333 | 🐛 3 | 🌐 Python | 📅 2026-09-14 - Codex-ready LinkedIn marketing bundle with a native .codex-plugin manifest and 11 skills: post writing with 20 tested hook formulas, AI-tell humanizer, pre-publish audit, comment and reply drafting, hook extraction, content planning, profile optimization, engager analytics, and thread monitoring; also works in Claude Code.
* [LetsFG](https://github.com/LetsFG/LetsFG) ⭐ 2,014 | 🐛 6 | 🌐 Python | 📅 2026-09-14 - Flight and hotel search and booking for AI agents across hundreds of airlines and the major booking sites, via a remote MCP server (Claude, ChatGPT, Cursor, Windsurf), CLI, Python/JS SDKs, and an Agent Skill, with free search after a one-time card connection and real airline PNRs on flight bookings.
* [KiCad Happy](https://github.com/aklofas/kicad-happy) ⭐ 1,207 | 🐛 2 | 🌐 Python | 📅 2026-09-13 - KiCad EDA skills for schematic analysis, PCB layout review, component sourcing, BOM management, and manufacturing preparation.
* [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-AI-Toolkit) ⭐ 1,106 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-14 - Backend for AI coding agents on Tencent CloudBase — database, auth, and functions via Plugin, Skills & MCP.
* [Digital Marketing Pro](https://github.com/indranilbanerjee/digital-marketing-pro) ⭐ 815 | 🐛 2 | 🌐 Python | 📅 2026-09-07 - Open-source AI marketing plugin for agencies — 154 skills, 25 specialist agents, 12-Part Strategy Flow, AEO/GEO, GSC AI Performance Report, Google Ads API v24, EU AI Act Article 50 / C2PA compliance.
* [Education Agent Skills](https://github.com/GarethManning/education-agent-skills) ⭐ 766 | 🐛 3 | 🌐 TypeScript | 📅 2026-08-28 - 131 evidence-based education skills for curriculum design, lesson planning, and assessment, with transparent evidence ratings and MCP server.
* [humanizer-ru](https://github.com/ilyautov/humanizer-ru) ⭐ 348 | 🐛 3 | 🌐 Python | 📅 2026-09-14 - Agent skill for Claude Code, Codex, Cursor and Gemini that rewrites Russian text to remove 64 AI-generation markers (bureaucratese, calques, ChatGPT fingerprints), with a corpus-calibrated scanner, audit mode and author-voice calibration.
* [QVeris Agent Toolkit](https://github.com/QVerisAI/qveris-agent-toolkit) ⭐ 263 | 🐛 8 | 🌐 JavaScript | 📅 2026-09-14 - Cross-client MCP toolkit for discovering, inspecting, quoting, and calling external tools with usage and settlement audits.
* [ru-text](https://github.com/talkstream/ru-text) ⭐ 231 | 🐛 1 | 🌐 Shell | 📅 2026-08-28 - Russian text quality — \~1,044 rules for typography, info-style, editorial, UX writing, and business correspondence.
* [Taisly Agent Kit](https://github.com/taisly/agent) ⭐ 219 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-06 - Publish short-form videos to TikTok, Instagram Reels, YouTube Shorts, X, and Facebook from Codex with the Taisly MCP server and bundled social media posting skill.
* [Telnyx](https://github.com/team-telnyx/ai) ⭐ 214 | 🐛 21 | 🌐 TypeScript | 📅 2026-09-14 - Telnyx toolkit for AI agents bundling Claude Code, Cursor, Gemini CLI, and OpenCode plugins, an agent toolkit for OpenAI/LangChain/CrewAI/Vercel AI SDK, a hosted MCP server, and a one-command CLI for messaging, voice, numbers, and account management.
* [Bitbucket CLI](https://github.com/avivsinai/bitbucket-cli) ⭐ 209 | 🐛 4 | 🌐 Go | 📅 2026-09-13 - Manage Bitbucket repos, PRs, branches, issues, webhooks, and pipelines for Data Center and Cloud.
* [X Twitter Scraper](https://github.com/Xquik-dev/x-twitter-scraper) ⭐ 198 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-04 - X/Twitter data, monitored workflows, HMAC webhooks, and MCP access through the Xquik REST API with confirmation-gated write guidance.
* [Codex Usage Tracker](https://github.com/douglasmonsky/codex-usage-tracker) ⭐ 196 | 🐛 11 | 🌐 Python | 📅 2026-08-20 - Track aggregate Codex token usage from local session logs with MCP tools for summaries, session detail, CSV export, and dashboard generation.
* [OC ChatGPT Multi Auth](https://github.com/ndycode/oc-chatgpt-multi-auth) ⭐ 187 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-14 - Codex setup skill and OpenCode plugin for ChatGPT Plus/Pro OAuth, GPT-5/Codex presets, and multi-account failover.
* [Backlot](https://github.com/brekkylab/backlot) ⭐ 174 | 🐛 28 | 🌐 Python | 📅 2026-09-14 - Local emulator for Slack, Gmail, Google Drive, GitHub, Jira, Notion, S3 and other enterprise SaaS APIs, reproducing their response shapes, pagination, auth and per-document ACLs over a corpus you supply, so agents and RAG pipelines can be tested with no vendor account; `backlot mcp` serves every source as MCP tools.
* [AgentCall](https://github.com/pattern-ai-labs/agentcall) ⭐ 155 | 🐛 2 | 🌐 Python | 📅 2026-08-10 - Lets Claude Code, Codex, Cursor, Gemini CLI, and 30+ other agents join Google Meet, Zoom, or Microsoft Teams as a speaking, listening, presenting participant with text-to-speech, live transcripts, screenshare, and an avatar camera feed.
* [Hostinger API MCP](https://github.com/hostinger/api-mcp-server) ⭐ 154 | 🐛 9 | 🌐 TypeScript | 📅 2026-09-14 - Manage Hostinger VPS, domains, DNS, hosting, and billing through MCP tools backed by the official Hostinger API.
* [Miro](https://github.com/miroapp/miro-ai) ⭐ 151 | 🐛 15 | 🌐 TypeScript | 📅 2026-09-10 - Official Miro MCP server and agent integrations for Claude Code, Codex, Gemini CLI, Cursor, and other AI tools — read and write Miro boards, create diagrams, extract context from boards, and generate code from designs.
* [unslop](https://github.com/MohamedAbdallah-14/unslop) ⭐ 137 | 🐛 3 | 🌐 Python | 📅 2026-09-14 - Strip AI writing patterns from text output — removes filler phrases, hedging language, and generic constructs to produce cleaner written content. Install: `npm install -g unslop`.
* [Zero Slop](https://github.com/manavmishra/ZeroSlop) ⭐ 119 | 🐛 5 | 🌐 Python | 📅 2026-09-13 - Say no to AI slop: a human-in-the-loop learning agentic workflow skill that scores text 0-100 for AI slop and rewrites it tastefully, with a standard-library Python scorer that has zero dependencies and runs offline.
* [Langfuse Observability](https://github.com/avivsinai/langfuse-mcp) ⭐ 105 | 🐛 2 | 🌐 Python | 📅 2026-09-10 - Query traces, debug exceptions, analyze sessions, and manage prompts via MCP tools.
* [im-ai-copyeditor](https://github.com/Turtle-Hwan/im-ai-copyeditor) ⭐ 99 | 🐛 0 | 🌐 Python | 📅 2026-09-08 - Korean copyediting skill for coding agents that fixes spelling, translation-style phrasing, AI tone, and style sentence by sentence.
* [Call-E](https://github.com/CALLE-AI/call-e-integrations) ⭐ 95 | 🐛 33 | 🌐 JavaScript | 📅 2026-09-14 - Plan, run, and inspect Call-E phone call workflows from Codex through the calle CLI.
* [Jenkins CLI](https://github.com/avivsinai/jenkins-cli) ⭐ 87 | 🐛 4 | 🌐 Go | 📅 2026-09-14 - GitHub CLI-style interface for Jenkins controllers with jobs, pipelines, runs, logs, artifacts, credentials, and nodes.
* [Agent Message Queue](https://github.com/avivsinai/agent-message-queue) ⭐ 85 | 🐛 12 | 🌐 Go | 📅 2026-09-14 - File-based inter-agent messaging with co-op mode, cross-project federation, and orchestrator integrations.
* [X (Twitter) Skills](https://github.com/sergebulaev/x-skills) ⭐ 77 | 🐛 0 | 🌐 Python | 📅 2026-09-12 - Codex-ready X (Twitter) marketing bundle with a native .codex-plugin manifest: tweet and thread writing with corpus-validated hook formulas (validated against \~450 top tweets), AI-tell humanizer, hook extraction, reply drafting, content planning, and audience insights; also works in Claude Code.
* [Cortex](https://github.com/cdeust/Cortex) ⭐ 73 | 🐛 6 | 🌐 Python | 📅 2026-09-12 - Persistent thermodynamic memory and cognitive-profiling MCP server for Claude Code, Codex, and Gemini CLI — heat/decay dynamics, predictive-coding write gates, knowledge graph, and intent-aware recall across sessions.
* [ScrapeGraph AI](https://github.com/ScrapeGraphAI/just-scrape) ⭐ 59 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-07 - AI-powered web scraping CLI to search, scrape, extract structured JSON, crawl, and monitor web pages via the ScrapeGraph AI API.
* [Azure Cosmos DB Agent Kit](https://github.com/AzureCosmosDB/cosmosdb-agent-kit) ⭐ 54 | 🐛 26 | 🌐 Python | 📅 2026-09-09 - Azure Cosmos DB best-practice skills and MCP tooling for Codex, Claude Code, Cursor, Gemini CLI, Grok Build, Kimi Code, GitHub Copilot, and other Agent Skills-compatible assistants.
* [Nimble](https://github.com/Nimbleway/agent-skills) ⭐ 53 | 🐛 4 | 🌐 Python | 📅 2026-08-26 - Web Search Agents that search, browse, extract, and reason across live pages and return cited, schema-enforced results, with self-learning retrieval that improves accuracy and lowers cost per task on repeat work, plus Search and Extract skills for fast raw web data in Claude Code, Codex, Cursor, and Grok Build.
* [OpenAI-Compatible Images](https://github.com/Syh1906/openai-compatible-imagegen) ⭐ 49 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-13 - Generate, edit, and batch-process images through OpenAI-compatible APIs using a standalone skill or a Codex App plugin with a canvas for annotating edit requests.
* [immich-photo-manager](https://github.com/drolosoft/immich-photo-manager) ⭐ 48 | 🐛 0 | 🌐 Python | 📅 2026-09-03 - MCP server and Claude Code plugin for self-hosted Immich photo libraries: CLIP and OCR search, geographic album curation, duplicate detection, people and faces, metadata repair, video frames and PDF photobooks, 94 tools and 13 skills tested live on Immich 2.x and 3.x, also via uvx or Docker.
* [AnyCap](https://github.com/anycap-ai/anycap) ⭐ 43 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-08 - Multimodal media generation, analysis, live web research, file sharing, and page publishing through one CLI, Agent Skill, and local MCP server.
* [PANews Agent Toolkit](https://github.com/panewslab/skills) ⭐ 42 | 🐛 2 | 🌐 JavaScript | 📅 2026-04-16 - Crypto and blockchain news discovery, authenticated creator publishing workflows, and page-to-Markdown reading.
* [Pronounce](https://github.com/anzy-renlab-ai/pronounce) ⭐ 39 | 🐛 4 | 🌐 Python | 📅 2026-09-01 - Pronounce developer jargon out loud: an MCP server (lookup/search) and skill backed by a 1,721-entry sourced dictionary with IPA, audio, and cited pronunciations for kubectl, nginx, YAML, JWT, and more.
* [Kachilu Browser](https://github.com/kachilu-inc/kachilu-browser) ⭐ 38 | 🐛 3 | 🌐 JavaScript | 📅 2026-05-12 - Anti-bot-aware browser automation for AI agents with MCP tools, CAPTCHA-aware workflows, and WSL2 Windows browser support.
* [Talivia Agent Kit](https://github.com/talivia-group/agent) ⭐ 36 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-01 - Install and verify revenue-first website analytics from Codex, connect payment attribution, and identify which traffic sources and customer journeys become revenue.
* [Hermes Tweet](https://github.com/Xquik-dev/hermes-tweet) ⭐ 34 | 🐛 4 | 🌐 Python | 📅 2026-09-08 - Hermes Agent X/Twitter plugin for read-first social research, monitoring, and approval-gated actions through Xquik.
* [Flow Studio Power Automate](https://github.com/ninihen1/power-automate-mcp-skills) ⭐ 33 | 🐛 6 | 🌐 JavaScript | 📅 2026-09-04 - Debug, build, and operate Power Automate flows via FlowStudio MCP with action-level inputs and outputs.
* [Substack MCP](https://github.com/conorbronsdon/substack-mcp) ⭐ 33 | 🐛 14 | 🌐 TypeScript | 📅 2026-09-14 - Safe Substack creator operations across publications: rich drafts, Notes, analytics, and consented subscribers; long-form posts stay draft-only, while Notes publish immediately.
* [TikTok Skills](https://github.com/sergebulaev/tiktok-skills) ⭐ 33 | 🐛 0 | 🌐 Python | 📅 2026-09-12 - Codex-ready TikTok marketing bundle with a native .codex-plugin manifest and 8 skills: 3-second hook scripting (spoken line plus on-screen text), caption and hashtag writing under the 2,200-char API limit, trend mapping, profile optimization, AI-tell humanizer, and comment drafting; publishes through Publora with approval before anything goes live; also works in Claude Code.
* [MorningAI](https://github.com/octo-patch/MorningAI) ⭐ 30 | 🐛 5 | 🌐 Python | 📅 2026-05-16 - AI news tracking skill that monitors 80+ entities across 6 sources (Reddit, HN, GitHub, Hugging Face, arXiv, X) and generates scored daily reports with infographics and message digests.
* [Kreuzberg](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Local document extraction for 91+ formats with skills for CLI usage, OCR, table extraction, output formats, and a local MCP server.
* [Kreuzberg Cloud](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Managed document extraction for Codex with API-key setup, presigned uploads, job tracking, webhook workflows, and usage guidance.
* [Kreuzcrawl](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Web crawling and scraping for Codex with skills for single-page scraping, site crawls, URL mapping, and headless browser fallback.
* [Codex Obsidian](https://github.com/greg-asher/codex-obsidian) ⭐ 25 | 🐛 3 | 📅 2026-04-22 - Local Obsidian note and vault workflows through the official desktop `obsidian` CLI.
* [Skill-Atlas](https://github.com/danielLublinsky/Skill-Atlas) ⭐ 23 | 🐛 1 | 🌐 Python | 📅 2026-08-16 - A third tier for Claude Code skills — dormant, zero tokens, still findable. Search a graph of your collection instead of preloading it.
* [Yandex Direct](https://github.com/nebelov/yandex-direct-for-all) ⭐ 21 | 🐛 2 | 🌐 Python | 📅 2026-07-17 - GitHub-ready Codex plugin bundle for Yandex Direct, Wordstat, Metrika, and Roistat.
* [BoondManager MCP Server](https://github.com/fauguste/boondmanager-mcp-server) ⭐ 19 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-14 - MCP server for the BoondManager staffing ERP/CRM exposing 182 tools, 12 prompts and 22 resources over candidates, resources, opportunities, projects, invoices and expense reports, with stdio and OAuth-protected HTTP transports.
* [Kindle Highlights](https://github.com/l3a0/claude-plugins) ⭐ 19 | 🐛 1 | 🌐 Python | 📅 2026-09-13 - Claude Code skill that exports a book's Kindle highlights to verbatim, location-cited Markdown, recovering the ones Amazon's export limit truncates or hides (macOS).
* [prompt-to-asset](https://github.com/MohamedAbdallah-14/prompt-to-asset) ⭐ 19 | 🐛 20 | 🌐 TypeScript | 📅 2026-09-11 - Route image-generation prompts to 30+ models (DALL-E, Stable Diffusion, Flux, Midjourney, and more) through a single MCP interface. Install: `npm install -g prompt-to-asset`.
* [Cargo Skills](https://github.com/getcargohq/cargo-skills) ⭐ 18 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-14 - GTM engineering for coding agents — 17 skills over the Cargo CLI for lead sourcing, contact enrichment and email verification, lead scoring, CRM sync, buying-signal monitoring, and workspace-as-code.
* [claude-math](https://github.com/vladimirrott/claude-math) ⭐ 17 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-18 - Emit mathematics as copy- and search-safe inline Unicode (∑, ≤, ℝ, x², matrices, set-builder) instead of LaTeX so equations stay legible in the Codex TUI, terminals, and Claude Code.
* [Thermal-Fluid Research Workflow](https://github.com/hanhuark/mechanical-engineering-research-skill) ⭐ 16 | 🐛 1 | 🌐 Python | 📅 2026-09-11 - Thermal-fluid mechanical engineering research workflow for literature review, technical writing, data analysis, presentations, proposals, coding, and AI/ML tools.
* [unic](https://github.com/DevopsArtFactory/unic) ⭐ 16 | 🐛 3 | 🌐 Go | 📅 2026-09-14 - Local MCP server exposing read-only AWS inspection tools to AI agents, including capability discovery, Backup vault listing, and context sync previews.
* [Codex Mem](https://github.com/2kDarki/codex-mem) ⭐ 13 | 🐛 3 | 🌐 TypeScript | 📅 2026-03-23 - Automatically capture, compress, and inject session context back into future Codex sessions.
* [Context Pack](https://github.com/Rothschildiuk/context-pack) ⭐ 12 | 🐛 3 | 🌐 Rust | 📅 2026-03-19 - Generate compact first-pass repository briefings for coding agents before deeper exploration.
* [Data Product Builder for dbt](https://github.com/entropy-data/dataproduct-builder-dbt) ⭐ 12 | 🐛 2 | 🌐 Shell | 📅 2026-05-28 - Full data-product lifecycle on dbt for Entropy Data: scaffold, audit, and integrate projects with ODCS, ODPS, OpenLineage, and GitHub Actions.
* [SysKnife](https://github.com/lacs-project/sysknife) ⭐ 12 | 🐛 48 | 🌐 Rust | 📅 2026-09-10 - Linux sysadmin co-pilot as an MCP server for Codex: plain-language requests become typed, risk-classified actions that a privileged daemon runs only after out-of-band terminal approval, with an Ed25519-signed audit chain and automatic rollback.
* [Scholar Feed](https://github.com/YGao2005/scholar-feed-mcp) ⭐ 11 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-08 - MCP server over 600k+ CS/AI/ML papers: rank by citations or forecast rising impact, trace 23.2M citation edges, and pull full text and BibTeX; `npx -y scholar-feed-mcp`.
* [Val Town](https://github.com/val-town/plugins) ⭐ 10 | 🐛 9 | 🌐 JavaScript | 📅 2026-09-14 - Build and deploy serverless TypeScript on Val Town from Codex — hosted MCP server plus skills for HTTP vals, cron, SQLite, email, OAuth, and React UI.
* [Codex SEO](https://github.com/BestLemoon/codex-seo) ⭐ 9 | 🐛 11 | 🌐 Python | 📅 2026-07-03 - Full-stack SEO audits, Google API workflows, backlinks analysis, reporting, and optional MCP extensions for Codex.
* [Rust Reverse Engineering](https://github.com/jingjing2222/rust-reverse-engineering-skill) ⭐ 9 | 🐛 3 | 🌐 Shell | 📅 2026-04-18 - Reverse engineer Rust binaries and libraries: triage targets, demangle symbols, recover crate namespaces, and map panic, unwind, async, and FFI paths.
* [sitemd](https://github.com/sitemd-cc/sitemd) ⭐ 9 | 🐛 2 | 🌐 HTML | 📅 2026-06-25 - Build websites from Markdown via MCP — 22 tools for creating pages, generating content, validating, running SEO audits, configuring settings, and deploying static sites to Cloudflare Pages.
* [WakeWire](https://github.com/glenncalleja/wakewire) ⭐ 9 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-14 - Push events from GitHub, Gmail, Slack, and any signed webhook (Linear, Sentry, ClickUp) straight into your Codex threads as new turns — event-driven triggers instead of polling, with HMAC verification, deduplication, and a durable delivery queue.
* [Codex Be Serious](https://github.com/lulucatdev/codex-be-serious) ⭐ 7 | 🐛 3 | 🌐 Shell | 📅 2026-06-01 - Enforce formal, textbook-grade written register across all agent output.
* [Apple Productivity](https://github.com/matk0shub/apple-productivity-mcp) ⭐ 6 | 🐛 4 | 🌐 Python | 📅 2026-03-27 - Local Apple Calendar and Reminders tooling for macOS with Codex plugin adapters.
* [AutoCAD Tianzheng Tools](https://github.com/summer521521/AutoCAD_Tianzheng_plugin) ⭐ 6 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to AutoCAD and Tianzheng HVAC through a local MCP server for DWG-aware HVAC drawing inspection and workflow automation.
* [Dodo Payments](https://github.com/dodopayments/dodo-agent-plugin) ⭐ 6 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-14 - Payments integration for checkouts, subscriptions, and billing with live API and documentation MCP servers with browser OAuth.
* [Unified AI System](https://github.com/happy520ai/unified-ai-system) ⭐ 6 | 🐛 13 | 🌐 JavaScript | 📅 2026-09-14 - Self-hosted AI gateway for Codex with provider-free prompt enhancement, nine governed MCP tools, and a credential-free Docker path.
* [Upwork Autopilot](https://github.com/klajdikkolaj/upwork-autopilot) ⭐ 6 | 🐛 8 | 🌐 JavaScript | 📅 2026-07-03 - Controlled Upwork job search, qualification, and proposal submission sessions through a dedicated Chrome profile.
* [Chrome DevTools](https://github.com/win4r/chrome-devtools-codex-plugin) ⭐ 5 | 🐛 4 | 📅 2026-03-27 - One-click Codex plugin wrapper for chrome-devtools-mcp.
* [Antigravity 2.0](https://github.com/comprono/antigravity-2-codex-plugin) ⭐ 4 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-07 - Local Codex bridge for Antigravity desktop with setup checks, model limit summaries, DevTools UI automation, and safe project/chat handoff.
* [PapersFlow](https://github.com/papersflow-ai/papersflow-codex-plugin) ⭐ 4 | 🐛 5 | 🌐 JavaScript | 📅 2026-08-29 - Paper discovery, citation verification, graph exploration, and DeepScan analysis.
* [Read Image](https://github.com/ZXY1240/read-image) ⭐ 4 | 🐛 6 | 🌐 Python | 📅 2026-09-14 - Read local images, videos, web pages, and Windows screenshots through Doubao, GLM, or Qwen-compatible vision APIs.
* [Remotion Plugin](https://github.com/tim-osterhus/codex-remotion-plugin) ⭐ 4 | 🐛 2 | 📅 2026-04-03 - Build parameterized Remotion videos in Codex with the official Remotion docs MCP, composition scaffolding, and a data-driven launch-video workflow.
* [Synta MCP](https://github.com/Synta-ai/n8n-mcp-codex-plugin-synta) ⭐ 4 | 🐛 1 | 📅 2026-04-03 - Build, edit, validate, and self-heal n8n workflows with Synta MCP tools and Codex-ready workflow guidance.
* [Task Scheduler](https://github.com/6Delta9/task-scheduler-codex-plugin) ⭐ 4 | 🐛 2 | 🌐 Python | 📅 2026-04-03 - OpenAI Codex plugin and local MCP server for turning task lists into realistic schedules with blocked dates, capacity overrides, overflow tracking, and markdown planning output.
* [Agent Vision](https://github.com/zfifteen/agent-vision) ⭐ 3 | 🐛 2 | 🌐 Shell | 📅 2026-07-14 - macOS-only local camera plugin for explicit snapshots, streaming controls, and file-backed image input.
* [Agentgram](https://github.com/jerryfane/agentgram) ⭐ 3 | 🐛 3 | 🌐 Python | 📅 2026-07-28 - Send explicit Telegram messages from Codex and local AI agents through a Telegram bot token and chat id.
* [AxonFlow](https://github.com/getaxonflow/axonflow-codex-plugin) ⭐ 3 | 🐛 4 | 🌐 Shell | 📅 2026-09-14 - Runtime governance for Codex with policy enforcement on terminal commands, advisory checks for non-terminal tools via skills, PII/secret detection, and compliance-grade audit trails. Self-hosted via Docker.
* [Feishu to Codex](https://github.com/zlsbksdxl/codex-lark) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-10 - Connect Codex to Feishu/Lark workflows for Docs, Messenger, Drive, Sheets, Base, Calendar, Tasks, Meetings, Mail, approvals, and more through the official Lark CLI.
* [Zotero Research Tools](https://github.com/summer521521/Zotero_Research_plugin) ⭐ 3 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to Zotero Desktop for local-library search, citation export, collection and tag inspection, and research workflow support.
* [AgentGuards](https://github.com/alelaguard/agentguards-plugins) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-08-30 - LLM security guardrails for Codex with enforcing hooks and MCP tools: jailbreak and prompt-injection detection, web-content scanning, data-exfiltration blocking, and destructive-command authorization.
* [Cadence Code](https://github.com/michael-L-i/cadence-code) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-09-08 - Fully local voice conversations for Claude Code, Codex, Cursor, and Antigravity on Apple Silicon, with selectable MLX speech and transcription models.
* [Canvas Apps Plugin Codex](https://github.com/Ratnam-Mishra/canvas-apps-plugin-codex) ⭐ 2 | 🐛 4 | 📅 2026-05-03 - Build and edit Microsoft Power Apps Canvas Apps using natural language and Canvas Authoring MCP server.
* [Cordon](https://github.com/ilyautov/cordon) ⭐ 2 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-12 - Deterministic trust boundary between untrusted content and agent actions for Claude Code, Gemini CLI, MCP hosts and LangChain that strips the hidden layer, keeps provenance of every piece of data, issues an intent certificate and gates calls against it with no model call anywhere on the hot path, covered by 998 tests over 18 pinned attack vectors.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-09 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.
* [Maestro: Costguard](https://github.com/mbanderas/costguard) ⭐ 2 | 🐛 7 | 🌐 TypeScript | 📅 2026-09-03 - Cost auditor for Codex that flags CI/cron and cloud-spend waste via read-only provider checks, then previews and applies surgical CI workflow fixes locally without writing to provider accounts or pushing git.
* [OrgX](https://github.com/useorgx/orgx-codex-plugin) ⭐ 2 | 🐛 6 | 🌐 JavaScript | 📅 2026-09-04 - MCP access and initiative-aware skills for organizational workflows.
* [Shots](https://github.com/hitSlop/shots) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-09-08 - Agent-native App Store screenshot, app icon, ASO, and localization workflows through the hosted Shots MCP server.
* [agentmailkit](https://github.com/ariaxhan/agentmailkit) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-28 - MCP server for scheduled LLM-written email digests from RSS, web and local sources: tools list\_jobs/run\_job/preview\_job/list\_plugins, local-first, run\_job dry-run by default; `pip install "agentmailkit[mcp]"` then `agentmailkit mcp`.
* [Computer Usage Summary](https://github.com/liuyewang/computer-usage-summary-skill) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-03 - Privacy-first, local ActivityWatch reports for app time, AFK time, projects, billable work, and redacted timelines across macOS, Windows, and Linux.
* [CONTAM Tools](https://github.com/summer521521/CONTAM_plugin) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-01 - Runs and inspects CONTAM airflow projects through a local MCP server with project guards, diagnostics, simulation helpers, and bridge workflows.
* [Coolify](https://github.com/Sevi-py/coolify-codex-plugin) ⭐ 1 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-11 - Control Coolify Cloud and self-hosted Coolify instances through API-aware workflow skills and local tools.
* [Exa Web Search](https://github.com/zlsbksdxl/codex-exa) ⭐ 1 | 🐛 2 | 🌐 Shell | 📅 2026-09-09 - Search and fetch current web sources in Codex through the official Exa MCP server with browser OAuth.
* [MATLAB Simulink Tools](https://github.com/summer521521/MATLAB_Simulink_plugin) ⭐ 1 | 🐛 0 | 🌐 MATLAB | 📅 2026-07-01 - Connects Codex to MATLAB and Simulink through a local MCP server for model inspection, script execution, and engineering workflow automation.
* [Nullcost](https://github.com/johnvouros/nullcost-plugin) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-12 - Catalog-backed free-tier, free-trial, and cheap developer-tool recommendations for Codex through bundled skills and MCP tools.
* [Ophis](https://github.com/ophis-fi/skills) ⭐ 1 | 🐛 3 | 📅 2026-09-07 - Onchain token swaps for Codex via the hosted Ophis MCP server, MEV-protected and gasless, built on CoW Protocol.
* [SEO Dungeon](https://github.com/avalonreset/seo-dungeon) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-10 - Gamified local SEO audits that turn website issues into 16-bit dungeon battles for Codex, Claude, and Gemini CLI workflows.
* [site-spec](https://github.com/ariaxhan/site-spec) ⭐ 1 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-11 - MCP server for website audit and auto-fix: 40 checks across SEO, accessibility, privacy, structured data and AI searchability, tools audit\_site/fix\_issue/compile\_spec/list\_checks; `npx -y site-spec-mcp`.
* [ThoughtProof MCP](https://github.com/ThoughtProof/thoughtproof-mcp) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-14 - Local MCP pre-action verification for agents: mandate + proposed action → ALLOW/BLOCK/UNCERTAIN; execute only on ALLOW.
* [Aient](https://github.com/aient-ai/aient-codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-06-02 - AI operations plugin for Codex that connects production telemetry, problem lifecycle context, and remediation workflows through Aient's MCP server.
* [CarsXE](https://github.com/carsxe/carsxe-codex-plugin) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-10 - Decode VINs, license plates, market value, vehicle history, recalls, liens, OBD codes, and more via the CarsXE API.
* [Droplinked](https://github.com/droplinked/droplinked-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-05 - Verified-inventory agentic commerce over a hosted MCP server, with merchant and product discovery, agent-initiated checkout, and onchain brand, credit-risk, and repayment attestations.
* [GH Project](https://github.com/zfifteen/gh-project-plugin) ⭐ 0 | 🐛 2 | 🌐 HTML | 📅 2026-05-15 - Create GitHub repositories from Codex with inferred defaults, native menus, explicit confirmation, and deterministic local cloning.
* [Lacuna Music](https://github.com/JOYLINK-LTD/lacuna-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-31 - Generate original instrumental music and vocal songs from Codex through the Lacuna MCP server.
* [Launch Fast](https://github.com/BlockchainHB/launchfast_codex_plugin) ⭐ 0 | 🐛 3 | 📅 2026-08-20 - Official Launch Fast plugin adapter for rapid SaaS deployment.
* [Mobazha](https://github.com/mobazha/mobazha-skills) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-05-03 - Decentralized e-commerce skills — deploy self-hosted stores, import products from Shopify/Amazon, configure custom domains and Telegram bots, set up Tor privacy, and manage your store via MCP.
* [OpenProject Codex](https://github.com/varaprasadreddy9676/openproject-codex-plugin) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-16 - OpenProject integration for Codex with project, team, work package, bulk workflow, boards, wiki, meeting, attachment, and reporting support.
* [ParlayAPI](https://github.com/JacobiusMakes/parlay-api-mcp) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-09-11 - Python MCP server for sports odds, player props, public event discovery, and account usage; account data tools require your own API key and allowances.
* [plori](https://github.com/plori-ai/codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-09-14 - Create and drive plori cloud agents (each an AI agent on its own cloud computer) over plori's remote MCP server, with OAuth auto-discovery.
* [SolidWorks GPT Plugin](https://github.com/Erfouni/solidworks-GPT-plugin) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-08-24 - Knowledge-backed SolidWorks design and validation workflows for Codex with standards lookup, CAD evidence gates, and consent-based session learning.
* [Storyflo](https://github.com/droplinked/storyflo-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-09-12 - Agentic newsroom over a hosted MCP server with narrated briefings, a news-versus-prediction-market Divergence Index, and a searchable declassified archive.
* [TokRepo Search](https://github.com/henu-wang/tokrepo-codex-plugin) ⭐ 0 | 🐛 4 | 📅 2026-04-02 - Search and install AI assets from TokRepo with a bundled skill and MCP server for Codex.
* [VidSeeds.ai](https://github.com/CarrotGamesStudios/vidseeds-mcp) ⭐ 0 | 🐛 2 | 📅 2026-07-20 - Hosted MCP connector for pre-upload video SEO, metadata optimization, AI thumbnails, and multi-platform publishing with workflow skills for Codex agents.
* [Mantis](./plugins/deonmenezes/mantishack) - Autonomous bug bounty hunter for authorized engagements — 7-phase FSM (RECON → AUTH → HUNT → CHAIN → VERIFY → GRADE → REPORT), parallel hunter sub-agents, cryptographic scope enforcement, and BLAKE3/Ed25519 Merkle event logs.
* [PDF Monster](https://github.com/jbaehova/pdf-monster) - Analyzes PDFs as extracted text, OCR text, rendered page images, and embedded figures for coding agents.
* [Token Harbor](https://github.com/NickHOI/Token-Harbor) - Turn Codex token usage into Sail Power for a local-first fishing, fleet, and harbor-building companion game.

### Grok Plugins

xAI Grok Build plugins can bundle skills, commands, agents, hooks, MCP servers,
and language-server configuration. A native plugin may include
`.grok-plugin/plugin.json`; install a repository with `grok plugin install
owner/repo --trust`. Add verified community plugins here in alphabetical order.
See the [official xAI plugin marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 247 | 🐛 424 | 🌐 Python | 📅 2026-09-14
and [Grok plugin guide](https://github.com/xai-org/grok-build/blob/main/crates/codegen/xai-grok-pager/docs/user-guide/09-plugins.md) ⭐ 26,739 | 🐛 0 | 🌐 Rust | 📅 2026-09-09
before submitting.

* [Grok Imagine Cinematic Studio](https://github.com/FineComputer14451/Grok-Imagine-Cinematic-Studio) ⭐ 27 | 🐛 4 | 🌐 Python | 📅 2026-09-12 - Independent multi-agent cinematic production suite (25 Role-Card agents, 64 skills, Production Bible workflow, Character DNA locking, native Grok Imagine Video 1.5 support) for Grok Build.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-09 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.

### Kimi Plugins

Kimi Code plugins package skills, agents, and MCP servers for the Kimi runtime.
Depending on the plugin version, a repository can expose `kimi.plugin.json` or
`.kimi-plugin/plugin.json`; install a GitHub repository with Kimi Code's
`/plugins install https://github.com/owner/repo` command. Add verified community
plugins here in alphabetical order. See the [official Kimi plugin documentation](https://github.com/MoonshotAI/kimi-code/blob/main/docs/en/customization/plugins.md) ⭐ 7,372 | 🐛 1,369 | 🌐 TypeScript | 📅 2026-09-14
before submitting.

* [deja](https://github.com/vshulcz/deja-vu) ⭐ 811 | 🐛 37 | 🌐 Go | 📅 2026-09-14 - Recalls the sessions the other coding agents on the machine already wrote to disk, including work from before it was installed, through MCP tools, a `/deja:recall` command and recall on every prompt.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-09 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.

### DeepSeek Harness Plugins

DeepSeek Harness (DSH) plugins are Cordis modules or npm packages that expose a
`dsh.bundle` manifest and can be installed with `dsh plugin add`. Add verified
community plugins here in alphabetical order. See the [official DeepSeek Harness
plugin tutorial](https://github.com/deepseek-ai/deepseek-harness/blob/master/docs/cordis-tutorial/01-first-plugin.md) ⭐ 223,781 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-11
and the [`dsh-plugin` community topic](https://github.com/topics/dsh-plugin) before
submitting a repository.

* [dsh-deja](https://github.com/vshulcz/deja-vu) ⭐ 811 | 🐛 37 | 🌐 Go | 📅 2026-09-14 - Brings the session history of nineteen other coding agents into DeepSeek Harness: recall, session digest and per-file history tools over a local index, plus optional automatic recall.
* [humanizer-ru](https://github.com/ilyautov/humanizer-ru) ⭐ 348 | 🐛 3 | 🌐 Python | 📅 2026-09-14 - Text-only `dsh.bundle` that mounts the humanizer-ru Agent Skill into DeepSeek Harness: rewrites Russian text to remove 64 markers of AI generation, with a corpus-calibrated scanner and audit mode; install with `dsh plugin --profile web add humanizer-ru` (npm) or `github:ilyautov/humanizer-ru`.
* [Engramory](https://github.com/tinqiao-oss/engramory) ⭐ 190 | 🐛 1 | 🌐 Python | 📅 2026-09-08 - Curated, file-based long-term memory for DSH agents — plain markdown notes in one store shared across hosts, with the index size cap enforced as a monotonic `ctx.tools.guard()` refusal rather than a reminder. Install: `dsh plugin --profile <name> add dsh-engramory`.
* [dsh-config-manager](https://github.com/xiajiajun516/dsh-config-manager) ⭐ 113 | 🐛 8 | 🌐 TypeScript | 📅 2026-09-13 - Backup, restore, export, import, migrate and sync your complete DeepSeek Harness (DSH) configuration — settings, model providers, plugins, MCP servers, skills, agent presets and workspaces — and restore your whole environment on a new machine with one click.

### ZCode Plugins & Localization

ZCode (Z.ai) ships its desktop UI with en-US/zh-CN dictionaries compiled into
`app.asar`; community packs add further locales on top of an installed app.
Add verified community localization packs and plugins here in alphabetical order.

* **[zcode-ru](https://github.com/warment/zcode-ru) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-05** — Russian (ru-RU) localization pack for the ZCode desktop app (3.10.1): 5,018 UI strings (100% of the renderer corpus), third language in the selector with English fallback, one-command installer with backup/restore. MIT.

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

After scaffolding with `$plugin-creator`, use [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 605 | 🐛 67 | 🌐 Python | 📅 2026-09-14 as your quality gate before publishing, review, or distribution.

For skill/plugin authoring workflows, [Codex SkillForge](https://github.com/f0d010c/skillforge) ⭐ 0 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-13 provides an ESLint-style CLI and GitHub Action for scaffolding, linting, smoke-testing, and packaging Codex skills/plugins before publishing.

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

* [Awesome DeepSeek Harness Plugins](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) ⭐ 15,685 | 🐛 240 | 🌐 Python | 📅 2026-09-13 - Community-maintained DSH plugin list and discovery reference.
* [Kimi Code](https://github.com/MoonshotAI/kimi-code) ⭐ 7,372 | 🐛 1,369 | 🌐 TypeScript | 📅 2026-09-14 - Official Kimi Code runtime and plugin documentation.
* [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) ⭐ 1,013 | 🐛 19 | 🌐 Python | 📅 2026-09-14 - Codex-focused catalog that inspired this cross-platform list.
* [xAI Grok Plugin Marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 247 | 🐛 424 | 🌐 Python | 📅 2026-09-14 - Official Grok Build plugin marketplace and catalog format.
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

Every plugin in this list is automatically ingested by the [HOL Plugin Registry](https://hol.org/registry/plugins), which runs each through the [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 605 | 🐛 67 | 🌐 Python | 📅 2026-09-14 to produce a trust score and security analysis.

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

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-14._
