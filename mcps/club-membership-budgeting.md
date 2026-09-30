# Club Membership Budgeting MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/club-membership-budgeting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregate dues, operational expenses, and participation projections for club financial planning.

## Description
This MCP server provides a suite of tools for club managers to perform precise financial forecasting. It allows for calculating revenue from membership tiers using `get_membership_dues`, aggregating costs for planned activities with `calculate_event_costs`, and forecasting travel expenditures via `estimate_travel_requirements`. Additionally, it can combine equipment and administrative costs through `sum_equipment_and_fees` and produce a comprehensive financial health overview using `generate_budget_forecast`.


## Available Tools (5)
- **estimate_travel_requirements**: Forecasts the total travel expenditure based on participant movement
- **generate_budget_forecast**: Provides a high-level overview of the club's financial health by comparing all revenue and expense streams
- **get_membership_dues**: Calculates the total projected revenue from membership dues based on participant counts and tier pricing
- **sum_equipment_and_fees**: Combines the total costs for physical equipment and administrative fees
- **calculate_event_costs**: Aggregates the total projected costs for all planned club events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Club Membership Budgeting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total revenue for 50 Standard members and 20 Premium members."

**🤖 AI Agent:**
> The total projected revenue from membership dues is $2,500.

---

**👤 You:**
> "What is the total cost for 3 events that cost $200, $350, and $150 respectively?"

**🤖 AI Agent:**
> The total event cost is $700, with an average of $233.33 per event.

---

**👤 You:**
> "Sum up equipment costs of $500 and $300, and administrative fees of $50 and $25."

**🤖 AI Agent:**
> The total equipment cost is $800, the total fees are $75, and the total operational cost is $875.


## ❓ FAQ

**Q: How do I calculate my total membership revenue?**
You can use the `get_membership_dues` tool by providing a JSON mapping of your membership tier IDs to the expected number of members in each tier.

**Q: Can I see a full overview of my club's financial health?**
Yes, once you have calculated your dues, event, travel, and operational costs, you can use `generate_budget_forecast` to see your projected surplus or deficit.

**Q: How are travel costs estimated?**
The `estimate_travel_requirements` tool calculates total travel costs and average costs per traveler based on the trip plans you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/club-membership-budgeting](https://vinkius.com/en/ai-agent-connect/club-membership-budgeting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Club Membership Budgeting** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `club-membership-budgeting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Club Membership Budgeting** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "club-membership-budgeting": {
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
