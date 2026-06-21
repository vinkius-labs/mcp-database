# U.S. Treasury Budget — Federal Revenue, Spending & Deficit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-treasury-budget-federal-revenue-spending-deficit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track the U.S. Federal Government's wallet. Access daily Treasury cash balances, monthly and yearly federal revenue/spending, and track the ongoing multi-trillion dollar budget deficit.

## Description
U.S. Treasury budget data.

### 4 Tools
- **Federal Deficit** — Monthly surplus/deficit tracking
- **Federal Revenue** — Government income sources
- **Federal Spending** — Government expenditure
- **Daily Cash Balance** — The U.S. government's checking account

### Zero Auth


## Available Tools
- **get_federal_revenue**: Shows current month and fiscal-year-to-date totals vs. prior year.

Get federal government revenue — tax receipts by source
- **get_federal_spending**: Shows current month gross outlays vs. prior year.

Get federal government spending by department and agency
- **get_deficit_surplus**: The U.S. fiscal year runs October 1 through September 30.

Get the federal budget deficit or surplus — fiscal year to date
- **get_daily_cash_balance**: This is the government's daily bank statement — how much cash the U.S. has on hand.

Get the daily operating cash balance of the U.S. Treasury
- **get_daily_debt_transactions**: Shows today, month-to-date, and fiscal-year-to-date amounts. Reveals the daily mechanics of how the U.S. finances its operations.

Get daily public debt transactions — issuance and redemptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Treasury Budget — Federal Revenue, Spending & Deficit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current U.S. budget deficit?"

**🤖 AI Agent:**
> 📊 **U.S. Federal Deficit**

For Fiscal Year 2025:
Total Deficit: $1,695,432,100,000
This represents the gap between $4.8T in revenue and $6.5T in outlays.

---

**👤 You:**
> "How much did the U.S. government collect in revenue last month?"

**🤖 AI Agent:**
> 📊 **Federal Revenue**

Total collections (March 2026): $354,112,000,000
Top Sources:
1. Individual Income Taxes: $192B
2. Social Insurance Taxes: $124B
3. Corporate Income Taxes: $22B

---

**👤 You:**
> "What is the daily Treasury cash balance?"

**🤖 AI Agent:**
> 📊 **Daily Treasury Statement**

Operating Cash Balance as of 2026-04-01:
- Total Balance: $825,443,000,000
- Federal Reserve Account: $820,111,000,000
- Tax and Loan Accounts: $5,332,000,000


## ❓ FAQ

**Q: What is the Daily Treasury Statement?**
It acts as the U.S. government's daily checking account statement, showing cash deposits and withdrawals.

**Q: When does the fiscal year start?**
The U.S. government fiscal year begins on October 1 and ends on September 30.

**Q: Is defense spending tracked here?**
Yes, the Monthly Treasury Statement provides outlays by agency, including the Department of Defense.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-treasury-budget-federal-revenue-spending-deficit](https://vinkius.com/mcp/us-treasury-budget-federal-revenue-spending-deficit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **U.S. Treasury Budget — Federal Revenue, Spending & Deficit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-treasury-budget-federal-revenue-spending-deficit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **U.S. Treasury Budget — Federal Revenue, Spending & Deficit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-treasury-budget-federal-revenue-spending-deficit": {
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
