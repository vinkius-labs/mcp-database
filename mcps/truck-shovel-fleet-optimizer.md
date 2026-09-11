# Truck-Shovel Fleet Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/truck-shovel-fleet-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimizes truck-to-shovel ratios, fleet size, and production capacity.

## Description
This MCP server provides advanced fleet matching capabilities for mining and construction operations. It calculates the ideal truck-to-shovel ratio using `get_optimal_truck_ratio` to minimize idle time. Users can determine total output with `calculate_production_capacity`, estimate necessary equipment with `estimate_required_fleet_size`, and model operational disruptions using `simulate_queuing_and_bunching` to account for haul time variance and bunching effects.


## Available Tools (4)
- **calculate_production_capacity**: Calculates the total material output of the fleet over a specific duration
- **get_optimal_truck_ratio**: Determines the ideal number of trucks to assign to a shovel to minimize idle time for both equipment types
- **estimate_required_fleet_size**: Calculates the number of trucks needed to meet a specific production target
- **simulate_queuing_and_bunching**: Estimates the impact of irregular truck arrivals on shovel productivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Truck-Shovel Fleet Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal truck-to-shovel ratio if a shovel loads in 2 minutes, a truck cycle takes 15 minutes, and availability is 90%?"

**🤖 AI Agent:**
> The optimal truck count for this configuration is 7 trucks to maintain maximum efficiency.

---

**👤 You:**
> "Calculate the production capacity for a fleet with 5 trucks, a shovel productivity of 500 units/hr, a ratio of 4, and 85% availability."

**🤖 AI Agent:**
> The total hourly production capacity is 425 units.

---

**👤 You:**
> "How many trucks are needed to reach 1000 units per hour if shovel productivity is 600 units/hr, truck cycle is 12 mins, shovel cycle is 3 mins, and availability is 95%?"

**🤖 AI Agent:**
> To meet the target of 1000 units per hour, you will require 18 trucks and 2 shovels.


## ❓ FAQ

**Q: How do I find the best number of trucks for my shovel?**
You can use the `get_optimal_truck_ratio` tool. Provide the shovel cycle time, truck cycle time, and equipment availability to find the ideal ratio.

**Q: Can I predict production delays caused by truck bunching?**
Yes, the `simulate_queuing_and_bunching` tool estimates the impact of irregular truck arrivals on shovel productivity and expected wait times.

**Q: How many trucks do I need to hit a specific production target?**
Use the `estimate_required_fleet_size` tool. Input your target production, shovel productivity, and cycle times to get the required truck and shovel counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/truck-shovel-fleet-optimizer](https://vinkius.com/en/ai-agent-connect/truck-shovel-fleet-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Truck-Shovel Fleet Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `truck-shovel-fleet-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Truck-Shovel Fleet Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truck-shovel-fleet-optimizer": {
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
