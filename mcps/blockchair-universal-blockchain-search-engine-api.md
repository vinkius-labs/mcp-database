# Blockchair (Universal Blockchain Search Engine & API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockchair-universal-blockchain-search-engine-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/blockchair-universal-blockchain-search-engine-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/blockchair-universal-blockchain-search-engine-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Query blocks, transactions, and addresses across multiple blockchains like Bitcoin and Ethereum using Blockchair's universal API.

## Description
Connect to **Blockchair**, the most advanced universal blockchain search engine, and explore decentralized data across 20+ networks including Bitcoin, Ethereum, and Litecoin through natural conversation.

### What you can do

- **Multi-Chain Stats** — Get real-time network health, difficulty, and block height for any supported blockchain using `get_blockchain_stats`.
- **Deep Address Inspection** — Retrieve balances, transaction history, and UTXO sets for specific wallet addresses with `get_address`.
- **SQL-like Filtering** — Query blocks and transactions using advanced filters (e.g., filter by fee, time, or value) via `filter_transactions` and `filter_blocks`.
- **Token & Contract Data** — Check ERC-20 token balances and inspect internal Ethereum contract calls using specialized tools.
- **HD Wallet Support** — Analyze entire HD wallets using extended public keys (xpub) with the `get_xpub` tool.

### How it works

1. Subscribe to this server
2. Enter your Blockchair API Key
3. Start querying blockchain data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and verify contract states without leaving your IDE or code editor.
- **Data Analysts** — Extract specific blockchain datasets using powerful filtering tools for research or reporting.
- **Crypto Enthusiasts** — Track wallet balances and monitor network congestion through simple natural language prompts.


## Available Tools
- **filter_blocks**: Example q: time(2023-01-01..2023-01-02),transaction_count(100..)

Query blocks using SQL-like filters
- **filter_transactions**: Example q: fee(10000..), s: fee(desc)

Query transactions using SQL-like filters
- **get_address**: Retrieve balance, history, and UTXO set for an address
- **get_block**: Retrieve details about a specific block
- **get_contract_calls**: Get Ethereum contract internal transactions
- **get_erc20_token_address**: Get the balance of a specific ERC-20 token for an address
- **get_blockchain_stats**: for the specified blockchain.

Get general information about a blockchain
- **get_transaction**: Retrieve details about a specific transaction
- **get_xpub**: Retrieve data for an entire HD wallet (xpub)
- **push_transaction**: Broadcast a raw hex-encoded transaction to the network
- **validate_address**: Check if an address is valid for a specific chain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blockchair (Universal Blockchain Search Engine & API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current stats for the Bitcoin network."

**🤖 AI Agent:**
> I've retrieved the latest Bitcoin stats. The current block height is 834,291, with a difficulty of 79.35T. There have been over 980 million transactions recorded on the network to date.

---

**👤 You:**
> "What is the balance and transaction history for Ethereum address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e?"

**🤖 AI Agent:**
> The address currently holds 12.5 ETH. I found 45 transactions in its history. The most recent transaction was a transfer of 1.2 ETH on 2024-03-15. Would you like to see the details of the last 5 transactions?

---

**👤 You:**
> "Find Bitcoin transactions with a fee higher than 50,000 satoshis from the last 24 hours."

**🤖 AI Agent:**
> I've filtered the Bitcoin transactions. I found 12 transactions matching your criteria. The highest fee observed was 120,500 satoshis for transaction hash 4a5e... Would you like the full list of hashes?


## Installation & Usage

To install and use the **Blockchair (Universal Blockchain Search Engine & API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockchair-universal-blockchain-search-engine-api](https://vinkius.com/mcp/blockchair-universal-blockchain-search-engine-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
