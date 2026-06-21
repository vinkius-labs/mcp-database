# FtmScan (Fantom Network Explorer) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ftmscan-fantom-network-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ftmscan-fantom-network-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ftmscan-fantom-network-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Fantom blockchain data directly—query wallet balances, transaction history, smart contract source code, and token transfers via FtmScan.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FtmScan (Fantom Network Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current FTM balance of address 0xbbbb6a3601eeed31c8245938021fb3d10e7c51e2?"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 1,250.45 FTM.

---

**👤 You:**
> "Show me the last 5 normal transactions for 0xbbbb6a3601eeed31c8245938021fb3d10e7c51e2 sorted by newest."

**🤖 AI Agent:**
> I've retrieved the 5 most recent normal transactions for that address. They include several transfers and contract interactions from the last few hours.

---

**👤 You:**
> "Get the verified source code for the contract at 0x04068da6a83afcfa0e13ba15a6696662335d5b75."

**🤖 AI Agent:**
> I have successfully retrieved the verified source code for the contract. It appears to be a SpookySwap LP token contract written in Solidity.


## Installation & Usage

To install and use the **FtmScan (Fantom Network Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ftmscan-fantom-network-explorer](https://vinkius.com/mcp/ftmscan-fantom-network-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
