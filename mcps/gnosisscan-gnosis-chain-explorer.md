# Gnosisscan (Gnosis Chain Explorer) MCP Server

Access Gnosis Chain data directly—query account balances, transaction history, and smart contract details via Gnosisscan.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gnosisscan-gnosis-chain-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 26

## Description
Connect your AI agent to the **Gnosis Chain** through the Gnosisscan API. This server allows you to inspect the blockchain, track xDAI balances, and analyze transaction flows without leaving your chat interface.

### What you can do

- **Account Auditing** — Retrieve xDAI balances for single or multiple addresses instantly.
- **Transaction History** — List normal and internal transactions, including paginated results and block ranges.
- **Token Tracking** — Monitor ERC20 and ERC721 (NFT) transfer events for any specific address or contract.
- **Smart Contract Insights** — Fetch verified Contract ABIs and Source Code for deep technical analysis.
- **Network Stats** — Get real-time data on block rewards, gas prices, and GNO price metrics.

### How it works

1. Subscribe to this server
2. Enter your Gnosisscan API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly fetch ABIs or check transaction receipts without switching to a browser.
- **Data Analysts** — aggregate balance data and token movements across multiple Gnosis Chain addresses.
- **DeFi Users** — track personal portfolio movements and internal contract interactions through natural language.


## Available Tools
- **get_account_balance_multi**: Get xDAI Balance for Multiple Addresses
- **get_account_balance**: Get xDAI Balance for a Single Address
- **get_account_minedblocks**: Get a List of Blocks Validated by Address
- **get_account_tokennfttx**: Get a List of ERC721 Token Transfer Events by Address
- **get_account_tokentx**: Get a List of ERC20 Token Transfer Events by Address
- **get_account_txlist_internal**: Get a List of Internal Transactions by Address
- **get_account_txlist**: Get a List of Normal Transactions By Address
- **get_block_bytime**: Get Block Number by Timestamp
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_contract_sourcecode**: Get Contract Source Code for Verified Source Codes
- **get_logs**: Get Event Logs
- **get_stats_ethsupply**: Get Total Supply of xDAI on Gnosis Chain
- **get_stats_gnoprice**: Get Last Price of Gnosis (GNO) and xDAI
- **get_tx_receiptstatus**: Check Transaction Receipt Status
- **get_tx_status**: Check Contract Execution Status
- **proxy_blocknumber**: eth_blockNumber Proxy
- **proxy_call**: eth_call Proxy
- **proxy_estimategas**: eth_estimateGas Proxy
- **proxy_gasprice**: eth_gasPrice Proxy
- **proxy_getblockbynumber**: eth_getBlockByNumber Proxy
- **proxy_getcode**: eth_getCode Proxy
- **proxy_getstorageat**: eth_getStorageAt Proxy
- **proxy_gettransactionbyhash**: eth_getTransactionByHash Proxy
- **proxy_gettransactionreceipt**: eth_getTransactionReceipt Proxy


## Installation & Usage

To install and use the **Gnosisscan (Gnosis Chain Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gnosisscan-gnosis-chain-explorer](https://vinkius.com/mcp/gnosisscan-gnosis-chain-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
