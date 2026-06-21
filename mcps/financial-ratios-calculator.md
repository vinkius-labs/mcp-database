# Financial Ratios Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/financial-ratios-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate essential financial health indicators including liquidity, solvency, and interest coverage ratios.

## Description
This MCP server provides specialized tools to quantify a company's financial stability. Use `get_short_term_liquidity_ratios` to determine how well a business can meet upcoming debt obligations using current assets and inventories. You can also use `get_long_term_solvency_ratios` to evaluate long-term capital structure through general liquidity and debt-to-equity ratios, or `get_interest_coverage_ratio` to assess the ability to service interest expenses from operating profits.


## Available Tools
- **get_interest_coverage_ratio**: Calculate interest coverage ratio
- **get_short_term_liquidity_ratios**: Calculate short-term liquidity ratios
- **get_long_term_solvency_ratios**: Calculate long-term solvency ratios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Financial Ratios Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my short-term liquidity ratios. I have 5000 in current assets, 2000 in inventory, 1000 in cash, and 2500 in current liabilities."

**🤖 AI Agent:**
> Your current ratio is 2.0, your quick ratio is 1.2, and your immediate ratio is 0.4.

---

**👤 You:**
> "What is my interest coverage ratio if my EBIT is 10000 and my interest expense is 2000?"

**🤖 AI Agent:**
> Your interest coverage ratio is 5.0, with a coverage margin of 80%.

---

**👤 You:**
> "Check my long-term solvency. Current assets: 10000, Non-current assets: 20000, Current liabilities: 5000, Non-current liabilities: 10000, Total equity: 15000."

**🤖 AI Agent:**
> Your general liquidity ratio is 2.0 and your debt-to-equity ratio is 1.0.


## ❓ FAQ

**Q: What financial ratios can I calculate?**
You can calculate short-term liquidity ratios (current, quick, and immediate), long-term solvency ratios (general liquidity and debt-to-equity), and interest coverage ratios.

**Q: What inputs are required for the liquidity tool?**
To use `get_short_term_liquidity_ratios`, you need to provide current assets, inventories, cash and equivalents, and current liabilities.

**Q: Does this tool handle errors like division by zero?**
Yes, the tools are designed to return error messages if inputs would result in invalid calculations, such as dividing by zero or using negative values for assets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/financial-ratios-calculator](https://vinkius.com/mcp/financial-ratios-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Financial Ratios Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `financial-ratios-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Financial Ratios Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "financial-ratios-calculator": {
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
