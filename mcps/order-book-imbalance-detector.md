# Order Book Imbalance Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/order-book-imbalance-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Detect market microstructure imbalances and spoofing risks in the Polymarket CLOB.

## Description
This MCP server provides deterministic microstructure analysis for the Polymarket Central Limit Order Book (CLOB). It allows AI agents to identify short-term price direction by analyzing liquidity skew and execution flow. Key capabilities include calculating the exact imbalance ratio to predict price pressure, evaluating `assess_spoofing_risk` to detect manipulative large orders, and using `calculate_execution_strategy` to determine optimal limit order placement. It is designed to help agents identify BUY or SELL signals based on real-time supply and demand imbalances.


## Available Tools (3)
- **assess_spoofing_risk**: Evaluates whether large orders are likely being used to manipulate the perception of liquidity
- **calculate_execution_strategy**: Recommends specific limit order placement to capitalize on the identified imbalance
- **get_imbalance_metrics**: Calculates the core imbalance ratio and identifies the predicted price pressure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Order Book Imbalance Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current market imbalance and predicted direction?"

**🤖 AI Agent:**
> The current imbalance ratio is 0.75, which indicates upward price pressure and a BUY signal.

---

**👤 You:**
> "Is there any significant spoofing risk in the current order book?"

**🤖 AI Agent:**
> No, all large orders are currently within 5% of the mid-price, indicating low spoofing risk.

---

**👤 You:**
> "Recommend a limit order strategy based on the current imbalance of 0.25."

**🤖 AI Agent:**
> With an imbalance ratio of 0.25, the recommended strategy is a SELL limit order at the best available ask price.


## ❓ FAQ

**Q: How is the imbalance ratio calculated?**
The ratio is calculated as the sum of all bid volumes divided by the total volume (sum of bid volumes plus sum of ask volumes).

**Q: What triggers a BUY or SELL signal?**
A BUY signal is triggered when the imbalance ratio exceeds 0.70, indicating upward pressure. A SELL signal is triggered when the ratio falls below 0.30, indicating downward pressure.

**Q: How does the tool detect spoofing?**
The `assess_spoofing_risk` tool flags a high risk if any large order is positioned more than 5% away from the current mid-price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/order-book-imbalance-detector](https://vinkius.com/ai-agent-connect/order-book-imbalance-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Order Book Imbalance Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `order-book-imbalance-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Order Book Imbalance Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "order-book-imbalance-detector": {
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
