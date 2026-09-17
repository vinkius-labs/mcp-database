# Wine Vintage Rating Impact MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-vintage-rating-impact)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze how vintage quality affects wine price, demand, and inventory value.

## Description
This MCP server provides specialized tools to calculate the economic impact of vintage ratings on wine inventory. By using the vintage adjustment model, it determines price premiums or discounts, predicts shifts in sales velocity, and calculates total inventory valuation adjustments. It accounts for regional vintage variation to ensure accuracy across different wine-growing areas.


## Available Tools (4)
- **get_regional_vintage_benchmark**: What is the historical average rating and price volatility for this specific region?
- **get_vintage_impact_analysis**: How does this specific vintage rating affect the price and demand of my current wine inventory?
- **get_demand_forecast_trend**: How much faster or slower will this wine sell given its vintage rating?
- **get_inventory_valuation_delta**: What is the total impact of vintage quality on my current stock's total value?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Vintage Rating Impact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How does a 'Great' vintage rating affect the price and demand for wine ID 123 in Bordeaux?"

**🤖 AI Agent:**
> A 'Great' vintage for this Bordeaux wine results in a 12% price premium and a 15% increase in expected sales velocity.

---

**👤 You:**
> "What is the total impact on my inventory value if I apply a 95 rating to wine ID 456?"

**🤖 AI Agent:**
> Applying a 95 rating to wine ID 456 results in a total inventory valuation adjustment of +$4,500.00.

---

**👤 You:**
> "What are the historical benchmarks for the Napa Valley region?"

**🤖 AI Agent:**
> The historical average rating for Napa Valley is 88, with a volatility index of 0.45 and an average base price of $75.00.


## ❓ FAQ

**Q: How does the tool account for different wine regions?**
The `get_vintage_impact_analysis` tool uses the provided `regionalContext` to adjust the impact factor based on historical volatility in that specific region.

**Q: Can I use qualitative ratings like 'Elite' or 'Great'?**
Yes, the tools accept both numerical 100-point scales and qualitative labels such as 'Elite', 'Great', 'Good', 'Average', or 'Poor'.

**Q: What is the purpose of the inventory valuation tool?**
The `get_inventory_valuation_delta` tool calculates the total currency impact on your entire stock based on the target vintage rating.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-vintage-rating-impact](https://vinkius.com/en/ai-agent-connect/wine-vintage-rating-impact)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Vintage Rating Impact** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-vintage-rating-impact` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Vintage Rating Impact** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-vintage-rating-impact": {
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
