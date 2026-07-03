# Subscription Cashflow Aligner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/subscription-cashflow-aligner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Find the safest day of the month to set subscription billing dates and minimize overdrafts.

## Description
The Subscription Cashflow Aligner helps you synchronize your recurring expenses with your primary income. By using tools like `find_best_subscription_day`, you can identify the optimal date for subscriptions to prevent account overdrafts. The server also provides `evaluate_billing_day` to test specific dates in isolation and `summarize_cashflow_health` to assess your overall financial stability based on fixed outflows.


## Available Tools (3)
- **summarize_cashflow_health**: Summarize the overall health of your cashflow
- **evaluate_billing_day**: Evaluate if a specific subscription day is safe
- **find_best_subscription_day**: Find the optimal day for a subscription to minimize overdrafts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subscription Cashflow Aligner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best day to set my Netflix subscription if I get paid on the 5th and have rent on the 1st?"

**🤖 AI Agent:**
> The safest day to set your Netflix billing is Day 6. Setting it on Day 1 results in a 2-day overdraft.

---

**👤 You:**
> "Check if moving my gym membership to the 15th is safe given my current expenses."

**🤖 AI Agent:**
> Yes, moving your gym membership to Day 15 is safe; it results in zero overdraft days for the month.

---

**👤 You:**
> "How healthy is my current cashflow with $3000 income and $2500 in fixed costs?"

**🤖 AI Agent:**
> Your current risk level is LOW_MARGIN, as your fixed outflows consume over 80% of your monthly income.


## ❓ FAQ

**Q: How does the tool determine the best day?**
The `find_best_subscription_day` tool simulates every day from 1 to 30, calculating how many days your balance would drop below zero for each date, and selects the one with the fewest overdrafts.

**Q: Can I test a single subscription change?**
Yes, use the `evaluate_billing_day` tool to simulate the impact of moving one specific subscription to a proposed date without changing others.

**Q: What does 'cashflow health' mean?**
Using `summarize_cashflow_health`, you can see your liquidity level (e.g., STABLE or CRITICAL) based on how much of your income is consumed by fixed monthly expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/subscription-cashflow-aligner](https://vinkius.com/mcp/subscription-cashflow-aligner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subscription Cashflow Aligner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subscription-cashflow-aligner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subscription Cashflow Aligner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subscription-cashflow-aligner": {
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
