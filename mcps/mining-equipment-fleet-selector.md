# Mining Equipment Fleet Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mining-equipment-fleet-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate optimal loader and truck fleet sizes for mining operations.

## Description
This MCP server provides specialized tools to design and optimize mining fleets. It calculates the required number of loading units using `loader_fleet_sizing_tool` and determines the necessary haul truck count with `truck_fleet_sizing_tool`. You can also evaluate the efficiency of equipment pairings via `equipment_match_analysis_tool` to ensure the number of bucket passes is optimized, and generate a comprehensive `fleet_productivity_report_tool` to identify bottlenecks between loading and hauling capacities.


## Available Tools (4)
- **equipment_match_analysis_tool**: Evaluates the efficiency of the pairing between a specific loader and truck
- **fleet_productivity_report_tool**: Provides a high-level summary of the total fleet's capability
- **loader_fleet_sizing_tool**: Determines the required capacity and number of loading units needed to meet a specific production target
- **truck_fleet_sizing_tool**: Calculates the number of haul trucks required to support the loading units and meet production targets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mining Equipment Fleet Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many loaders do I need for a target of 5000 cubic meters if density is 2.5 and I have 2000 operating hours with 85% availability and 80% utilization?"

**🤖 AI Agent:**
> You will need 2 loaders to meet the production target of 5000 cubic meters under the specified availability and utilization constraints.

---

**👤 You:**
> "Calculate the truck fleet for 5000 cubic meters, 100m haul distance, 20km/h speed, 5 minute loader cycle, 90% availability and 85% utilization."

**🤖 AI Agent:**
> The required truck fleet consists of 4 trucks to support the production target given the haul distance and cycle times.

---

**👤 You:**
> "Is a 10m3 bucket a good match for a 50m3 truck with a material density of 2.0?"

**🤖 AI Agent:**
> Yes, the equipment match is optimized as it requires 5 passes to fill the truck.


## ❓ FAQ

**Q: How does the tool calculate the number of trucks needed?**
The `truck_fleet_sizing_tool` calculates the truck count by analyzing the total cycle time, which includes loading, travel, and dumping, relative to the target production volume and machine availability.

**Q: What is an optimized equipment match?**
An optimized match occurs when the `equipment_match_analysis_tool` determines that the loader bucket capacity allows for 3 to 5 passes to fill a truck, balancing cycle time and payload efficiency.

**Q: Can I identify bottlenecks in my fleet?**
Yes, by using the `fleet_productivity_report_tool`, you can identify if your system capacity is limited by the loading fleet or the hauling fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mining-equipment-fleet-selector](https://vinkius.com/ai-agent-connect/mining-equipment-fleet-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mining Equipment Fleet Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mining-equipment-fleet-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mining Equipment Fleet Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mining-equipment-fleet-selector": {
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
