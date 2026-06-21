# Biconomy (Account Abstraction) MCP Server

Simplify blockchain interactions with Account Abstraction — get quotes, execute supertransactions, and track status via Biconomy.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/biconomy-account-abstraction)

## Overview
**Category:** developer-tools
**Tools Count:** 3

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


## Installation & Usage

To install and use the **Biconomy (Account Abstraction)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/biconomy-account-abstraction](https://vinkius.com/mcp/biconomy-account-abstraction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
