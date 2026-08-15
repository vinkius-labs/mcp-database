# Sharpe Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sharpe-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic risk-adjusted performance engine for financial metrics.

## Description
This MCP server provides a deterministic engine for calculating critical risk-adjusted performance metrics. It allows AI agents to evaluate investment efficiency using tools like `calculate_risk_adjusted_ratios` for Sharpe, Sortino, Treynor, and Information ratios, and `calculate_volatility_and_drawdown` for analyzing annualized returns, volatility, and maximum drawdown. It is designed for precise financial analysis using periodic return arrays.


## Available Tools (3)
- **calculate_risk_adjusted_ratios**: Calculate Sharpe, Sortino, Treynor, and Information ratios
- **calculate_volatility_and_drawdown**: Calculate annualized return, volatility, and max drawdown
- **get_periodic_constants**: Get standard period constants


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sharpe Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Sharpe Ratio for these returns: [0.01, 0.02, -0.01, 0.015, 0.005] with a 2% annualized risk-free rate and 252 periods per year."

**🤖 AI Agent:**
> The annualized Sharpe Ratio for the provided returns is 0.45.

---

**👤 You:**
> "What is the maximum drawdown for a series of returns: [0.05, -0.10, 0.02, 0.03, -0.05] using 12 periods per year?"

**🤖 AI Agent:**
> The maximum drawdown for this series is 14.5%.

---

**👤 You:**
> "Get the standard period constants for annualization."

**🤖 AI Agent:**
> The standard constants are: daily (252), weekly (52), and monthly (12).


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate the Sharpe Ratio, Sortino Ratio, Treynor Ratio, Information Ratio, annualized return, annualized volatility, and maximum drawdown using `calculate_risk_adjusted_ratios` and `calculate_volatility_and_drawdown`.

**Q: How should I format the returns input?**
Returns should be provided as an array of decimal numbers. For example, a 1% return should be entered as 0.01.

**Q: What are the supported annualization periods?**
The server uses standard financial constants: 252 for daily, 52 for weekly, and 12 for monthly. You can retrieve these using `get_periodic_constants`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sharpe-ratio-calculator](https://vinkius.com/mcp/sharpe-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sharpe Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sharpe-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sharpe Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sharpe-ratio-calculator": {
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
