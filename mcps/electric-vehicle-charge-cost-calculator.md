# Electric Vehicle Charge Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/electric-vehicle-charge-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate EV charging costs, distance efficiency, and monthly budget projections.

## Description
This MCP server provides a suite of tools to manage the financial aspects of electric vehicle ownership. Use `get_session_cost` to determine the exact price of a single charge including taxes and losses. Use `get_distance_cost` to understand how much each kilometer costs based on your vehicle's efficiency. You can also use `get_monthly_projection` to plan your monthly budget or `get_tariff_comparison` to decide between home and public charging stations.


## Available Tools (4)
- **get_distance_cost**: Determines how much it costs to travel a specific distance based on charging efficiency
- **get_monthly_projection**: Estimates the monthly budget required for EV charging
- **get_session_cost**: Calculates the total financial cost for a single charging event
- **get_tariff_comparison**: Compares the cost-effectiveness of home vs. public charging for a specific energy requirement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electric Vehicle Charge Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to add 50kWh to my EV if the rate is $0.25/kWh, with a 10% loss and 5% tax?"

**🤖 AI Agent:**
> The total cost for this charging session is $14.44.

---

**👤 You:**
> "If a session costs $12 and I added 40kWh, and my car uses 150Wh/km, what is my cost per km?"

**🤖 AI Agent:**
> The cost per kilometer is $0.45.

---

**👤 You:**
> "I charge 10 times a month at an average cost of $8 per session. What is my monthly projection?"

**🤖 AI Agent:**
> Your estimated monthly cost is $80.00, with a daily average of $2.67.


## ❓ FAQ

**Q: How does the tool account for energy loss?**
The `get_session_cost` tool uses an efficiency loss factor to account for the extra energy drawn from the grid that is lost as heat during the charging process.

**Q: Can I compare home and public charging costs?**
Yes, you can use the `get_tariff_comparison` tool to compare the total cost of charging at home versus using a public station for a specific energy requirement.

**Q: How do I estimate my monthly EV spending?**
You can use `get_monthly_projection` by providing the average cost of a session and how many times you charge per month.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/electric-vehicle-charge-cost-calculator](https://vinkius.com/en/ai-agent-connect/electric-vehicle-charge-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electric Vehicle Charge Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electric-vehicle-charge-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electric Vehicle Charge Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electric-vehicle-charge-cost-calculator": {
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
