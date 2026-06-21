# Column MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/column)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/column-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/column-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Empower your Agent to operate a chartered US bank. Create accounts, trigger wire transfers, and orchestrate paper payouts using natural text.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Column** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan our balance history within my Operational account ID. See exactly how much pure funds are settled and available for dispatch."

**🤖 AI Agent:**
> Checking your root sub-account ledgers. Account analysis verifies there is precisely $483,101.40 USD held exclusively as available limits after reconciling processing offsets.

---

**👤 You:**
> "Print out a $1,500 manual paper check paid out to 'Green Construction LLC'. Mail it to '55 Broad St, Chicago IL 60601'."

**🤖 AI Agent:**
> Check dispatched officially internally! Column array verifies that a routing print queue has secured the $1500 sum from your initial DDA account. It is poised for standard post-office tracking.

---

**👤 You:**
> "Initialize a Same-Day direct ACH batch targeting our landlord accounting info. Execute a $5,000 push towards Counterparty Router 02844 under entity RentalCorp."

**🤖 AI Agent:**
> Direct ACH operation generated natively. The target identifier '02844' has successfully been locked onto and 5,000 cents equivalents dispatched along standard US Clearing timelines.


## Installation & Usage

To install and use the **Column** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/column](https://vinkius.com/mcp/column)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
