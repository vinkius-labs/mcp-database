# Wemix Explorer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wemix-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wemix-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wemix-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore Wemix blockchain data — query accounts, track token transfers, and inspect blocks or extrinsics directly from your AI agent.

## Description
Connect your AI agent to the **Wemix Network** to gain real-time visibility into blockchain activity. This server provides a comprehensive suite of tools to audit addresses, monitor token movements, and analyze network health.

### What you can do

- **Account Auditing** — Retrieve detailed account info, token balances, and historical transfers for any Wemix address.
- **Block Inspection** — Fetch recent block lists or drill down into specific block heights and hashes for deep analysis.
- **Transaction Tracking** — Query extrinsics (transactions) and events to understand smart contract interactions and state changes.
- **Token Ecosystem** — List all available tokens on the network and fetch metadata for specific assets using symbols or IDs.
- **Network Monitoring** — Access live event streams and extrinsic logs to keep track of network-wide activity.

### How it works

1. Subscribe to this server
2. Enter your Wemix/Subscan API Key
3. Start querying the blockchain from Claude, Cursor, or any MCP client

No more manual searching through web explorers. Your AI acts as a blockchain analyst, providing structured data on demand.

### Who is this for?

- **Web3 Developers** — debug extrinsics and verify contract events directly from your IDE.
- **Crypto Analysts** — track whale movements and token distribution patterns via natural language.
- **Node Operators** — monitor block production and network events without leaving the terminal.


## Available Tools
- **get_account_info**: Get basic information for a specific account
- **list_account_tokens**: List tokens held by an account
- **list_account_transfers**: Get a list of transfers associated with an account
- **get_block**: Get detailed information for a specific block
- **list_blocks**: Get a list of recent blocks
- **get_event**: Get detailed information for a specific event
- **list_events**: Get a list of events
- **get_extrinsic**: Get detailed information for a specific extrinsic
- **list_extrinsics**: Get a list of recent extrinsics (transactions)
- **get_token**: Get detailed information for a specific token
- **list_tokens**: Get a list of tokens on the network


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wemix Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest blocks on the Wemix network."

**🤖 AI Agent:**
> I've retrieved the latest blocks. The most recent block is #14502134, produced 6 seconds ago with 12 extrinsics. Would you like to see the details of a specific block?

---

**👤 You:**
> "What tokens are held by the address 0x742d35Cc6634C0532925a3b844Bc454e4438f44e?"

**🤖 AI Agent:**
> Checking the wallet... This account holds 500 WEMIX, 1,200 WEMIX$, and 50 stWEMIX. I can also list the recent transfers for this address if you'd like.

---

**👤 You:**
> "Get details for extrinsic hash 0x123...abc"

**🤖 AI Agent:**
> Extrinsic 0x123...abc was finalized in block #14502100. It was a 'balances.transfer' call from address A to address B. The status is 'Success'.


## Installation & Usage

To install and use the **Wemix Explorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wemix-explorer](https://vinkius.com/mcp/wemix-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
