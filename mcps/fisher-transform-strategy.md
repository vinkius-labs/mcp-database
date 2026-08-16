# Fisher Transform Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fisher-transform-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic mean-reversion strategy using Fisher Transform to identify market exhaustion.

## Description
This MCP server provides tools to execute a deterministic mean-reversion trading strategy. It uses the Fisher Transform to convert price distributions into a Gaussian shape, making extreme market exhaustion visible. Users can use `calculate_fisher_indicators` to compute momentum metrics, `generate_trading_signals` to identify BUY and SELL reversals after sustained extreme zones, and `get_strategy_summary` to evaluate performance metrics like win rate and drawdown.


## Available Tools (3)
- **calculate_fisher_indicators**: Compute core Fisher Transform values and metrics
- **generate_trading_signals**: Evaluate indicators to determine BUY, SELL, or HOLD signals
- **get_strategy_summary**: Provide a statistical overview of strategy performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fisher Transform Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Fisher Transform indicators for these price arrays."

**🤖 AI Agent:**
> The Fisher Transform values have been calculated, including strength, extreme duration, and trigger distance for the provided price series.

---

**👤 You:**
> "Generate trading signals based on the provided Fisher indicators."

**🤖 AI Agent:**
> The strategy generated a BUY signal at price 150.25 with a stop-loss at 147.25 and a take-profit at 155.00.

---

**👤 You:**
> "Show me the performance summary for the last 50 trades."

**🤖 AI Agent:**
> The strategy achieved a win rate of 58% with a total profit factor of 1.45 and a maximum drawdown of 4.2%.


## ❓ FAQ

**Q: What is the core logic of this strategy?**
The strategy identifies extreme market exhaustion using the Fisher Transform. It triggers a BUY signal when the Fisher value crosses above the trigger line after being in a sustained oversold state, and a SELL signal when it crosses below after a sustained overbought state.

**Q: How are stop-loss and take-profit levels determined?**
Stop-loss is set at the most recent swing extreme or a 2% deviation from entry. Take-profit occurs when the Fisher value returns to the trigger line (zero) or reaches the opposite extreme threshold.

**Q: Which AI clients can use this MCP?**
This MCP can be used with Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fisher-transform-strategy](https://vinkius.com/mcp/fisher-transform-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fisher Transform Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fisher-transform-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fisher Transform Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fisher-transform-strategy": {
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
