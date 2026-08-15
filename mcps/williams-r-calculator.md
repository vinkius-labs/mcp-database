# Williams %R Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/williams-r-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis engine for Williams %R, divergence, and failure swing detection.

## Description
This MCP server provides a deterministic technical analysis engine for the Williams %R oscillator. It allows AI agents to calculate momentum levels, identify overbought and oversold zones, and detect critical market signals like divergence and failure swings. Use `calculate_williams_r` to compute oscillator values, `detect_divergence` to find price-momentum discrepancies, and `identify_failure_swings` to spot potential trend reversals.


## Available Tools (3)
- **calculate_williams_r**: Computes the raw Williams %R values for a provided series of price data
- **detect_divergence**: Identifies discrepancies between price action and momentum strength
- **identify_failure_swings**: Detects potential trend reversal signals based on failed momentum attempts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Williams %R Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Williams %R for these prices: High [10, 12, 11], Low [8, 9, 7], Close [9, 11, 8] with a period of 3."

**🤖 AI Agent:**
> The calculated Williams %R values are -33.33, -16.67, and -66.67.

---

**👤 You:**
> "Check if there is a divergence in this data: Price [100, 105, 102], WilliamsR [ -50, -40, -60]."

**🤖 AI Agent:**
> A Bearish Divergence was detected at index 2.

---

**👤 You:**
> "Identify failure swings for these prices: High [10, 12, 11], Low [8, 9, 7], Close [9, 11, 8] and WilliamsR [-33.33, -16.67, -66.67]."

**🤖 AI Agent:**
> No failure swings were identified in the provided series.


## ❓ FAQ

**Q: What is the Williams %R oscillator?**
The Williams %R is a momentum indicator that measures overbought and oversold levels by comparing the current closing price to a specific range of high and low prices over a set period.

**Q: How do I detect a trend reversal?**
You can use the `identify_failure_swings` tool to detect potential trend reversals where price attempts to break a previous swing but momentum fails to follow.

**Q: Can I detect divergences between price and momentum?**
Yes, the `detect_divergence` tool identifies Bullish and Bearish divergences by comparing price action against the Williams %R series.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/williams-r-calculator](https://vinkius.com/mcp/williams-r-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Williams %R Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `williams-r-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Williams %R Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "williams-r-calculator": {
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
