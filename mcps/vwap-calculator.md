# VWAP Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vwap-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Volume Weighted Average Price (VWAP) calculator with volatility bands and trend analysis.

## Description
This MCP server provides precise Volume Weighted Average Price (VWAP) calculations. It allows AI agents to compute cumulative VWAP, standard deviation volatility bands (±1, ±2, ±3), price position relative to the average, and the VWAP slope to identify trends. Use `calculate_vwap_metrics` for detailed data series or `get_vwap_summary` for a human-readable market snapshot. It supports various anchor periods including daily, weekly, monthly, and custom start dates.


## Available Tools (3)
- **calculate_vwap_metrics**: Performs the core calculation of the VWAP, its volatility bands, and directional indicators
- **get_vwap_summary**: Provides a simplified snapshot of the current market state relative to the VWAP
- **validate_input_data**: Ensures that the provided price and volume arrays are mathematically consistent and valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VWAP Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of the current market state using these prices: High [150, 152], Low [148, 149], Close [149, 151], Volume [1000, 1200] with a daily anchor."

**🤖 AI Agent:**
> The current VWAP is 149.85. The price is currently above the VWAP, and the trend is upward.

---

**👤 You:**
> "Calculate the detailed VWAP metrics for these values: High [10, 11], Low [9, 10], Close [9.5, 10.5], Volume [500, 600] using a weekly anchor."

**🤖 AI Agent:**
> The calculated VWAP values are [9.75, 10.25]. The price is currently above the VWAP, and the slope is positive.

---

**👤 You:**
> "Is this price data valid for VWAP? High [10, 9], Low [11, 8], Close [10, 9], Volume [100, 100]"

**🤖 AI Agent:**
> No, the data is invalid because the High price is lower than the Low price at the first index.


## ❓ FAQ

**Q: What is the difference between VWAP and a simple moving average?**
VWAP weights the price by the volume traded at each level, providing a more accurate view of the true average price compared to a simple moving average.

**Q: How do I reset the VWAP calculation?**
You can use the `anchorType` parameter to reset the calculation daily, weekly, monthly, or on a custom date.

**Q: Can I validate my price data before calculating?**
Yes, you can use the `validate_input_data` tool to ensure your high, low, close, and volume arrays are mathematically consistent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vwap-calculator](https://vinkius.com/ai-agent-connect/vwap-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VWAP Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vwap-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VWAP Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vwap-calculator": {
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
