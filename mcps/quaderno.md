# Quaderno MCP Server

Bring automated tax compliance and invoicing directly into your AI workflow — calculate global taxes, issue invoices, and manage CRM contacts in seconds.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/quaderno)

## Overview
**Category:** finance-accounting
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Quaderno** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quaderno](https://vinkius.com/mcp/quaderno)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
