# Roll Yield Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/roll-yield-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic signal engine for capturing returns from futures curve structures.

## Description
This MCP server provides advanced tools to identify profitable roll yield opportunities in futures markets. By analyzing the relationship between front-month and second-month contracts, it identifies market regimes like contango and backwardation. Use `calculate_roll_signals` to generate daily BUY/SELL/HOLD signals based on roll yield thresholds and trend confirmation. Use `analyze_roll_economics` to calculate expected roll returns and costs, or `get_curve_status` for a quick snapshot of the current market structure.


## Available Tools (3)
- **analyze_roll_economics**: Calculates the theoretical profit/loss metrics associated with the current curve structure
- **calculate_roll_signals**: Generates daily trading signals based on curve structure, roll yield thresholds, and trend confirmation
- **get_curve_status**: Provides a snapshot of the current market structure and yield


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roll Yield Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for the current futures curve."

**🤖 AI Agent:**
> The current signal is BUY. The market is in strong backwardation with a roll yield of -2.5%, and the front-month price is above its 20-day MA.

---

**👤 You:**
> "What is the current market structure and yield?"

**🤖 AI Agent:**
> The market is currently in contango with an annualized roll yield of 1.5%.

---

**👤 You:**
> "Calculate the expected economics for this roll."

**🤖 AI Agent:**
> The expected roll return is 0.45% with a projected roll cost of 0.12% due to the current contango structure.


## ❓ FAQ

**Q: How are trading signals generated?**
Signals are generated using `calculate_roll_signals`, which evaluates roll yield, curve structure, and 20-day moving average trends while enforcing liquidity filters.

**Q: What is the difference between contango and backwardation?**
Contango occurs when the second-month price is higher than the front-month price, resulting in negative roll yield. Backwardation occurs when the second-month price is lower, resulting in positive roll yield.

**Q: Does this tool require API keys for futures data?**
No. You connect via Vinkius Edge using your personal Connection Token. No external vendor API keys are required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/roll-yield-strategy-engine](https://vinkius.com/ai-agent-connect/roll-yield-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roll Yield Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roll-yield-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roll Yield Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roll-yield-strategy-engine": {
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
