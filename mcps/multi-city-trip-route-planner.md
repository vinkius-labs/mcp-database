# Multi-City Trip Route Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/multi-city-trip-route-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Validate, calculate metrics, and compare multi-city travel routes.

## Description
This MCP server provides tools to manage complex multi-city itineraries. You can use `validate_route_sequence` to ensure your trip meets minimum stay requirements, `calculate_route_metrics` to sum up total costs and travel times, `compare_routes` to find the most efficient path based on cost or time, and `get_stay_summary` to see a breakdown of time spent in each city.


## Available Tools (4)
- **calculate_route_metrics**: Aggregates the total cost and total travel time for a given sequence of legs
- **compare_routes**: Compares two different valid route sequences to identify the most efficient one
- **get_stay_summary**: Provides a breakdown of time spent in each city within a route
- **validate_route_sequence**: Checks if a specific sequence of cities adheres to all minimum stay constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-City Trip Route Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my route [Paris, London, Berlin] valid if I stay 2 nights in Paris and 1 night in London, given a 2-night minimum for Paris and 2-night minimum for London?"

**🤖 AI Agent:**
> No, the route is invalid because the stay in London (1 night) does not meet the minimum requirement of 2 nights.

---

**👤 You:**
> "What is the total cost for a trip from New York to Tokyo to Seoul with legs costing $800 and $500?"

**🤖 AI Agent:**
> The total cost for the trip is $1,300.

---

**👤 You:**
> "Show me a summary of my stay in [Rome, Florence, Venice] if I stay 3 nights in Rome and 2 nights in Florence."

**🤖 AI Agent:**
> Rome: 3 nights, Florence: 2 nights.


## ❓ FAQ

**Q: How do I know if my route is valid?**
You can use the `validate_route_sequence` tool. It checks if the number of nights spent in each city meets the required minimum stay rules.

**Q: Can I compare two different travel plans?**
Yes, the `compare_routes` tool allows you to compare two validated routes to see which one is better based on your preference for either cost or travel time.

**Q: How are total trip costs calculated?**
The `calculate_route_metrics` tool aggregates the costs and durations of all transport legs provided in your sequence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/multi-city-trip-route-planner](https://vinkius.com/en/ai-agent-connect/multi-city-trip-route-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-City Trip Route Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multi-city-trip-route-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-City Trip Route Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-city-trip-route-planner": {
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
