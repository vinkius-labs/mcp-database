# IoTeX (IoTeX Block Explorer API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iotex-iotex-block-explorer-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iotex-iotex-block-explorer-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iotex-iotex-block-explorer-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access IoTeX blockchain data — query accounts, blocks, transactions, and token details directly from your AI agent.

## Description
Connect to the **IoTeX** blockchain and explore real-time network data through natural conversation. This MCP server provides a comprehensive interface to the IoTeX Block Explorer API.

### What you can do

- **Account Insights** — Retrieve balances, nonces, and metadata for any IoTeX address using the `get_account` tool.
- **Transaction History** — Fetch a list of actions associated with an account via `get_account_actions` or inspect specific transactions with `get_action`.
- **Block Exploration** — Query detailed block data by height or hash using `get_block_by_height` and `get_block_by_hash`.
- **Network Activity** — Monitor the pulse of the network with `get_recent_actions` to see the latest transactions.
- **Token Analysis** — Get metadata for XRC20/XRC721 tokens and list their holders using `get_token` and `get_token_holders`.

### How it works

1. Subscribe to this server
2. (Optional) Enter your IoTeX API Key for higher rate limits
3. Start querying the IoTeX network from Claude, Cursor, or any MCP-compatible client

No more manual searching through web explorers. Your AI acts as a blockchain analyst, providing instant data on addresses, blocks, and tokens.

### Who is this for?

- **Web3 Developers** — quickly verify transaction statuses and account balances without leaving the code editor.
- **Data Analysts** — extract block and token holder data for research and reporting.
- **Crypto Enthusiasts** — monitor network activity and token metadata through simple chat commands.


## Available Tools
- **get_account_actions**: Get Account Transactions
- **get_account**: Get Account Details
- **get_action**: Get Action by Hash
- **get_block_by_hash**: Get Block by Hash
- **get_block_by_height**: Get Block by Height
- **get_recent_actions**: Get Recent Actions
- **get_token_holders**: Get Token Holders
- **get_token**: Get Token Details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IoTeX (IoTeX Block Explorer API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get account details and balance for IoTeX address io1prv56hmvfm08z6p6v6v6v6v6v6v6v6v6v6v6v6."

**🤖 AI Agent:**
> I've retrieved the details for account io1prv... The current balance is 1,250 IOTX with a nonce of 42. Would you like to see the recent transaction history for this address?

---

**👤 You:**
> "Show me the most recent actions on the IoTeX network."

**🤖 AI Agent:**
> Fetching recent network activity... I found the latest actions including several transfers and contract executions. The most recent was a transfer of 500 IOTX at block height 31054201.

---

**👤 You:**
> "What are the details for the token at contract address io1hp6y4...?"

**🤖 AI Agent:**
> Analyzing token metadata... This contract corresponds to the 'MachineFi' token (MFI). It has a total supply of 1,000,000,000 and 18 decimals. Should I list the current top holders?


## Installation & Usage

To install and use the **IoTeX (IoTeX Block Explorer API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iotex-iotex-block-explorer-api](https://vinkius.com/mcp/iotex-iotex-block-explorer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
