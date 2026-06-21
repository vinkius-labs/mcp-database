# CardanoScan (Cardano Block Explorer API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cardanoscan-cardano-block-explorer-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access real-time Cardano blockchain data — query addresses, transactions, blocks, and stake pools directly from your AI agent.

## Description
Connect your AI agent to the **CardanoScan API** to explore the Cardano blockchain with natural language. This server provides comprehensive access to on-chain data, from simple address balances to complex transaction UTXOs and network-wide epoch metrics.

### What you can do

- **Address Insights** — Retrieve detailed information for any Cardano address, including ADA balances and transaction history.
- **Transaction Deep-Dives** — Inspect specific transaction hashes and analyze their inputs and outputs (UTXOs) for precise tracking.
- **Network Monitoring** — Stay updated with the latest blocks, block heights, and current epoch details in real-time.
- **Stake Pool Exploration** — List all registered stake pools or fetch specific metadata for a target pool ID.
- **Native Asset Tracking** — Query information about native assets and monitor their transaction activity across the network.

### How it works

1. Subscribe to this server
2. Enter your CardanoScan API Key
3. Start exploring the Cardano ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Blockchain Developers** — Quickly verify transaction statuses and UTXO data without leaving the code editor.
- **Crypto Analysts** — Monitor network health, epoch transitions, and large address movements through conversation.
- **Stake Pool Delegators** — Check pool performance and metadata to make informed staking decisions.


## Available Tools (12)
- **get_address**: Get detailed information about a specific Cardano address
- **get_asset**: Get information about a specific native asset
- **get_block**: Get information about a specific block by its hash or number
- **get_epoch**: Get information about a specific epoch
- **get_latest_blocks**: Get a list of the most recent blocks added to the blockchain
- **get_latest_epoch**: Get details about the current/latest epoch
- **get_pool**: Get information about a specific stake pool
- **get_transaction**: Get comprehensive details for a specific transaction hash
- **get_transaction_utxos**: Get the inputs and outputs (UTXOs) for a specific transaction
- **list_address_transactions**: Get a list of transactions associated with a specific address
- **list_asset_transactions**: Get transactions involving a specific native asset
- **list_pools**: Get a paginated list of all registered stake pools


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CardanoScan (Cardano Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the balance and transaction count for address addr1q8..."

**🤖 AI Agent:**
> I've retrieved the details for that address. It currently holds 1,250 ADA and has been involved in 42 transactions. Would you like to see the most recent transactions?

---

**👤 You:**
> "Show me the latest blocks added to the Cardano blockchain."

**🤖 AI Agent:**
> Fetching the latest blocks... I found the most recent entries, including block height 10,452,120 produced by pool 'TICKER'. Each block contains detailed timestamps and transaction counts.

---

**👤 You:**
> "List the registered stake pools on Cardano."

**🤖 AI Agent:**
> I've compiled a list of registered stake pools. Notable pools currently active include 'IOG1', 'POOL2', and 'ADA3'. Would you like the specific metadata for any of these?


## ❓ FAQ

**Q: Can I see the specific inputs and outputs of a transaction hash?**
Yes. Use the `get_transaction_utxos` tool with the transaction hash. It will return the detailed list of all UTXO inputs and outputs associated with that specific record.

**Q: How do I check the current progress of the Cardano network epoch?**
You can use the `get_latest_epoch` tool to retrieve details about the current epoch, or `get_epoch` for a specific epoch number to see its timing and block count.

**Q: Is it possible to find information about a specific native asset or token?**
Absolutely. Use the `get_asset` tool with the Asset ID (Policy ID + Asset Name) to fetch its metadata, supply, and other on-chain characteristics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cardanoscan-cardano-block-explorer-api](https://vinkius.com/mcp/cardanoscan-cardano-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CardanoScan (Cardano Block Explorer API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cardanoscan-cardano-block-explorer-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CardanoScan (Cardano Block Explorer API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cardanoscan-cardano-block-explorer-api": {
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
