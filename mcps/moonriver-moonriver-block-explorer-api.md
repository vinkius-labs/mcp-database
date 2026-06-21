# Moonriver (Moonriver Block Explorer API) MCP Server

Query Moonriver blockchain data—blocks, transactions, account balances, and EVM tokens—directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/moonriver-moonriver-block-explorer-api)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect to the **Moonriver** network to inspect real-time blockchain activity. This server allows your AI agent to interact with the Moonriver Block Explorer API, providing deep insights into on-chain data without leaving your chat interface.

### What you can do

- **Block Exploration** — List recent blocks or fetch specific block details by height using `list_blocks` and `get_block`.
- **Transaction Tracking** — Query extrinsics (transactions) by address or hash to monitor network activity via `list_extrinsics` and `get_extrinsic`.
- **Account Analysis** — Retrieve balance information, metadata, and transfer history for any Moonriver address with `get_account_info` and `list_transfers`.
- **EVM Token Monitoring** — List ERC-20 and ERC-721 tokens and track their movements across the network using `list_evm_tokens`.
- **Network Metadata** — Get high-level information about the Moonriver network status with `get_metadata`.

### How it works

1. Subscribe to this server
2. Enter your Moonriver (Subscan-based) API Key
3. Start querying the Kusama-based parachain from Claude, Cursor, or any MCP client.

No more manually searching through block explorers. Your AI acts as a dedicated blockchain analyst.

### Who is this for?

- **Web3 Developers** — quickly verify transaction statuses and account balances without leaving the IDE.
- **Data Analysts** — extract block data and token transfer history for research and reporting.
- **Crypto Enthusiasts** — monitor wallet activity and network health through natural conversation.


## Available Tools
- **get_account_info**: Get account details
- **get_block**: Get block details
- **get_extrinsic**: Get extrinsic details
- **get_metadata**: Get Moonriver network metadata
- **list_blocks**: Get a list of blocks
- **list_evm_tokens**: Get token list
- **list_extrinsics**: Get a list of extrinsics (transactions)
- **list_transfers**: Get account transfers


## Installation & Usage

To install and use the **Moonriver (Moonriver Block Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moonriver-moonriver-block-explorer-api](https://vinkius.com/mcp/moonriver-moonriver-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
