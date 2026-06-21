# OKLink (Multi-chain Web3 Blockchain Data API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oklink-multi-chain-web3-blockchain-data-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/oklink-multi-chain-web3-blockchain-data-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/oklink-multi-chain-web3-blockchain-data-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access real-time blockchain data across multiple chains—query addresses, tokens, transactions, and blocks directly from your AI agent.

## Description
Connect to **OKLink**, the leading multi-chain data provider, to empower your AI with deep blockchain insights. This server allows you to navigate the decentralized web across dozens of supported networks including Bitcoin, Ethereum, BSC, and more.

### What you can do

- **Multi-chain Support** — List all supported networks and get specific chain metadata using `get_supported_chains` and `get_chain_info`.
- **Address Intelligence** — Retrieve summaries, balances, and full transaction histories for any wallet or contract with `get_address_summary` and `get_address_transactions`.
- **Token & NFT Insights** — Fetch ERC20 token lists, detailed token metrics, and NFT collection data using `get_token_list` and `get_nft_collection_info`.
- **Block & Transaction Data** — Inspect specific transaction hashes, block details, or the latest network activity with `get_transaction_detail` and `get_latest_block`.

### How it works

1. Subscribe to this server
2. Enter your OKLink API Key (Access Key)
3. Start querying on-chain data from Claude, Cursor, or any MCP-compatible client

No more manually searching through multiple block explorers. Your AI acts as a dedicated blockchain analyst, providing instant data for developers, traders, and researchers.


## Available Tools
- **get_address_summary**: Get summary information for a specific address
- **get_address_transactions**: Get a list of transactions for a specific address
- **get_block_detail**: Get detailed information about a specific block
- **get_block_transactions**: Get a list of transactions within a specific block
- **get_chain_info**: Get detailed information about a specific blockchain
- **get_latest_block**: Get the latest block information for a chain
- **get_nft_collection_info**: Get information about a specific NFT collection
- **get_supported_chains**: Get a summary of all supported blockchains
- **get_token_balance**: Get token balances for a specific address
- **get_token_detail**: Get detailed information about a specific token
- **get_token_list**: ) on a given blockchain.

Get a list of tokens on a specific chain
- **get_transaction_detail**: Get detailed information about a specific transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OKLink (Multi-chain Web3 Blockchain Data API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the balance and transaction summary for address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e on Ethereum."

**🤖 AI Agent:**
> I've retrieved the summary for that Ethereum address. It currently holds 12.5 ETH with a total of 150 transactions. Would you like to see the latest transaction history or specific token balances?

---

**👤 You:**
> "What is the latest block height on the Polygon network?"

**🤖 AI Agent:**
> The latest block on Polygon (MATIC) is at height 64,231,890. It was mined a few seconds ago. Do you want to inspect the transactions included in this block?

---

**👤 You:**
> "Get the details for transaction 0x5c504ed432cb51138bcf09aa5e8a410dd4a1e204ef84bfed1be16dfba1b22026 on Ethereum."

**🤖 AI Agent:**
> Analyzing transaction... This was a transfer of 500 USDC from 0x... to 0x... confirmed in block 18,402,100. The status is 'Success' and the gas fee was 0.002 ETH.


## Installation & Usage

To install and use the **OKLink (Multi-chain Web3 Blockchain Data API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oklink-multi-chain-web3-blockchain-data-api](https://vinkius.com/mcp/oklink-multi-chain-web3-blockchain-data-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
