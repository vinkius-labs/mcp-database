# Demand Forecast Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/demand-forecast-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Generate 3-month demand projections using SMA, WMA, and Exponential Smoothing methods.

## Description
This MCP server provides advanced forecasting capabilities to predict future demand based on historical data. It implements three distinct mathematical models: Simple Moving Average (`analyze_sma`), Weighted Moving Average (`analyze_wma`), and Exponential Smoothing (`analyze_exponential_smoothing`). For each method, the tools perform error backtesting to provide Mean Absolute Error (MAE) and Mean Absolute Percentage Error (MAPE), allowing you to identify the most accurate model for your specific dataset. Use these tools in Cursor, VS Code, Claude Desktop, or Windsurf to automate demand planning.


## Available Tools (3)
- **analyze_exponential_smoothing**: Calculate demand forecast using Exponential Smoothing
- **analyze_sma**: Calculate demand forecast using Simple Moving Average (SMA)
- **analyze_wma**: Calculate demand forecast using Weighted Moving Average (WMA)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Demand Forecast Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a 3-month forecast using SMA with a window size of 3 for this demand: [10, 12, 15, 14, 18]"

**🤖 AI Agent:**
> The `analyze_sma` tool has processed your data. The forecast for the next three months is [15.67, 15.67, 15.67] with a calculated MAPE of approximately 8.2%.

---

**👤 You:**
> "Use Exponential Smoothing to predict demand for [100, 110, 120] with alpha=0.5 and beta=0.3."

**🤖 AI Agent:**
> Using `analyze_exponential_smoothing`, the predicted demand for the next three periods is [130, 140, 150].

---

**👤 You:**
> "Analyze demand using WMA with weights [0.5, 0.3, 0.2] for data: [50, 60, 70]"

**🤖 AI Agent:**
> The `analyze_wma` tool calculated the forecast as [76, 76, 76] based on your provided weights and historical sequence.


## ❓ FAQ

**Q: What forecasting methods are supported?**
The server supports Simple Moving Average (`analyze_sma`), Weighted Moving Average (`analyze_wma`), and Exponential Smoothing (`analyze_exponential_smoothing`).

**Q: How is the accuracy of the forecast measured?**
Accuracy is measured using Mean Absolute Error (MAE) and Mean Absolute Percentage Error (MAPE) through a backtesting process on your historical data.

**Q: What inputs are required for the SMA tool?**
The `analyze_sma` tool requires an array of historical demand values and a window size representing the number of periods to include in the average.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/demand-forecast-calculator](https://vinkius.com/mcp/demand-forecast-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Demand Forecast Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `demand-forecast-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Demand Forecast Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "demand-forecast-calculator": {
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
