# Moving Average Ribbon Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/moving-average-ribbon-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze market trends and volatility using multi-layered Moving Average ribbons.

## Description
This MCP server provides a deterministic engine for analyzing market momentum through Moving Average (MA) ribbons. It allows AI agents to transform historical price data into multi-layered ribbons to identify trend strength, convergence, and breakout potential. Use `calculate_ribbon_values` to compute specific MA values for any period, `analyze_ribbon_geometry` to determine if the ribbon is in an expanded or compressed state, and `detect_squeeze_setup` to identify high-probability volatility breakouts following periods of compression.


## Available Tools (3)
- **analyze_ribbon_geometry**: Determine the qualitative state, trend direction, and width of the ribbon
- **calculate_ribbon_values**: Compute specific Moving Average values for every period requested
- **detect_squeeze_setup**: Identify if the current ribbon compression represents a Squeeze


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Average Ribbon Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the 10, 20, and 30 period SMA values for these closing prices: [150, 152, 151, 153, 155, 157, 156, 158, 160, 162]."

**🤖 AI Agent:**
> The SMA values are: 10-period: 154.4, 20-period: N/A (insufficient data), 30-period: N/A (insufficient data).

---

**👤 You:**
> "Analyze the ribbon geometry for these MA values: {'10': 155, '20': 150, '30': 145}."

**🤖 AI Agent:**
> The ribbon is in an ascending order, indicating an uptrend, with a width of 10.

---

**👤 You:**
> "Is there a squeeze setup if the current width is 2 and historical widths were [10, 12, 15, 14, 11]?"

**🤖 AI Agent:**
> Yes, a squeeze setup is detected with high confidence as the current width is a local minimum following an expansion.


## ❓ FAQ

**Q: What is a Moving Average Ribbon?**
A Moving Average Ribbon is a collection of multiple moving averages with different time periods plotted together to visualize trend direction and volatility.

**Q: How do I detect a market squeeze?**
You can use the `detect_squeeze_setup` tool to identify when the ribbon width reaches a local minimum after a period of expansion, signaling a potential breakout.

**Q: Can I use SMA or EMA?**
Yes, the `calculate_ribbon_values` tool supports both Simple Moving Average (SMA) and Exponential Moving Average (EMA) calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/moving-average-ribbon-calculator](https://vinkius.com/ai-agent-connect/moving-average-ribbon-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Average Ribbon Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-average-ribbon-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Average Ribbon Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-average-ribbon-calculator": {
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
