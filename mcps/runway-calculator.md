# Runway Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runway-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate business runway, cash exhaustion dates, and required funding to reach survival targets.

## Description
The Runway Calculator is a financial forecasting tool designed for businesses to manage liquidity. By using tools like `calculate_runway_metrics`, you can determine how many months of operational life remain based on your current cash balance and monthly burn rate. The server also provides `calculate_sustainable_burn` to find the maximum allowable spending to reach specific survival targets, `calculate_funding_required` to identify necessary capital raises, and `summarize_expenses` to aggregate individual costs into a single burn rate figure.


## Available Tools (4)
- **calculate_sustainable_burn**: Calculates the maximum allowable monthly spending to reach a specific survival target
- **calculate_funding_required**: Identifies how much new capital must be raised to achieve a specific runway goal
- **calculate_runway_metrics**: Determines the remaining operational duration and the date when funds will be exhausted
- **summarize_expenses**: Aggregates individual expense items into a single monthly burn rate figure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runway Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have $50,000 in the bank and my monthly burn rate is $5,000. How much runway do I have?"

**🤖 AI Agent:**
> You have 10 months of runway remaining. Your cash is predicted to reach zero on approximately October 24, 2025.

---

**👤 You:**
> "If I have $100,000 and want to survive for 24 months, what is my maximum sustainable burn rate?"

**🤖 AI Agent:**
> To reach a target runway of 24 months with $100,000 available, your maximum sustainable monthly burn rate is $4,166.67.

---

**👤 You:**
> "I have $20,000 left, my monthly burn is $2,000, and I want to reach 18 months of runway. How much do I need to raise?"

**🤖 AI Agent:**
> You need to raise $16,000 to achieve a target runway of 18 months.


## ❓ FAQ

**Q: How do I calculate my business runway?**
You can use the `calculate_runway_metrics` tool. Simply provide your current cash balance and your monthly burn rate to see how many months of runway you have left.

**Q: Can I calculate how much funding I need to raise?**
Yes, use the `calculate_funding_required` tool. Input your current cash balance, monthly burn rate, and your target runway duration to find the exact funding gap.

**Q: How can I aggregate my expenses?**
The `summarize_expenses` tool allows you to pass a JSON array of expense items (with categories and amounts) to calculate your total monthly burn rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runway-calculator](https://vinkius.com/mcp/runway-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runway Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `runway-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runway Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runway-calculator": {
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
