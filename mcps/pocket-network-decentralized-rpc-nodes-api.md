# Pocket Network (Decentralized RPC Nodes API) MCP Server

Access decentralized RPC nodes via Pocket Network — query accounts, blocks, nodes, and relay requests to multiple blockchains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pocket-network-decentralized-rpc-nodes-api)

## Overview
**Category:** developer-tools
**Tools Count:** 7

## Description
Connect your AI agent to the **Pocket Network** decentralized infrastructure to interact with blockchain data and RPC nodes through a single MCP interface.

### What you can do

- **Relay Requests** — Send RPC requests to external blockchains through decentralized Pocket nodes using the `relay_request` tool.
- **Network Inspection** — Query the state of accounts, specific blocks, and individual nodes directly on the Pocket Network.
- **App & Session Management** — Retrieve application details and identify the specific set of nodes assigned to an app for any given session.
- **Transaction Submission** — Submit signed transactions (staking, transfers) directly to the network via `submit_transaction`.

### How it works

1. Subscribe to this server
2. Enter your Pocket Node URL (POCKET_NODE_URL)
3. Start querying decentralized infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — interact with multiple chains without relying on centralized RPC providers
- **Node Operators** — monitor node status and network blocks directly from the terminal or AI chat
- **DApp Builders** — automate session checks and relay testing during the development lifecycle


## Available Tools
- **get_account**: Get Pocket Network account details
- **get_app**: Get Pocket Network app details
- **get_block**: Get Pocket Network block details
- **get_node**: Get Pocket Network node details
- **relay_request**: Requires payload, meta, and proof objects.

Send a relay request to an external blockchain
- **get_session**: Get Pocket Network session details
- **submit_transaction**: g., staking, sending POKT) to the network.

Submit a transaction to the Pocket Network


## Installation & Usage

To install and use the **Pocket Network (Decentralized RPC Nodes API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pocket-network-decentralized-rpc-nodes-api](https://vinkius.com/mcp/pocket-network-decentralized-rpc-nodes-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
