# Stochastic Oscillator Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stochastic-oscillator-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Stochastic Oscillator values, identify crossovers, and detect price-momentum divergences.

## Description
This MCP server provides precise technical analysis tools for the Stochastic Oscillator. It allows AI agents to compute %K and %D values, identify overbought and oversold conditions, detect bullish and bearish crossovers, and find price-momentum divergences. Use `calculate_stochastic_metrics` to generate core oscillator data, `detect_stochastic_divergence` to find discrepancies between price and momentum, and `get_oscillator_summary` for a quick snapshot of the current market trend.


## Available Tools (3)
- **get_oscillator_summary**: Provide a high-level snapshot of the current market state
- **calculate_stochastic_metrics**: Calculate core Stochastic Oscillator values (%K and %D) and identify signal states
- **detect_stochastic_divergence**: Identify discrepancies between price movement and oscillator momentum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stochastic Oscillator Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stochastic metrics for these prices: High [10, 12, 11], Low [8, 9, 8], Close [9, 11, 10]."

**🤖 AI Agent:**
> The calculated %K values are [45.2, 78.5, 50.0] and %D values are [40.1, 55.3, 58.2]. The current status is NEUTRAL.

---

**👤 You:**
> "Is the market currently overbought or oversold based on these %K values: [85, 88, 90] and %D values: [80, 82, 84]?"

**🤖 AI Agent:**
> The market is currently in the OVERBOUGHT zone as the most recent %K value is 90.

---

**👤 You:**
> "Check for divergences using these prices: High [100, 110, 115], Low [50, 45, 40] and %K values: [50, 55, 52]."

**🤖 AI Agent:**
> A BEARISH_DIVERGENCE was detected because the price reached a higher high of 115 while the %K value reached a lower high of 52.


## ❓ FAQ

**Q: What is the difference between Fast and Slow Stochastic?**
Fast Stochastic uses the raw %K calculation. Slow Stochastic applies smoothing to the %K values to reduce market noise, making it more reliable for trend identification.

**Q: How do I detect a bullish crossover?**
A bullish crossover occurs when the %K line crosses above the %D line, indicating accelerating upward momentum.

**Q: Can I use EMA instead of SMA for smoothing?**
Yes, the `calculate_stochastic_metrics` tool supports both SMA and EMA as moving average types for smoothing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stochastic-oscillator-calculator](https://vinkius.com/mcp/stochastic-oscillator-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stochastic Oscillator Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stochastic-oscillator-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stochastic Oscillator Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stochastic-oscillator-calculator": {
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
