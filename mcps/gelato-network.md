# Gelato Network MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gelato-network)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gelato-network-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gelato-network-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate Web3 transactions via Gelato — relay transactions, manage ERC-4337 UserOperations, and get real-time gas estimates across multiple chains.

## Description
Connect your **Gelato Network** account to any AI agent and automate complex Web3 infrastructure workflows through natural conversation. Gelato provides the ultimate reliability for transaction relaying and account abstraction.

### What you can do

- **Transaction Relaying** — Submit signed transactions for relaying on various chains, supporting both asynchronous and synchronous (wait-for-inclusion) modes.
- **Account Abstraction (ERC-4337)** — Submit and estimate gas for UserOperations using Gelato's high-performance Bundler.
- **Real-time Status Tracking** — Monitor the lifecycle of your relayed tasks using unique task IDs to ensure successful on-chain execution.
- **Gas & Fee Intelligence** — Retrieve token exchange rates, gas price data, and precise fee quotes for specific gas amounts and tokens.
- **Chain Capabilities** — Query supported payment tokens and fee collector addresses for any supported blockchain network.

### How it works

1. Subscribe to this server
2. Enter your Gelato API Key
3. Start automating your Web3 operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — integrate gasless transactions and account abstraction directly from your coding environment.
- **DevOps Engineers** — monitor transaction statuses and manage infrastructure costs without leaving the terminal.
- **Protocol Teams** — automate fee calculations and transaction relaying for cross-chain operations.


## Available Tools
- **bundler_estimate_user_operation_gas**: Estimate gas for a UserOperation
- **bundler_get_user_operation_by_hash**: Retrieve UserOperation details by hash
- **bundler_get_user_operation_gas_price**: Get current gas prices for UserOperations
- **bundler_get_user_operation_receipt**: Get the receipt of a UserOperation
- **bundler_send_user_operation**: Submit an ERC-4337 UserOperation
- **bundler_supported_entry_points**: List supported EntryPoint addresses
- **relayer_get_capabilities**: Get supported payment tokens and fee collectors
- **relayer_get_fee_data**: Get token exchange rates and gas price data
- **relayer_get_fee_quote**: Get a fee quote for a specific gas amount
- **relayer_get_status**: Check the status of a relayed transaction
- **relayer_send_transaction_sync**: Submit a transaction and wait for inclusion
- **relayer_send_transaction**: Returns a unique 32-byte task ID for tracking.

Submit a signed transaction for relaying


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gelato Network** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Relay this signed transaction data to address 0x123... on Polygon (chainId 137)."

**🤖 AI Agent:**
> I've submitted the transaction to Gelato Relayer. Your Task ID is 0xabc123... You can check its status anytime using this ID.

---

**👤 You:**
> "What is the current status of Gelato task 0x550e8400-e29b-41d4-a716-446655440000?"

**🤖 AI Agent:**
> The task is currently 'ExecSuccess'. It was included in block 1523421. Would you like to see the full transaction receipt?

---

**👤 You:**
> "Estimate gas for this UserOperation on Optimism (chainId 10)."

**🤖 AI Agent:**
> I've calculated the gas limits for your UserOperation on Optimism. The estimated callGasLimit is 45000 and verificationGasLimit is 120000.


## Installation & Usage

To install and use the **Gelato Network** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gelato-network](https://vinkius.com/mcp/gelato-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
