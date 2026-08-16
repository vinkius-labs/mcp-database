# Moving Average Envelope Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/moving-average-envelope-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates moving average center lines, upper/lower envelopes, and breakout signals.

## Description
This MCP provides technical analysis tools to calculate moving average envelopes. It computes central moving average lines (SMA or EMA) and offsets them by a specified percentage to create upper and lower bands. Use `calculate_envelope_series` to get a full historical dataset of envelopes, widths, and breakout signals. Use `get_latest_envelope_status` to check if the current price is overbought or oversold. Use `analyze_envelope_volatility` to track if the envelope width is expanding or contracting.


## Available Tools (3)
- **analyze_envelope_volatility**: Measures the expansion or contraction of the envelopes to assess changing volatility
- **calculate_envelope_series**: Computes the full series of moving averages and their corresponding upper and lower envelopes for a given price history
- **get_latest_envelope_status**: Provides a snapshot of the most recent calculation to determine current market state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Average Envelope Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the envelope series for these prices: [100, 102, 101, 105, 107, 106, 110] using a 5-period SMA and 2% envelope."

**🤖 AI Agent:**
> The calculated center line for the 5-period SMA is 104.2, with an upper envelope of 106.28 and a lower envelope of 102.12.

---

**👤 You:**
> "Is the current price of 150 overbought given a center line of 140 and a 5% envelope?"

**🤖 AI Agent:**
> Yes, the price is overbought because the upper envelope is 147 (140 * 1.05) and the current price of 150 is above it.

---

**👤 You:**
> "Check the latest status for prices [50, 51, 52, 53, 54, 55] with a 3-period EMA."

**🤖 AI Agent:**
> The current price is 55, the center line is 54.1, and the position is neutral.


## ❓ FAQ

**Q: What is the difference between SMA and EMA in this tool?**
SMA (Simple Moving Average) calculates the arithmetic mean of prices, while EMA (Exponential Moving Average) applies more weight to recent prices for faster response.

**Q: How do I know if a price breakout has occurred?**
A breakout is identified when the closing price moves outside the upper or lower envelope boundaries, which is captured in the `breakoutSignals` array from `calculate_envelope_series`.

**Q: Can I customize the envelope width?**
Yes, you can specify the `envelopePercentage` parameter in any of the tools to adjust the distance of the bands from the center line.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/moving-average-envelope-calculator](https://vinkius.com/ai-agent-connect/moving-average-envelope-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Average Envelope Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-average-envelope-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Average Envelope Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-average-envelope-calculator": {
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
