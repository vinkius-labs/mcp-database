# Fisher Transform Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fisher-transform-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic Ehlers Fisher Transform for trend and reversal detection.

## Description
This MCP server provides precise technical analysis tools for the Ehlers Fisher Transform. It allows AI agents to transform price data into a Gaussian-like distribution to identify trend reversals and momentum shifts. Use `calculate_fisher_transform` to generate the full indicator sequence, `get_reversal_signals` to pinpoint extreme price exhaustion, and `get_momentum_status` to evaluate current market direction based on the relationship between Fisher values and the trigger line.


## Available Tools (3)
- **calculate_fisher_transform**: Computes the full sequence of Fisher Transform values and related signals
- **get_momentum_status**: Determines the current market momentum
- **get_reversal_signals**: Filters and identifies specific instances of trend reversals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fisher Transform Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Fisher Transform for these prices: Highs [10, 12, 11, 13, 15], Lows [8, 9, 8, 10, 11]."

**🤖 AI Agent:**
> The Fisher Transform values for the provided series are [0.12, 0.45, 0.32, 0.88, 1.15].

---

**👤 You:**
> "Is the current momentum bullish or bearish if the Fisher value is 1.2 and the trigger line is 0.5?"

**🤖 AI Agent:**
> The current momentum is Bullish.

---

**👤 You:**
> "Find reversal signals for Fisher values [0.5, 1.6, 1.7, 0.4] and trigger lines [0.4, 0.5, 0.6, 0.5]."

**🤖 AI Agent:**
> Extreme reversal signals were detected at index 1 (Upper Extreme) and index 2 (Upper Extreme).


## ❓ FAQ

**Q: How do I calculate the indicator values?**
You can use the `calculate_fisher_transform` tool by providing arrays of high and low prices and an optional lookback period.

**Q: How can I identify market reversals?**
Use the `get_reversal_signals` tool to find extreme zones where the Fisher value exceeds the specified threshold.

**Q: What determines the current market momentum?**
The `get_momentum_status` tool determines if momentum is Bullish, Bearish, or Neutral by comparing the latest Fisher value to the trigger line.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fisher-transform-calculator](https://vinkius.com/mcp/fisher-transform-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fisher Transform Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fisher-transform-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fisher Transform Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fisher-transform-calculator": {
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
