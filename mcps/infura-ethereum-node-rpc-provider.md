# Infura (Ethereum Node RPC Provider) MCP Server

Access Ethereum blockchain data via Infura — query blocks, check balances, estimate gas, and interact with smart contracts directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/infura-ethereum-node-rpc-provider)

## Overview
**Category:** developer-tools
**Tools Count:** 20

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


## Installation & Usage

To install and use the **Infura (Ethereum Node RPC Provider)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infura-ethereum-node-rpc-provider](https://vinkius.com/mcp/infura-ethereum-node-rpc-provider)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
