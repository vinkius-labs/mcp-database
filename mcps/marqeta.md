# Marqeta MCP Server

Issue cards, manage users, and process payments via Marqeta's modern card issuing platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/marqeta)

## Overview
**Category:** money-moves
**Tools Count:** 31

## Description
Connect your **Marqeta** account to any AI agent to manage your card issuing infrastructure through natural conversation. This server provides comprehensive tools for managing the entire lifecycle of card programs.

### What you can do

- **User & Business Management** — Create and retrieve individual users or business entities to act as account holders.
- **Card Issuance** — Create physical or virtual payment cards and manage card products that define spending behaviors.
- **Funding & GPA Orders** — Move funds into account holder General Purpose Accounts (GPA) and manage ACH funding sources.
- **Inventory & Retrieval** — List users, fetch specific card details, and audit all cards associated with a specific user token.
- **Configuration** — Define card products with specific start dates and names to control your issuing environment.

### How it works

1. Subscribe to this server
2. Enter your Marqeta Application Token and Admin Access Token
3. Provide your Base URL (Sandbox or Production)
4. Start issuing cards and managing fintech workflows from your MCP-compatible client


## Available Tools
- **create_ach_funding_source**: Create an ACH funding source
- **create_auth_control**: Create an authorization control
- **create_business**: Create a new Marqeta business
- **create_card_product**: Create a new Marqeta card product
- **create_card**: Create a new Marqeta card
- **create_card_transition**: g., ACTIVE, SUSPENDED, TERMINATED).

Create a card transition
- **create_direct_deposit_transition**: g., to reverse a deposit).

Create a direct deposit transition
- **create_gpa_order**: Create a GPA order to fund an account
- **create_payment_card_funding_source**: Create a payment card funding source
- **create_pin_control_token**: Create a PIN control token
- **create_program_funding_source**: Create a program funding source
- **create_user**: Create a new Marqeta user
- **create_user_transition**: g., ACTIVE, SUSPENDED, CLOSED).

Create a user transition
- **create_velocity_control**: Create a velocity control
- **create_webhook**: Create a webhook
- **get_balances**: Retrieve balances for a user or business
- **get_business**: Retrieve a Marqeta business by token
- **get_card**: Retrieve a Marqeta card by token
- **get_direct_deposit**: Retrieve a direct deposit record
- **get_user**: Retrieve a Marqeta user by token
- **list_cards_by_user**: List all cards for a specific user
- **list_users**: List Marqeta users
- **perform_kyc**: Perform KYC verification for a user
- **ping_webhook**: Ping a webhook
- **provision_apple_pay**: Provision a card for Apple Pay
- **provision_google_pay**: Provision a card for Google Pay
- **reveal_pin**: Reveal a card PIN
- **simulate_authorization**: Simulate an authorization
- **simulate_clearing**: Simulate a clearing transaction
- **simulate_reversal**: Simulate a reversal
- **update_pin**: Set or update a card PIN


## Installation & Usage

To install and use the **Marqeta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marqeta](https://vinkius.com/mcp/marqeta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
