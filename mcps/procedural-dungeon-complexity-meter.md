# Procedural Dungeon Complexity Meter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/procedural-dungeon-complexity-meter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Analyze the structural complexity and player experience of procedural dungeon layouts.

## Description
This MCP server provides a suite of mathematical tools to evaluate the topology of procedurally generated dungeons. Use `analyze_dungeon_structure` to determine the difficulty rating and complexity score of a layout. Use `calculate_traversal_metrics` to predict player movement patterns, including backtrack percentage and estimated completion time. Finally, use `evaluate_density_and_exploration` to measure how effectively a dungeon utilizes its space and provides variety through exploration scores and room density.


## Available Tools (3)
- **analyze_dungeon_structure**: Provides a high-level overview of the dungeon's complexity and difficulty
- **calculate_traversal_metrics**: Analyzes the physical movement and efficiency of the dungeon layout
- **evaluate_density_and_exploration**: Measures how well the dungeon utilizes its space and offers variety


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Procedural Dungeon Complexity Meter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a dungeon with 30 rooms, 45 corridors, a branching factor of 2.5, and 5 loops."

**🤖 AI Agent:**
> The dungeon has a complexity score of 80, which is rated as a Hard maze.

---

**👤 You:**
> "Calculate the traversal metrics for a dungeon with 50 rooms, 60 corridors, 10 dead ends, a traversal depth of 15, and an average room time of 30 seconds."

**🤖 AI Agent:**
> The traversal depth is 15, the backtrack percentage is 20%, and the estimated completion time is 450 seconds.

---

**👤 You:**
> "Evaluate the density and exploration for a dungeon with 40 rooms, 1000 total area, 50 unique paths, and 200 total paths."

**🤖 AI Agent:**
> The exploration score is 0.25 and the optimal room density is 0.04.


## ❓ FAQ

**Q: How is the difficulty rating determined?**
The difficulty rating is based on the `graph_complexity_score`. Scores above 50 are rated as 'Hard maze', between 20 and 50 as 'Medium', and below 20 as 'Linear'.

**Q: What does the frustration flag indicate?**
A frustration flag is triggered if the backtrack percentage is greater than 60% (indicating too many dead ends) or less than 10% (indicating a layout that is too linear).

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/procedural-dungeon-complexity-meter](https://vinkius.com/ai-agent-connect/procedural-dungeon-complexity-meter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Procedural Dungeon Complexity Meter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `procedural-dungeon-complexity-meter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Procedural Dungeon Complexity Meter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "procedural-dungeon-complexity-meter": {
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
