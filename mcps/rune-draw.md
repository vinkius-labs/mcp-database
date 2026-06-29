# Rune Draw MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rune-draw)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [games](../categories/games.md)

An Elder Futhark divination engine for single, three, or five-rune readings.

## Description
Connect your AI agent to the ancient wisdom of the Elder Futhark. This MCP server provides a powerful engine for runic divination, allowing for single-rune omens, three-rune readings (Past, Present, Future), and complex five-rune spreads. Using `single_draw`, `multi_draw`, and `rune_metadata` tools, your agent can interpret the cosmic forces of the 24 runes plus the mysterious Void rune. Each draw includes orientation (upright or reversed) to provide deep, nuanced interpretations.


## Available Tools (3)
- **multi_draw**: Perform a multi-rune reading
- **rune_metadata**: Get metadata for a specific rune
- **single_draw**: Perform a single rune draw


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rune Draw** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a single rune reading for my day."

**🤖 AI Agent:**
> Your rune for today is Fehu (upright), representing wealth, prosperity, and new beginnings.

---

**👤 You:**
> "Perform a three-rune reading about my future career path."

**🤖 AI Agent:**
> Your reading shows: 1. Ansuz (upright) - communication and wisdom; 2. Isa (reversed) - stagnation or delays; 3. Jera (upright) - harvest and successful results.

---

**👤 You:**
> "What does the rune 'Thurisaz' mean?"

**🤖 AI Agent:**
> Thurisaz represents a thorn or giant, symbolizing reactive force, protection, and conflict.


## ❓ FAQ

**Q: What runes are included in the draw?**
The engine uses the 24 runes of the Elder Futhark plus a special 'Void' rune representing potentiality.

**Q: How do I perform a three-rune reading?**
Use the `multi_draw` tool and set the `count` parameter to '3'.

**Q: Can I look up specific rune meanings?**
Yes, you can use the `rune_metadata` tool to retrieve linguistic and symbolic properties for any rune.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rune-draw](https://vinkius.com/mcp/rune-draw)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rune Draw** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rune-draw` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rune Draw** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rune-draw": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
