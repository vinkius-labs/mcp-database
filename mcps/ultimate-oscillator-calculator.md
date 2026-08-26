# Ultimate Oscillator Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ultimate-oscillator-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Larry Williams' Ultimate Oscillator to detect momentum shifts and divergences.

## Description
This MCP server provides precise technical analysis tools for the Larry Williams Ultimate Oscillator (UO). It connects AI agents to financial momentum calculations, allowing for the identification of overbought and oversold conditions, centerline crosses, and price-oscillator divergences. Use `calculate_uo_values` to generate the oscillator series, `analyze_uo_signals` to find threshold crossings, and `detect_uo_divergence` to spot bullish or bearish momentum shifts.


## Available Tools (3)
- **detect_uo_divergence**: Detects bullish and bearish divergences between price action and the oscillator
- **analyze_uo_signals**: Identifies technical signals such as overbought/oversold levels and centerline crosses based on calculated UO values
- **calculate_uo_values**: Computes the raw Ultimate Oscillator values for a provided set of price data across the three standard timeframes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ultimate Oscillator Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Ultimate Oscillator values for these prices: highs [150, 155, 152], lows [145, 148, 146], closes [148, 153, 150]."

**🤖 AI Agent:**
> The calculated Ultimate Oscillator values for the provided price series are [45.2, 52.8, 48.5].

---

**👤 You:**
> "Are there any overbought signals in this UO sequence: [75, 72, 68, 45]?"

**🤖 AI Agent:**
> Yes, overbought signals were detected at index 0 and index 1.

---

**👤 You:**
> "Check for divergences using these prices and UO values: highs [10, 12, 11], lows [8, 9, 8], closes [9, 11, 10], uoValues [35, 40, 38]."

**🤖 AI Agent:**
> No divergences were detected in the provided data.


## ❓ FAQ

**Q: What is the Ultimate Oscillator?**
The Ultimate Oscillator is a momentum indicator developed by Larry Williams that uses three different timeframes to reduce false signals.

**Q: How do I identify overbought conditions?**
An asset is considered overbought when the oscillator value exceeds 70, which can be identified using the `analyze_uo_signals` tool.

**Q: Can this tool detect divergences?**
Yes, the `detect_uo_divergence` tool specifically identifies bullish and bearish divergences between price action and the oscillator.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ultimate-oscillator-calculator](https://vinkius.com/ai-agent-connect/ultimate-oscillator-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ultimate Oscillator Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ultimate-oscillator-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ultimate Oscillator Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ultimate-oscillator-calculator": {
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
