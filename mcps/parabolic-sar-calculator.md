# Parabolic SAR Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/parabolic-sar-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compute deterministic Parabolic SAR values, trend directions, and reversal signals.

## Description
This MCP server provides precise technical analysis tools for the Parabolic Stop and Reverse (SAR) indicator. It allows AI agents to calculate full SAR series, summarize current market trends, and identify specific reversal windows using customizable acceleration factors. Use `calculate_sar_series` to generate a complete sequence of trend data, `get_trend_summary` for a snapshot of the current market state, or `identify_reversal_windows` to pinpoint exactly when trend direction changed.


## Available Tools (3)
- **calculate_sar_series**: Optional AF parameters can be provided.

Computes the full sequence of SAR values and trend indicators for a given set of price data
- **get_trend_summary**: Optional AF parameters can be provided.

Provides a high-level summary of the current market state based on the most recent data points
- **identify_reversal_windows**: Optional AF parameters can be provided.

Extracts specific timeframes or indices where trend reversals occurred for signal analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parabolic SAR Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the SAR series for these prices: highs [10, 12, 13, 11], lows [9, 10, 11, 10]."

**🤖 AI Agent:**
> The calculated SAR values for the provided series are [9.0, 9.5, 10.2, 10.8] with an uptrend direction.

---

**👤 You:**
> "What is the current trend summary for highs [50, 52, 51] and lows [48, 49, 47]?"

**🤖 AI Agent:**
> The current trend is up, with the last SAR at 47.5 and the last extreme point at 52.

---

**👤 You:**
> "Find all reversal points in this data: highs [10, 15, 12, 8], lows [8, 13, 10, 6]."

**🤖 AI Agent:**
> A reversal from up to down occurred at index 2 with a price of 12.


## ❓ FAQ

**Q: How do I use the SAR calculation tool?**
You can provide arrays of high and low prices to the `calculate_sar_series` tool. You may also optionally specify the starting acceleration factor, the increment, and the maximum acceleration.

**Q: What is a trend reversal in this tool?**
A reversal is detected when the price crosses the current SAR value. The tool identifies these moments using `identify_reversal_windows`.

**Q: Can I customize the acceleration factor?**
Yes, you can adjust the `afStart`, `afIncrement`, and `afMax` parameters to suit different market volatility profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parabolic-sar-calculator](https://vinkius.com/mcp/parabolic-sar-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parabolic SAR Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parabolic-sar-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parabolic SAR Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parabolic-sar-calculator": {
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
