# Contract Income Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/contract-income-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forecast monthly contractor income based on contract dates, rates, and payment terms.

## Description
This MCP server provides precise financial planning for contractors. It calculates monthly income projections by analyzing contract lifecycles, hourly billing, and tax obligations. Use `get_monthly_forecast` to see a month-by-month breakdown of gross and net income, or `get_cash_flow_timing` to determine exactly when funds will hit your bank account based on specific payment terms. It also identifies potential income gaps using `get_gap_analysis` and provides aggregate totals via `get_contract_summary`.


## Available Tools (4)
- **get_cash_flow_timing**: Answers when money will actually hit the bank account
- **get_contract_summary**: Answers how much total income is expected from current contracts
- **get_gap_analysis**: Identifies months with no income
- **get_monthly_forecast**: Provides a month-by-month breakdown of projected income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contract Income Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my projected monthly income and net income after a 25% tax rate for the next six months."

**🤖 AI Agent:**
> January 2024: Gross $5,000, Tax $1,250, Net $3,750. February 2024: Gross $5,000, Tax $1,250, Net $3,750...

---

**👤 You:**
> "When will I actually receive my money for the work done in March 2024?"

**🤖 AI Agent:**
> Based on your 30-day payment terms, the income earned in March 2024 is expected to hit your bank account in April 2024.

---

**👤 You:**
> "How much total net income am I expected to earn from my current contracts?"

**🤖 AI Agent:**
> Your total expected net income from all current contracts is $15,500.


## ❓ FAQ

**Q: How does the tool handle tax calculations?**
You can specify a tax rate in the `get_monthly_forecast` tool to calculate your net income after tax reserves.

**Q: What is the difference between earned income and cash flow?**
Earned income is what you bill for work performed, while cash flow (calculated via `get_cash_flow_timing`) accounts for the delay in receiving payments based on your contract terms.

**Q: Can I identify months where I won't have any work?**
Yes, use the `get_gap_analysis` tool to identify specific months where no gross income is projected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/contract-income-forecast](https://vinkius.com/en/ai-agent-connect/contract-income-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contract Income Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contract-income-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contract Income Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contract-income-forecast": {
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
