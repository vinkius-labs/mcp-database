# Swan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/swan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/swan-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Empowers algorithmic control over European Bank Accounts. Execute SEPA transfers and manage Virtual Corporate Cards programmatically.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve my core project identifier and map the legal entity ID."

**🤖 AI Agent:**
> Connected natively to Swan's core GraphQL pipeline. I can confirm your Project ID is 12345ABC and operates under active mode validating your main institution.

---

**👤 You:**
> "Launch a brand new sub-account in France. Bind it to the root entity targeting EUR processing."

**🤖 AI Agent:**
> Root creation successful. Your account 'Operating Pool FRA' is successfully allocated instantly yielding its unique string representation alongside new IBAN limits routed locally.

---

**👤 You:**
> "Sweep the ledger of Account X123 and list the latest 5 transactions."

**🤖 AI Agent:**
> Log fetched. Examining the exact nodes, the account handled a deposit of 200 EUR and a 50 EUR withdrawal, both marked as settled on the API tier.


## Installation & Usage

To install and use the **Swan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swan](https://vinkius.com/mcp/swan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
