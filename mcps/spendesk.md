# Spendesk MCP Server

Empower your AI with real-time spend management. Track budgets, audit invoices, and review expense claims directly from your IDE.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/spendesk)

## Overview
**Category:** money-moves
**Tools Count:** 9

## Description
Bring your **Spendesk** financial operations natively into your AI workspace. Eliminate constant tab switching to check the finance dashboard. You can now use conversational prompts to audit real-time company expenses, verify specific payment IDs, and inspect active supplier invoices while writing your integration code or managing operational scripts.

### What you can do

- **Track Cash Flow** — Monitor organizational outflows by executing `list_payments`. Need deep details on a specific transaction? Pull exactly what happened using `get_payment_details`
- **Audit Invoices & Expenses** — Keep track of pending vendor bills via `list_invoices` and review employee out-of-pocket reimbursements triggering `list_expense_claims`
- **Supplier Management** — Check your registered vendor matrix using `list_suppliers` and pull contact or payment history directly calling `get_supplier_details`
- **Control Limits** — Actively supervise remaining budget allocations calling `list_budgets` and watch the assigned corporate limits on issued plastic/virtual via `list_cards`

### How it works

1. Subscribe to this AI integration server
2. Introduce your official Spendesk Access Token
3. Start using Claude, Cursor, or your terminal IDE to query financial states autonomously

Stop managing financial syncs blindly and asking accountants to pull limits. Let your local AI understand your company's real-time spending constraints directly before triggering automated actions.

### Who is this for?

- **Finance Engineers** — test accounting webhooks or integrations reading live Spendesk data intuitively through pure conversational chat formats
- **Operation Managers** — use an agent to build quick markdown summaries on active budgets or compile how much a specific team spent on software this month
- **Founders & Admins** — query team members (`list_members`) or verify immediately if a virtual card (`list_cards`) has enough cap for a high-value purchase without logging in


## Available Tools
- **get_payment_details**: Get detailed information about a specific payment
- **get_supplier_details**: Get detailed information about a specific supplier
- **list_budgets**: List all budgets and their spending status
- **list_cards**: List all virtual and physical cards issued
- **list_expense_claims**: List all employee expense claims and reimbursement requests
- **list_invoices**: List all invoices pending or processed
- **list_members**: List all team members with Spendesk access
- **list_payments**: List all payments in the Spendesk account
- **list_suppliers**: List all registered suppliers


## Installation & Usage

To install and use the **Spendesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spendesk](https://vinkius.com/mcp/spendesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
