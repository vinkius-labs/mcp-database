# Fireblocks MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fireblocks)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fireblocks-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fireblocks-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Securely manage digital assets, vault accounts, and blockchain transactions via the Fireblocks Digital Asset Platform directly from your AI agent.

## Description
Connect your **Fireblocks** workspace to any AI agent to orchestrate institutional-grade digital asset operations through natural language conversation.

### What you can do

- **Vault Management** — List, create, and inspect vault accounts and asset balances across your entire organization.
- **Transaction Orchestration** — Create, estimate fees, and monitor transactions across multiple blockchains with full lifecycle control.
- **Wallet Connectivity** — Manage internal and external wallets, and generate new deposit addresses for various assets.
- **Advanced Asset Support** — Interact with NFTs, staking positions, and smart contracts directly from the console.
- **Compliance & Security** — Validate travel rules, manage gas station settings, and retrieve screening information for transactions.

### How it works

1. Subscribe to this server
2. Enter your Fireblocks API Key and Private Key
3. Start managing your digital asset infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Treasury Managers** — instantly check balances across hundreds of vaults and initiate transfers without manual dashboard navigation.
- **DevOps Engineers** — automate the creation of vault accounts and deposit addresses during deployment workflows.
- **Compliance Officers** — quickly retrieve screening results and validate travel rule data for specific transactions.


## Available Tools
- **add_asset_to_wallet**: Add an asset/address to a wallet
- **add_contract**: Add a new contract to the whitelist
- **cancel_transaction**: Cancel a pending transaction
- **create_external_wallet**: Create a new external wallet container
- **create_internal_wallet**: Create a new internal wallet container
- **create_transaction**: Create a new transaction (Transfer, Mint, Burn, etc.)
- **create_vault_account_asset_address**: Generate a new deposit address
- **create_vault_account_asset**: Create a new wallet for an asset in a vault
- **create_vault_account**: Create a new vault account
- **create_webhook**: Create a new webhook subscription
- **drop_transaction**: Drop an ETH/EVM transaction
- **estimate_fee**: Estimate fees for a potential transaction
- **estimate_network_fee**: Get current network fee estimates for an asset
- **get_contract_asset**: Get details for a contract asset
- **get_gas_station**: Retrieve gas station settings
- **get_public_key_info**: Get the public key for a specific derivation path
- **get_screening_transaction**: Get compliance screening results for a transaction
- **get_transaction**: Get details of a specific transaction
- **get_vault_account_asset**: Get balance for a specific asset in a vault
- **get_vault_account**: Retrieve details for a specific vault account
- **list_assets**: List all supported assets
- **list_blockchains**: List all supported blockchains
- **list_contracts**: List whitelisted contracts
- **list_external_wallets**: List all external wallets
- **list_internal_wallets**: List all internal wallets
- **list_owned_nfts**: List all owned NFT tokens
- **list_staking_chains**: List supported staking chains
- **list_staking_positions**: List active staking positions
- **list_transactions**: Retrieve transaction history with filters
- **list_vasps**: List Virtual Asset Service Providers (VASPs)
- **list_vault_account_asset_addresses**: List deposit addresses for an asset
- **list_vault_accounts**: List vault accounts with pagination
- **list_webhook_notifications**: List notifications sent to a webhook
- **refresh_nfts**: Refresh NFT data for a vault account
- **register_asset**: Register a custom asset (e.g., ERC-20)
- **resend_webhooks**: Resend failed webhooks
- **stake_position**: Initiate a staking position
- **update_gas_station**: Update auto-fueling thresholds
- **update_vault_account**: Rename a vault account
- **validate_travel_rule**: Validate a transaction against Travel Rule requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fireblocks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 vault accounts in my Fireblocks workspace."

**🤖 AI Agent:**
> I've retrieved your vault accounts. You have 'Main Vault' (ID: 0), 'Staking-ETH' (ID: 5), and 'Trading-Hot' (ID: 12) among others. Would you like to see the asset balances for any of these?

---

**👤 You:**
> "What is the BTC balance in vault account ID 0?"

**🤖 AI Agent:**
> In vault account 0 (Main Vault), the BTC balance is 1.45 BTC available, with a total balance of 1.50 BTC (0.05 BTC pending).

---

**👤 You:**
> "Create a transaction to send 0.1 ETH from vault 0 to external wallet 'Exchange-Wallet'."

**🤖 AI Agent:**
> I've initiated the transaction request. Transaction ID: tx-98765. The status is currently 'SUBMITTED' and is awaiting approval in your Fireblocks console.


## Installation & Usage

To install and use the **Fireblocks** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fireblocks](https://vinkius.com/mcp/fireblocks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
