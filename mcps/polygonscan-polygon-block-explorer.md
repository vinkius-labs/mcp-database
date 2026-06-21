# Polygonscan (Polygon Block Explorer) MCP Server

Query the Polygon blockchain directly — check MATIC balances, track transactions, and inspect smart contracts via any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/polygonscan-polygon-block-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 17

## Description
Connect **Polygonscan** to your AI agent to gain real-time visibility into the Polygon (MATIC) network. This server allows you to fetch on-chain data using natural language, making blockchain analysis accessible without leaving your workspace.

### What you can do

- **Account Balances** — Retrieve MATIC balances for single or multiple addresses instantly.
- **Transaction History** — List normal and internal transactions for any wallet to audit activity.
- **Token Tracking** — Monitor ERC-20, ERC-721 (NFT), and ERC-1155 transfer events across the network.
- **Contract Inspection** — Fetch verified smart contract ABIs and source code for technical analysis.
- **Network Stats** — Get real-time MATIC price, supply data, and block rewards.

### How it works

1. Subscribe to this server
2. Enter your Polygonscan API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Quickly pull contract ABIs and transaction logs directly into your coding environment.
- **Crypto Analysts** — Audit wallet movements and token distributions using simple conversational prompts.
- **DeFi Users** — Check your balances and transaction statuses without opening a separate browser tab.


## Available Tools
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_balance_multi**: Get MATIC Balance for Multiple Addresses
- **get_balance**: Get MATIC Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_no_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_logs**: Get Logs
- **get_matic_price**: Get MATIC Last Price
- **get_matic_supply**: Get Total Supply of MATIC on Polygon
- **get_contract_source_code**: Get Contract Source Code for Verified Source Codes
- **get_token_1155_tx**: Get List of ERC-1155 Transfer Events
- **get_token_nft_tx**: Get List of ERC-721 (NFT) Transfer Events
- **get_token_tx**: Get List of ERC-20 Token Transfer Events
- **get_tx_list_internal**: Get List of Internal Transactions
- **get_tx_list**: Get List of Normal Transactions
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **get_tx_status**: Check Contract Execution Status


## Installation & Usage

To install and use the **Polygonscan (Polygon Block Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polygonscan-polygon-block-explorer](https://vinkius.com/mcp/polygonscan-polygon-block-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
