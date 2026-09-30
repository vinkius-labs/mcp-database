# Guest List Cost Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/guest-list-cost-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate event costs, per-guest expenses, and venue capacity limits.

## Description
This MCP server provides essential tools for event budget management. Use `get_total_budget` to calculate the full projected cost, `check_venue_capacity` to ensure your guest list fits the venue, `get_cost_sensitivity` to understand marginal costs, and `get_budget_summary` for a breakdown of fixed versus variable expenses.


## Available Tools (4)
- **check_venue_capacity**: Determines if the planned guest list fits within the venue's limits
- **get_budget_summary**: Provides a high-level breakdown of fixed versus variable cost proportions
- **get_cost_sensitivity**: Analyzes how much the total cost changes when the guest count fluctuates
- **get_total_budget**: Calculates the total projected cost of the event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guest List Cost Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 50 guests if meals are $30, drinks are $15, favors are $5, and the venue fee is $500?"

**🤖 AI Agent:**
> The total cost for 50 guests is $2,750.

---

**👤 You:**
> "Will 120 guests fit in a venue with a capacity of 100?"

**🤖 AI Agent:**
> No, the guest count exceeds the venue capacity by 20 people.

---

**👤 You:**
> "Give me a budget summary for 100 guests with $20 meals, $10 drinks, $5 favors, and a $1000 venue fee."

**🤖 AI Agent:**
> The total cost is $3,500, consisting of $1,000 in fixed costs and $2,500 in variable costs.


## ❓ FAQ

**Q: How do I calculate the total cost of my event?**
You can use the `get_total_budget` tool by providing the guest count, meal price, drink price, favor price, and the venue fee.

**Q: Can I check if my venue is too small?**
Yes, use the `check_venue_capacity` tool with your planned guest count and the venue's maximum occupancy.

**Q: How much will it cost to add more guests?**
The `get_cost_sensitivity` tool calculates the marginal cost per guest and the specific cost for adding ten more attendees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/guest-list-cost-planner](https://vinkius.com/en/ai-agent-connect/guest-list-cost-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guest List Cost Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `guest-list-cost-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guest List Cost Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guest-list-cost-planner": {
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
