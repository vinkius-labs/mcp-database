# Recurly MCP Server

Equip your AI to directly manage subscriptions, billing accounts, and invoices within your Recurly ecosystem without shifting interfaces.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/recurly)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your **Recurly** subscription billing and management platform securely to your conversational AI agent. Activating this integration transforms your AI into a dynamic revenue operations assistant, giving it the autonomy to look up accounts, adjust active subscription states, and analyze invoice pipelines directly from the terminal.

### What you can do

- **Account Management** — Quickly list your customer directory, view detailed billing profiles, or instantly create a new account mapping without opening the vendor console.
- **Subscription Operations** — Easily search and read subscription lifecycle states, enroll users in fresh catalog plans, un-cancel previous subscriptions, or permanently cancel an ongoing billing mandate.
- **Invoice & Plan Catalogs** — Retrieve the list of historical generated invoices to verify successful automated payments or pull all active billing models (Catalog Plans) to review available products.

### How it works

1. Add the Recurly MCP server to your authorized module list.
2. Configure the server using your specific Recurly subdomain alongside your Private API Key.
3. Chat seamlessly with your AI to process operations like revoking a subscription instance or querying for a customer's missing invoice.

### Who is this for?

- **RevOps & Finance Teams** — Pull billing analytics, track active subscription statuses, and instantly generate plan insights via conversational commands during reviews.
- **Customer Support Agents** — Quickly verify if an account holds a successful invoice payment or pause/cancel client subscriptions mid-chat without escalating to billing engineers.
- **Software Developers** — Interact safely with Recurly limits, list the ID structures of catalog plans, and test provisioning logic endpoints directly from the code editor.


## Available Tools
- **cancel_subscription**: This action is irreversible.

Cancels an active subscription
- **create_account**: Specify code, email, and name.

Creates a new customer account
- **create_subscription**: Creates a new subscription for an account
- **get_account_details**: Retrieves details for a specific customer account
- **get_subscription_details**: Retrieves details for a specific subscription
- **list_accounts**: Lists all customer accounts in Recurly
- **list_catalog_plans**: Lists all available subscription plans in the product catalog
- **list_invoices**: Lists all generated invoices
- **list_subscriptions**: Lists all subscriptions managed by Recurly
- **reactivate_subscription**: Reactivates a previously cancelled or expired subscription


## Installation & Usage

To install and use the **Recurly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recurly](https://vinkius.com/mcp/recurly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
