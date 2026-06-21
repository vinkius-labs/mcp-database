# Etherscan MCP Server

Query Ethereum and EVM-compatible blockchain data—check balances, transaction history, and token transfers directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/etherscan)

## Overview
**Category:** data-analytics
**Tools Count:** 19

## Description
Connect your **Etherscan** API key to any AI agent and gain instant access to on-chain data across Ethereum and other EVM-compatible networks through natural conversation.

### What you can do

- **Native Balances** — Retrieve the native token balance (ETH, MATIC, etc.) for single or multiple addresses (up to 20) using `get_balance` and `get_balance_multi`.
- **Transaction History** — Fetch comprehensive lists of normal and internal transactions for any wallet address with `get_tx_list` and `get_tx_list_internal`.
- **Token Tracking** — Monitor transfers for ERC-20, ERC-721 (NFTs), and ERC-1155 tokens using specialized tools like `get_token_tx` and `get_token_nft_tx`.
- **Multi-Chain Support** — Query data across different networks by specifying the `chainid` (e.g., 1 for Ethereum, 137 for Polygon).
- **Granular Filtering** — Filter transaction results by block range, pagination, and sort order to find exactly what you need.

### How it works

1. Subscribe to this server
2. Enter your Etherscan API Key
3. Start auditing wallets and tracking transfers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug smart contract interactions and verify transaction statuses directly from your IDE.
- **Crypto Analysts** — Track whale movements, token distributions, and wallet activity without manual block explorer searches.
- **DeFi Users** — Monitor your portfolio balances and transaction history through a simple chat interface.


## Available Tools
- **get_address_token_balance**: Get address portfolio (PRO)
- **get_balance_multi**: Get native token balances for multiple addresses
- **get_balance**: Get native token balance for an address
- **get_abi**: Get Contract ABI
- **get_address_tag**: Get address name tag (PRO Plus)
- **get_block_no_by_time**: Get block number by timestamp
- **get_block_number**: Get latest block number
- **get_eth_price**: Get Ether last price
- **get_eth_supply**: Get total supply of Ether
- **get_gas_oracle**: Get Gas Oracle
- **get_logs**: Get event logs
- **get_source_code**: Get Contract Source Code
- **get_transaction_by_hash**: Get transaction by hash
- **get_token_1155_tx**: Get ERC-1155 token transfers for an address
- **get_token_nft_tx**: Get ERC-721 token transfers for an address
- **get_token_tx**: Get ERC-20 token transfers for an address
- **get_tx_list_internal**: Get internal transactions for an address
- **get_tx_list**: Max 10,000 records.

Get normal transactions for an address
- **verify_source_code**: Verify Contract Source Code


## Installation & Usage

To install and use the **Etherscan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/etherscan](https://vinkius.com/mcp/etherscan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
