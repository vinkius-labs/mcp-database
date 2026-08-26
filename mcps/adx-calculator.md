# ADX-Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/adx-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Average Directional Index (ADX) calculator using Wilder's smoothing.

## Description
This MCP server provides precise technical analysis tools for measuring trend strength and direction. It implements the Average Directional Index (ADX) using Wilder's smoothing method. Users can utilize `calculate_adx_indicators` to generate a full series of trend metrics, `get_latest_adx_summary` for the most recent trend state, or `validate_price_data` to ensure price arrays meet the required structural criteria for calculation.


## Available Tools (3)
- **validate_price_data**: Checks if the provided price arrays are valid for indicator calculation
- **calculate_adx_indicators**: Calculates the core ADX, +DI, -DI, and trend metrics for a provided set of price data
- **get_latest_adx_summary**: Retrieves the most recent trend analysis from a set of price data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ADX-Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ADX indicators for these prices: High [150, 155, 152], Low [145, 148, 147], Close [148, 152, 150]."

**🤖 AI Agent:**
> The calculated ADX series shows a trend strength of Weak Trend and a directional bias of Uptrend.

---

**👤 You:**
> "Give me the latest ADX summary for the following data: High [10, 12, 11], Low [8, 9, 8], Close [9, 11, 10]."

**🤖 AI Agent:**
> The most recent ADX is 22.5, indicating a Weak Trend with an Uptrend bias.

---

**👤 You:**
> "Is this price data valid for a 14-period ADX calculation: High [10, 11], Low [9, 10], Close [9.5, 10.5]?"

**🤖 AI Agent:**
> No, the data is insufficient for a 14-period calculation as there are only 2 data points.


## ❓ FAQ

**Q: What is the purpose of this tool?**
It calculates the Average Directional Index (ADX) to quantify trend strength and directional bias using high, low, and close price data.

**Q: How is trend strength determined?**
A trend is considered strong when the ADX value exceeds 25.

**Q: What data is required for calculation?**
You must provide arrays of high prices, low prices, and close prices. The arrays must have matching lengths and sufficient data points for the chosen period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/adx-calculator](https://vinkius.com/ai-agent-connect/adx-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ADX-Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adx-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ADX-Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adx-calculator": {
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
