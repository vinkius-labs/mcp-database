# Cronoscan (Cronos Block Explorer) MCP Server

Access Cronos blockchain data — check CRO balances, track transactions, inspect smart contracts, and monitor token transfers directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cronoscan-cronos-block-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 24

## Description
Connect to **Cronoscan** to analyze the Cronos blockchain through natural conversation. This server provides a comprehensive suite of tools for developers, traders, and analysts to interact with Cronos network data without leaving their AI interface.

### What you can do

- **Account Analysis** — Check CRO balances for single or multiple addresses and retrieve detailed transaction histories (normal and internal).
- **Token Tracking** — Monitor ERC-20 and ERC-721 (NFT) transfer events, check specific token balances, and track total supply metrics.
- **Smart Contract Insights** — Fetch contract ABIs and verified source code for deep technical inspection and security auditing.
- **Network Monitoring** — Get real-time data on gas prices, block rewards, and the current market price of CRO.
- **Geth Proxy Support** — Execute standard Ethereum-compatible RPC calls like `eth_call`, `eth_getTransactionReceipt`, and `eth_estimateGas` for advanced interactions.

### How it works

1. Subscribe to this server
2. Enter your Cronoscan API Key
3. Start querying Cronos blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug transactions and inspect contract source code directly from your coding environment.
- **Crypto Analysts** — Track whale movements, monitor token distributions, and generate on-chain reports via chat.
- **DeFi Users** — Check your portfolio balances and transaction status across the Cronos ecosystem instantly.


## Available Tools
- **get_balance_multi**: Get CRO Balance for Multiple Addresses
- **get_balance**: Get CRO Balance for a Single Address
- **get_eth_price**: Get CRO Last Price
- **get_eth_supply**: Get Total Supply of CRO on Cronos
- **get_abi**: Get Contract ABI for Verified Source Codes
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_logs**: Get Logs
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_eth_block_number**: Proxy: eth_blockNumber
- **proxy_eth_call**: Proxy: eth_call
- **proxy_eth_estimate_gas**: Proxy: eth_estimateGas
- **proxy_eth_gas_price**: Proxy: eth_gasPrice
- **proxy_eth_get_block_by_number**: Proxy: eth_getBlockByNumber
- **proxy_eth_get_code**: Proxy: eth_getCode
- **proxy_eth_get_storage_at**: Proxy: eth_getStorageAt
- **proxy_eth_get_transaction_by_hash**: Proxy: eth_getTransactionByHash
- **proxy_eth_get_transaction_receipt**: Proxy: eth_getTransactionReceipt
- **get_token_balance**: Get ERC20-Token Account Balance by ContractAddress
- **get_token_nft_tx**: Get ERC721 Token Transfer Events by Address
- **get_token_supply**: Get ERC20-Token Total Supply by ContractAddress
- **get_token_tx**: Get ERC20 Token Transfer Events by Address
- **get_tx_list_internal**: Get a List of Internal Transactions By Address
- **get_tx_list**: Get a List of Normal Transactions By Address


## Installation & Usage

To install and use the **Cronoscan (Cronos Block Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cronoscan-cronos-block-explorer](https://vinkius.com/mcp/cronoscan-cronos-block-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
