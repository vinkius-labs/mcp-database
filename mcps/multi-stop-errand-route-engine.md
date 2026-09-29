# Multi-Stop Errand Route Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/multi-stop-errand-route-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates feasible errand sequences considering travel time, service duration, and operating hours.

## Description
This MCP server provides an intelligent routing engine designed to solve complex errand scheduling problems. It calculates an optimal, feasible sequence of stops by accounting for travel time matrices, service durations at each location, and the specific operating hours of each stop. Users can define mandatory stops that must be included in the route, and the engine will identify any unreachable locations that cannot be serviced within their required windows. Use `calculate_errand_route` to generate a full itinerary, `validate_stop_availability` to check if a location is open, `get_travel_metrics` for specific durations, or `summarize_route_efficiency` to analyze time usage.


## Available Tools (4)
- **calculate_errand_route**: Generates the most efficient sequence of stops that satisfies all mandatory requirements and time constraints
- **get_travel_metrics**: Retrieves the travel duration between two specific locations
- **summarize_route_efficiency**: Analyzes a completed route to provide insights into time usage
- **validate_stop_availability**: Checks if a specific stop can be serviced at a specific time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-Stop Errand Route Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a route starting at 09:00 AM including stops A, B, and C, where C is mandatory."

**🤖 AI Agent:**
> The optimal route is [A, C, B]. You will finish at 11:30 AM. Stop B was unreachable due to closing times.

---

**👤 You:**
> "Is the grocery store (ID: store_123) open at 2024-10-25T14:00:00Z?"

**🤖 AI Agent:**
> Yes, the grocery store is open and available for service at that time.

---

**👤 You:**
> "How much time was spent traveling in my last route?"

**🤖 AI Agent:**
> The total travel time for your completed route was 45 minutes.


## ❓ FAQ

**Q: How does the engine handle mandatory stops?**
The engine prioritizes mandatory stops. If a mandatory stop cannot be reached within its operating hours after accounting for travel and previous service times, it will be listed in the unreachable stops.

**Q: Can I check if a specific location is open before planning a route?**
Yes, you can use the `validate_stop_availability` tool to verify if a specific stop can be serviced at a given arrival time based on its operating hours.

**Q: What information is needed to calculate a route?**
To use `calculate_errand_route`, you need to provide the list of all potential stop IDs, the mandatory stop IDs, the start time, a travel time matrix, service durations, and the operating hours for each stop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/multi-stop-errand-route-engine](https://vinkius.com/en/ai-agent-connect/multi-stop-errand-route-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-Stop Errand Route Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multi-stop-errand-route-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-Stop Errand Route Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-stop-errand-route-engine": {
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
