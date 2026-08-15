# Ultimate Momentum Indicator Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ultimate-momentum-indicator-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic technical analysis tool that synthesizes multi-timeframe momentum oscillators into a single weighted indicator.

## Description
This MCP server provides precise technical analysis tools for calculating the Weighted Ultimate Momentum (UMI). By synthesizing short, medium, and long-term momentum oscillators, it identifies trend strength and reversal zones. Use `get_umi_analysis` to derive core UMI values and moving averages, `detect_umi_signals` to find zero-line crosses and overbought/oversold entries, or `get_momentum_summary` for a high-level snapshot of current market momentum.


## Available Tools (3)
- **detect_umi_signals**: 
- **get_momentum_summary**: g., Strong Bullish, Overextended) for a specific index in a price series

Provides a high-level snapshot of the current momentum state at a specific point in time
- **get_umi_analysis**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ultimate Momentum Indicator Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the UMI analysis for this price series: [150.2, 152.5, 151.0, 153.4, 155.0, 154.2, 156.8, 158.0, 157.5, 159.0]"

**🤖 AI Agent:**
> The UMI analysis for the provided series shows a positive momentum trend with a current UMI value of 2.45 and a strong trend alignment.

---

**👤 You:**
> "Check the momentum summary for the last price in this series: [100, 102, 101, 105, 107, 106, 108, 110, 112, 115] at index 9."

**🤖 AI Agent:**
> The current momentum state is Strong Bullish with a UMI of 4.12 and confirmed multi-timeframe trend alignment.

---

**👤 You:**
> "Are there any zero-line crosses in these UMI values: [1.5, 0.5, -0.2, -1.5, -0.5, 0.8, 2.0]?"

**🤖 AI Agent:**
> Yes, there is an upward zero-line cross at index 5 and a downward zero-line cross at index 2.


## ❓ FAQ

**Q: How is the UMI value calculated?**
The UMI is a weighted average of three momentum oscillators. The short period carries a weight of 4, the medium period a weight of 2, and the long period a weight of 1, all divided by 7.

**Q: What constitutes a strong trend?**
A strong trend is identified when the momentum of all three oscillators (short, medium, and long) share the same mathematical sign.

**Q: How can I find overbought or oversold signals?**
You can use the `detect_umi_signals` tool to identify when the UMI enters extreme zones, such as exceeding the upper threshold for overbought or falling below the lower threshold for oversold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ultimate-momentum-indicator-calculator](https://vinkius.com/mcp/ultimate-momentum-indicator-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ultimate Momentum Indicator Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ultimate-momentum-indicator-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ultimate Momentum Indicator Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ultimate-momentum-indicator-calculator": {
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
