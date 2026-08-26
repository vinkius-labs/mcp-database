# CCI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cci-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Commodity Channel Index (CCI) indicator for technical analysis.

## Description
This MCP server provides precise Commodity Channel Index (CCI) calculations to identify market momentum, overbought/oversold conditions, and price divergences. Use `calculate_cci_series` to generate historical CCI values, `analyze_cci_signals` to detect zero-line crosses and extreme reversal zones, or `detect_cci_divergence` to find discrepancies between price action and momentum. It connects your AI assistant to professional-grade technical indicators.


## Available Tools (3)
- **detect_cci_divergence**: Identifies discrepancies between price movement and CCI momentum
- **analyze_cci_signals**: Interprets a series of CCI values to identify specific technical signals
- **calculate_cci_series**: Calculates the full sequence of CCI values for a given historical dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CCI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the CCI series for these prices: Highs [10, 12, 11], Lows [8, 9, 8], Closes [9, 11, 10] with a period of 2."

**🤖 AI Agent:**
> The calculated CCI values for the provided period are [15.4, -5.2].

---

**👤 You:**
> "Analyze these CCI values for signals: [120, 150, -10, -110]."

**🤖 AI Agent:**
> The analysis detected an OVERBOUGHT signal at index 0, an EXTREME_REVERSAL_HIGH at index 1, and an OVERSOLD signal at index 3.

---

**👤 You:**
> "Check for divergence with these prices and CCI values: Highs [10, 12, 11], Lows [8, 9, 8], Closes [9, 11, 10], CCI [5, 10, 5]."

**🤖 AI Agent:**
> No divergence was detected in the provided dataset.


## ❓ FAQ

**Q: What is the Commodity Channel Index?**
The CCI is a momentum-based indicator used to identify cyclical trends and extreme price levels in financial markets.

**Q: How do I detect a bullish signal?**
You can use `analyze_cci_signals` to identify a BULLISH_CROSS when the CCI value moves from below zero to above zero.

**Q: Can this tool identify price reversals?**
Yes, `analyze_cci_signals` identifies EXTREME_REVERSAL_HIGH and EXTREME_REVERSAL_LOW when values exceed 200 or fall below -200.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cci-calculator](https://vinkius.com/ai-agent-connect/cci-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CCI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cci-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CCI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cci-calculator": {
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
