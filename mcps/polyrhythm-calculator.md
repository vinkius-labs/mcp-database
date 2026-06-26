# Polyrhythm Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polyrhythm-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise alignment, attack timestamps, and subdivision grids for complex polyrhythms.

## Description
The Polyrhythm Calculator is a precision engine designed to bridge the gap between musical intuition and mathematical accuracy. It allows you to analyze multi-layered rhythmic patterns by calculating exactly when different rhythms coincide. Using tools like `find_sync_point`, you can determine the exact pulse where all layers align, or use `get_layer_attacks` to find precise millisecond timestamps for every note in a sequence. Whether you are working with simple duple rhythms or complex polyphonic structures, this MCP provides the temporal data needed for perfect rhythmic programming and composition.


## Available Tools (4)
- **get_grid_resolution**: Calculates the minimum subdivision grid resolution
- **get_layer_attacks**: Calculates attack timestamps for each layer
- **find_sync_point**: Finds the sync point for a polyrhythm
- **get_rhythm_complexity**: Determines the complexity of a rhythm pattern


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polyrhythm Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "At what pulse does a 3:4 polyrhythm reset?"

**🤖 AI Agent:**
> A 3:4 polyrhythm reaches its alignment point at pulse 12, which marks the completion of one full rhythmic cycle.

---

**👤 You:**
> "Give me the attack timestamps for a 2:3 rhythm at 120 BPM for 1 measure."

**🤖 AI Agent:**
> At 120 BPM, the attacks for layer 0 occur at 0.0ms and 500.0ms, while layer 1 attacks occur at 0.0ms, 400.0ms, and 800.0ms.

---

**👤 You:**
> "What is the grid resolution for a 5:4 rhythm at 100 BPM?"

**🤖 AI Agent:**
> The minimum subdivision unit is 20.0ms, with 3 ticks per beat.


## ❓ FAQ

**Q: How do I find when my rhythms will align?**
Use the `find_sync_point` tool by providing an array of rhythm counts (e.g., [3, 4] for a 3:4 polyrhythm). It will return the alignment pulse and cycle duration.

**Q: Can I get precise timestamps for notes in milliseconds?**
Yes, the `get_layer_attacks` tool calculates the exact millisecond timestamp for every attack in each layer based on your provided BPM and number of measures.

**Q: What is the minimum subdivision grid?**
You can use `get_grid_resolution` to find the smallest rhythmic unit (in ms) and the number of ticks per beat required to represent all attacks perfectly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polyrhythm-calculator](https://vinkius.com/mcp/polyrhythm-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polyrhythm Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polyrhythm-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polyrhythm Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polyrhythm-calculator": {
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
