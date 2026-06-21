# Alchemy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alchemy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/alchemy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/alchemy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage blockchain data — audit wallets, NFTs, and transactions via AI.

## Description
Empower your AI agent to orchestrate your entire web3 research and blockchain auditing workflow with **Alchemy**, the comprehensive platform for decentralized data. By connecting Alchemy to your agent, you transform complex RPC querying into a natural conversation. Your agent can instantly retrieve wallet balances, audit NFT ownership, and query transaction receipts without you ever touching a block explorer. Whether you are conducting investment research or monitoring digital assets, your agent acts as a real-time blockchain analyst, ensuring your data is always precise and up-to-the-minute.

### What you can do

- **Wallet Auditing** — Retrieve high-resolution balances for any Ethereum or compatible address, including native and ERC-20 tokens.
- **NFT Oversight** — Audit the NFT collection for specific owners to maintain a clear view of digital asset distribution and metadata.
- **Transaction Intelligence** — Query real-time transaction receipts to understand the status and outcome of blockchain events instantly.
- **Network Discovery** — Retrieve the latest block numbers to assist in regional and temporal blockchain planning.
- **Operational Monitoring** — Check API status to ensure your web3 research workflow is always operational across supported networks.

### How it works

1. Subscribe to this server
2. Enter your Alchemy API Key and select your target Network
3. Start managing your blockchain intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — monitor smart contract events and retrieve blockchain metadata straight from your workflow.
- **Investors & Analysts** — verify wallet balances and audit NFT portfolios without manual searching.
- **Security Researchers** — perform rapid audits of transaction receipts and identify relevant asset markers through natural language.
- **Operations Leads** — automate blockchain data querying to orchestrate cross-functional decentralized teams smoothly.


## Available Tools
- **check_api_status**: Check if the Alchemy service is operational
- **get_wallet_balance**: Get the balance of an Ethereum address in wei
- **get_latest_block_number**: Get the number of the most recent block
- **get_owned_nfts**: Get all NFTs owned by a specific address
- **get_token_balances**: Get all ERC-20 token balances for a specific address
- **get_transaction_receipt**: Get the receipt of a transaction by hash


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alchemy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the balance of Ethereum address '0x123...' using Alchemy?"

**🤖 AI Agent:**
> I've retrieved the balance for that address! The current balance is 1.5 ETH (represented in wei). I can assist you with the ERC-20 token balances for this wallet if you'd like.

---

**👤 You:**
> "Show all NFTs owned by '0x456...'."

**🤖 AI Agent:**
> I've identified 5 NFTs in that wallet! Notable items include an 'Art Blocks' piece and a 'CryptoPunk'. I can provide the full token ID and collection metadata for each if you'd like.

---

**👤 You:**
> "What is the latest block number on 'eth-mainnet'?"

**🤖 AI Agent:**
> I've retrieved the latest block number for Ethereum Mainnet! It is currently identified as block #19,250,000 (hex: 0x125B9A0). I can assist you with a specific transaction audit from this block if needed.


## Installation & Usage

To install and use the **Alchemy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alchemy](https://vinkius.com/mcp/alchemy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
