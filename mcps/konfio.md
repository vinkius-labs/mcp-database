# Konfío MCP Server

Automate your Konfío SMB banking and lending. Manage loans, pay invoices, track credit cards, and emit SAT-compliant CFDIs directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/konfio)

## Overview
**Category:** money-moves
**Tools Count:** 14

## Description
Connect your **Konfío** business account to any AI agent and manage Mexico's leading SMB financial suite through natural conversation. Whether you need to pay a loan, check credit limits, or emit electronic invoices (CFDIs), the AI handles the heavy lifting.

### What you can do

- **Loan Management** — Track active business loans, get amortization schedules, and make direct loan payments from your connected accounts
- **Credit Cards** — Review corporate credit card spending, check available limits, and fetch monthly statements for reconciliation
- **Electronic Invoicing (CFDI 4.0)** — List emitted and received SAT invoices, and generate new legally compliant invoices with automatic stamp generation
- **B2B Transfers** — Create SPEI transfers to suppliers and employees directly from your Konfío account
- **Credit Line Monitoring** — Check your business credit score status and apply for new working capital credit lines

### How it works

1. Subscribe to this server
2. Enter your Konfío Business API credentials
3. Start managing your PYME finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SMB Owners (PYMEs)** — monitor cash flow and loan balances without opening multiple banking apps
- **Accountants** — programmatically pull CFDI invoices and credit card transactions for end-of-month reconciliation
- **Finance Teams** — automate supplier SPEI transfers and invoice generation


## Available Tools
- **check_credit_status**: Check business credit rating and eligibility status
- **create_invoice**: 0 invoice for a client. Requires client RFC, tax regime, items, and CFDI usage code.

Create and emit a new electronic invoice (CFDI)
- **create_transfer**: Create a supplier B2B transfer (SPEI)
- **get_business_profile**: Get Konfío business profile
- **get_cc_statement**: Get a credit card monthly statement
- **get_credit_card**: Get business credit card details
- **get_loan_details**: Get details of a specific business loan
- **get_payment_schedule**: Get the amortization schedule for a loan
- **list_cc_transactions**: List credit card transactions
- **list_invoices**: You can filter by issued (emitted) or received invoices.

List electronic invoices (CFDIs)
- **list_loans**: List active and past business loans
- **list_transfers**: List B2B outgoing wire transfers
- **make_loan_payment**: Make a payment towards a business loan
- **request_credit_line**: Submit a new credit line request


## Installation & Usage

To install and use the **Konfío** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/konfio](https://vinkius.com/mcp/konfio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
