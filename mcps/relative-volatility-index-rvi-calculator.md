# Relative Volatility Index (RVI) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/relative-volatility-index-rvi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and analyze volatility momentum using the Relative Volatility Index.

## Description
This MCP server provides deterministic technical analysis tools for the Relative Volatility Index (RVI). Unlike the RSI, the RVI uses standard deviation to weight volatility momentum. Use `rvi_calculate` to generate RVI values from price series, `rvi_detect_signals` to identify overbought, oversold, or midpoint crossover conditions, and `rvi_check_divergence` to find discrepancies between price action and volatility trends.


## Available Tools (3)
- **rvi_calculate**: Calculates the raw RVI values and core technical indicators for a given price series
- **rvi_check_divergence**: Identifies discrepancies between price action and volatility momentum
- **rvi_detect_signals**: Analyzes the RVI series to identify actionable patterns like overbought/oversold conditions and crossovers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative Volatility Index (RVI) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RVI for these closing prices: [150.2, 152.5, 151.0, 153.4, 155.0, 154.2, 156.8, 158.0, 157.5, 159.0]"

**🤖 AI Agent:**
> The calculated RVI values for the provided series are [55.2, 58.4, 54.1, 59.8, 62.3, 60.1, 65.4, 68.2, 66.5, 70.1].

---

**👤 You:**
> "Are there any overbought signals in this RVI series: [45, 50, 55, 72, 75, 71, 48]?"

**🤖 AI Agent:**
> Yes, there are overbought signals at index 3 (value 72), index 4 (value 75), and index 5 (value 71).

---

**👤 You:**
> "Check for divergence between prices [100, 102, 101, 103, 102] and RVI values [50, 52, 51, 53, 52]."

**🤖 AI Agent:**
> No significant divergence patterns were detected in the provided data window.


## ❓ FAQ

**Q: How does RVI differ from RSI?**
While RSI uses price velocity, RVI uses standard deviation to weight the upward and downward volatility movement.

**Q: What are the overbought and oversold levels?**
Typically, an RVI value above 70 is considered overbought, and a value below 30 is considered oversold.

**Q: Can I detect price divergence?**
Yes, you can use the `rvi_check_divergence` tool to identify bullish or bearish divergence between price and volatility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/relative-volatility-index-rvi-calculator](https://vinkius.com/ai-agent-connect/relative-volatility-index-rvi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative Volatility Index (RVI) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-volatility-index-rvi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative Volatility Index (RVI) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-volatility-index-rvi-calculator": {
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
