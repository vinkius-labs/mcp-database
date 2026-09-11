# Haulage Cost Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/haulage-cost-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize mining logistics by calculating haulage costs and fleet requirements.

## Description
This MCP server provides specialized tools for mining logistics optimization. It allows AI agents to calculate the economic impact of haulage routes by determining cost per tonne-kilometer, estimating the required truck fleet size for production schedules, and aggregating total operational expenditures. Use `analyze_haulage_scenario` to get a complete economic profile of a route, or `estimate_fleet_requirements` to plan capacity based on cycle times and available operational hours.


## Available Tools (4)
- **analyze_haulage_scenario**: Provides a comprehensive overview of a specific haulage route's economic profile
- **calculate_haulage_efficiency**: Calculates the fundamental cost efficiency of the current haulage setup
- **estimate_fleet_requirements**: Determines the number of trucks needed to meet a specific production goal
- **get_total_operational_cost**: Aggregates all variable costs to provide a total expenditure estimate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Haulage Cost Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost per tonne-kilometer for a 5km haul moving 10,000 tonnes with a total cost of $5,000?"

**🤖 AI Agent:**
> The cost per tonne-kilometer is $0.10.

---

**👤 You:**
> "How many trucks are needed to move 5,000 tonnes if each truck carries 50 tonnes, has a 2-hour cycle time, and we have 40 hours of available time?"

**🤖 AI Agent:**
> You will need 13 trucks to meet this production goal.

---

**👤 You:**
> "Calculate the total operational cost for fuel at $2,000, tires at $1,500, and maintenance at $1,000."

**🤖 AI Agent:**
> The total operational cost is $4,500.


## ❓ FAQ

**Q: How can I calculate the efficiency of my current haulage route?**
You can use the `calculate_haulage_efficiency` tool by providing the haul distance, total tonnage, and the sum of fuel, tire, and maintenance costs.

**Q: How do I determine how many trucks I need for a production goal?**
Use the `estimate_fleet_requirements` tool. You will need to provide the target production tonnage, the capacity of a single truck, the cycle time per trip, and the total available operational time.

**Q: What costs are included in the total operational cost calculation?**
The `get_total_operational_cost` tool aggregates three primary drivers: fuel consumption, tire wear, and mechanical maintenance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/haulage-cost-optimization](https://vinkius.com/en/ai-agent-connect/haulage-cost-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Haulage Cost Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `haulage-cost-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Haulage Cost Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "haulage-cost-optimization": {
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
