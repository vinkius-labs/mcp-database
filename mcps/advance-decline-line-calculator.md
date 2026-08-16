# Advance-Decline Line Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/advance-decline-line-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate market breadth indicators like ADL, McClellan Oscillator, and divergence.

## Description
This MCP server provides deterministic tools for calculating critical market breadth indicators. Use `get_daily_breadth_metrics` to compute Net Advancers and the cumulative Advance-Decline Line (ADL). Use `get_oscillator_metrics` to derive the AD Line Oscillator and the McClellan Oscillator from historical data. Finally, use `get_summation_and_divergence` to track the long-term Summation Index and detect bullish or bearish divergences between price indices and the ADL.


## Available Tools (3)
- **get_daily_breadth_metrics**: Calculates the fundamental daily breadth figures including Net Advancers and the updated ADL
- **get_oscillator_metrics**: Calculates momentum indicators (AD Line Oscillator and McClellan Oscillator) using historical daily data
- **get_summation_and_divergence**: Provides long-term trend tracking via the Summation Index and identifies potential trend reversals via Divergence detection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Advance-Decline Line Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the current ADL given 150 advancing, 100 declining, and a previous ADL of 500."

**🤖 AI Agent:**
> The net advancers are 50, and the new cumulative ADL is 550.

---

**👤 You:**
> "What is the McClellan Oscillator if the 19-day EMA of net advancers is 10 and the 39-day EMA is 4?"

**🤖 AI Agent:**
> The McClellan Oscillator is 6.

---

**👤 You:**
> "Check for divergence if the price index hit a new high but the ADL did not."

**🤖 AI Agent:**
> A bearish divergence has been detected.


## ❓ FAQ

**Q: What is the Advance-Decline Line (ADL)?**
The ADL is a cumulative indicator that tracks the running total of Net Advancers (advancing stocks minus declining stocks) to show market breadth trends.

**Q: How do I detect market divergence?**
You can use the `get_summation_and_divergence` tool. It compares the price index history against the ADL history to identify bullish or bearish divergence signals.

**Q: Can I calculate the McClellan Oscillator?**
Yes, the `get_oscillator_metrics` tool calculates both the AD Line Oscillator and the McClellan Oscillator using historical Net Advancer data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/advance-decline-line-calculator](https://vinkius.com/ai-agent-connect/advance-decline-line-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Advance-Decline Line Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `advance-decline-line-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Advance-Decline Line Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "advance-decline-line-calculator": {
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
