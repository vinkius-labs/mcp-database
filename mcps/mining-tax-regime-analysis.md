# Mining Tax Regime Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mining-tax-regime-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify fiscal impact, government take, and effective tax rates for mining projects.

## Description
This MCP server provides an analytical engine to quantify the fiscal impact of taxation, royalties, and incentives on mining project economics. It allows users to calculate the effective tax rate, determine the total government take, and evaluate after-tax project economics. Use `get_project_tax_summary` to assess the total tax burden, `calculate_depreciation_impact` to model asset depreciation, `evaluate_incentive_impact` to account for tax holidays, and `simulate_project_economics` to find the final net profit for investors.


## Available Tools (4)
- **calculate_depreciation_impact**: Determines how much the depreciation of mining equipment affects taxable income
- **evaluate_incentive_impact**: Calculates how tax holidays or specific incentives modify the final tax liability
- **get_project_tax_summary**: Provides a high-level overview of the total tax burden and government involvement
- **simulate_project_economics**: Provides the final remaining value for investors after all fiscal obligations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mining Tax Regime Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total tax burden for a project with 100M revenue, 40M operating costs, 30% corporate tax, 5% mining tax, and 3% royalty?"

**🤖 AI Agent:**
> The total tax paid is 28,000,000, resulting in an effective tax rate of 46.67% and a government take of 28%.

---

**👤 You:**
> "Calculate the net profit for a project with 50M revenue, 20M operating costs, 5M depreciation, and 10M total taxes."

**🤖 AI Agent:**
> The net profit for the project is 15,000,000 with a profit margin of 30%.

---

**👤 You:**
> "How much depreciation is there for a 10M asset with a 5 year useful life in year 2?"

**🤖 AI Agent:**
> The annual depreciation amount is 2,000,000, and the remaining asset value is 6,000,000.


## ❓ FAQ

**Q: How do I calculate the government take?**
You can use the `get_project_tax_summary` tool to calculate the total government take by providing revenue, operating costs, and tax rates.

**Q: Can I model tax holidays?**
Yes, the `evaluate_incentive_impact` tool allows you to determine if a tax holiday is active and how it modifies your tax liability.

**Q: How is depreciation handled?**
The `calculate_depreciation_impact` tool calculates annual depreciation based on asset value and useful life to determine its impact on taxable income.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mining-tax-regime-analysis](https://vinkius.com/ai-agent-connect/mining-tax-regime-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mining Tax Regime Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mining-tax-regime-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mining Tax Regime Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mining-tax-regime-analysis": {
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
