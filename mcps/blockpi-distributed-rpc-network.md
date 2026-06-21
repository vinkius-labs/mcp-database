# BlockPi (Distributed RPC Network) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blockpi-distributed-rpc-network)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/blockpi-distributed-rpc-network-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/blockpi-distributed-rpc-network-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Access distributed blockchain RPC nodes via BlockPi — monitor RU balances, track consumption, and execute JSON-RPC calls across multiple networks.

## Description
Connect your **BlockPi** account to any AI agent to manage your distributed RPC infrastructure and interact with blockchain networks directly through natural language.

### What you can do

- **Resource Monitoring** — Check your Request Unit (RU) balance and wallet balance in USD across different networks like Ethereum or Polygon.
- **Usage Analytics** — Track RU consumption over 1, 3, or 7 days to optimize your dApp's performance and infrastructure costs.
- **Package Management** — Inspect active RU packages, including SKU details, remaining amounts, and precise expiration timestamps.
- **Multi-Chain RPC** — Execute generic JSON-RPC calls (like `eth_blockNumber`, `eth_call`, or `eth_getBalance`) on Ethereum, BSC, Polygon, Solana, and more.

### How it works

1. Subscribe to this server
2. Enter your BlockPi API Key
3. Start querying blockchain data and managing your node resources from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — quickly check node health, balances, and execute RPC methods without leaving the terminal or code editor.
- **DevOps Engineers** — monitor infrastructure consumption and package expiration to ensure zero downtime for decentralized applications.
- **Data Analysts** — fetch raw blockchain data directly through natural language queries using standard RPC methods.


## Available Tools
- **rpc_call**: g., eth_blockNumber, eth_call, eth_getBalance) on the specified network.

Make a generic JSON-RPC call to a supported blockchain network
- **get_package_expiration**: Get details about active RU packages
- **get_ru_balance**: Get remaining Request Unit (RU) balance
- **get_ru_consumed**: Get RU consumption for a specific endpoint
- **get_wallet_balance**: Get remaining wallet balance in USD


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BlockPi (Distributed RPC Network)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my current RU balance and wallet balance on Ethereum."

**🤖 AI Agent:**
> I've checked your BlockPi account for the Ethereum network. You have 1,250,000 RU remaining and a wallet balance of $45.20 USD.

---

**👤 You:**
> "Show me the RU consumption for the last 3 days on Polygon."

**🤖 AI Agent:**
> In the last 3 days on the Polygon network, your endpoints have consumed a total of 450,000 RU.

---

**👤 You:**
> "Get the latest block number on Arbitrum using an RPC call."

**🤖 AI Agent:**
> Executing `eth_blockNumber` on Arbitrum... The current block height is 184,209,112.


## Installation & Usage

To install and use the **BlockPi (Distributed RPC Network)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blockpi-distributed-rpc-network](https://vinkius.com/mcp/blockpi-distributed-rpc-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
