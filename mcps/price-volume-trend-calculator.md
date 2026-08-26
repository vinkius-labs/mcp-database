# Price Volume Trend Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/price-volume-trend-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze market momentum using Price Volume Trend (PVT) and divergence detection.

## Description
This MCP server provides advanced technical analysis tools to calculate the Price Volume Trend (PVT) indicator. Unlike standard On-Balance Volume (OBV), PVT scales volume by the magnitude of price changes, offering a more sensitive view of market momentum. Use `calculate_pvt_metrics` to obtain cumulative PVT values, moving averages, and trend signals like Accumulation or Distribution. Use `detect_pvt_divergences` to identify potential trend reversals when price and volume-weighted momentum decouple. Finally, use `compare_pvt_obv` to evaluate how price volatility influences volume-driven trends.


## Available Tools (3)
- **compare_pvt_obv**: Compares PVT to OBV
- **calculate_pvt_metrics**: 
- **detect_pvt_divergences**: Identifies price/PVT divergences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Price Volume Trend Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the PVT metrics for these closing prices [150, 155, 153, 158] and volumes [1000, 1200, 1100, 1300]."

**🤖 AI Agent:**
> The calculated PVT values are [0, 60, 30, 120], with a trend signal of Trend Confirmation.

---

**👤 You:**
> "Check for divergences between these prices [10, 12, 11, 13] and these PVT values [100, 150, 120, 140]."

**🤖 AI Agent:**
> A Bearish Divergence was detected at index 3 because the price reached a new high while the PVT failed to do so.

---

**👤 You:**
> "Compare the PVT trend to OBV for these prices [100, 105, 102] and volumes [500, 600, 400] with PVT values [0, 25, 15]."

**🤖 AI Agent:**
> The correlation is 0.85, indicating High Volatility Sensitivity in the PVT trend compared to OBV.


## ❓ FAQ

**Q: How does PVT differ from OBV?**
While OBV treats all volume changes as binary, PVT scales the volume by the percentage of the price move, making it more sensitive to the intensity of price action.

**Q: What are the primary signals provided?**
The server detects Accumulation, Distribution, and Trend Confirmation signals, as well as Bullish and Bearish divergences.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this MCP to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/price-volume-trend-calculator](https://vinkius.com/ai-agent-connect/price-volume-trend-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Price Volume Trend Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `price-volume-trend-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Price Volume Trend Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "price-volume-trend-calculator": {
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
