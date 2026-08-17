# Futures Relative Value Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-relative-value-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify mispricings between related futures contracts using statistical z-scores and fundamental fair value models.

## Description
This MCP server provides a deterministic framework for executing relative value trades in futures markets. By connecting AI agents to real-time price series and fundamental data, it identifies arbitrage opportunities where the price ratio between two assets deviates from its statistical mean or its theoretical fair value. The server uses `analyze_futures_relationship` to ensure liquidity and correlation, `calculate_theoretical_fair_value` to establish a fundamental baseline, and `generate_trading_signal` to produce actionable BUY or SELL directions based on z-scores and quality/logistics adjustments.

### Available Tools

`analyze_relationship_tool`, `calculate_fair_value_tool`, `generate_signal_tool`, `analyze_relationship`, `calculate_fair_value`, `generate_signal`


## Available Tools (3)
- **analyze_relationship**: Evaluates the statistical and liquidity-based relationship between two futures contracts
- **calculate_fair_value**: Determines the expected ratio between two contracts based on historical averages and physical market drivers
- **generate_signal**: Computes the daily trading signal by comparing the current price ratio against statistical bounds and fundamental fair values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Relative Value Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the relationship between WTI and Brent crude and check if there is a trading signal."

**🤖 AI Agent:**
> The correlation between WTI and Brent is 0.92 and both are highly liquid. The current z-score is -2.4 and the ratio is higher than the theoretical fair value, resulting in a BUY_A_SELL_B signal.

---

**👤 You:**
> "Calculate the theoretical fair value for a spread between two energy contracts."

**🤖 AI Agent:**
> The calculated theoretical fair value ratio is 1.05 based on the provided historical average, quality adjustment, and logistics costs.

---

**👤 You:**
> "Is there a signal for the current price ratio of these two futures?"

**🤖 AI Agent:**
> The current signal is NEUTRAL because the ratio change over the last 30 days was only 2%, which falls below the 5% noise filter threshold.


## ❓ FAQ

**Q: What kind of futures contracts can I trade with this strategy?**
The strategy is designed for highly liquid, related commodities. It uses `analyze_futures_relationship` to verify that both contracts have an Open Interest greater than 10,000 and a correlation higher than 0.8 before generating a signal. Tools available: `analyze_relationship_tool`, `calculate_fair_value_tool`, `generate_signal_tool`.

**Q: How is the theoretical fair value calculated?**
The fair value is determined by the `calculate_theoretical_fair_value` tool, which sums the historical average ratio, the quality adjustment (intrinsic value difference), and the logistics cost (transportation expense).

**Q: What triggers a trading signal?**
A signal is generated via `generate_trading_signal` when the z-score indicates a significant deviation. A BUY signal occurs if the z-score is below -2.0 and the ratio is above the theoretical value. A SELL signal occurs if the z-score is above 2.0 or the ratio is below the theoretical value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-relative-value-strategy](https://vinkius.com/ai-agent-connect/futures-relative-value-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Relative Value Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-relative-value-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Relative Value Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-relative-value-strategy": {
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
