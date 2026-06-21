# Snowtrace (Avalanche Explorer) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snowtrace-avalanche-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snowtrace-avalanche-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snowtrace-avalanche-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Explore the Avalanche C-Chain — check AVAX balances, track ERC-20/NFT transfers, and inspect smart contract data directly from your AI agent.

## Description
Connect to the **Snowtrace** explorer and bring real-time Avalanche blockchain data into your AI workflows. Monitor addresses, analyze transactions, and audit smart contracts without leaving your conversation.

### What you can do

- **Account Analytics** — Retrieve AVAX balances for single or multiple addresses (up to 20) in a single request.
- **Transaction History** — List normal and internal transactions for any wallet, including block ranges and sorting options.
- **Token Tracking** — Monitor ERC-20 and ERC-721 (NFT) transfer events to track asset movements across the network.
- **Contract Inspection** — Fetch verified source code and ABIs for smart contracts to understand protocol logic.
- **Network Stats** — Access block rewards, total AVAX supply, and the latest price data directly from the chain.

### How it works

1. Subscribe to this server
2. Enter your Snowtrace API Key
3. Start querying Avalanche data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly fetch contract ABIs and debug transaction execution status from your IDE.
- **Data Analysts** — aggregate wallet balances and token transfer history for on-chain research.
- **Crypto Enthusiasts** — monitor your portfolio and track NFT movements using natural language.


## Available Tools
- **get_avax_balance_multi**: Get AVAX Balance for Multiple Addresses
- **get_avax_balance**: Get AVAX Balance for a Single Address
- **check_verify_status**: Check Verification Status
- **get_avax_last_price**: Get AVAX Last Price
- **get_avax_total_supply**: Get Total Supply of AVAX
- **get_contract_abi**: Get Contract ABI
- **get_block_countdown**: Get Estimated Block Countdown
- **get_block_number_by_time**: Get Block Number by Timestamp
- **get_block_reward**: Get Block Rewards
- **get_logs**: Get Logs
- **get_contract_source_code**: Get Contract Source Code
- **check_contract_execution_status**: Check Contract Execution Status
- **check_transaction_receipt_status**: Check Transaction Receipt Status
- **get_mined_blocks**: Get Blocks Mined by Address
- **get_token_balance**: Get ERC-20 Token Balance for Address
- **get_erc721_transfers**: Get ERC-721 (NFT) Token Transfer Events
- **get_token_total_supply**: Get ERC-20 Token Total Supply
- **get_erc20_transfers**: Get ERC-20 Token Transfer Events
- **get_internal_transactions**: Get Internal Transactions
- **get_normal_transactions**: Get Normal Transactions by Address
- **verify_source_code**: Verify Source Code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snowtrace (Avalanche Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current AVAX balance of 0x742d35Cc6634C0532925a3b844Bc454e4438f44e?"

**🤖 AI Agent:**
> I've checked the address on the Avalanche C-Chain. The current balance is 15.42 AVAX.

---

**👤 You:**
> "Show me the last 5 ERC-20 transfers for wallet 0x123..."

**🤖 AI Agent:**
> Fetching recent token activity... I found 5 recent transfers, including 100 USDC received and two outgoing transfers of JOE tokens. Would you like the transaction hashes for these?

---

**👤 You:**
> "Get the ABI for the contract at 0x60ae616a2155ee3d9a68541ba4544862310933d4."

**🤖 AI Agent:**
> I have retrieved the ABI for the verified contract. It contains 24 functions, including `swapExactTokensForTokens` and `addLiquidity`. I can help you format a specific call if needed.


## Installation & Usage

To install and use the **Snowtrace (Avalanche Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snowtrace-avalanche-explorer](https://vinkius.com/mcp/snowtrace-avalanche-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
