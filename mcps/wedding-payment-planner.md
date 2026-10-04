# Wedding Payment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wedding-payment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate payment timelines, cash flow forecasts, and budget summaries for wedding planning.

## Description
This MCP server provides essential financial tools for wedding planning. It allows AI agents to organize vendor obligations into a monthly `get_payment_calendar`, forecast liquid cash requirements using `get_cash_flow_forecast`, estimate guest-dependent costs with `estimate_variable_costs`, and provide a final financial overview via `calculate_budget_summary`. It helps ensure wedding budgets are managed effectively by tracking deposits, balances, and contingency reserves.


## Available Tools (4)
- **calculate_budget_summary**: Provides a high-level overview of the remaining budget after all planned expenses and contingencies
- **estimate_variable_costs**: Calculates the projected costs for guest-dependent items like catering and venue per-head fees
- **get_cash_flow_forecast**: Determines the cumulative amount of liquid cash needed before each specific due date
- **get_payment_calendar**: Generates a chronological timeline of all required payments organized by month


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Payment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my wedding payment schedule for 2025."

**🤖 AI Agent:**
> January 2025: $500 (1 payment)
February 2025: $1,200 (2 payments)

---

**👤 You:**
> "How much cash do I need to have ready by June 15th, 2025?"

**🤖 AI Agent:**
> You will need a cumulative total of $3,500 in liquid cash by June 15th, 2025, to cover all vendor obligations up to that date.

---

**👤 You:**
> "What is my remaining budget after all expenses and a 10% contingency?"

**🤖 AI Agent:**
> After accounting for all vendor payments, guest costs, and your 10% contingency reserve, you have $1,500 remaining in your budget.


## ❓ FAQ

**Q: How can I see my monthly wedding expenses?**
You can use the `get_payment_calendar` tool to generate a chronological timeline of all vendor payments organized by month.

**Q: How do I know if I have enough cash for upcoming vendor payments?**
The `get_cash_flow_forecast` tool calculates the cumulative cash needed before each due date, helping you manage liquidity.

**Q: Can I estimate costs for catering based on my guest list?**
Yes, the `estimate_variable_costs` tool calculates projected costs for guest-dependent items like catering, including a buffer for fluctuations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wedding-payment-planner](https://vinkius.com/en/ai-agent-connect/wedding-payment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Payment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-payment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Payment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-payment-planner": {
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
