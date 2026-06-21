# Scrollscan MCP Server

Explore the Scroll L2 blockchain — check account balances, track transactions (normal, internal, ERC20/721/1155), and inspect contract ABIs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/scrollscan)

## Overview
**Category:** developer-tools
**Tools Count:** 33

## Description
Connect to **Scrollscan** and bring real-time Scroll L2 blockchain data into your AI-powered workflows. Whether you are debugging smart contracts or monitoring wallet activity, this server provides the essential tools for on-chain analysis.

### What you can do

- **Account Balances** — Fetch Ether balances for single or multiple addresses simultaneously
- **Transaction History** — Retrieve comprehensive lists of normal and internal transactions with block range filtering
- **Token Tracking** — Monitor transfer events for ERC20, ERC721 (NFTs), and ERC1155 tokens for any address
- **Contract Inspection** — Access verified contract ABIs to understand and interact with smart contracts
- **Network Insights** — List blocks mined by specific addresses and query internal transactions by hash

### How it works

1. Subscribe to this server
2. Enter your Scrollscan API Key
3. Start querying Scroll L2 data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug transaction flows and fetch contract ABIs directly from your code editor
- **Data Analysts** — aggregate on-chain activity and token movements without manual exports
- **Crypto Enthusiasts** — monitor portfolio balances and NFT transfers through natural conversation


## Available Tools
- **check_verify_status**: Check Source Code Verification Status
- **get_account_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_account_balance**: Get Ether Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_contract_source_code**: Get Contract Source Code for Verified Source Codes
- **get_erc1155_token_tx**: Get ERC1155 Token Transfer Events by Address
- **get_erc20_token_tx**: Get ERC20 Token Transfer Events by Address
- **get_erc721_token_tx**: Get ERC721 Token Transfer Events by Address
- **get_eth_price**: Get Ether Last Price
- **get_eth_supply**: Get Total Supply of Ether on Scroll
- **get_internal_tx_list_by_block_range**: Get Internal Transactions by Block Range
- **get_internal_tx_list_by_hash**: Get Internal Transactions by Transaction Hash
- **get_internal_tx_list**: Get Internal Transactions by Address
- **get_logs**: Get Logs
- **get_mined_blocks**: Get List of Blocks Mined by Address
- **get_normal_tx_list**: Get Normal Transactions By Address
- **get_token_balance**: Get ERC20-Token Balance for Address by ContractAddress
- **get_token_supply**: Get ERC20-Token TotalSupply by ContractAddress
- **get_tx_receipt_status**: Check Check Transaction Receipt Status
- **get_tx_status**: Check Transaction Receipt Status
- **proxy_block_number**: eth_blockNumber
- **proxy_call**: eth_call
- **proxy_estimate_gas**: eth_estimateGas
- **proxy_gas_price**: eth_gasPrice
- **proxy_get_block_by_number**: eth_getBlockByNumber
- **proxy_get_code**: eth_getCode
- **proxy_get_storage_at**: eth_getStorageAt
- **proxy_get_transaction_by_hash**: eth_getTransactionByHash
- **proxy_get_transaction_receipt**: eth_getTransactionReceipt
- **verify_source_code**: Verify Source Code


## Installation & Usage

To install and use the **Scrollscan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scrollscan](https://vinkius.com/mcp/scrollscan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
