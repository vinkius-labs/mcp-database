# Blockscout MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockscout)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/blockscout-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/blockscout-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore Ethereum-based blockchains directly from your AI agent. Query addresses, tokens, transactions, and smart contracts via Blockscout's open-source API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blockscout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the balance and ENS name for address 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045."

**🤖 AI Agent:**
> I've retrieved the details for that address. It currently holds 1,245 ETH, is associated with the ENS name 'vitalik.eth', and has a total of 12,432 transactions.

---

**👤 You:**
> "List all token balances for 0x742d35Cc6634C0532925a3b844Bc454e4438f44e."

**🤖 AI Agent:**
> I found several tokens in this wallet. It holds 500 USDT, 10.5 LINK, and 2 NFTs from the 'Bored Ape Yacht Club' collection. Would you like more details on a specific token?

---

**👤 You:**
> "Check the status and gas used for transaction 0x5c504ed432cb511de36b21cdd8187727a1714170f96219109512ee1000673974."

**🤖 AI Agent:**
> Transaction 0x5c50... was successful. It was included in block 12,345,678 and used 21,000 gas units with a total fee of 0.000441 ETH.


## Installation & Usage

To install and use the **Blockscout** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockscout](https://vinkius.com/mcp/blockscout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
