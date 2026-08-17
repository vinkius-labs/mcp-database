# Crush Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crush-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze soybean processing margins and generate deterministic trading signals.

## Description
This MCP server provides tools to evaluate soybean processing margins, known as crush spreads. By analyzing the relationship between soybean futures and its products (meal and oil), users can identify market extremes. Use `calculate_crush_signals` to detect BUY or SELL signals based on z-score deviations, or `get_crush_statistics` to analyze historical volatility and spread ranges.


## Available Tools (3)
- **calculate_crush_signals**: Computes daily crush spreads, statistical indicators, and trading signals
- **get_seasonal_crush_patterns**: Identifies the historical relationship between soybean supply tightness and crush spread widening
- **get_crush_statistics**: Analyzes the historical behavior and volatility of the crush spread


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crush Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the current crush signals for these soybean prices: [12.5, 12.6, 12.4], meal prices: [350, 355, 352], oil prices: [15, 16, 15.5], and soybean OI: [10000, 11000, 10500], meal OI: [8000, 8500, 8200], and oil OI: [6000, 6500, 6200]."

**🤖 AI Agent:**
> The current signal is BUY with a crush spread of $1.85 and a z-score of -2.1, suggesting a compressed margin opportunity.

---

**👤 You:**
> "What is the historical volatility of the crush spread for these prices?"

**🤖 AI Agent:**
> The historical volatility for the provided period is 0.45 with an average spread of $1.65.

---

**👤 You:**
> "Show me the seasonal patterns for soybean supply tightness."

**🤖 AI Agent:**
> Margins historically expand during months 7 and 8 due to increased supply tightness.


## ❓ FAQ

**Q: What is a crush spread?**
A crush spread is the profit margin for processors who buy soybeans and sell the resulting meal and oil.

**Q: How are trading signals generated?**
Signals are generated using `calculate_crush_signals` when the z-score indicates the margin is significantly compressed or expanded relative to its moving average.

**Q: What are the liquidity requirements?**
The strategy requires all constituent contracts to have an Open Interest greater than 5,000 to ensure sufficient liquidity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crush-spread-strategy](https://vinkius.com/ai-agent-connect/crush-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crush Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crush-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crush Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crush-spread-strategy": {
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
