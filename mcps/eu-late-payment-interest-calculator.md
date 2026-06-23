# EU Late Payment Interest Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-late-payment-interest-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate interest and fixed compensation for overdue commercial payments according to the EU Late/Late Payment Directive (2011/7/EU).

## Description
This MCP server provides a precise way to calculate the financial burden of late B2B payments in the European Union. It automates the complex process of determining interest accrual based on the ECB reference rate plus an 8% margin, as mandated by the EU Late Payment Directive (2011/7/EU). You can use `calculate_accrued_interest` to find the variable cost of delay, `calculate_fixed_compensation` to determine the fixed administrative recovery fee based on debt tiers, or `get_total_overdue_cost` for a comprehensive view of both interest and compensation.


## Available Tools (3)
- **calculate_accrued_interest**: You need the original invoice amount, the due date, and the current calculation date.

Calculates the interest accrued on an unpaid invoice based on the EU Late Payment Directive
- **calculate_fixed_compensation**: The amount depends on the total value of the outstanding debt.

Calculates the fixed administrative recovery fee for an overdue payment
- **get_total_overdue_cost**: Calculates the total financial burden, including both accrued interest and fixed compensation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Late Payment Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much interest has accumulated on an invoice of €500 that was due on 2024-01-01, calculated as of 2024-06-01?"

**🤖 AI Agent:**
> The interest accrued is €35.89, and the total days overdue is 152 days.

---

**👤 You:**
> "What is the fixed compensation for a debt of €1500?"

**🤖 AI Agent:**
> The fixed administrative recovery fee for an invoice of €1500 is €100.

---

**👤 You:**
> "Calculate the total cost for a €2000 invoice due on 2023-12-01, with calculation date 2024-03-01."

**🤖 AI Agent:**
> The total financial burden is €175.42, consisting of €75.42 in interest and €100.00 in fixed compensation.


## ❓ FAQ

**Q: How is the interest rate determined?**
The tool uses the European Central Bank (ECB) reference rate for the relevant period and adds a fixed margin of 8 percentage points, as required by EU law.

**Q: What is the fixed compensation amount?**
The compensation amount depends on the invoice value: €40 for small debts, €70 for medium debts, and €100 for large debts.

**Q: Can I calculate the total cost in one go?**
Yes, use the `get_total_overdue_cost` tool to receive a breakdown of both interest and compensation along with the final grand total.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-late-payment-interest-calculator](https://vinkius.com/mcp/eu-late-payment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU Late Payment Interest Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eu-late-payment-interest-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU Late Payment Interest Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-late-payment-interest-calculator": {
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
