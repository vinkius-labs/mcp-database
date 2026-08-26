# Relative Vigor Index (RVI) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/relative-vigor-index-rvi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis tool for RVI, signal lines, and momentum signals.

## Description
This MCP server provides precise technical analysis tools for the Relative Vigor Index (RVI). It allows AI agents to calculate RVI values, generate signal lines, and identify critical momentum signals like zero-line crosses, signal crossovers, and price/RVI divergences. Use `calculate_rvi_metrics` to process OHLC data, `get_rvi_summary` for trend and volatility overviews, or `detect_divergence_patterns` to isolate specific divergence events.


## Available Tools (3)
- **detect_divergence_patterns**: Isolates and describes price/RVI divergences
- **get_rvi_summary**: Provides a high-level statistical overview of RVI state
- **calculate_rvi_metrics**: Calculates RVI, Signal Line, and momentum signals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative Vigor Index (RVI) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RVI metrics for this OHLC data: [{"open": 100, "high": 105, "low": 95, "close": 102}, {"open": 102, "high": 108, "low": 101, "close": 107}, {"open": 107, "high": 110, "low": 105, "close": 109}, {"open": 109, "high": 112, "low": 108, "close": 111}, {"open": 111, "high": 115, "low": 110, "close": 114}]"

**🤖 AI Agent:**
> The calculated RVI values and signal line trends indicate a bullish momentum for the provided dataset.

---

**👤 You:**
> "Is there a current trend in these RVI values: [0.1, 0.2, 0.15, 0.3, 0.4] and signal line values: [0.0, 0.1, 0.1, 0.2, 0.3]?"

**🤖 AI Agent:**
> The current trend is Bullish with a recent increase in momentum.

---

**👤 You:**
> "Check for divergences in this price and RVI data."

**🤖 AI Agent:**
> No divergence patterns were detected in the provided data.


## ❓ FAQ

**Q: What signals can this tool identify?**
The tool identifies zero-line crosses, signal crossovers, and bullish or bearish divergences using `calculate_rvi_metrics` and `detect_divergence_patterns`.

**Q: How is the RVI smoothed?**
RVI components are smoothed using a Simple Moving Average (SMA) over a user-defined period, which defaults to 10.

**Q: What data format is required?**
The tools require JSON arrays of OHLC (Open, High, Low, Close) price data or arrays of RVI/Signal Line float values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/relative-vigor-index-rvi-calculator](https://vinkius.com/ai-agent-connect/relative-vigor-index-rvi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative Vigor Index (RVI) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-vigor-index-rvi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative Vigor Index (RVI) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-vigor-index-rvi-calculator": {
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
