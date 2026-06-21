# Billsby MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/billsby)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage subscription billing via Billsby — list customers, subscriptions, and invoices directly from any AI agent.

## Description
Connect your **Billsby** account to any AI agent and orchestrate your subscription billing workflows through natural conversation.

### What you can do

- **Customer Management** — List, retrieve, and create customer profiles within your billing system.
- **Subscription Oversight** — Query and manage subscriptions, plans, and add-ons linked to your customers.
- **Invoicing Audits** — Access recent invoices and their payment statuses to ensure steady cash flow.
- **Product Catalog** — Retrieve available products and their pricing structures from Billsby.

### How it works

1. Subscribe to this server
2. Enter your Billsby API Key and your Company Domain
3. Start managing your subscriptions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders** — quickly check active subscriptions and customer statuses without logging into the dashboard.
- **Support Teams** — retrieve billing histories and active plans for users instantly.
- **Finance Operations** — audit invoices and product configurations using natural language.


## Available Tools (10)
- **create_customer**: Create a new customer
- **get_customer_subscriptions**: List subscriptions for a specific customer
- **get_customer**: Get specific customer details
- **get_subscription**: Get specific subscription details
- **list_addons**: List available add-ons
- **list_customers**: List all customers
- **list_invoices**: List recent invoices
- **list_plans**: List all subscription plans
- **list_products**: List all products
- **list_subscriptions**: List all subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Billsby** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active customers."

**🤖 AI Agent:**
> I've retrieved your customers. You have 3 recent users: 'John Doe' (ID: c_1), 'Jane Smith' (ID: c_2), and 'Alice Brown' (ID: c_3).

---

**👤 You:**
> "Show subscriptions for customer c_1."

**🤖 AI Agent:**
> Customer c_1 has one active subscription: 'Premium Plan' ($49/mo), which started on January 1st.

---

**👤 You:**
> "List all available subscription plans."

**🤖 AI Agent:**
> I've retrieved your plans. You have 3 active plans: 'Basic' ($10/mo), 'Pro' ($25/mo), and 'Enterprise' (Custom).


## ❓ FAQ

**Q: Can I check which subscription plan a customer is currently on?**
Yes! Use the `get_customer_subscriptions` tool with the Customer Unique ID. It will fetch all active and inactive plans for that user.

**Q: Does the integration allow me to cancel a subscription?**
Currently, the toolset focuses on querying and management functions (listing customers, checking invoices). Canceling or modifying subscription billing dates must be done on the Billsby platform.

**Q: Can I list all available subscription plans?**
Yes. Use the `list_plans` tool to retrieve all subscription plans configured in your Billsby account, including their pricing and cycles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/billsby](https://vinkius.com/mcp/billsby)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Billsby** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `billsby` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Billsby** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "billsby": {
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
