# Blockchain.com Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockchaincom-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access real-time Bitcoin blockchain data via Blockchain.com — query blocks, transactions, and addresses directly from any AI agent.

## Description
Connect your AI agent to the **Blockchain.com Data API** and orchestrate your cryptocurrency and blockchain analysis workflows through natural conversation.

### What you can do

- **Block Oversight** — Retrieve details for the latest or specific Bitcoin blocks including height and hashes.
- **Transaction Auditing** — Query and inspect individual transactions to verify payments and mempool status.
- **Address Intelligence** — Monitor balances and transaction histories for any public Bitcoin address.
- **Market Insights** — Access real-time BTC ticker prices across various fiat currencies and historical market charts.
- **Network Health** — Retrieve general Bitcoin network statistics, including difficulty and total block count.
- **Mempool Monitoring** — Get real-time stats on the memory pool to track pending network load.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Blockchain.com API Key for higher rate limits
3. Start exploring the blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Analysts** — quickly check address balances and transaction confirmations without a separate explorer.
- **Financial Researchers** — retrieve historical price charts and network difficulty data straight from their editor.
- **Web3 Developers** — verify on-chain data and monitor mempool activity using natural language.


## Available Tools
- **get_address**: Get balance and transaction history for a Bitcoin address
- **get_block_count**: Get the current total block count (height)
- **get_block**: Get details of a specific block by hash
- **get_chart**: Retrieve historical chart data (e.g. market-price, n-transactions)
- **get_latest_block**: Get details of the latest Bitcoin block
- **get_mempool_stats**: Get current mempool statistics
- **get_network_stats**: Get general Bitcoin network statistics
- **get_ticker**: Get current BTC prices in various fiat currencies
- **get_transaction**: Get details of a specific transaction by hash
- **list_unconfirmed_transactions**: List current unconfirmed transactions in the mempool


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blockchain.com Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the balance for Bitcoin address 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa."

**🤖 AI Agent:**
> I've checked the address. It currently has a balance of 72.73 BTC. It has received a total of 105.44 BTC and sent 32.71 BTC across 3,500 transactions.

---

**👤 You:**
> "Show me the latest block hash and height."

**🤖 AI Agent:**
> The latest block is at height 835,421. Its hash is `00000000000000000003...`. It was mined about 8 minutes ago and contains 2,450 transactions.

---

**👤 You:**
> "What's the current market price of Bitcoin?"

**🤖 AI Agent:**
> Bitcoin is currently trading at $65,420.50 USD. In other currencies, it's €60,123.40 EUR and £51,234.80 GBP.


## ❓ FAQ

**Q: Can I check the balance of any Bitcoin address?**
Yes! Use the `get_address` tool with the public Bitcoin address. Your agent will fetch the current balance (in Satoshis) and the transaction history directly from the blockchain.

**Q: How do I see the current price of Bitcoin in USD?**
Simply ask the agent to `get_ticker`. It will retrieve the latest exchange rates for BTC across multiple currencies, including USD, EUR, and GBP.

**Q: Does the integration allow sending Bitcoin?**
No. For security reasons, the current toolset is focused exclusively on blockchain data discovery and analysis (Read-Only). Sending transactions requires a private wallet and specialized signing procedures not supported by this data-centric server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockchaincom-data](https://vinkius.com/mcp/blockchaincom-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blockchain.com Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `blockchaincom-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blockchain.com Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blockchaincom-data": {
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
