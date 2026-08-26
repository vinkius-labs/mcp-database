# Water Rights Valuation Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/water-rights-valuation-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Economic assessment of agricultural water rights using income and market methods.

## Description
This MCP server provides specialized tools for the economic valuation of agricultural water rights. It allows users to determine the expected annual yield using `calculate_annual_yield`, estimate the total current worth via `calculate_present_value`, and evaluate competitiveness through `compare_to_market`. Additionally, it can model environmental risks using `assess_drought_impact` to adjust reliability based on drought severity. It is designed for agricultural economists and water managers to assess asset value based on allocation, reliability, and market conditions.


## Available Tools (4)
- **calculate_annual_yield**: Determines the expected economic output of the water right for a single year
- **assess_drought_impact**: Adjusts the reliability of the water right based on environmental risk factors
- **compare_to_market**: Evaluates whether the calculated value of the water right is competitive compared to current market trading prices
- **calculate_present_value**: Estimates the total current worth of the water right over its useful life


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Rights Valuation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected annual value for 500 acre-feet of water with 90% reliability and a crop value of $150 per acre-foot?"

**🤖 AI Agent:**
> The expected annual value is $67,500.

---

**👤 You:**
> "Calculate the present value for a water right with an annual value of $50,000, a 20-year utility, a 5% discount rate, and a priority factor of 1.2."

**🤖 AI Agent:**
> The present value of the water right is $754,518.15.

---

**👤 You:**
> "If the current reliability is 0.85 and the drought severity index is 0.4, what is the adjusted reliability?"

**🤖 AI Agent:**
> The adjusted reliability is 0.68.


## ❓ FAQ

**Q: How does the engine account for drought risk?**
The `assess_drought_impact` tool adjusts the reliability of a water right based on a drought severity index, reducing the expected availability of water during periods of scarcity.

**Q: Can I compare my calculated value to local market prices?**
Yes, you can use the `compare_to_market` tool to compare your calculated valuation against current local market rates per acre-foot.

**Q: What is the difference between annual yield and present value?**
Annual yield is the expected economic output for a single year, while present value is the total current worth of the water right over its entire useful life, discounted to today.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/water-rights-valuation-engine](https://vinkius.com/ai-agent-connect/water-rights-valuation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Rights Valuation Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-rights-valuation-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Rights Valuation Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-rights-valuation-engine": {
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
