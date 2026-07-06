# Arweave MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arweave)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Interact with the Arweave permaweb — query network info, check wallet balances, inspect transactions, and calculate storage costs directly from your AI agent.

## Description
Connect to the **Arweave** network and manage permanent data storage through natural conversation. This MCP server allows your AI agent to query the blockweave, check transaction statuses, and interact with the permaweb ecosystem.

### What you can do

- **Network Monitoring** — Get real-time network status, height, and peer information using `get_network_info` and `get_peers`.
- **Transaction Inspection** — Retrieve transaction metadata, status, and raw data using unique IDs with `get_transaction` and `get_transaction_data`.
- **Wallet Management** — Check balances in Winstons and find the last transaction for any wallet address via `get_wallet_balance`.
- **Storage Economics** — Calculate the exact cost to store data on the permaweb with `get_storage_price`.
- **Advanced Querying** — Use `query_graphql` to search for specific data and tags across the entire network.

### How it works

1. Subscribe to this server
2. (Optional) Provide a custom Arweave Gateway URL
3. Start querying the permaweb from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly check transaction confirmations and network status without leaving the terminal or IDE.
- **Data Analysts** — query the permaweb using GraphQL to extract insights from permanent data.
- **Crypto Users** — monitor wallet balances and storage costs for permanent file uploads.


## Available Tools (13)
- **get_block_by_height**: Retrieve a block by its height
- **get_storage_price**: Get the cost in Winstons to store data
- **get_transaction_data**: Retrieve the data associated with a transaction
- **get_transaction_offset**: Get the byte offset and size of the transaction data
- **get_transaction_status**: g., pending, confirmed).

Get the status of a transaction
- **get_transaction**: Retrieve a transaction by its ID
- **get_wallet_balance**: Get the balance of a wallet address in Winstons
- **get_wallet_last_tx**: Get the ID of the last transaction sent by the wallet
- **get_network_info**: Get current Arweave network status
- **get_peers**: Get a list of peer addresses known to the node
- **query_graphql**: Execute a GraphQL query against the Arweave network
- **submit_transaction**: Submit a new transaction to the network
- **get_block_by_hash**: Retrieve a block by its hash


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arweave** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status and height of the Arweave network?"

**🤖 AI Agent:**
> I've retrieved the network info. The Arweave network is currently at height 1,542,890 with the current block hash starting with 'zX9...'. The node version is 2.7.2.

---

**👤 You:**
> "Check the balance for Arweave wallet address 3pD7...x9A."

**🤖 AI Agent:**
> The balance for wallet 3pD7...x9A is 1,250,000,000 Winstons, which is equivalent to 0.00125 AR.

---

**👤 You:**
> "How much does it cost to store 500MB on Arweave right now?"

**🤖 AI Agent:**
> Calculating storage price for 524,288,000 bytes... The current cost is approximately 45,200,000 Winstons (0.0000452 AR).


## ❓ FAQ

**Q: How do I check the cost to store a specific amount of data?**
You can use the `get_storage_price` tool. Just provide the number of bytes you intend to store, and the agent will return the price in Winstons (where 1 AR = 10^12 Winstons).

**Q: Can I retrieve the actual content of a transaction?**
Yes. Use the `get_transaction_data` tool with the specific Transaction ID (txid). The agent will fetch the data associated with that transaction from the blockweave.

**Q: How do I know if a transaction has been confirmed by the network?**
Use the `get_transaction_status` tool. It will return the current status of the transaction, including whether it is pending or confirmed, and the number of confirmations if available.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arweave](https://vinkius.com/mcp/arweave)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arweave** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arweave` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arweave** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arweave": {
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
