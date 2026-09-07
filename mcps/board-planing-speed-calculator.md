# Board Planing Speed Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/board-planing-speed-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate minimum planing speeds and drag profiles for surfboards.

## Description
This MCP server provides hydrodynamic analysis for surfboard design and performance. Use `get_minimum_planing_speed` to find the threshold speed required for a rider to lift the board out of the water. You can also use `get_drag_profile` to analyze resistance across speed increments, `get_optimal_operating_window` to find the most efficient velocity range, or `compare_configurations` to evaluate how different fin setups and rocker levels impact performance.


## Available Tools (4)
- **compare_configurations**: Evaluates how changing the fin setup or rocker affects the planing performance
- **get_drag_profile**: Analyzes how drag changes across different speed increments for a specific board setup
- **get_minimum_planing_speed**: Determines the threshold speed required for the board to begin planing
- **get_optimal_operating_window**: Identifies the ideal speed range for performance and efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Board Planing Speed Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum planing speed for a 75kg rider on a 180cm x 50cm board with a thruster setup, rocker level 4, and concave depth 3?"

**🤖 AI Agent:**
> The minimum planing speed for this setup is 5.2 m/s, with an optimal speed range of 5.5-7.0 m/s and a drag coefficient of 0.045.

---

**👤 You:**
> "Show me the drag profile for a 80kg rider on a 190cm x 52cm board with rocker level 5."

**🤖 AI Agent:**
> At 4 m/s, the drag coefficient is 0.03; at 6 m/s, it is 0.05; and at 8 m/s, it is 0.08.

---

**👤 You:**
> "What is the best speed range for a 70kg rider on a 175cm x 48cm board with a quad fin setup?"

**🤖 AI Agent:**
> The ideal speed range for this board is 5.8 m/s to 7.2 m/s, providing an efficiency rating of 8.5.


## ❓ FAQ

**Q: How do I calculate the minimum speed for my board?**
Use the `get_minimum_planing_speed` tool by providing the rider's weight, board dimensions, fin configuration, rocker level, and concave depth.

**Q: Can I compare different fin setups?**
Yes, the `compare_configurations` tool allows you to compare multiple fin setups and rocker levels against a baseline to see the impact on speed and drag.

**Q: What is the optimal speed range?**
The optimal speed range is the velocity window where the lift-to-drag ratio is maximized. You can find this using `get_optimal_operating_window`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/board-planing-speed-calculator](https://vinkius.com/ai-agent-connect/board-planing-speed-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Board Planing Speed Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `board-planing-speed-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Board Planing Speed Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "board-planing-speed-calculator": {
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
