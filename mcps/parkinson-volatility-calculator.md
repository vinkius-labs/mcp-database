# Parkinson Volatility Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/parkinson-volatility-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise Parkinson volatility using high-low price ranges.

## Description
This MCP server provides a deterministic engine for calculating Parkinson volatility. By utilizing the high-low price range instead of just closing prices, it captures intraday price movement more effectively. Use `calculate_parkinson_volatility` for direct calculations, `get_volatility_context` to compare Parkinson volatility against close-to-close moves and percentile ranks, or `compare_volatilities` to evaluate the ratio of intraday to end-of-day volatility across multiple timeframes.


## Available Tools (3)
- **compare_volatilities**: Answers how the current intraday volatility (Parkinson) compares to the end-of-day volatility (Close-to-Close) over multiple timeframes
- **get_volatility_context**: Provides a comparative view of Parkinson volatility against standard close-to-close volatility and its percentile rank
- **calculate_parkinson_volatility**: Calculates the annualized Parkinson volatility for a specific set of price data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parkinson Volatility Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Parkinson volatility for these high prices [105, 106, 104] and low prices [100, 101, 99] with a lookback of 3 and annualization of 252."

**🤖 AI Agent:**
> The annualized Parkinson volatility for the provided data is 0.245.

---

**👤 You:**
> "Compare the intraday and end-of-day volatility for these prices."

**🤖 AI Agent:**
> The Parkinson volatility is 0.15 and the close-to-close volatility is 0.12, resulting in a ratio of 1.25, indicating significant intraday movement.

---

**👤 You:**
> "What is the volatility percentile rank for the current market conditions?"

**🤖 AI Agent:**
> The current Parkinson volatility is at the 85th percentile relative to its historical distribution.


## ❓ FAQ

**Q: What is Parkinson volatility?**
Parkinson volatility is a measure of historical volatility that uses the high and low prices of an asset within a period, providing a more efficient estimate than standard close-to-close volatility.

**Q: How does this compare to close-to-close volatility?**
Parkinson volatility uses the intraday range, making it more sensitive to price swings within a period. You can use `compare_volatilities` to see the ratio between Parkinson and close-to-close volatility.

**Q: Can I calculate volatility for different timeframes?**
Yes, you can specify different lookback periods in the tools to evaluate volatility across various timeframes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/parkinson-volatility-calculator](https://vinkius.com/ai-agent-connect/parkinson-volatility-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parkinson Volatility Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parkinson-volatility-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parkinson Volatility Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parkinson-volatility-calculator": {
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
