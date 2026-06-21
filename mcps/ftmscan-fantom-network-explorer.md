# FtmScan (Fantom Network Explorer) MCP Server

Access Fantom blockchain data directly—query wallet balances, transaction history, smart contract source code, and token transfers via FtmScan.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ftmscan-fantom-network-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 19

## Description
Connect to the **Fantom Network** through FtmScan to inspect on-chain activity using natural language. This server allows your AI agent to act as a blockchain explorer, providing real-time data on accounts, transactions, and smart contracts.

### What you can do

- **Account Analytics** — Retrieve FTM balances for single or multiple addresses and track transaction history (normal and internal).
- **Token Tracking** — Monitor ERC-20 and ERC-721 (NFT) transfer events across the network.
- **Smart Contract Inspection** — Fetch verified source code and ABIs for any deployed contract to understand its logic.
- **Transaction Status** — Check the execution status and receipts of specific transaction hashes.
- **Network Data** — Get the current FTM price, total supply, and block rewards.

### How it works

1. Subscribe to this server
2. Enter your FtmScan API Key
3. Start querying the Fantom blockchain from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — quickly verify contract code and transaction statuses without leaving the IDE.
- **Crypto Analysts** — track whale movements and token distributions through simple conversation.
- **DeFi Users** — check wallet balances and recent activity across the Fantom ecosystem.


## Available Tools
- **get_block_countdown**: Get Estimated Block Countdown Time
- **get_block_reward**: Get Block Rewards
- **get_contract_abi**: Get Contract ABI
- **get_contract_source_code**: Get Contract Source Code
- **get_erc20_token_balance**: Get ERC20 Token Balance for Address
- **get_erc20_token_supply**: Get ERC20 Token Total Supply
- **get_erc20_transfers**: Get List of ERC20 Token Transfer Events
- **get_erc721_transfers**: Get List of ERC721 Token Transfer Events
- **get_eth_block_number**: Get Latest Block Number (Proxy)
- **get_eth_transaction_by_hash**: Get Transaction by Hash (Proxy)
- **get_ftm_balance_multi**: Get FTM Balance for Multiple Addresses
- **get_ftm_balance**: Get FTM Balance for a Single Address
- **get_ftm_last_price**: Get FTM Last Price
- **get_ftm_total_supply**: Get Total Supply of FTM
- **get_internal_transactions**: Get List of Internal Transactions
- **get_logs**: Get Event Logs
- **get_normal_transactions**: Get List of Normal Transactions
- **get_transaction_receipt_status**: Check Transaction Receipt Status
- **get_transaction_status**: Check Transaction Execution Status


## Installation & Usage

To install and use the **FtmScan (Fantom Network Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ftmscan-fantom-network-explorer](https://vinkius.com/mcp/ftmscan-fantom-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
