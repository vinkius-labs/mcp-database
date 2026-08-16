# Elder Ray Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/elder-ray-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Bulls Power, Bears Power, and detect market setups and divergences.

## Description
This MCP server provides deterministic technical analysis tools for the Elder Ray Index. It allows AI agents to calculate Bulls Power and Bears Power using EMA-based calculations. Users can identify specific Bullish and Bearish setups, detect zero-line crosses, and find momentum divergences between price action and power indices using `calculate_elder_ray_indicators`, `identify_market_setups`, and `detect_signal_events`.


## Available Tools (3)
- **calculate_elder_ray_indicators**: Performs core Elder Ray Index calculations for Bulls and Bears Power
- **identify_market_setups**: Detects bullish and bearish market setups
- **detect_signal_events**: Identifies zero-line crosses and momentum divergences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elder Ray Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Elder Ray indicators for these prices: High [150, 155], Low [140, 145], Close [145, 150]."

**🤖 AI Agent:**
> The calculated Bulls Power is [5, 10] and Bears Power is [-5, -5] based on the provided price series.

---

**👤 You:**
> "Check if there is a bullish setup with Bulls Power [2, 5] and Bears Power [-3, -1]."

**🤖 AI Agent:**
> Yes, a bullish setup is detected because Bulls Power is positive and rising while Bears Power is negative and rising toward zero.

---

**👤 You:**
> "Are there any zero-line crosses in the provided data?"

**🤖 AI Agent:**
> A zero-line cross for Bulls Power was detected at index 5.


## ❓ FAQ

**Q: What is the default EMA period used?**
The default EMA period is 13, but it can be customized via the `calculate_elder_ray_indicators` tool.

**Q: How are bullish setups identified?**
A bullish setup is identified when Bulls Power is positive and rising, while Bears Power is negative and rising toward zero.

**Q: Can I detect divergences?**
Yes, the `detect_signal_events` tool identifies momentum divergences where price direction contradicts the power indices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/elder-ray-index-calculator](https://vinkius.com/ai-agent-connect/elder-ray-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elder Ray Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elder-ray-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elder Ray Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elder-ray-index-calculator": {
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
