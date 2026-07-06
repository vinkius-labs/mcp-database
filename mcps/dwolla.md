# Dwolla MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dwolla)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate payments and bank transfers via Dwolla — manage customers, funding sources, and initiate transfers directly from any AI agent.

## Description
Connect your **Dwolla** account to any AI agent and take full control of your payment infrastructure through natural conversation.

### What you can do

- **Customer Management** — Create, list, and update individual or business customers directly from the chat
- **Funding Sources** — Link bank accounts or balances and manage them for specific customers or your main account
- **Transfer Orchestration** — Initiate and track transfers between funding sources with full visibility of the transaction lifecycle
- **Verification Workflows** — Handle micro-deposit verification to ensure secure bank account linking
- **Account Insights** — Retrieve organizational account details and funding source statuses instantly

### How it works

1. Subscribe to this server
2. Enter your Dwolla Access Token and Environment (sandbox or production)
3. Start managing your fintech operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — test payment flows and verify customer data without leaving the IDE
- **Operations Teams** — monitor transfer statuses and manage customer records through simple queries
- **Product Managers** — audit funding sources and account balances during development cycles


## Available Tools (30)
- **create_beneficial_owner**: Create a beneficial owner for a business customer
- **create_customer_funding_source**: Create a funding source for a customer
- **create_customer**: Create a new customer
- **create_document**: Create a document for a customer
- **create_funding_source**: Create a funding source
- **create_label**: Create a label for a customer
- **create_webhook_subscription**: Create a webhook subscription
- **get_account**: Retrieve Dwolla account details
- **get_customer**: Retrieve a customer
- **get_document**: Retrieve a document
- **get_event**: Retrieve an event
- **get_funding_source**: Retrieve a funding source
- **get_mass_payment**: Retrieve a mass payment
- **get_transfer**: Retrieve a transfer
- **initiate_kba**: Initiate a KBA session for a customer
- **initiate_mass_payment**: Initiate a mass payment
- **initiate_transfer**: Requires HAL _links in the payload.

Initiate a transfer
- **list_account_transfers**: List transfers for an account
- **list_beneficial_owners**: List beneficial owners for a customer
- **list_customers**: List or search customers
- **list_events**: List events
- **list_labels**: List labels for a customer
- **list_webhook_subscriptions**: List webhook subscriptions
- **retry_webhook**: Retry a webhook
- **update_customer**: Update a customer
- **update_funding_source**: g., passing { removed: true }).

Update or remove a funding source
- **verify_kba**: Verify KBA answers
- **verify_micro_deposits**: Verify micro-deposits for a funding source
- **list_account_funding_sources**: List funding sources for an account
- **cancel_transfer**: Cancel a pending transfer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dwolla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers in my Dwolla account."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 3 customers: Jane Doe (ID: cust-001), John Smith (ID: cust-002), and Acme Corp (ID: cust-003). Would you like to see details for one of them?

---

**👤 You:**
> "Get details for customer ID cust-001."

**🤖 AI Agent:**
> Fetching details for Jane Doe (cust-001)... She is a 'verified' personal customer with email jane@example.com. Her account was created on 2023-10-15.

---

**👤 You:**
> "Initiate a transfer of $50 between source 'src-123' and destination 'dest-456'."

**🤖 AI Agent:**
> Transfer initiated successfully. The transaction ID is 'trans-789'. The status is currently 'pending'.


## ❓ FAQ

**Q: How do I verify a bank account using micro-deposits?**
Use the `verify_micro_deposits` tool by providing the Funding Source ID and the two deposit amounts. This ensures the bank account is active and owned by the customer.

**Q: Can I create a new customer directly through the AI?**
Yes! Use the `create_customer` tool with a JSON payload containing the customer's details like firstName, lastName, and email.

**Q: How can I see the history of transfers for my organization?**
You can use the `list_account_transfers` tool with your Account ID to retrieve all recent and past fund movements associated with your Dwolla account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dwolla](https://vinkius.com/mcp/dwolla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dwolla** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dwolla` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dwolla** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dwolla": {
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
