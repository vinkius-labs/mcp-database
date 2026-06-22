# Investment Profitability Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/investment-profitability-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare net returns of CDB, Treasury Selic, Savings, and DI Funds after regressive income tax.

## Description
This MCP server provides an analytical engine to compare the net profitability of various fixed-income instruments. By using tools like `compare_all_instruments`, you can see a side-by-side comparison of CDB, Treasury Selic, Savings, and DI Funds after applying the Brazilian regressive income tax schedule based on your investment duration.


## Available Tools (3)
- **get_tax_rate_by_duration**: Retrieves the specific income tax percentage applicable based on duration
- **calculate_net_profit**: Returns profitability breakdown.

Calculates the gross profit, tax amount, and net profit for a specific investment setup
- **compare_all_instruments**: Provides a side-by-side comparison of all supported investment types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Investment Profitability Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare all investments for $10,000 over 400 days with a 12% CDI."

**🤖 AI Agent:**
> For a $10,000 investment over 400 days at 12% CDI, the net results are: CDB (100% CDI): $1,035.20, Treasury Selic: $1,035.20, Savings: $850.00, DI Fund: $1,035.20.

---

**👤 You:**
> "What is the tax rate for an investment held for 200 days?"

**🤖 AI Agent:**
> The applied income tax percentage for 200 days is 17.5%.

---

**👤 You:**
> "Calculate net profit for $5,000 at 11% CDI for 800 days with a 100% multiplier."

**🤖 AI Agent:**
> The gross profit is $440.00, the tax amount is $88.00, and the final net profit is $352.00.


## ❓ FAQ

**Q: How does the tax calculation work?**
The tool uses a regressive tax table where the percentage decreases as the investment duration increases.

**Q: Which instruments are supported?**
Supported instruments include CDB, Treasury Selic, Savings (Poupança), and DI Funds.

**Q: Can I calculate profit for a specific amount?**
Yes, use the `calculate_net_profit` tool by providing your principal amount, days held, and CDI rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/investment-profitability-comparator](https://vinkius.com/mcp/investment-profitability-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Investment Profitability Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `investment-profitability-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Investment Profitability Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "investment-profitability-comparator": {
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
