# SuperTrend Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/supertrend-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic SuperTrend indicator for trend direction and stop-loss levels.

## Description
This MCP server provides precise technical analysis tools for the SuperTrend indicator. It uses an iterative state machine to calculate trend direction, flip signals, and dynamic stop-loss levels based on volatility. Use `calculate_supertrend` to generate a full historical series or `get_latest_supertrend_state` to identify the current market trend and support/resistance levels. It also includes `validate_price_data` to ensure your price arrays are mathematically consistent before analysis.


## Available Tools (3)
- **get_latest_supertrend_state**: Retrieves the most recent calculated values from a provided dataset
- **calculate_supertrend**: Calculates the complete series of SuperTrend values, trend directions, and signals
- **validate_price_data**: Ensures that price arrays are mathematically sound and consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SuperTrend Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the SuperTrend for these prices: High [10, 12, 11], Low [8, 9, 10], Close [9, 11, 10]."

**🤖 AI Agent:**
> The trend direction is 1 (uptrend) with a stop-loss level of 9.5.

---

**👤 You:**
> "What is the current market status for these prices: High [100, 105], Low [95, 100], Close [98, 103]?"

**🤖 AI Agent:**
> The current trend is 1 (up) and the current stop-loss level is 100.0.

---

**👤 You:**
> "Check if this price data is valid: High [10, 9], Low [11, 10], Close [10, 9]."

**🤖 AI Agent:**
> The data is invalid because the high price is lower than the low price in the second bar.


## ❓ FAQ

**Q: How do I use the SuperTrend indicator?**
You can use `calculate_supertrend` to get a full dataset of trend directions and stop-loss levels, or `get_latest_supertrend_state` to quickly check the current market status.

**Q: What are the default ATR settings?**
The default ATR period is 10 and the default multiplier is 3.0, but these can be customized in the tool inputs.

**Q: How can I ensure my data is valid?**
Use the `validate_price_data` tool to check if your high, low, and close price arrays are mathematically sound and consistent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/supertrend-calculator](https://vinkius.com/ai-agent-connect/supertrend-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SuperTrend Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supertrend-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SuperTrend Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supertrend-calculator": {
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
