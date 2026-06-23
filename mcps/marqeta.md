# Marqeta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marqeta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Issue cards, manage users, and process payments via Marqeta's modern card issuing platform.

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


## Available Tools (31)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marqeta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 users registered in my Marqeta environment."

**🤖 AI Agent:**
> I've retrieved the users. Here are the most recent 10 account holders, including 'John Doe' (Token: user_abc123) and 'Jane Smith' (Token: user_xyz789).

---

**👤 You:**
> "Issue a new virtual card for user token 'user_888' using card product 'prod_999'."

**🤖 AI Agent:**
> Processing card issuance... Success! A new virtual card has been created for user_888. The card token is 'card_555666' and it is currently active.

---

**👤 You:**
> "Fund $50.00 USD to user 'u_789' from funding source 'fs_000'."

**🤖 AI Agent:**
> Creating GPA order... The funding of $50.00 USD to user u_789 was successful. Order token: gpa_order_12345.


## ❓ FAQ

**Q: How can I see all cards belonging to a specific person?**
Use the `list_cards_by_user` tool by providing the user's unique token. The agent will return a list of all physical and virtual cards associated with that account holder.

**Q: How do I add money to a user's card account?**
You can use the `create_gpa_order` tool. You'll need the user token, the amount, currency code, and a funding source token to move funds into their General Purpose Account.

**Q: Is it possible to register a legal entity instead of an individual?**
Yes, use the `create_business` tool to create a business entity. You can then retrieve its details using the `get_business` tool with the business token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marqeta](https://vinkius.com/mcp/marqeta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marqeta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marqeta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marqeta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marqeta": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
