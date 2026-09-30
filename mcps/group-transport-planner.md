# Group Transport Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/group-transport-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare group travel options by cost, capacity, and accessibility.

## Description
This MCP server provides tools to optimize group mobility. It allows users to find suitable transport modes based on passenger count and luggage volume, compare the total and per-person costs of different options, estimate travel duration including walking time to pickup points, and evaluate accessibility for passengers with wheelchairs or strollers. Use `find_transport_options` to start your search and `compare_travel_costs` to find the best value.


## Available Tools (4)
- **calculate_travel_duration**: Estimate total travel time including transit and boarding overhead
- **compare_travel_costs**: Compare economic impact of different transport modes
- **evaluate_accessibility_score**: Determine suitability for groups with mobility constraints
- **find_transport_options**: Retrieve available transport modes that accommodate group size and luggage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Transport Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find transport options for 4 people with 3 large suitcases."

**🤖 AI Agent:**
> The available options are a Sedan (capacity 4) and an SUV (capacity 5).

---

**👤 You:**
> "Which is cheaper for 6 people: a Minivan or a Shuttle?"

**🤖 AI Agent:**
> The Minivan costs $45 total ($7.50 per person), while the Shuttle costs $60 total ($10.00 per person).

---

**👤 You:**
> "How long will it take to get to the station if I walk 500 meters?"

**🤖 AI Agent:**
> The total travel time is 25 minutes.


## ❓ FAQ

**Q: How do I find vehicles that fit my group?**
You can use the `find_transport_options` tool by providing the number of passengers and the total luggage volume.

**Q: Can I check if a transport option is wheelchair accessible?**
Yes, use the `evaluate_accessibility_score` tool to check suitability for wheelchair or stroller users.

**Q: How is the total travel time calculated?**
The `calculate_travel_duration` tool calculates the sum of the transit time and the time spent walking to the pickup point.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/group-transport-planner](https://vinkius.com/en/ai-agent-connect/group-transport-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Transport Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-transport-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Transport Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-transport-planner": {
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
