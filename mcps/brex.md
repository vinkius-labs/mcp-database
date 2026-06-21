# Brex MCP Server

Equip your AI to navigate your Brex suite. Spin up virtual cards, route new team members, and check daily cash allocations through natural chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/brex)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
The **Brex MCP Server** bridges standard large language models directly via the `platform.brexapis.com` to your startup's core spend engine. By delivering a single static User Token, you enable the most flexible financial assistant available.

### What you can do

- **Agile Employee Onboarding** — `brex_create_user` directly provisions employees with their associated hierarchical structure. Follow it up with `brex_create_card` to hand them digital spend capacity securely limited.
- **Accounting Snapshots** — You don't need to load the Brex dash to trace down runaway expenses. Trigger `brex_list_transactions` to pull highly contextualized raw CSV data into your AI workspace.
- **Accounts Payable Controls** — Draft and approve external entity vendors via `brex_create_vendor` and initiate routing payments `brex_pay_vendor` seamlessly, letting internal routing protocols map out the wires.

### How it works

1. In your Brex settings, you can generate an immediate `User Token` (typically starting with `user_token_`).
2. This token natively identifies you and limits AI actions safely within your existing managerial permissions level.
3. Drop this into your client credentials and authorize AI access.

### Who is this for?

- **Forward-Thinking CFOs / FinOps** — Handle your routine accounting actions strictly through language.
- **Startups Scaling** — Automatically loop AI agents to handle corporate card provisioning to cloud instances without manual checks.


## Available Tools
- **brex_create_card**: Useful for giving employees isolated cards for SaaS subscriptions.

Issue a dynamic Virtual Corporate Card
- **brex_create_user**: You must provide a valid email, first name, and last name.

Invite a new employee / user to Brex
- **brex_create_vendor**: Create a Vendor in AP (Accounts Payable)
- **brex_get_balance**: Get main cash balance of the Brex Cash accounts
- **brex_list_budgets**: List budget programs assigned to teams
- **brex_list_cards**: List all issued cards across the company
- **brex_list_transactions**: Sweep historical Brex card and account transactions
- **brex_list_users**: List all users in the Brex company account
- **brex_list_vendors**: List saved Vendors inside Brex AP
- **brex_pay_vendor**: Orchestrate a vendor payment (Send Money)


## Installation & Usage

To install and use the **Brex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brex](https://vinkius.com/mcp/brex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
