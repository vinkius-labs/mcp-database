# Arbiscan (Arbitrum Explorer) MCP Server

Explore Arbitrum blockchain data — check balances, track transactions, and inspect smart contract source code directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arbiscan-arbitrum-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 16

## Description
Connect your AI agent to **Arbiscan** to query the Arbitrum L2 network in real-time. This MCP server allows you to fetch blockchain data without leaving your chat interface or IDE.

### What you can do

- **Account Auditing** — Check Ether balances for single or multiple addresses simultaneously.
- **Transaction Tracking** — Retrieve full history for normal, internal, ERC20, and ERC721 (NFT) transactions.
- **Contract Intelligence** — Fetch verified source code and ABIs to understand how dApps operate.
- **Network Insights** — Get real-time ETH price on Arbitrum, total supply, and block rewards.
- **Developer Tools** — Submit and verify contract source code directly through the API.

### How it works

1. Subscribe to this server
2. Enter your Arbiscan API Key
3. Start querying Arbitrum data from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Inspect contract ABIs and source code while writing code in your IDE.
- **Crypto Analysts** — Track whale movements and token transfers using natural language.
- **Security Researchers** — Quickly audit transaction history and internal calls for suspicious activity.


## Available Tools
- **get_abi**: Get Contract ABI for Verified Source Codes
- **get_balance_multi**: Get Ether Balance for Multiple Addresses
- **get_balance**: Get Ether Balance for a Single Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_eth_price**: Get Ether Last Price
- **get_eth_supply**: Get Total Supply of Ether on Arbitrum
- **get_logs**: Get Event Logs
- **get_source_code**: Get Contract Source Code for Verified Source Codes
- **get_status**: Check Contract Execution Status
- **get_token_nft_tx**: Get List of ERC721 Token Transfer Events By Address
- **get_token_tx**: Get List of ERC20 Token Transfer Events By Address
- **get_tx_list_internal**: Get List of Internal Transactions By Address
- **get_tx_list**: Get List of Normal Transactions By Address
- **get_tx_receipt_status**: Check Transaction Receipt Status
- **verify_source_code**: Verify Source Code


## Installation & Usage

To install and use the **Arbiscan (Arbitrum Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arbiscan-arbitrum-explorer](https://vinkius.com/mcp/arbiscan-arbitrum-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
