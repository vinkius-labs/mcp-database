# Swan MCP Server

Empowers algorithmic control over European Bank Accounts. Execute SEPA transfers and manage Virtual Corporate Cards programmatically.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/swan)

## Overview
**Category:** money-moves
**Tools Count:** 9

## Description
The **Swan MCP Server** embeds a complete European Banking-as-a-Service architecture into Vinkius LLMs.

### What you can do

- **Automated Root Provisioning** — Instantly spin up local branch operations allocating FRA or ESP IBAN formats through `swan_create_account`.
- **Card Administration** — Ask the agent to generate custom virtual Mastercards assigned exclusively to distinct contractors utilizing `swan_add_virtual_card`.
- **Direct SEPA Execution** — Move exact funds safely parsing external creditor data natively through `swan_create_sepa_transfer` directly across European networks.

### How it works

1. Login to your Swan Partner dashboard.
2. In Developer Settings, forge a Project Access Token granting server-to-server structural authority.
3. Bind the token securely into Vinkius and set the 'sandbox' environment flag explicitly if performing simulation sweeps.

### Who is this for?

- **Agile Fintechs** — Embed full neobank ledgers natively.
- **Corporate Orchestrators** — Distribute vendor cards programmatically mitigating manual issuance risks.


## Available Tools
- **swan_add_virtual_card**: Provisions a robust Mastercard Virtual Debit
- **swan_cancel_card**: Permanently cancel a specific corporate card
- **swan_create_account**: Requires an existing AccountHolderId.

Dynamically provision a European Account under your ledger
- **swan_create_sepa_transfer**: Initiate a standard European SEPA Credit Transfer
- **swan_get_accounts**: List all operational Swan Bank Accounts/IBANs
- **swan_get_project_info**: Fetch overarching details about your connected Swan Project Node
- **swan_get_transactions**: Retrieve the ledger history for a specific Account
- **swan_list_cards**: List all physical and virtual cards
- **swan_simulate_incoming_transfer**: Sandbox Only - Inject fake money


## Installation & Usage

To install and use the **Swan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swan](https://vinkius.com/mcp/swan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
