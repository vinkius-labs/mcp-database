# Dividend Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dividend-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate gross and net dividend income, annual projections, and dividend yields.

## Description
This MCP server provides essential tools for equity investors to manage dividend expectations. Use `get_gross_dividend_income` to find total cash from a single payment, `get_projected_annual_income` to estimate yearly earnings, `get_dividend_yield_impact` to calculate percentage returns, and `get_net_income_estimate` to account for withholding taxes.


## Available Tools (4)
- **get_dividend_yield_impact**: Calculate dividend yield percentage
- **get_gross_dividend_income**: Calculate total gross dividend income from share count and dividend per share
- **get_net_income_estimate**: Estimate net dividend income after taxes
- **get_projected_annual_income**: Calculate projected annual dividend income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dividend Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total cash will I receive if I have 500 shares and the dividend is $0.50 per share?"

**🤖 AI Agent:**
> You will receive a total of $250.00.

---

**👤 You:**
> "What is the dividend yield if the dividend is $2.00 and the stock price is $50.00?"

**🤖 AI Agent:**
> The dividend yield is 4.0%.

---

**👤 You:**
> "If I have 100 shares with a $1.00 dividend and a 15% tax rate, what is my net income?"

**🤖 AI Agent:**
> Your net income after taxes will be $85.00.


## ❓ FAQ

**Q: How do I calculate my total dividend income?**
You can use the `get_gross_dividend_income` tool by providing your total share count and the dividend amount per share.

**Q: Does this tool account for taxes?**
Yes, the `get_net_income_estimate` tool allows you to input a tax rate to see your actual cash after withholding taxes.

**Q: Can I project my yearly earnings?**
Yes, use `get_projected_annual_income` and specify how many times per year the dividend is paid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dividend-total](https://vinkius.com/en/ai-agent-connect/dividend-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dividend Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dividend-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dividend Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dividend-total": {
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
