# Column MCP Server

Empower your Agent to operate a chartered US bank. Create accounts, trigger wire transfers, and orchestrate paper payouts using natural text.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/column)

## Overview
**Category:** money-moves
**Tools Count:** 12

## Description
The **Column MCP Server** effectively bypasses standard FinTech wrappers and ties your artificial intelligence directly to one of the only nationally chartered US banks built originally around raw Developer APIs.

### What you can do

- **Automated Clearing** — Use `column_create_ach_transfer` to reliably settle recurring vendor payouts directly out of your native balance without relying on external UI web panels.
- **Establish Corporate Entities** — Hook your conversational bots to construct KYC/KYB verified operational clusters `column_create_entity` ready to map against newly minted bank account numbers (`column_create_bank_account`).
- **Physical Check Writing** — Astonishing API feature: send literal paper checks natively out to US addresses. Formulate text like "Mail a $40 check to John's address in Texas for maintenance" and the `column_create_check` prints and bounds the ledger payload directly.

### How it works

1. Sign up onto the Column Bank developer web-app.
2. In your security setup, obtain your developer `API Key` token string which doubles inherently as basic auth credentials internally.
3. Integrate the token strictly into the application parameters right here inside the MCP interface.

### Who is this for?

- **Hardcore FinOps** — Handle heavy capital movement routing arrays entirely via deterministic Agent actions scaling limitlessly.
- **Property / Payroll Managers** — Rapidly push independent paper checks leveraging address endpoints via chat interfaces.


## Available Tools
- **column_create_ach_transfer**: Fire an ACH to an external routing/account number
- **column_create_bank_account**: Establish a DDA (Demand Deposit Account)
- **column_create_check**: Very useful for legacy vendor systems.

Generate and mail a paper check
- **column_create_entity**: In production, this goes through compliance screening.

Register a business or person KYC target inside Column
- **column_create_wire_transfer**: Fire an immediate Wire transfer
- **column_get_balance**: Audit settled funds inside a Bank Account
- **column_get_bank_account**: Fetch specific DDA details (Routing info)
- **column_get_statement**: Retrieve the generated bank statement artifacts
- **column_list_entities**: View all active KYC profiles under the charter
- **column_list_transfers**: Sweep historical ACH payment operations
- **column_list_webhooks**: View all registered listening streams
- **column_simulate_ach**: Trigger Sandbox inbound money movement


## Installation & Usage

To install and use the **Column** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/column](https://vinkius.com/mcp/column)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
