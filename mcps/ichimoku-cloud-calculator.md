# Ichimoku Cloud Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ichimoku-cloud-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic engine for Ichimoku Kinko Hyo indicator components and signals.

## Description
This MCP server provides a deterministic engine for calculating all Ichimoku Kinko Hyo indicator components. It allows AI agents to compute Tenkan-sen, Kijun-sen, Senkou Span A, Senkou Span B, and Chikou Span from price data. Users can use `calculate_ichimoku_components` to generate the full indicator set, `analyze_kumo_status` to determine price position relative to the cloud and thickness, and `detect_tk_cross` to identify bullish or bearish momentum signals.


## Available Tools (3)
- **detect_tk_cross**: Identifies if a bullish or bearish Tenkan-sen/Kijun-sen crossover has occurred at the most recent data point
- **analyze_kumo_status**: Determines the relationship between the current price and the cloud, and calculates cloud thickness
- **calculate_ichimoku_components**: Calculates the raw Ichimoku indicator lines for a given series of price data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ichimoku Cloud Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Ichimoku components for these prices: High [10, 12, 11], Low [8, 9, 10], Close [9, 11, 10]."

**🤖 AI Agent:**
> The calculated components for the provided price series are Tenkan-sen: 10.0, Kijun-sen: 9.5, Senkou Span A: 9.75, Senkou Span B: 9.5, and Chikou Span: 10.0.

---

**👤 You:**
> "Is the price of 105 above, below, or inside a cloud where Span A is 100 and Span B is 95?"

**🤖 AI Agent:**
> The price is above the cloud.

---

**👤 You:**
> "Check for a TK cross with Tenkan-sen [10, 12] and Kijun-sen [11, 11]."

**🤖 AI Agent:**
> A bullish signal has been detected.


## ❓ FAQ

**Q: What components does this server calculate?**
The server calculates Tenkan-sen, Kijun-sen, Senkou Span A, Senkou Span B, and Chikou Span, and provides tools to analyze Kumo status and TK crosses.

**Q: How do I detect a trend reversal?**
You can use the `detect_tk_cross` tool to identify bullish or bearish crossovers between the Tenkan-sen and Kijun-sen lines.

**Q: Can I customize the indicator periods?**
Yes, the `calculate_ichimoku_components` tool allows you to specify custom periods for Tenkan-sen, Kijun-sen, Senkou Span B, and displacement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ichimoku-cloud-calculator](https://vinkius.com/ai-agent-connect/ichimoku-cloud-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ichimoku Cloud Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ichimoku-cloud-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ichimoku Cloud Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ichimoku-cloud-calculator": {
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
