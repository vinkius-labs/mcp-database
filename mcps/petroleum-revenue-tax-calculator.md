# Petroleum Revenue Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/petroleum-revenue-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates petroleum revenue tax (PRT) liability and after-tax cash flow.

## Description
This MCP server provides tools to calculate Petroleum Revenue Tax (PRT) and net liquidity for petroleum operators. It handles the full fiscal sequence, including calculating taxable profit using `get_taxable_profit`, determining tax liability with `calculate_prt_liability`, and finding final cash flow via `calculate_after_tax_cash_flow`. It also provides revenue breakdowns using `get_revenue_summary`.


## Available Tools (4)
- **calculate_prt_liability**: Calculates the specific tax amount owed to the government
- **get_revenue_summary**: Provides a high-level breakdown of total revenue components
- **get_taxable_profit**: Determines the profit amount subject to taxation
- **calculate_after_tax_cash_flow**: Determines the net liquidity available to the operator


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petroleum Revenue Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the taxable profit for a project with 1000 gross revenue, 100 oil allowance, 200 operating costs, and 150 capital allowances?"

**🤖 AI Agent:**
> The taxable profit is 550.

---

**👤 You:**
> "Calculate the PRT liability for a taxable profit of 500 with a tax rate of 0.35."

**🤖 AI Agent:**
> The PRT liability is 175.

---

**👤 You:**
> "What is the after-tax cash flow if gross revenue is 1000, operating costs are 200, and PRT liability is 175?"

**🤖 AI Agent:**
> The after-tax cash flow is 625.


## ❓ FAQ

**Q: How do I calculate the taxable profit?**
You can use the `get_taxable_profit` tool by providing the gross revenue, oil allowance, operating costs, and capital allowances.

**Q: Can I calculate the final cash flow?**
Yes, use the `calculate_after_tax_cash_flow` tool with the gross revenue, operating costs, and the calculated PRT liability.

**Q: What is included in the gross revenue?**
Gross revenue includes the market value of production and any tariff income, which can be summarized using `get_revenue_summary`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/petroleum-revenue-tax-calculator](https://vinkius.com/en/ai-agent-connect/petroleum-revenue-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petroleum Revenue Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petroleum-revenue-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petroleum Revenue Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petroleum-revenue-tax-calculator": {
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
