# Refill Station Route Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refill-station-route-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Compares refill routes using a unified cost index based on distance, transport mode, and time.

## Description
This MCP server provides tools to evaluate and compare different refill station routes. It calculates a unified cost index by combining transport costs (adjusted by mode), product pricing, parking fees, and the economic value of travel time. Use `compare_routes` to rank multiple paths or `calculate_route_efficiency` for a detailed cost breakdown of a single trip.


## Available Tools (4)
- **compare_routes**: Compares multiple provided routes to find the most efficient option based on the unified cost index
- **get_mode_factor**: g., Heavy Freight, Light Van, Electric Courier).

Retrieves the specific multiplier for a given transport mode
- **validate_route_integrity**: Checks if a route's parameters are logically consistent and within valid bounds
- **calculate_route_efficiency**: Calculates the specific cost breakdown for a single provided route


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refill Station Route Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two routes: Route A has 50km distance, Light Van mode, $2 product price, 100 quantity, $5 parking, 1 hour travel time, and $15 time value rate. Route B has 40km distance, Electric Courier mode, $2 product price, 100 quantity, $10 parking, 0.5 hour travel time, and $15 time value rate."

**🤖 AI Agent:**
> Route B is the most efficient option with a lower unified cost index compared to Route A.

---

**👤 You:**
> "Calculate the efficiency for a route with 120km distance, Heavy Freight mode, $5 product price, 500 quantity, $20 parking fees, 3 hours travel time, and $20 time value rate."

**🤖 AI Agent:**
> The total cost index is $2,780, consisting of $1,200 transport cost, $2,500 product cost, $20 parking, and $60 time value.

---

**👤 You:**
> "What is the multiplier for an Electric Courier?"

**🤖 AI Agent:**
> The multiplier for the Electric Courier mode is 0.8.


## ❓ FAQ

**Q: How is the route efficiency calculated?**
The efficiency is determined by a unified cost index, which sums the transport cost (distance multiplied by the mode factor), the total product cost, all parking fees, and the time value.

**Q: What transport modes are supported?**
Supported modes include Heavy Freight, Light Van, and Electric Courier. You can use `get_mode_factor` to check the specific multiplier for each.

**Q: Can I validate a route before comparing it?**
Yes, use the `validate_route_integrity` tool to ensure distance, quantity, and travel time are logically consistent and within valid bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refill-station-route-comparator](https://vinkius.com/en/ai-agent-connect/refill-station-route-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refill Station Route Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refill-station-route-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refill Station Route Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refill-station-route-comparator": {
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
