# Commodity Selection Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/commodity-selection-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the Commodity Selection Index (CSI) to identify momentum-driven trends relative to volatility.

## Description
This MCP server provides a deterministic engine for calculating the Commodity Selection Index (CSI). By analyzing the ratio of momentum to volatility, it helps identify clean price trends. Use `calculate_csi_series` to generate a full time-series of normalized values, `get_csi_signals` to interpret specific index levels for overbought or oversold conditions, and `validate_market_data` to ensure your price arrays are mathematically sound before processing.


## Available Tools (3)
- **validate_market_data**: Ensures the provided price arrays are mathematically viable
- **calculate_csi_series**: Calculates the full time-series of the Commodity Selection Index (CSI)
- **get_csi_signals**: Analyzes a specific CSI value to provide a qualitative trading signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commodity Selection Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the CSI series for these prices: High [105, 106, 107], Low [100, 101, 102], Close [102, 104, 106]."

**🤖 AI Agent:**
> { "csiValues": [45.2, 52.8, 58.1], "status": "success" }

---

**👤 You:**
> "What is the signal for a CSI value of 85?"

**🤖 AI Agent:**
> { "signalType": "Overbought", "description": "Momentum is extremely high relative to volatility.", "isExtreme": true }

---

**👤 You:**
> "Is this market data valid? High [10, 11], Low [12, 10], Close [11, 10.5]"

**🤖 AI Agent:**
> { "isValid": false, "errorMessage": "High must be greater than or equal to Low at index 0" }


## ❓ FAQ

**Q: What is the Commodity Selection Index (CSI)?**
The CSI is a technical indicator that measures price momentum relative to volatility, helping traders find strong trends that are not just market noise.

**Q: How do I know if a trend is strong?**
You can use `get_csi_signals` to analyze specific values. High values (above 80) indicate strong momentum, while low values (below 20) suggest low momentum relative to volatility.

**Q: Can I validate my data before calculating the index?**
Yes, the `validate_market_data` tool checks if your high, low, and close price arrays are mathematically consistent and have matching lengths.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/commodity-selection-index-calculator](https://vinkius.com/ai-agent-connect/commodity-selection-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Commodity Selection Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `commodity-selection-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Commodity Selection Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "commodity-selection-index-calculator": {
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
