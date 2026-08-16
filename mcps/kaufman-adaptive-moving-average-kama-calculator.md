# Kaufman Adaptive Moving Average (KAMA) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kaufman-adaptive-moving-average-kama-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate adaptive moving averages that adjust to market volatility.

## Description
This MCP server provides a deterministic engine for calculating the Kaufman Adaptive Moving Average (KAMA). Unlike standard moving averages, KAMA uses an Efficiency Ratio (ER) to adjust its smoothing speed, allowing it to filter out market noise during sideways movement and react quickly during strong trends. Use `calculate_kama_series` to generate full trend datasets, `get_latest_kama_status` to extract current trend metrics, or `analyze_kama_volatility_regime` to identify if the market is trending or ranging.


## Available Tools (3)
- **analyze_kama_volatility_regime**: Determines whether the market is currently in a trending or ranging regime based on the efficiency of recent movements
- **calculate_kama_series**: Computes the full sequence of KAMA values and trend metrics for a provided set of prices
- **get_latest_kama_status**: Extracts the most recent trend and volatility data from a pre-calculated series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kaufman Adaptive Moving Average (KAMA) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the KAMA series for these closing prices: [150.2, 151.5, 152.1, 150.8, 153.4, 154.2, 155.0, 154.5, 156.2, 157.5]"

**🤖 AI Agent:**
> [{"kama": 151.2, "er": 0.85, "slope": 0.4, "trend": "UP"}, ...]

---

**👤 You:**
> "Is the market currently in a trending or ranging regime based on these prices: [10, 11, 10, 11, 10, 11, 10, 11, 10, 11]?"

**🤖 AI Agent:**
> {"averageER": 0.1, "regime": "RANGING"}

---

**👤 You:**
> "What is the latest trend status for this KAMA data: [{"kama": 100, "slope": 0.5, "trend": "UP"}]?"

**🤖 AI Agent:**
> {"currentKama": 100, "currentSlope": 0.5, "currentTrend": "UP", "isTrending": true}


## ❓ FAQ

**Q: How does KAMA differ from a standard EMA?**
Standard EMAs use a constant smoothing factor. KAMA uses an Efficiency Ratio to change its smoothing speed based on market volatility, making it more responsive to trends and less sensitive to noise.

**Q: Can I get the current trend status directly?**
Yes, you can use the `get_latest_kama_status` tool to retrieve the current KAMA value, slope, and trend direction from a series.

**Q: What determines the market regime?**
The `analyze_kama_volatility_regime` tool determines if the market is TRENDING or RANGING by comparing the most recent Efficiency Ratio to the average ER of the series.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kaufman-adaptive-moving-average-kama-calculator](https://vinkius.com/ai-agent-connect/kaufman-adaptive-moving-average-kama-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kaufman Adaptive Moving Average (KAMA) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kaufman-adaptive-moving-average-kama-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kaufman Adaptive Moving Average (KAMA) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kaufman-adaptive-moving-average-kama-calculator": {
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
