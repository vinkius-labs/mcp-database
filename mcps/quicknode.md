# QuickNode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quicknode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/quicknode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/quicknode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage blockchain infrastructure via QuickNode — create data streams, configure webhooks, and interact with RPC nodes directly from your AI agent.

## Description
Connect your **QuickNode** account to any AI agent to orchestrate Web3 infrastructure through natural language. This server provides a comprehensive suite of tools to manage high-performance blockchain data pipelines and queries.

### What you can do

- **Streams Management** — Create, list, and update real-time data streams for historical and live blockchain ingestion using `create_stream` and `list_streams`.
- **Webhooks** — Deploy webhooks from templates (like EVM wallet filters or contract events) to deliver real-time events to your HTTP endpoints via `create_webhook`.
- **KV Store** — Manage key-value pairs and lists to power advanced server-side filtering logic for your streams using `create_kv_list` and `create_kv_set`.
- **Core RPC** — Access fundamental blockchain data, such as retrieving the most recent block number using `rpc_eth_blocknumber`.

### How it works

1. Subscribe to this server
2. Provide your QuickNode API Key and RPC URL
3. Start building and monitoring your Web3 infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Rapidly prototype and manage data pipelines without leaving the terminal or IDE.
- **Data Engineers** — Orchestrate complex blockchain data ingestion workflows using natural language commands.
- **DevOps Teams** — Monitor and update infrastructure configurations, webhooks, and streams on the fly.


## Available Tools
- **create_kv_list**: Create a new KV Store list
- **create_kv_set**: Create a KV Store key-value pair
- **create_stream**: Create a new QuickNode stream
- **create_webhook**: Create a webhook from a template
- **delete_kv_set**: Delete a KV Store key-value pair
- **delete_stream**: Delete a QuickNode stream
- **delete_webhook**: Delete a QuickNode webhook
- **get_kv_list**: Retrieve items from a KV Store list
- **get_kv_set**: Retrieve a value from KV Store sets
- **get_stream**: Retrieve details of a specific QuickNode stream
- **list_streams**: List all active QuickNode streams
- **list_webhooks**: Retrieve all QuickNode webhooks
- **rpc_eth_blocknumber**: Returns the number of the most recent block
- **rpc_eth_call**: Executes a new message call immediately without creating a transaction
- **rpc_eth_getlogs**: Returns an array of all logs matching a given filter object
- **rpc_eth_gettransactionreceipt**: Returns the receipt of a transaction by hash
- **update_kv_list**: Add or remove items from a KV Store list
- **update_stream**: Update an existing QuickNode stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuickNode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active QuickNode streams."

**🤖 AI Agent:**
> I've retrieved your streams. You have 2 active streams: 'Mainnet-Ingest' (ID: st_123) and 'Polygon-Archive' (ID: st_456). Would you like the details for one of them?

---

**👤 You:**
> "Create a new webhook for EVM wallet filtering using the template 'evmWalletFilter'."

**🤖 AI Agent:**
> I'm creating the webhook with the 'evmWalletFilter' template. Please provide the configuration JSON for the addresses you want to monitor.

---

**👤 You:**
> "What is the current block number on the network?"

**🤖 AI Agent:**
> The most recent block number on the connected network is 18,452,910.


## Installation & Usage

To install and use the **QuickNode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quicknode](https://vinkius.com/mcp/quicknode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
