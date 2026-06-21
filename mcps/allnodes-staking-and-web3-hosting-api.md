# Allnodes (Staking and Web3 Hosting API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/allnodes-staking-and-web3-hosting-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/allnodes-staking-and-web3-hosting-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/allnodes-staking-and-web3-hosting-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage staking, validators, and Web3 hosting infrastructure directly from any AI agent via Allnodes.

## Description
Connect your **Allnodes** account to any AI agent to automate your blockchain infrastructure management. Allnodes provides a non-custodial platform for staking, nodes, and hosting.

### What you can do

- **Staking & Delegations** — Monitor your staking positions and retrieve detailed delegation data across supported networks.
- **Validator Management** — List, inspect, and manage your active validators with ease.
- **Web3 Hosting** — Query available bare-metal and instant servers, or provision new hosting environments.
- **Node Operations** — Access full node metadata and perform maintenance actions like restarts directly from your conversation.
- **SSH Security** — Manage your SSH public keys to ensure secure access to your hosted infrastructure.

### How it works

1. Subscribe to this server
2. Enter your Allnodes API Token
3. Start managing your crypto infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Blockchain Developers** — Deploy and monitor nodes without leaving your IDE or terminal.
- **Crypto Investors** — Track staking rewards and validator health through natural language.
- **DevOps Engineers** — Automate server provisioning and SSH key management for Web3 stacks.


## Available Tools
- **add_ssh_key**: Add a new SSH Key
- **get_delegation**: Get a specific delegation
- **get_delegations**: Get all delegations
- **get_fullnode**: Get a specific full node
- **get_fullnodes**: Get all full nodes
- **get_instant_server_profiles**: Get all available Instant server installation profiles
- **get_instant_server_upgrades**: Get all available Instant server upgrades
- **get_instant_servers**: Get all available Instant servers
- **get_servers**: Get all bare-metal servers
- **get_ssh_keys**: Get all SSH Keys
- **get_validator**: Get a specific validator
- **get_validators**: Get all validators
- **host_instant_server**: Host an Instant server
- **host_node**: g., ETH validator, Masternode). Provide required fields based on the currency.

Host a validator or masternode
- **prepare_deterministic**: Prepare deterministic registration
- **remove_ssh_key**: Remove an SSH Key
- **remove_validator**: Remove a validator
- **restart_fullnode**: Restart a full node
- **staking_action**: g., stake, unstake, withdraw, claim) for various currencies (ETH, SOL, DOT, TRX, etc.).

Perform a staking action
- **submit_deterministic**: Submit deterministic registration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Allnodes (Staking and Web3 Hosting API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bare-metal servers on Allnodes."

**🤖 AI Agent:**
> I've retrieved your bare-metal servers. You currently have 2 active servers: 'Main-ETH-Node' (ID: srv-8821) and 'Backup-Validator' (ID: srv-9932).

---

**👤 You:**
> "What installation profiles are available for instant server ID 'srv-123'?"

**🤖 AI Agent:**
> Checking profiles for srv-123... I found 3 available profiles: 'Ubuntu 22.04 LTS', 'Debian 11', and 'CentOS Stream 9'. Which one would you like to use?

---

**👤 You:**
> "Get the details for my validator with ID 'val-888'."

**🤖 AI Agent:**
> Inspecting validator val-888... This is an Ethereum validator. Status: Active. Uptime: 99.9%. Current rewards: 1.2 ETH. Would you like to see the full metadata?


## Installation & Usage

To install and use the **Allnodes (Staking and Web3 Hosting API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/allnodes-staking-and-web3-hosting-api](https://vinkius.com/mcp/allnodes-staking-and-web3-hosting-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
