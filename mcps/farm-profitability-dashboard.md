# Farm Profitability Dashboard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/farm-profitability-dashboard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate comprehensive farm profitability, EBITDA, and crop efficiency metrics.

## Description
The Farm Profitability Dashboard provides a detailed financial analysis of your harvest. By using tools like `get_crop_economic_breakdown`, you can see the revenue, COGS, and contribution margin for each individual crop. The `get_farm_financials` tool calculates your total gross revenue, EBITDA, and ROI, accounting for both variable production costs and fixed property expenses. Additionally, use `get_area_efficiency_and_ranking` to analyze land efficiency through profit per hectare and identify which crops are performing best via a profitability ranking.


## Available Tools (3)
- **get_area_efficiency_and_ranking**: Analyzes land efficiency and crop ranking
- **get_crop_economic_breakdown**: Calculates revenue, cost, and margin for each specific crop
- **get_farm_financials**: Calculates overall financial health of the farm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Farm Profitability Dashboard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the revenue, cost, and margin for my corn and soybean crops? Fixed costs are 5000."

**🤖 AI Agent:**
> For Corn: Gross Revenue is $12,000, COGS is $8,000, and Contribution Margin is $4,000. For Soybeans: Gross Revenue is $15,000, COGS is $10,000, and Contribution Margin is $5,000.

---

**👤 You:**
> "What is the overall financial health of my farm?"

**🤖 AI Agent:**
> Your total gross revenue is $27,000, your farm EBITDA is $12,000, and your Return on Investment (ROI) is 44.4%.

---

**👤 You:**
> "Which of my crops should I prioritize for the next season based on efficiency?"

**🤖 AI Agent:**
> Based on your data, Soybeans are your top performer with a higher contribution margin percentage, followed by Corn.


## ❓ FAQ

**Q: How can I see the margin for each specific crop?**
Use the `get_crop_economic_breakdown` tool by providing a JSON array of your crops data and your total fixed costs.

**Q: How is the farm's overall EBITDA calculated?**
The `get_farm_financials` tool calculates EBITDA by subtracting both the variable production costs of all crops and your total fixed property costs from your total gross revenue.

**Q: Can I identify which crops are most profitable per hectare?**
Yes, the `get_area_efficiency_and_ranking` tool provides profit per hectare and a ranking of crops based on their contribution margin percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/farm-profitability-dashboard](https://vinkius.com/mcp/farm-profitability-dashboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Farm Profitability Dashboard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `farm-profitability-dashboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Farm Profitability Dashboard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "farm-profitability-dashboard": {
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
