# DebtPayPro MCP Server

Equip your AI agent to manage contacts, track payments, and monitor sales opportunities via the DebtPayPro API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/debtpaypro)

## Overview
**Category:** sales-automation
**Tools Count:** 10

## Description
Integrate **DebtPayPro**, the specialized CRM for the debt settlement and financial services industry, directly into your AI workflow. Manage your customer database, track scheduled payments and debt portfolios, and monitor sales opportunities using natural language.

### What you can do

- **Contact Management** — List and retrieve detailed profiles for your CRM contacts and leads.
- **Payment Tracking** — Monitor payment history and upcoming scheduled payments for specific clients.
- **Debt Portfolio Oversight** — List and review debts associated with your contacts.
- **Sales & Task Monitoring** — Track active sales opportunities and manage pending CRM tasks and follow-ups.

### How it works

1. Connect the DebtPayPro integration to your AI assistant.
2. Authorize using your DebtPayPro API Key (found in your admin settings).
3. Optimize your debt settlement operations through intuitive conversation.

### Who is this for?

- **Debt Settlement Agents** — Quickly check client balances and payment statuses on the go.
- **Compliance Officers** — Audit contact profiles and debt records via chat.
- **Sales Managers** — Monitor lead pipelines and team task completion during planning.


## Available Tools
- **create_new_contact**: Persists a new contact record with the provided name and email, returning the newly generated system ID.

Add a new contact to the DebtPayPro database
- **get_account_details**: Returns account-level metadata such as company name, API permissions, and system version.

Retrieve metadata for your DebtPayPro account
- **get_contact_details**: Resolves demographic data, associated case numbers, and the current status of their debt settlement program.

Get detailed profile information for a specific contact
- **list_crm_contacts**: Returns contact metadata including system IDs, names, and primary contact information.

List all contacts in your DebtPayPro CRM
- **list_contact_debts**: Returns a list of enrolled debts, including creditor names, original balances, and current settlement status.

List all debts associated with a specific contact
- **list_sales_opportunities**: Returns a list of active opportunities including projected case value, current stage in the sales cycle, and assigned sales representative.

List active sales opportunities and leads
- **list_contact_payments**: Returns a history of processed payments and a schedule of future installments towards their debt settlement plan.

List payment history and scheduled payments for a contact
- **list_crm_tasks**: Returns task descriptions, due dates, and associated contact or case identifiers.

List pending tasks and follow-ups in the system
- **list_upcoming_payments**: Returns upcoming transaction metadata for proactive account management.

List payments scheduled for the next 7 days (mock logic)
- **search_contacts_by_name**: Matches the search term against names and email addresses using partial case-insensitive matching.

Search for a contact by name or email keyword


## Installation & Usage

To install and use the **DebtPayPro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/debtpaypro](https://vinkius.com/mcp/debtpaypro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
