# U.S. Treasury Full — Complete Fiscal & Debt Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-treasury-full-complete-fiscal-debt-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The definitive U.S. Treasury Mega-Server: 13 tools covering national debt ($34T+), interest rates, auction results, federal budget accounting (revenue, spending, deficit), daily cash balances, and official exchange rates. Total access to the financial pulse of the U.S. government without API keys.

## Description
The **ultimate U.S. Treasury Mega-Server** — 13 tools.

### 13 Tools
- 💸 Debt (3) — National debt to penny, interest rates, auctions
- 🏛️ Budget (4) — Deficit, revenue, spending, internal daily cash
- 🌍 FX (2) — Exchange rates & history
- 🛠️ Generic (4) — Query any Fiscal Data API endpoint

### Zero Authentication


## Available Tools (13)
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
- **get_national_debt**: S. national debt (Total Public Debt Outstanding) updated daily by the Treasury Department. Breaks down into Debt Held by the Public (marketable securities) and Intragovernmental Holdings (trust funds like Social Security). As of 2026, the national debt exceeds $39 trillion.

Get the U.S. national debt to the penny — updated daily
- **get_debt_history**: Format: YYYY-MM-DD. Useful for tracking debt growth over specific periods — fiscal years, election cycles, presidencies, economic crises.

Get national debt for a specific date range
- **get_public_debt_breakdown**: Shows both Debt Held by the Public and Intragovernmental Holdings.

Get the Statement of Public Debt — breakdown by security type
- **get_avg_interest_rates**: These rates reflect the cost of borrowing for the federal government. Updated monthly.

Get average interest rates on U.S. Treasury securities
- **get_treasury_auctions**: The bid-to-cover ratio indicates investor demand — higher ratios = stronger demand for U.S. debt.

Get results of Treasury securities auctions — Bills, Notes, Bonds
- **get_treasury_exchange_rates**: Updated quarterly. Covers 170+ currencies against the U.S. dollar. These are the official rates used for government accounting and reporting.

Get official Treasury exchange rates for 170+ currencies
- **get_exchange_rate_for_currency**: Use the currency name or country (e.g., "Euro", "Japan-Yen", "Brazil-Real", "United Kingdom-Pound"). Updated quarterly.

Get Treasury exchange rate history for a specific currency
- **query_treasury_dataset**: treasury.gov. Provide the API endpoint path (e.g., /v2/accounting/od/debt_to_penny). Supports filter, sort, fields, and pagination parameters. See fiscaldata.treasury.gov for all available datasets.

Query any Treasury Fiscal Data dataset by endpoint path


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Treasury Full — Complete Fiscal & Debt Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a complete summary of the U.S. fiscal state: current debt, latest deficit, and cash balance."

**🤖 AI Agent:**
> 📊 **U.S. Treasury: Fiscal State Overview**

- National Debt: $34,812,456,789.12
- Fiscal Year Deficit to Date: $845,000,000,000
- Current Treasury Cash Balance: $825,443,000,000

---

**👤 You:**
> "Extract federal spending vs federal revenue for the last 6 months"

**🤖 AI Agent:**
> 📊 **U.S. Federal Revenues vs. Outlays (6 Months)**

- Mar 2026: Revenue $354B | Outlays $492B | Deficit $138B
- Feb 2026: Revenue $271B | Outlays $567B | Deficit $296B
- Jan 2026: Revenue $477B | Outlays $455B | Surplus $22B

---

**👤 You:**
> "Show historic exchange rates for USD -> GBP to analyze currency fluctuations"

**🤖 AI Agent:**
> 📊 **Historical Rates: UK (Pound Sterling)**

- Mar 2026: 0.79 GBP per 1 USD
- Dec 2025: 0.78 GBP per 1 USD
- Sep 2025: 0.82 GBP per 1 USD


## ❓ FAQ

**Q: Why build a mega server?**
Because an AI agent performs better when all context is centralized. By combining Debt, FX and Budget into one tool suite, the prompt routing evaluates economic dependencies efficiently.

**Q: Is there an API Rate Limit?**
No official API key is required, however they rate limit by IP if abused. This server utilizes graceful error handling.

**Q: Are these figures inflation adjusted?**
Values are nominal as recorded by accounting ledgers. The AI agent must query CPI (Consumer Price Index) if adjustment is required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-treasury-full-complete-fiscal-debt-intelligence](https://vinkius.com/mcp/us-treasury-full-complete-fiscal-debt-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **U.S. Treasury Full — Complete Fiscal & Debt Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-treasury-full-complete-fiscal-debt-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **U.S. Treasury Full — Complete Fiscal & Debt Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-treasury-full-complete-fiscal-debt-intelligence": {
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
