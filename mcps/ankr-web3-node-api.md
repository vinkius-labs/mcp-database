# Ankr (Web3 Node API) MCP Server

Access high-performance Web3 RPC nodes via Ankr. Query block data, check wallet balances, and interact with smart contracts across multiple EVM chains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ankr-web3-node-api)

## Overview
**Category:** developer-tools
**Tools Count:** 32

## Description
Connect your AI agent to **Ankr's** global node infrastructure and interact with blockchain data through natural language. This server provides a direct bridge to Ethereum and other EVM-compatible chains.

### What you can do

- **Chain Queries** — Fetch the latest block numbers and detailed block information by hash or number across supported networks.
- **Account Auditing** — Check wallet balances, transaction counts (nonces), and retrieve the smart contract code at any address.
- **Transaction Analysis** — Inspect transaction details and receipts, or estimate gas costs for potential on-chain operations.
- **Smart Contract Interaction** — Execute `eth_call` to read contract states or simulate complex multi-transaction scenarios with `eth_simulateV1`.
- **State Inspection** — Access raw storage slots with `eth_getStorageAt` and filter event logs with `eth_getLogs` for deep data analysis.

### How it works

1. Subscribe to this server
2. Enter your Ankr JWT Token
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

No more manual JSON-RPC requests or complex Postman setups. Your AI acts as a blockchain developer or data analyst.

### Who is this for?

- **Web3 Developers** — quickly debug smart contracts, check nonces, and verify deployments directly from the IDE.
- **DeFi Researchers** — analyze on-chain state, simulate transactions, and fetch historical logs without writing custom scripts.
- **Data Analysts** — retrieve real-time blockchain metrics and block data for reporting and monitoring.


## Available Tools
- **ankr_getAccountBalance**: Retrieves all token balances for a wallet
- **ankr_getBlocks**: Retrieves full info for a range of blocks
- **ankr_getInteractions**: Lists all blockchains a wallet has interacted with
- **ankr_getNFTHolders**: Lists all holders of a specific NFT collection
- **ankr_getNFTMetadata**: Retrieves metadata for a specific NFT
- **ankr_getNFTsByOwner**: Retrieves all NFTs owned by an address across multiple chains
- **ankr_getTokenPrice**: Returns the current USD price of a token
- **ankr_getTokenTransfers**: Returns historical token transfer data
- **eth_blockNumber**: Returns the most recent block number
- **eth_call**: Executes a call without creating a transaction
- **eth_estimateGas**: Estimates gas needed for a transaction
- **eth_getBalance**: Returns the balance of an address
- **eth_getBlockByHash**: Returns block information by hash
- **eth_getBlockByNumber**: Returns block information by number
- **eth_getCode**: Returns the code at a given address
- **eth_getLogs**: Returns logs matching filter criteria
- **eth_getStorageAt**: Returns the value from a storage position
- **eth_getTransactionByHash**: Returns transaction details
- **eth_getTransactionCount**: Returns the number of transactions sent from an address (nonce)
- **eth_getTransactionReceipt**: Returns the receipt of a transaction
- **eth_sendRawTransaction**: Submits a signed transaction to the network
- **eth_simulateV1**: Simulates multiple blocks/transactions
- **getAccountInfo**: Returns all info associated with a Pubkey
- **getBalance**: Returns the lamport balance of an account
- **getBlockHeight**: Returns the current block height
- **getBlock**: Returns identity and transaction info for a confirmed block
- **getEpochInfo**: Returns information about the current epoch
- **getLatestBlockhash**: Returns the latest blockhash for transaction building
- **getProgramAccounts**: Returns all accounts owned by a program
- **getTransaction**: Returns details for a confirmed transaction
- **sendTransaction**: Submits a signed transaction
- **simulateTransaction**: Simulates a transaction to check for errors


## Installation & Usage

To install and use the **Ankr (Web3 Node API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ankr-web3-node-api](https://vinkius.com/mcp/ankr-web3-node-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
