# Asset Valuation DCF MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/asset-valuation-dcf)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate oil and gas asset NPV using discounted cash flow analysis.

## Description
This MCP server provides specialized tools for upstream oil and gas economic modeling. It allows AI agents to perform complex discounted cash flow (DCF) valuations by processing production forecasts, price decks, and cost estimates. Users can calculate the primary Net Present Value (NPV) using `calculate_asset_value`, perform sensitivity analysis on economic drivers with `analyze_sensitivity`, compare values against industry benchmarks via `get_comparable_multiples`, and assess production viability with `evaluate_reserves_longevity`.


## Available Tools (4)
- **calculate_asset_value**: Calculates the primary Net Present Value (NPV) of the oil and gas asset
- **evaluate_reserves_longevity**: Assesses the economic viability and duration of the asset's production
- **get_comparable_multiples**: Compares the calculated asset value against industry-standard metrics
- **analyze_sensitivity**: Determines how sensitive the asset's value is to changes in critical economic drivers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Asset Valuation DCF** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the NPV for an asset with a production forecast of 100 units in year 1 and 50 units in year 2, a price deck of [80, 75], costs of 10 per year, and a 10% discount rate."

**🤖 AI Agent:**
> The calculated Net Present Value (NPV) for the asset is $11,363.64.

---

**👤 You:**
> "What are the comparable multiples for an asset valued at $500M with 100M barrels of total production?"

**🤖 AI Agent:**
> The value per unit of production is $5.00.

---

**👤 You:**
> "How long will this asset remain economically viable if revenue is [100, 80, 60, 40] and operating costs are [50, 50, 50, 50]?"

**🤖 AI Agent:**
> The asset has an economic life of 3 years.


## ❓ FAQ

**Q: What is the primary use case for this server?**
It is used to estimate the economic worth of oil and gas assets through discounted cash flow modeling and sensitivity testing.

**Q: Can I test how price changes affect my asset value?**
Yes, you can use the `analyze_sensitivity` tool to determine how shifts in variables like the price deck impact the total NPV.

**Q: How does the tool handle terminal value?**
The `calculate_asset_value` tool accepts an optional terminal value parameter to account for the asset's worth at the end of the forecast period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/asset-valuation-dcf](https://vinkius.com/en/ai-agent-connect/asset-valuation-dcf)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Asset Valuation DCF** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `asset-valuation-dcf` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Asset Valuation DCF** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "asset-valuation-dcf": {
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
