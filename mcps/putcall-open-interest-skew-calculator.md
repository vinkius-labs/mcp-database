# Put/Call Open Interest Skew Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/putcall-open-interest-skew-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic analysis of put/call open interest skew, max pain, and market sentiment levels.

## Description
This MCP server provides deterministic tools for analyzing options market sentiment through open interest data. It calculates the Put/Call (PC) ratio per strike, identifies the Max Pain strike, and determines key support and resistance levels based on OI concentration. Users can also analyze the skew slope via linear regression of PC ratio against moneyness to detect fear or greed extremes. Use `analyze_strike_data` to extract core price levels, `calculate_skew_metrics` to evaluate the skew slope, and `get_market_sentiment_summary` for a qualitative market overview.


## Available Tools (3)
- **analyze_strike_data**: Analyze strike data
- **calculate_skew_metrics**: Calculate skew
- **get_market_sentiment_summary**: Get sentiment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Put/Call Open Interest Skew Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this strike data: strikes [100, 105, 110], callOis [50, 100, 150], putOis [100, 50, 20], underlyingPrice 105."

**🤖 AI Agent:**
> The Max Pain strike is 105. Support is at 100 with 100 Put OI, and resistance is at 110 with 150 Call OI.

---

**👤 You:**
> "What is the current market sentiment based on these metrics?"

**🤖 AI Agent:**
> The market sentiment is Bearish due to a high PC ratio and a positive skew slope.

---

**👤 You:**
> "Calculate the skew metrics for these strike ratios."

**🤖 AI Agent:**
> The skew slope is 0.45, and no extreme sentiment was detected.


## ❓ FAQ

**Q: What is the purpose of this MCP?**
It provides mathematical analysis of options open interest, including skew, max pain, and support/resistance levels.

**Q: How do I identify market support and resistance?**
The `analyze_strike_data` tool identifies the support strike as the highest Put OI and the resistance strike as the highest Call OI.

**Q: Can I detect market fear using this tool?**
Yes, `calculate_skew_metrics` identifies fear extremes when there is an unusually high concentration of Put OI at OTM strikes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/putcall-open-interest-skew-calculator](https://vinkius.com/mcp/putcall-open-interest-skew-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Put/Call Open Interest Skew Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `putcall-open-interest-skew-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Put/Call Open Interest Skew Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "putcall-open-interest-skew-calculator": {
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
