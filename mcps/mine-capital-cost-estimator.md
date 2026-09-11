# Mine Capital Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mine-capital-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates pre-production and sustaining CAPEX for mining projects.

## Description
This MCP server provides specialized tools for mining project financial planning. It allows users to calculate pre-production CAPEX using factorial, parametric, or detailed methods, and estimate sustaining CAPEX over a mine's lifecycle. Users can retrieve regional cost adjustments via `get_location_multiplier` and perform complex financial adjustments using `apply_currency_and_inflation` to account for inflation and currency fluctuations.


## Available Tools (4)
- **apply_currency_and_inflation**: Adjusts a base cost figure for inflation and converts it to a specified currency
- **estimate_pre_production_capex**: Calculates the total initial capital required to start mining operations
- **estimate_sustaining_capex**: Predicts the ongoing capital needed to maintain the mine throughout its lifecycle
- **get_location_multiplier**: Retrieves the cost adjustment factor for a specific geographic region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Capital Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate the pre-production CAPEX for an open pit mine with a capacity of 5,000,000 tonnes per year and a location factor of 1.2 using the parametric method."

**🤖 AI Agent:**
> The estimated pre-production CAPEX for the open pit mine is $450,000,000, including a $45,000,000 contingency allowance.

---

**👤 You:**
> "What is the annual sustaining CAPEX for an underground mine with 2,000,000 tonnes annual capacity and a 15-year mine life with a 0.05 equipment replacement rate?"

**🤖 AI Agent:**
> The annual sustaining CAPEX is $12,500,000, with a total lifetime sustaining CAPEX of $187,500,000.

---

**👤 You:**
> "Get the location multiplier for Australia."

**🤖 AI Agent:**
> The location multiplier for Australia is 1.15.


## ❓ FAQ

**Q: What estimation methods are supported?**
The server supports factorial, parametric, and detailed estimation methodologies via the `estimate_pre_production_capex` tool.

**Q: Can I adjust for regional cost differences?**
Yes, you can use `get_location_multiplier` to find the specific adjustment factor for a geographic region.

**Q: How does the tool handle inflation?**
The `apply_currency_and_inflation` tool applies compound inflation over a specified number of years to your base amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mine-capital-cost-estimator](https://vinkius.com/en/ai-agent-connect/mine-capital-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Capital Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-capital-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Capital Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-capital-cost-estimator": {
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
