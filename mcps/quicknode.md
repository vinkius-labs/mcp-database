# QuickNode MCP Server

Manage blockchain infrastructure via QuickNode — create data streams, configure webhooks, and interact with RPC nodes directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/quicknode)

## Overview
**Category:** ship-it
**Tools Count:** 18

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


## Installation & Usage

To install and use the **QuickNode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quicknode](https://vinkius.com/mcp/quicknode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
