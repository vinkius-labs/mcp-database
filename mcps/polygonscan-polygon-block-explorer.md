# Polygonscan (Polygon Block Explorer) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polygonscan-polygon-block-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/polygonscan-polygon-block-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/polygonscan-polygon-block-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Query the Polygon blockchain directly — check MATIC balances, track transactions, and inspect smart contracts via any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polygonscan (Polygon Block Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current MATIC balance of address 0x0000000000000000000000000000000000001010?"

**🤖 AI Agent:**
> I've checked the address. The current MATIC balance for 0x000...1010 is 15,240.45 MATIC.

---

**👤 You:**
> "List the last 5 normal transactions for address 0x123..."

**🤖 AI Agent:**
> Fetching transaction history... I found the 5 most recent transactions for that address. The latest one was a transfer of 50 MATIC to 0xabc... on block 62451203.

---

**👤 You:**
> "Get the ERC-20 token transfer events for address 0x456..."

**🤖 AI Agent:**
> I've retrieved the ERC-20 transfer events. There are several recent transfers, including 100 USDC and 500 LINK tokens moving through this address.


## Installation & Usage

To install and use the **Polygonscan (Polygon Block Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polygonscan-polygon-block-explorer](https://vinkius.com/mcp/polygonscan-polygon-block-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
