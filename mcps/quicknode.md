# QuickNode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/quicknode)
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


## Available Tools (18)
- **delete_stream**: Ensure the provided Stream ID is correct.

Delete a QuickNode stream
- **create_stream**: Create a new QuickNode stream
- **create_webhook**: Create a webhook from a template
- **list_webhooks**: Retrieve all QuickNode webhooks
- **update_kv_list**: Must specify a key and either add or remove items.

Add or remove items from a KV Store list
- **create_kv_list**: Create a new KV Store list
- **create_kv_set**: Both the key and value must be provided.

Create a KV Store key-value pair
- **delete_kv_set**: Specify the key to be removed.

Delete a KV Store key-value pair
- **delete_webhook**: Use the unique Webhook ID for deletion.

Delete a QuickNode webhook
- **get_kv_list**: Specify the key of the list to query.

Retrieve items from a KV Store list
- **get_kv_set**: Provide the key associated with the desired value.

Retrieve a value from KV Store sets
- **get_stream**: Provide a valid Stream ID.

Retrieve details of a specific QuickNode stream
- **list_streams**: Do not attempt to list non-existent streams.

List all active QuickNode streams
- **rpc_eth_blocknumber**: This tool requires no input parameters.

Returns the number of the most recent block
- **rpc_eth_call**: Provide the transaction object and block number.

Executes a new message call immediately without creating a transaction
- **rpc_eth_getlogs**: Provide a filter object JSON string.

Returns an array of all logs matching a given filter object
- **rpc_eth_gettransactionreceipt**: Provide a valid transaction hash as input.

Returns the receipt of a transaction by hash
- **update_stream**: Must provide both a Stream ID and at least one update parameter.

Update an existing QuickNode stream


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


## ❓ FAQ

**Q: How do I check the current block height on Ethereum?**
You can use the `rpc_eth_blocknumber` tool. It will return the most recent block number from the blockchain network connected to your RPC URL.

**Q: Can I create a stream to monitor specific blockchain datasets?**
Yes, use the `create_stream` tool. You can specify the dataset (e.g., 'block', 'traces') and the destination (e.g., 'webhook', 's3') to start ingesting data immediately.

**Q: How do I manage lists for my stream filters?**
Use the `create_kv_list` tool to initialize a list and `update_kv_list` to add or remove items. These lists can be referenced in your Streams JavaScript filter functions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/quicknode](https://vinkius.com/en/ai-agent-connect/quicknode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QuickNode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quicknode` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QuickNode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quicknode": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
