# Celoscan (Celo Network Explorer) MCP Server

Access Celo network data via Celoscan — check account balances, track transactions, and inspect smart contracts directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/celoscan-celo-network-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 18

## Description
Connect your **Celoscan** API key to any AI agent to explore the Celo blockchain with ease. Analyze addresses, verify contract code, and audit transaction history through natural language.

### What you can do

- **Account Insights** — Fetch CELO balances for single or multiple addresses instantly to monitor wallet holdings.
- **Transaction History** — Query normal and internal transactions, including ERC20 and ERC721 (NFT) transfer events for any address.
- **Smart Contract Auditing** — Retrieve verified contract ABIs and source code for deep technical inspection and debugging.
- **Network Monitoring** — Check blocks mined by specific addresses and verify the receipt status of any transaction hash.

### How it works

1. Subscribe to this server
2. Enter your Celoscan API Key
3. Start querying the Celo Network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly pull contract ABIs and source code into your IDE to understand protocol implementations.
- **Data Analysts** — export transaction histories and token movements for reporting and on-chain forensics.
- **Crypto Users** — monitor wallet balances and transaction statuses without leaving your chat interface.


## Available Tools
- **get_erc20_token_balance**: Get ERC20-Token Account Balance by ContractAddress
- **get_erc20_token_supply**: Get ERC20-Token Total Supply by ContractAddress
- **get_account_balance**: Get CELO Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_contract_abi**: Get Contract ABI for Verified Smart Contracts
- **get_contract_source_code**: Get Contract Source Code for Verified Smart Contracts
- **get_account_balance_multi**: Get CELO Balance for Multiple Addresses
- **get_erc20_transfers**: Get a List of ERC20 Token Transfer Events By Address
- **get_erc721_transfers**: Get a List of ERC721 Token Transfer Events By Address
- **get_internal_transactions**: Get a List of Internal Transactions By Address
- **get_last_celo_price**: Get Last Price of CELO
- **get_mined_blocks**: Get list of Blocks Mined by Address
- **get_normal_transactions**: Get a List of Normal Transactions By Address
- **get_total_celo_supply**: Get Total Supply of CELO on the Celo Network
- **get_transaction_execution_status**: Check Contract Execution Status
- **get_transaction_receipt_status**: Check Transaction Receipt Status


## Installation & Usage

To install and use the **Celoscan (Celo Network Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/celoscan-celo-network-explorer](https://vinkius.com/mcp/celoscan-celo-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
