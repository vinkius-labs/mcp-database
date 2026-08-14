# Bollinger Bands Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bollinger-bands-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate volatility bands, squeeze states, and price positioning.

## Description
This MCP server provides deterministic technical analysis tools for volatility monitoring. Use `get_bollinger_bands` to calculate the middle band, upper and lower volatility limits, bandwidth, and %B. Use `detect_volatility_squeeze` to identify periods of extreme volatility contraction. Finally, use `get_band_summary` to receive a high-level status report on market volatility and potential breakout signals.


## Available Tools (3)
- **detect_volatility_squeeze**: 
- **get_band_summary**: 
- **get_bollinger_bands**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bollinger Bands Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Bollinger Bands for these prices: [150.2, 152.5, 151.0, 149.8, 153.4, 155.0, 154.2]"

**🤖 AI Agent:**
> The middle band is 152.1, the upper band is 155.4, and the lower band is 148.8. The current bandwidth is 4.47% and %B is 0.62, placing the price within the bands.

---

**👤 You:**
> "Is there a volatility squeeze happening with this bandwidth history: [2.5, 2.4, 2.6, 2.3, 2.2, 2.1, 1.9]?"

**🤖 AI Agent:**
> Yes, a squeeze is detected as the current bandwidth is at a historical low.

---

**👤 You:**
> "Give me a summary of the volatility state for a middle band of 100, upper band of 110, lower band of 90, and a detected squeeze."

**🤖 AI Agent:**
> Status: Squeeze Detected. Volatility State: Tight. Recommendation: Watch for breakout.


## ❓ FAQ

**Q: How do I calculate the volatility bands?**
You can use the `get_bollinger_bands` tool by providing an array of closing prices. You can also optionally specify the lookback period and the standard deviation multiplier.

**Q: What is a volatility squeeze?**
A squeeze occurs when market volatility contracts significantly. The `detect_volatility_squeeze` tool identifies this by checking if the current bandwidth is at a 6-month low.

**Q: Can I get a summary of the current market state?**
Yes, the `get_band_summary` tool provides a qualitative status, volatility state, and recommendation based on the calculated bands and squeeze status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bollinger-bands-calculator](https://vinkius.com/mcp/bollinger-bands-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bollinger Bands Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bollinger-bands-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bollinger Bands Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bollinger-bands-calculator": {
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
