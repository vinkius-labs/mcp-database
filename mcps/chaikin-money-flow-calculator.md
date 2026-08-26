# Chaikin Money Flow Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/chaikin-money-flow-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis engine for CMF, A/D Line, and momentum signals.

## Description
This MCP server provides a deterministic technical analysis engine to evaluate market pressure. It calculates core indicators including Money Flow Multiplier (MFM), Money Flow Volume (MFV), and the Accumulation/Distribution (A/D) Line. Users can use `calculate_money_flow` to generate these metrics, `analyze_cmf_signals` to identify zero-line crosses and sustained accumulation or distribution phases, and `detect_cmf_divergence` to find discrepancies between price action and momentum.


## Available Tools (3)
- **calculate_money_flow**: Computes core technical indicators (MFM, MFV, A/D Line, and CMF)
- **analyze_cmf_signals**: Identifies zero-line crosses and sustained accumulation/distribution phases
- **detect_cmf_divergence**: Detects discrepancies between price action and money flow momentum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chaikin Money Flow Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the money flow metrics for these prices: high [10, 12, 11], low [8, 9, 10], close [9, 11, 10.5], and volume [100, 150, 120]."

**🤖 AI Agent:**
> The calculated Money Flow Multiplier (MFM) for the final period is 0.5, and the Chaikin Money Flow (CMF) for the period is 0.12.

---

**👤 You:**
> "Check for momentum signals in these CMF values: [0.1, 0.3, 0.4, -0.1, -0.3]."

**🤖 AI Agent:**
> A bearish zero-line cross was detected at index 3.

---

**👤 You:**
> "Are there any divergences between these prices [100, 95, 90] and CMF values [0.1, 0.2, 0.3]?"

**🤖 AI Agent:**
> A bullish divergence was detected where prices made lower lows while CMF made higher lows.


## ❓ FAQ

**Q: What indicators does this server calculate?**
The server calculates the Money Flow Multiplier, Money Flow Volume, Accumulation/Distribution Line, and Chaikin Money Flow (CMF).

**Q: How do I detect bullish divergences?**
You can use the `detect_cmf_divergence` tool, which identifies bullish divergences when prices make lower lows but CMF makes higher lows.

**Q: Can I customize the CMF lookback period?**
Yes, the `calculate_money_flow` tool allows you to specify a custom `cmfPeriod`. If not provided, it defaults to 20.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/chaikin-money-flow-calculator](https://vinkius.com/ai-agent-connect/chaikin-money-flow-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chaikin Money Flow Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chaikin-money-flow-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chaikin Money Flow Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chaikin-money-flow-calculator": {
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
