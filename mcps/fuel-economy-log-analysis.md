# Fuel Economy Log Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fuel-economy-log-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze vehicle fuel efficiency, cost per distance, and performance trends.

## Description
This MCP server provides analytical tools to track and evaluate vehicle fuel performance. It processes chronological fueling records to calculate efficiency, cost per distance, and period-over-period trends. Use `get_fill_up_summary` to view individual fueling events and efficiency per interval, `get_period_metrics` for aggregated data over specific timeframes, `get_performance_trends` to compare current performance against previous periods, and `search_fuel_logs` to filter specific refueling events.


## Available Tools (4)
- **get_fill_up_summary**: Provides a detailed list of individual fueling events and the efficiency achieved during each interval
- **get_performance_trends**: Compares the current period's efficiency and cost against the most recent prior period to show changes
- **get_period_metrics**: Calculates aggregated fuel efficiency and cost metrics over a specific timeframe
- **search_fuel_logs**: Allows searching for specific fueling events based on date ranges or minimum volume thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fuel Economy Log Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the fuel efficiency summary for vehicle V123."

**🤖 AI Agent:**
> The fuel efficiency for vehicle V123 shows an average efficiency of 12.5 km/L across 5 recorded fill-ups.

---

**👤 You:**
> "What were my fuel metrics between 2024-01-01 and 2024-01-31 for vehicle V123?"

**🤖 AI Agent:**
> For the period 2024-01-01 to 2024-01-31, the vehicle covered 1,200 km with a total fuel consumption of 100L, resulting in an efficiency of 12 km/L and a cost per distance of $0.15/km.

---

**👤 You:**
> "Compare my fuel performance for the last 30 days against the previous 30 days for vehicle V123."

**🤖 AI Agent:**
> Your fuel efficiency improved by 5% compared to the previous 30-day period, and your cost per distance decreased by $0.02/km.


## ❓ FAQ

**Q: How is fuel efficiency calculated?**
Efficiency is determined by the distance traveled between two consecutive fill-ups divided by the volume of fuel required to refill the tank.

**Q: Can I compare my fuel costs between different months?**
Yes, you can use `get_performance_trends` to compare the current period's efficiency and cost against the most recent prior period.

**Q: What data is required to use these tools?**
The tools require a valid `vehicleId` and, for period-based queries, specific ISO 8601 date ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fuel-economy-log-analysis](https://vinkius.com/en/ai-agent-connect/fuel-economy-log-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fuel Economy Log Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fuel-economy-log-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fuel Economy Log Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fuel-economy-log-analysis": {
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
