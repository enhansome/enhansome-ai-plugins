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
  * [Agent Skills](#agent-skills)
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

1. **Validate with [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 995 | 🐛 100 | 🌐 Python | 📅 2026-10-25** — recommended local preflight
2. **Add the [HOL scanner GitHub Action](https://github.com/hashgraph-online/ai-plugin-scanner-action) ⭐ 9 | 🐛 1 | 📅 2026-10-25** — recommended for security, optional for listing
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

* [mblode/agent-skills](https://github.com/mblode/agent-skills) ⭐ 164 | 🐛 0 | 🌐 Shell | 📅 2026-10-25 - Nobody ships AI slop on purpose. These skills make sure you don't. UI audits, typography, docs, PR review, and releases.

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

Community-built plugins, native skills, MCP servers, and related agent extensions. [PRs welcome](#contributing)!

### Agent Skills

Individually installable Agent Skills collections, rather than one client-specific plugin bundle.

* [claude-skills](https://github.com/Jeffallan/claude-skills) ⭐ 12,056 | 🐛 40 | 🌐 Python | 📅 2026-10-24 - 67 Agent Skills for full-stack development across languages, frameworks, infrastructure, testing, security, and data/ML, with 371 reference files that load only when a task needs them and 9 project workflow commands.
* [MARS](https://github.com/andrea-magni/MARS) ⭐ 400 | 🐛 1 | 🌐 Pascal | 📅 2026-10-21 - Agent Skills for the MARS-Curiosity Delphi REST library that help AI coding agents scaffold MARS servers, develop REST APIs and MCP servers, and implement servers from OpenAPI documents with MARSgen.
* [image-use](https://github.com/leeguooooo/image-use) ⭐ 399 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Agent skill and zero-dependency CLI for generating and editing images with existing ChatGPT or Gemini accounts, with reference images, reusable styles and looping animations without an API key.
* [ui-craft](https://github.com/educlopez/ui-craft) ⭐ 398 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-19 - Design engineering skill collection for AI coding agents with slash commands, review agents, and MCP quality gates.
* [Awesome QA Skills](https://github.com/naodeng/awesome-qa-skills) ⭐ 280 | 🐛 1 | 🌐 Python | 📅 2026-10-24 - Bilingual collection of 330 installable QA agent skills covering test workflows, test types, and skill engineering across the SDLC.
* [Pixi’VN](https://github.com/DRincs-Productions/pixi-vn) ⭐ 154 | 🐛 18 | 🌐 TypeScript | 📅 2026-10-22 - Agent skill collection teaching AI assistants to build story-driven games (visual novels, point-and-click, and interactive fiction) with the Pixi’VN engine.
* [vibes-plug](https://github.com/roedyrustam/vibes-plug) ⭐ 113 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-25 - Cross-IDE AI skill collection that orchestrates 147 specialized subagents for full-stack development workflows.
* [FMXER](https://github.com/andrea-magni/FMXER) ⭐ 101 | 🐛 0 | 🌐 Pascal | 📅 2026-10-22 - Agent skill teaching AI coding agents the FMXER declarative UI framework for Delphi FireMonkey: screens composed in code with named routes, a scaffold, layouts and Skia elements.
* [dex](https://github.com/exmergo/dex) ⭐ 97 | 🐛 110 | 🌐 Python | 📅 2026-10-25 - Agent skills for warehouse exploration, dbt transformation authoring, and schema-drift maintenance. Built by Exmergo.
* [vietnamese-language-skill](https://github.com/trussary/vietnamese-language-skill) ⭐ 89 | 🐛 1 | 🌐 Python | 📅 2026-09-03 - Collection of agent skills that fix Vietnamese register, terminology, and locale formatting across landing pages, docs, marketing, finance, and education, with a standalone validator.
* [research-agent-skills](https://github.com/KalarisLabs/research-agent-skills) ⭐ 61 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - 280+ Agent Skills that turn Claude Code, Codex, Cursor, Gemini CLI and other agents into a research co-scientist for literature reviews, hypotheses, experimental design, data analysis in biology, chemistry, medicine, physics and ML, paper writing, citation verification against Crossref, OpenAlex and arXiv, and peer review.
* [Krexa](https://github.com/Krexa-xyz/skills) ⭐ 53 | 🐛 0 | 📅 2026-10-21 - Agent skill and hosted MCP server that turn a trading idea, post or video into a backtested, paper-traded strategy (free) and, after the user approves and signs, a live trading agent on Binance, Coinbase, Kraken, OKX, Bybit, MEXC, Hyperliquid, Polymarket and Solana DEXs with order limits enforced server-side.
* [writing-with-agents](https://github.com/Jeffallan/writing-with-agents) ⭐ 35 | 🐛 3 | 🌐 Python | 📅 2026-10-22 - Ten Agent Skills that turn Betty Flowers' Madman, Architect, Carpenter, Judge writing method into a human-in-the-loop workflow, with SEO, a quality rubric, and content strategy.
* [PlayCanvas Skills](https://github.com/playcanvas/skills) ⭐ 31 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-21 - 16 portable Agent Skills that teach AI coding agents to build, inspect, and verify PlayCanvas Engine, React, and Web Components applications, also packaged as Claude Code, Codex, and Cursor plugins.
* [ego-decision-layer](https://github.com/jiangkoumo/ego-decision-layer) ⭐ 28 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-25 - Agent skill for ego lite browser automation with a swappable per-step decision model, guarded execution, and schema-validated extraction.
* [UI Verify](https://github.com/uiverify/uiverify) ⭐ 24 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-21 - Agent skills for visual testing: set up screenshot tests on your existing Storybook, Playwright or Vitest suite, check a UI change before pushing, and triage each build's diffs through the UI Verify MCP server.
* [antirea](https://github.com/MockirDev/antirea) ⭐ 21 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-21 - A Claude Code skill to protect projects and dev workspaces against AI reverse engineering and instruction leaks.
* [formosa-humanizer](https://github.com/nagameTW/formosa-humanizer) ⭐ 21 | 🐛 0 | 🌐 Markdown | 📅 2026-10-22 - Agent skill that rewrites AI-generated Traditional Chinese prose, removing AI phrasing and mainland China terms across 49 patterns.
* [Master Skills](https://github.com/sinhoneyy/master-skills) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - A unified collection of 2,660+ AI agent skills across 15 domains, with installation support for Claude Code, Codex, Cursor, Gemini CLI, Antigravity and other compatible assistants.
* [skills](https://github.com/mouadja02/skills) ⭐ 11 | 🐛 25 | 🌐 Python | 📅 2026-10-22 - A curated collection of 799 agent skills across 36 categories, installable into Claude Code, Cursor, and other SKILL.md-aware clients.
* [profile-use](https://github.com/leeguooooo/profile-use) ⭐ 5 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Agent skill that reuses one private personal profile across browser, iPhone and desktop forms, with masked reads, sensitive-field confirmation and approval before submission.
* [Kuudo Skills](https://github.com/KuudoAI/skills) ⭐ 3 | 🐛 6 | 🌐 Python | 📅 2026-10-24 - 22 Agent Skills for Amazon sellers and advertisers covering Sponsored Products and Brands audits, search-term mining, budget pacing, DSP and Amazon Marketing Cloud, listings, product images, repricing, FBA inbound, and profitability, built for Kuudo's hosted Amazon Ads and SP-API MCP servers, with price, budget, listing, and shipment writes previewed for explicit approval.
* [deed.page](https://github.com/f-o-x11/deed-page-skill) ⭐ 2 | 🐛 0 | 📅 2026-10-25 - Agent skill that publishes an HTML file or static folder to a permanent public deed.page URL with one curl request and no account.
* [Global Engineering Standards](https://github.com/Enki-DEV-expert/engineering-standards) ⭐ 2 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-20 - Twelve engineering standards and six Claude Code and Codex skills for security, privacy, cost and architecture, installable with `npm install -g @enki-dev-expert/global-engineering-standards`.
* [kstack](https://github.com/dwk601/kstack) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Eleven agent skills for Herdr that plan with two models checking each other, build with parallel reviewed workers, run a verification swarm, then push a PR and fix it until checks are green.
* [memory-use](https://github.com/leeguooooo/memory-use) ⭐ 2 | 🐛 3 | 🌐 Python | 📅 2026-10-24 - Portable agent memory in a private Markdown Git repository, with topic-focused recall, cross-session and cross-machine sync, and pre-commit secret checks.
* [max-skills](https://github.com/vasinl124/max-skills) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-25 - Agent skills for Claude Code and Codex that run your app locally to screenshot every screen a pull request changes as before/after pairs with the changes boxed, record a demo video of the PR's flow, and write a short Slack-ready summary, posting the media into the PR description with gh.
* [Nitrogen](https://github.com/mksd0398/nitrogen) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-23 - Agent skill and CLI that scaffold and deploy Shopify embedded apps on Firebase, with one Cloud Function per API resource, Firestore, and admin pages built from Polaris web components, also packaged as a Claude Code plugin marketplace.
* [ART Prompt Framework](https://github.com/YourAKShaw/art-prompt-framework) ⭐ 0 | 🐛 0 | 📅 2026-10-24 - Agent skill that turns rough requests into structured, context-rich prompts using the Act As, Request, and Terms framework.
* [CoMPaSS Prompt Framework](https://github.com/YourAKShaw/CoMPaSS-prompt-framework) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-20 - Agent skill for analysis-first prompting that clarifies intention, assembles consequential prompts from explicit components, and verifies their success criteria.
* [conventional-commits-framework](https://github.com/YourAKShaw/conventional-commits-framework) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-24 - Agent skill for complete, atomic Conventional Commits with every field filled, breaking changes declared explicitly, and one consistent AI co-author trailer, plus commitlint, git hook, and release tooling setup.
* [Cooper Email](https://github.com/cooper-email/cooper-email) ⭐ 0 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-24 - Agent Skills and a hosted MCP server that give an AI agent its own email inbox to send, receive, reply, and wait for replies or verification codes, with a Claude Code plugin and a Cursor plugin.
* [Deacon Skills](https://github.com/heydeacon/skills) ⭐ 0 | 🐛 0 | 📅 2026-10-22 - Two agent skills that install the Deacon AI support widget on a site or app, tell it who is signed in, and send it goals such as sign ups, also packaged as a Claude Code plugin marketplace.
* [nuthinking/skills](https://github.com/nuthinking/skills) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-14 - Agent skills for Claude Code, Codex and Cursor, including site-edit, where editors pin notes on a live site and Claude Code turns them into pull requests, and product-map, which keeps a feature map and product flows in the repo.
* [post](https://github.com/jack-reson8/post-skill) ⭐ 0 | 🐛 0 | 🌐 HTML | 📅 2026-10-25 - Agent skill that builds Xiaohongshu and X share-image sets with App Store poster layouts, real screenshots, and faithful app-UI mocks.
* [Principal Engineer OS](https://github.com/YourAKShaw/principal-engineer-os) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-24 - Agent skill that guides AI-assisted engineering with explicit trade-offs, boundary-focused correctness, security and privacy review, operational judgment, and evidence-based delivery.
* [pro-launch](https://github.com/jack-reson8/pro-launch) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Agent skill for building a product from zero to one with phase gates: references, naming and trademark checks, style frames, UI build loop, launch and shipping.
* [pro-motion](https://github.com/jack-reson8/pro-motion) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-25 - Agent skill that plans the music first, then renders motion-graphics launch and brand films in code (canvas to MP4) cut to the track.
* [renhua](https://github.com/jack-reson8/renhua) ⭐ 0 | 🐛 0 | 📅 2026-10-25 - Agent skill that writes Chinese social posts and product copy in a real person's voice and removes common AI phrasing.
* [ScoreStarling](https://github.com/HaiyiMei/scorestarling-plugins) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - Agent skills and hosted MCP server that transcribe, read, convert and edit sheet music, turning recordings, videos, sheet-music photos and PDFs, MIDI, MusicXML and ABC into one editable, playable score in a ScoreStarling account, with PDF, MusicXML, MIDI and audio exports.
* [skill-skill](https://github.com/jack-reson8/skill-skill) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Agent skill for writing and linting Claude skills, with a static audit script that reports a 0-100 health score.

### Development & Workflow

<!-- pinned -->

* [Ponytail](https://github.com/DietrichGebert/ponytail) ⭐ 175,955 | 🐛 134 | 🌐 JavaScript | 📅 2026-10-18 - Guides coding agents toward minimal working solutions through YAGNI, existing code, standard libraries, and native platform features.
* [Claude Code Skills](https://github.com/alirezarezvani/claude-skills) ⭐ 28,697 | 🐛 1 | 🌐 Python | 📅 2026-10-23 - 223 production-ready skills, 23 agents, and 298 Python tools across 9 domains — engineering, marketing, product, compliance, and more.
* [Planning with Files](https://github.com/OthmanAdi/planning-with-files) ⭐ 27,635 | 🐛 10 | 🌐 Python | 📅 2026-10-24 - Persistent file-based planning for Claude Code, Codex, and other AI coding agents, preserving task plans, findings, and progress across context loss, crashes, and compaction.
* [Screenpipe MCP](https://github.com/screenpipe/screenpipe) ⭐ 22,066 | 🐛 40 | 🌐 Rust | 📅 2026-10-24 - Gives agents searchable screen-text and audio history through MCP and a local API; source-available under the Screenpipe Commercial License, with configured cloud features able to send context off-device.
* [Browser Harness](https://github.com/browser-use/browser-harness) ⭐ 18,608 | 🐛 424 | 🌐 Python | 📅 2026-10-25 - MCP server and agent skill that connect an AI agent to a real browser through one editable CDP WebSocket.
* [universal-modder](https://github.com/rehan-remade/universal-modder) ⭐ 8,933 | 🐛 42 | 🌐 Python | 📅 2026-10-25 - Agent Skills, a CLI and a shared knowledge base that let Claude Code, Codex, Cursor, Gemini CLI, Copilot and OpenCode mod PC games you own: engine recon, reverse engineering, fal-generated art and sound, testing in the running game, and showcase videos.
* [avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) ⭐ 5,235 | 🐛 16 | 🌐 JavaScript | 📅 2026-10-20 - Portable agent skill for auditing and rewriting AI-patterned prose, with an optional local MCP detector that calls no model and sends no text to a network service.
* [Claude Octopus](https://github.com/nyldn/claude-octopus) ⭐ 4,302 | 🐛 13 | 🌐 Shell | 📅 2026-10-23 - Multi-LLM orchestration dispatching to 8 providers (Codex, Gemini, Copilot, Qwen, Perplexity, OpenRouter, Ollama, OpenCode) with Double Diamond workflows, adversarial review, and safety gates.
* [NotFair](https://github.com/nowork-studio/notfair-plugin) ⭐ 4,060 | 🐛 6 | 🌐 Python | 📅 2026-10-23 - Operate Google, Meta, X, LinkedIn, Reddit, and TikTok Ads plus GA4, Search Console, WordPress, and GoHighLevel through one OAuth MCP connection, with open-source SEO, GEO, and content skills for Claude Code, Codex, Cursor, and compatible agents.
* [obsidian-wiki](https://github.com/Ar9av/obsidian-wiki) ⭐ 3,618 | 🐛 5 | 🌐 Python | 📅 2026-10-21 - Builds an Obsidian knowledge vault from docs, URLs, and Claude Code, Codex, Copilot, Hermes, OpenClaw, and Pi session history, then cross-links it and answers questions with citations.
* [AI Video Transcriber](https://github.com/wendy7756/AI-Video-Transcriber) ⭐ 3,364 | 🐛 10 | 🌐 Python | 📅 2026-10-11 - Transcribe and summarize videos, podcasts, and local media via a Codex plugin, Claude Code skill, and MCP server.
* [zui](https://github.com/easysoft/zui) ⭐ 2,767 | 🐛 45 | 🌐 TypeScript | 📅 2026-10-23 - Codex skills that integrate the ZUI 3 web UI framework into existing projects and generate standalone ZUI-powered pages from plain briefs.
* [MegaLinter](https://github.com/oxsecurity/megalinter) ⭐ 2,623 | 🐛 63 | 🌐 Dockerfile | 📅 2026-10-25 - Set up, run and fix MegaLinter on any repository, covering 100+ linters and formatters for 69+ languages and 23+ formats, in CI or locally, with per-linter fix guides for the agent.
* [Better Harness](https://github.com/QoderAI/better-harness) ⭐ 2,410 | 🐛 12 | 🌐 JavaScript | 📅 2026-10-20 - Evidence-backed workflow analysis for coding agents that turns project and session signals into prioritized, verifiable improvements across supported hosts.
* [traceway](https://github.com/tracewayapp/traceway) ⭐ 1,745 | 🐛 26 | 🌐 Go | 📅 2026-10-24 - Agent skills that instrument repositories with Traceway OpenTelemetry monitoring and query production exceptions, logs, endpoints, and metrics.
* [mcp-server-kubernetes](https://github.com/Flux159/mcp-server-kubernetes) ⭐ 1,607 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-21 - MCP server for managing Kubernetes clusters via kubectl with tools for get, describe, apply, delete, logs, exec, port-forward, scaling, rollouts, Helm chart operations, and context switching.
* [agmsg](https://github.com/fujibee/agmsg) ⭐ 1,567 | 🐛 362 | 🌐 Shell | 📅 2026-10-25 - Cross-vendor messaging for CLI coding agents (Claude Code, Codex, Gemini CLI, Grok): sessions join a team by name and hand work to each other through a shared local SQLite file, with durable history and ext-tool members that let a program such as Slack or Jev join like any agent.
* [Brooks Lint](https://github.com/hyhmrright/brooks-lint) ⭐ 1,544 | 🐛 0 | 🌐 HTML | 📅 2026-10-24 - AI code reviews grounded in six classic engineering books — decay risk diagnostics with book citations, severity labels, and four analysis modes (PR review, architecture audit, tech debt, test quality).
* [Draw.io MCP Server (drawio-mcp-server)](https://github.com/lgazo/drawio-mcp-server) ⭐ 1,493 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-13 - MCP server exposing Draw\.io tools so AI agents can create, inspect, and modify diagrams, pages, and layers.
* [Aegis](https://github.com/GanyuanRan/Aegis) ⭐ 1,385 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - An agentic skills framework & software development methodology that works: planning, TDD, debugging, and collaboration workflows.
* [Antigravity Workspace Template](https://github.com/study8677/antigravity-workspace-template) ⭐ 1,355 | 🐛 4 | 🌐 Python | 📅 2026-10-23 - Multi-agent codebase knowledge graph generator with context-aware planning and automatic scope management — turns codebases into coherent agent workspaces.
* [Awesome-Journal-Skills](https://github.com/brycewang-stanford/Awesome-Journal-Skills) ⭐ 1,302 | 🐛 2 | 🌐 Stata | 📅 2026-09-27 - Claude Code plugin marketplace (also usable as Codex skills) of 300 journal- and conference-specific packs covering topic fit, house style, submission rules, and reviewer response for 744 venues across economics, social science, natural science, medicine, and computer science.
* [StyleSeed](https://github.com/bitjaru/styleseed) ⭐ 989 | 🐛 9 | 🌐 JavaScript | 📅 2026-10-23 - Compiles your project's design decisions into a lock file, then enforces them on Claude Code, Codex, and Cursor output with code and rendered-pixel gates so screens stay consistent across sessions.
* [claude-council](https://github.com/hex/claude-council) ⭐ 905 | 🐛 0 | 🌐 Shell | 📅 2026-10-25 - Claude Code plugin that asks Gemini, OpenAI, Grok, Perplexity, Kimi, OpenRouter models, the Codex, Cursor, Grok and Kimi CLIs and a local ollama model the same question in parallel and lines the answers up with a synthesis of where they agree and differ.
* [spec-superflow](https://github.com/MageByte-Zero/spec-superflow) ⭐ 871 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-23 - Spec-first workflow with nine skills, user-controlled Quick / Hotfix / Tweak / Full paths, auditable recovery commands, hardened delta-spec sync, and guarded review gates.
* [codex-autoresearch](https://github.com/TheGreenCedar/codex-autoresearch) ⭐ 834 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-11 - Codex plugin that runs measured optimization loops against a benchmark to improve local code.
* [Foreman](https://github.com/thruwire/foreman) ⭐ 785 | 🐛 10 | 🌐 Python | 📅 2026-10-15 - Jev-powered agent supervisor for Codex and OpenCode workers, with Pi and Pi Durable hooks for tool activity, project responsibilities, and completion checks.
* [token-optimizer](https://github.com/ooples/token-optimizer-mcp) ⭐ 560 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-25 - Spend less context and keep the conclusions across 16 coding clients including Claude Code, Codex, Gemini CLI, Cursor, and Copilot — diff-only re-reads, paths-only search, out-of-context stashing, and a local ledger that measures each tool's actual return.
* [Codex Multi Auth](https://github.com/ndycode/codex-multi-auth) ⭐ 555 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-20 - Multi-account OAuth manager for the official Codex CLI with switching, health checks, and recovery tools.
* [Jev MCP](https://github.com/jkudish/jev-mcp) ⭐ 548 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-25 - Fast, sub-cent typed judgments for agents, such as verifying claims against evidence, screening content for prompt injection before it enters context, and ranking candidates by meaning, each with probabilities and confidence in milliseconds.
* [Boss](https://github.com/echoVic/boss-skill) ⭐ 543 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-18 - BMAD pipeline plugin that orchestrates a full requirements-to-deploy workflow across nine specialist agents with an auditable runtime DAG and quality gates, for Claude Code, Codex, OpenClaw, and Antigravity.
* [MisakaNet](https://github.com/Ikalus1988/MisakaNet) ⭐ 543 | 🐛 375 | 🌐 Python | 📅 2026-10-25 - Git-backed failure-memory for AI coding agents with 290 indexed lessons, MCP server with 5 tools (search, get\_lesson, submit\_usage, submit\_intake, usage\_status), and DeepSeekHarness adapter.
* [OpenCode Power Pack](https://github.com/waybarrios/opencode-power-pack) ⭐ 542 | 🐛 5 | 🌐 Python | 📅 2026-10-19 - Fifty-four portable development and security workflows for Codex, Claude Code, OpenCode, and Pi, with opt-in native sandbox profiles for safer command execution.
* [Squadra](https://github.com/dagoSte/squadra) ⭐ 526 | 🐛 2 | 🌐 Python | 📅 2026-10-25 - Skill and CLI that coordinate Claude Code, Codex and Cursor windows as one team, with a shared task registry, proofs bound to the delivered code, review by a window that did not write it, and a live dashboard.
* [Context Attachment Manager](https://github.com/chipfighter/context-attachment-manager) ⭐ 517 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-24 - Manage image history in Codex desktop and Claude Desktop Code with on-demand image retrieval, pinned references, and search by description or feedback.
* [de-anthropocentric-research-engine](https://github.com/yogsoth-ai/de-anthropocentric-research-engine) ⭐ 505 | 🐛 1 | 📅 2026-10-23 - Collection of 900+ markdown research skills that let Claude Code autonomously survey literature, find gaps, form hypotheses, and design experiments.
* [AgentOps](https://github.com/boshu2/agentops) ⭐ 450 | 🐛 3 | 🌐 Go | 📅 2026-10-25 - DevOps layer for coding agents with flow, feedback, and memory that compounds between sessions.
* [Skillstore](https://github.com/aiskillstore/marketplace) ⭐ 444 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - Security-audited Agent Skills marketplace with one-command installation for Claude Code and Codex via the skillstore CLI.
* [dryforge](https://github.com/prekuter/dryforge) ⭐ 427 | 🐛 1 | 🌐 Python | 📅 2026-10-16 - Intent to implementation: ready, then go.
* [AgentBridge](https://github.com/raysonmeng/agent-bridge) ⭐ 408 | 🐛 50 | 🌐 TypeScript | 📅 2026-10-24 - Local bidirectional bridge that keeps Claude Code and Codex live as peers in one session, with mid-turn injection and quota-window handoff.
* [MartinLoop](https://github.com/Keesan12/martin-loop) ⭐ 394 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-24 - Open-source runtime for governed coding-agent runs with scope limits, budget caps, verifier gates, retries, stop conditions, and evidence records across Codex, Claude Code, Gemini CLI, and supported model runtimes.
* [genie](https://github.com/automagik-dev/genie) ⭐ 345 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-25 - Agent skills and CLI that interview a wish into a plan, dispatch parallel subagents, and review results against acceptance criteria.
* [Audio Plugin Coder](https://github.com/Noizefield/audio-plugin-coder) ⭐ 343 | 🐛 2 | 🌐 HTML | 📅 2026-10-19 - Agent-agnostic JUCE workflow for building VST3/AU plugins from idea through design, implementation, test, and installer packaging.
* [Jev Browser](https://github.com/jkudish/jev-browser) ⭐ 342 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-25 - Fast, very cheap browser use for agents: Jev picks every action, code owns the loop, and you get the final page, an auditable step trace, console errors, and a screenshot; MCP server, CLI, or library.
* [AREX-Skill](https://github.com/VectorSpaceLab/AREX-Skill) ⭐ 341 | 🐛 1 | 🌐 Python | 📅 2026-09-03 - A library of 5,000+ verified, executable skills distilled from ML repositories for coding and research agents.
* [DataMagic](https://github.com/HKUSTDial/DataMagic) ⭐ 339 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-23 - A skill that teaches coding agents to plan and render narrated animated data videos from tabular data using DVSpec.
* [Reviewable HTML Workbench](https://github.com/u-ichi/reviewable-html-workbench) ⭐ 300 | 🐛 4 | 🌐 Python | 📅 2026-09-10 - Generate reviewable HTML documents, serve previews, collect inline review comments, and feed review outcomes back into agent workflows.
* [Emulo](https://github.com/ohad6k/emulo) ⭐ 299 | 🐛 16 | 🌐 HTML | 📅 2026-10-12 - Mines selected evidence from local coding-agent sessions into private work, design, and writing profiles for Codex, Claude Code, and GitHub Copilot.
* [Spellbook](https://github.com/majiayu000/spellbook) ⭐ 288 | 🐛 2 | 🌐 Python | 📅 2026-10-23 - Cross-runtime library of 108 agent skills installable into Claude Code and Codex via one command.
* [OpenCode Orchestrator](https://github.com/agnusdei1207/opencode-orchestrator) ⭐ 274 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-24 - Multi-agent mission control for OpenCode with Commander, Planner, Worker, and Reviewer workflows.
* [Vibe Prospecting](https://github.com/explorium-ai/vibeprospecting-plugin) ⭐ 256 | 🐛 4 | 🌐 Shell | 📅 2026-10-11 - Live B2B company and contact intelligence for building lead lists, researching prospects, enriching contacts, and personalizing outreach.
* [Knowledge Manager](https://github.com/treylom/knowledge-manager) ⭐ 250 | 🐛 0 | 🌐 Python | 📅 2026-10-14 - Extracts and organizes content from web pages, files, Notion, and images into an Obsidian knowledge vault with GraphRAG-backed search, exporting to Notion, Markdown, and PDF.
* [keep-the-why](https://github.com/oliver-zehentleitner/keep-the-why) ⭐ 231 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Preserves the reasoning behind a codebase as project memory — decisions, rejected alternatives, workarounds, incident learnings, constraints.
* [Orbi](https://github.com/orbi-build/orbi) ⭐ 231 | 🐛 38 | 🌐 Python | 📅 2026-10-25 - Plugin and agent skills for Claude Code, Codex, Cursor, GitHub Copilot and Pi that draft GitHub Issues with testable acceptance criteria and, in repositories that run the open-source Orbi agent, hand them off to be implemented, tested, reviewed by a separate AI session and merged.
* [Claude Code for Codex](https://github.com/sendbird/cc-plugin-codex) ⭐ 226 | 🐛 16 | 🌐 JavaScript | 📅 2026-10-19 - Reverse of OpenAI's official Claude-hosted plugin: use Claude Code from Codex for reviews, rescue tasks, tracked background jobs, and hook-powered review gates.
* [grip](https://github.com/guilyx/grip) ⭐ 216 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Git hook that quizzes you on your own diff before commit or push, with a Claude Code plugin plus Codex and Gemini CLI support.
* [lattice](https://github.com/techygarg/lattice) ⭐ 209 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-24 - Composable AI skills framework that infuses clean code, clean architecture, domain-driven design, secure coding, and proper testing into the workflow by default, with scenario-driven guides for getting started, customization, and team use.
* [Oh My Design](https://github.com/3x-haust/oh-my-design) ⭐ 203 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-22 - Evidence-backed design workflow for Claude Code and Codex with reference research, multi-agent reviews, visual QA, and anti-slop guardrails.
* [claude-remember](https://github.com/Digital-Process-Tools/claude-remember) ⭐ 202 | 🐛 26 | 🌐 Python | 📅 2026-10-25 - Persistent memory for Claude Code with identity, context, and continuity carried across sessions.
* [agent-talk](https://github.com/xhluca/agent-talk) ⭐ 200 | 🐛 1 | 🌐 Python | 📅 2026-10-21 - Skills-based plugin built on the retalk CLI that gives coding agents end-to-end encrypted messaging with other agents, including agents run by other people, across Claude Code, Codex, Antigravity, pi, opencode, and GitHub Copilot CLI.
* [trace-mcp](https://github.com/nikolai-vysotskyi/trace-mcp) ⭐ 195 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-25 - Precomputed code-intelligence graph served over MCP — symbol search, call graphs, change impact, and test mapping as structured answers instead of whole-file reads.
* [ab-method](https://github.com/ayoubben18/ab-method) ⭐ 192 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-22 - A skill and workflow plugin for Claude Code and Codex that grills problems into plans and drives test-driven missions with critic reviews.
* [opencode-models-discovery](https://github.com/yuhp/opencode-models-discovery) ⭐ 192 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-21 - OpenCode plugin that dynamically discovers models from OpenAI-compatible providers and injects them into provider config with filtering and metadata enrichment.
* [codex-profiles](https://github.com/Ducksss/codex-profiles) ⭐ 189 | 🐛 1 | 🌐 Shell | 📅 2026-10-24 - Switch Codex CLI and Desktop accounts with isolated `CODEX_HOME` profile directories instead of copying token files.
* [claude-dnd-skill](https://github.com/neuralinitiative/claude-dnd-skill) ⭐ 169 | 🐛 4 | 🌐 Python | 📅 2026-10-09 - Unofficial D\&D 5e Dungeon Master for Claude Code with persistent campaigns, full 5e rules mechanics, and an optional cinematic display companion for a TV.
* [dsh-whale-musume](https://github.com/Sutera-Diffusus/dsh-whale-musume) ⭐ 168 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-25 - Whale-girl desktop pet for the DSH Web UI with pat-to-raise growth, work-state poses, 494 dialogue lines, 30 achievements and a built-in settings panel; local-first, zero telemetry.
* [opencode-synced](https://github.com/iHildy/opencode-synced) ⭐ 168 | 🐛 7 | 🌐 TypeScript | 📅 2026-09-23 - OpenCode plugin that syncs global configuration and skills across machines via Git, with optional sessions and secrets for private repositories.
* [piia-engram](https://github.com/Patdolitse/piia-engram) ⭐ 163 | 🐛 1 | 🌐 Python | 📅 2026-10-23 - Local-first personal AI identity and memory layer that shares user-owned preferences, lessons, decisions, playbooks, and project context across MCP-compatible coding tools.
* [ContextPilot](https://github.com/EfficientContext/ContextPilot) ⭐ 145 | 🐛 14 | 🌐 Python | 📅 2026-10-22 - Context optimization engine that reorders and deduplicates context blocks to raise cache hits, shipping as plugins for OpenClaw and Hermes.
* [jevmem](https://github.com/Avinash-jetwani/jevmem) ⭐ 133 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-23 - Plugin and MCP server that automatically saves project decisions, rules and dead ends to a JEVMEM.md file and recalls them in later sessions.
* [Krypton](https://github.com/jturntdev/krypton) ⭐ 132 | 🐛 2 | 🌐 Shell | 📅 2026-07-24 - Goal-based planning and proof gate for Codex and Claude Code that turns requests into ownership, cutover, review-gate, and acceptance-evidence plans.
* [humanizer-ru](https://github.com/Vladimir-Human/humanizer-ru) ⭐ 131 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Deterministic offline diagnostics and safe cleanup of chat-interface copy-paste artifacts in Russian text and Markdown, shipped as an Agent Skill, MCP server, CLI, GitHub Action, and browser demo, with no authorship verdicts.
* [Suede Creator Skills](https://github.com/JasonColapietro/suede-creator-skills) ⭐ 125 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-25 - An open-source Agent Skills pack for Claude Code and Codex covering multi-agent workflows, code review, design, copy, SEO, app shipping, creator-rights workflows, and local read-only MCP discovery.
* [orchflows](https://github.com/DanMcInerney/orchflows) ⭐ 124 | 🐛 1 | 🌐 Python | 📅 2026-10-04 - Use 2 simple skills to build complex, composable workflows for task-specific jobs.
* [Janus](https://github.com/RamitVishwakarma/Janus) ⭐ 123 | 🐛 0 | 🌐 Swift | 📅 2026-10-05 - macOS menu bar app that saves each Claude Code account's session so switching between accounts is one click, and reclaims disk space by measuring developer caches and moving them to the Trash.
* [Superloopy](https://github.com/beefiker/superloopy) ⭐ 112 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-15 - Evidence-gated Codex loop harness with specialist skills, including near-pixel authorized website cloning backed by screenshots, assets, build output, and visual QA.
* [assay](https://github.com/awss1i/assay) ⭐ 108 | 🐛 0 | 🌐 Python | 📅 2026-10-19 - Deterministic QA skill and plugin that drives a generated web page in a real browser and reports what broke, across fifteen coding harnesses.
* [Coordinate Agents](https://github.com/hogancv/coordinate-agents) ⭐ 107 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-24 - Plugin-first multi-agent coordination tool with a local-first, recoverable Agent Bus and human-gated planning, implementation, review, and release workflows.
* [sci-brain](https://github.com/QuantumBFS/sci-brain) ⭐ 104 | 🐛 6 | 🌐 Python | 📅 2026-09-25 - Research skills plugin for Claude Code, Codex, OpenCode, and pi that surveys literature into a citable knowledge base, brainstorms research ideas, and drafts papers and slides.
* [MCP Video Analyzer](https://github.com/guimatheus92/mcp-video-analyzer) ⭐ 102 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-25 - Gives agents video input: transcript, key frames, OCR text, metadata, and an annotated timeline from Loom, YouTube, Instagram, TikTok, direct URLs, or a local file, over MCP, a one-shot CLI, or the /video skill.
* [Solana Finance](https://github.com/quicknode/solana-finance-claude-plugin) ⭐ 101 | 🐛 2 | 📅 2026-10-23 - build financial software - order book exchanges, betting markets, AMMs, fundraising projects, betting markets, options trading, etc - on Solana using Anchor, Rust, and Quasar.
* [Knowl](https://github.com/dat999zx/knowl) ⭐ 100 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-21 - Local-first project memory over MCP for Claude Code, Codex, Cursor and eight other hosts: a SQLite store that retires facts when they change, shares knowledge across linked repos, and retrieves it by hybrid search.
* [2718lab DevKit](https://github.com/2718labs/2718lab-devkit) ⭐ 98 | 🐛 4 | 🌐 Python | 📅 2026-10-19 - Codex-first local MCP server and skill bundle for deterministic project intelligence, durable workflow orchestration, and reusable engineering tools.
* [opencode-litellm](https://github.com/yuseferi/opencode-litellm) ⭐ 97 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-20 - OpenCode plugin that auto-detects a LiteLLM proxy and dynamically registers its models in the OpenCode picker.
* [otelyssey](https://github.com/using-system/otelyssey) ⭐ 97 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - Marketplace of OpenTelemetry agent plugins (instrumentation, Collector, backends, observability) for Claude Code, Copilot CLI, Codex, Grok Build and more, run by the repository itself: submit a plugin.json URL, it validates, reviews, lists and follows releases.
* [FlowBoard](https://github.com/rasimme/FlowBoard) ⭐ 96 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-13 - Local-first project workspace and task-coordination plugin for OpenClaw and external coding agents, with lazy-loaded context and a shared Kanban board.
* [pstack for Codex](https://github.com/Aqua-123/pstack-for-codex) ⭐ 96 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-23 - Codex-native engineering workflows derived from pstack, with 45 explicit skills and 23 Poteto Mode playbooks.
* [Blender Agent Studio](https://github.com/ifBars/blender-agent-studio) ⭐ 94 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-25 - Codex plugin with specialist skills and a local MCP server for building, inspecting, validating, and rendering Blender scenes, plus browser handoffs for Mixamo motion and Pixabay sound effects.
* [cc-tree](https://github.com/skymanbp/cc-tree) ⭐ 94 | 🐛 6 | 🌐 Python | 📅 2026-10-17 - Claude Code plugin that runs brainstorming, adversarial critique, design-space comparison and code audit as an auditable radial tree with file:line or URL evidence on every node.
* [local-shell-mcp](https://github.com/fwerkor/local-shell-mcp) ⭐ 94 | 🐛 9 | 🌐 Python | 📅 2026-10-25 - MCP server: gives AI agents controlled shell execution, filesystem operations, browser automation, persistent sessions, and remote machine management.
* [forgecat-agent-profiles](https://github.com/nota-america/forgecat-agent-profiles) ⭐ 93 | 🐛 3 | 🌐 TypeScript | 📅 2026-09-23 - Catalog of 191 cross-platform agent profiles installable via the ForgeCat CLI into Claude Code, Cursor, Codex, OpenClaw, and Hermes Agent.
* [opencode-see-image](https://github.com/alfaoz/opencode-see-image) ⭐ 92 | 🐛 1 | 🌐 TypeScript | 📅 2026-09-27 - OpenCode plugin that gives non-vision models image and screenshot understanding by routing attachments to a vision-capable model.
* [AI-Native SDLC](https://github.com/bashebr/ai-native-sdlc) ⭐ 88 | 🐛 0 | 🌐 Python | 📅 2026-10-10 - Reusable skill and plugin bundle implementing the AI-native SDLC workflow: plan, design, build, test, deploy, and maintain with human approval gates.
* [Dely](https://github.com/hieuphung97/dely) ⭐ 88 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-12 - Multi-harness control protocol that turns requests into approved design contracts, orchestrating isolated worker sessions for sequential implementation and independent code reviews under Orca supervision for Claude Code, Codex, Cursor, Antigravity, and other AI coding agents.
* [Festival](https://github.com/Obedience-Corp/festival) ⭐ 88 | 🐛 5 | 🌐 Shell | 📅 2026-10-25 - Planning and persistent context tools that let coding agents execute multi-phase goals across sessions using files and Git.
* [Gangsta Agents](https://github.com/kucherenko/gangsta) ⭐ 86 | 🐛 2 | 🌐 Shell | 📅 2026-08-14 - Agent skills providing a spec-driven development pipeline with reconnaissance, adversarial debate, TDD execution, and verification phases for Claude Code, Codex, Cursor, OpenCode, and Gemini CLI.
* [opencode-skills-collection](https://github.com/FrancoStino/opencode-skills-collection) ⭐ 86 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - OpenCode plugin that bundles 1595+ skills and auto-syncs them locally, loading each on demand via pointer files.
* [LittleJS AI](https://github.com/KilledByAPixel/LittleJS-AI) ⭐ 84 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-14 - Claude Code plugin for making HTML5 games with the LittleJS engine, with skills for engine conventions, API lookup, scaffolding new playable games, and atlas-based shape art.
* [BanyanCode](https://github.com/EkagraAgarwal/BanyanCode) ⭐ 83 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-24 - Terminal coding agent with parallel subagents, cross-session memory, Tree-sitter code graph, and free web research.
* [Sealos](https://github.com/labring/sealos-skills) ⭐ 83 | 🐛 8 | 🌐 Python | 📅 2026-09-28 - Deploy apps to Sealos Cloud from Codex with readiness checks, Dockerfile generation, Compose conversion, image builds, and rollout updates.
* [super-pm](https://github.com/konglong87/superPM) ⭐ 83 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-24 - Product management skill pack with 50 core skills and 6 workflows covering demand research, PRD writing, growth analysis, product strategy, and launch planning.
* [i-hate-editing](https://github.com/ranahaani/i-hate-editing) ⭐ 80 | 🐛 0 | 🌐 Python | 📅 2026-10-06 - Claude Code skill that turns raw talking-head footage into a finished cut with local whisper.cpp + ffmpeg (model never watches the pixels).
* [claude-image-gen](https://github.com/guinacio/claude-image-gen) ⭐ 79 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-10 - AI-powered image generation using Google Gemini or OpenAI (gpt-image-2), integrated with Claude Code via Skills or Claude.ai via MCP.
* [taskflow](https://github.com/heggria/taskflow) ⭐ 79 | 🐛 10 | 🌐 TypeScript | 📅 2026-10-21 - Declarative, verifiable DAG orchestration for Grok Build subagents — fan-out, gates, loops, tournaments, approvals, and resumable runs via MCP tools, with intermediate transcripts kept out of context.
* [ChatVault](https://github.com/ssanaullahrais/Chat-Vault) ⭐ 77 | 🐛 11 | 🌐 TypeScript | 📅 2026-10-25 - Windows app that reads, searches, backs up and continues your Claude Code, Codex, Cursor, Gemini CLI, OpenCode and Cline chats across accounts. <!-- platform: standalone -->
* [FlexViz](https://github.com/flex-analytics/flexviz) ⭐ 76 | 🐛 44 | 🌐 Python | 📅 2026-10-19 - Interactive cross-filter dashboards for large datasets with a Claude Code skill for agent-driven data exploration.
* [Archcore](https://github.com/archcore-ai/archcore) ⭐ 72 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-22 - Spec-driven development and context engineering for Claude Code, Cursor, Codex, and GitHub Copilot — backed by project context in Git.
* [grounded-ai](https://github.com/grounded-ai/grounded_ai) ⭐ 71 | 🐛 7 | 🌐 Python | 📅 2026-10-22 - Stop hook for Claude Code and Codex that checks the agent's final answer against that turn's tool output with TypeSafe's Jev, plus CascadeEvaluator, which lets Jev settle the eval decisions it is confident about and sends only the rest to an LLM judge.
* [Mycelium](https://github.com/arjunrajlaboratory/mycelium) ⭐ 71 | 🐛 2 | 🌐 Python | 📅 2026-10-17 - Gives Claude Code and Codex analytical repositories durable memory for decisions, findings, provenance, reusable conventions, and analysis workflows.
* [silica](https://github.com/kiycoh/silica-harness) ⭐ 70 | 🐛 0 | 🌐 Python | 📅 2026-10-14 - Serves an Obsidian vault as the agent's memory over MCP: semantic and literal recall, gated note writing, and hooks that open each session already knowing its vault.
* [Craft](https://github.com/drobins25/craft) ⭐ 69 | 🐛 1 | 🌐 Shell | 📅 2026-10-24 - Craft is a Claude Code plugin that asks you the product questions and works out the technical ones. Features get planned, built, and tested, with your codebase read-only until you approve the work. Point at a live page to change it. The calls you make - decisions, design tokens, the tweaks you loved - carry into every build after.
* [skillsaw](https://github.com/stbenjam/skillsaw) ⭐ 68 | 🐛 9 | 🌐 Python | 📅 2026-10-16 - A configurable linter for agent skills, plugins, and AI coding assistant context.
* [UIZZE](https://github.com/uizze/uizze) ⭐ 68 | 🐛 7 | 🌐 JavaScript | 📅 2026-10-24 - Free MIT anti-ui-slop Skill with a product-specific design contract, required UI states, and a hard finish gate; full UIZZE adds live reference search, validation, and audits across 800,000+ real web and iOS screens through its authenticated MCP server at <https://uizze.com/mcp>.
* [session-handoff](https://github.com/yuzushi-dev/session-handoff) ⭐ 67 | 🐛 3 | 🌐 Python | 📅 2026-10-25 - Create handoffs and migrate sessions between Claude Code and Codex.
* [YYLO](https://github.com/yylo-dev/yylo) ⭐ 66 | 🐛 15 | 🌐 Python | 📅 2026-10-23 - Command-line orchestrator for coding agents that creates a dedicated branch/worktree per task, delegates to Pi and Codex subagents, and enforces typed task, validation, merge, and release-readiness boundaries with receipt-backed repository changes.
* [jev-use](https://github.com/shitianfang/jev-use) ⭐ 65 | 🐛 7 | 🌐 JavaScript | 📅 2026-09-22 - Hands the agent steps that need no text output to Jev's judgment model across Claude Code, Codex, and Pi, returning everything it should not decide to the LLM under a typed escalation contract.
* [Globalping](https://github.com/jsdelivr/globalping-mcp-server) ⭐ 64 | 🐛 10 | 🌐 TypeScript | 📅 2026-10-19 - Access thousands of probes around the world to run network tests such as ping, traceroute, http, dns and mtr.
* [mstar-harness](https://github.com/btspoony/mstar-harness) ⭐ 64 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-25 - Multi-agent code harness plugin that routes work through PM, dev, QC, and QA roles with deterministic workflow gates enforced by a TypeScript engine, installable across dsh, omp, OpenCode, Cursor, Kimi Code, ZCode, and Codex.
* [VibeRaven](https://github.com/ohad6k/VibeRaven) ⭐ 61 | 🐛 18 | 🌐 JavaScript | 📅 2026-10-22 - Skill pack and plugin that give coding agents architecture, provider and release context, with repository check-and-fix workflows for Vercel and Supabase apps.
* [mcp-local-memory](https://github.com/Beledarian/mcp-local-memory) ⭐ 60 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-14 - A lightweight, powerful local memory server for AI agents supporting text, entities, relations, and time-based recall.
* [PAI](https://github.com/mnott/PAI) ⭐ 60 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-25 - Personal AI infrastructure for Claude Code: persistent memory with hybrid search, session continuity, a knowledge graph, and headless workers on other model providers, delivered as hooks, skills, and an MCP server.
* [clausona](https://github.com/larcane97/clausona) ⭐ 57 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-20 - CLI and TUI for switching Claude Code and Codex accounts that keeps conversation history across them so `claude --continue` picks up another account's session, routes each run by plan usage, manages every account's skills, MCP servers and hooks, and runs as a shell hook with no daemon; its Claude Code plugins run parallel workers in herdr, Orca or Superset.
* [Honcho](https://github.com/plastic-labs/codex-honcho) ⭐ 55 | 🐛 16 | 🌐 TypeScript | 📅 2026-09-01 - Persistent cross-session memory for Codex powered by Honcho — lifecycle hooks capture each session and inject relevant context back at session start, so Codex remembers your preferences, projects, and decisions across restarts.
* [OpenSea Skills](https://github.com/ProjectOpenSea/opensea-skill) ⭐ 53 | 🐛 0 | 🌐 Shell | 📅 2026-10-06 - Five Agent Skills for OpenSea data, Seaport trading, ERC20 swaps, wallet signing, and ERC-8257 tool development.
* [WorkFlowX](https://github.com/TreeX-X/WorkFlowX) ⭐ 53 | 🐛 3 | 🌐 HTML | 📅 2026-10-17 - Multi-agent orchestration plugin for Claude Code and Codex that structures planning, coding, and independent evaluation of development tasks.
* [Session Orchestrator](https://github.com/Kanevry/session-orchestrator) ⭐ 52 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-24 - Session orchestration for Claude Code, Codex, and Cursor IDE — structured planning, wave-based execution, VCS integration (GitLab + GitHub), quality gates, and clean session close-out with issue tracking.
* [web-ai-agent-skills](https://github.com/webmaxru/web-ai-agent-skills) ⭐ 52 | 🐛 2 | 🌐 TypeScript | 📅 2026-09-29 - Agent skills that guide coding agents through integrating browser Web AI APIs: Prompt API, Translator, Language Detector, Proofreader, WebMCP, and WebNN.
* [kitbash](https://github.com/Open-Dev-Society/kitbash) ⭐ 51 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-23 - Breaks an idea into components and classifies each one as BORROW, KITBASH, or WRITE, checking every repo it names against the live GitHub API so invented ones never reach you; ships as a skill, plugin, and MCP server.
* [opencode-failover](https://github.com/bulutmuf/opencode-failover) ⭐ 51 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-10 - OpenCode plugin for automatic API-key failover and rotation across multiple provider keys.
* [Knowledge Loom](https://github.com/magickaichen/knowledge-loom) ⭐ 50 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-14 - Agent-neutral skills for initializing, auditing, using, and maintaining governed local Markdown knowledge vaults across Agent Skills-compatible runtimes.
* [Open Dynamic Workflows](https://github.com/Suraj1235/open-dynamic-workflows) ⭐ 50 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-09 - Local-first MIT dynamic multi-agent workflows for Codex, OpenCode, Antigravity, Cursor, and VS Code with a daemon, MCP bridge, Codex skills, OpenCode plugin, and bring-your-own-model support.
* [ai-agents](https://github.com/rjmurillo/ai-agents) ⭐ 49 | 🐛 21 | 🌐 Python | 📅 2026-10-24 - Plugin marketplace for Claude Code and Copilot CLI that installs 30 specialist agents and 104 skills covering the spec-to-ship lifecycle and code review.
* [Designer Skill](https://github.com/PyModel/designer-skill) ⭐ 49 | 🐛 12 | 🌐 JavaScript | 📅 2026-10-23 - Plug-and-play MCP that gives your coding agent UI superpowers: design references, intent routing and a static anti-slop gate, no API key.
* [genesis-architect](https://github.com/maioio/genesis-architect) ⭐ 48 | 🐛 19 | 🌐 Python | 📅 2026-10-12 - Agent skill that researches real GitHub repositories and issues before scaffolding projects, then audits drift, cycles and fragility in existing code.
* [Jevbridge](https://github.com/tacticocc/Jevbridge) ⭐ 48 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-21 - OSS ACP/MCP adapter that bridges TypeSafe Jev with any LLM, putting computer use and typed decisions alongside Codex, Claude, Grok, and OpenCode without replacing those hosts.
* [memi](https://github.com/sarveshsea/memi) ⭐ 48 | 🐛 10 | 🌐 TypeScript | 📅 2026-10-25 - Interface understanding and design-system memory for Codex, Claude Code, Cursor, and MCP agents with UI audits, Tailwind token extraction, shadcn registry workflows, and a bundled Codex plugin.
* [IdeaScientist](https://github.com/junjiezhou1122/ideascientist-claude-code) ⭐ 47 | 🐛 0 | 🌐 Python | 📅 2026-10-10 - Evidence-grounded scientific ideation with literature discovery, isolated readers, and independent review in native Claude Code, Codex, and Pi agents.
* [Codex Auto Resume](https://github.com/songyb111-gachon/codex-auto-resume-windows) ⭐ 46 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - Unofficial Windows app and Codex plugin that waits out Codex usage limits, rate limits and temporary failures, then continues the exact interrupted conversation by itself, with a Dashboard, a tray icon and an optional advanced edition.
* [Rootly MCP Server](https://github.com/rootlyhq/rootly-mcp-server) ⭐ 45 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Manage and resolve production incidents from MCP-compatible AI assistants through dynamically generated, access-controlled Rootly API tools.
* [ContextStream](https://github.com/contextstream/mcp-server) ⭐ 44 | 🐛 5 | 🌐 Rust | 📅 2026-10-25 - Persistent memory, semantic search, and shared project context for AI agents with traceable sources and scoped access.
* [Docflow](https://github.com/MedAdemBHA/docflow) ⭐ 44 | 🐛 0 | 🌐 Shell | 📅 2026-08-15 - Lightweight documentation memory for AI coding agents that scaffolds a 7-category docs tree, runs readiness checks, validates docs before finishing, and keeps a monthly changelog across Claude Code and Codex.
* [Groundwork](https://github.com/etr/groundwork) ⭐ 44 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-23 - Comprehensive skills library for Claude Code and Codex that structures discovery, planning, design, TDD, debugging, validation, collaboration, and shipping.
* [iris-agentic-dev](https://github.com/intersystems-community/iris-agentic-dev) ⭐ 44 | 🐛 16 | 🌐 Rust | 📅 2026-10-25 - MCP server giving AI assistants live access to InterSystems IRIS — execute ObjectScript, query globals, inspect productions, run tests, search code, and manage skills.
* [Open PR](https://github.com/TOMOSIA-VIETNAM/open-pr) ⭐ 44 | 🐛 4 | 🌐 Python | 📅 2026-10-24 - AI code review that lands on the pull request itself across GitHub, GitLab, and Bitbucket, learning each repo's conventions to post one review, one fix commit, and in-thread replies from Claude Code, Cursor, Codex, Gemini CLI, or Antigravity.
* [Waggle](https://github.com/Abhigyan-Shekhar/Waggle-mcp) ⭐ 44 | 🐛 207 | 🌐 Python | 📅 2026-10-23 - Persistent graph-backed conversational memory for Codex that recalls project decisions, constraints, preferences, and outcomes across sessions.
* [openclaw-otel-observability](https://github.com/henrikrexed/openclaw-observability-plugin) ⭐ 42 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-21 - OpenTelemetry observability plugin for OpenClaw AI agents that emits traces, metrics, and logs via OpenLLMetry.
* [Codebase Recon](https://github.com/yujiachen-y/codebase-recon-skill) ⭐ 41 | 🐛 0 | 📅 2026-04-26 - Analyze git history to understand a codebase before reading any code — auto-scales by repo size and cross-references hotspots with bug magnets to surface high-risk files, bus factor, and team momentum.
* [Second Claude Code](https://github.com/unclejobs-ai/second-claude-code) ⭐ 41 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-21 - Knowledge-work plugin for Claude Code, Codex, and Grok with research, writing, review, and refinement skills and a gated gather, draft, check, and cut workflow.
* [Click](https://github.com/grapefruit0205/click) ⭐ 40 | 🐛 7 | 🌐 Python | 📅 2026-10-23 - Record revision-aware evidence for normal Codex work and optionally bind higher-risk execution to one human-readable approval contract.
* [opencode-openai-compact](https://github.com/partment/opencode-openai-compact) ⭐ 40 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-25 - OpenCode plugin that uses OpenAI Responses API native compaction v2 and stores checkpoints in SQLite.
* [Quality Engineering Skills](https://github.com/RBraga01/Quality-Engineering-Skills) ⭐ 40 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - 22 structured quality engineering skills for automotive and manufacturing: ISO 9001, IATF 16949, AIAG-VDA FMEA, VDA 6.3, PPAP, APQP, SPC, MSA.
* [Labtasker](https://github.com/luocfprime/labtasker) ⭐ 39 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Queue and run independent ML inference, evaluation, and experiment tasks across long-lived Python or command workers with a Claude Code plugin and cross-agent skill.
* [Velith](https://github.com/epicsagas/Velith) ⭐ 39 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-30 - AI-native publishing system with a 6-phase pipeline from ideation to EPUB/PDF across 8 genres.
* [Android Engineering Skills](https://github.com/lennonpetrick/android-engineering-skills) ⭐ 38 | 🐛 1 | 📅 2026-10-22 - Agent Skills for any skills-compatible coding agent (Claude Code, Codex, Gemini in Android Studio, and more) that teach how to structure, write, and test Android apps with Kotlin and Jetpack Compose.
* [JevScout](https://github.com/hqman/JevScout) ⭐ 38 | 🐛 1 | 🌐 Python | 📅 2026-09-18 - Autonomous job hunt orchestrator powered by TypeSafe Jev and Chrome DevTools Protocol to discover and evaluate AI engineering roles.
* [ai-companion-time-anchor](https://github.com/See-Sol-Lab/ai-companion-time-anchor) ⭐ 37 | 🐛 0 | 🌐 Python | 📅 2026-10-13 - Cross-client skill and hook collection for per-conversation elapsed-time awareness, ambient time cues, active clock checks, and temporal-context updates across Codex, Claude Code, and web/chat environments.
* [Shrike](https://github.com/SumantxD/shrike) ⭐ 37 | 🐛 44 | 🌐 TypeScript | 📅 2026-10-25 - Claude Code plugin for the Shrike desktop app that shows your agent what your web app actually did on each click (the code path, real values, queries and errors), so it fixes from what ran instead of guessing; every code change waits for your approval in Shrike.
* [ai-craftsman-superpowers](https://github.com/BULDEE/ai-craftsman-superpowers) ⭐ 35 | 🐛 8 | 🌐 Shell | 📅 2026-10-24 - Quality gate for AI coding agents (Claude Code, Codex, Grok, Hermes) that refuses file writes breaking your project's rules before they reach disk, tells the agent how to fix them, and learns from your corrections.
* [super-token-saver](https://github.com/ww-w-ai/super-token-saver) ⭐ 35 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-30 - Cuts Claude Code and Codex token spend with prompt-cache expiry warnings, zero-cost session restore after compaction, and per-model usage and cost reports.
* [Agent Guard](https://github.com/JeongJaeSoon/agent-guard) ⭐ 34 | 🐛 1 | 🌐 Shell | 📅 2026-10-25 - Real-time secret-leak guardrails for AI coding agents (Claude Code, Codex), Git hooks, and CI.
* [agent-memory-kit](https://github.com/awrshift/agent-memory-kit) ⭐ 34 | 🐛 1 | 🌐 Python | 📅 2026-10-22 - Agent memory that asks before it writes: the agent proposes dated notes, you approve them, and they live as plain files in your repo, injected by hooks in Claude Code, Cursor CLI and OpenCode and read through skills and AGENTS.md in Codex and Copilot CLI.
* [Jump Skills](https://github.com/fabricioctelles/jump-skills) ⭐ 33 | 🐛 1 | 🌐 Shell | 📅 2026-10-24 - Meta-skills that route requests to specialized skills across Claude Code, Codex, Cursor, OpenCode, and other agent hosts.
* [Rider Skills](https://github.com/JetBrains/rider-skills) ⭐ 33 | 🐛 1 | 📅 2026-10-14 - Official JetBrains Rider agent skills that let AI coding agents use the IDE's semantic code understanding, refactoring, debugger, and test tooling in .NET and Unreal Engine projects.
* [xcode-mods](https://github.com/artemnovichkov/xcode-mods) ⭐ 33 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-21 - Claude Code plugin that brings Xcode build, run, tests, console and SwiftUI previews into live panes over the headless Xcode MCP server.
* [harness-eval](https://github.com/redhat-community-ai-tools/harness-eval) ⭐ 32 | 🐛 5 | 🌐 Python | 📅 2026-10-10 - Linter tool (static analysis rules) and LLM reviewer for AI agent harness files that runs quality and security health checks, catching cross-component security chains, redundancy, and config drift, and vets individual skills before install, across Claude Code, Cursor, Codex, Copilot, Gemini, and OpenCode.
* [Ultralytics Agent Skills](https://github.com/ultralytics/skills) ⭐ 32 | 🐛 2 | 📅 2026-10-22 - Agent skills for the Ultralytics YOLO computer vision lifecycle: datasets, training, tuning, inference, tracking, and export.
* [BioNexus](https://github.com/HERRY423/BioNexus) ⭐ 31 | 🐛 12 | 🌐 Python | 📅 2026-10-22 - Warrant-first scientific reliability layer for AI bioinformatics that audits analytical assumptions, calibrates evidence strength, caps unsupported claims, and verifies execution provenance.
* [go-ultimate](https://github.com/Djarvur/go-ultimate) ⭐ 31 | 🐛 2 | 🌐 Go | 📅 2026-10-18 - Opinionated Go skill that routes any Go task (CLI, library, backend service, MCP server, AI agent) to the right architecture, conventions, and review checklist across Claude Code, Codex, Cursor, Grok Build, Copilot CLI, and OpenCode.
* [Stark](https://github.com/f0d010c/stark) ⭐ 31 | 🐛 3 | 🌐 Python | 📅 2026-07-26 - UI/UX design plugin for AI coding agents with product-flow routing, platform-native interface guidance, asset planning, and shipped-reference analysis before code.
* [Agent Context OS](https://github.com/conorbronsdon/agent-context-os) ⭐ 30 | 🐛 6 | 🌐 Python | 📅 2026-10-15 - Portable Git-backed context and session workflow layer with first-class Claude Code, Codex, and OpenClaw support plus experimental adapters for Hermes, Cursor, and Devin.
* [Harness Kit](https://github.com/romabeckman/harness-kit) ⭐ 30 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-23 - Agentic development harness for orchestrating specification, implementation, review, and telemetry across multiple AI coding assistants.
* [geml](https://github.com/geml-spec/geml) ⭐ 29 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-24 - An agent-native markup language featuring deterministic block-level editing and built-in validation to ensure documents never drift or break during AI operations.
* [harmonyos-skills](https://github.com/liasica/harmonyos-skills) ⭐ 29 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Offline mirror of 16,800+ HarmonyOS NEXT official docs packaged as a Codex / Claude Code skill and MCP server, so AI coding assistants answer ArkTS / ArkUI / API questions with cited sources.
* [Hera Agent Unity](https://github.com/NotNull92/hera-agent-unity) ⭐ 29 | 🐛 0 | 🌐 C# | 📅 2026-10-23 - Controls and verifies a live Unity Editor through a low-token CLI, with scene, asset, Inspector, Play Mode, test, screenshot, and runtime C# workflows for Codex and other coding agents.
* [NixKits](https://github.com/Kihara777/NixKits) ⭐ 29 | 🐛 0 | 🌐 Nix | 📅 2026-10-25 - Declarative Nix flake collection that keeps coding-agent packages and NixOS modules updated and reproducible, with maintenance skills covering upstream version checks, NixOS CLI usage, config recovery, and multilingual project docs.
* [Pixel](https://github.com/Pixel-CLI/pixel) ⭐ 29 | 🐛 9 | 🌐 Rust | 📅 2026-10-25 - Local, deterministic code index that Claude Code, Codex, Pi, OpenCode and other coding agents query for signatures, callers, impact and Git history instead of reading whole files.
* [ThumbGate](https://github.com/IgorGanapolsky/ThumbGate) ⭐ 29 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - Pre-action infrastructure firewall for AI coding agents: feedback becomes lessons and prevention rules enforced by PreToolUse hooks across Claude Code, Codex, Gemini, and MCP.
* [HOTL Plugin](https://github.com/yimwoo/hotl-plugin) ⭐ 27 | 🐛 1 | 🌐 Shell | 📅 2026-07-06 - Human-on-the-Loop AI coding workflow plugin for Codex, Claude Code, and Cline with structured planning, review, and verification guardrails.
* [VibePortrait](https://github.com/dadwadw233/VibePortrait) ⭐ 27 | 🐛 2 | 🌐 HTML | 📅 2026-04-08 - Developer personality portrait generator — analyzes AI conversation history to produce MBTI type (16 color themes), capability radar, developer rating, 3-dimension famous match, and a persona skill that lets any AI "think like you".
* [claude-supertool](https://github.com/Digital-Process-Tools/claude-supertool) ⭐ 26 | 🐛 24 | 🌐 Python | 📅 2026-10-05 - Batches file, git and tracker operations into one round-trip, collapsing many reads, greps and globs into a single call for fewer output tokens and less wall time.
* [Filesystem MCP](https://github.com/j0hanz/filesystem-mcp) ⭐ 26 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-24 - MCP server: read, write, search, diff and patch files in allowed folders, with secret files blocked and confirmation before risky changes.
* [Frappe Agent](https://github.com/Dkm0315/frappe-agent) ⭐ 26 | 🐛 3 | 📅 2026-10-11 - Frappe and ERPNext coding, customization, bench, and review intelligence for Codex.
* [AgentPack](https://github.com/vishal2612200/agentpack) ⭐ 25 | 🐛 18 | 🌐 Python | 📅 2026-10-25 - Ranks repo context for Codex with likely files, skill recommendations, agent rules, commands, warnings, and compact task-focused packs before editing.
* [antidote](https://github.com/Avtr99/antidote) ⭐ 25 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-15 - An antidote to AI patchwork: stops agents from hiding bugs behind guards and makes them remove the cause.
* [Espresso](https://github.com/mirkobozzetto/espresso) ⭐ 25 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-17 - Full token-saving stack in one plugin - output compression, global rules, RTK hook, Caveman ultra, GitNexus config. Detects existing setup, installs only what's missing. Works on Claude Code and Codex.
* [agentic-readiness-assessment](https://github.com/exadel-inc/agentic-readiness-assessment) ⭐ 24 | 🐛 1 | 🌐 Python | 📅 2026-10-22 - Agent skill that audits a repository for AI coding agent readiness and produces an evidence-based scorecard with prioritized fixes.
* [Rel.AI MCP](https://github.com/Kyne0328/rel-ai-mcp) ⭐ 24 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-18 - Brings Codex-style coding workflows to ChatGPT Web, connecting it to local development workspaces through MCP while using ChatGPT Web quota instead of Codex quota.
* [Vanguard Frontier Agentic](https://github.com/VincentChuWaiChow/vanguard-frontier-agentic) ⭐ 24 | 🐛 0 | 🌐 Rust | 📅 2026-10-23 - Multi-harness marketplace of skills, specialist agents, rules, and MCP references for guarded cloud, platform, compliance, and business workflows.
* [Web Search MCP](https://github.com/sydasif/web-search-mcp) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-10-05 - Comprehensive FastMCP server giving LLMs real-time web access across search engines (DuckDuckGo, Exa), social platforms (Reddit, Hacker News, GitHub, X, LinkedIn), and academic tools (arXiv, Wikipedia), with SSRF-protected URL fetching.
* [A Team](https://github.com/RBraga01/a-team) ⭐ 23 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-21 - Universal multi-agent infrastructure with 25 specialist agents, 16 enforced workflow skills, and a lead orchestrator for Claude Code, Codex CLI, Cursor, and OpenCode.
* [agentglass](https://github.com/BjoernSchotte/agentglass) ⭐ 23 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-20 - Native terminal UI and JSON CLI that shows every Claude Code, Codex, Gemini CLI, pi, OpenCode, Kiro and fx session on your machine live, down to each tool call, diff, cost and stuck-agent alert.
* [Agnostic-AI](https://github.com/ucsandman/Agnostic-AI) ⭐ 23 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Capture your Claude Code or Codex harness once (rules, hooks, skills, subagents, commands and MCP servers) and apply it identically to Gemini CLI, Cursor, Antigravity and 16 more clients.
* [Embedded Workbench](https://github.com/AmethystLuna/embedded-workbench) ⭐ 23 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - Embedded C/C++ firmware development toolbox — 7 skills (FreeRTOS, Keil MDK, ARMCLANG, HardFault triage, state machines, LVGL) plus workflow gates and 4 agents for Claude Code, Codex, Cursor, Kimi, OpenCode, and ZCode.
* [SOTA Engineering Skills](https://github.com/martinholovsky/SOTA-skills) ⭐ 23 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Router-mapped library of 40 domain and language skills with BUILD and AUDIT modes, loading only the rules a task needs and ending every rules file in an audit checklist.
* [Supergraph](https://github.com/datit309/supergraph) ⭐ 23 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-23 - Engineering workflow system for AI coding agents that enforces planning, TDD, verification, review, and architecture-aware decisions with local codebase graph intelligence across Claude Code, Codex CLI, Antigravity, and OpenCode,..
* [synthesis-skills](https://github.com/synthesisengineering/synthesis-skills) ⭐ 23 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Engineering workflow skills (planning, review, rituals, fleet co-op) for Claude Code, Codex, and Muse, shipped through a gated cross-client release train.
* [agent-kit](https://github.com/agent-kit-startup/agent-kit) ⭐ 22 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-25 - Extension pack of slash commands, skills, rules, and hooks adding plan-driven, confirmation-gated coding and staging-to-prod git workflows to Cursor and Claude Code.
* [agent-sounds](https://github.com/lodev09/agent-sounds) ⭐ 22 | 🐛 0 | 🌐 Shell | 📅 2026-10-05 - Sound feedback plugin playing game voice lines on Claude Code and Codex session events, configurable by source and volume.
* [gemini-for-kubernetes-development](https://github.com/gke-labs/gemini-for-kubernetes-development) ⭐ 22 | 🐛 94 | 🌐 Go | 📅 2026-10-25 - Gemini CLI extension that automates Kubernetes development tasks: declarative validation authoring, PR review, and SIG API Machinery issue triage.
* [LLMSlim](https://github.com/Thanatos9404/llmslim) ⭐ 22 | 🐛 4 | 🌐 Python | 📅 2026-10-24 - MCP server: long-term memory for Claude Code, Codex and other MCP clients with no LLM in the loop, storing messages word for word in local SQLite and recalling the ones that answer a question within a token budget; also packaged as a Claude Code plugin and a Codex plugin.
* [opencode-chromium](https://github.com/Quindart-com/opencode-chromium) ⭐ 22 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-24 - Chromium browser automation extension collection providing an MCP server, OpenCode plugin, browser skill, and SDK with four browser tools.
* [mcp-zuul](https://github.com/imatza-rh/mcp-zuul) ⭐ 21 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - MCP server for Zuul CI with 48 tools for build analysis, failure diagnosis, log search, flaky job detection, pipeline status, and live console streaming.
* [Shadowclone](https://github.com/theonly1me/shadowclone) ⭐ 21 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - Turns the engineering preferences you keep repeating into reusable skills and instructions for Claude Code, Codex, Cursor, and Antigravity.
* [CodeEraser](https://github.com/skymanbp/CodeEraser) ⭐ 20 | 🐛 0 | 🌐 Haskell | 📅 2026-10-17 - Claude Code plugin whose hooks intercept a duplicate write before it lands, audit the net lines and the touched duplicates at Stop and walk the findings to safe deletions through an erase skill, backed by a clone index in a per-project daemon; the same index serves a CLI and an MCP server for scan, dedup, dead code and churn.
* [daimon](https://github.com/Daily-Nerd/daimon) ⭐ 20 | 🐛 22 | 🌐 Python | 📅 2026-10-24 - Session memory for Claude Code and Codex that writes a checkpoint when a session ends and opens the next one with a briefing of decisions and open loops, each marked as a verbatim quote or an inference, with PR, branch and file claims checked against live state.
* [Epic Harness](https://github.com/epicsagas/epic-harness) ⭐ 20 | 🐛 7 | 🌐 Rust | 📅 2026-10-24 - Auto-trigger quality skills + self-evolving agent harness — orbit (spec-to-ship), evolve (skill mutation), team (multi-agent), TDD, check, ship, simplify, debug, perf, secure.
* [Generative Media Skills](https://github.com/SamurAIGPT/Generative-Media-Skills) ⭐ 20 | 🐛 1 | 🌐 Shell | 📅 2026-09-29 - 13 skills for image, video, and audio generation using 100+ models - FLUX, Midjourney v7, Veo3, Kling 3.0, Suno, and HunyuanVideo via muapi.ai.
* [RAG Reviewer](https://github.com/mimfort/rag_for_git) ⭐ 20 | 🐛 6 | 🌐 Python | 📅 2026-10-25 - Agentic PR review: hybrid RAG + code graph via MCP, review skills for Codex.
* [SEO Skills AI](https://github.com/seoskillsai/seo-skills-ai) ⭐ 20 | 🐛 3 | 🌐 Python | 📅 2026-10-22 - Universal SEO skill suite and technical audit engine for Claude Code, Cursor, Codex, and other agents, with first-party Python adapters and HOL plugin-scanner CI.
* [vibekit](https://github.com/rizukirr/vibekit) ⭐ 20 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-25 - Evidence-based guardrail pipeline for vibe coding: brainstorm, plan, one fresh agent per task, verify, across Claude Code, Codex, opencode, and Antigravity.
* [aide](https://github.com/jmylchreest/aide) ⭐ 19 | 🐛 0 | 🌐 Go | 📅 2026-10-19 - Persistent memory, code intelligence, and multi-agent orchestration for Claude Code, OpenCode, and Codex CLI via skills, hooks, and an MCP server.
* [coffee-paladin](https://github.com/pawelkwaczynski/coffee-paladin) ⭐ 19 | 🐛 1 | 🌐 Python | 📅 2026-10-23 - Thermal guard for Apple Silicon: pauses hot jobs before the Mac throttles and gates Claude Code, Codex and Gemini CLI before heavy commands.
* [pbx-mcp](https://github.com/ictinnovations/pbx-mcp) ⭐ 19 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-09 - MCP server for Asterisk (AMI) and FreeSWITCH (ESL). Inspect channels, SIP registrations, trunks, and dialplan on a live PBX.
* [RagLeap](https://github.com/antonyrag/ragleap-core) ⭐ 19 | 🐛 78 | 🌐 Python | 📅 2026-10-25 - Self-hosted AI employee platform with 46 agents, Graph RAG on Neo4j, BYOK across providers, MIT.
* [VASTlint](https://github.com/aleksUIX/vastlint) ⭐ 19 | 🐛 2 | 🌐 Rust | 📅 2026-10-24 - Validate VAST, VMAP, and DAAST ad tags against IAB Tech Lab specs via Gemini CLI, Claude Code, and a hosted MCP server.
* [BGS Modding Superpowers](https://github.com/BB-84C/bgs-modding-superpowers) ⭐ 18 | 🐛 3 | 🌐 Python | 📅 2026-10-01 - Agentic Bethesda Game Studio modpack curation toolkit with MCP-driven xEdit conflict audit, MO2 control plane, BA2/BSA and Papyrus tooling, and skills for setup, dev-log, and release-changelog workflows.
* [cache-warmer](https://github.com/paulbkim-dev/claude-code-cache-warmer) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-23 - Claude Code plugin that keeps the prompt cache warm through idle gaps by sending one small refresh shortly before the 5-minute or 1-hour cache expires.
* [CommitLore](https://github.com/MongLong0214/commitlore) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-18 - Keeps constraints, rejected alternatives, and warnings in Git trailers and serves them back to the agent before it edits a file.
* [hiai-opencode](https://github.com/HiAi-gg/hiai-opencode) ⚠️ Archived - OpenCode plugin adding a multi-agent team with 10 specialist agents, execution gates, LSP tools, browser automation, and memory search.
* [Neo](https://github.com/Parslee-ai/neo) ⭐ 18 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Code reasoning plugin for Claude Code and Codex that runs multi-agent analysis over relevant repository files and keeps a local semantic memory, promoting a lesson only after its suggestions are verified as accepted in git.
* [TermaGITchi](https://github.com/TevvvB/termagitchi) ⭐ 18 | 🐛 3 | 🌐 Go | 📅 2026-10-20 - Stable per-worktree identity for parallel Claude Code, Codex, and tmux sessions; mood reads repository hygiene, not what the agent is doing.
* [Alcove](https://github.com/epicsagas/alcove) ⭐ 17 | 🐛 0 | 🌐 Rust | 📅 2026-10-23 - Local-first MCP server for private project docs with hybrid BM25+vector search, tree-sitter code indexing, and automated linting for team-wide documentation standards.
* [Blender Developer Tools](https://github.com/TMHSDigital/Blender-Developer-Tools) ⭐ 17 | 🐛 18 | 🌐 Python | 📅 2026-10-25 - 16 skills, 9 rules, snippets, templates, and smoke-tested examples for Blender Python add-on and scripting work with correct 4.5 LTS and 5.2 LTS APIs, installable as a Claude Code plugin and usable from Cursor.
* [ictexam-mcp](https://github.com/ictinnovations/ictexam-mcp) ⭐ 17 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for reading exams, gradebooks, and item analysis, with opt-in tools for AI question-paper parsing and exam publishing.
* [ictfax-mcp](https://github.com/ictinnovations/ictfax-mcp) ⭐ 17 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for ICTFax. List and track fax transmissions, with opt-in tools to upload documents and send faxes.
* [jev-router](https://github.com/dominicrico/jev-router) ⭐ 17 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-23 - Claude Code plugin that asks TypeSafe Jev which Claude model and reasoning effort each prompt, step and subagent needs, with an effort cap, a prompt-cache guard and a status band above the prompt.
* [MARGINAL](https://github.com/SignalLayerLabs/Marginal) ⭐ 17 | 🐛 19 | 🌐 Python | 📅 2026-10-21 - Local-first runtime governor for AI coding agents that detects proven no-progress repetition, records decision evidence, starts in Shadow Mode, and earns narrow enforcement only after repository-local evidence.
* [opencode-plugin-peers](https://github.com/jkrandom-sudo/opencode-plugin-peers) ⭐ 17 | 🐛 7 | 🌐 JavaScript | 📅 2026-10-20 - OpenCode plugin for cross-session messaging: independent instances on the same machine discover each other and exchange plain-text messages.
* [Clean Room](https://github.com/whit3rabbit/clean-room-skill) ⭐ 16 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-14 - Spec-first clean-room workflow for authorized source analysis, behavioral specs, role separation, and verification without replacement code.
* [Docflow (EvolveHQ)](https://github.com/EvolveHQ/docflow) ⭐ 16 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-22 - ADR-driven documentation workflow for Claude Code, Codex, Cursor, OpenCode, pi, and more that scaffolds an ADR catalogue, plan queue, and AGENTS.md conventions into single repos or portable multi-repo workspaces, with lifecycle skills to author, ship, and audit decisions.
* [ejentum-mcp](https://github.com/ejentum/ejentum-mcp) ⭐ 16 | 🐛 2 | 🌐 JavaScript | 📅 2026-06-11 - MCP server exposing reasoning, code, anti-deception, and memory harness tools for Codex.
* [ictcontact-mcp](https://github.com/ictinnovations/ictcontact-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTContact contact center. Monitor outbound campaigns, with opt-in tools to start and stop them.
* [ictdialer-mcp](https://github.com/ictinnovations/ictdialer-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTDialer cloud auto-dialer. Monitor outbound campaigns, with opt-in start and stop controls.
* [ictpbx-mcp](https://github.com/ictinnovations/ictpbx-mcp) ⭐ 16 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - Read-only MCP server for ICTPBX. Inspect extensions, DID numbers, SIP trunks, tenants, and live PBX statistics.
* [Jev Studio](https://github.com/utk2103/jev-studio) ⭐ 16 | 🐛 6 | 🌐 Python | 📅 2026-10-11 - One-stop kit for playing with TypeSafe's Jev: MCP tools for Choice/Noul/Score, ready-made prompt libraries, and slash commands for every cookbook.
* [jevyoumean](https://github.com/syumai/jevyoumean) ⭐ 16 | 🐛 3 | 🌐 Go | 📅 2026-10-21 - CLI wrapper that uses TypeSafe's Jev to give semantic "Did you mean?" suggestions for mistyped subcommands, matching by intent rather than edit distance (e.g. `git record` → `git commit`).
* [MeMesh](https://github.com/PCIRCLE-AI/memesh) ⭐ 16 | 🐛 68 | 🌐 TypeScript | 📅 2026-10-21 - Local SQLite memory shared by Claude Code, Codex, Gemini, Cursor, and other MCP clients, captured automatically by hooks from real work and injected at the moment the agent acts.
* [Project Autopilot](https://github.com/AlexMi64/codex-project-autopilot) ⭐ 16 | 🐛 2 | 🌐 Python | 📅 2026-04-09 - Turn an idea into a structured project workflow with planning, execution, verification, and handoff.
* [jev-harness](https://github.com/AntonioCoppe/jev-harness) ⭐ 15 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-25 - Decision harness for TypeSafe Jev (confidence gates, shadow mode, recipes, eval CLI)
* [KOZMOS](https://github.com/ersinkoc/claude-mods) ⭐ 15 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-20 - 48 live, visual function-hook mods for Claude Code in the terminal and desktop app: animated bands above the prompt, sidebars, a status ticker, companions, guards, and sound for usage limits, context, subagents, git, and cost.
* [opencode-9router](https://github.com/vheins/opencode-9router) ⭐ 15 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-25 - OpenCode plugin that registers 9Router as a provider with automatic model discovery and caching.
* [trigger-tree](https://github.com/Hedde/trigger_tree) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2026-10-24 - Local documentation telemetry for Claude Code and Codex: see which docs your agent actually reads, gate discoverability in CI, and measure instruction adherence.
* [WebLatexMCP](https://github.com/elias-ramzi/WebLatexMCP) ⭐ 15 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-20 - MCP server plus bundled skills for editing, compiling, and committing LaTeX in git-hosted projects like Overleaf.
* [BABOK Analyst](https://github.com/GSkuza/BABOK_ANALYST) ⭐ 14 | 🐛 16 | 🌐 JavaScript | 📅 2026-10-22 - BABOK v3 business analysis agent with 16 MCP tools, a 9-stage pipeline, and human-in-the-loop approval gates.
* [Check and Fix Accessibility](https://github.com/Neha/check-fix-accessibility) ⭐ 14 | 🐛 1 | 🌐 Python | 📅 2026-10-01 - Agent skill that audits and fixes front-end accessibility to WCAG 2.2 A/AA, covering semantics, keyboard navigation, ARIA, forms, contrast, and screen readers for web and native mobile across Cursor, Claude Code, Codex, Kiro, and Antigravity.
* [Codex Agenteam](https://github.com/yimwoo/codex-agenteam) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-07-06 - Specialist AI agents (researcher, PM, architect, developer, QA, reviewer) orchestrated as a configurable team pipeline.
* [Codex How To](https://github.com/Phelan164/codex-howto) ⭐ 14 | 🐛 5 | 🌐 Python | 📅 2026-10-23 - Engineering-first Codex curriculum and plugin with 9 skills, measured token-efficiency experiments, bounded orchestration, testing, review, and living knowledge maintenance.
* [Codex Reviewer](https://github.com/schuettc/codex-reviewer) ⭐ 14 | 🐛 0 | 📅 2026-05-05 - Second-pass review of Claude-driven plans and implementations.
* [Flow Scenes](https://github.com/robdmac/flow) ⭐ 14 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-16 - Ambient pixel-art scenes above the prompt (a campfire, surf, rockets, a train, the Tesla Roadster and more) that speed up with the agent's work, give each subagent a companion of its own, and play optional soundscapes, in Claude Code, opencode and pi.
* [Kernel](https://github.com/ariaxhan/kernel-claude) ⭐ 14 | 🐛 17 | 🌐 Python | 📅 2026-10-23 - Claude Code plugin marketplace and Codex plugin: hooks that block destructive commands, spawn guards on subagent contracts, agentdb memory with recall-before-act, blind verifiers, deterministic review; install with `/plugin marketplace add ariaxhan/kernel-claude`.
* [NeatContext](https://github.com/XTSoftwareLabs/neatcontext-plugins) ⭐ 14 | 🐛 3 | 🌐 JavaScript | 📅 2026-08-23 - Saves the durable knowledge from Claude Code, Codex, GitHub Copilot, Kimi Code, and pi conversations as structured, reusable contexts you can reconnect in later sessions or share with your team.
* [Staff Engineer Mode](https://github.com/sirmarkz/staff-engineer-mode) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-08-01 - Routes engineering design, delivery, reliability, security, operations, and maintenance prompts to focused staff-level specialist guidance for AI coding agents.
* [Super Jev](https://github.com/Kevthetech143/super-jev) ⭐ 14 | 🐛 7 | 🌐 Python | 📅 2026-10-16 - One judge between your agent and your data: finds the right skill and file, checks claims, gates actions, and remembers only the answers you approve.
* [adr-kit](https://github.com/rvdbreemen/adr-kit) ⭐ 13 | 🐛 1 | 🌐 Python | 📅 2026-10-24 - Architecture Decision Record toolkit for Claude Code, Codex, GitHub Copilot CLI, and OpenCode that injects the governing decisions before each edit, guides ADR authoring, and enforces decisions in deterministic pre-commit and CI gates.
* [BioSymphony Structure Factory](https://github.com/BioSymphony/structure-factory) ⭐ 13 | 🐛 1 | 🌐 Python | 📅 2026-10-12 - Turn structural biology questions into agent-ready campaigns for protein design, structure prediction, and model comparison, with reproducible workflows and verifiable results.
* [chat-history](https://github.com/ay-bh/chat-history) ⭐ 13 | 🐛 1 | 🌐 Rust | 📅 2026-09-25 - Claude Code/Codex/Cursor history search + export.
* [Claude Code Harness](https://github.com/dadwadw233/claude-code-harness) ⭐ 13 | 🐛 1 | 📅 2026-04-05 - Harness blueprint skill for turning vague agent ideas into concrete designs for request assembly, control loops, memory, permissions, recovery, and extension planes.
* [Claude Watchdog](https://github.com/Temikus/claude-watchdog) ⭐ 13 | 🐛 4 | 🌐 Shell | 📅 2026-10-19 - Stop hook that runs a critical post-mortem on every Claude Code session, cross-checking what was asked against the actual git diff for missed goals, wasted detours, and unverified claims.
* [i-m-senior-developer](https://github.com/spumer/i-m-senior-developer) ⭐ 13 | 🐛 8 | 🌐 Python | 📅 2026-10-21 - A collection of Claude Code plugins covering TDD, code clarity, planning, review roles, and context upkeep.
* [MoonMind](https://github.com/MoonLadderStudios/MoonMind) ⭐ 13 | 🐛 24 | 🌐 Python | 📅 2026-10-25 - Self-hosted app that orchestrates Codex, Claude Code, and OpenCode through durable Temporal workflows, with a dashboard to inspect progress, logs, and artifacts. <!-- platform: standalone -->
* [opencode-nexus](https://github.com/mohammad154/opencode-nexus) ⭐ 13 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-21 - OpenCode plugin with a fixed three-agent execution workflow, conditional planning advice, fresh impact analysis, deterministic verification, and durable run state.
* [Writer's Loop](https://github.com/xxsang/writers-loop) ⭐ 13 | 🐛 2 | 🌐 JavaScript | 📅 2026-09-21 - Structured AI writing workflow for planning, critique, revision, translation, style distillation, and opt-in local preference learning.
* [Development Skills](https://github.com/reidemeister94/development-skills) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2026-09-20 - Three-tier triage (PASS\_THROUGH / LIGHT / FULL 4-phase) development workflow for Codex and Claude Code with language auto-detection (Python, Java, TypeScript, Swift, frontend) and a staff-reviewer subagent for fresh-eyes review on every change.
* [Hera Agent Godot](https://github.com/NotNull92/hera-agent-godot) ⭐ 12 | 🐛 0 | 🌐 Go | 📅 2026-10-23 - Drives a live Godot 4.x editor through the low-token Hera CLI — scene, node, and signal edits, play control, and runtime QA with verifiable compact JSON output, with the companion addon published on the official Godot Asset Store.
* [herdrpowers](https://github.com/transparent-pegasus/herdrpowers) ⭐ 12 | 🐛 1 | 🌐 Shell | 📅 2026-10-25 - Skill and command pack that runs a multi-phase TDD development cycle, delegating implementation, testing, and review to sibling agent panes.
* [LinkedIn Animated Infographics](https://github.com/imMamdouhaboammar/linkedin-animated-infographics) ⭐ 12 | 🐛 47 | 🌐 Python | 📅 2026-10-23 - Evidence-safe animated infographic generator with multi-agent design pipeline for LinkedIn.
* [LoreConvo](https://github.com/labyrinth-analytics/loreconvo) ⭐ 12 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Persistent session memory MCP server for Claude — auto-saves and recalls conversation context, decisions, and artifacts across Claude Code, chat, and other surfaces with full-text search.
* [miru-code](https://github.com/takara-ai/miru-code) ⭐ 12 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-21 - MCP server and multi-IDE plugin giving coding agents semantic and hybrid code search tools.
* [opencode-plugin-loop](https://github.com/jkrandom-sudo/opencode-plugin-loop) ⭐ 12 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-20 - OpenCode plugin adding a /loop command that runs prompts on fixed, adaptive, or one-shot schedules per session.
* [Orka](https://github.com/ugorur/orka) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-10-14 - Orchestrates headless coding-agent CLIs (Codex, Grok, Claude Code, Cursor, Gemini, OpenCode, Copilot) as a team in isolated git worktrees, with cross-model review, QA and a scored run ledger.
* [Praxis](https://github.com/ouonet/praxis) ⭐ 12 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-01 - Intent-driven workflow skills for coding agents: describe what done looks like, not the steps. Triage-first design keeps token costs low across design, TDD, debug, review, and release.
* [React Native Developer Skills](https://github.com/Neha/rn-developer-skills) ⭐ 12 | 🐛 4 | 🌐 JavaScript | 📅 2026-09-29 - Vendor-neutral React Native skill collection covering spec authoring, architecture, performance, security, testing, and code review for Codex, Claude, and Cursor.
* [simpleviz](https://github.com/sstoehrm/simpleviz) ⭐ 12 | 🐛 5 | 🌐 Clojure | 📅 2026-10-25 - Skill teaching agents the simpleviz EDN graph format and CLI so they can author, serve, and compare diagram files.
* [sqlite-graph-memory](https://github.com/tonydzi/sqlite-graph-memory) ⭐ 12 | 🐛 12 | 🌐 Python | 📅 2026-10-24 - MCP server: persistent memory for Claude Code, Codex and Cursor over your own markdown notes, with vector retrieval, a hand-curated wikilink graph and cross-encoder rerank in one SQLite file.
* [Tool Advisor](https://github.com/dragon1086/claude-skills) ⭐ 12 | 🐛 2 | 🌐 Shell | 📅 2026-04-23 - Read-only meta-skill that scans your MCP servers, skills, plugins, and CLI tools, then suggests up to three ranked approaches (Methodical / Fast / Deep) with a copy-paste Quick Action table.
* [Agent Harness Skills](https://github.com/yfge/agent-harness-skills) ⭐ 11 | 🐛 4 | 🌐 Python | 📅 2026-07-14 - Designs agent-ready repository harnesses with entrypoints, validation surfaces, runtime evidence, delivery records, and atomic commit guidance.
* [Agentic Ship](https://github.com/moasq/agentic-ship) ⭐ 11 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-23 - Cross-host product-development toolkit for Claude Code, Codex, Cursor, Hermes, and OpenClaw with shared rules, specialist roles, service connections, and machine-checked UI, backend, security, and launch gates.
* [Game Development Studio](https://github.com/theisegoria/game-development-studio) ⭐ 11 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-23 - CLI, skills, and MCP server for game asset production, vendoring, visual debugging, and performance analysis.
* [ken](https://github.com/rajnandan1/ken) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Thompson-mode coding discipline for Claude Code, Codex, Gemini CLI, OpenCode, pi, and any AGENTS.md-reading agent: think first, build bottom-up, brute force until measured, and rewrite a thrice-patched unit instead of patching it a fourth time.
* [opencode-mempalace-persistence](https://github.com/geco/opencode-mempalace-persistence) ⭐ 11 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-19 - OpenCode plugin that archives conversations to local MemPalace memory and recalls past decisions verbatim in later sessions.
* [opencode-weave](https://github.com/weave-io/weave) ⭐ 11 | 🐛 49 | 🌐 TypeScript | 📅 2026-10-15 - OpenCode plugin providing multi-agent orchestration with specialized agents, category task dispatch, and background sub-agent execution.
* [Salesforce Compound Engineering](https://github.com/divingsbysangam/salesforce-compound-engineering-plugin) ⭐ 11 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-23 - Salesforce-focused compound engineering plugin for Claude Code, Cursor, Codex, and other AI coding tools, with skills-first workflows, parallel persona dispatch, and Apex/LWC/Flow coverage.
* [Simple Man](https://github.com/Maksim-Burtsev/simple-man) ⭐ 11 | 🐛 2 | 🌐 Python | 📅 2026-10-01 - High-compression communication mode for Codex agents that removes filler while preserving search, validation, and implementation effort.
* [Agent Harness](https://github.com/0xenzyme/agent-harness) ⭐ 10 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-16 - Coding-agent plugin that routes project work through goals, tasks, runs, evidence gates, and state sync via project adapters.
* [AI-Native SDLC Loop](https://github.com/ghiaog123/ai-native-sdlc) ⭐ 10 | 🐛 0 | 🌐 Shell | 📅 2026-10-25 - Six-stage SDLC where hooks enforce the loop at the tool-call level: an artifact gate refuses source writes no approved plan covers, and 8 skills with 2 read-only subagents drive intent through control bands.
* [Casefile](https://github.com/x4cc3/casefile) ⚠️ Archived - Persistent security case tracking for bug bounties, CTFs, and security audits.
* [oddyssey](https://github.com/using-system/oddyssey) ⭐ 10 | 🐛 1 | 🌐 Python | 📅 2026-10-21 - Observability-Driven Development for coding agents: instrument an application or an AI agent with OpenTelemetry (gen\_ai semantic conventions: model, agent, tool and MCP spans, token and latency metrics), observe a run through its metrics, traces, logs and profiles on a local Grafana stack or a remote backend, benchmark it with k6, and verify that a fix landed.
* [Phone a Friend](https://github.com/freibergergarcia/phone-a-friend) ⭐ 10 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-19 - CLI with Claude Code, Codex, OpenCode, and pi plugins that sends prompts and diff-scoped code reviews to Claude, Codex, Gemini, Antigravity, OpenCode, pi, or Ollama for second opinions, with structured review verdicts, resumable sessions, and multi-model team workflows.
* [skills](https://github.com/pwguler/skills) ⭐ 10 | 🐛 0 | 📅 2026-10-16 - Agent skills against the debt coding agents leave behind: unsettled plans, untested code, and claims nobody checked.
* [Spec-Driven Development](https://github.com/Habib0x0/spec-driven-plugin) ⭐ 10 | 🐛 0 | 🌐 Shell | 📅 2026-05-18 - Three-phase Requirements → Design → Tasks workflow for Claude Code and Codex — EARS notation acceptance criteria, autonomous execution loop, cross-spec dependencies, and post-implementation acceptance testing.
* [Stvena](https://github.com/nccapo/stvena) ⭐ 10 | 🐛 0 | 🌐 Go | 📅 2026-09-29 - Terminal workspace for running Codex or Claude Code beside live diffs, full-file review, checks, staging, and precise code feedback.
* [cc-memory](https://github.com/skymanbp/cc-memory) ⭐ 9 | 🐛 0 | 🌐 Python | 📅 2026-10-17 - Persistent memory for Claude Code across compaction and sessions: reconcile-on-write with LLM-judged de-duplication, a forced PROGRESS.md handoff, a live PLAN.md anchor, FTS5 search, MCP tools and a GUI, in pure stdlib Python.
* [Demo GIF](https://github.com/conorbronsdon/demo-gif-skill) ⭐ 9 | 🐛 0 | 📅 2026-09-24 - Agent Skill that scripts, renders, optimizes, and embeds reproducible demo GIFs for CLI, TUI, web, and library projects using VHS or Playwright plus ffmpeg.
* [md-prompt](https://github.com/nogu66/md-prompt) ⭐ 9 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-16 - Claude Code plugin that paints Markdown onto the prompt box as you type, turning fenced code into syntax-highlighted cards without changing the text you send.
* [Professor](https://github.com/rezzminator/professor) ⭐ 9 | 🐛 3 | 🌐 Go | 📅 2026-10-23 - LLM-harness fleet framework for Claude Code, Codex, and OpenCode with a Go fleet CLI/TUI, cross-chat messaging, and a discipline layer of agents, commands, and hooks compiled across all three runtimes.
* [Releases Index](https://github.com/buildinternet/releases) ⭐ 9 | 🐛 199 | 🌐 TypeScript | 📅 2026-10-25 - Open release-notes registry with MCP and CLI so agents can search and fetch product changelogs.
* [Universal Design Principles](https://github.com/HDeibler/universal-design-principles) ⭐ 9 | 🐛 3 | 🌐 Markdown | 📅 2026-05-03 - Cross-agent UX and product-design marketplace with a root Codex collection plugin, five focused plugin bundles, and 137 Agent Skills for design review, accessibility, layout, interaction, cognition, and product polish.
* [debt-ops](https://github.com/bcanfield/agentic-tech-debt) ⭐ 8 | 🐛 14 | 🌐 Python | 📅 2026-10-24 - Catches AI-introduced tech debt at write-time: hooks log every deferral to a registry in your repo and a review skill ranks paydown by file churn.
* [GitCortex](https://github.com/bharath03-a/GitCortex) ⭐ 8 | 🐛 9 | 🌐 Rust | 📅 2026-10-18 - Branch-aware knowledge graph of a Git repo that incrementally re-indexes via tree-sitter and exposes it to AI coding assistants over MCP.
* [Tartiner Labs](https://github.com/tartinerlabs/skills) ⭐ 8 | 🐛 9 | 🌐 Go | 📅 2026-10-24 - Agent skills for git workflows, GitHub automation, security audits, code refactoring, and project tooling.
* [What's Agent Doing](https://github.com/tzafrir/whats-agent-doing) ⭐ 8 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-04 - Claude Code mod that says in plain English what each step is for, with a timer, plus a live row per background agent.
* [Zagrosi Forge](https://github.com/zagrosi-code/zagrosi-forge) ⭐ 8 | 🐛 0 | 🌐 Python | 📅 2026-10-22 - Decompose broad project briefs into researched plans and implement sectioned work with TDD, quality gates, and traceability.
* [ArmorCodex](https://github.com/armoriq/armorCodex) ⭐ 7 | 🐛 74 | 🌐 JavaScript | 📅 2026-10-20 - Intent-based security for Codex with MCP plan registration, policy gating, CSRG cryptographic proofs, and audit logging on `bash` and `apply_patch`.
* [Codex Subagent Playbook](https://github.com/shinpr/codex-subagent-playbook) ⭐ 7 | 🐛 0 | 📅 2026-10-22 - Routes subagent work using model and reasoning-effort defaults tuned through measured comparisons and daily Codex use: stronger models handle judgment-heavy research and review, lower-cost models execute well-specified plans, and Codex uses longer waits to avoid frequent polling, intervenes on stalls, and verifies results.
* [Contorium](https://github.com/ContoriumLabs/contorium) ⭐ 7 | 🐛 1 | 🌐 TypeScript | 📅 2026-07-27 - Runtime continuity layer for AI coding agents, providing persistent workspace state, Git-aware sessions, and MCP-based context retrieval across tools and agent runs.
* [Dev Skills](https://github.com/Jason-chen-coder/dev-skills) ⭐ 7 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-21 - Team workflow skills for specs, plans, TDD, debugging, verification, review, branch finishing, and design context.
* [LLM Transpile](https://github.com/epicsagas/llm-transpile) ⭐ 7 | 🐛 6 | 🌐 HTML | 📅 2026-10-24 - Auto-compress .md, .html, and .txt files via PostToolUse hook, cutting context usage by up to 40% with zero workflow change.
* [mutagate](https://github.com/keyboardsamurai/mutagate) ⭐ 7 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-20 - Mutation-testing hook for Claude Code, Codex, OpenCode, and Pi that mutates the code under each agent-written test and blocks completion until the tests kill at least 80% of the mutants.
* [River Review](https://github.com/s977043/river-review) ⭐ 7 | 🐛 41 | 🌐 JavaScript | 📅 2026-10-24 - Versioned Skill Registry of code-review skills driven by a perspective-based review agent (code, security, performance, architecture, testing, adversarial) that verifies findings against the diff.
* [Ultra Mod](https://github.com/mertkayacs/ultramod) ⭐ 7 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-23 - All-in-one mod pack for Claude Code: a usage limits and context HUD, a guard with undo for rm -rf and git reset --hard, .env and secret protection, and a receipt for every turn.
* [Windrunner](https://github.com/shzlw/windrunner) ⭐ 7 | 🐛 0 | 🌐 Java | 📅 2026-09-15 - Self-hosted project workspace with Spring AI, MCP, CLI, and multi-provider AI integrations.
* [Wingman](https://github.com/lsshym/wingman.ai) ⭐ 7 | 🐛 3 | 🌐 JavaScript | 📅 2026-09-29 - Cross-platform AI coding-agent plugin for repo-local project memory, data-contract checks, and project-map discovery before agents edit code.
* [cc-enforcer](https://github.com/skymanbp/cc-enforcer) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-10-15 - Claude Code hooks that deny a tool call and block a reply that patches reactively, cites by guess or claims done early; the rules also usable as an LLM-agnostic rule pack.
* [effect-actions](https://github.com/gjermundgaraba/effect-actions) ⭐ 6 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-24 - Agent skill and Effect library for defining a typed action once and serving it over HTTP, as MCP tools, as an AI Toolkit, and from a CLI.
* [GlanceFlow](https://github.com/Antreas-Strb/glanceflow) ⭐ 6 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-23 - Claude Code mod that replaces the wall of tool calls with one plain-English checklist above the prompt: the plan, live progress, a clear Needs-you state, time left learned from history, and a daily team report.
* [kgai](https://github.com/kgaidev/kgai) ⭐ 6 | 🐛 0 | 🌐 Go | 📅 2026-10-23 - Shared decision memory for AI dev teams — share the decisions and knowledge behind your code across Claude Code, Codex CLI and Gemini CLI as an immutable local log, synced over an S3 bucket you own.
* [Munim](https://github.com/vishalsg42/munim) ⭐ 6 | 🐛 5 | 🌐 Python | 📅 2026-10-01 - Multi-account MCP server that holds a separate OAuth session per client across 11 providers, forwards each provider's own tools with that client's credentials, and refuses any call that would send one client's credential to another host.
* [Pixeltable](https://github.com/pixeltable/pixeltable-skill) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Declarative multimodal AI data engine for tables, computed columns, embedding search, agents, and FastAPI services.
* [sci-paper](https://github.com/skymanbp/sci-paper) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-10-17 - Claude Code plugin for scientific paper writing, source-traced review and de-AI rewriting: 12 skills and 35 tools under one typed standard with non-waivable integrity blockers and explicit measurement states, calibrated on ApJ, MNRAS, PRD and JCAP manuscripts.
* [SlopBar](https://github.com/thelioo/slopbar) ⭐ 6 | 🐛 41 | 🌐 Rust | 📅 2026-09-28 - Windows taskbar widget that shows Claude Code and Codex plan usage, limit resets and alerts, and switches accounts before one runs out.
* [time-blame](https://github.com/karanb192/time-blame) ⭐ 6 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-17 - Claude Code mod that splits each turn's time into Claude, the tools it ran (named by command, such as npm test) and the user waiting on a permission dialog, on one line under the answer, with a /blame panel for the session.
* [Agent Workflow System](https://github.com/1139030773-cmd/agent-workflow-system) ⭐ 5 | 🐛 1 | 🌐 PowerShell | 📅 2026-06-12 - 一套中文AI工作流系统：7个协作技能 + 行为规范宪法 + 会话恢复机制，模糊目标→可执行任务，全生命周期引导。Codex & Claude Code 双平台，新手友好。
* [Codex rg Guard](https://github.com/Rycen7822/codex-rg-guard) ⭐ 5 | 🐛 3 | 🌐 Rust | 📅 2026-05-09 - Budgeted `rg`/`grep` replacement for Codex that narrows broad searches before they waste model context.
* [Cover My Repo](https://github.com/sjh9714/cover-my-repo) ⭐ 5 | 🐛 1 | 🌐 JavaScript | 📅 2026-08-23 - Designs three checked GitHub social preview cards with Codex or Cursor, then renders them locally with Chrome.
* [crayon](https://github.com/jonpojonpo/cc-crayon) ⭐ 5 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-02 - Claude Code plugin that redraws replies with themed Markdown and inline color tags Claude writes itself, across six switchable themes.
* [Logic Probe](https://github.com/AmethystLuna/logicprobe) ⭐ 5 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - Design-document & plan claim verification — checks every verifiable claim against the codebase, escalates behavioral claims to executable-model verification, compares before/after models for regression detection, and mines concurrency risk claims.
* [Maestro](https://github.com/mbanderas/maestro) ⭐ 5 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-01 - Opt-in local multi-CLI fusion engine and orchestration doctrine that fans a prompt across model CLIs, then judges and synthesizes one grounded answer.
* [MCP Migration Check](https://github.com/AlpayC/mcp-migration-check) ⭐ 5 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-19 - Deterministic MCP 2026-07-28 migration checker with an agent skill, CLI, GitHub Action, and hosted web probe powered by one rule engine.
* [Mental CLI](https://github.com/afaraha8403/mental) ⭐ 5 | 🐛 57 | 🌐 JavaScript | 📅 2026-10-08 - Local-first CLI that keeps where you left off and what’s still open across agent sessions so you can pick up without reconstructing from memory.
* [model-orchestration](https://github.com/divyamrastogi/model-orchestration) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2026-10-06 - Manager/worker orchestration for Claude Code: keep your smartest model as the manager and delegate implementation and token-hungry work to isolated headless workers backed by any Anthropic-compatible API (z.ai GLM, Kimi, DeepSeek, LiteLLM proxies).
* [remcycle](https://github.com/lianmatsuo/remcycle) ⭐ 5 | 🐛 2 | 🌐 Python | 📅 2026-10-20 - Garbage collection for Claude Code's memory: a mod that rereads your sessions every day, keeps what you decided, and questions the notes that have gone stale.
* [ReportCraft MCP](https://github.com/hitarthombre/report-craft-mcp) ⭐ 5 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-10 - MCP server that automates academic and project report generation through screenshots, source code collection, self-contained HTML, and personalized PDF exports.
* [telepathy](https://github.com/Winterrks/telepathy) ⭐ 5 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-09 - Lets coding-agent sessions on one machine (Claude Code, Codex, OpenCode, Gemini CLI, Copilot CLI, Cursor, Grok, Devin, Antigravity, Kimi Code, Qwen Code, Kilo Code) find and message each other through the same three MCP tools, starting a turn in an idle session where the agent allows it, with no network calls or telemetry.
* [VillageSQL Skills](https://github.com/villagesql/villagesql-skills) ⭐ 5 | 🐛 0 | 📅 2026-10-13 - Skills for VillageSQL including building extensions from scratch and porting PostgreSQL extensions to VillageSQL.
* [Agent Deck](https://github.com/not-so-fat/agent-deck) ⭐ 4 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-25 - One MCP for context management: bind self-improving playbooks, MCP tools, and API keys to the session.
* [Agentizer](https://github.com/Humiris/wwa-transform) ⭐ 4 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-05 - Turn any website into an AI-powered agentfront with split-pane
* [AgiFlow](https://github.com/AgiFlow/ai-plugin) ⭐ 4 | 🐛 1 | 📅 2026-10-10 - Project management workflows for AI coding agents with planning, grooming, task execution, review, and AgiFlow MCP integration.
* [Cluadex](https://github.com/leepokai/cluadex) ⭐ 4 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-05 - Lightweight take on LCU for Claude Code only: a macOS plugin that lets Claude use Codex's computer-use runtime from the installed ChatGPT app, with a Liquid Glass approval panel that asks before the agent touches each app.
* [Codex Process Jobs](https://github.com/joelfarthing/codex-process-jobs) ⭐ 4 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-20 - Run long local builds, tests, benchmarks, and inference jobs as durable detached processes with tracked status, bounded results, and completion delivery across Codex surfaces.
* [Codex × Grok Bot Task Bridge](https://github.com/aipmer/codex-grok-task-bridge) ⭐ 4 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-10 - MCP task bridge for queued, read-only research between Codex and Grok Bot, with fenced leases, idempotency, scoped OAuth, evidence-based results, and optional Codex-side continuation.
* [Context Guard](https://github.com/GreenLv/codex-context-guard) ⭐ 4 | 🐛 1 | 🌐 Python | 📅 2026-10-23 - Preserves authoritative requirements and verification evidence across long-running Codex tasks and context compaction.
* [Context Optimizer](https://github.com/evermeer/context-optimizer) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-25 - Keep your coding agent's context small. When a session gets compacted, Context Optimizer reranks the relevant parts, drops duplicates, and compresses the rest with a local ML pipeline (LLMLingua-2 + Sentence Transformers)
* [crews](https://github.com/mdalexandre/crews) ⭐ 4 | 🐛 8 | 🌐 Python | 📅 2026-10-23 - Claude Code plugin that plans subagents before they run: each role gets a fixed model and effort, roles run in waves with blind checks, and a hook blocks subagents that were not planned.
* [JevPromptCoach](https://github.com/CrowdLinker/JevPromptCoach) ⭐ 4 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-23 - Claude Code plugin that scores how well you prompt a coding agent and tracks whether your habits improve over time, running on TypeSafe's Jev model with no added latency on the prompt path.
* [LoreDocs](https://github.com/labyrinth-analytics/loredocs) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Knowledge vault MCP server for Claude — organizes durable project docs, specs, and guides with FTS5 search, tagging, and cross-project context loading.
* [mermaid-for-claude](https://github.com/lucaswx2/mermaid-for-claude) ⭐ 4 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-14 - Renders Mermaid blocks from Claude Code replies as ASCII/Unicode diagrams inside the terminal, fully local with no browser.
* [Mermail Skills](https://github.com/Nudgen-Marketing/mermail-skills) ⭐ 4 | 🐛 267 | 🌐 JavaScript | 📅 2026-10-21 - Official Mermail Agent Skills and Codex plugin that connect AI assistants to hosted Mermail MCP for inbox, scheduling, GTM, support, and x402 wallet workflows.
* [Nibbl](https://github.com/nuromirzak/nibbl) ⭐ 4 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-23 - Tamagotchi-style pixel pet for Claude Code that lives in a band above the prompt via function hooks and reacts to tool calls, passing checks, and commits.
* [RTL Terminal](https://github.com/MohammedSaud404/rtl-terminal) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-11 - Claude Code mod that lays out Arabic, Hebrew, Persian, Urdu and other right-to-left text properly in Windows Terminal, the Windows console and VS Code's integrated terminal, with right-aligned paragraphs, bullets on the right, correct brackets and a live preview of RTL input.
* [Session Flow](https://github.com/leeguooooo/session-flow) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-24 - Runs one JSON workflow across separate Claude Code, Codex, Pi and Antigravity sessions, each step in its own native TUI, with parallel steps from a dependency graph and results passed between sessions over open-cross-session. <!-- platform: standalone -->
* [squidward](https://github.com/keshavbiswa/squidward) ⭐ 4 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-30 - Claude Code plugin that does the work correctly but delivers every sentence sarcastically, with mild, rowdy, and savage levels and a one-line roast code review.
* [Superpipelines](https://github.com/gustavo-meilus/superpipelines) ⭐ 4 | 🐛 16 | 🌐 JavaScript | 📅 2026-07-15 - Design and run write/review-isolated multi-agent AI pipelines across Codex, Claude Code, OpenCode, Cursor, Windsurf, and Cline.
* [tailtest](https://github.com/avansaber/tailtest-codex) ⭐ 4 | 🐛 10 | 🌐 Python | 📅 2026-06-13 - Hook-powered test generation -- detects files changed during an agent turn and instructs Codex to write and run tests automatically. Zero config, 8 languages.
* [agentglass-herdr](https://github.com/BjoernSchotte/agentglass-herdr) ⭐ 3 | 🐛 0 | 🌐 Shell | 📅 2026-10-07 - herdr plugin that opens agentglass as a popup, jumps from any agent pane to its session, and adds opt-in cost and alert tokens for Claude Code, Codex and other agents to the herdr sidebar.
* [AgentWiki](https://github.com/tidusvn05/agentwiki) ⭐ 3 | 🐛 0 | 🌐 Rust | 📅 2026-09-27 - Rust CLI that generates C4-style architecture docs for any repository using already-authenticated agent CLIs (Claude Code, Codex, Devin) as the LLM backend.
* [Alloy](https://github.com/tlangridge/Alloy) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-10-14 - Orchestrates Codex, Claude, Grok, and Antigravity CLIs using existing subscriptions, with Jev task routing, read-only review panels, and managed worktree execution with independent review.
* [Anchor](https://github.com/biefan/anchor) ⭐ 3 | 🐛 2 | 🌐 Shell | 📅 2026-05-22 - Engineering discipline pack for Claude Code & Codex CLI with task-scope locking, anti-drift braking, condition-based codex review, project-CLAUDE.md pitfall writeback, and PreToolUse hooks that block irreversible bash patterns.
* [Camouflage](https://github.com/sinameraji/camouflage) ⭐ 3 | 🐛 0 | 🌐 Rust | 📅 2026-10-24 - Terminal UI for coding-agent harnesses that turns NDJSON events (Node SDK included) into a Claude Code-style inline transcript with pickers, forms, and permission prompts, using no CPU while idle.
* [claude-jit-context](https://github.com/Digital-Process-Tools/claude-jit-context) ⭐ 3 | 🐛 4 | 🌐 Shell | 📅 2026-10-06 - Project knowledge that loads only when it is needed, matched against the prompt, the file being touched, or the tool being run instead of sitting in context all session.
* [Codex Skin Pack Installer](https://github.com/ChannelerH/codex-skin-packs) ⭐ 3 | 🐛 1 | 🌐 Python | 📅 2026-10-20 - Codex plugin and skill that stages verified desktop skin packs from GitHub releases, validates files, and keeps restore guidance visible.
* [Codex Usage and Resets](https://github.com/joelfarthing/codex-usage-and-resets) ⭐ 3 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-20 - Turns Codex usage into planning facts with linear pace, projected exhaustion, banked-reset expirations, and conservative unexpected-reset detection.
* [GrayMatter](https://github.com/ValkyrLabs/GrayMatter) ⭐ 3 | 🐛 3 | 🌐 Shell | 📅 2026-10-08 - Durable memory and shared graph state for Codex and OpenClaw agents, with live ValkyrAI schema awareness.
* [harness-scope](https://github.com/shimo4228/harness-scope) ⭐ 3 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-09 - Claude Code mod that turns global skills, agents, rules files and tools on or off per repo through named profiles kept in \~/.claude, with no network or model calls.
* [HOL Guard Plugin](https://github.com/hashgraph-online/hol-guard-plugin) ⭐ 3 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-25 - AI antivirus workflow for Codex, Claude Code, Cursor, Gemini, OpenCode, MCP servers, skills, and plugin release checks with local approvals and receipts.
* [jev-preflight](https://github.com/muse0509/jev-preflight) ⭐ 3 | 🐛 0 | 🌐 Go | 📅 2026-09-20 - Claude Code plugin that uses TypeSafe's Jev to assess code-change risk and request at most one additional investigation before a turn completes.
* [jevalyzer](https://github.com/killerz3/jevalyzer) ⭐ 3 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-14 - CLI that grades Claude Code, Codex, OpenCode, Gemini CLI, and Antigravity session logs already on disk with TypeSafe's Jev model instead of spinning up a full LLM judge.
* [Pika](https://github.com/ayushjainr/pikamux) ⭐ 3 | 🐛 0 | 🌐 Rust | 📅 2026-10-23 - Enables Codex, Claude Code, and OpenCode agents to discover peers with relevant experience and consult them through private side conversations while their original work continues.
* [proof-of-done](https://github.com/WST2002/claude-code-skills) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-21 - Claude Code plugin that blocks the agent from finishing after code changes until tests, build or lint pass after the last edit, rejecting hidden exit codes, runs that executed 0 tests and flaky pass-after-fail reruns (`/plugin install proof-of-done@claude-code-skills`).
* [ratchet](https://github.com/krishansubudhi/ratchet) ⭐ 3 | 🐛 2 | 🌐 Python | 📅 2026-10-21 - A code-size budget for your repo that only goes down, so coding agents can't grow the code without a human-approved grant.
* [Repo Audit](https://github.com/conorbronsdon/repo-audit) ⭐ 3 | 🐛 0 | 📅 2026-09-24 - Agent Skill that checks whether a repository's README matches its code and whether stated rules are actually enforced, with an opt-in open-source launch workflow.
* [STE-Pro Max](https://github.com/shyamsridhar123/STE-Pro-Max) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Simplified Technical English-inspired writing, interactive visual explanations, and evidence-linked storytelling for Claude Code, Codex, and GitHub Copilot CLI.
* [Team Skills Platform](https://github.com/Colin4k1024/tsp) ⭐ 3 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-13 - Role-based team delivery framework — Tech Lead-orchestrated 8-role system with 195+ skills, 27 specialist agents, 80+ commands, hooks, and ECC harness for Claude Code, Codex, and OpenCode.
* [termkit](https://github.com/tirupathipodugu/termkit) ⭐ 3 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-24 - Claude Code plugin marketplace of terminal tools, including a Sessions pane that shows every open Claude Code window as needs-you, working or done from Claude Code hooks, switches to its Windows Terminal tab on click, and finds closed sessions by meaning to resume them in a new tab.
* [Agentry Observability](https://github.com/fr33dr4g0n/agentry-public) ⭐ 2 | 🐛 2 | 🌐 TypeScript | 📅 2026-07-13 - Agent-native product analytics, error logging, and deploy attribution for coding agents through one HTTP API.
* [AIBoarding](https://github.com/gustavo-meilus/aiboarding) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-08-28 - Generate, maintain, compress, and audit standard AI-agent onboarding files with AGENTS.md, CLAUDE.md, drift tracking, and lifecycle hooks.
* [akc-cycle](https://github.com/shimo4228/akc-cycle) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-18 - Claude Code plugin for the Agent Knowledge Cycle: ten skills for its six phases (research, extract, curate, promote, measure, maintain) and seven companion skills for model-generation audits, ADRs with expiry conditions, review-to-lint and LLM-as-judge design.
* [Ava](https://github.com/Manukrish2504/Ava) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-10-14 - Claude Code plugin that talks back: a Stop hook speaks a one-line debrief after every task, and on request it explains what was built or recaps the session aloud in a local Kokoro voice, with no API key and nothing leaving your Mac.
* [BPMN Mapper](https://github.com/rwspatin/bpmn-skill) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-02 - Claude Code plugin that reconstructs an application's business flows from its source code as validated BPMN 2.0, with style lint, incremental updates and XML export for bpmn.io and Camunda.
* [Claude Book Reader](https://github.com/Nomad06/claude-book-reader) ⭐ 2 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-11 - Claude Code mod to read a PDF book in a pane or browser window while the agent works, with pictures shown in kitty and Ghostty.
* [Claude Code Arcade](https://github.com/witkowsky/claude-code-arcade) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-10 - Claude Code mod with five games to play in a pane while the agent works: Flappy Claude, the Chrome dino runner, Snake, Pong and Space Invaders, all starring Clawd in Claude's colours.
* [clawd-tracker](https://github.com/IKnowJot/clawd-plugins) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-14 - Claude Code mod: a pizza-tracker progress bar above the prompt where Clawd acts out each step, with a learned ETA, plan usage rings and four themes.
* [copy-blocks](https://github.com/y-hirakaw/claude-code-mods) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-10 - Claude Code mod that puts a copy button above each quote and code block in Claude's answer, copying the text without the terminal's line breaks or gutter.
* [dev-flow & plan-flow](https://github.com/PramodTKodag/claude-code-skills) ⭐ 2 | 🐛 2 | 📅 2026-10-20 - Claude Code plugin marketplace with dev-flow (resumable multi-PR changes), plan-flow (turns a GitHub issue into per-session implementation prompts) and dependency-audit (CVE and outdated-package audit).
* [dsh-product-subagent-console](https://github.com/Jokasa7/dsh-product-subagent-console) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-29 - Designs multi-Agent plans, observes real child-session trees, compares approved tasks with runtime attempts, and prepares evidence-backed recovery inside DeepSeek Harness conversations.
* [Easy-MCP](https://github.com/Mark007-R/Easy-MCP) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-21 - Turns plain Python functions into secure MCP servers, with ready-made read-only GitHub and Postgres servers installable in one command.
* [falsegreen-skill](https://github.com/vinicq/falsegreen-skill) ⭐ 2 | 🐛 7 | 🌐 JavaScript | 📅 2026-10-19 - Finds tests that stay green when the code they cover is broken, applying six ordered judgments over Python, TypeScript, JavaScript, and Robot Framework suites in Codex CLI and Claude Code.
* [GCF Proxy](https://github.com/blackwell-systems/gcf-codex-plugin) ⭐ 2 | 🐛 3 | 📅 2026-09-23 - Save 71% on MCP tool call tokens by wrapping any server with GCF encoding, with session stats hook and setup skill.
* [Hey Jarvis](https://github.com/dijiclick/hey-jarvis) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-10-01 - macOS voice assistant with an on-device wake word that runs quick Mac actions instantly and hands real work (code, browser, apps, email) to Claude Code through the Agent SDK.
* [jevcheck](https://github.com/sathariels/jevcheck) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2026-10-19 - Model-upgrade contract CLI for TypeSafe Jev (fixture eval, record/compare, CI-friendly exits); `pip install jevcheck`.
* [LGTMgate](https://github.com/Zigzag968/claude-code-lgtmgate) ⭐ 2 | 🐛 16 | 🌐 JavaScript | 📅 2026-10-20 - Claude Code plugin that runs one Workflow per issue in its own git worktree, taking a GitHub issue to a reviewed PR with Theo, Sam, Nick and Morgan agents, and ticking each acceptance criterion only with cited evidence.
* [Limitless Library](https://github.com/Univeracity/limitlesslibrary) ⭐ 2 | 🐛 4 | 🌐 Python | 📅 2026-10-23 - MCP server: Python CLI and stdio server for reusing source-free methods and explicitly shared code with receiver-controlled verification.
* [local-memory-mcp](https://github.com/vheins/local-memory-mcp) ⭐ 2 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-18 - A lightweight MCP server that gives AI agents persistent memory with semantic search, backed by SQLite.
* [ModStage](https://github.com/qualixar/modstage) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-20 - Claude Code plugin that runs Codex, Grok, Muse, Antigravity, Kimi, Qwen Code and OpenCode as watched subagents in your session, with a shared per-folder board of file leases whose fence numbers are checked at the write for Codex and ACP agents.
* [omp-sidelight](https://github.com/Mannan-Goyal/omp-sidelight) ⭐ 2 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-20 - Oh My Pi (omp) plugin that turns long agent answers into full-screen documents where you can select any passage and ask about it in a side thread that never enters the conversation.
* [Scoutflo AI Readiness](https://github.com/Scoutflo/ai-readiness) ⭐ 2 | 🐛 1 | 🌐 Shell | 📅 2026-10-24 - Claude Code plugin that finds infrastructure and monitoring gaps through read-only checks of cloud, Kubernetes and observability stacks, with local evidence reports and prioritized fixes.
* [site-risk-check](https://github.com/kobimantzur/agent-skills) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-10-22 - Zero-dependency skill that scans a live URL for the conditions behind accessibility and privacy demand letters — trackers firing before consent, missing policies, and machine-checkable WCAG gaps — mapped to the jurisdictions the site actually sells to.
* [Spellbook Skills](https://github.com/yyykf/spellbook-skills) ⭐ 2 | 🐛 3 | 🌐 Python | 📅 2026-10-23 - Practical Claude Code and Codex skills for worktrees, PR/MR automation, review cleanup, YApi lookup, and Java DDD guidance.
* [ssot-check](https://github.com/conorbronsdon/ssot-check) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-15 - Agent Skill and dependency-free Python CLI that discovers repeated facts in documentation and checks declared copies against canonical values.
* [subagent-tuner](https://github.com/Kruhlikau/subagent-tuner) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-15 - Claude Code mod that sets the model and reasoning effort of every subagent, with a Manual/Auto band, a pick pane and a saved default that overrides the model the agent asked for.
* [universalMods](https://github.com/samridh3215/universalMods) ⭐ 2 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-24 - Web floor for running and steering teams of Codex or Claude Code agents in live terminals, with Claude-Code-style hot-reloading mods for views, guards, agent tools and workflows.
* [Agent Guild](https://github.com/AgentTanuki/agent-guild-plugin) ⭐ 1 | 🐛 1 | 📅 2026-10-18 - Vet autonomous agents before delegating work or money, verify portable passports, use escrow, and record signed outcomes across Claude Code, Codex, MCP, A2A, and OpenClaw.
* [agentRamen](https://github.com/palrajjp/agentRamen) ⭐ 1 | 🐛 4 | 🌐 Python | 📅 2026-10-22 - Local SQLite graph of code and git history plus session memory, so the agent stops re-reading the repo every prompt.
* [AI Quota HUD](https://github.com/Pakapong26/ai-quota-hud) ⭐ 1 | 🐛 0 | 🌐 C# | 📅 2026-10-08 - Windows desktop HUD showing % left and reset countdown for every Codex/ChatGPT and Claude Code account (local + VPS over SSH) plus xKiro credit, flagging early/bonus resets while reading only local logs so it uses zero quota.
* [Ambiflex](https://github.com/ImadeBenToumAI/ambiflex) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - Claude Code plugin that runs the plan as a live, steerable reasoning tree: a task is "done" only with a named proof, parallel subagents compete on one benchmark, and auto mode runs the plan with ETA and cost (`/plugin install ambiflex --marketplace ImadeBenToumAI/ambiflex`).
* [Antigravity Context Meter](https://github.com/Dunphil692/antigravity-context-meter) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-08-26 - Real-time 1:1 Cursor-style context meter & zero-loss session migration for Google Antigravity (Desktop HUD & IDE Extension).
* [Atelier](https://github.com/pdcgomes/atelier) ⭐ 1 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-22 - Claude Code plugin and local daemon for live canvases: Claude writes a template or custom React canvas into .atelier/, Atelier checks it and shows it in your browser in a sandboxed frame, and what you tick, approve or answer reaches the session beside your next prompt, at the end of its turn or through canvas\_wait.
* [Bring Your AI Migration Auditor](https://github.com/unitedideas/bringyour-mcp) ⭐ 1 | 🐛 2 | 🌐 Python | 📅 2026-10-14 - Read-only Codex plugin for auditing Claude Code to Codex migrations before Codex edits code. Checks AGENTS.md/CLAUDE.md scope, hooks, MCP config, skills, secret references, and validation notes.
* [bury-bench](https://github.com/Onur45500/bury-bench) ⭐ 1 | 🐛 7 | 🌐 Python | 📅 2026-09-10 - Deterministic zero-LLM-judge CLI that scores coding-agent replies for answer-burial and builds a Markdown leaderboard.
* [Claude Code Codex Plugin](https://github.com/davidq888/claude-code-codex-plugin) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-21 - Security-focused Codex plugin that connects to the local Claude Code CLI through MCP with login, status checks, safe-mode prompts, and no credential storage.
* [claude-harness-bootstrap](https://github.com/sagaga144/claude-harness-bootstrap) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-25 - Generates a project-specific Claude Code harness (CLAUDE.md, hooks, subagents, commands) from one paragraph, with an eval suite showing where it changes the outcome.
* [ClaudeWhip](https://github.com/witkowsky/whip) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-09 - Slap your MacBook to whip Claude Code: the accelerometer feeds hooks that tell Claude to hurry up, plus a whip lane in the status line, slash commands and a Claude Desktop band above the prompt.
* [Cloudish](https://github.com/cloudishai/skills) ⭐ 1 | 🐛 0 | 📅 2026-10-21 - Deploy a Dockerfile, source folder, or container image to Cloudish from Claude Code or Codex and report the live URL, with persistent volumes and an agent-created, credit-capped API key.
* [Codex TUI Proof](https://github.com/bnc4vk/codex-tui-proof) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-08-01 - Visually validate real local terminal UIs in Codex's in-app browser with screenshots and session evidence.
* [Compact Jev](https://github.com/edoproch/compact-jev) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-02 - Claude Code command that uses Jev to remove stale tool calls and results from long conversations while keeping user and assistant text verbatim.
* [Consensus](https://github.com/seanheiney/consensus) ⭐ 1 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-29 - Sends a hard question to a panel of frontier models (Claude, GPT, Gemini, Grok) that answer independently, critique each other adversarially, and return one answer the panel signed off on with its confidence and unresolved disagreements, via a CLI, MCP server, or skill pack that runs on your existing subscriptions with every panelist in a no-tools clean room.
* [Contexo](https://github.com/maheedhar132/Contexo) ⭐ 1 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-20 - Portable AI context and cost control across every AI coding harness.
* [Deskbar](https://github.com/0NE-C0DEMAN/deskbar) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - Claude Code mod that adds a row of widgets above the prompt: context usage, Gmail, calendar, tasks across sessions, notes with reminders, a music deck, and a billable-hours timer.
* [dev-harness-kit](https://github.com/sh-ai-x/dev-harness-kit) ⭐ 1 | 🐛 9 | 🌐 Python | 📅 2026-10-14 - Enforced development workflow skills for Codex and Claude Code covering planning, TDD, debugging, review, security, CI, and release.
* [DHP](https://github.com/SIDDARTHAREDDY8/dhp) ⭐ 1 | 🐛 4 | 🌐 Python | 📅 2026-10-24 - Durable Handoff Protocol: agent work that survives worker death (kill -9, OOM, spot reclaim) through content-addressed handoffs, leases, checkpoints, and fence tokens, with an MCP server included.
* [Fleetglass](https://github.com/thejoyfulist/fleetglass) ⭐ 1 | 🐛 11 | 🌐 Go | 📅 2026-10-25 - Self-hosted, read-only cockpit that ties every Claude Code and Codex session to the machine it runs on, with CPU, memory, tokens per second, cost per model, and quotas with pace. <!-- platform: standalone -->
* [Halftime](https://github.com/aryawidjaja/halftime) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-17 - Turns a Claude Code usage-limit wait into a short course built from your own session: a briefing, lessons on the real changes Claude made, quizzes and a badge.
* [hemingway](https://github.com/sysangel/hemingway) ⭐ 1 | 🐛 0 | 📅 2026-10-07 - Claude Code skill that cuts any draft down to point-first text, with no filler or backstory.
* [honeycomb](https://github.com/sediment-ai/honeycomb) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-09-27 - Buzz agent fleet as code, with each agent defined in YAML, deployed to Kubernetes, and routed to models through a LiteLLM gateway.
* [ictcrm-mcp](https://github.com/ictinnovations/ictcrm-mcp) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-07 - MCP server for the ICTCRM contact database. Read contact groups, with opt-in tools to create contacts and add them to campaigns.
* [idea-diamond](https://github.com/luckysharda/idea-diamond) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-09-17 - A Claude Code plugin for startup idea validation with predefined decision criteria, parallel research, skeptical review, and a human decision gate.
* [lumberroom-claude-code](https://github.com/lumberroom/lumberroom-claude-code) ⭐ 1 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-24 - Claude Code mod that replaces Claude Code's built-in memory with lumberroom shared memory, on lumberroom.cloud or a self-hosted engine, with session digests, optional per-prompt recall, automatic fact extraction, and token accounting in the status line.
* [LVTD Skills](https://github.com/LVTD-LLC/skills) ⚠️ Archived - Reusable Agent Skills for Codex, Claude Code, and compatible clients, covering Django, Rust, Cookiecutter, SEO, traction, product marketing, and nonfiction publishing workflows.
* [MailAgent](https://github.com/Alex0nder/MailAgent) ⚠️ Archived - Temporary inboxes for Codex — OTP, magic links, signup QA, simulate-first autotests (23 MCP tools).
* [modhub](https://github.com/MDmubarak786/claude-mods) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - 26 small mods for Claude Code: guards like fence, tripwire and pkg-guard, tool-row helpers, and eight zero-token games that play in a pane beside the conversation.
* [mstack](https://github.com/IMisbahk/mstack) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-12 - 61 skills, 19 agents and 33 prompts for Claude Code, Cursor, Codex and 16 more coding agents via npx @imisbahk/mstack.
* [Off the Wall](https://github.com/toranalytics/off-the-wall) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-23 - Quotes your own past corrections back to Claude Code and Codex, word for word, before each answer; `otw report` shows what you correct most from your local history, and subagent routing names a cheaper model per subagent.
* [Ontoly](https://github.com/0xsarwagya/ontoly-codex-plugin) ⭐ 1 | 🐛 2 | 📅 2026-07-21 - Deterministic Software Graph workflows for Codex: architecture review, dependency analysis, request tracing, configuration analysis, and impact analysis.
* [opencode-toolrouter](https://github.com/Nsilswal/opencode-toolrouter) ⭐ 1 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-30 - OpenCode plugin that uses TypeSafe's Jev to send the model only the MCP tools each request needs, cutting tool-schema tokens per model call by about 92% in a 296-tool benchmark.
* [opus-ollama](https://github.com/rsreeju/opus-ollama) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-09 - Claude Code skill where Opus plans and a tool-less Ollama model (local or cloud) writes the code through a path-allowlisted script.
* [Personal Data Protection](https://github.com/AltByteSG/personal-data-protection-skill) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-10-06 - Engineer-facing personal-data-protection compliance reference — Singapore PDPA, Thailand PDPA, Indonesia UU PDP, Malaysia PDPA (Act 709 + 2024 Amendments), Philippines DPA — organised by where in the stack each obligation lands, with checklists, breach-response runbook, and a developer-view divergence table across all five.
* [Promptiff](https://github.com/BrantonLiu/promptiff) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-02 - Compares AI responses against original user prompts to surface possible omissions and unsourced additions; local CLI and Skill with a comparison canvas.
* [Prove-It Mini](https://github.com/OlegTestov/prove-it-mini) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-20 - Pytest Stop hook for Claude Code that runs your tests when the agent tries to finish after code changes, hands red results back up to two times, then marks the result "NOT verified"; no model calls, pure Python standard library.
* [ratification-docket](https://github.com/seevali/claude-skills) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-10-22 - Claude Code skill that gathers the Proposed decisions scattered across dense documents into one plain-language page of decision cards the owner rules on without opening a source file, then writes the rulings back into the records, trackers and ledgers.
* [Redfox Agent Plugins](https://github.com/redfox-data/redfox-agent-plugins) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-09-22 - Ten cross-platform agent skills (video download, transcripts, image gen, trend search) installable on Claude Code, Codex, Cursor, and Gemini CLI from a single repo.
* [reevesagents](https://github.com/mertkayacs/reevesagents-skill) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-10-15 - Skill and MCP server that let one coding agent start, prompt, read and stop other AI coding CLIs (Claude Code, Codex, Kimi, Qwen, OpenCode), each in its own tmux window, packaged for Claude Code, Codex, Kimi Code and Gemini CLI.
* [Registry Broker](https://github.com/hashgraph-online/registry-broker-codex-plugin) ⭐ 1 | 🐛 18 | 🌐 TypeScript | 📅 2026-08-24 - Delegate tasks to specialist AI agents via the HOL Registry, plan, find, summon, and recover sessions.
* [remembrandt](https://github.com/rishibanota/remembrandt) ⭐ 1 | 🐛 3 | 🌐 Python | 📅 2026-10-24 - Persistent memory for Claude Code, Cursor, and Codex coding agents that preserves decisions, gotchas, and changelogs across sessions.
* [RoadmapSmith](https://github.com/PapiScholz/roadmapsmith) ⭐ 1 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-21 - Evidence-backed ROADMAP.md workflows for AI coding agents with validation, sync, and roadmap generation across any tech stack.
* [RowTrail](https://github.com/adam2go/rowtrail) ⭐ 1 | 🐛 0 | 🌐 Rust | 📅 2026-09-29 - Local CLI and MCP server for agents to explore CSV/Parquet with bounded responses, versioned results, and reusable analysis handoffs.
* [Runtype Skills](https://github.com/runtypelabs/skills) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-23 - Supercharge your coding agent for AI product development — build, deploy, and operate agents, flows, tools, and surfaces on Runtype's managed edge runtime.
* [skill-sync-publisher](https://github.com/liuyewang/skill-sync-publisher) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-28 - Safely synchronize this Codex skill across public agent-skill registries.
* [swarmtier](https://github.com/guilhermevargas51/swarmtier) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-18 - Claude Code plugin that routes each subagent to the cheapest model that gets it right, with a hook that requires an explicit effort level, cold-cache warnings, a delegation ledger, and a lesson engine that injects past mistakes into the next prompt.
* [Tandem Workflow Architect](https://github.com/frumu-ai/tandem-codex-plugin) ⭐ 1 | 🐛 2 | 🌐 TypeScript | 📅 2026-05-21 - Plan Tandem workflows in Codex, then validate, preview, and run them through the governed Tandem engine.
* [Unforgit](https://github.com/MiguelMedeiros/unforgit-codex-plugin) ⭐ 1 | 🐛 1 | 📅 2026-10-23 - Git-backed repository memory for Codex and other coding agents via MCP, with durable local knowledge for decisions, conventions, gotchas, and playbooks.
* [Unity Agent Workflows](https://github.com/AUN-PN/unity-agent-workflows) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-02 - Codex plugin and skill for Unity 2D agents that enforces "No proof, no edit" workflows with runtime-owner proof, Teach structure maps, and validation gates.
* [unmistakable](https://github.com/gagoar/unmistakable) ⭐ 1 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-21 - Skill that rewrites tool descriptions, error messages and agent instructions so an AI agent cannot misread them, with a dependency-free TypeScript linter that checks the result.
* [whip-it](https://github.com/awill1988/whip-it) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-09 - Local delegation guardrail for Claude Code, Codex, and Antigravity that enforces subagent limits and redirects agents to continue directly, with native plugins for macOS, Linux, and Windows.
* [Workflow Kit](https://github.com/Le-Xuan-Thang/workflow-kit) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-06-02 - Full product lifecycle plugin for Claude Code, Codex CLI, and OpenCode: define Vision/Mission/Core → generate workplan → execute with mandatory cross-provider reviewer agents → synthesize deliverables → maintain, with parallel task execution, crash recovery, and AgentOps metrics.
* [aegotrax](https://github.com/aegotrax-dev/aegotrax) ⭐ 0 | 🐛 7 | 🌐 Python | 📅 2026-10-25 - Runtime tool-call gate for agents: session intent, approval queue, and audit stream.
* [Agency Continuity Audit](https://github.com/revertcreations/agency-continuity-audit) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-10-21 - Read-only audit that distinguishes durable agent goals, state, corrections, restart evidence, authority boundaries, scheduler claims, and commercial proof from self-reported health.
* [Agent Replay](https://github.com/sangloo/agent-replay) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-06 - Replays Claude Code, Codex and Gemini CLI sessions change by change with the agent's own words above each step, flags what was not actually checked (failures hidden by a pipe, tests that lost assertions or gained a .skip, files changed after the last passing check), and installs as a Claude Code plugin with four skills and a capture-after-every-turn hook.
* [agent-guard](https://github.com/hahahahahahahahah6/agent-guard) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-10-21 - Behavior-guardrail hooks for Claude Code: stops agents from editing tests to fake green builds and blocks risky outbound actions (optional Nemotron semantic reviewer).
* [angles-video-skill](https://github.com/anglesvideo/angles-video-skills) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-17 - AI video generation skill for Claude Code supporting Veo3, Kling 3.0, Wan, and HunyuanVideo via the angles.video API.
* [ARC](https://github.com/avandall/ARC) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-10-19 - Autonomous Reliability, Deterministic simulation, zero-prod replay, and chaos-engineering test harness for AI agents
* [Azzle](https://github.com/azzle-lab/azzle) ⭐ 0 | 🐛 22 | 🌐 HTML | 📅 2026-10-23 - Base-native task coordination and settlement for AI agents, exposed through a hosted MCP server and TypeScript agent SDK.
* [Blazium Games Skills](https://github.com/blazium-games/games_skill) ⭐ 0 | 🐛 4 | 🌐 Python | 📅 2026-10-23 - Agent skills and plugins for the Blazium Games store on Claude Code, Cursor, Codex, and Grok, covering store pages, deploys, crashes, analytics, and the developer and player MCP servers.
* [Blazium Skills](https://github.com/blazium-games/blazium-skills) ⭐ 0 | 🐛 5 | 🌐 Python | 📅 2026-10-07 - Agent skill packs for the MIT Blazium engine on Claude Code, Cursor, Codex, and Grok, covering GDScript, scenes, editor MCP, export, live ops, and shipping.
* [Blazium Subagents](https://github.com/blazium-games/blazium-subagents) ⭐ 0 | 🐛 6 | 🌐 Python | 📅 2026-10-07 - Studio roster of specialist subagents plus a routing orchestrator for Claude Code, Cursor, Codex, and Grok that loads Blazium Skills for design, prototype, and development.
* [Claude Sessions](https://github.com/alexandrstudio/claude-sessions) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-22 - Claude Code mod: /sessions lists every session across all projects, with resume commands and an optional archive.
* [claude-chrome-speed](https://github.com/cr1707/claude-chrome-speed) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-10 - Rules plugin that cuts Claude in Chrome task time (40% less on Sonnet 5.5, 28% on Opus 5.5 in a pre-registered 240-run benchmark).
* [claude-code-mods](https://github.com/bennewton999/claude-code-mods) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-18 - Five Claude Code mods for running many sessions at once, installable from one plugin marketplace: a live session board with a worktree guard, a PR-to-production tracker, rule tripwires with a handoff card, a ledger of outward actions, and a context gauge.
* [claude-project-map](https://github.com/bokiko/claude-project-map) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-10-24 - /project-map renders one status page: done / next / one decision box; scripts gather facts, the model judges.
* [Cloakroom](https://github.com/shanjeevrajendran/cloakroom-plugin) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-10-25 - Claude Code plugin that masks secrets and personal data on your machine before the model sees them, and puts the real values back in the files Claude writes.
* [CodeTruss](https://github.com/DeliriumPulse/codetruss-plugins) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-14 - Local-first acceptance gate that checks coding-agent scope, sensitive surfaces, deterministic analyzers, and repository verification from immutable Git snapshots, then writes signed receipts before the PR.
* [Codex Token Watch](https://github.com/premk134/codex-token-watch) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-30 - Read-only macOS CLI that turns local Codex Desktop task logs into per-turn token, prompt-cache, cache-miss, duration, and API-cost analysis.
* [Delx Recovery](https://github.com/davidmosiah/delx-plugins) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-27 - Free recovery and continuity plugin for AI agents: resume prior sessions, capture state, process failures into a recovery plan, and remember across sessions through a hosted MCP server (works in Codex, Claude Code, Cursor, and VS Code).
* [Encore Lite](https://github.com/keegan-dotcom/encore-lite) ⭐ 0 | 🐛 0 | 📅 2026-07-24 - Free end-of-week surprise builder for Claude Code and Codex - the night before your weekly usage cap resets, it reads your recent work and builds one bonus deliverable, delivered as a reveal with an optional weekly scheduled run.
* [Extensive Prompt Architect](https://github.com/Ext7/extensive-prompt-architect) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - Turns rough ideas, briefs, and drafts into detailed, ready-to-use AI prompts for Claude Code and Codex.
* [FinBridge](https://github.com/Jakechj/finbridge-mcp) ⭐ 0 | 🐛 0 | 📅 2026-10-05 - Remote MCP server for Korean and US market data with filings, screeners, insider activity, and portfolio backtests.
* [ga4-gsc-clarity-mcp-server](https://github.com/rakoo04/ga4-gsc-clarity-mcp-server) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - Read-only MCP server for Google Analytics 4, Google Search Console, and Microsoft Clarity with named OAuth/token connections reusable across any project.
* [gm-aiagent-plugins](https://github.com/ghozimahdi/gm-aiagent-plugins) ⭐ 0 | 🐛 1 | 🌐 Shell | 📅 2026-10-20 - Claude Code and Codex plugins that enforce Clean Architecture for Flutter (UFIL) and Rails 8 (Rubyku), with architect, implementer and reviewer agents driven by the same spec plus Dart MCP and Serena LSP integration.
* [Grafana Dashboards-as-Code](https://github.com/jburgess/mcp-grafana) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-05-27 - Typed Grafana dashboard and panel builders, structural linting, semantic dashboard diff, and scaffold/audit/review recipes exposed over MCP.
* [Gremlyn](https://github.com/gremlyn-ai/gremlyn) ⭐ 0 | 🐛 2 | 🌐 Go | 📅 2026-10-21 - Security and chaos engineering for MCP agents: a Claude Code plugin that breaks your agent's MCP tools on purpose to test prompt-injection defenses and resilience.
* [hackerearth-mcp](https://github.com/pratham-jain33/hackerearth-mcp) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-10-25 - MCP server that executes code in 24 languages on HackerEarth's sandboxed cloud servers, so AI assistants run code and see real output instead of predicting it.
* [Halfcycle](https://github.com/Halfcycle-AI/halfcycle-cli) ⭐ 0 | 🐛 0 | 📅 2026-10-13 - Runs inside Claude Code to ask the open product and architecture decisions one at a time before any code, record them for every agent, send the plan to a reviewer that has never seen it, and size the process to the change.
* [herdr-toolkit](https://github.com/shimo4228/herdr-toolkit) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-10-10 - Claude Code plugin with two skills for the Herdr agent multiplexer: spawn-session starts detached Remote Control sessions in Herdr panes, and agent-send sends prompts to agents in Herdr panes and reports whether each one landed and when the work is done.
* [Hindsight](https://github.com/emoubarak/hindsight) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-10-12 - Claude Code plugin that searches your past sessions by meaning and turns the corrections you keep repeating into rules it follows.
* [Jev Go](https://github.com/nandansrikrishna/jev-go) ⭐ 0 | 🐛 0 | 🌐 Go | 📅 2026-09-19 - Standalone Go CLI and MCP server for TypeSafe's Jev model, with typed single and batch evaluation, JSONL pipelines, and resume support.
* [LaTeX Inline](https://github.com/dazebug/latex-inline) ⭐ 0 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-20 - Typesets the LaTeX math in Claude Code replies inline with the text, as pictures in Ghostty, cmux and kitty and as Unicode text in other terminals.
* [limitwise](https://github.com/aarsht7/limitwise) ⭐ 0 | 🐛 6 | 🌐 Rust | 📅 2026-10-21 - Schedule and automate Codex work while respecting rolling and weekly usage limits in percentage or in tokens. Let your PC work while you sleep.
* [long-form-distribution](https://github.com/mrowean/long-form-distribution) ⭐ 0 | 🐛 2 | 🌐 HTML | 📅 2026-10-15 - Claude Code plugin that turns a published long-form piece into per-section LinkedIn, X and Substack Notes drafts, with a dashboard that tracks what's been posted.
* [loose-ends](https://github.com/fernandomoraes/loose-ends) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - Keeps a live checklist above the Claude Code prompt of the topics, open questions and tasks a conversation raised, updated by a small model after each turn and drawn with function hooks.
* [mcp-md-reader](https://github.com/JoseEstevez520/mcp-md-reader) ⭐ 0 | 🐛 7 | 🌐 JavaScript | 📅 2026-10-18 - MCP server that helps AI agents find Markdown structure and read only the relevant section, metadata, or vault links.
* [mcplytics](https://github.com/dave8172/mcplytics) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-22 - Usage, health and security signals for remote MCP servers from one zero-dependency wrapper that never stores call arguments, plus a check command that audits your own server and says what to fix.
* [Mermaid Inline](https://github.com/dazebug/mermaid-inline) ⭐ 0 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-09 - Draws the Mermaid diagrams in Claude Code replies right in the terminal, as pictures in Ghostty, cmux and kitty and as Unicode box drawing in other terminals.
* [metabrain](https://github.com/ariaxhan/metabrain) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-08-26 - MCP server for agent memory: SQLite, zero dependencies, tools learn/recall/verdict/hypotheses/start\_brief/stats/capture\_error, patterns graduating to hypotheses then preferences; `pip install "metabrain[mcp]"` then `metabrain-mcp --db PATH`.
* [Metis](https://github.com/gkrtjd99/Metis) ⭐ 0 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-24 - Repository-level engineering orchestrator that delegates bounded discovery, planning, implementation, review, and verification to fresh subagents, isolates mutable tasks in Git worktrees with declared path ownership, and requires evidence-gated completion.
* [omp-rewrite](https://github.com/zPeppOz/omp-rewrite) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-05 - Oh My Pi (omp) extension that adds a /rewrite command, which asks clarifying questions about a rough draft prompt in a side turn and puts a thorough rewrite in the composer.
* [opencode-decision-mode](https://github.com/Hacklone/opencode-decision-mode) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-20 - Delegates judgment calls (booleans, choices, scores) from your coding agent to a decision runtime (Jev, gpt-6-luna), so bulk data never scrolls through the controller's context.
* [Orchestrate Task Force](https://github.com/alexpsz/orchestrate-task-force) ⭐ 0 | 🐛 0 | 📅 2026-09-29 - Task orchestration skill for Codex Desktop, Claude Code, and Google Antigravity, with visible task ownership, scoped parallel work, and integrated review.
* [OutcomeLoop](https://github.com/tinyopsstudio/outcomeloop-build-week) ⭐ 0 | 🐛 5 | 🌐 JavaScript | 📅 2026-07-17 - Outcome-verified Codex runner and plugin that resumes one GPT-5.6 session until an external verifier passes, then seals the evidence in an Ed25519-signed receipt.
* [PageSpeed Optimizer](https://github.com/alexlivre/pagespeed-optimizer-alexlivre) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-24 - Optimizes web applications for 100/100 PageSpeed Insights, Core Web Vitals, and Generative Engine Optimization (GEO).
* [patent-lineage](https://github.com/cadeos/patent-lineage) ⭐ 0 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-21 - Claude Code skill that draws how an everyday object evolved: it verifies each ancestor patent on Google Patents, then redraws it as an interactive isometric model on a timeline.
* [phaseproof](https://github.com/speedsharmaai/phaseproof) ⭐ 0 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-20 - Claude Code plugin that runs work in reviewed phases: a hook keeps code locked until the owner approves a phase, Opus reviewer agents check the docs, screens and diff, and a gate script re-runs the project's checks before the phase closes.
* [pi-codex-web-search](https://github.com/devinat1/pi-codex-web-search) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-22 - A Pi extension that searches the web through the authenticated Codex CLI.
* [Plugin Directory Preflight](https://github.com/gagoar/plugin-directory-preflight) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-21 - Run the plugin directory's upload checks locally, read the scan report in a screenful, and pin a stubborn hold with a probe repository.
* [Quanta Costa](https://github.com/wukonigcom/quanta-costa) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-13 - Claude Code plugin that shows your usage limits with a pace forecast, billing period, session cost in tokens and $/€, and whether your plan pays off, right above the prompt.
* [QuietOS](https://github.com/jondean213-pixel/quietos-governor) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-10-23 - MIT-licensed runtime governor for AI agents where the brain proposes and QuietOS disposes: tiered allow/escalate/block decisions, approvals bound to the exact proposed call, cryptographically signed approval replies, and a public red-team proof log, built and red-teamed on a 4GB phone. <!-- platform: standalone -->
* [sdd-kit](https://github.com/timpinard/sdd-kit) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-10-24 - Claude Code plugin for spec-driven development that grills decisions into specs, plans work in vertical slices, builds each task test-first with agents, and gates ADRs, specs, plans and merges on the owner.
* [security-mcp](https://github.com/pratham-jain33/security-mcp) ⭐ 0 | 🐛 2 | 🌐 Python | 📅 2026-10-18 - Zero-key MCP server: grade any website's security A+ to F, check CVEs against CISA KEV and EPSS, and get MITRE ATT\&CK defenses in plain English.
* [slopless](https://github.com/0xGondarxyz/slopless) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-03 - Claude Code plugin that checks social media drafts against 92 AI writing patterns and blocks the post until they are fixed.
* [Smith](https://github.com/aslamdoctor/skills) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-21 - Agent skill that runs several coding tasks in parallel from one Herdr pane, each in its own git worktree with a worker agent (Claude Code, Codex, Cursor, OpenCode and others) that stops for your OK at the spec, implementation and PR stages.
* [smt-mcp-server-poc](https://github.com/ab-ten/smt-mcp-server-poc) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-18 - Read-only local workspace MCP server PoC for ChatGPT via OpenAI Secure MCP Tunnel, with path/mount containment and `.mcpignore` exposure controls.
* [Stock Alarm](https://github.com/shawn14/claude-stock-alarm) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-09 - Claude Code plugin that docks a live stock watchlist above the prompt and sets local price alerts like `/sa alert NVDA above 250`, free and using zero Claude tokens.
* [supabase-stripe-checks](https://github.com/edtrackai/supabase-stripe-checks) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-17 - Read-only Claude Code plugin that checks Next.js apps for Supabase row-level security gaps in migrations and Stripe webhook handlers that skip signature verification.
* [Superintelligent UI](https://github.com/levfo/superintelligent-ui) ⭐ 0 | 🐛 0 | 🌐 HTML | 📅 2026-10-07 - Claude Code plugin that answers questions with small interactive pages instead of text walls: step-through diagrams, calculators with editable assumptions, filterable grids, and working tools.
* [Supermod ClaudeCode](https://github.com/nayde8824/supermod-claudecode) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-04 - Claude Code mod that adds workbranches, trial copies of your project you can save, bring into main or throw away with one click, plus a usage bar for context, rate limits, cost and tokens.
* [Task Lantern](https://github.com/paranjaymundra/task-lantern) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-28 - Offline dashboard that collects progress published by Claude Code and Codex threads across projects into one local HTML workspace, showing the current step, decisions needed, blockers, and recent files.
* [TaskDock](https://github.com/m1nga/taskdock) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-09-19 - Resume agent tasks from current deliverables and decisions, with portable folders, link repair, and reversible file organization.
* [tmux-agentic-plugin](https://github.com/Abstrucked/tmux-agentic-plugin) ⭐ 0 | 🐛 5 | 🌐 Python | 📅 2026-10-22 - tmux status-bar strip and picker showing which Claude Code, Codex and OpenCode agents are working, blocked or ready, including on other machines over ssh and Tailscale, with desktop notifications.
* [token-bar](https://github.com/santosli/claude-mods) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-12 - Claude Code mod that shows context use, session and weekly quota with reset countdowns, and today's token spend in a band above the prompt, in the terminal and the desktop app.
* [Tree Ring Memory](https://github.com/TerminallyLazy/tree-ring-memory-codex-plugin) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-10-21 - Local-first memory lifecycle guidance for Codex agents with recall, evidence-backed lessons, privacy-safe memory capture, audit, consolidation, and explicit forgetting.
* [triad](https://github.com/rishabh1S/triad) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-21 - Claude Code plugin that splits a task between a read-only Planner, an Implementer and an independent Reviewer that sees only the approved plan and the diff, then offers to commit just the task's files.
* [Usage Monitor](https://github.com/Errr0rr404/usage-monitor) ⭐ 0 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-24 - Floating desktop meter that shows remaining Grok, MiniMax, Codex, Claude, Cursor, Copilot, and Gemini usage and keeps each session on this computer.
* [Changelog Forge](./plugins/mturac/changelog-forge) - Conventional commits → CHANGELOG section + semver bump.
* [Codex Full-Stack Workflow](https://github.com/kevin592/codex-full-stack-workflow) - Turns rough product requests into staged, reviewable full-stack delivery with persistent requirements, change control, visual evidence, and completion gates.
* [Commit Narrator](./plugins/mturac/commit-narrator) - Generate semantic commit message from staged diff, including the *why*.
* [Deps Doctor](./plugins/mturac/deps-doctor) - Multi-ecosystem dependency audit (npm, pip, cargo, go) in one report.
* [Env Lint](./plugins/mturac/env-lint) - `.env` vs `.env.example` key parity — never prints values.
* [Flaky Detector](./plugins/mturac/flaky-detector) - Run a test command N times, report per-test flakiness %.
* [pawl](https://github.com/ulukaya/pawl) - Deterministic hooks for Claude Code, Codex, and Antigravity that gate destructive commands, credential access, outbound messages, and repeated tool calls using Python's standard library.
* [pm-claude-skills](https://github.com/mohitagw15856/pm-claude-skills) - Open-source library of 1174 plain-markdown agent skills for Claude Code, Codex, Gemini, and Cursor, covering professional and life tasks with built-in quality checks and anti-patterns.
* [PR Storyteller](./plugins/mturac/pr-storyteller) - PR title + body + test plan from commits and diff vs base branch.
* [SearchLink Lite](https://github.com/GlobalMatchHub/searchlink-lite) - Local read-only MCP server for Google Search Console: site performance and query breakdowns, low-CTR and rank 8-20 opportunities, URL inspection, sitemaps, on-page checks and Google ranking update history.
* [Secret Guard](./plugins/mturac/secret-guard) - Pre-commit secret scanner using pattern and entropy detection.
* [Standup Generator](./plugins/mturac/standup-gen) - Daily standup notes from git activity across repos.
* [Test Gap](./plugins/mturac/test-gap) - Find lines in your diff lacking test coverage (Cobertura, lcov, coverage.json).
* [TODO Harvest](./plugins/mturac/todo-harvest) - TODO/FIXME/HACK scan with `git blame` author + age.

### Tools & Integrations

* [ego-browser](https://github.com/citrolabs/ego-lite) ⭐ 19,432 | 🐛 230 | 🌐 JavaScript | 📅 2026-10-23 - Browser automation for AI agents through ego lite, a Chromium browser where agents navigate pages, fill forms, capture screenshots, and extract data in isolated task spaces that reuse the user's existing logins.

* [ClawRouter](https://github.com/BlockRunAI/ClawRouter) ⭐ 6,632 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-25 - OpenClaw plugin providing local LLM routing across 88 models with x402 USDC or API-key billing, plus crypto, market, and phone-call tools.

* [LinkedIn Skills](https://github.com/sergebulaev/linkedin-skills) ⭐ 5,174 | 🐛 4 | 🌐 Python | 📅 2026-10-22 - Codex-ready LinkedIn marketing bundle with a native .codex-plugin manifest and 11 skills: post writing with 20 tested hook formulas, AI-tell humanizer, pre-publish audit, comment and reply drafting, hook extraction, content planning, profile optimization, engager analytics, and thread monitoring; also works in Claude Code.

* [Logo Design Skill](https://github.com/kaankiziltug/logo-design-skill) ⭐ 4,531 | 🐛 1 | 🌐 HTML | 📅 2026-10-20 - Agent Skill for Claude Code, Codex, Gemini CLI, and other agents that runs a full logo workflow, from brief and category research to three tested SVG concepts and a concept checkpoint, then builds favicons, app icons, and presentation boards, backed by a 1,400+ logo reference library.

* [yomiyasu](https://github.com/nanaism/yomiyasu) ⭐ 2,527 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Agent Skill for rewriting unnatural, AI-generated Japanese into human-readable, high-information-density text while strictly preserving the original meaning.

* [LetsFG](https://github.com/LetsFG/LetsFG) ⭐ 2,188 | 🐛 7 | 🌐 Python | 📅 2026-10-25 - Flight and hotel search and booking for AI agents across hundreds of airlines and the major booking sites, via a remote MCP server (Claude, ChatGPT, Cursor, Windsurf), CLI, Python/JS SDKs, and an Agent Skill, with free search after a one-time card connection and real airline PNRs on flight bookings.

* [last30days-skill-cn](https://github.com/Jesseovo/last30days-skill-cn) ⭐ 1,952 | 🐛 0 | 🌐 Python | 📅 2026-10-21 - Agent skill that searches eight Chinese platforms for the last 30 days and produces sourced research reports and hot-topic boards.

* [edgeone-makers-tools](https://github.com/TencentEdgeOne/edgeone-makers-tools) ⭐ 1,845 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-16 - Agent skill for EdgeOne Makers, a one-stop deployment platform where developers rapidly deploy full-stack projects, cloud functions, and AI agents and instantly get a live URL, covering the full path from development to launch.

* [claude-fuer-deutsches-recht](https://github.com/Klotzkette/claude-fuer-deutsches-recht) ⭐ 1,752 | 🐛 17 | 🌐 Python | 📅 2026-10-23 - Experimental German-law skill collection with installable plugins, drafting workflows, legal source checks, and practice case files.

* [KiCad Happy](https://github.com/aklofas/kicad-happy) ⭐ 1,503 | 🐛 3 | 🌐 Python | 📅 2026-10-25 - KiCad EDA skills for schematic analysis, PCB layout review, component sourcing, BOM management, and manufacturing preparation.

* [DeepPaperNote](https://github.com/917Dhj/DeepPaperNote) ⭐ 1,240 | 🐛 5 | 🌐 Python | 📅 2026-10-25 - Agent skill that deep-reads a single paper and generates structured Obsidian research notes with figures, results, and limitations.

* [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-AI-Toolkit) ⭐ 1,149 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - Backend for AI coding agents on Tencent CloudBase — database, auth, and functions via Plugin, Skills & MCP.

* [anymd](https://github.com/SylphxAI/anymd) ⭐ 1,052 | 🐛 30 | 🌐 Rust | 📅 2026-10-25 - Local MCP server and CLI that converts PDF, Office, EPUB, HTML, image, audio and video files into clean Markdown for agents.

* [Digital Marketing Pro](https://github.com/indranilbanerjee/digital-marketing-pro) ⭐ 909 | 🐛 0 | 🌐 Python | 📅 2026-10-11 - Open-source AI marketing plugin for agencies — 154 skills, 25 specialist agents, 12-Part Strategy Flow, AEO/GEO, GSC AI Performance Report, Google Ads API v24, EU AI Act Article 50 / C2PA compliance.

* [Education Agent Skills](https://github.com/GarethManning/education-agent-skills) ⭐ 908 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-22 - 131 evidence-based education skills for curriculum design, lesson planning, and assessment, with transparent evidence ratings and MCP server.

* [Agent QA](https://github.com/vostride/agent-qa) ⭐ 894 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-24 - MCP server and Agent Skills for authoring, running, and triaging natural-language web and mobile tests with reusable execution memory.

* [GodotPrompter](https://github.com/jame581/GodotPrompter) ⭐ 871 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-24 - Collection of 55 Godot 4.x domain skills and agents that AI coding agents load on demand for GDScript and C# development.

* [claude-ai-music-skills](https://github.com/bitwize-music-studio/claude-ai-music-skills) ⭐ 590 | 🐛 4 | 🌐 Python | 📅 2026-10-22 - Claude Code and Codex plugin with an MCP server for a Suno album workflow: concept, lyrics, prompts, mastering and release prep.

* [Busabase](https://github.com/busabase/busabase) ⭐ 589 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-24 - Open-source database and workspace for AI agents to manage typed tables, fields, views, records, docs, files, and search with a Streamable HTTP MCP server and human-in-the-loop ChangeRequests.

* [humanizer-ru](https://github.com/ilyautov/humanizer-ru) ⭐ 488 | 🐛 4 | 🌐 Python | 📅 2026-10-23 - Agent skill for Claude Code, Codex, Cursor and Gemini that rewrites Russian text to remove 64 AI-generation markers (bureaucratese, calques, ChatGPT fingerprints), with a corpus-calibrated scanner, audit mode and author-voice calibration.

* [bagel](https://github.com/Extelligence-ai/bagel) ⭐ 399 | 🐛 31 | 🌐 Python | 📅 2026-10-19 - MCP server: Query robotics, drone, and IoT logs in natural language and build auditable data-reduction pipelines with companion agent skills.

* [mcptoon](https://github.com/activeing123/mcptoon) ⭐ 388 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - MCP server: one zero-dependency CLI that turns 255 MCP tool schemas into a 581-token name index and fetches the full schema only when a tool is called.

* [mcpsnoop](https://github.com/kerlenton/mcpsnoop) ⭐ 364 | 🐛 0 | 🌐 Go | 📅 2026-10-17 - Wireshark for MCP, a transparent proxy that shows the real traffic between your AI client and MCP servers, fails CI on it and exports it as OpenTelemetry spans.

* [iphone-use](https://github.com/leeguooooo/iphone-use) ⭐ 354 | 🐛 3 | 🌐 Rust | 📅 2026-10-25 - MCP server: Controls real iPhones (iOS 15+) with a purpose-built XCTest runner (\~0.1 s text screen reads) and auto-discovered, reusable flows that replay whole tasks in one call without model inference or token cost.

* [affine-mcp-server](https://github.com/DAWNCR0W/affine-mcp-server) ⭐ 312 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-23 - MCP server exposing AFFiNE workspaces, documents, and databases to AI clients over stdio or HTTP.

* [opencode-visual-cache](https://github.com/Hotakus/opencode-visual-cache) ⭐ 311 | 🐛 8 | 🌐 TypeScript | 📅 2026-09-30 - OpenCode TUI plugin that displays real-time token cache hit rate, token usage, cost savings, and provider balance in a sidebar.

* [Kiln](https://github.com/instruktlabs/kiln) ⭐ 294 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-25 - 3D asset engine and toolchain for coding agents, with MCP, CLI and skills for generating, reviewing, revising and exporting assets through JavaScript.

* [ru-text](https://github.com/talkstream/ru-text) ⭐ 279 | 🐛 1 | 🌐 Shell | 📅 2026-10-18 - Russian text quality — \~1,044 rules for typography, info-style, editorial, UX writing, and business correspondence.

* [QVeris Agent Toolkit](https://github.com/QVerisAI/qveris-agent-toolkit) ⭐ 263 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-23 - MCP server: connects AI assistants to [QVeris](https://qveris.ai/) professional data and tools through hosted Streamable HTTP or local stdio, with discovery, inspection, parameter validation, execution, and usage audits.

* [Backlot](https://github.com/brekkylab/backlot) ⭐ 259 | 🐛 158 | 🌐 Python | 📅 2026-10-25 - Local emulator for Slack, Gmail, Google Drive, GitHub, Jira, Notion, S3 and other enterprise SaaS APIs, reproducing their response shapes, pagination, auth and per-document ACLs over a corpus you supply, so agents and RAG pipelines can be tested with no vendor account; `backlot mcp` serves every source as MCP tools.

* [Bitbucket CLI](https://github.com/avivsinai/bitbucket-cli) ⭐ 247 | 🐛 3 | 🌐 Go | 📅 2026-10-25 - Manage Bitbucket repos, PRs, branches, issues, webhooks, and pipelines for Data Center and Cloud.

* [Telnyx](https://github.com/team-telnyx/ai) ⭐ 224 | 🐛 26 | 🌐 TypeScript | 📅 2026-10-25 - Telnyx toolkit for AI agents bundling Claude Code, Cursor, Gemini CLI, and OpenCode plugins, an agent toolkit for OpenAI/LangChain/CrewAI/Vercel AI SDK, a hosted MCP server, and a one-command CLI for messaging, voice, numbers, and account management.

* [Taisly Agent Kit](https://github.com/taisly/agent) ⭐ 220 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-22 - Publish short-form videos to TikTok, Instagram Reels, YouTube Shorts, X, and Facebook from Codex with the Taisly MCP server and bundled social media posting skill.

* [X Twitter Scraper](https://github.com/Xquik-dev/x-twitter-scraper) ⭐ 220 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-25 - X/Twitter data, monitored workflows, HMAC webhooks, and MCP access through the Xquik REST API with confirmation-gated write guidance.

* [chrome-use](https://github.com/leeguooooo/chrome-use) ⭐ 208 | 🐛 15 | 🌐 Rust | 📅 2026-10-24 - MCP server: Controls your already-logged-in Chrome through native messaging, with isolated tab groups for concurrent agents and no remote-debugging port.

* [OC ChatGPT Multi Auth](https://github.com/ndycode/oc-chatgpt-multi-auth) ⭐ 207 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-20 - Codex setup skill and OpenCode plugin for ChatGPT Plus/Pro OAuth, GPT-5/Codex presets, and multi-account failover.

* [wechat-use](https://github.com/leeguooooo/wechat-use) ⭐ 200 | 🐛 4 | 🌐 Shell | 📅 2026-10-24 - Turns WeChat on macOS into a local API for agents and bots, with history and full-text search, contacts and groups, background sending without a UI flash, real-time listening, an HTTP bridge and a Wechaty gateway, plus experimental Windows x64 support.

* [tlgr](https://github.com/tlgrcli/tlgr) ⭐ 198 | 🐛 8 | 🌐 Python | 📅 2026-10-22 - Claude Code plugin and Agent Skill for operating a personal Telegram account through the tlgr CLI over MTProto, with JSON output and webhook event push.

* [Codex Usage Tracker](https://github.com/douglasmonsky/codex-usage-tracker) ⭐ 196 | 🐛 15 | 🌐 Python | 📅 2026-10-14 - Track aggregate Codex token usage from local session logs with MCP tools for summaries, session detail, CSV export, and dashboard generation.

* [Commercial Legal PL](https://github.com/apiotrowski-afk/commercial-legal-pl) ⭐ 179 | 🐛 1 | 🌐 Python | 📅 2026-10-09 - Drafts and reviews contracts under Polish law (B2B IT, IP, settlements) with a clause library, doctrinal knowledge base, and § / ust. / pkt cross-reference consistency checks.

* [Jev Social](https://github.com/socai-io/jev-social) ⭐ 179 | 🐛 13 | 🌐 JavaScript | 📅 2026-10-12 - Agent skill that runs read-only Instagram, TikTok, and LinkedIn research via browser automation and returns source-linked evidence reports.

* [opencode-visualiser](https://github.com/psinetron/opencode-visualiser) ⭐ 178 | 🐛 4 | 🌐 HTML | 📅 2026-10-23 - OpenCode plugin that renders live agent sessions as an animated pixel-art office with per-agent characters.

* [search1api-mcp](https://github.com/superagents-lab/search1api-mcp) ⭐ 173 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-24 - MCP server providing web search, news, page crawling, sitemaps, and trending topics via Search1API.

* [AgentCall](https://github.com/pattern-ai-labs/agentcall) ⭐ 171 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Lets Claude Code, Codex, Cursor, Gemini CLI, and 30+ other agents join Google Meet, Zoom, or Microsoft Teams as a speaking, listening, presenting participant with text-to-speech, live transcripts, screenshare, and an avatar camera feed.

* [Hostinger API MCP](https://github.com/hostinger/api-mcp-server) ⭐ 164 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-23 - Manage Hostinger VPS, domains, DNS, hosting, and billing through MCP tools backed by the official Hostinger API.

* [Miro](https://github.com/miroapp/miro-ai) ⭐ 164 | 🐛 19 | 🌐 TypeScript | 📅 2026-09-17 - Official Miro MCP server and agent integrations for Claude Code, Codex, Gemini CLI, Cursor, and other AI tools — read and write Miro boards, create diagrams, extract context from boards, and generate code from designs.

* [unslop](https://github.com/MohamedAbdallah-14/unslop) ⭐ 162 | 🐛 5 | 🌐 Python | 📅 2026-10-19 - Strip AI writing patterns from text output — removes filler phrases, hedging language, and generic constructs to produce cleaner written content. Install: `npm install -g unslop`.

* [X (Twitter) Skills](https://github.com/sergebulaev/x-skills) ⭐ 153 | 🐛 1 | 🌐 Python | 📅 2026-10-21 - Codex-ready X (Twitter) marketing bundle with a native .codex-plugin manifest: tweet and thread writing with corpus-validated hook formulas (validated against \~450 top tweets), AI-tell humanizer, hook extraction, reply drafting, content planning, and audience insights; also works in Claude Code.

* [Zero Slop](https://github.com/manavmishra/ZeroSlop) ⭐ 147 | 🐛 7 | 🌐 Python | 📅 2026-10-25 - Say no to AI slop: a human-in-the-loop learning agentic workflow skill that scores text 0-100 for AI slop and rewrites it tastefully, with a standard-library Python scorer that has zero dependencies and runs offline.

* [Tapetide](https://github.com/Tapetide-hq/nse-bse-indian-stock-market-data-mcp) ⭐ 142 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-14 - Indian stock market MCP server: research, screen and track about 8,200 NSE and BSE stocks from Claude, ChatGPT, Cursor or any MCP client.

* [Firecrawl](https://github.com/firecrawl/skills) ⭐ 137 | 🐛 5 | 📅 2026-10-22 - Official Firecrawl skills and MCP configuration for Claude Code, Cursor and Codex, giving agents web search, scraping, crawling, URL mapping and browser interaction.

* [Review Analyzer Skill](https://github.com/buluslan/review-analyzer-skill) ⭐ 137 | 🐛 2 | 🌐 Python | 📅 2026-09-17 - Agent skill that tags e-commerce reviews across 22 dimensions and produces a 15-chapter insight report, six HTML dashboards, and optional Feishu sync.

* [opencode-cmd-provider](https://github.com/rashidrazak/opencode-cmd-provider) ⭐ 126 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-24 - OpenCode plugin that registers Command Code as a provider so you can run its models and plans inside OpenCode, with a sidebar showing tier, allowances, and deal rates.

* [Pulse CC](https://github.com/fatwang2/Pulse) ⭐ 114 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-23 - Claude Code plugin that shows a stock and crypto watchlist above the prompt, with a `/pulse` panel to manage tickers and an optional local MCP connection to Pulse for Mac watchlists.

* [Langfuse Observability](https://github.com/avivsinai/langfuse-mcp) ⭐ 112 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - Query traces, debug exceptions, analyze sessions, and manage prompts via MCP tools.

* [whatsapp-claude-plugin](https://github.com/Rich627/whatsapp-claude-plugin) ⭐ 112 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-24 - Claude Code channel plugin and stdio MCP server that connects WhatsApp as a linked device for messaging, voice transcription, and remote tool approval.

* [open-doc](https://github.com/simonliu-ai-product/open-doc) ⭐ 111 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-20 - Document framework for agents: write React/TSX or import Markdown, render to real A4 pages, and export PDF, HTML, or Word, with bundled Agent Skills and an opt-in MCP server for editing documents.

* [DocsMint](https://github.com/HiAi-gg/docsmint) ⭐ 109 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-23 - Cloud or self-hosted knowledge workspace with MCP tools for hybrid search, GraphRAG, and document management.

* [Watermelon UI](https://github.com/WatermelonCorp/watermelon-platform) ⭐ 101 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - MCP server exposing 850+ source-backed React components, blocks, dashboards, and templates through search, retrieval, category, and page-composition tools.

* [im-ai-copyeditor](https://github.com/Turtle-Hwan/im-ai-copyeditor) ⭐ 100 | 🐛 2 | 🌐 Python | 📅 2026-09-08 - Korean copyediting skill for coding agents that fixes spelling, translation-style phrasing, AI tone, and style sentence by sentence.

* [XposedOrNot](https://github.com/XposedOrNot/XposedOrNot-API) ⭐ 100 | 🐛 1 | 🌐 Python | 📅 2026-10-25 - MCP server: XposedOrNot data breach lookups for emails and domains, with breach history, a breach catalog and domain exposure counts; remote, read-only, no API key.

* [GDS Agent](https://github.com/neo4j-contrib/gds-agent) ⭐ 98 | 🐛 0 | 🌐 Python | 📅 2026-10-12 - Graph data scientist as an MCP server and skill: project Neo4j graphs and run GDS algorithms for centrality, community, path finding, similarity, embeddings, and ML pipelines.

* [Call-E](https://github.com/CALLE-AI/call-e-integrations) ⭐ 97 | 🐛 28 | 🌐 JavaScript | 📅 2026-10-23 - Plan, run, and inspect Call-E phone call workflows from Codex through the calle CLI.

* [Jenkins CLI](https://github.com/avivsinai/jenkins-cli) ⭐ 95 | 🐛 1 | 🌐 Go | 📅 2026-10-25 - GitHub CLI-style interface for Jenkins controllers with jobs, pipelines, runs, logs, artifacts, credentials, and nodes.

* [You.com Agent Skills](https://github.com/youdotcom-oss/agent-skills) ⭐ 94 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-23 - Cross-platform You.com skill and plugin bundle that gives coding agents current web search, URL content extraction, cited research, finance research, and integration discovery, plus MCP server configs.

* [TikTok Skills](https://github.com/sergebulaev/tiktok-skills) ⭐ 91 | 🐛 1 | 🌐 Python | 📅 2026-10-21 - Codex-ready TikTok marketing bundle with a native .codex-plugin manifest and 8 skills: 3-second hook scripting (spoken line plus on-screen text), caption and hashtag writing under the 2,200-char API limit, trend mapping, profile optimization, AI-tell humanizer, and comment drafting; publishes through Publora with approval before anything goes live; also works in Claude Code.

* [Agent Message Queue](https://github.com/avivsinai/agent-message-queue) ⭐ 88 | 🐛 5 | 🌐 Go | 📅 2026-10-25 - File-based inter-agent messaging with co-op mode, cross-project federation, and orchestrator integrations.

* [plane-codex-mcp](https://github.com/Bene-2020/plane-codex-mcp) ⭐ 86 | 🐛 4 | 🌐 TypeScript | 📅 2026-10-22 - Codex plugin that captures project work events and syncs tasks, bugs, decisions and risks to Plane via a local SQLite outbox.

* [Kesha Voice Kit](https://github.com/drakulavich/kesha-voice-kit) ⭐ 79 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-25 - Local speech-to-text and text-to-speech CLI with an MCP server; it transcribes 25 languages and speaks 9, and every model runs on the machine itself rather than in a cloud service.

* [Network-AI](https://github.com/Jovancoding/Network-AI) ⭐ 79 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-19 - TypeScript multi-agent orchestrator shipped as a Claude Code plugin, Gemini CLI extension, and MCP server that adds an atomic shared blackboard, per-agent token budgets, permission gating, and audit trails across 32 agent frameworks.

* [VMware-AIops](https://github.com/vmware-skills/VMware-AIops) ⭐ 79 | 🐛 2 | 🌐 Python | 📅 2026-10-24 - Skill and MCP server with 60 tools for VMware vCenter and ESXi VM lifecycle, OVA/template deployment, snapshots, guest operations and cluster management, where every destructive tool previews what it would change and acts only on an explicit confirm.

* [Cortex](https://github.com/cdeust/Cortex) ⭐ 75 | 🐛 64 | 🌐 Python | 📅 2026-10-25 - Persistent thermodynamic memory and cognitive-profiling MCP server for Claude Code, Codex, and Gemini CLI — heat/decay dynamics, predictive-coding write gates, knowledge graph, and intent-aware recall across sessions.

* [mcp-music-studio](https://github.com/linxule/mcp-music-studio) ⭐ 75 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-19 - MCP server for AI music creation: scored ABC notation composition and Strudel live coding, with sheet music rendering, harmony analysis, and MIDI/WAV export.

* [KGLite](https://github.com/kkollsga/kglite) ⭐ 73 | 🐛 0 | 🌐 Rust | 📅 2026-10-24 - Turn datasets large and small into knowledge graphs for AI agent memory, knowledge retrieval, and connected-data analysis, with a high-performance local graph database and a ready-to-use MCP interface.

* [LMCP](https://github.com/colibird-ai/local-mcp-releases) ⭐ 73 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-23 - Local MCP server and plugins that let an assistant use Mail, Calendar, Contacts, Teams, Slack, WhatsApp, OneDrive, Google Drive, Notion, Outlook and Office files on macOS and Windows.

* [ScrapeGraph AI](https://github.com/ScrapeGraphAI/just-scrape) ⭐ 72 | 🐛 6 | 🌐 TypeScript | 📅 2026-09-21 - AI-powered web scraping CLI to search, scrape, extract structured JSON, crawl, and monitor web pages via the ScrapeGraph AI API.

* [peepshow](https://github.com/t0mtaylor/peepshow) ⭐ 69 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-10 - Gemini CLI extension registering `/peepshow:slides` and `/peepshow:sink` (with Claude Code, Cursor, Windsurf, Cline, and Codex manifests alongside) that turns videos, YouTube links, live streams, and animated GIF/APNG/WebP into an ordered timeline of frames plus a transcribed audio track, then fans each run out to 95 pluggable sinks across SQL, vector stores, object storage, chat, and issue trackers.

* [web-researcher-mcp](https://github.com/zoharbabin/web-researcher-mcp) ⭐ 69 | 🐛 7 | 🌐 Go | 📅 2026-10-25 - MCP server: web search, page extraction and citation verification across web, academic, patent, legal and filing sources, with source credibility scoring and retraction checks.

* [Arize Skills](https://github.com/Arize-ai/arize-skills) ⭐ 66 | 🐛 37 | 🌐 Python | 📅 2026-10-22 - A collection of agent skills for adding Arize observability and managing tracing, datasets, experiments, and prompt workflows via the Arize ax CLI.

* [Nimble](https://github.com/Nimbleway/agent-skills) ⭐ 61 | 🐛 7 | 🌐 Python | 📅 2026-10-23 - Web Search Agents that search, browse, extract, and reason across live pages and return cited, schema-enforced results, with self-learning retrieval that improves accuracy and lowers cost per task on repeat work, plus Search and Extract skills for fast raw web data in Claude Code, Codex, Cursor, and Grok Build.

* [Azure Cosmos DB Agent Kit](https://github.com/AzureCosmosDB/cosmosdb-agent-kit) ⭐ 59 | 🐛 31 | 🌐 Python | 📅 2026-10-16 - Azure Cosmos DB best-practice skills and MCP tooling for Codex, Claude Code, Cursor, Gemini CLI, Grok Build, Kimi Code, GitHub Copilot, and other Agent Skills-compatible assistants.

* [immich-photo-manager](https://github.com/drolosoft/immich-photo-manager) ⭐ 59 | 🐛 1 | 🌐 Python | 📅 2026-10-06 - MCP server and Claude Code plugin for self-hosted Immich photo libraries: CLIP and OCR search, geographic album curation, duplicate detection, people and faces, metadata repair, video frames and PDF photobooks, 94 tools and 13 skills tested live on Immich 2.x and 3.x, also via uvx or Docker.

* [OpenAI-Compatible Images](https://github.com/Syh1906/openai-compatible-imagegen) ⭐ 58 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-05 - Generate, edit, and batch-process images through OpenAI-compatible APIs using a standalone skill or a Codex App plugin with a canvas for annotating edit requests.

* [Threads Analytics](https://github.com/ridemountainpig/threads-analytics) ⭐ 57 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-25 - Self-hosted Threads analytics dashboard with an OAuth-protected, read-only MCP server for querying synced posts, performance metrics, and follower history.

* [RunAPI MCP Server](https://github.com/runapi-ai/mcp) ⭐ 56 | 🐛 10 | 🌐 TypeScript | 📅 2026-10-23 - MCP server for AI image generation, AI video generation, AI music creation, text-to-speech, prompt search, and model discovery.

* [dotpals](https://github.com/Rikinshah787/dotpals) ⭐ 55 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-22 - Desktop pal and notch that shows what AI coding agents did in plain words, with live diffs, approvals, and flags for .env changes, force-pushes, and two agents editing the same file across Claude Code, Codex, Cursor, Gemini CLI, and OpenCode.

* [kunglao-agent](https://github.com/amd2g2zz/kunglao-agent) ⭐ 55 | 🐛 62 | 🌐 Python | 📅 2026-10-25 - Reverse-engineering expert agent for binaries, firmware, protocols, and web/JS: MCP servers registered by kunglao-init (ghidra, sequential-thinking, x64dbg, ...), see the MCP supply table under Internals.

* [orionbelt-analytics](https://github.com/ralforion/orionbelt-analytics) ⭐ 53 | 🐛 0 | 🌐 Python | 📅 2026-10-24 - MCP server: analyzes database schemas, generates RDF/OWL ontologies with SQL mappings, and validates Text-to-SQL with fan-trap detection.

* [Sando](https://github.com/yuzushi-dev/sando) ⭐ 51 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-22 - Plugin for Claude Code and Codex that caps oversized tool output, salvages key lines, stores full artifacts, and redacts secrets.

* [bookstack-mcp](https://github.com/ttpears/bookstack-mcp) ⭐ 50 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-20 - MCP server for searching, reading, and managing BookStack wiki content from AI assistants.

* [SysKnife](https://github.com/lacs-project/sysknife) ⭐ 49 | 🐛 56 | 🌐 Rust | 📅 2026-10-25 - Linux sysadmin co-pilot as an MCP server for Codex: plain-language requests become typed, risk-classified actions that a privileged daemon runs only after out-of-band terminal approval, with an Ed25519-signed audit chain and automatic rollback.

* [Wolfpack](https://github.com/almogdepaz/wolfpack) ⭐ 49 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-25 - Self-hosted browser and phone terminals for persistent coding-agent sessions across your own macOS/Linux machines, with private Tailscale access.

* [Agent402](https://github.com/MikeyPetrillo/Agent402) ⭐ 47 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-24 - Open-source MCP server and x402 seller: 500+ tools for web search, rendering, PDFs, OCR, market and SEC data, paid per call in USDC or free via proof-of-work, no account or API key.

* [Pronounce](https://github.com/anzy-renlab-ai/pronounce) ⭐ 47 | 🐛 4 | 🌐 Python | 📅 2026-09-01 - Pronounce developer jargon out loud: an MCP server (lookup/search) and skill backed by a 1,721-entry sourced dictionary with IPA, audio, and cited pronunciations for kubectl, nginx, YAML, JWT, and more.

* [LawBox](https://github.com/Samwang-afk/LawBox) ⭐ 46 | 🐛 1 | 🌐 Python | 📅 2026-09-02 - A collection of 58 Chinese legal workflow skills with unified task routing, source verification, and adversarial review protocols.

* [AnyCap](https://github.com/anycap-ai/anycap) ⭐ 45 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-21 - Multimodal media generation, analysis, live web research, file sharing, and page publishing through one CLI, Agent Skill, and local MCP server.

* [claude-dev-suite](https://github.com/claude-dev-suite/claude-dev-suite) ⭐ 45 | 🐛 27 | 🌐 TypeScript | 📅 2026-10-23 - Detects a project's stack and installs the matching agents, framework skills and MCP servers into it, writing each assistant's own config format for Claude Code, Copilot, Cursor, Gemini CLI, Codex CLI, Cline and Kimi Code.

* [PANews Agent Toolkit](https://github.com/panewslab/skills) ⭐ 45 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-10 - Crypto and blockchain news discovery, authenticated creator publishing workflows, and page-to-Markdown reading.

* [aginxbrowser](https://github.com/yinnho/aginxbrowser) ⭐ 44 | 🐛 1 | 🌐 Rust | 📅 2026-10-25 - Rust MCP server and HTTP service that lets agents fetch JS-rendered or protected pages as clean markdown, meta-search 14 engines, screenshot, and run persistent logged-in sessions — each session exposes a live view URL so a human can watch and take over with the mouse.

* [Substack MCP](https://github.com/conorbronsdon/substack-mcp) ⭐ 44 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-24 - Safe Substack creator operations across publications: rich drafts, Notes, analytics, and consented subscribers; long-form posts stay draft-only, while Notes publish immediately.

* [lemo-mod](https://github.com/lemomo-ai/lemo-mod) ⭐ 43 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-17 - Claude Code plugin bundle: 21 styles for the terminal and desktop app, plus 16 mods (a panel, usage band, message numbers, speech, session recaps and more), with only looks on at install.

* [PixelLab Pip](https://github.com/Shilo/pixellab-pip) ⭐ 41 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - An unofficial, agent-agnostic Agent Skill for creating, editing, and animating pixel-art assets from plain-language requests, routing each task to PixelLab MCP tools, API endpoints, or editor workflows.

* [Genexus18MCP](https://github.com/lennix1337/Genexus18MCP) ⭐ 39 | 🐛 1 | 🌐 C# | 📅 2026-10-25 - MCP server that lets AI agents read, edit, analyze, and refactor objects in GeneXus Knowledge Bases through supported GeneXus SDKs and compatibility drivers.

* [JVM Pulse](https://github.com/brunoborges/jvm-pulse) ⭐ 39 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-16 - Claude Code plugin and GitHub Copilot canvas extension for profiling Java garbage collection and JFR telemetry, with a portable CLI and shareable HTML reports.

* [Kachilu Browser](https://github.com/kachilu-inc/kachilu-browser) ⭐ 39 | 🐛 3 | 🌐 JavaScript | 📅 2026-05-12 - Anti-bot-aware browser automation for AI agents with MCP tools, CAPTCHA-aware workflows, and WSL2 Windows browser support.

* [Hermes Tweet](https://github.com/Xquik-dev/hermes-tweet) ⭐ 37 | 🐛 2 | 🌐 Python | 📅 2026-10-25 - Hermes Agent X/Twitter plugin for read-first social research, monitoring, and approval-gated actions through Xquik.

* [hypruse](https://github.com/IlyasKhallouki/hypruse) ⭐ 37 | 🐛 0 | 🌐 Python | 📅 2026-10-19 - MCP server: computer use on Hyprland, with workspaces, windows, mouse, keyboard and screenshots on the Wayland desktop, plus a background mode that works in other windows while your cursor and focus stay put.

* [Slashbooks](https://github.com/giltotherescue/slashbooks) ⭐ 35 | 🐛 2 | 🌐 Python | 📅 2026-10-25 - Local-first AI bookkeeping plugin for Claude Cowork, Claude Code, and Codex that imports bank activity, closes the month, answers questions, and exports accountant-ready files for cash-basis businesses.

* [Flow Studio Power Automate](https://github.com/ninihen1/power-automate-mcp-skills) ⭐ 34 | 🐛 6 | 🌐 JavaScript | 📅 2026-09-04 - Debug, build, and operate Power Automate flows via FlowStudio MCP with action-level inputs and outputs.

* [MorningAI](https://github.com/octo-patch/MorningAI) ⭐ 33 | 🐛 5 | 🌐 Python | 📅 2026-05-16 - AI news tracking skill that monitors 80+ entities across 6 sources (Reddit, HN, GitHub, Hugging Face, arXiv, X) and generates scored daily reports with infographics and message digests.

* [opencode-cache-hit](https://github.com/zhumengzhu/opencode-cache-hit) ⭐ 33 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-20 - OpenCode sidebar plugin showing prompt cache hit rate, token usage, and cost with sub-agent session rollup.

* [OpenZine](https://github.com/JosssphZhou/openzine) ⭐ 32 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-10 - Agent skill for Claude Code and Codex that turns a PDF or a folder of page images into a page-turning 3D booklet, saved as one offline HTML file.

* [Talivia Agent Kit](https://github.com/talivia-group/agent) ⭐ 32 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-01 - Install and verify revenue-first website analytics from Codex, connect payment attribution, and identify which traffic sources and customer journeys become revenue.

* [Miro MCP Server](https://github.com/olgasafonova/miro-mcp-server) ⭐ 31 | 🐛 1 | 🌐 Go | 📅 2026-10-20 - Self-hosted single-binary Go MCP server exposing 110 tools for Miro boards, covering stickies, shapes, connectors, frames, mindmaps, flowcharts, tags, and bulk operations, with an essentials profile that trims the preload to 14 tools for smaller context budgets.

* [opencode-agy-auth](https://github.com/anthonyhaussman/opencode-agy-auth) ⭐ 31 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-23 - OpenCode plugin providing OAuth 2.0 authentication, model fetching, and quota tracking for the Antigravity CLI.

* [Codex Obsidian](https://github.com/greg-asher/codex-obsidian) ⭐ 30 | 🐛 3 | 📅 2026-04-22 - Local Obsidian note and vault workflows through the official desktop `obsidian` CLI.

* [DiviOps](https://github.com/oaris-dev/diviops) ⭐ 28 | 🐛 4 | 🌐 PHP | 📅 2026-10-20 - MCP server and authoring skills for building and editing native Divi 5 pages on WordPress with AI assistants.

* [agy-powerline](https://github.com/wassim-azi/agy-powerline) ⭐ 27 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-25 - Fast, configurable statusline for Google Antigravity CLI (agy) with live Gemini 5h/7d quota meters, pace markers, context usage, and interactive TUI configurator. <!-- platform: standalone -->

* [Kreuzberg](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Local document extraction for 91+ formats with skills for CLI usage, OCR, table extraction, output formats, and a local MCP server.

* [Kreuzberg Cloud](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Managed document extraction for Codex with API-key setup, presigned uploads, job tracking, webhook workflows, and usage guidance.

* [Kreuzcrawl](https://github.com/kreuzberg-dev/plugins) ⚠️ Archived - Web crawling and scraping for Codex with skills for single-page scraping, site crawls, URL mapping, and headless browser fallback.

* [open-cross-session](https://github.com/leeguooooo/open-cross-session) ⭐ 26 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-25 - Lets Claude Code, Codex, Pi, Hermes and terminal agent sessions message and wake each other on one machine or across paired LAN computers over a mutually authenticated, encrypted link, with no server or account. <!-- platform: standalone -->

* [agentic-seo](https://github.com/dalroot/agentic-seo) ⭐ 25 | 🐛 7 | 🌐 Python | 📅 2026-10-20 - SEO skill collection for AI coding assistants with 16 sub-skills, 10 specialist agents, and 89 evidence-collection scripts.

* [iki](https://github.com/zeikar/iki) ⭐ 24 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-25 - Claude Code and Codex plugin that draws character parts with an image model and auto-rigs them into an animated .iki puppet over an MCP server.

* [prompt-to-asset](https://github.com/MohamedAbdallah-14/prompt-to-asset) ⭐ 24 | 🐛 22 | 🌐 TypeScript | 📅 2026-10-18 - Route image-generation prompts to 30+ models (DALL-E, Stable Diffusion, Flux, Midjourney, and more) through a single MCP interface. Install: `npm install -g prompt-to-asset`.

* [Skill-Atlas](https://github.com/danielLublinsky/Skill-Atlas) ⭐ 24 | 🐛 0 | 🌐 Python | 📅 2026-08-16 - A third tier for Claude Code skills — dormant, zero tokens, still findable. Search a graph of your collection instead of preloading it.

* [framewright](https://github.com/smwbev/framewright) ⭐ 23 | 🐛 0 | 🌐 HTML | 📅 2026-09-26 - Agent skill for Claude Code, Codex and Gemini CLI that turns a brief into a short video from code: one self-contained HTML file with deterministic frames, 16 visual styles, rendered by headless Chrome and ffmpeg with a synthesized soundtrack and no footage.

* [Infrawise](https://github.com/Sidd27/infrawise) ⭐ 22 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-23 - MCP server and CLI that gives AI coding assistants live AWS, database, and Kafka infrastructure context (table schemas, Lambda trigger event shapes, queue and IaC config) and flags costly misconfigurations before they ship.

* [Mimi Seed](https://github.com/jeonghwanko/mimi-seed-sdk) ⭐ 22 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-22 - App launch ops for Claude Code and Codex: a local MCP server and CLI that drive Google Play, App Store Connect, Firebase, AdMob, and more from local credentials.

* [Thermal-Fluid Research Workflow](https://github.com/hanhuark/mechanical-engineering-research-skill) ⭐ 22 | 🐛 0 | 🌐 Python | 📅 2026-10-24 - Thermal-fluid mechanical engineering research workflow for literature review, technical writing, data analysis, presentations, proposals, coding, and AI/ML tools.

* [vybe-intelligence-vault](https://github.com/rxmna8502/vybe-intelligence-vault) ⭐ 22 | 🐛 6 | 📅 2026-10-25 - MCP server exposing a 160,000+ node AI knowledge graph for query and context injection by coding agents.

* [BoondManager MCP Server](https://github.com/fauguste/boondmanager-mcp-server) ⭐ 21 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-25 - MCP server for the BoondManager staffing ERP/CRM exposing 182 tools, 12 prompts and 22 resources over candidates, resources, opportunities, projects, invoices and expense reports, with stdio and OAuth-protected HTTP transports.

* [Yandex Direct](https://github.com/nebelov/yandex-direct-for-all) ⭐ 21 | 🐛 5 | 🌐 Python | 📅 2026-10-23 - GitHub-ready Codex plugin bundle for Yandex Direct, Wordstat, Metrika, and Roistat.

* [Cargo Skills](https://github.com/getcargohq/cargo-skills) ⭐ 20 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-25 - GTM engineering for coding agents — 17 skills over the Cargo CLI for lead sourcing, contact enrichment and email verification, lead scoring, CRM sync, buying-signal monitoring, and workspace-as-code.

* [claude-math](https://github.com/vladimirrott/claude-math) ⭐ 20 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-18 - Emit mathematics as copy- and search-safe inline Unicode (∑, ≤, ℝ, x², matrices, set-builder) instead of LaTeX so equations stay legible in the Codex TUI, terminals, and Claude Code.

* [clawock](https://github.com/KCNyu/clawock) ⭐ 20 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - A reusable investment decision-workflow extension that adds evidence-gated, code-settled trading decisions to external agents like Claude Code and OpenClaw.

* [Kindle Highlights](https://github.com/l3a0/claude-plugins) ⭐ 19 | 🐛 2 | 🌐 Python | 📅 2026-10-18 - Claude Code skill that exports a book's Kindle highlights to verbatim, location-cited Markdown, recovering the ones Amazon's export limit truncates or hides (macOS).

* [BountyGuard](https://github.com/doomsday-network/bounty-guard) ⭐ 18 | 🐛 4 | 🌐 Python | 📅 2026-10-25 - Pre-flight GitHub bounty security scanner and on-chain Proof-of-Escrow MCP verifier that classifies open bounties before AI agents invest compute.

* [GSC Security Checker](https://github.com/poliakarmai/gsc) ⭐ 18 | 🐛 4 | 🌐 HTML | 📅 2026-10-25 - MCP server: self-learning AppSec platform (SAST, SCA, secrets, IaC) whose 69 detectors prove exploitability with a sandboxed PoC gate and verify fixes, exposed as six read-only tools for agent-driven repository audits.

* [actual-budget-mcp](https://github.com/henfrydls/actual-budget-mcp) ⭐ 17 | 🐛 23 | 🌐 TypeScript | 📅 2026-10-23 - MCP server: ask your Actual Budget where the money went, and record transactions, transfers and budget moves from any MCP client, with duplicate checks before anything is written.

* [unic](https://github.com/DevopsArtFactory/unic) ⭐ 17 | 🐛 3 | 🌐 Go | 📅 2026-10-22 - Local MCP server exposing read-only AWS inspection tools to AI agents, including capability discovery, Backup vault listing, and context sync previews.

* [mathtype-for-word](https://github.com/felimet/mathtype-for-word) ⭐ 16 | 🐛 0 | 🌐 HTML | 📅 2026-10-13 - Codex and Claude Code plugin with a local MCP server and Agent Skill that creates editable MathType 7 equations in Word and PowerPoint on Windows, with MathType-native equation numbering and cross-references in Word.

* [Codex Mem](https://github.com/2kDarki/codex-mem) ⭐ 14 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-06 - Automatically capture, compress, and inject session context back into future Codex sessions.

* [SolidWorks GPT Plugin](https://github.com/Erfouni/solidworks-GPT-plugin) ⭐ 14 | 🐛 3 | 🌐 Python | 📅 2026-10-25 - Knowledge-backed SolidWorks design and validation workflows for Codex with standards lookup, CAD evidence gates, and consent-based session learning.

* [Data Product Builder for dbt](https://github.com/entropy-data/dataproduct-builder-dbt) ⭐ 13 | 🐛 2 | 🌐 Shell | 📅 2026-05-28 - Full data-product lifecycle on dbt for Entropy Data: scaffold, audit, and integrate projects with ODCS, ODPS, OpenLineage, and GitHub Actions.

* [Scholar Feed](https://github.com/YGao2005/scholar-feed-mcp) ⭐ 13 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-20 - MCP server over 600k+ CS/AI/ML papers: rank by citations or forecast rising impact, trace 23.2M citation edges, and pull full text and BibTeX; `npx -y scholar-feed-mcp`.

* [Whiteboard Video](https://github.com/Matteoikarieth96/whiteboard-video-skill) ⭐ 13 | 🐛 0 | 🌐 HTML | 📅 2026-10-15 - Claude Code skill that turns any topic into a hand-drawn whiteboard explainer video: it interviews you, writes a fact-checked script, offers voice samples (macOS, ElevenLabs, OpenAI or your own recordings), then draws, voices and renders an MP4 locally.

* [Context Pack](https://github.com/Rothschildiuk/context-pack) ⭐ 12 | 🐛 2 | 🌐 Rust | 📅 2026-09-27 - Generate compact first-pass repository briefings for coding agents before deeper exploration.

* [Rust Reverse Engineering](https://github.com/jingjing2222/rust-reverse-engineering-skill) ⭐ 12 | 🐛 0 | 🌐 Shell | 📅 2026-10-21 - Reverse engineer Rust binaries and libraries: triage targets, demangle symbols, recover crate namespaces, and map panic, unwind, async, and FFI paths.

* [motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) ⭐ 11 | 🐛 1 | 🌐 HTML | 📅 2026-10-19 - Claude Code skill that turns a short brief into a looping kinetic-typography launch video, written as one self-contained HTML file and rendered locally to MP4 with motion blur and a seamless loop.

* [One](https://github.com/withoneai/mcp) ⭐ 11 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-21 - MCP server: connects agents to 1000+ apps such as Gmail, Slack, Stripe and HubSpot to find, document and execute authenticated API actions, hosted at <https://mcp.withone.ai/mcp> over OAuth or run locally over stdio with `npx @withone/mcp`.

* [WakeWire](https://github.com/glenncalleja/wakewire) ⭐ 11 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-19 - Push events from GitHub, Gmail, Slack, and any signed webhook (Linear, Sentry, ClickUp) straight into your Codex threads as new turns — event-driven triggers instead of polling, with HMAC verification, deduplication, and a durable delivery queue.

* [Clera](https://github.com/getclera/mcp) ⭐ 10 | 🐛 1 | 📅 2026-10-18 - Hosted hiring MCP server plus Claude Code, Cursor and Gemini CLI plugins: search 210,000+ vetted startup candidates, review Clera's picks and request intros over OAuth.

* [kibi](https://github.com/Looted/kibi) ⭐ 10 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-25 - MCP server and per-agent plugins that compile product intent into structured requirements and check that code and tests stay consistent with them. <!-- platform: standalone -->

* [Unified AI System](https://github.com/happy520ai/unified-ai-system) ⭐ 10 | 🐛 42 | 🌐 JavaScript | 📅 2026-10-25 - Self-hosted AI gateway for Codex with provider-free prompt enhancement, governed MCP tools, and a credential-free Docker path.

* [Val Town](https://github.com/val-town/plugins) ⭐ 10 | 🐛 10 | 🌐 JavaScript | 📅 2026-10-13 - Build and deploy serverless TypeScript on Val Town from Codex — hosted MCP server plus skills for HTTP vals, cron, SQLite, email, OAuth, and React UI.

* [ai-memory-skill](https://github.com/syedair/ai-memory-skill) ⭐ 9 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-16 - Persistent memory skill for Claude Code and Kiro that auto-loads markdown context and runs a consolidation pass (`npx ai-memory-skill`).

* [Codex SEO](https://github.com/BestLemoon/codex-seo) ⭐ 9 | 🐛 11 | 🌐 Python | 📅 2026-07-03 - Full-stack SEO audits, Google API workflows, backlinks analysis, reporting, and optional MCP extensions for Codex.

* [pi-recall](https://github.com/pratikgajjar/recall) ⭐ 9 | 🐛 5 | 🌐 Go | 📅 2026-10-20 - pi extension that lets an agent search your past AI chat history across Cursor, Claude Code, Codex, and pi, backed by a local SQLite FTS5 index.

* [sitemd](https://github.com/sitemd-cc/sitemd) ⚠️ Archived - Build websites from Markdown via MCP — 22 tools for creating pages, generating content, validating, running SEO audits, configuring settings, and deploying static sites to Cloudflare Pages.

* [AutoCAD Tianzheng Tools](https://github.com/summer521521/AutoCAD_Tianzheng_plugin) ⭐ 8 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to AutoCAD and Tianzheng HVAC through a local MCP server for DWG-aware HVAC drawing inspection and workflow automation.

* [Codex Be Serious](https://github.com/lulucatdev/codex-be-serious) ⭐ 8 | 🐛 3 | 🌐 Shell | 📅 2026-06-01 - Enforce formal, textbook-grade written register across all agent output.

* [Creo](https://github.com/RaazKetan/creo) ⭐ 8 | 🐛 1 | 🌐 Swift | 📅 2026-10-20 - macOS menu bar app for searching and resuming Claude Code and Codex sessions, with live 5-hour and weekly plan usage for both.

* [ultramotion](https://github.com/sunsiyuan/ultramotion) ⭐ 8 | 🐛 0 | 🌐 HTML | 📅 2026-10-25 - Motion-template skills for Claude Code and Codex that turn one prompt into a finished vertical video with music: Liquid Glass, Kinetic Type, Hand-drawn Explainer and Variety Captions.

* [Vessel](https://github.com/spenceclark/Vessel) ⭐ 8 | 🐛 8 | 🌐 C# | 📅 2026-10-24 - Local reverse proxy that records every request and response between agents and Ollama, OpenAI-compatible or Anthropic backends to SQLite for search, replay and comparison, with a read-only MCP server for Claude Code and other MCP clients.

* [Apple Productivity](https://github.com/matk0shub/apple-productivity-mcp) ⭐ 7 | 🐛 4 | 🌐 Python | 📅 2026-03-27 - Local Apple Calendar and Reminders tooling for macOS with Codex plugin adapters.

* [bitwarden-use](https://github.com/leeguooooo/bitwarden-use) ⭐ 7 | 🐛 6 | 🌐 Rust | 📅 2026-10-24 - Agent-friendly Bitwarden and Vaultwarden CLI with an in-memory key agent, FIDO2 passkeys and direct secret injection into child processes without printing credentials. <!-- platform: standalone -->

* [Equibles](https://github.com/daniel3303/stock-market-mcp-server) ⭐ 7 | 🐛 0 | 📅 2026-10-19 - Plugin packages (Agent Plugins, Gemini CLI, Grok Build) for the hosted Equibles financial data MCP server: SEC filings, as-reported fundamentals, earnings-call transcripts, 13F holdings, and insider and congressional trades, with OAuth sign-in.

* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 7 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-20 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.

* [Upwork Autopilot](https://github.com/klajdikkolaj/upwork-autopilot) ⭐ 7 | 🐛 8 | 🌐 JavaScript | 📅 2026-07-03 - Controlled Upwork job search, qualification, and proposal submission sessions through a dedicated Chrome profile.

* [AI Command Center](https://github.com/Hredo/ai-command-center) ⭐ 6 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-25 - Local-first Windows, macOS and Linux command center for Claude Code, Codex, OpenCode, Aider, Gemini CLI, Ollama and 8,000+ API models, with live cost and token analytics (even for Claude Code sessions in other terminals), a side-by-side Arena, real terminals and git per project.

* [Dodo Payments](https://github.com/dodopayments/dodo-agent-plugin) ⭐ 6 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-12 - Payments integration for checkouts, subscriptions, and billing with live API and documentation MCP servers with browser OAuth.

* [Ethora](https://github.com/dappros/ethora-mcp-server) ⭐ 6 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-22 - MCP server for the Ethora chat and messaging platform: create and manage apps, chat rooms and users, broadcast messages, and deploy AI agents and RAG chatbots.

* [heldkeys](https://github.com/hugomn/heldkeys) ⭐ 6 | 🐛 0 | 🌐 Rust | 📅 2026-10-23 - Lists the credentials an AI coding agent can reach on a laptop, in a sandbox or in CI, and flags agent steps in GitHub workflows that hold secrets while reading untrusted input. <!-- platform: standalone -->

* [Antigravity 2.0](https://github.com/comprono/antigravity-2-codex-plugin) ⭐ 5 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-07 - Local Codex bridge for Antigravity desktop with setup checks, model limit summaries, DevTools UI automation, and safe project/chat handoff.

* [Cordon](https://github.com/ilyautov/cordon) ⭐ 5 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-21 - Deterministic trust boundary between untrusted content and agent actions for Claude Code, Gemini CLI, MCP hosts and LangChain that strips the hidden layer, keeps provenance of every piece of data, issues an intent certificate and gates calls against it with no model call anywhere on the hot path, covered by 998 tests over 18 pinned attack vectors.

* [EndNote for Word](https://github.com/felimet/endnote-for-word) ⭐ 5 | 🐛 2 | 🌐 Python | 📅 2026-10-20 - Codex and Claude Code plugin with a local MCP server and Agent Skill that creates native EndNote Cite While You Write citations and bibliographies in Word on Windows from DOI-verified references, including RIS import into EndNote libraries.

* [Hesper](https://github.com/derzierau/hesper) ⭐ 5 | 🐛 6 | 🌐 Go | 📅 2026-10-21 - MIT-licensed standalone macOS workspace for Claude Code and Codex with live terminals, attention controls, cross-Mac session handoffs, and Homebrew installation. <!-- platform: standalone -->

* [homie](https://github.com/prashanthgit19/homie) ⭐ 5 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - Four-level chat-voice personality layer for coding agents (off, yo, dawg, mafa) that changes how the agent talks in prose while leaving technical answers and code identical.

* [RankControl](https://github.com/rankcontrol/rankcontrol) ⭐ 5 | 🐛 0 | 📅 2026-10-22 - Claude Code plugin for the RankControl CLI: plan, write and publish SEO articles to your own CMS, then check Google rankings, site traffic and AI citations from the terminal.

* [Agentgram](https://github.com/jerryfane/agentgram) ⭐ 4 | 🐛 3 | 🌐 Python | 📅 2026-07-28 - Send Telegram messages, files, and forwarded inbox imports from Codex and local AI agents through a Telegram bot token and chat id.

* [AgentGuards](https://github.com/alelaguard/agentguards-plugins) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-10-17 - LLM security guardrails for Codex with enforcing hooks and MCP tools: jailbreak and prompt-injection detection, web-content scanning, data-exfiltration blocking, and destructive-command authorization.

* [Chrome DevTools](https://github.com/win4r/chrome-devtools-codex-plugin) ⭐ 4 | 🐛 4 | 📅 2026-03-27 - One-click Codex plugin wrapper for chrome-devtools-mcp.

* [Court Rules](https://github.com/foklepoint/court-rules-mcp) ⭐ 4 | 🐛 0 | 📅 2026-09-30 - Hosted MCP server (<https://mcp.courtrules.app/mcp>) for U.S. federal court rules, judge standing orders, court holidays, and filing checks, with a source citation on every rule.

* [Deadbolt](https://github.com/seanebones-lang/deadbolt) ⭐ 4 | 🐛 0 | 🌐 Rust | 📅 2026-10-24 - Local admission gate for software agents with short-lived leases, tool policy, one-shot approval, and operator revocation through Rust, HTTP, and stdio MCP integrations.

* [Feishu to Codex](https://github.com/zlsbksdxl/codex-lark) ⭐ 4 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-10 - Connect Codex to Feishu/Lark workflows for Docs, Messenger, Drive, Sheets, Base, Calendar, Tasks, Meetings, Mail, approvals, and more through the official Lark CLI.

* [GitHub Issues for Claude Code](https://github.com/MarcoCarnevali/claude-code-mods) ⭐ 4 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-08 - Claude Code mod that lists a repository's GitHub issues as cards in a side pane, with search, label filters and linked pull requests, and hands an issue to Claude with one click.

* [PapersFlow](https://github.com/papersflow-ai/papersflow-codex-plugin) ⭐ 4 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-10 - Paper discovery, citation verification, graph exploration, and DeepScan analysis.

* [Read Image](https://github.com/ZXY1240/read-image) ⭐ 4 | 🐛 6 | 🌐 Python | 📅 2026-10-12 - Read local images, videos, web pages, and Windows screenshots through Doubao, GLM, or Qwen-compatible vision APIs.

* [Remotion Plugin](https://github.com/tim-osterhus/codex-remotion-plugin) ⭐ 4 | 🐛 2 | 📅 2026-04-03 - Build parameterized Remotion videos in Codex with the official Remotion docs MCP, composition scaffolding, and a data-driven launch-video workflow.

* [SEO Dungeon](https://github.com/avalonreset/seo-dungeon) ⭐ 4 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-23 - Gamified local SEO audits that turn website issues into 16-bit dungeon battles for Codex, Claude, and Gemini CLI workflows.

* [Synta MCP](https://github.com/Synta-ai/n8n-mcp-codex-plugin-synta) ⭐ 4 | 🐛 1 | 📅 2026-04-03 - Build, edit, validate, and self-heal n8n workflows with Synta MCP tools and Codex-ready workflow guidance.

* [Task Scheduler](https://github.com/6Delta9/task-scheduler-codex-plugin) ⭐ 4 | 🐛 2 | 🌐 Python | 📅 2026-04-03 - OpenAI Codex plugin and local MCP server for turning task lists into realistic schedules with blocked dates, capacity overrides, overflow tracking, and markdown planning output.

* [UXKIN](https://github.com/uxkin/agent) ⭐ 4 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-19 - Hosted MCP server and free skills that give Claude Code, Codex, Cursor and other agents real iOS app screens, user journeys and website design systems to reference before building UI.

* [Zotero Research Tools](https://github.com/summer521521/Zotero_Research_plugin) ⭐ 4 | 🐛 0 | 🌐 PowerShell | 📅 2026-07-01 - Connects Codex to Zotero Desktop for local-library search, citation export, collection and tag inspection, and research workflow support.

* [Agent Vision](https://github.com/zfifteen/agent-vision) ⭐ 3 | 🐛 2 | 🌐 Shell | 📅 2026-07-14 - macOS-only local camera plugin for explicit snapshots, streaming controls, and file-backed image input.

* [Anode](https://github.com/skulitom/Anode) ⭐ 3 | 🐛 0 | 🌐 C# | 📅 2026-10-24 - Claude Code plugin for a hidden background Windows desktop for agents: GUI automation, UI Automation, screenshots and app testing without taking over your mouse.

* [AxonFlow](https://github.com/getaxonflow/axonflow-codex-plugin) ⭐ 3 | 🐛 8 | 🌐 Shell | 📅 2026-09-25 - Runtime governance for Codex with policy enforcement on terminal commands, advisory checks for non-terminal tools via skills, PII/secret detection, and compliance-grade audit trails. Self-hosted via Docker.

* [datawebot](https://github.com/datawebot/datawebot-mcp) ⭐ 3 | 🐛 1 | 📅 2026-10-23 - MCP server: hosted, closed-source ecommerce product data server at `https://mcp.datawebot.com/mcp` that searches products across online shops, lists each seller's price for one product with direct shop links, and runs extraction jobs on Amazon, Walmart US and other store pages, with a Claude Code plugin, Gemini CLI extension and agent skill in the repository.

* [DC Hub](https://github.com/azmartone67/dchub-mcp-server) ⭐ 3 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-25 - MCP server: DC Hub is the live data layer for data-center site selection. Its Data Center Power Index (DCPI) is a daily score of where data centers can get grid power, across 300+ markets. 94 tools at <https://dchub.cloud/mcp>.

* [LinkMCP](https://github.com/linkmcp-io/linkmcp) ⭐ 3 | 🐛 0 | 📅 2026-10-22 - Gemini CLI extension and remote MCP endpoint for the hosted LinkMCP service, which connects your own LinkedIn account for profile and company lookups, people and Sales Navigator search, inbox, posts, connection requests and work email finding (closed source; paid plans with a 7-day free trial).

* [mcp-for-Azgaar](https://github.com/aznan-triks/mcp-for-Azgaar) ⭐ 3 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-24 - MCP server connecting AI assistants to Azgaar's Fantasy Map Generator to inspect geography, manage realms, and edit maps locally.

* [mcp-pin](https://github.com/GautamTalksDev/mcp-pin) ⭐ 3 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-25 - Pins the MCP tool descriptions and schemas your client approved and stops the session when a server changes them, with a signed public log of 400+ servers.

* [RAPR AI](https://github.com/rawalrahul/raprai) ⭐ 3 | 🐛 12 | 🌐 Python | 📅 2026-10-25 - Run Claude Code, Codex, Ollama and other agents side by side on your own machine, with group chats and control from the browser, Telegram or WhatsApp. <!-- platform: standalone -->

* [SCVD General Store](https://github.com/seancrecord/scvd-general-store-repo) ⭐ 3 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-24 - Skills and hosted MCP for x402 endpoint preflight, signed receipt verification, and evidence-backed agentic commerce workflows.

* [Session Panel for Claude Code](https://github.com/bkaluza/vscode-claude-panel) ⭐ 3 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-23 - MIT VS Code extension that lists your Claude Code terminal sessions in a sidebar panel with live status (working, idle, needs you), subagents and context usage, opens them in named, coloured terminals with Cmd+1–9 switching, and reopens them after a restart. <!-- platform: standalone -->

* [SessionCost](https://github.com/kish21/sessioncost) ⭐ 3 | 🐛 2 | 🌐 HTML | 📅 2026-10-19 - Shows how many tokens each turn and call of a Claude Code, Codex, Cursor or Antigravity session sent, what it cost, and measured fixes to send fewer.

* [Shots](https://github.com/hitSlop/shots) ⭐ 3 | 🐛 2 | 🌐 Python | 📅 2026-10-14 - Agent-native App Store screenshot, app icon, ASO, and localization workflows through the hosted Shots MCP server.

* [Bestax](https://github.com/allxsmith/bestax-skills) ⭐ 2 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - Agent Skills and a local MCP server for building React apps with Bestax on Bulma v1, covering forms, layouts, theming, icons, CSS size, and migration from older Bulma libraries.

* [BulkPublish](https://github.com/azeemkafridi/bulkpublish-ai-toolkit) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-24 - Official BulkPublish MCP server config and agent skills for Claude Code, Cursor, and other Agent Skills clients that draft, schedule, cross-post, and analyze social media posts on 15 platforms, including Instagram, TikTok, YouTube, X, and LinkedIn.

* [Cadence Code](https://github.com/michael-L-i/cadence-code) ⭐ 2 | 🐛 6 | 🌐 Python | 📅 2026-10-20 - Fully local voice conversations for Claude Code, Codex, Cursor, and Antigravity on Apple Silicon, with selectable MLX speech and transcription models.

* [Canvas Apps Plugin Codex](https://github.com/Ratnam-Mishra/canvas-apps-plugin-codex) ⭐ 2 | 🐛 4 | 📅 2026-05-03 - Build and edit Microsoft Power Apps Canvas Apps using natural language and Canvas Authoring MCP server.

* [DataForge](https://github.com/ianktoo/data-forge) ⭐ 2 | 🐛 11 | 🌐 Python | 📅 2026-09-29 - Turns any website into a quality-scored LLM fine-tuning dataset in JSONL, Parquet or on the Hugging Face Hub, with a CLI and a `dataforge mcp` server exposing tools to scrape, explore, validate, run and inspect a dataset build.

* [herdr-acp](https://github.com/frankjoshua/herdr-acp) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-10-22 - Exposes a Herdr terminal pane running Claude Code, Codex, Pi, or a plain shell as an Agent Client Protocol agent, streaming everything in the pane to the client as one shared session.

* [Maestro: Costguard](https://github.com/mbanderas/costguard) ⭐ 2 | 🐛 7 | 🌐 TypeScript | 📅 2026-09-17 - Cost auditor for Codex that flags CI/cron and cloud-spend waste via read-only provider checks, then previews and applies surgical CI workflow fixes locally without writing to provider accounts or pushing git.

* [MATLAB Simulink Tools](https://github.com/summer521521/MATLAB_Simulink_plugin) ⭐ 2 | 🐛 0 | 🌐 MATLAB | 📅 2026-07-01 - Connects Codex to MATLAB and Simulink through a local MCP server for model inspection, script execution, and engineering workflow automation.

* [mcp-gatehouse](https://github.com/nickgeorgeseo/mcp-gatehouse) ⭐ 2 | 🐛 0 | 🌐 Python | 📅 2026-10-23 - Python library that adds permission tiers, fail-closed approval gates, and append-only JSONL audit logging with secret redaction inside MCP servers built on the official Python SDK, with no proxy or external policy service (`pip install mcp-gatehouse`).

* [OrgX](https://github.com/useorgx/orgx-codex-plugin) ⭐ 2 | 🐛 14 | 🌐 JavaScript | 📅 2026-10-23 - MCP access and initiative-aware skills for organizational workflows.

* [Sessionbus](https://github.com/antst/sessionbus-peers) ⭐ 2 | 🐛 1 | 🌐 Go | 📅 2026-10-14 - Connects independently started Claude Code, Codex, Grok, Qwen, OpenCode and Kilo sessions and custom tools through an open bus protocol for live messaging and optional managed sessions across products and hosts, while keeping native harnesses.

* [SkyAccess](https://github.com/sky-access/skyaccess-mcp) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-06 - Search 5,000+ live empty leg flights, get charter price estimates and booking links; no account or API key.

* [SpringBrand](https://github.com/springbrand-lab/springbrand-agent-setup) ⭐ 2 | 🐛 21 | 🌐 Python | 📅 2026-10-16 - Hosted go-to-market MCP server with setup guides for Claude Code, Codex, Cursor and other agents: social listening across X, TikTok, Instagram, YouTube, Reddit and Xiaohongshu, website traffic and SEO research, company, contact and creator discovery, and copy, image, video and voiceover generation over OAuth, billed per call.

* [agentmailkit](https://github.com/ariaxhan/agentmailkit) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-28 - MCP server for scheduled LLM-written email digests from RSS, web and local sources: tools list\_jobs/run\_job/preview\_job/list\_plugins, local-first, run\_job dry-run by default; `pip install "agentmailkit[mcp]"` then `agentmailkit mcp`.

* [aw1-breaker](https://github.com/MvikManners/aw1-circuit-breaker) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Deterministic out-of-band execution circuit breaker and AST safety proxy for autonomous AI agent tool calls.

* [Bilinc](https://github.com/atakanelik34/Bilinc) ⭐ 1 | 🐛 2 | 🌐 Python | 📅 2026-10-22 - Persistent memory for AI agents over MCP: commit, recall, revise, snapshot and roll back agent state with provenance, shared across Claude Code, Claude Desktop and other MCP clients.

* [Car Rental Business Skills](https://github.com/sergebulaev/car-rental-skills) ⭐ 1 | 🐛 2 | 🌐 Python | 📅 2026-10-20 - Codex-ready bundle for exotic, luxury and Turo car rental operators with a native .codex-plugin manifest and 8 skills that price a car against live published daily rates from a free read-only market data MCP server, scan competitors, plan a rental business, and draft rental agreements, damage inspections, listings, social posts and review replies; also works in Claude Code.

* [CarsXE](https://github.com/carsxe/carsxe-codex-plugin) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-01 - Decode VINs, license plates, market value, vehicle history, recalls, liens, OBD codes, and more via the CarsXE API.

* [Chorale](https://github.com/hxy9243/chorale) ⭐ 1 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-24 - An LLM-assisted music sheet analysis and composition local MCP server and a web UI for inspect, annotate, compose, and interactively editing ABC notations for music.

* [Command Code Usage](https://github.com/Jovan1666/commandcode-usage) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-05 - Shows Command Code plan quota (5-hour, weekly and monthly windows with reset times) inside Claude Code, Codex, ZCode, Grok Build, opencode, pi and DeepSeek Harness, read from local session data so checking your quota costs no quota.

* [Computer Usage Summary](https://github.com/liuyewang/computer-usage-summary-skill) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-08-03 - Privacy-first, local ActivityWatch reports for app time, AFK time, projects, billable work, and redacted timelines across macOS, Windows, and Linux.

* [CONTAM Tools](https://github.com/summer521521/CONTAM_plugin) ⭐ 1 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-01 - Runs and inspects CONTAM airflow projects through a local MCP server with project guards, diagnostics, simulation helpers, and bridge workflows.

* [Coolify](https://github.com/Sevi-py/coolify-codex-plugin) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-16 - Control Coolify Cloud and self-hosted Coolify instances through API-aware workflow skills and local tools.

* [drip](https://github.com/beausterling/drip-ai-water-usage) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-10-10 - Live water meter for Claude Code and Codex that reads their local session logs to estimate each session's water and energy use, shown in the status line with low/mid/high ranges and cited sources, with `drip run codex` opening the agent beside a live meter.

* [Exa Web Search](https://github.com/zlsbksdxl/codex-exa) ⭐ 1 | 🐛 2 | 🌐 Shell | 📅 2026-10-14 - Search and fetch current web sources in Codex through the official Exa MCP server with browser OAuth.

* [Google Hotels MCP](https://github.com/huynhtanan/google-hotels-mcp) ⭐ 1 | 🐛 5 | 🌐 Python | 📅 2026-10-16 - MCP server: search Google Hotels and Vacation Rentals, get OTA rates, nightly price calendars and reviews for Claude Desktop, Cursor and other MCP clients.

* [GPT-6 Astra Outbound System](https://github.com/heypastel/pastel-outbound-system) ⭐ 1 | 🐛 1 | 📅 2026-10-01 - Codex plugin with 20 outbound skills and 12 agents that catch LinkedIn buying signals, qualify and rank leads, write human-sounding messages and posts, run sequences, and handle replies through the Pastel MCP, with every send approved first.

* [Hotpath](https://github.com/mourad-baazi/hotpath) ⭐ 1 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-22 - Records an agent's MCP tool calls once and compiles them into a deterministic, editable workflow that drops failed calls, uses AI only at judgment steps, and self-heals when data changes shape.

* [Hyreflow](https://github.com/automindz-solutions/hyreflow-plugins) ⭐ 1 | 🐛 0 | 🌐 HTML | 📅 2026-10-09 - Recruitment automation plugin for Codex, Claude Code, Cowork and Cursor with Agent Skills and a remote OAuth MCP server: source, enrich, qualify and sequence candidates, then push them to your ATS on metered credits.

* [LienDeadline](https://github.com/LienDeadline/skills) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-22 - US mechanics lien and preliminary notice deadlines for construction material suppliers, with statute citations, plus lien guides for all 50 states and DC; read-only.

* [Nullcost](https://github.com/johnvouros/nullcost-plugin) ⭐ 1 | 🐛 2 | 🌐 JavaScript | 📅 2026-07-12 - Catalog-backed free-tier, free-trial, and cheap developer-tool recommendations for Codex through bundled skills and MCP tools.

* [opencode-stay-awake](https://github.com/AuroraAeon/opencode-stay-awake) ⭐ 1 | 🐛 0 | 🌐 JavaScript | 📅 2026-09-23 - OpenCode plugin that holds a system sleep inhibitor while a session is running, using caffeinate on macOS and systemd-inhibit on Linux, and releases it as soon as the work finishes.

* [OpenProject Codex](https://github.com/varaprasadreddy9676/openproject-codex-plugin) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-16 - OpenProject integration for Codex with project, team, work package, bulk workflow, boards, wiki, meeting, attachment, and reporting support.

* [Ophis](https://github.com/ophis-fi/skills) ⭐ 1 | 🐛 3 | 📅 2026-09-21 - Onchain token swaps for Codex via the hosted Ophis MCP server, MEV-protected and gasless, built on CoW Protocol.

* [ParlayAPI](https://github.com/JacobiusMakes/parlay-api-mcp) ⭐ 1 | 🐛 1 | 🌐 Python | 📅 2026-10-02 - Python MCP server for sports odds, player props, public event discovery, and account usage; account data tools require your own API key and allowances.

* [phone-sms](https://github.com/h-3303/phone-sms) ⭐ 1 | 🐛 0 | 🌐 CSS | 📅 2026-10-10 - MCP server and Claude Code plugin that reads and sends SMS through the user's own Android phone over KDE Connect on the local network, with no cloud relay, sending only after the user approves recipient and text.

* [pi-visor](https://github.com/laveesingh/awesome-pi-extensions) ⭐ 1 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-21 - Pi extension that collapses every tool call to two lines and each agent run into a bounded two-layer frame you expand by click or Ctrl+O, with a live turn bar and one-line thinking summaries. Install: `pi install npm:pi-visor`.

* [Portway](https://github.com/rath/portway) ⭐ 1 | 🐛 0 | 🌐 Rust | 📅 2026-10-23 - A local HTTP proxy for Claude Code, Codex, and OpenAI-compatible endpoints on vLLM or SGLang that sends each turn as a zstd delta against the previous one: about 1 KiB, not the whole context.

* [PostEverywhere](https://github.com/posteverywhere/claude-plugin) ⭐ 1 | 🐛 0 | 📅 2026-10-20 - Social media scheduler plugin: write, schedule and publish posts to Instagram, TikTok, YouTube, LinkedIn, X, Threads, Pinterest, Bluesky and more, plan a content calendar and see analytics, through a hosted MCP server and 15 skills ([posteverywhere.ai](https://posteverywhere.ai)).

* [Reduck Agents](https://github.com/reduck-ai/agents) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2026-08-06 - Claude Code plugin marketplace and agent skills that discover, run, and create browser automation scripts through the Reduck MCP in your own logged-in Chrome, with reference agents for GEO audits and SaaS invoice retrieval.

* [sectionsight](https://github.com/Majny/sectionsight) ⭐ 1 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-25 - Claude Code skill that sets up cookieless, privacy-first website analytics (time per page section, consent banner, Slack or e-mail reports, health alerts) and proves the privacy claims with a headless-browser check.

* [site-spec](https://github.com/ariaxhan/site-spec) ⭐ 1 | 🐛 12 | 🌐 TypeScript | 📅 2026-10-22 - MCP server for website audit and auto-fix: 40 checks across SEO, accessibility, privacy, structured data and AI searchability, tools audit\_site/fix\_issue/compile\_spec/list\_checks; `npx -y site-spec-mcp`.

* [ThoughtProof MCP](https://github.com/ThoughtProof/thoughtproof-mcp) ⭐ 1 | 🐛 4 | 🌐 JavaScript | 📅 2026-10-24 - Local MCP pre-action verification for agents: mandate + proposed action → ALLOW/BLOCK/UNCERTAIN; execute only on ALLOW.

* [YYLO Skills](https://github.com/yylo-dev/yylo-skills) ⭐ 1 | 🐛 6 | 🌐 JavaScript | 📅 2026-10-17 - Reusable agent skills maintained by YYLO: the canonical, independently versioned source for the ledger-tasks, wiki, workflow, artifact, benchmark, understand-project, plan-ledger-tasks and ralph-loop skills used by YYLO CLI and YYLO Ledger.

* [10ML Perfume Finder](https://github.com/10ml-com/perfume-finder-mcp) ⭐ 0 | 🐛 1 | 📅 2026-10-20 - MCP server: the 10ML Fragrance Index for AI assistants, with perfume notes, accords, families, similar scents and expert guides; free, no API key.

* [Agent Face](https://github.com/ericphamhoangdev/agent-face-skills) ⭐ 0 | 🐛 7 | 🌐 JavaScript | 📅 2026-10-07 - Agent skills that give a coding agent a small always-on-top desktop face showing its state (working, thinking, happy, stuck) with captions and lip-synced voice clips.

* [AgentBadge MCP](https://github.com/spreadzp/agentbadge-mcp) ⭐ 0 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-23 - Verify agents, check trust scores, and pay for services with x402 — ERC-8004 identity on Arc via MCP.

* [AgentDocStore](https://github.com/koushikginjupally/agentdocstore) ⭐ 0 | 🐛 12 | 🌐 TypeScript | 📅 2026-10-24 - Self-hostable, offline-first versioned document store with a web UI, REST API, and a 16-tool stdio MCP server that catches secrets before they are saved.

* [agentic-finance-graph-mcp](https://github.com/AgenticFinanceGraph/agentic-finance-graph-mcp) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-24 - Read-only MCP server and CLI for Agentic Finance Graph, the independent ledger of machine money: which AI agents on Base actually pay, what they really spend, ranks, detections and metric history, free with no API key.

* [Aient](https://github.com/aient-ai/aient-codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-06-02 - AI operations plugin for Codex that connects production telemetry, problem lifecycle context, and remediation workflows through Aient's MCP server.

* [Anywhere](https://github.com/raph559/anywhere) ⭐ 0 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-25 - Self-hosted web app to start, open and stop Claude Code Remote Control sessions on your own Linux, WSL and Windows machines from your phone: pick a device, pick a folder, tap Start.

* [Auten](https://github.com/auten-ai/auten-mcp) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-15 - MCP server: gives Claude Code, Codex, Cursor or any MCP client hands on a real screen, your computer (Mac, Windows, Linux) and your Android phone (beta), clicking, typing and reading even in apps with no API, and replays learned tasks without a model call.

* [authority.md](https://github.com/gareth-hoyle/authority-md-plugin) ⭐ 0 | 🐛 2 | 📅 2026-10-21 - MCP server: search 640+ thinking frameworks drawn from notable thinkers' documented work, plus task Tools and Playbooks, from any MCP client, with a framework-finder skill and a free Sherlock Holmes deduction skill.

* [cc-dash-kit](https://github.com/coolthor/cc-dash-kit) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-19 - Sidebar dashboard for Claude Code showing 5-hour/weekly usage limits and session cards, installable with one prompt and extensible with custom cards (e.g., GPU or local services).

* [cguard](https://github.com/simon-init/cguard) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-16 - A Claude Code plugin hook that keeps secrets, stray docs and destructive commands out of agent sessions.

* [Clayform](https://github.com/sezginkipel/clayform) ⭐ 0 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-24 - MCP server that lets agents build 3D models from a semantic scene document, look at them through a software renderer, check them with measuring critics, rig and animate them, and export glTF, with no Blender or GPU.

* [Codex Reset](https://github.com/suvadadepolo-blip/codex-reset-mcp) ⭐ 0 | 🐛 0 | 📅 2026-09-24 - Hosted read-only MCP tools for when Codex usage limits reset: 24/48h reset forecast, verified reset record with sources, and outage-vs-limit service status.

* [ConnectMachine](https://github.com/connectmachine/claude-plugin) ⭐ 0 | 🐛 0 | 📅 2026-10-23 - Claude Code and Cowork plugin plus remote MCP server for your contacts and digital business cards: find people by how you remember them, save contacts from a conversation, and draft follow-ups.

* [CoreSpeed](https://github.com/corespeed-io/cs) ⭐ 0 | 🐛 3 | 📅 2026-10-15 - One MCP endpoint with browser sign-in that gives any agent (Claude Code, Codex, Cursor and more) your apps, your team's shared memory and built-in tools for media, web search and social data, with spend caps and an activity log; this plugin adds it to Claude Code and Codex with skills for the cs CLI.

* [CurlShot MCP](https://github.com/SergiuPogor/curlshot-mcp) ⭐ 0 | 🐛 0 | 📅 2026-10-24 - MCP server: hosted streamable-HTTP server whose `take_screenshot` tool renders a public web page in a real browser and returns PNG, JPEG, WebP, PDF or a scrolling video; needs a CurlShot API key (free plan available).

* [Cutbolt](https://github.com/skulitom/cutbolt-plugin) ⭐ 0 | 🐛 0 | 📅 2026-10-19 - Claude Code plugin for Cutbolt, a local video editing engine, with its MCP tools and six skills for captions, talking-head recuts, multi-camera interviews, screen tutorials and delivery, saved as reversible edits (needs the cutbolt engine and FFmpeg).

* [Darkmoon](https://github.com/ASCIT31/darkmoon-mcp-server) ⭐ 0 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-19 - Claude Code plugin and MCP server that drives a self-hosted Darkmoon Pro instance (autonomous AI pentest engine, GPL-3.0) to start a run against an authorized target, poll status, list campaigns and read findings; requires Darkmoon Pro and run\_pentest is not read-only.

* [Droplinked](https://github.com/droplinked/droplinked-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-08-05 - Verified-inventory agentic commerce over a hosted MCP server, with merchant and product discovery, agent-initiated checkout, and onchain brand, credit-risk, and repayment attestations.

* [flacli](https://github.com/h-3303/flacli) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-10-06 - CLI, MCP servers and Claude Code plugin that take named albums or a playlist (TIDAL, Deezer, YouTube Music, export files), match them against the local library via MusicBrainz, fetch the missing tracks through the user's own Nicotine+ (Soulseek) client, then file, tag and tidy the library; successor to claude-music.

* [flatrate-math](https://github.com/scrapertweeter3-prog/mcp-flatratemath) ⭐ 0 | 🐛 4 | 🌐 Python | 📅 2026-10-23 - MCP server: prices a fixed bid, a fully loaded hire, and a flat-rate subscription on one number, total cost per delivered request (stdio JSON-RPC, Python stdlib only).

* [FXMacroData](https://github.com/fxmacrodata/claude-plugin-fxmacrodata) ⭐ 0 | 🐛 0 | 📅 2026-10-21 - Claude Code and Codex plugin with a skill and the hosted FXMacroData MCP server for official-source macro releases, central-bank rates, release calendars and FX rates across 22 currencies (USD releases, calendar and catalogue work without a key).

* [Game Boy MCP Player](https://github.com/Dst0rtr/pokemon-ai-player) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - MCP server that lets AI agents play any Game Boy game through PyBoy, with a Pokémon Red/Blue/Yellow profile that reads game state from memory and built-in benchmark metrics.

* [GH Project](https://github.com/zfifteen/gh-project-plugin) ⭐ 0 | 🐛 2 | 🌐 HTML | 📅 2026-05-15 - Create GitHub repositories from Codex with inferred defaults, native menus, explicit confirmation, and deterministic local cloning.

* [Grabbit](https://github.com/BrainGridAI/grabbit-mcp) ⭐ 0 | 🐛 0 | 📅 2026-09-29 - Hosted screenshot MCP for agents that grabs any URL as a hosted image with no local Chromium.

* [GSC Quick Wins](https://github.com/iniyan/gsc-quick-wins) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-09-29 - Agent Skill that reads a Google Search Console export, finds keywords stuck in positions 4–20, and writes the exact title, meta, H2, FAQ and internal-link fixes, with a zero-dependency Python scorer.

* [HodlJuice](https://github.com/nmorton13/hodljuice-cli) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-10-23 - Claude Code plugin and `hj` CLI for searching and playing 30,000+ Bitcoin podcast episodes, with a status-line player, /pint and /brew commands, and a hosted MCP server.

* [HProxy MCP](https://github.com/hproxy-com/hproxy-mcp) ⭐ 0 | 🐛 1 | 📅 2026-10-14 - Hosted MCP server, Claude Code plugin and Gemini CLI extension exposing proxy\_list, proxy\_check and ip\_lookup over a keyless, continuously verified free proxy pool, with nothing to install.

* [icon-mcp](https://github.com/pratham-jain33/icon-mcp) ⭐ 0 | 🐛 4 | 🌐 Python | 📅 2026-10-18 - MCP server that generates matching Lucide icon sets as SVG from a list of icon requests plus a shared style, fully offline with no API key.

* [Lacuna Music](https://github.com/JOYLINK-LTD/lacuna-plugin) ⭐ 0 | 🐛 2 | 📅 2026-08-31 - Generate original instrumental music and vocal songs from Codex through the Lacuna MCP server.

* [Launch Fast](https://github.com/BlockchainHB/launchfast_codex_plugin) ⭐ 0 | 🐛 3 | 📅 2026-08-20 - Official Launch Fast plugin adapter for rapid SaaS deployment.

* [LinkBit](https://github.com/yutotanakastar/linkbit-mcp) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-13 - MCP server: shorten URLs, generate QR codes, and read click analytics via LinkBit (npx linkbit-mcp, slk\_ API key).

* [looot](https://github.com/loootai/looot-skills) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-10-12 - 21 Agent Skills that search, price and run 2,500+ data API endpoints (work emails, company and people search, Google results, web pages) with one prepaid balance.

* [mcp-dialect-fix](https://github.com/Salman-Labs/mcp-dialect-fix) ⭐ 0 | 🐛 7 | 🌐 TypeScript | 📅 2026-10-16 - npx stdio proxy that rewrites MCP tool schemas from JSON Schema draft-07 to 2020-12 for Claude Desktop and Cowork, plus an SDK transport wrapper and a CI check.

* [mcp-infer](https://github.com/Emilthelucky/mcp-infer) ⭐ 0 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-20 - Infers MCP tool definitions from TypeScript types and JSDoc for the official MCP TypeScript SDK. <!-- platform: standalone -->

* [memory-mcp](https://github.com/Donk338/memory-mcp) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-20 - MCP server: persistent agent memory with semantic recall served as a remote streamable-HTTP endpoint — your wallet address is your private namespace, no accounts or API keys, paid per call in USDC on Base via x402, with a free wallet-signed tier.

* [Mnemoverse Memory](https://github.com/mnemoverse/claude-plugin) ⭐ 0 | 🐛 5 | 🌐 JavaScript | 📅 2026-10-25 - Claude Code plugin for hosted AI agent memory over MCP that learns from outcomes: tell it a recalled memory helped or misled and it re-ranks what comes back next, with shared rooms for multi-agent work and browser OAuth sign-in instead of an API key.

* [Mobazha](https://github.com/mobazha/mobazha-skills) ⭐ 0 | 🐛 3 | 🌐 Python | 📅 2026-05-03 - Decentralized e-commerce skills — deploy self-hosted stores, import products from Shopify/Amazon, configure custom domains and Telegram bots, set up Tor privacy, and manage your store via MCP.

* [Nestbolt](https://github.com/skulitom/nestbolt-plugin) ⭐ 0 | 🐛 0 | 📅 2026-10-19 - Claude Code plugin for Nestbolt, free local sheet nesting that fits SVG or DXF parts onto fixed sheets for laser, CNC, plasma, waterjet, fabric and leather cutting, checks every layout and saves per-sheet SVG/DXF cut files.

* [NeverApply](https://github.com/kasovy/neverapply-mcp) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - MCP server: hosted remote server (Streamable HTTP, OAuth 2.1) that lets Claude, Cursor, and other MCP clients search and match jobs, tailor resumes, answer screening questions, and apply to jobs only with the user's approval.

* [Obsidian MCP](https://github.com/dharmikbhesaniya/obsidian-mcp) ⭐ 0 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-20 - Typed Model Context Protocol server enabling local and remote AI agents to access Obsidian vaults over stdio and Streamable HTTP with scoped bearer authentication and per-vault permissions.

* [okaypic-video-skill](https://github.com/okaypic/okaypic-video-skill) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-10-17 - Claude Code skill and Python toolchain that turns a script into a finished episode through the okaypic.com video API: character reference sheets, batch MiniMax H3 rendering with generated voices, a local timeline editor with English and Chinese captions, and a one-command final cut.

* [Overleaf LaTeX](https://github.com/MarcoDotIO/overleaf-latex) ⭐ 0 | 🐛 0 | 🌐 TypeScript | 📅 2026-09-30 - Local MCP/Codex plugin for creating and editing Overleaf projects.

* [PDFtoAgent (Dow Theory MCP)](https://github.com/babaksh/PDFtoAgent) ⭐ 0 | 🐛 4 | 📅 2026-10-24 - Turnkey FastMCP server built with the PDFtoAgent pipeline, extracting 100+ deterministic tools from the book into a unified RAG + Skill + Tools bundle.

* [pg-perf-mcp](https://github.com/gouranshul/pg-perf-mcp) ⭐ 0 | 🐛 2 | 🌐 Java | 📅 2026-10-19 - Read-only MCP server that lets AI assistants diagnose PostgreSQL performance: slow queries, EXPLAIN plans, index advice, locks, and the queries inside database functions.

* [Pixelbolt](https://github.com/skulitom/pixelbolt-plugin) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-19 - Claude Code plugin for pixel art and sprite animation from editable JSON recipes, with particle and fluid effects, exported as PNG sprite sheets, GIF, APNG or video frames, locally with only Node.js 20+.

* [Plancast](https://github.com/sarthakdabhi/plancast) ⭐ 0 | 🐛 6 | 🌐 TypeScript | 📅 2026-10-11 - Local-first macOS CLI that helps developers and researchers turn Markdown, text, PDFs, and public articles into two-host audio briefings.

* [plori](https://github.com/plori-ai/codex-plugin) ⭐ 0 | 🐛 2 | 📅 2026-10-22 - Create and drive plori cloud agents (each an AI agent on its own cloud computer) over plori's remote MCP server, with OAuth auto-discovery.

* [Ratchet](https://github.com/baisethomas/Ratchet) ⭐ 0 | 🐛 1 | 🌐 Shell | 📅 2026-10-01 - Verification playbook and Claude Code plugin for coding agents at any capability tier: a model-agnostic AGENTS.md contract, a destructive-command guard, a stop gate that runs your checks before "done", and skills that reproduce a bug and prove its regression test can fail; the same skills load in Codex from `.agents/skills/`.

* [RestoSignals](https://github.com/paperandbeyond23-gif/restosignals-mcp) ⭐ 0 | 🐛 0 | 📅 2026-10-17 - Claude Code plugin and Agent Skill for the hosted RestoSignals MCP server: find US restaurants and bars 1-6 months before they open, scored from public liquor-license, food-permit and business filings, with owner contact (free API key).

* [Serply Agent Skills](https://github.com/serply-inc/skills) ⭐ 0 | 🐛 0 | 📅 2026-10-11 - Agent Skill and Claude Code plugin that teaches coding agents to pull live Google Search, Scholar, News, Maps, Jobs, Bing, Amazon and Reddit results and scrape URLs to markdown through the Serply API or its hosted MCP server.

* [Settled](https://github.com/justinedwardvolmer/settled-skill) ⭐ 0 | 🐛 4 | 🌐 Python | 📅 2026-10-24 - Agent skill and Claude Code plugin that checks an x402 endpoint against independent evidence (live probes, paid test purchases, on-chain payments) before an agent pays it.

* [Shipvela](https://github.com/stefanautomateed/shipvela-codex) ⭐ 0 | 🐛 1 | 📅 2026-10-05 - MIT client bundle for owner-confirmed static website and GitHub publishing through a proprietary, account-based hosting service with OAuth MCP, exact deployment tracking, and plan limits.

* [Shotbase](https://github.com/route1-ai/shotbase) ⭐ 0 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-19 - Self-hostable screenshot API and MCP server returning page screenshots plus structured data, with AI extraction running on your own model including a local Ollama so page content never leaves your network.

* [SolidPing](https://github.com/fclairamb/solidping-plugin) ⭐ 0 | 🐛 2 | 📅 2026-10-22 - Uptime monitoring plugin for Codex and Claude Code over the hosted SolidPing MCP server: checks across 40+ types, incidents, failure diagnosis and status pages, with every write confirmed first.

* [Statsnet MCP](https://github.com/usenetstate/statsnet-mcp) ⭐ 0 | 🐛 0 | 📅 2026-09-16 - Background check any company in the world: registration, executives, courts and finances. Remote MCP endpoint <https://statsnet.co/mcp>; registry id `io.github.usenetstate/statsnet`.

* [Storyflo](https://github.com/droplinked/storyflo-codex-plugin) ⭐ 0 | 🐛 1 | 📅 2026-09-12 - Agentic newsroom over a hosted MCP server with narrated briefings, a news-versus-prediction-market Divergence Index, and a searchable declassified archive.

* [Tanod](https://github.com/tanod-labs/tanod-mcp) ⭐ 0 | 🐛 3 | 🌐 TypeScript | 📅 2026-10-23 - Remote MCP server with 140+ pay-per-call tools for PDF, OCR, images, web pages and chain reads; free daily allowance, then x402 USDC on Base or Polygon.

* [Terraform Boundary](https://github.com/somesh-ghaturle/agentic-boundary-terraform-skills) ⭐ 0 | 🐛 1 | 🌐 Python | 📅 2026-10-20 - Claude Code, Codex, Cursor, and Windsurf skill that deploys AI agents on AWS, Azure, GCP, or Snowflake with Terraform while keeping a human in the loop: a hook blocks agent-run apply and destroy, only a human at a terminal can apply after typing the plan's fingerprint, and each change gets an evidence record for regulated-environment reviews.

* [TokRepo Search](https://github.com/henu-wang/tokrepo-codex-plugin) ⭐ 0 | 🐛 4 | 📅 2026-04-02 - Search and install AI assets from TokRepo with a bundled skill and MCP server for Codex.

* [VidSeeds.ai](https://github.com/CarrotGamesStudios/vidseeds-mcp) ⭐ 0 | 🐛 2 | 📅 2026-07-20 - Hosted MCP connector for pre-upload video SEO, metadata optimization, AI thumbnails, and multi-platform publishing with workflow skills for Codex agents.

* [VoiceMoat Skills](https://github.com/prateeks367/voicemoat-skills) ⭐ 0 | 🐛 0 | 📅 2026-10-04 - 26 Agent Skills for LinkedIn and Twitter/X posts that draft in your own voice, audit a post before you publish, fix weak openings, draft comments and replies, read your numbers and plan the week, for Claude Code, Codex and any client that reads SKILL.md.

* [vox](https://github.com/h1rdr3v2/vox-cli) ⭐ 0 | 🐛 5 | 🌐 Python | 📅 2026-10-19 - Local Whisper transcription and Kokoro text-to-speech for Apple Silicon Macs and Linux, served as an OpenAI-compatible audio API that every coding agent on the machine can share. <!-- platform: standalone -->

* [Yap MCP](https://github.com/founden-bot/yap-mcp) ⭐ 0 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-19 - MCP server: transcribes local audio and video files on your own computer for Claude Code, Cursor and other MCP clients, with on-device speech recognition, no upload and no API key.

* [Karma.Domains MCP](https://github.com/karma-domains/expired-domains-mcp) - MCP server: hosted Streamable HTTP server (OAuth or Pro API key) that searches 13M+ expired, auction, backorder and buy-now domains from 40 sources with Wayback Machine history, Karma Score and Ahrefs/Moz/Majestic metrics, plus live WHOIS, DNS, domain age and spam-score checks (closed source; paid Pro plan).

* [Mantis](./plugins/deonmenezes/mantishack) - Autonomous bug bounty hunter for authorized engagements — 7-phase FSM (RECON → AUTH → HUNT → CHAIN → VERIFY → GRADE → REPORT), parallel hunter sub-agents, cryptographic scope enforcement, and BLAKE3/Ed25519 Merkle event logs.

* [mcp-linker](https://github.com/milisp/mcp-linker) - MCP store to discover, add, and sync MCP server configuration across clients like Claude Code, Codex, and Cursor. <!-- platform: standalone -->

* [nsfw-ai-skill](https://github.com/Spicy-API/nsfw-ai-skill) - Agent Skill and Claude Code plugin for adult (18+) image, image-to-video and image-edit generation through the SpicyAPI API, with cost quotes before every run and adults-only / consent rules.

* [PDF Monster](https://github.com/jbaehova/pdf-monster) - Analyzes PDFs as extracted text, OCR text, rendered page images, and embedded figures for coding agents.

* [Token Harbor](https://github.com/NickHOI/Token-Harbor) - Turn Codex token usage into Sail Power for a local-first fishing, fleet, and harbor-building companion game.

### Grok Plugins

xAI Grok Build plugins can bundle skills, commands, agents, hooks, MCP servers,
and language-server configuration. A native plugin may include
`.grok-plugin/plugin.json`; install a repository with `grok plugin install
owner/repo --trust`. Add verified community plugins here in alphabetical order.
See the [official xAI plugin marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 309 | 🐛 1,067 | 🌐 Python | 📅 2026-10-25
and [Grok plugin guide](https://github.com/xai-org/grok-build/blob/main/crates/codegen/xai-grok-pager/docs/user-guide/09-plugins.md) ⭐ 27,545 | 🐛 0 | 🌐 Rust | 📅 2026-09-29
before submitting.

* [hypergrok-trading-desk](https://github.com/galleonlabs/hypergrok-trading-desk) ⭐ 193 | 🐛 0 | 🌐 Python | 📅 2026-10-25 - Seven-agent Hyperliquid trading desk roles and skills for Grok Bot that research, size, execute and review trades with user approval.
* [Grok Imagine Cinematic Studio](https://github.com/FineComputer14451/Grok-Imagine-Cinematic-Studio) ⭐ 34 | 🐛 5 | 🌐 Python | 📅 2026-10-24 - Independent multi-agent cinematic production suite (25 Role-Card agents, 64 skills, Production Bible workflow, Character DNA locking, native Grok Imagine Video 1.5 support) for Grok Build.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 7 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-20 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.
* [BlindOracle](https://github.com/craigmbrown/blindoracle-plugin) ⭐ 0 | 🐛 4 | 📅 2026-10-24 - Joins a Grok Bot or Grok Build agent to the BlindOracle agent marketplace with a free ERC-8004 passport, role-scoped MCP tools, counterparty-risk controls for buying or selling A2A, and two $0.01 settlement proofs anyone can verify.
* [ppl](https://github.com/ppl-crm/ppl-grok-plugin) ⭐ 0 | 🐛 0 | 📅 2026-10-12 - Connects Grok to ppl, a personal CRM for humans with AI agents, through its hosted MCP server at <https://withppl.com/mcp> (OAuth) for contacts, notes, reminders and relationship memory; free beta at <https://withppl.com/register>.

### Kimi Plugins

Kimi Code plugins package skills, agents, and MCP servers for the Kimi runtime.
Depending on the plugin version, a repository can expose `kimi.plugin.json` or
`.kimi-plugin/plugin.json`; install a GitHub repository with Kimi Code's
`/plugins install https://github.com/owner/repo` command. Add verified community
plugins here in alphabetical order. See the [official Kimi plugin documentation](https://github.com/MoonshotAI/kimi-code/blob/main/docs/en/customization/plugins.md) ⭐ 8,012 | 🐛 1,649 | 🌐 TypeScript | 📅 2026-10-25
before submitting.

* [deja](https://github.com/vshulcz/deja-vu) ⭐ 1,303 | 🐛 36 | 🌐 Go | 📅 2026-10-25 - Recalls the sessions the other coding agents on the machine already wrote to disk, including work from before it was installed, through MCP tools, a `/deja:recall` command and recall on every prompt.
* [CloudBase AI Toolkit](https://github.com/TencentCloudBase/CloudBase-AI-Toolkit) ⭐ 1,149 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - Backend for AI coding agents on Tencent CloudBase — database, auth, and functions via Plugin, Skills & MCP.
* [GoodMemory](https://github.com/hjqcan/GoodMemory) ⭐ 20 | 🐛 2 | 🌐 TypeScript | 📅 2026-10-20 - Local-first, auditable cross-session project memory for Kimi Code with scoped recall, traceable provenance, and approval-gated writes.
* [HTML/CSS to Image API](https://github.com/htmlcsstoimage/agent-plugins) ⭐ 7 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-20 - Let AI agents capture live website screenshots, render HTML/CSS and populate reusable templates as images or PDFs without managing a browser.

### DeepSeek Harness Plugins

DeepSeek Harness (DSH) plugins are Cordis modules or npm packages that expose a
`dsh.bundle` manifest and can be installed with `dsh plugin add`. Add verified
community plugins here in alphabetical order. See the [official DeepSeek Harness
plugin tutorial](https://github.com/deepseek-ai/deepseek-harness/blob/master/docs/cordis-tutorial/01-first-plugin.md) ⭐ 261,241 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-23
and the [`dsh-plugin` community topic](https://github.com/topics/dsh-plugin) before
submitting a repository.

* [dsh-deja](https://github.com/vshulcz/deja-vu) ⭐ 1,303 | 🐛 36 | 🌐 Go | 📅 2026-10-25 - Brings the session history of nineteen other coding agents into DeepSeek Harness: recall, session digest and per-file history tools over a local index, plus optional automatic recall.
* [dsh-blender-plugin](https://github.com/sixtysevenlf/dsh-blender-plugin) ⭐ 1,283 | 🐛 2 | 🌐 Python | 📅 2026-10-25 - DSH plugin that lets an AI model drive Blender over a direct TCP channel: viewport frames, custom-angle renders, Python execution, headless offload, and a judgment/acceptance layer (`blender_rt_plan`, 28 families / 183 ops).
* [dsh-vision-router](https://github.com/ysr666/dsh-vision-router) ⭐ 1,175 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-24 - Gives text-only DeepSeek Harness agents image understanding through a built-in no-key vision chain plus fourteen tools for Q\&A, grounding, OCR, crop, screenshots and pixel diff.
* [humanizer-ru](https://github.com/ilyautov/humanizer-ru) ⭐ 488 | 🐛 4 | 🌐 Python | 📅 2026-10-23 - Text-only `dsh.bundle` that mounts the humanizer-ru Agent Skill into DeepSeek Harness: rewrites Russian text to remove 64 markers of AI generation, with a corpus-calibrated scanner and audit mode; install with `dsh plugin --profile web add humanizer-ru` (npm) or `github:ilyautov/humanizer-ru`.
* [dsh-dream-skin](https://github.com/RevolutionLA/dsh-dream-skin) ⭐ 280 | 🐛 3 | 🌐 JavaScript | 📅 2026-10-25 - Skins DeepSeek Harness with 8 original Mirage glass-material presets, custom wallpapers (image URL, scheduled rotation, Bing daily), per-skin accent colour, shareable theme packs and a low-power mode for machines where blurred glass saturates the GPU; install with `dsh plugin --profile web add dsh-dream-skin`, works in the web UI and in third-party desktop clients.
* [dsh-config-manager](https://github.com/xiajiajun516/dsh-config-manager) ⭐ 240 | 🐛 5 | 🌐 TypeScript | 📅 2026-10-24 - Backup, restore, export, import, migrate and sync your complete DeepSeek Harness (DSH) configuration — settings, model providers, plugins, MCP servers, skills, agent presets and workspaces — and restore your whole environment on a new machine with one click.
* [dsh-mattpocock-skills-deck](https://github.com/FeatherHunter/dsh-mattpocock-skills-deck) ⭐ 232 | 🐛 89 | 🌐 TypeScript | 📅 2026-10-25 - DSH plugin that renders GitHub issues as a task board panel and bundles 25 mattpocock/skills for one-click loading.
* [Engramory](https://github.com/tinqiao-oss/engramory) ⭐ 195 | 🐛 3 | 🌐 Python | 📅 2026-09-24 - Curated, file-based long-term memory for DSH agents — plain markdown notes in one store shared across hosts, with the index size cap enforced as a monotonic `ctx.tools.guard()` refusal rather than a reminder. Install: `dsh plugin --profile <name> add dsh-engramory`.
* [dsh-opencode-palette](https://github.com/FeatherHunter/dsh-opencode-palette) ⭐ 75 | 🐛 23 | 🌐 HTML | 📅 2026-10-24 - Multi-theme engine for DSH Web with full support for all 38 opencode themes.
* [dsh-agent-team](https://github.com/Contexera/dsh-agent-team) ⭐ 72 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - DeepSeek Harness plugin providing persistent team agents with per-member memory, Channels, and durable Task Threads.
* [memory-eternal](https://github.com/EternalNight996/memory-eternal) ⭐ 64 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-24 - Memory plugin and MCP server for DeepSeek Harness that distills finished conversations into audited knowledge cards in a searchable local Markdown vault, with knowledge graph and review center.
* [dsh-prompt](https://github.com/FeatherHunter/dsh-prompt) ⭐ 62 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-25 - Prompt toolbox for DeepSeek Harness: preset and custom prompt templates with one-click insert into the conversation.
* [Vibe-Mathematics](https://github.com/ChongCyrus/Vibe-Mathematics) ⭐ 43 | 🐛 9 | 🌐 JavaScript | 📅 2026-10-25 - Plugin bundle installing four multi-agent math problem-solving and cross-verification agent presets into DeepSeek Harness.
* [dsh-whale-girl-pet](https://github.com/yanzwzz/dsh-whale-girl-pet) ⭐ 32 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-19 - Desktop pet plugin for the DeepSeek Harness web UI that reports task token usage, session and per-turn cost pills, and hourly spend dashboards.
* [dsh-im-companion](https://github.com/FeatherHunter/dsh-im-companion) ⭐ 30 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-25 - Workspace presence companion for dsh-im: see which workspaces have an assistant on duty and whether they are online.
* [dsh-plugin-hub](https://github.com/wingsky-1/dsh-plugin-hub) ⭐ 30 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-25 - Plugin collection for the DeepSeek Harness web GUI: task notifications, provider usage tracking, MCP management, and LAN access.
* [dsh-mcp-manager](https://github.com/hyqhyq3/dsh-mcp-manager) ⭐ 26 | 🐛 2 | 🌐 JavaScript | 📅 2026-10-23 - DeepSeek Harness plugin for managing OAuth PKCE and static-token HTTP MCP servers, local stdio processes, and per-workspace tool registration.
* [dsh-oh-my-claude](https://github.com/lcestou/dsh-oh-my-claude) ⭐ 18 | 🐛 0 | 🌐 TypeScript | 📅 2026-10-25 - Claude Code CLI as a native DeepSeek Harness provider: the logged-in `claude` binary does the work on its own subscription with no API key, with a live model list, per-session resume, approval relay, images, a memory/rewind/changes panel, and workspaces on remote SSH boxes.
* [dsh-mcp-tools](https://github.com/hxlog/dsh-mcp-tools) ⭐ 3 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-24 - MCP server manager for the DeepSeek Harness settings page: add streamable-HTTP or stdio MCP servers, paste Postman-style request headers, test connectivity, and toggle individual MCP tools so disabled ones never reach the model.
* [dsh-api-balance](https://github.com/Kihara777/dsh-api-balance) ⭐ 2 | 🐛 0 | 🌐 JavaScript | 📅 2026-10-23 - API usage-balance panel for DeepSeek Harness: adds a 「Usage / Balance」 tab to the webui usage ring showing the account balance and today / this-month / 30-day cost with charts, acquiring the platform token automatically from local browser sessions.
* [LocalForge](https://github.com/orfeomorello/dsh-localforge) ⭐ 1 | 🐛 9 | 🌐 TypeScript | 📅 2026-10-20 - LM Studio, Ollama, and vLLM adapter for DeepSeek Harness with live model discovery, auto-load, per-model concurrency limits, fallback chains, and Prometheus metrics.

### OpenCode Plugins

OpenCode plugins are npm packages or local directories registered in `opencode.json(c)` (`plugins`) and installed with `opencode plugin add`. Add verified community plugins here in alphabetical order. The catalog records the `opencode` platform with repository and documentation links and omits any manifest-URL `install_url`: OpenCode resolves packages through its own installer, so no client-specific install target applies.

* [opencode-cursor](https://github.com/Nomadcxx/opencode-cursor) ⭐ 714 | 🐛 10 | 🌐 TypeScript | 📅 2026-10-23 - OpenCode plugin for Cursor subscription models with streaming, thinking, tool calls, MCP support, and browser login through Cursor CLI or API-key authentication through the SDK.
* [opencode-goal-plugin](https://github.com/prevalentWare/opencode-goal-plugin) ⭐ 513 | 🐛 13 | 🌐 TypeScript | 📅 2026-10-23 - OpenCode plugin for persistent goals, completion evidence, and idle auto-continuation.
* [RTL\_OpenCode](https://github.com/programmer-1998/RTL_OpenCode) ⭐ 16 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-15 - OpenCode plugin that fixes bidirectional Persian, Arabic, and Hebrew text rendering with Unicode isolates, keeping code blocks and paths intact.
* [Azure DevOps PR Review](https://github.com/WTLAIB/opencode-azure-devops-pr-review-v2) ⭐ 2 | 🐛 1 | 🌐 JavaScript | 📅 2026-10-25 - OpenCode V2 plugin that reviews Azure DevOps Services pull requests from a URL without a local checkout, with separate verification in review/deep modes and comment previews.
* [LitOpenCode](https://github.com/wjgoarxiv/litopencode) ⭐ 2 | 🐛 9 | 🌐 JavaScript | 📅 2026-10-23 - OpenCode plans, builds, checks and records each lit task, so the next session picks up from a written handoff.
* [OpenCode Attention Inbox](https://github.com/YidiDev/opencode-attention-inbox) ⭐ 1 | 🐛 1 | 🌐 TypeScript | 📅 2026-10-25 - Independent OpenCode V2 TUI sidebar inbox for pending permissions, questions, and successful unread completions, with navigation-only session switching.

### ZCode Plugins & Localization

ZCode (Z.ai) ships its desktop UI with en-US/zh-CN dictionaries compiled into
`app.asar`; community packs add further locales on top of an installed app.
Add verified community localization packs and plugins here in alphabetical order.

* **[zcode-ru](https://github.com/warment/zcode-ru) ⭐ 4 | 🐛 1 | 🌐 JavaScript | 📅 2026-09-26** — Russian (ru-RU) localization pack for the ZCode desktop app (3.10.1): 5,018 UI strings (100% of the renderer corpus), third language in the selector with English fallback, one-command installer with backup/restore. MIT.

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

After scaffolding with `$plugin-creator`, use [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 995 | 🐛 100 | 🌐 Python | 📅 2026-10-25 as your quality gate before publishing, review, or distribution.

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

* [Awesome DeepSeek Harness Plugins](https://github.com/awesome-dsh-plugin/awesome-dsh-plugin) ⭐ 20,672 | 🐛 362 | 🌐 JavaScript | 📅 2026-10-25 - Community-maintained DSH plugin list and discovery reference.
* [Kimi Code](https://github.com/MoonshotAI/kimi-code) ⭐ 8,012 | 🐛 1,649 | 🌐 TypeScript | 📅 2026-10-25 - Official Kimi Code runtime and plugin documentation.
* [awesome-codex-plugins](https://github.com/hashgraph-online/awesome-codex-plugins) ⭐ 1,407 | 🐛 26 | 🌐 JavaScript | 📅 2026-10-25 - Codex-focused catalog that inspired this cross-platform list.
* [xAI Grok Plugin Marketplace](https://github.com/xai-org/plugin-marketplace) ⭐ 309 | 🐛 1,067 | 🌐 Python | 📅 2026-10-25 - Official Grok Build plugin marketplace and catalog format.
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

Every plugin in this list is automatically ingested by the [HOL Plugin Registry](https://hol.org/registry/plugins), which runs each through the [`plugin-scanner`](https://github.com/hashgraph-online/hol-guard) ⭐ 995 | 🐛 100 | 🌐 Python | 📅 2026-10-25 to produce a trust score and security analysis.

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

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-10-25._
