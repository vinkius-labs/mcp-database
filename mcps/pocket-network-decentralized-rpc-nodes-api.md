# Pocket Network (Decentralized RPC Nodes API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pocket-network-decentralized-rpc-nodes-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pocket-network-decentralized-rpc-nodes-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pocket-network-decentralized-rpc-nodes-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access decentralized RPC nodes via Pocket Network — query accounts, blocks, nodes, and relay requests to multiple blockchains.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pocket Network (Decentralized RPC Nodes API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get account details for the POKT address 12345..."

**🤖 AI Agent:**
> I've retrieved the account details for address 12345... The current balance is 5,000 POKT and the account is currently in an 'Unstaked' state.

---

**👤 You:**
> "Show me the nodes assigned to app public key ABCDE for Ethereum (0021)."

**🤖 AI Agent:**
> Querying session details... I found 5 nodes assigned to your application for the current session on Ethereum. Would you like the specific addresses of these nodes?

---

**👤 You:**
> "Relay this RPC payload to the blockchain: { "method": "eth_blockNumber", ... }"

**🤖 AI Agent:**
> Sending relay request through Pocket nodes... The request was successful. The current block height on the target chain is 18,450,210.


## Installation & Usage

To install and use the **Pocket Network (Decentralized RPC Nodes API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pocket-network-decentralized-rpc-nodes-api](https://vinkius.com/mcp/pocket-network-decentralized-rpc-nodes-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
