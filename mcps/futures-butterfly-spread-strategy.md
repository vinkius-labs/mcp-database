# Futures Butterfly Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-butterfly-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate deterministic trading signals for futures butterfly spreads using z-score mean reversion.

## Description
This MCP server provides deterministic trading signals for futures butterfly spreads. It identifies opportunities by calculating the butterfly value and its z-score relative to a moving average. Use `calculate_butterfly_signals` to detect compressed or expanded spreads based on liquidity and contract spacing. You can also use `validate_contract_structure` to ensure contract triplets meet liquidity requirements, or `get_butterfly_financial_metrics` to calculate potential profit width and convergence targets.


## Available Tools (3)
- **calculate_butterfly_signals**: Generates daily trading signals and technical metrics for a set of three futures contracts
- **get_butterfly_financial_metrics**: Calculates the specific profit-taking and risk metrics for a current butterfly position
- **validate_contract_structure**: Checks if a triplet of futures contracts meets the required structural and liquidity criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Butterfly Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for these futures: near price [100, 102], middle price [50, 51], far price [105, 104], open interest [6000, 6000, 6000], and intervals ['Mar24', 'Jun24', 'Sep24']."

**🤖 AI Agent:**
> The signal for the second day is BUY with a butterfly value of 3.0 and a z-score of -2.1.

---

**👤 You:**
> "Check if these contracts are valid for a butterfly spread: Mar24, Jun24, Sep24 with OI of 7000 each."

**🤖 AI Agent:**
> The contract structure is valid for trading.

---

**👤 You:**
> "Calculate the financial metrics for a butterfly with near price 100, middle price 50, far price 105, and a moving average of 5."

**🤖 AI Agent:**
> The butterfly width is 5.0 and the convergence target is 5.0.


## ❓ FAQ

**Q: What triggers a BUY signal?**
A BUY signal is triggered when the `butterfly_z_score` is less than -2.0, indicating the butterfly is compressed and the middle contract is overpriced relative to the wings.

**Q: How does the liquidity filter work?**
The server uses `validate_contract_structure` to ensure all three contracts have an Open Interest greater than 5,000 before a signal is considered valid.

**Q: Can I calculate profit targets?**
Yes, you can use `get_butterfly_financial_metrics` to determine the butterfly width and the convergence target based on the moving average.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-butterfly-spread-strategy](https://vinkius.com/ai-agent-connect/futures-butterfly-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Butterfly Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-butterfly-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Butterfly Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-butterfly-spread-strategy": {
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
