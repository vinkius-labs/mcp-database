# Lineascan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lineascan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lineascan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lineascan-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Linea blockchain — check ETH balances, track ERC-20/NFT transfers, and inspect smart contract source code directly from your AI.

## Description
Connect to **Lineascan** and empower your AI agent with real-time access to the Linea network. This server provides a comprehensive suite of tools for blockchain analysis, transaction tracking, and smart contract interaction.

### What you can do

- **Account Analysis** — Retrieve ETH balances for single or multiple addresses and list blocks mined by specific accounts.
- **Transaction Tracking** — Query normal and internal transaction histories, as well as ERC-20 and ERC-721 (NFT) transfer events with full metadata.
- **Contract Intelligence** — Fetch ABIs and source code for verified smart contracts to understand underlying logic and security.
- **Network Insights** — Access block rewards, gas estimates, and transaction receipts to monitor network health and costs.

### How it works

1. Subscribe to this server
2. Enter your Lineascan API Key
3. Start querying the Linea blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly inspect contract ABIs and source code without leaving your IDE.
- **Data Analysts** — track token movements and transaction volumes across the Linea ecosystem.
- **Crypto Users** — monitor wallet balances and transaction statuses through natural language.


## Available Tools
- **balance_multi**: Get ETH balances for multiple addresses
- **check_verify_status**: Check the status of a verification request
- **eth_block_number**: Returns the number of the most recent block
- **eth_call**: Executes a new message call immediately without creating a transaction
- **eth_estimate_gas**: Generates an estimate of how much gas is needed for a transaction
- **eth_get_block_by_number**: Returns information about a block by number
- **eth_get_transaction_by_hash**: Returns information about a transaction by hash
- **eth_get_transaction_receipt**: Returns the receipt of a transaction by hash
- **eth_price**: Get the current price of ETH in USD and BTC
- **eth_supply**: Get the total supply of ETH on Linea
- **get_abi**: Get the Contract ABI for a verified smart contract
- **get_balance**: Get ETH balance for a single address
- **get_block_countdown**: Get estimated time remaining until a block is mined
- **get_block_no_by_time**: Get block number by timestamp
- **get_block_reward**: Get block and uncle rewards by block number
- **get_logs**: Get event logs with filtering options
- **get_mined_blocks**: Get a list of blocks mined by an address
- **get_source_code**: Get the Source Code for a verified smart contract
- **get_status**: Check the execution status of a transaction
- **get_tx_receipt_status**: Check the receipt status of a transaction
- **token_nft_tx**: Get a list of ERC-721 Token Transfer Events for an address
- **token_tx**: Get a list of ERC-20 Token Transfer Events for an address
- **tx_list_internal**: Get a list of Internal transactions for an address
- **tx_list**: Get a list of Normal transactions for an address
- **verify_source_code**: Submit a contract for verification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lineascan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ETH balance of the address 0x1234567890abcdef1234567890abcdef12345678?"

**🤖 AI Agent:**
> I've checked the balance for that address on Linea. It currently holds 1.25 ETH.

---

**👤 You:**
> "List the last 5 ERC-20 token transfers for address 0xabc...123."

**🤖 AI Agent:**
> I found the recent ERC-20 transfers for that address. The most recent ones include transfers of USDC and WETH. Would you like the specific transaction hashes?

---

**👤 You:**
> "Get the ABI and source code for the contract at 0x789...def."

**🤖 AI Agent:**
> I've retrieved the data for the contract. It is a verified 'LiquidityPool' contract. I have the ABI ready for function calls and the Solidity source code for your review.


## Installation & Usage

To install and use the **Lineascan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lineascan](https://vinkius.com/mcp/lineascan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
