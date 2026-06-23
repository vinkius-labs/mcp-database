# U.S. Treasury Debt — National Debt & Interest Rates MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-treasury-debt-national-debt-interest-rates)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access real-time data on the U.S. National Debt (currently $34T+). Retrieve 'Debt to the Penny', monitor average interest rates on Treasury securities, and access results from Treasury auctions.

## Description
U.S. Treasury debt data.

### 3 Tools
- **National Debt** — Debt to the Penny ($34T+)
- **Interest Rates** — Average interest rates on U.S. debt
- **Treasury Auctions** — Auction results for Bills, Notes, and Bonds

### Zero Auth


## Available Tools (5)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Treasury Debt — National Debt & Interest Rates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the exact current U.S. National debt?"

**🤖 AI Agent:**
> 📊 **U.S. Treasury: Debt to the Penny**

The most recent data (2026-03-31):
- Total Public Debt Outstanding: $34,812,456,789.12
- Intragovernmental Holdings: $7,123,456,789.12
- Debt Held by the Public: $27,689,000,000.00

---

**👤 You:**
> "What is the average interest rate on Treasury Bills?"

**🤖 AI Agent:**
> 📊 **U.S. Treasury Average Interest Rates**

Average interest rates for March 2026:
- Treasury Bills: 5.12%
- Treasury Notes: 4.58%
- Treasury Bonds: 4.75%

---

**👤 You:**
> "Show me the result of the last Treasury auction"

**🤖 AI Agent:**
> 📊 **Treasury Auctions**

Recent 10-Year Treasury Note Auction (2026-03-15):
- Amount Accepted: $42,000,000,000
- High Yield: 4.25%
- Bid-to-Cover Ratio: 2.54


## ❓ FAQ

**Q: What is 'Debt to the Penny'?**
It is the exact daily public debt of the United States, updated each business day. It includes all Treasury securities issued to the public.

**Q: How often are the interest rates updated?**
Average interest rates are typically reported at the end of each month.

**Q: Do I need authentication?**
No, all Treasury Fiscal Data API endpoints are public and do not require API keys.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-treasury-debt-national-debt-interest-rates](https://vinkius.com/mcp/us-treasury-debt-national-debt-interest-rates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **U.S. Treasury Debt — National Debt & Interest Rates** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-treasury-debt-national-debt-interest-rates` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **U.S. Treasury Debt — National Debt & Interest Rates** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-treasury-debt-national-debt-interest-rates": {
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
