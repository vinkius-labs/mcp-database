# Arms Index (TRIN) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/arms-index-trin-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the Arms Index (TRIN) to measure market breadth and sentiment.

## Description
This MCP server provides deterministic tools to calculate the Arms Index (TRIN), a key momentum indicator for market breadth. Use `calculate_daily_trin` to determine current market sentiment, `get_trin_moving_average` to identify trends over time, and `get_trin_statistics` to find statistical outliers via Z-score and percentile rank. It helps identify bullish pressure, bearish pressure, or extreme fear in the market.


## Available Tools (3)
- **get_trin_moving_average**: Analyzes the trend of TRIN values over a specific period
- **calculate_daily_trin**: Computes the single-day TRIN value based on current market breadth and volume data
- **get_trin_statistics**: Provides a statistical comparison of the current TRIN against historical data to identify extremes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arms Index (TRIN) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the current TRIN with 150 advancing stocks, 50 declining stocks, 1000000 advancing volume, and 500000 declining volume."

**🤖 AI Agent:**
> The calculated TRIN is 3.0, which indicates extreme fear.

---

**👤 You:**
> "What is the sentiment if the TRIN is 0.75?"

**🤖 AI Agent:**
> The sentiment is bullish.

---

**👤 You:**
> "Get the statistical Z-score for a TRIN of 1.5 given a history of [1.0, 1.2, 1.1, 1.3, 1.4]."

**🤖 AI Agent:**
> The Z-score is 2.12 and the percentile rank is 95%.


## ❓ FAQ

**Q: What does a TRIN value below 1.0 indicate?**
A TRIN value below 1.0 indicates bullish sentiment, suggesting buying pressure in advancing stocks.

**Q: How can I identify extreme fear in the market?**
Extreme fear is indicated when the TRIN value exceeds 2.0, which often serves as a contrarian bullish signal.

**Q: Can I calculate the moving average of the TRIN?**
Yes, you can use the `get_trin_moving_average` tool to calculate the arithmetic mean of TRIN values over a specified period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/arms-index-trin-calculator](https://vinkius.com/ai-agent-connect/arms-index-trin-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arms Index (TRIN) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arms-index-trin-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arms Index (TRIN) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arms-index-trin-calculator": {
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
