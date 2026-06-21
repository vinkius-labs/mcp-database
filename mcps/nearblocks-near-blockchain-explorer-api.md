# Nearblocks (Near Blockchain Explorer API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nearblocks-near-blockchain-explorer-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nearblocks-near-blockchain-explorer-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nearblocks-near-blockchain-explorer-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Near blockchain — query account balances, transactions, tokens, and network statistics directly via AI.

## Description
Connect to the **Nearblocks API** to inspect the Near Protocol blockchain. This MCP server allows any AI agent to fetch real-time data about accounts, transactions, blocks, and tokens without leaving the chat interface.

### What you can do

- **Account Insights** — Retrieve balances, transaction history, and token holdings (FTs and NFTs) for any Near account.
- **Blockchain Monitoring** — Fetch the latest blocks and transactions to stay updated on network activity.
- **Token Analysis** — List all tokens on the network or get deep details for specific token contracts.
- **Network Health** — Monitor global network statistics including TPS, gas prices, and current block height.

### How it works

1. Subscribe to this server
2. Enter your Nearblocks API Key (optional but recommended for higher limits)
3. Start querying the Near blockchain from your favorite MCP client.

### Who is this for?

- **Web3 Developers** — Debug transactions and verify contract states directly from your IDE.
- **Crypto Analysts** — Track whale movements and monitor network performance in real-time.
- **DeFi Users** — Check your portfolio and transaction history through natural conversation.


## Available Tools
- **get_account_details**: Get basic information about a specific Near account
- **get_account_inventory**: Get NFTs owned by a Near account
- **get_account_tokens**: Get tokens owned by a Near account
- **get_account_transactions**: Get a list of transactions for a Near account
- **get_block_details**: Get details of a specific block
- **get_latest_blocks**: Get a list of the most recent blocks
- **get_network_stats**: Get general network statistics
- **get_recent_transactions**: Get a list of the most recent transactions
- **get_token_details**: Get details of a specific token contract
- **get_token_list**: Get a list of tokens on the network
- **get_transaction_details**: Get details of a specific transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nearblocks (Near Blockchain Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest blocks from the Near blockchain."

**🤖 AI Agent:**
> I've retrieved the most recent blocks. The latest block is at height 115,234,001 with hash '9aB...'. Would you like to see the details of a specific block?

---

**👤 You:**
> "Show me the transaction history for account 'vinkius.near'."

**🤖 AI Agent:**
> I found 10 recent transactions for 'vinkius.near'. The most recent was a 'FunctionCall' to 'app.near' 5 minutes ago. Should I fetch the full details for that specific transaction?

---

**👤 You:**
> "What are the details for transaction hash 8nZ...?"

**🤖 AI Agent:**
> Transaction 8nZ... was successful. It involved a transfer of 5 NEAR from 'sender.near' to 'receiver.near' at block 115,233,980. Gas used: 2.4 Tgas.


## Installation & Usage

To install and use the **Nearblocks (Near Blockchain Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nearblocks-near-blockchain-explorer-api](https://vinkius.com/mcp/nearblocks-near-blockchain-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
