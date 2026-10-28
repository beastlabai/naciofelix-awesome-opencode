<div align="center">THIS IS A WORK IN PROGRESS, EXPECT REGULAR UPDATES </div>

<div align="center">

<img src="https://raw.githubusercontent.com/anomalyco/opencode/dev/packages/console/app/src/asset/logo-ornate-light.svg" alt="OpenCode" width="100">

<br>
<br>

# Awesome OpenCode

**The definitive curated collection of everything OpenCode.**

Plugins · Projects · Integrations · Providers · MCP Servers · Skills · Resources

<br>

[![GitHub Stars](https://img.shields.io/github/stars/anomalyco/opencode?style=flat-square&logo=github&logoColor=white&label=OpenCode&color=181717)](https://github.com/anomalyco/opencode)
[![Discord](https://img.shields.io/discord/1391832426048651334?style=flat-square&logo=discord&logoColor=white&color=5865F2&label=Discord)](https://opencode.ai/discord)
[![License](https://img.shields.io/badge/CC0--1.0-blue?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square)](CONTRIBUTING.md)

<br>

<table>
<tr>
<td align="center"><strong>160K+</strong><br><sub>GitHub Stars</sub></td>
<td align="center"><strong>900+</strong><br><sub>Contributors</sub></td>
<td align="center"><strong>7.5M+</strong><br><sub>Monthly Devs</sub></td>
<td align="center"><strong>75+</strong><br><sub>LLM Providers</sub></td>
</tr>
</table>

<br>

</div>

---

## Contents

- [Quick Start](#quick-start)
- [Features at a Glance](#features-at-a-glance)
- [Plugins](#plugins)
- [Projects & Integrations](#projects--integrations)
- [Agent Collections](#agent-collections)
- [LLM Providers](#llm-providers)
- [MCP Servers](#mcp-servers)
- [Agent Skills](#agent-skills)
- [Themes & UI](#themes--ui)
- [Editor Integrations](#editor-integrations)
- [SDK & Development](#sdk--development)
- [Guides & Tutorials](#guides--tutorials)
- [Community & Resources](#community--resources)
- [Contributing](#contributing)

---

## Quick Start

```bash
curl -fsSL https://opencode.ai/install | bash
```

Or use your preferred package manager:

| Manager | Command |
|:---|:---|
| **npm** | `npm i -g opencode-ai@latest` |
| **Homebrew** | `brew install anomalyco/tap/opencode` |
| **Scoop** | `scoop install opencode` |
| **Arch** | `sudo pacman -S opencode` |
| **mise** | `mise use -g opencode` |

OpenCode is also available as a **[Desktop App (Beta)](https://opencode.ai/download)** for macOS, Windows, and Linux.

---

## Features at a Glance

| | Feature | Description |
|:---|:---|:---|
| ⚡ | **LSP Enabled** | Automatically loads the right LSPs for the LLM |
| 🔄 | **Multi-Session** | Start multiple agents in parallel on the same project |
| 🔗 | **Share Links** | Share a link to any session for reference or debugging |
| 🐙 | **GitHub Copilot** | Log in with GitHub to use your Copilot account |
| 🤖 | **ChatGPT Plus/Pro** | Log in with OpenAI to use your ChatGPT subscription |
| 🧠 | **Any Model** | 75+ LLM providers through Models.dev, including local models |
| 🖥️ | **Any Editor** | Terminal interface, desktop app, and IDE extension |
| 🛠️ | **Agent Skills** | Reusable, loadable SKILL.md definitions for specialized behavior |
| 🔌 | **MCP Servers** | Connect external tools via Model Context Protocol |
| 🔒 | **Privacy First** | No code or context data stored — works in sensitive environments |

---

## Plugins

> Extend OpenCode with community-built plugins. Add them to your `opencode.json` under the `"plugin"` key.

<details>
<summary><strong>Authentication & Access</strong></summary>
<br>

| Plugin | Description |
|:---|:---|
| [opencode-openai-codex-auth](https://github.com/numman-ali/opencode-openai-codex-auth) | Use your ChatGPT Plus/Pro subscription instead of API credits |
| [opencode-gemini-auth](https://github.com/jenslys/opencode-gemini-auth) | Use your existing Gemini plan instead of API billing |
| [opencode-antigravity-auth](https://github.com/NoeFabris/opencode-antigravity-auth) | Use Antigravity's free models instead of API billing |
| [opencode-google-antigravity-auth](https://github.com/shekohex/opencode-google-antigravity-auth) | Google Antigravity OAuth with search and robust API handling |

</details>

<details>
<summary><strong>Developer Experience</strong></summary>
<br>

| Plugin | Description |
|:---|:---|
| [opencode-notificator](https://github.com/panta82/opencode-notificator) | Desktop notifications and sound alerts for OpenCode sessions |
| [opencode-notifier](https://github.com/mohak34/opencode-notifier) | Desktop notifications for permission, completion, and error events |
| [opencode-notify](https://github.com/kdcokenny/opencode-notify) | Native OS notifications — know when tasks complete |
| [opencode-zellij-namer](https://github.com/24601/opencode-zellij-namer) | AI-powered automatic Zellij session naming |
| [opencode-wakatime](https://github.com/angristan/opencode-wakatime) | Track OpenCode usage with WakaTime |
| [opencode-sentry-monitor](https://github.com/stolinski/opencode-sentry-monitor) | Trace and debug AI agents with Sentry AI Monitoring |

</details>

<details>
<summary><strong>Code Intelligence</strong></summary>
<br>

| Plugin | Description |
|:---|:---|
| [opencode-type-inject](https://github.com/nick-vi/opencode-type-inject) | Auto-inject TypeScript/Svelte types into file reads |
| [opencode-md-table-formatter](https://github.com/franlol/opencode-md-table-formatter) | Clean up markdown tables produced by LLMs |
| [opencode-morph-fast-apply](https://github.com/JRedeker/opencode-morph-fast-apply) | 10x faster code editing with Morph Fast Apply API |
| [opencode-morph-plugin](https://github.com/morphllm/opencode-morph-plugin) | Fast Apply, WarpGrep codebase search, and context compaction |
| [oh-my-opencode](https://github.com/code-yeongyu/oh-my-opencode) | Background agents, pre-built LSP/AST/MCP tools, curated agents |

</details>

<details>
<summary><strong>Context & Memory</strong></summary>
<br>

| Plugin | Description |
|:---|:---|
| [opencode-dynamic-context-pruning](https://github.com/Tarquinen/opencode-dynamic-context-pruning) | Optimize token usage by pruning obsolete tool outputs |
| [opencode-vibeguard](https://github.com/inkdust2021/opencode-vibeguard) | Redact secrets/PII before LLM calls; restore locally |
| [opencode-supermemory](https://github.com/supermemoryai/opencode-supermemory) | Persistent memory across sessions using Supermemory |
| [opencode-skillful](https://github.com/zenobi-us/opencode-skillful) | Lazy load prompts on demand with skill discovery and injection |

</details>

<details>
<summary><strong>Workflow & Automation</strong></summary>
<br>

| Plugin | Description |
|:---|:---|
| [opencode-daytona](https://github.com/daytonaio/daytona/tree/main/libs/opencode-plugin) | Run sessions in isolated Daytona sandboxes with live previews |
| [opencode-devcontainers](https://github.com/athal7/opencode-devcontainers) | Multi-branch devcontainer isolation with shallow clones |
| [opencode-pty](https://github.com/shekohex/opencode-pty) | Run background processes in a PTY with interactive input |
| [opencode-shell-strategy](https://github.com/JRedeker/opencode-shell-strategy) | Prevents hangs from TTY-dependent operations |
| [opencode-helicone-session](https://github.com/H2Shami/opencode-helicone-session) | Inject Helicone session headers for request grouping |
| [opencode-firecrawl](https://github.com/firecrawl/opencode-firecrawl) | Web scraping, crawling, and search via Firecrawl CLI |
| [opencode-jfrog-plugin](https://github.com/jfrog/opencode-jfrog-plugin) | Seamless JFrog platform integration |
| [opencode-websearch-cited](https://github.com/ghoulr/opencode-websearch-cited) | Native websearch with Google grounded-style citations |
| [opencode-worktree](https://github.com/kdcokenny/opencode-worktree) | Zero-friction git worktrees for OpenCode |
| [opencode-scheduler](https://github.com/different-ai/opencode-scheduler) | Schedule recurring jobs with cron syntax |

</details>

<details>
<summary><strong>Orchestration & Planning</strong></summary>
<br>

| Plugin | Description |
|:---|:---|
| [opencode-conductor](https://github.com/derekbar90/opencode-conductor) | Protocol-driven Context → Spec → Plan → Implement lifecycle |
| [opencode-multi-llm](https://github.com/beastlabai/multi-llm-plugin) | Parallel plan, code, and commit reviews across 19 coding CLIs, with validated findings, task generation, implementation, and automated revision. |
| [opencode-background-agents](https://github.com/kdcokenny/opencode-background-agents) | Claude Code-style background agents with async delegation |
| [opencode-workspace](https://github.com/kdcokenny/opencode-workspace) | Multi-agent orchestration harness — 16 components, one install |
| [@plannotator/opencode](https://github.com/backnotprop/plannotator/tree/main/apps/opencode-plugin) | Interactive plan review with visual annotation |
| [@openspoon/subtask2](https://github.com/spoons-and-mirrors/subtask2) | Extend /commands into a powerful orchestration system |
| [micode](https://github.com/vtemian/micode) | Structured Brainstorm → Plan → Implement workflow |
| [octto](https://github.com/vtemian/octto) | Interactive browser UI for AI brainstorming |
| [ocx](https://github.com/kdcokenny/ocx) | OpenCode extension manager with portable, isolated profiles |

</details>

---

## Projects & Integrations

> Community-built tools and integrations that work with OpenCode.

| Project | Description |
|:---|:---|
| [OpenChamber](https://github.com/btriapitsyn/openchamber) | Web / Desktop App and VS Code Extension for OpenCode |
| [OpenWork](https://github.com/different-ai/openwork) | Open-source alternative to Claude Cowork, powered by OpenCode |
| [CodeNomad](https://github.com/NeuralNomadsAI/CodeNomad) | Desktop, Web, Mobile and Remote Client App for OpenCode |
| [portal](https://github.com/hosenur/portal) | Mobile-first web UI for OpenCode over Tailscale/VPN |
| [kimaki](https://github.com/remorses/kimaki) | Discord bot to control OpenCode sessions via SDK |
| [OpenCode-Obsidian](https://github.com/mtymek/opencode-obsidian) | Obsidian plugin that embeds OpenCode in Obsidian's UI |
| [ai-sdk-provider-opencode-sdk](https://github.com/ben-vargas/ai-sdk-provider-opencode-sdk) | Vercel AI SDK provider for using OpenCode via `@opencode-ai/sdk` |
| [opencode plugin template](https://github.com/zenobi-us/opencode-plugin-template) | Template for building OpenCode plugins |

---

## Agent Collections

> Pre-configured agents and agent frameworks for specialized workflows.

| Agent | Description |
|:---|:---|
| [Agentic](https://github.com/Cluster444/agentic) | Modular AI agents and commands for structured development |
| [opencode-agents](https://github.com/darrenhinde/opencode-agents) | Configs, prompts, agents, and plugins for enhanced workflows |

---

## LLM Providers

> OpenCode supports **75+ LLM providers** via [Models.dev](https://models.dev).

<details>
<summary><strong>Cloud Providers</strong></summary>
<br>

| Provider | Highlights |
|:---|:---|
| [OpenAI](https://opencode.ai/docs/providers/#openai) | ChatGPT Plus/Pro login or API keys |
| [Anthropic](https://opencode.ai/docs/providers/#anthropic) | Claude models with OAuth |
| [GitHub Copilot](https://opencode.ai/docs/providers/#github-copilot) | Use your Copilot subscription |
| [Google Vertex AI](https://opencode.ai/docs/providers/#google-vertex-ai) | Gemini models via GCP |
| [Amazon Bedrock](https://opencode.ai/docs/providers/#amazon-bedrock) | Multi-provider via AWS |
| [Azure OpenAI](https://opencode.ai/docs/providers/#azure-openai) | OpenAI models on Azure |
| [xAI](https://opencode.ai/docs/providers/#xai) | Grok models |
| [DeepSeek](https://opencode.ai/docs/providers/#deepseek) | DeepSeek V4 Pro |

</details>

<details>
<summary><strong>Aggregators & Gateways</strong></summary>
<br>

| Provider | Highlights |
|:---|:---|
| [OpenCode Zen](https://opencode.ai/docs/zen) | Curated, tested models by the OpenCode team |
| [OpenRouter](https://opencode.ai/docs/providers/#openrouter) | Access models from many providers |
| [OpenCode Go](https://opencode.ai/docs/go) | Low-cost subscription for popular models |
| [Helicone](https://opencode.ai/docs/providers/#helicone) | LLM observability + gateway |
| [Cloudflare AI Gateway](https://opencode.ai/docs/providers/#cloudflare-ai-gateway) | Unified endpoint, no separate API keys |

</details>

<details>
<summary><strong>Fast Inference</strong></summary>
<br>

| Provider | Highlights |
|:---|:---|
| [Groq](https://opencode.ai/docs/providers/#groq) | Ultra-fast LPU inference |
| [Cerebras](https://opencode.ai/docs/providers/#cerebras) | Wafer-scale inference engine |
| [Fireworks AI](https://opencode.ai/docs/providers/#fireworks-ai) | Fast open model inference |
| [Together AI](https://opencode.ai/docs/providers/#together-ai) | Open model hosting |

</details>

<details>
<summary><strong>Local & Self-Hosted</strong></summary>
<br>

| Provider | Highlights |
|:---|:---|
| [Ollama](https://opencode.ai/docs/providers/#ollama) | Run models locally with ease |
| [LM Studio](https://opencode.ai/docs/providers/#lm-studio) | Local model management |
| [llama.cpp](https://opencode.ai/docs/providers/#llamacpp) | Direct llama-server integration |
| [Hugging Face](https://opencode.ai/docs/providers/#hugging-face) | 17+ inference providers |

</details>

<details>
<summary><strong>View all 75+ providers</strong></summary>
<br>

302.AI · Amazon Bedrock · Anthropic · Atomic Chat · Azure OpenAI · Azure Cognitive Services · Baseten · Cerebras · Cloudflare AI Gateway · Cloudflare Workers AI · Cortecs · DeepSeek · Deep Infra · DigitalOcean · FrogBot · Fireworks AI · GitLab Duo · GitHub Copilot · Google Vertex AI · Groq · Hugging Face · Helicone · llama.cpp · IO.NET · LM Studio · Moonshot AI · MiniMax · NVIDIA · Nebius Token Factory · Ollama · Ollama Cloud · OpenAI · OpenCode Zen · OpenRouter · LLM Gateway · SAP AI Core · STACKIT · OVHcloud AI Endpoints · Scaleway · Together AI · Venice AI · Vercel AI Gateway · xAI · Z.AI · ZenMux

</details>

---

## MCP Servers

> Connect external tools to OpenCode via the [Model Context Protocol](https://opencode.ai/docs/mcp-servers/).

| Server | Description | Type |
|:---|:---|:---|
| [Sentry](https://mcp.sentry.dev) | Query Sentry issues, projects, and errors | Remote (OAuth) |
| [Context7](https://github.com/upstash/context7) | Search through documentation | Remote |
| [Grep by Vercel](https://grep.app) | Search code snippets on GitHub | Remote |

**Adding an MCP Server:**

```jsonc
{
  "$schema": "https://opencode.ai/config.json",
  "mcp": {
    "context7": {
      "type": "remote",
      "url": "https://mcp.context7.com/mcp"
    },
    "my-local-tool": {
      "type": "local",
      "command": ["npx", "-y", "my-mcp-command"]
    }
  }
}
```

---

## Agent Skills

> Reusable behavior definitions loaded on-demand via `SKILL.md` files. [Learn more](https://opencode.ai/docs/skills/).

Skills can be placed in:

- `.opencode/skills/<name>/SKILL.md` — project-level
- `~/.config/opencode/skills/<name>/SKILL.md` — global
- `.claude/skills/<name>/SKILL.md` — Claude-compatible
- `.agents/skills/<name>/SKILL.md` — agent-compatible

```markdown
---
name: git-release
description: Create consistent releases and changelogs
---

## What I do
- Draft release notes from merged PRs
- Propose a version bump
- Provide a copy-pasteable `gh release create` command
```

Browse the [opencode.ai/docs/ecosystem](https://opencode.ai/docs/ecosystem/) for community skills and agent configs.

---

## Themes & UI

> OpenCode ships with a beautiful TUI and supports custom themes. [Learn more](https://opencode.ai/docs/themes/).

Configure themes in your `opencode.json` or pick from built-in options. OpenCode also features:

- **Keyboard-driven interface** with customizable [keybinds](https://opencode.ai/docs/keybinds/)
- **Tab switching** between Build and Plan agents
- **Image support** — drag and drop images into the terminal
- **File fuzzy search** with the `@` key
- **Undo/Redo** with `/undo` and `/redo` commands

---

## Editor Integrations

| Editor | Integration |
|:---|:---|
| **VS Code** | Built-in IDE extension — [docs](https://opencode.ai/docs/ide/) |
| **Neovim** | [opencode.nvim](https://github.com/NickvanDyke/opencode.nvim) — editor-aware prompts |
| **Neovim (alt)** | [opencode.nvim](https://github.com/sudo-tee/opencode.nvim) — terminal frontend |
| **Obsidian** | [OpenCode-Obsidian](https://github.com/mtymek/opencode-obsidian) — embedded UI |
| **Zellij** | [opencode-zellij-namer](https://github.com/24601/opencode-zellij-namer) — auto session naming |

---

## SDK & Development

> Build on top of OpenCode with the official SDK, Server API, and Plugin system.

| Resource | Description |
|:---|:---|
| [SDK](https://opencode.ai/docs/sdk/) | TypeScript SDK for programmatic access |
| [Server](https://opencode.ai/docs/server/) | Run OpenCode as a server |
| [Plugins](https://opencode.ai/docs/plugins/) | Plugin development guide |
| [Custom Tools](https://opencode.ai/docs/custom-tools/) | Define your own tools |
| [Config Reference](https://opencode.ai/docs/config/) | Full configuration documentation |

---

## Guides & Tutorials

### Official Documentation

| Guide | Link |
|:---|:---|
| Getting Started | [opencode.ai/docs](https://opencode.ai/docs/) |
| Configuration | [opencode.ai/docs/config](https://opencode.ai/docs/config/) |
| Agents | [opencode.ai/docs/agents](https://opencode.ai/docs/agents/) |
| Tools | [opencode.ai/docs/tools](https://opencode.ai/docs/tools/) |
| Rules (AGENTS.md) | [opencode.ai/docs/rules](https://opencode.ai/docs/rules/) |
| Models | [opencode.ai/docs/models](https://opencode.ai/docs/models/) |
| Permissions | [opencode.ai/docs/permissions](https://opencode.ai/docs/permissions/) |
| Formatters | [opencode.ai/docs/formatters](https://opencode.ai/docs/formatters/) |
| Commands | [opencode.ai/docs/commands](https://opencode.ai/docs/commands/) |
| Troubleshooting | [opencode.ai/docs/troubleshooting](https://opencode.ai/docs/troubleshooting/) |

### Essential Commands

| Command | Description |
|:---|:---|
| `/init` | Initialize OpenCode for a project (generates `AGENTS.md`) |
| `/connect` | Configure LLM provider API keys |
| `/models` | Select and switch between models |
| `/share` | Create a shareable link to the current conversation |
| `/undo` | Undo the last set of changes |
| `/redo` | Redo previously undone changes |
| `Tab` | Switch between Build and Plan agents |
| `@` | Fuzzy search for files in the project |

---

## Community & Resources

| Resource | Link |
|:---|:---|
| **GitHub** | [github.com/anomalyco/opencode](https://github.com/anomalyco/opencode) |
| **Documentation** | [opencode.ai/docs](https://opencode.ai/docs/) |
| **Discord** | [opencode.ai/discord](https://opencode.ai/discord) |
| **X (Twitter)** | [x.com/opencode](https://x.com/opencode) |
| **Ecosystem** | [opencode.ai/docs/ecosystem](https://opencode.ai/docs/ecosystem/) |
| **opencode.cafe** | [opencode.cafe](https://opencode.cafe) — Community aggregator |
| **Changelog** | [opencode.ai/changelog](https://opencode.ai/changelog) |
| **Enterprise** | [opencode.ai/enterprise](https://opencode.ai/enterprise/) |

---

## Contributing

Contributions are welcome! To add a project, plugin, or resource:

1. Fork this repository
2. Add your entry to the appropriate section
3. Keep descriptions concise (one line)
4. Open a pull request

Please ensure your addition is relevant to the OpenCode ecosystem. If your project uses "opencode" in its name, please add a note to your README clarifying it is not affiliated with the OpenCode team.

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

---

<div align="center">

**[OpenCode](https://opencode.ai)** · Built by [Anomaly](https://anoma.ly)

</div>
