# Biconomy (Account Abstraction) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/biconomy-account-abstraction)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/biconomy-account-abstraction-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/biconomy-account-abstraction-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Simplify blockchain interactions with Account Abstraction — get quotes, execute supertransactions, and track status via Biconomy.

## Description
Connect your **Biconomy** developer account to any AI agent to streamline Web3 operations through Account Abstraction. This server enables agents to handle complex on-chain flows with ease.

### What you can do

- **Supertransaction Quotes** — Generate optimized quotes for complex transaction flows, including gasless (sponsored) options using the `get_quote` tool.
- **Transaction Execution** — Submit signed payloads for execution on-chain via Biconomy's robust infrastructure using `execute_supertx`.
- **Status Tracking** — Monitor the real-time progress of your Supertransactions using the `get_explorer_status` tool.
- **Flexible Account Modes** — Full support for Smart Accounts, EOA, and EOA-7702 account modes.

### How it works

1. Subscribe to this server
2. Enter your Biconomy API Key
3. Start orchestrating Web3 intents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Rapidly prototype and test complex transaction flows without manual script writing.
- **dApp Operators** — Automate maintenance tasks and user operations using natural language.
- **DeFi Power Users** — Execute multi-step transactions with optimized gas and simplified signing.


## Available Tools
- **execute_supertx**: Requires the full quote object with signatures added to payloadToSign.

Execute a signed Supertransaction
- **get_explorer_status**: Track the execution status of a Supertransaction
- **get_quote**: Get a Supertransaction quote from Biconomy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Biconomy (Account Abstraction)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a quote for a smart-account transaction for owner 0x123... with a simple intent flow."

**🤖 AI Agent:**
> I've generated the Supertransaction quote. The optimal route has been identified. You can now sign the payload for execution. Would you like to see the fee details?

---

**👤 You:**
> "Execute this signed supertransaction: [JSON payload]"

**🤖 AI Agent:**
> Submitting the Supertransaction to Biconomy... Execution started! Your Supertransaction Hash is 0xabc... You can use this hash to track the status.

---

**👤 You:**
> "Check the status of supertransaction 0xabc123..."

**🤖 AI Agent:**
> The Supertransaction 0xabc123... is currently 'Success'. It has been confirmed on-chain. You can view the full details in the Biconomy explorer.


## Installation & Usage

To install and use the **Biconomy (Account Abstraction)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/biconomy-account-abstraction](https://vinkius.com/mcp/biconomy-account-abstraction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
