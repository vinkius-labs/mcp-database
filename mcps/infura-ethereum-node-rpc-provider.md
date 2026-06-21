# Infura (Ethereum Node RPC Provider) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infura-ethereum-node-rpc-provider)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/infura-ethereum-node-rpc-provider-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/infura-ethereum-node-rpc-provider-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access Ethereum blockchain data via Infura — query blocks, check balances, estimate gas, and interact with smart contracts directly from any AI agent.

## Description
Connect your **Infura** account to any AI agent to interact with the Ethereum blockchain using natural language. This MCP server provides a robust bridge to Infura's high-performance RPC nodes.

### What you can do

- **Blockchain Queries** — Fetch the latest block number, block details by hash or number, and transaction counts.
- **Account & Contract Data** — Check balances for any Ethereum address, retrieve smart contract code, and get transaction nonces.
- **Transaction Analysis** — Inspect transaction details and receipts using hashes to debug or track on-chain activity.
- **Gas & Network Metrics** — Get current gas prices, fee history, and suggested gas fees for optimal transaction scheduling.
- **Smart Contract Interaction** — Execute read-only calls to smart contracts using `eth_call` and estimate gas for potential transactions.

### How it works

1. Subscribe to this server
2. Enter your Infura API Key (Project ID)
3. (Optional) Specify your target network (e.g., mainnet, sepolia)
4. Start querying Ethereum data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — debug transactions and check contract states directly from your IDE without leaving the code.
- **Data Analysts** — pull real-time blockchain metrics and block data for quick analysis through conversation.
- **Crypto Enthusiasts** — monitor wallet balances and network congestion levels using simple natural language commands.


## Available Tools
- **eth_blockNumber**: Get the number of the most recent block
- **eth_call**: Execute a new message call immediately
- **eth_chainId**: Get the chain ID
- **eth_estimateGas**: Estimate gas needed for a transaction
- **eth_feeHistory**: Get transaction fee history
- **eth_gasPrice**: Get current gas price
- **eth_getBalance**: Get the balance of an account
- **eth_getBlockByHash**: Get information about a block by hash
- **eth_getBlockByNumber**: Get information about a block by number
- **eth_getBlockTransactionCountByHash**: Get transaction count in a block by hash
- **eth_getBlockTransactionCountByNumber**: Get transaction count in a block by number
- **eth_getCode**: Get code at a given address
- **eth_getFilterChanges**: Get changes for a filter
- **eth_getLogs**: Get logs matching a filter
- **eth_getTransactionByHash**: Get transaction information by hash
- **eth_getTransactionCount**: Get the number of transactions sent from an address (nonce)
- **eth_getTransactionReceipt**: Note: Receipt is not available for pending transactions.

Get the receipt of a transaction by hash
- **eth_newFilter**: Create a new filter for polling
- **eth_sendRawTransaction**: Send a signed transaction
- **get_suggested_gas_fees**: Get suggested gas fees (EIP-1559)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infura (Ethereum Node RPC Provider)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current block number on Ethereum?"

**🤖 AI Agent:**
> The most recent block number is 0x11B560F (decimal: 18568719).

---

**👤 You:**
> "Check the balance of 0x742d35Cc6634C0532925a3b844Bc454e4438f44e at the latest block."

**🤖 AI Agent:**
> The balance for that address is 0xde0b6b3a7640000 wei, which is equivalent to 1.0 ETH.

---

**👤 You:**
> "What are the suggested gas fees right now?"

**🤖 AI Agent:**
> Based on current network conditions, the suggested base fee is 15 Gwei with a priority fee of 1.5 Gwei for a standard transaction.


## Installation & Usage

To install and use the **Infura (Ethereum Node RPC Provider)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infura-ethereum-node-rpc-provider](https://vinkius.com/mcp/infura-ethereum-node-rpc-provider)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
