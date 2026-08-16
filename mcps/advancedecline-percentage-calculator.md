# Advance/Decline Percentage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/advancedecline-percentage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate market breadth, sentiment classification, and trend divergence.

## Description
This MCP server provides high-precision tools for analyzing market breadth. Use `calculate_market_breadth` to determine advance, decline, and net breadth percentages along with sentiment classification (Strong Bullish, Moderate Bullish, Neutral, or Bearish). Use `calculate_technical_breadth_status` to find the percentage of stocks above their 20-day moving average, and `analyze_trend_divergence` to identify potential trend reversals by comparing cumulative breadth against price movements.


## Available Tools (3)
- **analyze_trend_divergence**: Evaluate the relationship between cumulative breadth and price movement
- **calculate_market_breadth**: Calculate fundamental market breadth metrics and sentiment classification
- **calculate_technical_breadth_status**: Determine the percentage of the market exhibiting bullish technical characteristics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Advance/Decline Percentage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the market breadth for 100 advancing, 50 declining, and 50 unchanged stocks out of a 200 stock universe."

**🤖 AI Agent:**
> The advance percentage is 50%, the decline percentage is 25%, and the net breadth percentage is 25%. The market sentiment is Neutral.

---

**👤 You:**
> "What is the technical breadth if 75 stocks are above their 20-day moving average in a 100 stock universe?"

**🤖 AI Agent:**
> The technical breadth is 75%.

---

**👤 You:**
> "Check for divergence between a cumulative breadth series [10, 12, 15] and a price series [100, 98, 95]."

**🤖 AI Agent:**
> A bullish divergence is detected because the cumulative breadth is rising while the price is falling.


## ❓ FAQ

**Q: How is market sentiment classified?**
Sentiment is classified based on the Advance Percentage: Strong Bullish (> 60%), Moderate Bullish (50-60%), Neutral (40-50%), and Bearish (< 40%).

**Q: What is the purpose of the divergence tool?**
The `analyze_trend_divergence` tool identifies potential trend reversals by detecting when the direction of cumulative net breadth moves opposite to the direction of price.

**Q: Can I calculate technical strength?**
Yes, you can use `calculate_technical_breadth_status` to determine the percentage of the market trading above their 20-day moving average.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/advancedecline-percentage-calculator](https://vinkius.com/ai-agent-connect/advancedecline-percentage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Advance/Decline Percentage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `advancedecline-percentage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Advance/Decline Percentage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "advancedecline-percentage-calculator": {
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
