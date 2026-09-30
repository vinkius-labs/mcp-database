# Reunion Travel Cost Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reunion-travel-cost-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate, track, and reconcile group travel expenses.

## Description
This MCP server provides tools to manage the financial complexities of group trips. It allows users to aggregate total costs using `calculate_trip_totals`, determine specific individual responsibilities with `calculate_individual_share`, generate clear debt settlement instructions via `generate_settlement_plan`, and monitor spending limits with `analyze_budget_health`.


## Available Tools (4)
- **analyze_budget_health**: Compares actual spending against a predefined budget to identify overages
- **calculate_individual_share**: Determines how much a specific person is responsible for paying
- **calculate_trip_totals**: Aggregates all expenses to provide a high-level overview of the trip's financial footprint
- **generate_settlement_plan**: Produces a list of transactions required to settle all debts between group members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reunion Travel Cost Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost of our trip so far?"

**🤖 AI Agent:**
> The total trip cost is $1,250.00, consisting of $500 for lodging, $300 for transport, $250 for food, and $200 for activities.

---

**👤 You:**
> "How much does Alex owe?"

**🤖 AI Agent:**
> Alex owes a total of $150.00 based on their participation in the shared expenses.

---

**👤 You:**
> "Who needs to pay whom to settle the group expenses?"

**🤖 AI Agent:**
> To settle all debts, Jordan should pay $50.00 to Taylor, and Casey should pay $30.00 to Taylor.


## ❓ FAQ

**Q: How can I see the total cost of the trip?**
You can use the `calculate_trip_totals` tool to get a breakdown of all expenses including lodging, transport, and food.

**Q: How do we settle debts between group members?**
The `generate_settlement_plan` tool creates a list of specific transactions to ensure everyone pays their fair share.

**Q: Can I check if we are overspending?**
Yes, the `analyze_budget_health` tool compares your actual spending against your set budget thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reunion-travel-cost-planner](https://vinkius.com/en/ai-agent-connect/reunion-travel-cost-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reunion Travel Cost Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reunion-travel-cost-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reunion Travel Cost Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reunion-travel-cost-planner": {
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
