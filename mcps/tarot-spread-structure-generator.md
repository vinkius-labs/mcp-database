# Tarot Spread Structure Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tarot-spread-structure-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Provides deterministic structural blueprints for tarot spreads, including positions and reading sequences.

## Description
This MCP server acts as a structural architect for tarot practitioners. It provides the exact layout blueprints for various tarot spreads without drawing cards. Use `get_spread_blueprint` to retrieve the full architecture of a spread, including position meanings and reading order. You can also use `list_available_spreads` to see all supported layouts or `get_spread_complexity_metrics` to understand the depth of a specific spread.


## Available Tools (3)
- **get_spread_complexity_metrics**: Analyzes a spread to determine its depth and utility for different types of readings
- **get_spread_blueprint**: Retrieves the complete structural definition for a specific named tarot spread
- **list_available_spreads**: Provides a list of all structural layouts currently supported by the generator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tarot Spread Structure Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the structure of the Celtic Cross spread?"

**🤖 AI Agent:**
> The Celtic Cross spread consists of 10 positions. The sequence starts with the central card representing the current situation, followed by the crossing card representing the immediate obstacle, and continues through the surrounding positions for past, goal, and future influences.

---

**👤 You:**
> "List all the tarot spreads available in this tool."

**🤖 AI Agent:**
> The available spreads are: Three Card Spread, Celtic Cross, Horseshoe Spread, and Five Card Spread.

---

**👤 You:**
> "How complex is the Three Card Spread?"

**🤖 AI Agent:**
> The Three Card Spread is classified as a Simple spread with a primary focus on Time-based or situational analysis.


## ❓ FAQ

**Q: Does this tool draw tarot cards?**
No, this tool is purely structural. It provides the layout, position meanings, and sequence for spreads, but does not perform card drawing.

**Q: How can I see which spreads are available?**
You can use the `list_available_spreads` tool to get a complete list of all supported tarot layouts.

**Q: Can I get the details for a specific spread?**
Yes, use `get_spread_blueprint` with the specific name of the spread to get its positions, meanings, and orientation rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tarot-spread-structure-generator](https://vinkius.com/ai-agent-connect/tarot-spread-structure-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tarot Spread Structure Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tarot-spread-structure-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tarot Spread Structure Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tarot-spread-structure-generator": {
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
