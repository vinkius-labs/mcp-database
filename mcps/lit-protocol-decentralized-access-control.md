# Lit Protocol (Decentralized Access Control) MCP Server

Manage decentralized access control, Programmable Key Pairs (PKPs), and execute immutable Lit Actions within TEEs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lit-protocol-decentralized-access-control)

## Overview
**Category:** security-compliance
**Tools Count:** 20

## Description
Connect to **Lit Protocol** to orchestrate decentralized identity and access control. This server allows your AI to manage Programmable Key Pairs (PKPs), organize them into groups, and execute secure Lit Actions.

### What you can do

- **Account Management** — Create accounts, verify existence, and manage scoped usage API keys for secure day-to-day operations.
- **Programmable Key Pairs (PKP)** — Generate and list decentralized wallets (PKPs) owned by your account to act as distributed identities.
- **Access Control Groups** — Create groups, add/remove PKPs, and manage permissions for complex decentralized access schemas.
- **Lit Actions** — Register and execute immutable JavaScript programs inside Trusted Execution Environments (TEEs) using IPFS CIDs or inline code.
- **Security & Permissions** — Update usage key scopes and manage action-to-group mappings dynamically to ensure granular control.

### How it works

1. Subscribe to this server
2. Enter your Lit Protocol API Key
3. Start managing decentralized keys and executing secure actions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — automate the management of PKPs and Lit Actions without leaving your development environment.
- **Security Engineers** — audit access control groups and manage usage keys through natural language queries.
- **dApp Builders** — quickly test and execute Lit Actions in TEEs to verify decentralized logic.


## Available Tools
- **add_action_to_group**: Add an IPFS CID to a group
- **add_action**: Register a standalone action (name + CID)
- **add_group**: Create a new group
- **add_pkp_to_group**: Add a PKP to a specific group
- **add_usage_api_key**: Create a scoped usage key
- **check_account_exists**: Verify if an account exists for the provided API key
- **confirm_payment**: Finalize credit top-up after payment
- **create_account**: Create a new Lit account
- **create_payment_intent**: Create a Stripe PaymentIntent (min $5.00)
- **create_wallet**: Request a new PKP for the account
- **execute_lit_action**: Provide either code or ipfs_id.

Execute a Lit Action
- **get_billing_balance**: Check credit balance
- **list_actions**: List registered actions
- **list_api_keys**: List usage keys (metadata only)
- **list_groups**: List all groups
- **list_wallets**: List all PKPs owned by the account
- **remove_group**: Delete a group
- **remove_pkp_from_group**: Remove a PKP from a group
- **remove_usage_api_key**: Delete a usage key
- **update_usage_api_key**: Update permissions for a usage key


## Installation & Usage

To install and use the **Lit Protocol (Decentralized Access Control)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lit-protocol-decentralized-access-control](https://vinkius.com/mcp/lit-protocol-decentralized-access-control)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
