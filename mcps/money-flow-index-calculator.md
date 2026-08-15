# Money Flow Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/money-flow-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Money Flow Index (MFI) and detect price divergences.

## Description
This MCP server provides technical analysis tools to calculate the Money Flow Index (MFI), a momentum oscillator that measures the intensity of money flowing in and out of an asset. It includes tools to `calculate_mfi` using price and volume data, `analyze_mfi_levels` to identify overbought or oversold conditions, and `detect_mfi_divergence` to find discrepancies between price action and momentum.


## Available Tools (3)
- **analyze_mfi_levels**: 
- **calculate_mfi**: 
- **detect_mfi_divergence**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Money Flow Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the MFI for these prices and volumes: High [10, 12, 11], Low [8, 9, 10], Close [9, 11, 10], Volume [100, 150, 120] with a period of 2."

**🤖 AI Agent:**
> The calculated MFI values are [50.0, 45.5].

---

**👤 You:**
> "Are there any overbought signals in these MFI values: [75, 82, 85]?"

**🤖 AI Agent:**
> Yes, the MFI values indicate overbought conditions.

---

**👤 You:**
> "Check for divergence with prices [100, 105, 102] and MFI values [50, 55, 52]."

**🤖 AI Agent:**
> No significant divergences were detected in the provided data.


## ❓ FAQ

**Q: What is the Money Flow Index?**
The Money Flow Index (MFI) is a momentum oscillator that uses both price and volume data to measure the strength of price movements.

**Q: How do I check for overbought conditions?**
You can use the `analyze_mfi_levels` tool. It identifies overbought conditions when the MFI value exceeds 80.

**Q: Can this tool detect trend reversals?**
Yes, by using `detect_mfi_divergence`, you can identify bullish or bearish divergences that often precede trend reversals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/money-flow-index-calculator](https://vinkius.com/mcp/money-flow-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Money Flow Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `money-flow-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Money Flow Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "money-flow-index-calculator": {
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
