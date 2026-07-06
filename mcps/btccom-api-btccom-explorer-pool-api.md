# BTC.com API (BTC.com Explorer & Pool API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/btccom-api-btccom-explorer-pool-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time Bitcoin blockchain data and mining pool statistics including blocks, transactions, addresses, and worker performance.

## Description
Connect to the **BTC.com API** to integrate comprehensive Bitcoin blockchain exploration and mining pool management into your AI workflows. This server provides a dual-purpose interface for both public blockchain data and private mining operations.

### What you can do

- **Blockchain Explorer** — Query specific blocks, transactions, and unconfirmed mempool data using hashes or heights.
- **Address Analysis** — Fetch balances, UTXOs, and complete transaction history for any Bitcoin address.
- **Mining Pool Stats** — Monitor your account hashrate (15m, 24h), rejection rates, and historical performance.
- **Worker Management** — List all mining workers and inspect individual statistics to identify active, inactive, or dead units.
- **Financial Tracking** — Retrieve payment history and account-level statistics directly through your agent.

### How it works

1. Subscribe to this server
2. (Optional) Enter your BTC.com Access Key to enable Pool API features
3. Start querying Bitcoin data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Developers** — Verify transaction inputs/outputs and debug address balances without leaving the code editor.
- **Mining Operators** — Monitor farm health and hashrate stability through natural language queries.
- **Data Analysts** — Extract real-time blockchain metrics and block metadata for research and reporting.


## Available Tools (13)
- **get_address_transactions**: Get address transactions
- **get_address_utxo**: Get unspent transaction outputs (UTXO) for an address
- **get_block**: Get block information by hash or height
- **get_block_transactions**: Get transactions for a specific block
- **get_hashrate_history**: Requires BTC_COM_ACCESS_KEY.

Get hashrate history
- **get_latest_block**: Get the latest block information
- **get_payment_history**: Requires BTC_COM_ACCESS_KEY.

Get payment history
- **get_transaction**: Get transaction details
- **get_unconfirmed_transactions**: Get unconfirmed transactions
- **get_worker_list**: Requires BTC_COM_ACCESS_KEY.

Get worker list
- **get_worker_stats**: Requires BTC_COM_ACCESS_KEY.

Get worker stats
- **get_account_stats**: Requires BTC_COM_ACCESS_KEY.

Get account hashrate and stats
- **get_address_summary**: Get address summary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BTC.com API (BTC.com Explorer & Pool API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest block information from the Bitcoin network."

**🤖 AI Agent:**
> I've retrieved the latest block. Height: 834291, Hash: 0000000000000000000... It contains 3,421 transactions and was mined at...

---

**👤 You:**
> "Show me the balance and summary for Bitcoin address 1A1zP1eP5QGefi2DMPTfTL5SLmv7DivfNa."

**🤖 AI Agent:**
> Using `get_address_summary`, I found that this address has a total balance of 99.98 BTC with 1,204 transactions recorded.

---

**👤 You:**
> "List all my active mining workers and their current hashrate."

**🤖 AI Agent:**
> I've fetched your worker list. You have 12 active workers. Worker 'Antminer_S19_01' is currently hashing at 104 TH/s.


## ❓ FAQ

**Q: Can I check the balance of a specific Bitcoin address without an API key?**
Yes. Explorer tools like `get_address_summary` and `get_address_transactions` are public and do not require a BTC_COM_ACCESS_KEY.

**Q: How do I monitor the status of my mining workers?**
You can use `get_worker_list` to see all workers and their status (Active/Inactive/Dead), or `get_worker_stats` with a specific Worker ID for detailed metrics.

**Q: Does this server support unconfirmed transactions?**
Yes, the `get_unconfirmed_transactions` tool allows you to fetch a list of transactions currently in the Bitcoin mempool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/btccom-api-btccom-explorer-pool-api](https://vinkius.com/mcp/btccom-api-btccom-explorer-pool-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BTC.com API (BTC.com Explorer & Pool API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `btccom-api-btccom-explorer-pool-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BTC.com API (BTC.com Explorer & Pool API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "btccom-api-btccom-explorer-pool-api": {
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
