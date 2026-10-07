# Carpool Emissions & Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/carpool-emissions-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Distributes trip emissions and costs among carpool riders based on distance and occupancy.

## Description
This MCP server provides precise allocation logic for carpool journeys. It calculates how carbon emissions and financial costs should be shared among riders by analyzing route distance, fuel usage, and specific pickup detours. Use `calculate_emissions_distribution` to determine individual carbon footprints, `calculate_cost_split` to divide trip expenses, and `calculate_detour_impact` to quantify the extra distance caused by specific rider pickups. It also offers `get_trip_summary` for a high-level view of environmental efficiency.


## Available Tools (4)
- **calculate_emissions_distribution**: Determines how much carbon emissions each rider is responsible for
- **get_trip_summary**: Provides a high-level overview of the efficiency and environmental impact of a carpool
- **calculate_detour_impact**: Quantifies the specific "penalty" or extra distance added to a trip due to a rider's pickup/drop-off requirements
- **calculate_cost_split**: Determines the financial cost assigned to each rider


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carpool Emissions & Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much CO2 is each rider responsible for if the total emissions are 5.0kg, rider A traveled 10km, and rider B traveled 15km?"

**🤖 AI Agent:**
> Rider A is responsible for 2.0kg of CO2 and Rider B is responsible for 3.0kg of CO2.

---

**👤 You:**
> "Calculate the cost split for a $20 trip where Rider A traveled 5km and Rider B traveled 15km."

**🤖 AI Agent:**
> Rider A's allocated cost is $5.00 and Rider B's allocated cost is $15.00.

---

**👤 You:**
> "What was the environmental impact of a trip with 4 riders, 40km total distance, and 8.0kg total emissions?"

**🤖 AI Agent:**
> The per-person emissions were 2.0kg, and you saved 6.0kg of CO2 compared to single-occupancy trips.


## ❓ FAQ

**Q: How are emissions distributed among riders?**
Emissions are distributed proportionally based on the distance each rider travels, including any detours required for their pickup or drop-off, relative to the total distance.

**Q: Can I calculate the extra distance caused by a detour?**
Yes, you can use the `calculate_detour_impact` tool to find the specific distance penalty added to the primary route for each rider.

**Q: Does this tool account for the number of people in the car?**
Yes, occupancy is a key factor in calculating the `get_trip_summary` and determining the proportional distribution of emissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/carpool-emissions-cost-splitter](https://vinkius.com/en/ai-agent-connect/carpool-emissions-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carpool Emissions & Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carpool-emissions-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carpool Emissions & Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carpool-emissions-cost-splitter": {
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
