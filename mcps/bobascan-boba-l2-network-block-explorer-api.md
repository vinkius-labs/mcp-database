# Bobascan (Boba L2 Network Block Explorer API) MCP Server

Access Boba L2 Network blockchain data — query balances, transaction histories, and smart contract ABIs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bobascan-boba-l2-network-block-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 25

## Description
Connect to the **Boba Network** (L2) through Bobascan's API. This MCP server allows your AI to act as a blockchain analyst, retrieving real-time data from the Boba L2 explorer.

### What you can do

- **Account Analysis** — Fetch Ether balances for single or multiple addresses on the Boba L2 network.
- **Transaction History** — List normal, internal, and token (ERC20/ERC721) transfer events for any wallet address.
- **Smart Contract Inspection** — Retrieve verified source code and ABIs to understand contract logic and interact with dApps.
- **Network Stats** — Get current gas prices, block rewards, and ETH price data directly from the chain.
- **Proxy Actions** — Perform low-level JSON-RPC calls like getting block numbers or transaction receipts.

### How it works

1. Subscribe to this server
2. Enter your Bobascan API Key
3. Start querying the Boba L2 network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly inspect contract ABIs and source code without leaving the IDE.
- **Data Analysts** — automate the retrieval of transaction lists and token transfers for reporting.
- **DeFi Users** — check wallet balances and transaction statuses through natural language.


## Available Tools
- **get_abi**: Get Contract ABI for Verified Source Codes
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_execution_status**: Check Contract Execution Status
- **get_eth_price**: Get Ether Last Price
- **get_eth_supply**: Get Total Supply of Ether on Boba Network
- **get_ether_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_ether_balance**: Get Ether Balance for a Single Address
- **get_logs**: Get Logs
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_token_balance**: Get ERC20-Token Balance for Address by ContractAddress
- **get_token_nft_tx**: Get a List of ERC721 Token Transfer Events By Address
- **get_token_supply**: Get ERC20-Token Total Supply by ContractAddress
- **get_token_tx**: Get a List of ERC20 Token Transfer Events By Address
- **get_tx_list_internal**: Get a List of Internal Transactions By Address
- **get_tx_list**: Get a List of Normal Transactions By Address
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **proxy_block_number**: eth_blockNumber
- **proxy_call**: eth_call
- **proxy_estimate_gas**: eth_estimateGas
- **proxy_gas_price**: eth_gasPrice
- **proxy_get_block_by_number**: eth_getBlockByNumber
- **proxy_get_code**: eth_getCode
- **proxy_get_transaction_by_hash**: eth_getTransactionByHash
- **proxy_get_transaction_receipt**: eth_getTransactionReceipt


## Installation & Usage

To install and use the **Bobascan (Boba L2 Network Block Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bobascan-boba-l2-network-block-explorer-api](https://vinkius.com/mcp/bobascan-boba-l2-network-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
