# Stochastic RSI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/stochastic-rsi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Stochastic RSI indicator with signal detection.

## Description
This MCP server provides precise technical analysis by computing the Stochastic RSI indicator. It applies the stochastic formula to Wilder's smoothed RSI values to identify momentum shifts. Users can use `calculate_stoch_rsi` to retrieve full series data and signals, `get_current_market_state` for immediate trend and overbought/oversold status, or `detect_divergence_patterns` to find historical price and indicator disagreements. It is designed for traders needing exact, deterministic calculations for crossovers, divergences, and threshold breaches.


## Available Tools (3)
- **calculate_stoch_rsi**: 
- **detect_divergence_patterns**: 
- **get_current_market_state**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stochastic RSI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current market state for these closing prices: [45.2, 46.1, 45.8, 47.2, 48.5, 48.0, 49.1]?"

**🤖 AI Agent:**
> The current market state is bullish with a %K of 85.5 and a %D of 78.2, indicating an overbought condition.

---

**👤 You:**
> "Are there any divergence patterns in this price series: [100, 105, 102, 110, 108, 115]?"

**🤖 AI Agent:**
> A bearish divergence was detected where the price reached a higher high at index 5, but the indicator momentum showed a lower high.

---

**👤 You:**
> "Calculate the Stochastic RSI signals for these prices: [50, 51, 52, 51, 50, 49, 48, 47, 46, 45]?"

**🤖 AI Agent:**
> The indicator shows an oversold signal as the %K value dropped below 20.


## ❓ FAQ

**Q: How does this server calculate RSI?**
The server uses Wilder's smoothing method to calculate the initial RSI values, ensuring compatibility with standard technical analysis tools.

**Q: Can I detect trend reversals?**
Yes, you can use `detect_divergence_patterns` to identify where price and indicator momentum disagree, or check for crossovers between %K and %D.

**Q: What are the default parameters?**
The default settings are an RSI period of 14, a Stochastic period of 14, %K smoothing of 3, and a %D period of 3.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/stochastic-rsi-calculator](https://vinkius.com/ai-agent-connect/stochastic-rsi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stochastic RSI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stochastic-rsi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stochastic RSI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stochastic-rsi-calculator": {
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
