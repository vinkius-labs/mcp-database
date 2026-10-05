# Restaurant Table Turn Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/restaurant-table-turn-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Forecasts seating capacity, table turnover, labor, and break-even points.

## Description
This MCP server provides essential forecasting tools for restaurant operations. Use `forecast_capacity` to determine guest volume, `calculate_financials` to find break-even points, `staffing_requirement` to plan labor, and `reservation_load_analysis` to manage walk-in capacity.


## Available Tools (4)
- **forecast_capacity**: Forecasts how many guests can be served during a specific service window
- **calculate_financials**: Calculates expected revenue, costs, and break-even points
- **reservation_load_analysis**: Analyzes the load of reservations against projected capacity
- **staffing_requirement**: Determines staffing needs based on volume and labor targets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restaurant Table Turn Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many guests can I serve with 50 seats, a turnover rate of 3, and a 5-hour service window?"

**🤖 AI Agent:**
> You can serve 150 guests with a seat utilization of 100%.

---

**👤 You:**
> "What is my break-even point if I have 1000 in fixed costs, a 25 average check, and 10 variable cost per guest?"

**🤖 AI Agent:**
> You need 67 guests to reach your break-even point.

---

**👤 You:**
> "I have 200 expected guests and 120 are already reserved. How many walk-ins can I expect?"

**🤖 AI Agent:**
> You can expect 80 walk-in guests, which represents a reservation density of 60%.


## ❓ FAQ

**Q: How do I calculate my total guest capacity?**
You can use the `forecast_capacity` tool by providing your seating capacity, turnover rate, and the service window duration.

**Q: Can this tool help with staffing?**
Yes, the `staffing_requirement` tool calculates the target labor budget and recommended staff count based on your projected covers and labor cost targets.

**Q: How do I find my break-even point?**
Use the `calculate_financials` tool with your projected covers, average check, fixed costs, and variable costs per cover to find the break-even covers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/restaurant-table-turn-plan](https://vinkius.com/en/ai-agent-connect/restaurant-table-turn-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restaurant Table Turn Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restaurant-table-turn-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restaurant Table Turn Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restaurant-table-turn-plan": {
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
