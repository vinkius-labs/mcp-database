# Airport Transfer Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/airport-transfer-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Compare taxi, rideshare, transit, and other airport transport options.

## Description
This MCP server provides a decision-support engine for travelers. It evaluates and compares various transportation modalities for airport transit based on cost, time, and logistical constraints. Use `compare_transport_options` to see a full comparison of all methods, `get_transit_schedules` for public transport timings, `calculate_rideshare_estimates` for vehicle tier pricing, and `evaluate_walking_feasibility` to check if walking is practical given your luggage.


## Available Tools (4)
- **calculate_rideshare_estimates**: Estimates the cost and availability of various rideshare vehicle tiers
- **compare_transport_options**: Provides a comprehensive comparison of all available transport methods for a specific trip
- **evaluate_walking_feasibility**: Determines if walking is a viable option based on distance and passenger needs
- **get_transit_schedules**: Retrieves available public transit routes and their specific timings for a route


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airport Transfer Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare all transport options from JFK Airport to Manhattan for 2 people with 2 bags departing tomorrow at 10:00 AM."

**🤖 AI Agent:**
> The best option is a Rideshare (XL) costing $55 with a 45-minute duration, or Public Transit costing $12 with a 70-minute duration.

---

**👤 You:**
> "What are the transit schedules from Heathrow to Central London for June 15th?"

**🤖 AI Agent:**
> The Express Line departs every 15 minutes, with the next available departures at 09:00, 09:15, and 09:30.

---

**👤 You:**
> "Is it feasible to walk from the terminal to the parking garage with 3 bags?"

**🤖 AI Agent:**
> Walking is not viable because you have 3 bags.


## ❓ FAQ

**Q: How do I compare all available transport methods at once?**
You can use the `compare_transport_options` tool to get a comprehensive breakdown of costs and durations for all modalities.

**Q: Can I check if walking is feasible with my luggage?**
Yes, the `evaluate_walking_feasibility` tool specifically checks if walking is viable based on distance and your luggage count.

**Q: Does this tool provide rideshare pricing?**
Yes, you can use `calculate_rideshare_estimates` to see different vehicle tiers and their estimated costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/airport-transfer-comparator](https://vinkius.com/en/ai-agent-connect/airport-transfer-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airport Transfer Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `airport-transfer-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airport Transfer Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airport-transfer-comparator": {
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
