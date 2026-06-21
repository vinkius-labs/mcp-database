# Blocknative (Ethereum Mempool API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blocknative-ethereum-mempool-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Get real-time Ethereum gas price suggestions based on live mempool data from Blocknative.

## Description
Connect to the **Blocknative Gas Platform** to access high-confidence gas price estimations directly from your AI agent. By monitoring the Ethereum mempool in real-time, this server helps you optimize transaction costs and speed.

### What you can do

- **Real-time Gas Prices** — Fetch current gas price suggestions categorized by confidence levels (99%, 95%, 70%, etc.)
- **Mempool Insights** — Access data derived from live mempool conditions to ensure your transactions get included in the next block
- **Cost Optimization** — Compare different gas price tiers to balance between cost and speed for your Ethereum operations

### How it works

1. Subscribe to this server
2. Enter your Blocknative API Key
3. Ask your AI for the latest gas prices before sending any transaction

### Who is this for?

- **Web3 Developers** — Integrate gas estimation into your development workflow to avoid overpaying or stuck transactions
- **DeFi Traders** — Monitor gas spikes to time your swaps and liquidity provisions perfectly
- **Crypto Enthusiasts** — Quickly check network congestion levels through natural language


## Available Tools
- **get_gas_prices**: Get real-time gas price suggestions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blocknative (Ethereum Mempool API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the current Ethereum gas prices according to Blocknative?"

**🤖 AI Agent:**
> I've fetched the latest gas prices. For a 99% confidence of inclusion in the next block, the suggested base fee is 15 Gwei with a priority fee of 1.5 Gwei. Lower confidence tiers (70%) are around 12 Gwei.

---

**👤 You:**
> "Give me gas price suggestions for a high-priority transaction."

**🤖 AI Agent:**
> For high priority, you should use the 99% confidence tier. Blocknative suggests a Max Fee of 18.5 Gwei and a Priority Fee of 2.0 Gwei based on current mempool congestion.

---

**👤 You:**
> "Is the Ethereum network congested right now? Check the gas prices."

**🤖 AI Agent:**
> Checking the mempool... Gas prices are currently elevated, with the 99% confidence tier at 45 Gwei. This suggests significant activity or a spike in demand on the network.


## ❓ FAQ

**Q: How can I get the most accurate gas price for an urgent Ethereum transaction?**
Use the `get_gas_prices` tool. It fetches high-confidence suggestions directly from Blocknative's mempool monitoring, providing you with the exact values needed for rapid inclusion.

**Q: What confidence levels does the gas price tool provide?**
The `get_gas_prices` tool returns estimations for various confidence intervals (typically 99%, 95%, 90%, 80%, and 70%), allowing you to choose the right balance between cost and certainty.

**Q: Does this tool monitor the live Ethereum mempool?**
Yes. The `get_gas_prices` action leverages Blocknative's global node network to analyze pending transactions in the mempool, ensuring the suggestions reflect current network conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blocknative-ethereum-mempool-api](https://vinkius.com/mcp/blocknative-ethereum-mempool-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blocknative (Ethereum Mempool API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blocknative-ethereum-mempool-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blocknative (Ethereum Mempool API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blocknative-ethereum-mempool-api": {
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
