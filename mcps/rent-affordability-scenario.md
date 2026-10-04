# Rent Affordability Scenario MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rent-affordability-scenario)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluate housing options against income, debts, and savings goals.

## Description
This MCP server provides tools to determine the true affordability of rental properties. It calculates housing share, monthly leftover cash, and upfront move-in costs. Use `generate_affordability_report` to get a complete financial overview, `analyze_budget_feasibility` to test a single rent amount, `calculate_move_in_costs` for liquidity requirements, or `rank_housing_options` to compare multiple properties.


## Available Tools (4)
- **analyze_budget_feasibility**: Determine if a single proposed rent amount is sustainable based on the user's current financial profile
- **calculate_move_in_costs**: Calculate the total liquidity required to initiate a new lease
- **generate_affordability_report**: Provide a comprehensive summary of a specific housing scenario
- **rank_housing_options**: Compare multiple potential rental properties and rank them by financial suitability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rent Affordability Scenario** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I earn $5000 net. My debts are $400, utilities are $200, commute is $150, and food is $500. I want to save 20%. Is a $1500 rent affordable?"

**🤖 AI Agent:**
> With a $1500 rent, your housing share is 30%. After all expenses and your 20% savings goal ($1000), you will have $1750 leftover each month. This is sustainable.

---

**👤 You:**
> "How much cash do I need upfront for a $2000 apartment with a 2-month security deposit and $300 in application fees?"

**🤖 AI Agent:**
> You will need $4300 upfront ($2000 for first month, $4000 for security deposit, and $300 for fees).

---

**👤 You:**
> "Compare these options: 'Sunset Lofts' at $1800, 'Park View' at $2100, and 'City Center' at $1600. My net income is $4000 and I have $500 in monthly expenses."

**🤖 AI Agent:**
> The ranked options are: 1. 'City Center' (affordability score: $1900), 2. 'Sunset Lofts' (affordability score: $1700), 3. 'Park View' (affordability score: $1400).


## ❓ FAQ

**Q: How does the tool calculate sustainability?**
Sustainability is determined by checking if the monthly leftover cash remains zero or greater after subtracting rent, debts, utilities, commute, essential living costs, and the target savings rate from the net income.

**Q: Can I compare multiple apartments at once?**
Yes, you can use `rank_housing_options` to provide a list of potential properties and receive a ranked list based on which option leaves you with the most monthly cash.

**Q: What is included in the upfront cash calculation?**
The `calculate_move_in_costs` tool calculates the sum of the first month's rent, the security deposit (based on your multiplier), and any additional move-in fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rent-affordability-scenario](https://vinkius.com/en/ai-agent-connect/rent-affordability-scenario)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rent Affordability Scenario** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rent-affordability-scenario` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rent Affordability Scenario** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rent-affordability-scenario": {
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
