# Seat Count Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seat-count-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate required vehicles and fleet efficiency for traveler groups.

## Description
This MCP server provides precise logistics planning tools for transport managers. It allows AI agents to determine the exact number of vehicles needed for any group size using `get_required_vehicles`. Users can also evaluate fleet efficiency with `calculate_utilization_rate`, get a complete overview of fleet needs via `get_fleet_configuration`, or compare different vehicle capacities using `compare_vehicle_options` to find the most efficient transport solution.


## Available Tools (4)
- **calculate_utilization_rate**: Evaluates how efficiently the assigned fleet is being used
- **compare_vehicle_options**: Compares two different vehicle types to see which one is more efficient for a specific group size
- **get_fleet_configuration**: Provides a summary of the fleet needs and the resulting empty space
- **get_required_vehicles**: Determines how many vehicles must be deployed to accommodate a specific number of travelers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seat Count Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 15-seat minivans do I need for 40 travelers?"

**🤖 AI Agent:**
> You will need 3 minivans to accommodate 40 travelers.

---

**👤 You:**
> "What is the utilization rate for 25 people in 30-seat buses?"

**🤖 AI Agent:**
> The utilization rate is 83.33% with 5 empty seats.

---

**👤 You:**
> "Is it better to use 10-seat vans or 20-seat buses for 35 people?"

**🤖 AI Agent:**
> Using 20-seat buses is more efficient, as it requires only 2 vehicles compared to 4 vans, reducing empty seats.


## ❓ FAQ

**Q: How do I know how many vehicles I need?**
You can use the `get_required_vehicles` tool to find the exact number of vehicles needed based on your total traveler count and the capacity of each vehicle.

**Q: Can I compare different vehicle sizes?**
Yes, the `compare_vehicle_options` tool allows you to compare two different vehicle capacities to see which one results in better efficiency for your specific group.

**Q: How is fleet efficiency measured?**
Efficiency is measured using `calculate_utilization_rate`, which provides the utilization percentage and the number of empty seats remaining in the fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seat-count-calculator](https://vinkius.com/en/ai-agent-connect/seat-count-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seat Count Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seat-count-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seat Count Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seat-count-calculator": {
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
