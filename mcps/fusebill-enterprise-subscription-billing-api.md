# Fusebill (Enterprise Subscription Billing API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fusebill-enterprise-subscription-billing-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Automate enterprise subscription billing via Fusebill — manage customers, track subscriptions, and handle billing lifecycles directly from any AI agent.

## Description
Connect your **Fusebill** enterprise account to any AI agent to streamline your subscription management and billing operations through natural conversation.

### What you can do

- **Customer Management** — List, retrieve, create, activate, or cancel customer records directly within your workflow
- **Subscription Tracking** — Query active or historical subscriptions to monitor recurring revenue and plan statuses
- **Detailed Metadata** — Fetch complete profiles for customers and subscriptions, including IDs, emails, and currency settings
- **Lifecycle Control** — Move customers through activation and cancellation phases without switching to the Fusebill dashboard

### How it works

1. Subscribe to this server
2. Enter your Fusebill API Key
3. Start managing your billing lifecycle from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance & Ops Teams** — quickly check customer statuses and manage subscription lifecycles without manual data entry
- **Developers** — integrate billing data into development workflows or verify customer records during testing
- **Customer Success** — instantly retrieve subscription details to provide better support to enterprise clients


## Available Tools (7)
- **get_subscription**: Get details for a specific Fusebill subscription
- **list_customers**: Supports pagination, filtering, and sorting.

List Fusebill customers
- **list_subscriptions**: Supports pagination, filtering, and sorting.

List Fusebill subscriptions
- **activate_customer**: Activate a Fusebill customer
- **cancel_customer**: Cancel a Fusebill customer
- **create_customer**: Create a new Fusebill customer
- **get_customer**: Get details for a specific Fusebill customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fusebill (Enterprise Subscription Billing API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Fusebill customers with the first name 'Jessica'."

**🤖 AI Agent:**
> I've searched your records. I found 2 customers matching 'Jessica': Jessica Jones (ID: 44556) and Jessica Smith (ID: 77889). Would you like to see the full details for either of them?

---

**👤 You:**
> "Get the details for subscription ID 987654."

**🤖 AI Agent:**
> Retrieving subscription 987654... This is an 'Active' subscription for 'Global Enterprise' plan, billing in USD. It is currently assigned to customer 'Tech Solutions Inc'.

---

**👤 You:**
> "Create a new customer: Michael Scott, email michael@dundermifflin.com, currency USD."

**🤖 AI Agent:**
> Processing... Customer 'Michael Scott' has been successfully created with ID 102938. The primary email is set to michael@dundermifflin.com and currency is USD. Would you like to activate this customer now?


## ❓ FAQ

**Q: Can I create a new customer directly through the AI?**
Yes! Use the `create_customer` tool by providing the first name, last name, and optional details like email and currency. The agent will confirm the creation and return the new Customer ID.

**Q: How do I check the status of a specific subscription?**
Simply provide the Subscription ID to the `get_subscription` tool. The agent will retrieve the full metadata, including its current status, plan details, and associated customer information.

**Q: Is it possible to cancel a customer's account using this integration?**
Yes, the `cancel_customer` tool allows you to change a customer's status to 'Cancelled' using their unique Customer ID. This action is performed securely through the Fusebill API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fusebill-enterprise-subscription-billing-api](https://vinkius.com/mcp/fusebill-enterprise-subscription-billing-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fusebill (Enterprise Subscription Billing API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fusebill-enterprise-subscription-billing-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fusebill (Enterprise Subscription Billing API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fusebill-enterprise-subscription-billing-api": {
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
