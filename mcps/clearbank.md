# ClearBank MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clearbank)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clearbank-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clearbank-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Empowers algorithmic control over UK Payment Clearing. Execute massive Digital-Signature encrypted transaction structures natively.

## Description
The **ClearBank MCP Server** wraps incredibly defensive digital signatures (RSA-SHA256 PEM) autonomously underneath a native Language Model Chat interface. Meaning, your AI has programmatic limits to fire secure European and British payment rails on command natively.

### Core Functionality

- **Virtual Account Provisioning** — Manage deeply nested multi-layered B2B structures. Automatically provision Sort-Code ledgers via `clearbank_create_account`.
- **Payment Initiation (FPS & CHAPS)** — Run automated payroll or contractor compensation using direct clearing paths via `clearbank_create_faster_payment`.
- **Algorithmic Tracing** — Check real-time payment states organically utilizing `clearbank_get_payment_status`.

### How it works

1. From your ClearBank Institution interface, spawn your API Profile and export a standard RSA `.pem` private key.
2. Vinkius natively utilizes the `CLEARBANK_PRIVATE_KEY` constructing Cryptographic Hashes generating RSA Digital Signatures implicitly on every Chat-driven Tool call to authenticate accurately with clearing servers.

### Use Cases

- **Baas Platforms** — Direct integration validating funds exactly when needed under FPS limits.
- **Treasury Automation** — Have the Agent review your high-volume clearing state.


## Available Tools
- **clearbank_create_account**: Provision a new virtual UK Account
- **clearbank_create_chaps_payment**: Can only be done during BofE operating hours.

Dispatch a CHAPS High-Value Wire
- **clearbank_create_faster_payment**: Dispatch an instant UK Faster Payment
- **clearbank_get_account_balances**: Assess live balances for a specific account
- **clearbank_get_accounts**: List all internal ClearBank ledgers
- **clearbank_get_payment_status**: Inspect if an FPS or CHAPS instruction settled
- **clearbank_get_transactions**: View deep transaction logs of the Account
- **clearbank_suspend_account**: Immediately freeze an Account preventing transfers out/in


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClearBank** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check our main UK sub-account. View the balances mapped onto it to find liquid limits."

**🤖 AI Agent:**
> Ledger analysis received intact from the ClearBank engine. Validating Account limits, your latest pool exposes a highly liquid GBP availability with 0 reserves held.

---

**👤 You:**
> "Initialize an FPS transfer. Send £1,500 from Account 'ACC-12' natively to sort code '404040' account '12341234'."

**🤖 AI Agent:**
> Faster Payment routed through Clearing nodes flawlessly via keys validating successful message verification! Target beneficiary successfully received the £1500 liquid push across ClearBank's live FPS.

---

**👤 You:**
> "Suspend suspicious account ID ACC-99 via API."

**🤖 AI Agent:**
> Account ACC-99 has been updated. The operational status returned Suspended, freezing future payouts seamlessly.


## Installation & Usage

To install and use the **ClearBank** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clearbank](https://vinkius.com/mcp/clearbank)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
