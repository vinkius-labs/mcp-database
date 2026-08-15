# Klinger Oscillator Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klinger-oscillator-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic technical analysis engine for Klinger Volume Oscillator metrics.

## Description
This MCP server provides precise technical analysis tools for the Klinger Volume Oscillator (KVO). It allows AI agents to compute KVO values, signal lines, and volume force series using historical price and volume data. Additionally, it provides specialized tools to `identify_crossovers` between the KVO and its signal line, and `detect_divergences` between price action and KVO momentum to identify potential trend reversals.


## Available Tools (3)
- **calculate_kvo_metrics**: Computes the primary Klinger Oscillator values and the signal line
- **detect_divergences**: Identifies instances where price action and KVO momentum are moving in opposing directions
- **identify_crossovers**: Detects points where the KVO crosses its signal line


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klinger Oscillator Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Klinger Oscillator metrics for these prices: High [10, 12, 11], Low [8, 9, 8], Close [9, 11, 10], and Volume [100, 150, 120]."

**🤖 AI Agent:**
> The calculated KVO values and signal line for the provided dataset are ready for analysis.

---

**👤 You:**
> "Are there any bullish crossovers in this KVO series: [2, 5, 8, 4, 1] and signal line [3, 3, 3, 3, 3]?"

**🤖 AI Agent:**
> A bullish crossover was detected at index 1 where the KVO moved above the signal line.

---

**👤 You:**
> "Check for divergences between these prices: High [10, 15, 14], Low [5, 10, 9], Close [7, 12, 11] and KVO values [2, 5, 4]."

**🤖 AI Agent:**
> A bearish divergence was identified where the price reached a higher high but the KVO reached a lower high.


## ❓ FAQ

**Q: What does the Klinger Oscillator measure?**
The Klinger Oscillator measures volume-based momentum to identify trend changes and potential reversals by analyzing the relationship between price action and volume force.

**Q: How can I find trend reversals using this tool?**
You can use `identify_crossovers` to find when the KVO crosses its signal line, or `detect_divergences` to find discrepancies between price movement and KVO momentum.

**Q: What data is required for calculations?**
To use `calculate_kvo_metrics`, you must provide arrays for high prices, low prices, close prices, and volume data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klinger-oscillator-calculator](https://vinkius.com/mcp/klinger-oscillator-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Klinger Oscillator Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `klinger-oscillator-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Klinger Oscillator Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "klinger-oscillator-calculator": {
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
