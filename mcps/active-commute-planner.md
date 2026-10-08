# Active Commute Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/active-commute-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Compare walking, cycling, transit, and driving options based on weather and distance.

## Description
This MCP server provides a multi-modal comparison engine to evaluate commute options. Use `compare_commute_options` to see a side-by-side view of viable modes, or `get_commute_recommendation` to find the best path based on your priority for speed or cost. It accounts for weather conditions and transit availability to ensure accurate results.


## Available Tools (4)
- **compare_commute_options**: Provides a side-by-side comparison of all viable modes for a single trip
- **get_commute_recommendation**: Suggests the best mode based on user preferences
- **get_mode_feasibility**: Determines if a specific mode is a viable option for the given environmental and temporal conditions
- **calculate_mode_metrics**: Calculates the estimated time and cost for a specific mode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Active Commute Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare my commute options for a 5km trip in clear weather where transit is running."

**🤖 AI Agent:**
> For a 5km trip in clear weather, your best options are: Cycling (15 mins, $0), Transit (20 mins, $2.50), or Walking (60 mins, $0).

---

**👤 You:**
> "What is the best way to travel 10km if I want to save money and it is raining?"

**🤖 AI Agent:**
> Since you prioritize cost and it is raining, the best recommendation is Transit, costing $2.50.

---

**👤 You:**
> "Is cycling a good option for a 3km trip in snow?"

**🤖 AI Agent:**
> No, cycling is not a viable option during snow conditions.


## ❓ FAQ

**Q: How does weather affect my commute options?**
Weather impacts the viability and speed of active modes. For example, `get_mode_feasibility` can tell you if walking or cycling is safe during snow or extreme heat.

**Q: Can I prioritize cost over speed?**
Yes, you can use `get_commute_recommendation` and set the priority to 'cost' to find the most economical way to travel.

**Q: Does it consider public transit schedules?**
Yes, by providing the `isOperatingHours` parameter, the tools can determine if transit is a viable option for your trip.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/active-commute-planner](https://vinkius.com/en/ai-agent-connect/active-commute-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Active Commute Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `active-commute-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Active Commute Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "active-commute-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
