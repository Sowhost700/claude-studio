<div align="center">

```
 ██████╗██╗      █████╗ ██╗   ██╗██████╗ ███████╗    ███████╗████████╗██╗   ██╗██████╗ ██╗ ██████╗ 
██╔════╝██║     ██╔══██╗██║   ██║██╔══██╗██╔════╝    ██╔════╝╚══██╔══╝██║   ██║██╔══██╗██║██╔═══██╗
██║     ██║     ███████║██║   ██║██║  ██║█████╗      ███████╗   ██║   ██║   ██║██║  ██║██║██║   ██║
██║     ██║     ██╔══██║██║   ██║██║  ██║██╔══╝      ╚════██║   ██║   ██║   ██║██║  ██║██║██║   ██║
╚██████╗███████╗██║  ██║╚██████╔╝██████╔╝███████╗    ███████║   ██║   ╚██████╔╝██████╔╝██║╚██████╔╝
 ╚═════╝╚══════╝╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚══════╝    ╚══════╝   ╚═╝    ╚═════╝ ╚═════╝ ╚═╝ ╚═════╝
```

**The unified Claude AI development stack. Six tools. One repo. Zero compromise.**

[![MIT License](https://img.shields.io/badge/License-MIT-white?style=flat-square&labelColor=000000&color=ffffff)](LICENSE)
[![Built by SLIME](https://img.shields.io/badge/Built%20by-er4700345--coder-white?style=flat-square&labelColor=000000&color=ffffff)](https://github.com/er4700345-coder)
[![Stack](https://img.shields.io/badge/Stack-Claude%20%2B%20AI%20Agents-white?style=flat-square&labelColor=000000&color=ffffff)](https://github.com/er4700345-coder/claude-studio)
[![Stars](https://img.shields.io/github/stars/er4700345-coder/claude-studio?style=flat-square&labelColor=000000&color=ffffff)](https://github.com/er4700345-coder/claude-studio/stargazers)

---

</div>

## WHAT IS THIS

> Claude Studio is not another AI wrapper. It is an **opinionated, production-ready stack** that turns Claude into a full autonomous development environment — with planning, memory, design intelligence, browser control, automation, and performance optimization all wired together as one system.

Six of the most powerful Claude-adjacent repos on GitHub — curated, integrated, documented, and ready to run.

---

## THE STACK

<table>
<tr>
<td width="50%" valign="top">

### `01` — SUPERPOWERS
**github.com/obra/superpowers**

> Makes Claude plan before it codes.

Runs a full research → spec → plan → test → build loop. Your agent stops guessing and starts thinking like a senior dev.

`122k ⭐` &nbsp; `10k forks` &nbsp; `MIT`

</td>
<td width="50%" valign="top">

### `02` — EVERYTHING-CLAUDE-CODE
**github.com/affaan-m/everything-claude-code**

> Full performance system for Claude Code.

Better context handling, faster task execution, pre-built skills — all in one package. The engine room.

`116k ⭐` &nbsp; `15.1k forks` &nbsp; `MIT`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### `03` — UI UX PRO MAX
**github.com/nextlevelbuilder/ui-ux-pro-max-skill**

> Design intelligence for Claude.

Forces a real design direction before any code gets written — typography, color systems, animations. Intentional, every time.

`54k ⭐` &nbsp; `5.2k forks` &nbsp; `MIT`

</td>
<td width="50%" valign="top">

### `04` — BROWSER-USE
**github.com/browser-use/browser-use**

> Claude controls a real browser.

Click buttons. Fill forms. Take screenshots. Run parallel sessions. No API? Claude goes in directly.

`84.9k ⭐` &nbsp; `9.8k forks` &nbsp; `MIT`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### `05` — CLAUDE-MEM
**github.com/thedotmack/claude-mem**

> Persistent memory across sessions.

Stop re-explaining your project every new chat. Claude-mem captures everything, compresses it with AI, injects it back on next session.

`42.3k ⭐` &nbsp; `3.2k forks`

</td>
<td width="50%" valign="top">

### `06` — N8N-MCP
**github.com/czlonkowski/n8n-mcp**

> Claude Code meets n8n automation.

Claude doesn't just write workflows — it tests and validates them. Backend automation with actual feedback loops.

`16.9k ⭐` &nbsp; `2.9k forks` &nbsp; `MIT`

</td>
</tr>
</table>

---

## HOW IT ALL FITS TOGETHER

```
┌─────────────────────────────────────────────────────────┐
│                    CLAUDE STUDIO                        │
│                                                         │
│  ┌─────────────┐        ┌─────────────────────────┐    │
│  │ SUPERPOWERS │───────▶│  EVERYTHING-CLAUDE-CODE │    │
│  │  (PLANNER)  │        │      (PERFORMANCE)      │    │
│  └─────────────┘        └───────────┬─────────────┘    │
│                                     │                   │
│         ┌───────────────────────────┼──────────────┐   │
│         ▼                           ▼              ▼   │
│  ┌─────────────┐        ┌──────────────┐  ┌──────────┐ │
│  │ UI UX PRO   │        │  BROWSER-USE │  │  N8N-MCP │ │
│  │    MAX      │        │  (WEB AGENT) │  │ (AUTOMAT)│ │
│  │  (DESIGN)   │        └──────────────┘  └──────────┘ │
│  └─────────────┘                                        │
│                                                         │
│  ┌──────────────────────────────────────────────────┐  │
│  │                   CLAUDE-MEM                     │  │
│  │              (MEMORY — RUNS UNDER ALL)           │  │
│  └──────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────┘
```

---

## QUICK START

```bash
# 1. Clone Claude Studio
git clone https://github.com/er4700345-coder/claude-studio
cd claude-studio

# 2. Init submodules (all 6 tools)
git submodule update --init --recursive

# 3. Follow individual setup per module
# Each tool has its own /docs — see below
```

---

## REPO STRUCTURE

```
claude-studio/
├── README.md
├── modules/
│   ├── superpowers/          → github.com/obra/superpowers
│   ├── everything-claude/    → github.com/affaan-m/everything-claude-code
│   ├── ui-ux-pro-max/        → github.com/nextlevelbuilder/ui-ux-pro-max-skill
│   ├── browser-use/          → github.com/browser-use/browser-use
│   ├── claude-mem/           → github.com/thedotmack/claude-mem
│   └── n8n-mcp/              → github.com/czlonkowski/n8n-mcp
├── docs/
│   ├── SETUP.md
│   ├── ARCHITECTURE.md
│   └── USE_CASES.md
└── .gitmodules
```

---

## USE CASES

| Goal | Modules Used |
|---|---|
| Build a full-stack app from scratch | Superpowers + Everything-Claude-Code + UI UX Pro Max |
| Automate a website workflow (no API) | Browser-use + n8n-MCP |
| Never lose context across sessions | Claude-mem (always on) |
| Spin up a designed UI fast | UI UX Pro Max + Everything-Claude-Code |
| Full autonomous dev agent loop | All 6 |

---

## .gitmodules

```ini
[submodule "modules/superpowers"]
	path = modules/superpowers
	url = https://github.com/obra/superpowers

[submodule "modules/everything-claude"]
	path = modules/everything-claude
	url = https://github.com/affaan-m/everything-claude-code

[submodule "modules/ui-ux-pro-max"]
	path = modules/ui-ux-pro-max
	url = https://github.com/nextlevelbuilder/ui-ux-pro-max-skill

[submodule "modules/browser-use"]
	path = modules/browser-use
	url = https://github.com/browser-use/browser-use

[submodule "modules/claude-mem"]
	path = modules/claude-mem
	url = https://github.com/thedotmack/claude-mem

[submodule "modules/n8n-mcp"]
	path = modules/n8n-mcp
	url = https://github.com/czlonkowski/n8n-mcp
```

---

## CONTRIBUTING

This is a living stack. If a better tool drops, it gets swapped in. PRs welcome — but the bar is high.

---

<div align="center">

**Built by [er4700345-coder](https://github.com/er4700345-coder)**

`Claude Studio` — Because one tool was never enough.

</div>
