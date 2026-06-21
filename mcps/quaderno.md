# Quaderno MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quaderno)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/quaderno-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/quaderno-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Bring automated tax compliance and invoicing directly into your AI workflow — calculate global taxes, issue invoices, and manage CRM contacts in seconds.

## Description
Connect your **Quaderno** account to any AI agent and bring powerful tax compliance, invoicing, and customer management capabilities directly into your automated workflows.

### What you can do

- **Tax Calculations on the Fly** — Instantly determine the accurate sales tax, VAT, or GST based on the customer's region and amount before finalizing sales logic
- **Invoice Management** — Search and retrieve generated invoices, audit billing records, and verify transactions perfectly formatted via intelligent prompts
- **Generate Transactions** — Transact and issue invoices seamlessly by sending a simple JSON array of itemized products and line item prices
- **Full Contact CRM** — Map your users fully by creating, modifying, retrieving, and safely deleting user contacts and billing profiles natively

### How it works

1. Subscribe to this server
2. Authorize using your Quaderno Account API URL and unique API Key
3. Start querying customer billing and global taxes from Claude, Cursor, or any MCP-compatible wrapper

### Who is this for?

- **E-Commerce Founders** — prompt your AI to check what taxes apply to a specific customer base during a new global promotion launch
- **Finance Engineers** — instantly look up invoices by contact ID while coding billing webhooks, avoiding dashboard fatigue
- **Client Success Managers** — edit a mispelled client billing address rapidly mid-conversation before generating a new transaction record


## Available Tools
- **calculate_taxes**: Calculates applicable taxes for a potential sale
- **create_contact**: Specify email, first name, and last name.

Creates a new contact in Quaderno
- **create_transaction**: Provide the contact ID and a JSON array of items.

Records a new transaction and issues an invoice
- **delete_contact**: This action is irreversible.

Deletes a contact from Quaderno
- **get_contact**: Retrieves details for a specific contact
- **get_invoice**: Retrieves details for a specific invoice
- **list_contacts**: Lists all contacts (customers) in the Quaderno account
- **list_invoices**: Lists all issued invoices
- **list_transactions**: Lists all recorded transactions
- **update_contact**: Provide a JSON payload with the changes.

Updates an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quaderno** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the taxes for a $150 plan sold to a user in Berlin, Germany (Postal Code 10115)."

**🤖 AI Agent:**
> Based on Quaderno's calculation (`calculate_taxes` tool), applying the standard DE tax rate (19% VAT) to the $150 amount adds $28.50 in taxes. The final user total will be $178.50. Would you like to create a transaction with these exact amounts?

---

**👤 You:**
> "Fetch the billing details and history for contact ID #9822."

**🤖 AI Agent:**
> Contact #9822 is Acorn Corp (acorn-billing@example.com). They are located in NY, USA. Their VAT profile is clean. Would you like me to use `list_invoices` to find all recent transactions associated with their profile?

---

**👤 You:**
> "Update contact #9822 to change its first name to 'Acorn Group Inc'."

**🤖 AI Agent:**
> I've processed the `update_contact` request. The first_name field on contact #9822 has been successfully patched to 'Acorn Group Inc'. Their records are fully refreshed.


## Installation & Usage

To install and use the **Quaderno** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quaderno](https://vinkius.com/mcp/quaderno)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
