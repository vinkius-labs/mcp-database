# Digital Nomad Month Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-nomad-month-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan your monthly relocation with precise budget and workday capacity estimates.

## Description
The Digital Nomad Month Planner helps you synchronize the logistics of moving to a new destination. It calculates total monthly costs including lodging, food, transport, and fixed expenses like visas and insurance. You can also use `calculate_workday_capacity` to estimate your productive hours based on local connectivity, or `estimate_daily_burn_rate` to understand your daily cash outflow. This tool is designed to bridge the gap between travel dreams and operational reality.


## Available Tools (4)
- **compare_destination_tiers**: Allows a user to see how much a change in lifestyle impacts the total monthly cost
- **estimate_daily_burn_rate**: Calculates the amount of cash required for daily operational expenses
- **calculate_workday_capacity**: Determines how many productive hours a nomad can realistically expect in a month
- **get_monthly_budget_summary**: Provides a comprehensive breakdown of all estimated costs for a one-month stay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Nomad Month Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total monthly budget for a mid-range stay in Lisbon?"

**🤖 AI Agent:**
> The estimated total monthly cost for a mid-range stay in Lisbon is $2,450, which includes lodging, coworking, food, transport, visa, insurance, and data.

---

**👤 You:**
> "How many hours can I work in Bali if I plan to work 8 hours a day with medium connectivity?"

**🤖 AI Agent:**
> You can expect approximately 224 productive hours in Bali, with an estimated 16 hours of downtime due to connectivity factors.

---

**👤 You:**
> "What is my daily burn rate for a budget lifestyle in Medellin?"

**🤖 AI Agent:**
> Your daily variable cost in Medellin for a budget lifestyle is $45 per day.


## ❓ FAQ

**Q: How are the monthly costs calculated?**
Costs are calculated by multiplying the daily rates for your chosen lifestyle tier by 30 days, while visa and insurance fees are added as flat monthly amounts.

**Q: Can I compare different lifestyle tiers?**
Yes, you can use the `compare_destination_tiers` tool to see the exact cost difference and percentage increase when moving from budget to mid-range or luxury tiers.

**Q: How does internet reliability affect my planning?**
When using `calculate_workday_capacity`, specifying low connectivity reliability will increase your estimated downtime, providing a more realistic view of your monthly productive hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-nomad-month-planner](https://vinkius.com/en/ai-agent-connect/digital-nomad-month-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Nomad Month Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-nomad-month-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Nomad Month Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-nomad-month-planner": {
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
