# Blockscout MCP Server

Explore Ethereum-based blockchains directly from your AI agent. Query addresses, tokens, transactions, and smart contracts via Blockscout's open-source API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/blockscout)

## Overview
**Category:** developer-tools
**Tools Count:** 14

## Description
Connect any **Blockscout** explorer instance to your AI agent for deep on-chain analysis and real-time blockchain data retrieval.

### What you can do

- **Address & Balance Auditing** — Fetch native balances, transaction counts, and ENS names for any wallet or contract address.
- **Token Portfolio Tracking** — List all ERC-20, ERC-721, and ERC-1155 tokens held by an address with a single query.
- **Transaction Inspection** — Get detailed status, gas usage, and decoded input data for any transaction hash.
- **Block & Network Health** — Retrieve block metadata (miner, fees, timestamps) and check the explorer's indexing status.
- **Developer Tools** — Access verified contract ABIs and transaction histories using Etherscan-compatible endpoints.

### How it works

1. Subscribe to this server
2. Provide the Base URL of your preferred Blockscout instance (e.g., `https://eth.blockscout.com`)
3. (Optional) Enter your API Key for higher rate limits
4. Start querying blockchain data from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Verify contract deployments and debug transactions directly from your IDE.
- **Data Analysts** — Extract on-chain metrics and token distributions through natural language.
- **Crypto Power Users** — Monitor wallet balances and portfolio movements without leaving your chat interface.


## Available Tools
- **get_account_balance**: Get native balance for an address (Etherscan API)
- **get_account_internal_transactions**: Get internal transactions by address (Etherscan API)
- **get_account_transactions**: Get transactions by address (Etherscan API)
- **get_address**: Retrieve address details
- **get_block**: Get block details
- **get_contract_abi**: Get contract ABI (Etherscan API)
- **get_contract_source_code**: Get contract source code (Etherscan API)
- **get_indexing_status**: Get indexing status
- **get_logs**: Get event logs (Etherscan API)
- **get_token**: Get token info
- **get_total_supply**: Get total supply of native coin (Etherscan API)
- **get_transaction**: Get transaction details
- **json_rpc**: Execute a standard Ethereum JSON-RPC 2.0 method
- **list_token_balances**: List token balances for an address


## Installation & Usage

To install and use the **Blockscout** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockscout](https://vinkius.com/mcp/blockscout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
