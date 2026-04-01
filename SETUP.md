# SETUP GUIDE — CLAUDE STUDIO

## Prerequisites

- Claude Code installed (`npm install -g @anthropic-ai/claude-code`)
- Python 3.10+ (for browser-use + claude-mem)
- Node.js 18+ (for n8n-MCP)
- n8n instance (self-hosted or cloud) — only if using module 06

---

## Step 1 — Clone with submodules

```bash
git clone --recurse-submodules https://github.com/er4700345-coder/claude-studio
cd claude-studio
```

Or if already cloned:

```bash
git submodule update --init --recursive
```

---

## Step 2 — Module Setup

### 01 · Superpowers
```bash
cd modules/superpowers
# Follow: https://github.com/obra/superpowers
```

### 02 · Everything-Claude-Code
```bash
cd modules/everything-claude
# Follow: https://github.com/affaan-m/everything-claude-code
```

### 03 · UI UX Pro Max
```bash
cd modules/ui-ux-pro-max
# Follow: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill
```

### 04 · Browser-use
```bash
cd modules/browser-use
pip install browser-use
playwright install
# Follow: https://github.com/browser-use/browser-use
```

### 05 · Claude-mem
```bash
cd modules/claude-mem
# Follow: https://github.com/thedotmack/claude-mem
```

### 06 · n8n-MCP
```bash
cd modules/n8n-mcp
npm install
# Set N8N_URL and N8N_API_KEY in .env
# Follow: https://github.com/czlonkowski/n8n-mcp
```

---

## Step 3 — Run

Each module runs independently inside Claude Code.
Point Claude Code at whichever module you want active,
or run all via your own orchestration layer.
