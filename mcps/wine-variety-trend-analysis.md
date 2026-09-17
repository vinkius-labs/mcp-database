# Wine Variety Trend Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-variety-trend-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Analyze wine variety market trends, growth rates, and future market share projections.

## Description
This MCP server provides deep market intelligence for the wine industry. It allows AI agents to retrieve historical sales data using `get_variety_performance`, predict future market shifts with `forecast_market_trends`, and evaluate regional variety dominance via `analyze_market_composition`. Additionally, agents can assess how specific consumer preferences impact popularity through `cross_reference_style_trends`.


## Available Tools (4)
- **analyze_market_composition**: Provides a snapshot of all varieties within a region to identify leaders and laggards
- **cross_reference_style_trends**: g., "Crisp Whites") is trending in a region.

Evaluates how specific style trends are impacting variety popularity in a region
- **forecast_market_trends**: Predicts future market share and identifies the status of varieties
- **get_variety_performance**: Retrieves the historical sales and growth metrics for a specific variety


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Variety Trend Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current performance of Cabernet Sauvignon in North America?"

**🤖 AI Agent:**
> Cabernet Sauvignon in North America currently holds a 15% market share with an annual growth rate of 2.4%.

---

**👤 You:**
> "Predict the market share for Chardonnay in Western Europe over the next 5 years."

**🤖 AI Agent:**
> Chardonnay is projected to reach a 12.5% market share in Western Europe over the next 5 years with an emerging status.

---

**👤 You:**
> "Which varieties are currently trending in the 'Crisp Whites' category in North America?"

**🤖 AI Agent:**
> In the Crisp Whites category in North America, Sauvignon Blanc and Pinot Grigio are the dominant varieties.


## ❓ FAQ

**Q: How can I see if a specific wine is growing in popularity?**
You can use the `forecast_market_trends` tool to see the projected CAGR and status of a variety.

**Q: Can I compare different wine styles in a specific region?**
Yes, the `cross_reference_style_trends` tool allows you to evaluate how specific style categories are trending in a given market.

**Q: What data is available for regional market breakdowns?**
The `analyze_market_composition` tool provides a full breakdown of all varieties, their market share, and their growth status within a region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-variety-trend-analysis](https://vinkius.com/en/ai-agent-connect/wine-variety-trend-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Variety Trend Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-variety-trend-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Variety Trend Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-variety-trend-analysis": {
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
