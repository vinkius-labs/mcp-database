# Crack Spread Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/crack-spread-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze refinery profitability by calculating crack spreads and hedge ratios.

## Description
This MCP server provides essential tools for refinery economics. Use `get_current_spread` to calculate immediate profitability based on crude and product prices. Analyze market cycles with `get_historical_trend`, determine risk mitigation strategies using `calculate_hedge_ratio`, and adjust yields based on crude characteristics with `get_quality_impact_adjustment`.


## Available Tools (4)
- **calculate_hedge_ratio**: Determines the optimal ratio of financial hedging required to mitigate price risk
- **get_current_spread**: Calculates the immediate profitability of a specific refinery configuration based on current market prices
- **get_historical_trend**: Analyzes how the crack spread for a specific configuration has moved over a given period
- **get_quality_impact_adjustment**: Provides the adjustment factor required based on the specific characteristics of a crude oil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crack Spread Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current 3-2-1 crack spread if crude is $80 and gasoline/diesel are $110 and $95?"

**🤖 AI Agent:**
> The current 3-2-1 crack spread value is $55.00 per barrel.

---

**👤 You:**
> "Show me the historical trend for the 5-3-2 spread in the US Gulf Coast from 2023-01-01 to 2023-12-31."

**🤖 AI Agent:**
> The average spread for the period was $42.50 with a volatility of 5.2 and an upward trend direction.

---

**👤 You:**
> "Calculate a hedge ratio for a spread of $50 with a volatility of 4 and risk tolerance of 0.5."

**🤖 AI Agent:**
> The recommended hedge ratio is 0.65, with an estimated hedge cost of $12.50.


## ❓ FAQ

**Q: How do I calculate the current margin?**
You can use the `get_current_spread` tool by providing the crude price, product prices, and the specific spread type like 3-2-1.

**Q: Can I account for crude quality?**
Yes, use `get_quality_impact_adjustment` to find the factor based on API gravity and sulfur content.

**Q: How is the hedge ratio determined?**
The `calculate_hedge_ratio` tool determines the ratio based on the current spread value, historical volatility, and your risk tolerance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/crack-spread-analysis](https://vinkius.com/en/ai-agent-connect/crack-spread-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crack Spread Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crack-spread-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crack Spread Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crack-spread-analysis": {
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
