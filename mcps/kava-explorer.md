# Kava Explorer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kava-explorer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kava-explorer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kava-explorer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Explore the Kava blockchain — inspect accounts, track transactions (extrinsics), monitor blocks, and analyze validator performance via Subscan.

## Description
Connect your AI agent to the **Kava Network** through this comprehensive explorer server. Powered by Subscan, it provides deep visibility into on-chain data, from simple account balances to complex validator metrics.

### What you can do

- **Account Auditing** — Retrieve detailed account info, token balances, and historical rewards or slash events for any Kava address.
- **Transaction Tracking** — Query specific extrinsics by hash or index, or list recent transactions with advanced filtering by module and call.
- **Network Monitoring** — Fetch real-time block data, list recent blocks, and inspect system events emitted by the blockchain.
- **Staking & Governance** — Access a complete list of validators and drill down into specific validator performance and staking details.

### How it works

1. Subscribe to this server
2. Enter your Subscan API Key
3. Start querying Kava mainnet data directly from your favorite AI client

### Who is this for?

- **Web3 Developers** — Debug extrinsics and monitor events without leaving your terminal or code editor.
- **Crypto Analysts** — Extract account balances and reward history for financial reporting and research.
- **Node Operators** — Monitor validator status and network health through natural language queries.


## Available Tools
- **get_account_info**: Get basic information for a Kava account
- **get_account_reward_slash**: Get rewards and slashes for an account
- **get_account_token**: Get token balances for an account
- **get_block**: Get block details by height or hash
- **list_blocks**: Get a list of blocks
- **list_events**: Get a list of events with filtering options
- **get_extrinsic**: Get extrinsic details by hash or index
- **list_extrinsics**: Get a list of extrinsics
- **get_validator**: Get details for a specific validator
- **list_validators**: Get a list of validators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kava Explorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the balance and account info for Kava address kava1..."

**🤖 AI Agent:**
> I've retrieved the account info for kava1... The account currently holds 1,250 KAVA with a nonce of 42. Would you like to see the specific token balances as well?

---

**👤 You:**
> "What are the latest blocks on the Kava network?"

**🤖 AI Agent:**
> Fetching the most recent blocks... The latest block is #5,402,120, produced 6 seconds ago by validator 'KavaLabs'. There were 12 extrinsics in this block.

---

**👤 You:**
> "Check the rewards and slashes for address kava1..."

**🤖 AI Agent:**
> I found 15 reward events for this address in the last 24 hours, totaling 5.2 KAVA. No slash events were detected in the recent history.


## Installation & Usage

To install and use the **Kava Explorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kava-explorer](https://vinkius.com/mcp/kava-explorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
