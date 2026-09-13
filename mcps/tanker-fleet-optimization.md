# Tanker Fleet Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tanker-fleet-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize tanker fleet sizing, vessel mix, and charter strategies for oil transportation.

## Description
This MCP server provides advanced analytical tools to optimize tanker fleet operations. It allows users to calculate the necessary capacity for specific oil volumes using `analyze_demand_requirements`, determine the most efficient combination of vessel sizes with `calculate_optimal_vessel_mix`, and decide between owned or chartered capacity via `optimize_charter_strategy`. Additionally, users can test fleet resilience against market volatility using `simulate_fleet_utilization`.


## Available Tools (4)
- **analyze_demand_requirements**: Analyzes oil demand requirements across specific routes and timeframes
- **calculate_optimal_vessel_mix**: Calculates the best combination of vessel sizes to meet demand
- **optimize_charter_strategy**: Determines the most cost-effective strategy for using owned vs chartered vessels
- **simulate_fleet_utilization**: Simulates how the fleet and charter plan perform under seasonality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tanker Fleet Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total capacity needed for 500,000 barrels from Route A to Route B over 30 days?"

**🤖 AI Agent:**
> The total capacity required for the specified route and volume is 500,000 barrels, with a peak demand period identified in the first 10 days.

---

**👤 You:**
> "Should I charter more vessels if market rates are low?"

**🤖 AI Agent:**
> Based on the current market rates and your owned fleet cost, a Charter-Heavy strategy is recommended to minimize total estimated costs.

---

**👤 You:**
> "What happens to my fleet utilization if market volatility increases by 50%?"

**🤖 AI Agent:**
> With a seasonality factor of 1.5, your utilization rate is projected to be 85% with a capacity buffer of 15,000 barrels to prevent service failures.


## ❓ FAQ

**Q: How do I determine the required vessel capacity?**
You can use the `analyze_demand_requirements` tool by providing your oil volumes, routes, and timeframes to get a summary of total capacity needed.

**Q: Can I simulate market volatility?**
Yes, the `simulate_fleet_utilization` tool allows you to apply a seasonality factor to see how your fleet and charter plan perform during demand surges.

**Q: How is the vessel mix decided?**
The `calculate_optimal_vessel_mix` tool analyzes demand and available capacities to suggest a combination that minimizes unused space and maximizes efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tanker-fleet-optimization](https://vinkius.com/en/ai-agent-connect/tanker-fleet-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tanker Fleet Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tanker-fleet-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tanker Fleet Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tanker-fleet-optimization": {
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
