# BscScan (BNB Chain Explorer) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bscscan-bnb-chain-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bscscan-bnb-chain-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bscscan-bnb-chain-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access real-time BNB Chain data—check balances, track BEP-20/BEP-721 transfers, and inspect verified smart contracts directly from your AI agent.

## Description
Connect your AI agent to **BscScan** to explore the BNB Chain ecosystem with unprecedented depth. This server provides a comprehensive suite of tools to query blockchain data, from simple balance checks to complex smart contract inspections.

### What you can do

- **Wallet Analytics** — Retrieve BNB balances for single or multiple addresses instantly.
- **Transaction History** — Fetch normal and internal transactions to audit wallet activity.
- **Token Tracking** — Monitor BEP-20 and BEP-721 (NFT) transfer events across the network.
- **Smart Contract Auditing** — Access verified source code and ABIs for deep technical analysis.
- **Network Status** — Check transaction receipt statuses and execution results.

### How it works

1. Subscribe to this server
2. Enter your BscScan API Key
3. Start querying the BNB Chain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly fetch ABIs and source code without leaving your IDE.
- **Crypto Analysts** — automate the tracking of whale movements and token distributions.
- **DeFi Users** — verify transaction statuses and wallet balances through natural language.


## Available Tools
- **get_bep20_transfers**: Get List of BEP-20 Token Transfer Events by Address
- **get_bep721_transfers**: Get List of BEP-721 (NFT) Token Transfer Events by Address
- **get_block_countdown**: Get Estimated Block Countdown Time by BlockNo
- **get_block_reward**: Get Block Rewards by BlockNo
- **get_bnb_balance_multi**: Get BNB Balance for Multiple Addresses
- **get_bnb_balance**: Get BNB Balance for a Single Address
- **get_bsc_price**: Get Last Price of BNB
- **get_bsc_supply**: Get Total Supply of BNB on BSC
- **get_contract_abi**: Get Contract ABI for Verified Source Codes
- **get_contract_execution_status**: Check Contract Execution Status
- **get_contract_source_code**: Get Contract Source Code for Verified Source Codes
- **get_eth_block_number**: Get Current Block Number (Proxy)
- **get_eth_transaction_by_hash**: Get Transaction by Hash (Proxy)
- **get_internal_transactions**: Get List of Internal Transactions by Address
- **get_normal_transactions**: Get List of Normal Transactions by Address
- **get_transaction_receipt_status**: Check Transaction Receipt Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BscScan (BNB Chain Explorer)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the BNB balance for address 0x000000000000000000000000000000000000dEaD"

**🤖 AI Agent:**
> I've checked the balance for that address. It currently holds 0.00 BNB.

---

**👤 You:**
> "List the last 5 BEP-20 token transfers for 0xbb4CdB9CBd36B01bD1cBaEBF2De08d9173bc095c"

**🤖 AI Agent:**
> I've retrieved the recent BEP-20 transfers for that address. [List of transfers with token names, amounts, and timestamps].

---

**👤 You:**
> "Get the source code for the contract at 0x0e09fabb73bd3ade0a17ecc321fd13a19e81ce82"

**🤖 AI Agent:**
> I've fetched the verified source code for the PancakeSwap: Token contract. It includes the Solidity files and compiler settings used for deployment.


## Installation & Usage

To install and use the **BscScan (BNB Chain Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bscscan-bnb-chain-explorer](https://vinkius.com/mcp/bscscan-bnb-chain-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
