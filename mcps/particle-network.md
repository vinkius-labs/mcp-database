# Particle Network MCP Server

Manage Web3 infrastructure via Particle Network — handle Account Abstraction, UserOperations, and identity management directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/particle-network)

## Overview
**Category:** developer-tools
**Tools Count:** 16

## Description
Connect your **Particle Network** project to any AI agent to streamline your Web3 development and user management workflows. This server provides comprehensive tools for Account Abstraction (AA), Bundler operations, and identity verification.

### What you can do

- **User Identity** — Retrieve detailed user profiles using UUIDs, tokens, or social identities (JWT/UID) and verify project membership.
- **Account Abstraction** — Fetch smart account details (Biconomy, Simple, etc.) and manage session keys for seamless UX.
- **UserOperations** — Construct, estimate gas, and send UserOperations (UserOps) across multiple EVM chains.
- **Bundler & Paymaster** — Access bundler services for transaction receipts and use Paymaster tools to sponsor gas fees or check balances.
- **Chain Support** — Interact with various EVM-compatible chains and Solana for address verification.

### How it works

1. Subscribe to this server
2. Enter your Particle Project Server Key
3. Start orchestrating your Web3 backend from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — quickly debug UserOperations and check smart account states without manual RPC calls.
- **DApp Architects** — simulate gas fees and verify session key validity during the design phase.
- **DevOps & Support** — inspect user identities and project associations to resolve integration issues faster.


## Available Tools
- **aa_create_sessions**: Generates transactions to initialize session keys
- **aa_create_user_op**: Constructs a UserOperation from transactions
- **aa_get_fee_quotes**: Returns UserOp objects for different gas payment methods
- **aa_get_smart_account**: Get smart account info (BICONOMY, SIMPLE, etc)
- **aa_send_user_op**: Pushes a signed UserOperation to the network
- **aa_validate_session**: Checks the validity of a session key
- **eth_estimate_user_operation_gas**: Returns gas estimates for a UserOp
- **eth_get_user_operation_by_hash**: Returns UserOp details by its hash
- **eth_get_user_operation_receipt**: Retrieves the receipt of a UserOp
- **eth_send_user_operation**: Submits a UserOperation to the bundler
- **eth_supported_entry_points**: Returns supported EntryPoint addresses
- **get_user_info_by_identity**: Retrieve user details using a social identity
- **get_user_info**: Retrieve user details using UUID and Token
- **is_project_user**: Check if a wallet address belongs to a user in your project
- **pm_paymaster_balance**: Returns the USD balance of the project's Paymaster
- **pm_sponsor_user_operation**: Returns a Paymaster signature for sponsorship


## Installation & Usage

To install and use the **Particle Network** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/particle-network](https://vinkius.com/mcp/particle-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
