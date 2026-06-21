# Shiden Scan (Shiden Network Block Explorer) MCP Server

Explore Shiden Network blockchain data—blocks, extrinsics, accounts, and EVM contracts—directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shiden-scan-shiden-network-block-explorer)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect to the **Shiden Network** (the multi-chain smart contract layer on Kusama) and query live blockchain data through natural language conversation.

### What you can do

- **Block & Extrinsic Tracking** — List recent blocks or fetch specific extrinsics by hash to monitor network activity and finality.
- **Account Auditing** — Retrieve detailed balance information (transferable, bonded, reserved) and transaction history for any SS58 address.
- **EVM Contract Inspection** — Fetch metadata and transaction logs for smart contracts deployed on Shiden's Ethereum-compatible layer.
- **Market Data** — Get real-time SDN token price, market capitalization, and 24h trading volume.
- **Network Metadata** — Access chain-specific details like token decimals, SS58 prefixes, and network naming conventions.

### How it works

1. Subscribe to this server
2. Enter your Shiden Scan (Subscan) API Key
3. Start querying the Shiden blockchain from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Debug extrinsics and verify contract deployments without leaving your code editor.
- **Crypto Analysts** — Track large transfers and monitor SDN market metrics via simple chat commands.
- **Node Operators** — Quickly check block heights and network metadata to ensure synchronization.


## Available Tools
- **get_account_info**: Retrieve balance and metadata for a specific account
- **get_block**: Retrieve details for a specific block
- **list_blocks**: Retrieve a list of blocks
- **get_evm_contract**: Retrieve information about a deployed smart contract
- **list_evm_transactions**: Retrieve transactions related to a specific contract
- **get_extrinsic**: Retrieve details for a specific extrinsic
- **list_extrinsics**: Retrieve a list of extrinsics
- **get_metadata**: Retrieve metadata about the Shiden Network
- **get_token_price**: Retrieve the current price of the SDN token
- **list_transfers**: Retrieve a list of transfers for a specific account


## Installation & Usage

To install and use the **Shiden Scan (Shiden Network Block Explorer)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shiden-scan-shiden-network-block-explorer](https://vinkius.com/mcp/shiden-scan-shiden-network-block-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
