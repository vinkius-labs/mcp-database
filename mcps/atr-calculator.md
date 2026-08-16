# ATR-Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/atr-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Average True Range and classify market volatility.

## Description
This MCP server provides deterministic technical analysis tools to measure market volatility. Use `calculate_atr` to determine the Average True Range as a percentage of price and receive a volatility classification (low, medium, or high). You can also use `get_volatility_thresholds` to retrieve historical percentile boundaries or `validate_price_data` to ensure your price arrays are mathematically sound for analysis.


## Available Tools (3)
- **validate_price_data**: Ensures that price arrays are mathematically sound and ready for technical analysis
- **calculate_atr**: Calculates the Average True Range and volatility classification for a given set of price data
- **get_volatility_thresholds**: Retrieves the historical percentile boundaries used to classify volatility levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ATR-Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ATR for these prices: High [150, 155, 152], Low [145, 148, 147], Close [148, 152, 150]."

**🤖 AI Agent:**
> The calculated ATR is 3.5% and the volatility level is medium.

---

**👤 You:**
> "What are the volatility thresholds for this dataset using Wilder's smoothing with a period of 14?"

**🤖 AI Agent:**
> The historical thresholds are: Low: 1.2%, Medium: 2.5%, and High: above 2.5%.

---

**👤 You:**
> "Check if these price arrays are valid: High [10, 12], Low [11, 9], Close [10.5, 10]."

**🤖 AI Agent:**
> The data is invalid because the low price in the second period is higher than the high price.


## ❓ FAQ

**Q: What is the difference between the smoothing methods?**
The server supports Wilder's smoothing (the traditional method), Simple Moving Average (SMA), and Exponential Moving Average (EMA).

**Q: How is volatility classified?**
Volatility is classified as low, medium, or high based on where the current ATR percentage sits within the historical distribution of the provided data.

**Q: Can I validate my price data before calculating ATR?**
Yes, you can use the `validate_price_data` tool to check if your high, low, and close price arrays are consistent and valid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/atr-calculator](https://vinkius.com/ai-agent-connect/atr-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ATR-Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `atr-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ATR-Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "atr-calculator": {
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
