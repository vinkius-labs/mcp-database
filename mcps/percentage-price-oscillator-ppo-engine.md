# Percentage Price Oscillator (PPO) Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/percentage-price-oscillator-ppo-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic engine for calculating normalized price momentum via PPO indicators.

## Description
This MCP server provides a deterministic engine for calculating the Percentage Price Oscillator (PPO), a momentum indicator that measures the percentage difference between fast and slow EMAs. Unlike standard MACD, PPO is normalized, allowing for consistent momentum comparison across different assets. Use `calculate_ppo_metrics` to generate the oscillator, signal line, and histogram. You can also use `detect_ppo_events` to identify zero-line crosses and signal crossovers, or `detect_ppo_divergence` to find discrepancies between price action and momentum. For comparative analysis, `compare_with_macd` provides a direct look at PPO versus absolute MACD values.


## Available Tools (4)
- **calculate_ppo_metrics**: Calculates the full suite of PPO indicators
- **compare_with_macd**: Provides a comparative analysis between PPO and standard MACD
- **detect_ppo_divergence**: Finds discrepancies between price movements and PPO momentum
- **detect_ppo_events**: Identifies specific momentum triggers like zero-line crosses and signal crossovers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Percentage Price Oscillator (PPO) Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the PPO metrics for these closing prices: [150.2, 152.5, 151.0, 153.4, 155.0, 154.2, 156.8]."

**🤖 AI Agent:**
> The PPO oscillator value is 0.45, the signal line is 0.32, and the histogram is 0.13.

---

**👤 You:**
> "Are there any bullish divergences in this price series: [100, 105, 102, 108, 104, 110]?"

**🤖 AI Agent:**
> No bullish divergences were detected in the provided price series.

---

**👤 You:**
> "Compare the PPO and MACD for these prices: [50, 51, 52, 51, 50, 49]."

**🤖 AI Agent:**
> The PPO shows a momentum decline of -0.15%, while the MACD shows an absolute difference of -0.45.


## ❓ FAQ

**Q: How is PPO different from MACD?**
MACD measures the absolute difference between EMAs, while PPO measures the percentage difference. This normalization makes PPO better for comparing momentum across different assets with different price scales.

**Q: What are the default periods for the calculation?**
The default settings are a fast period of 12, a slow period of 26, and a signal period of 9.

**Q: Can I detect trend reversals using this server?**
Yes, you can use `detect_ppo_events` to find zero-line crosses and signal crossovers, which are common indicators of momentum shifts and potential trend reversals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/percentage-price-oscillator-ppo-engine](https://vinkius.com/ai-agent-connect/percentage-price-oscillator-ppo-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Percentage Price Oscillator (PPO) Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `percentage-price-oscillator-ppo-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Percentage Price Oscillator (PPO) Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "percentage-price-oscillator-ppo-engine": {
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
